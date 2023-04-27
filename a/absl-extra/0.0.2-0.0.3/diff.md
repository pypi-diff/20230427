# Comparing `tmp/absl_extra-0.0.2.tar.gz` & `tmp/absl_extra-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.tar", last modified: Thu Apr 13 20:48:33 2023, max compression
+gzip compressed data, was "absl_extra-0.0.3.tar", last modified: Thu Apr 27 21:47:47 2023, max compression
```

## Comparing `absl_extra-0.0.2.tar` & `absl_extra-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1185 2023-04-13 20:48:25.615127 absl_extra-0.0.2/Readme.md
--rw-r--r--   0        0        0     4664 2023-04-13 20:48:25.615127 absl_extra-0.0.2/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-13 20:48:25.615127 absl_extra-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 absl_extra-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1271 2023-04-27 21:47:38.824325 absl_extra-0.0.3/Readme.md
+-rw-r--r--   0        0        0     4741 2023-04-27 21:47:38.824325 absl_extra-0.0.3/absl_extra.py
+-rw-r--r--   0        0        0     6066 2023-04-27 21:47:38.824325 absl_extra-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 absl_extra-0.0.3/PKG-INFO
```

### Comparing `absl_extra-0.0.2/Readme.md` & `absl_extra-0.0.3/Readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,32 +2,40 @@
 
 A collection of utils I commonly use for running my experiments.
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
-- Inject `ml_collections.ConfigDict` from `config_file`, if kwargs provided.
-- Inject `pymongo.collection.Collection` if `mongo_config` kwargs provided.
+- Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
+- Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
 
 Minimal example
 ```python
-from os import environ
+import os
+import functools
 from pymongo.collection import Collection
-from absl import flags
+from absl import flags, app
 from ml_collections import ConfigDict
-from absl_extra import App, SlackNotifier, MongoConfig
+from absl_extra import hook_main, SlackNotifier, MongoConfig
 
 
 FLAGS = flags.FLAGS
 flags.DEFINE_integer("some_flag", default=4, help=None)
 
-def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
+@functools.partial(
+    hook_main,
+    app_name="some_name",
+    config_file="config.py",
+    mongo_config=MongoConfig(
+        uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+    ),
+    notifier=SlackNotifier(
+        slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+    ),
+)
+def main(cmd: str, config: ConfigDict, db: Collection) -> None:
+    pass
 
 if __name__ == "__main__":
-    app = App(
-        notifier=SlackNotifier(slack_token=environ["SLACK_TOKEN"], channel_id=environ["CHANNEL_ID"]),
-        config_file="config.py",
-        mongo_config=MongoConfig(uri=environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
-   )
     app.run(main)
 ```
```

### Comparing `absl_extra-0.0.2/absl_extra.py` & `absl_extra-0.0.3/absl_extra.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
 import json
 from importlib import util
 from typing import Callable, NamedTuple
-from functools import partial
-
-
+from functools import partial, wraps
 from absl import app, flags, logging
 
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
+else:
+    logging.warning("pymongo not installed.")
 
 
 if util.find_spec("ml_collections"):
     from ml_collections import config_flags
+else:
+    logging.warning("ml_collections not installed")
 
 
 class MongoConfig(NamedTuple):
     uri: str
     db_name: str
-    collection: str
+    collection: str | None = None
 
 
 class Notifier:
     def notify_job_started(self, cmd: str):
         logging.info(f"Job {cmd} started.")
 
     def notify_job_finished(self, cmd: str):
@@ -87,66 +89,70 @@
                         },
                     }
                 ],
                 text="Job Finished!",
             )
             raise ex
 
+else:
+    logging.warning("slack_sdk not installed.")
+
 
 class ExceptionHandlerImpl(app.ExceptionHandler):
     def __init__(self, cmd: str, notifier: Notifier):
         self.cmd = cmd
         self.notifier = notifier
 
     def handle(self, exc: Exception):
         self.notifier.notify_job_failed(self.cmd, exc)
 
 
-class App:
-    def __init__(
-        self,
-        *,
-        app_name: str | None = None,
-        notifier: Notifier | None = None,
-        config_file: str | None = None,
-        mongo_config: MongoConfig | None = None,
-    ):
-        if app_name is not None:
-            self.app_name = app_name
-        if notifier is None:
-            notifier = Notifier()
-        self.notifier = notifier
-        if config_file is not None:
-            self.config = config_flags.DEFINE_config_file("config")
-        if mongo_config is not None:
-            self.db = (
-                MongoClient(mongo_config.uri)
-                .get_database(mongo_config.db_name)
-                .get_collection(mongo_config.collection)
-            )
-
-    def run(self, main: Callable):
-        if hasattr(self, "app_name"):
-            app_name = self.app_name
+def hook_main(
+    main: Callable,
+    app_name: str | None = None,
+    notifier: Notifier | None = None,
+    config_file: str | None = None,
+    mongo_config: MongoConfig | None = None,
+):
+    if notifier is None:
+        notifier = Notifier()
+    if util.find_spec("ml_collections") and config_file is not None:
+        config = config_flags.DEFINE_config_file("config")
+    else:
+        config = None
+    if util.find_spec("pymongo") and mongo_config is not None:
+        db = MongoClient(mongo_config.uri).get_database(mongo_config.db_name)
+        if mongo_config.collection is not None:
+            db = db.get_collection(mongo_config.collection)
+    else:
+        db = None
+
+    @wraps(main)
+    def wrapper(cmd: str):
+        if app_name is None:
+            _app_name = cmd
         else:
-            app_name = "app"
-        ex_handler = ExceptionHandlerImpl(app_name, self.notifier)
-        app.install_exception_handler(ex_handler)
+            _app_name = app_name
+
+        app.install_exception_handler(ExceptionHandlerImpl(cmd, notifier))
+
         kwargs = {}
-        if hasattr(self, "config"):
+        if config is not None:
             logging.info(
-                f"Config: {json.dumps(self.config.value, sort_keys=True, indent=4)}"
+                f"Config: {json.dumps(config.value, sort_keys=True, indent=4)}"
             )
             logging.info("-" * 50)
-            kwargs["config"] = self.config.value
-        if hasattr(self, "db"):
-            kwargs["db"] = self.db
+            kwargs["config"] = config.value
+        if db is not None:
+            kwargs["db"] = db
 
         logging.info("-" * 50)
         logging.info(
             f"Flags: {json.dumps(flags.FLAGS.flag_values_dict(), sort_keys=True, indent=4)}"
         )
         logging.info("-" * 50)
 
-        self.notifier.notify_job_started(app_name)
+        notifier.notify_job_started(app_name)
         app.run(partial(main, **kwargs))
-        self.notifier.notify_job_finished(app_name)
+        notifier.notify_job_finished(app_name)
+
+    return wrapper
```

### Comparing `absl_extra-0.0.2/pyproject.toml` & `absl_extra-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "absl_extra"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.2"  # Required
+version = "0.0.3"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A wrapper to run and monitor absl app."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `absl_extra-0.0.2/PKG-INFO` & `absl_extra-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper to run and monitor absl app.
 Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -24,33 +24,41 @@
 
 A collection of utils I commonly use for running my experiments.
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
-- Inject `ml_collections.ConfigDict` from `config_file`, if kwargs provided.
-- Inject `pymongo.collection.Collection` if `mongo_config` kwargs provided.
+- Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
+- Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
 
 Minimal example
 ```python
-from os import environ
+import os
+import functools
 from pymongo.collection import Collection
-from absl import flags
+from absl import flags, app
 from ml_collections import ConfigDict
-from absl_extra import App, SlackNotifier, MongoConfig
+from absl_extra import hook_main, SlackNotifier, MongoConfig
 
 
 FLAGS = flags.FLAGS
 flags.DEFINE_integer("some_flag", default=4, help=None)
 
-def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
+@functools.partial(
+    hook_main,
+    app_name="some_name",
+    config_file="config.py",
+    mongo_config=MongoConfig(
+        uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+    ),
+    notifier=SlackNotifier(
+        slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+    ),
+)
+def main(cmd: str, config: ConfigDict, db: Collection) -> None:
+    pass
 
 if __name__ == "__main__":
-    app = App(
-        notifier=SlackNotifier(slack_token=environ["SLACK_TOKEN"], channel_id=environ["CHANNEL_ID"]),
-        config_file="config.py",
-        mongo_config=MongoConfig(uri=environ["MONGO_URI"], db_name="my_project", collection="experiment_1"),
-   )
     app.run(main)
 ```
```

