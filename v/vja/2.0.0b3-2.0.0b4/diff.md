# Comparing `tmp/vja-2.0.0b3.tar.gz` & `tmp/vja-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0b3.tar", last modified: Mon Apr 10 07:45:01 2023, max compression
+gzip compressed data, was "vja-2.0.0b4.tar", last modified: Mon Apr 24 08:34:51 2023, max compression
```

## Comparing `vja-2.0.0b3.tar` & `vja-2.0.0b4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.706604 vja-2.0.0b3/
--rw-r--r--   0 root         (0) root         (0)     8295 2023-04-10 07:45:01.706604 vja-2.0.0b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-10 07:45:01.707604 vja-2.0.0b3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-10 07:43:50.000000 vja-2.0.0b3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.702604 vja-2.0.0b3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)     9497 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-10 07:43:50.000000 vja-2.0.0b3/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.705604 vja-2.0.0b3/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6802 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17567 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/list_service.py
--rwxrwxrwx   0 root         (0) root         (0)     6008 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3289 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)    10031 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-04-10 07:43:50.000000 vja-2.0.0b3/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:45:01.706604 vja-2.0.0b3/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8295 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-10 07:45:01.000000 vja-2.0.0b3/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.204191 vja-2.0.0b4/
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-04-24 08:34:51.204191 vja-2.0.0b4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-24 08:34:51.204191 vja-2.0.0b4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-24 08:33:47.000000 vja-2.0.0b4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.200190 vja-2.0.0b4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10091 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.203191 vja-2.0.0b4/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6802 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17734 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/list_service.py
+-rwxrwxrwx   0 root         (0) root         (0)     6008 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)    10333 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.204191 vja-2.0.0b4/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0b3/PKG-INFO` & `vja-2.0.0b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
@@ -41,14 +41,17 @@
           ```
           (If you cloned from git, you may copy the folder .vjacli to your `$HOME` directory instead.)
         - Adjust to your needs.
           `frontend_url` and `api_url` must point to your own Vikunja server.
           Especially, the api_url must be reachable from your client. This can be verified, for example
           by `curl https://mydomain.com/api/v1/info`
         
+        You may change the location of the configuration directory with an environment variable
+        like `VJA_CONFIGDIR=/not/my/home`
+        
         ### Description of configuration
         
         #### Required options
         
         | Section       | Option       | Description                                                 |
         |---------------|--------------|-------------------------------------------------------------|
         | [application] | api_url      | The service instance of Vikunja to which vja should connect |
```

### Comparing `vja-2.0.0b3/setup.py` & `vja-2.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/tests/conftest.py` & `vja-2.0.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/tests/test_basic.py` & `vja-2.0.0b4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/tests/test_command.py` & `vja-2.0.0b4/tests/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,28 @@
 class TestCloneTask:
     def test_clone_task(self, runner):
         before = json_for_task_id(runner, 1)
         res = invoke(runner, 'clone 1 title of new task cloned from 1')
         after = json_for_created_task(runner, res.output)
         assert after['project'] == before['project']
         assert after['due_date'] == before['due_date']
+        assert after['labels'] == before['labels']
         assert after['title'] != before['title']
         assert after['id'] != before['id']
         assert after['created'] != before['created']
+        assert after['position'] != before['position']
+        assert after['kanban_position'] != before['kanban_position']
+#        assert after['bucket_id'] != before['bucket_id'] # TODO: Need to create a second bucket to test this
+
+
+    def test_clone_task_keeping_bucket(self, runner):
+        before = json_for_task_id(runner, 1)
+        res = invoke(runner, 'clone 1 --bucket title of new task with labels cloned from 1')
+        after = json_for_created_task(runner, res.output)
+        assert after['bucket_id'] == before['bucket_id']
 
 
 class TestEditGeneral:
     def test_edit_title(self, runner):
         before = json_for_task_id(runner, 1)
         new_title = f'{before["title"]}42'
         res = runner.invoke(cli, ['edit', '1', '-i', f'{new_title}'])
```

### Comparing `vja-2.0.0b3/tests/test_query.py` & `vja-2.0.0b4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/apiclient.py` & `vja-2.0.0b4/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/authenticate.py` & `vja-2.0.0b4/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/cli.py` & `vja-2.0.0b4/vja/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,18 +218,20 @@
     ctx.invoke(task_show, tasks=[task.id])
 
 
 @cli.command('clone', aliases=['copy'],
              help='Clone task with given task_id. Set the new title')
 @click.argument('task_id', required=True, type=click.INT)
 @click.argument('title', required=True, nargs=-1)
+@click.option('is_clone_bucket', '-b', '--bucket', is_flag=True,
+              help='Clone kanban bucket too. Default: False')
 @with_application
 @click.pass_context
-def task_clone(ctx, application, task_id, title):
-    task = application.command_service.clone_task(task_id, " ".join(title))
+def task_clone(ctx, application, task_id, title, is_clone_bucket=False):
+    task = application.command_service.clone_task(task_id, " ".join(title), is_clone_bucket)
     click.echo(f'Created task {task.id} in project {task.project.id} as clone from {task_id}')
     ctx.invoke(task_show, tasks=[task.id])
 
 
 @cli.command('edit', aliases=['modify', 'update'],
              help='Modify task/tasks. (Opens task in browser if no options are given)')
 @click.argument('task_ids', required=True, type=click.INT, nargs=-1)
```

### Comparing `vja-2.0.0b3/vja/config.py` & `vja-2.0.0b4/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/filter.py` & `vja-2.0.0b4/vja/filter.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/list_service.py` & `vja-2.0.0b4/vja/list_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/model.py` & `vja-2.0.0b4/vja/model.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/output.py` & `vja-2.0.0b4/vja/output.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/parse.py` & `vja-2.0.0b4/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/service_command.py` & `vja-2.0.0b4/vja/service_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,25 +81,31 @@
         task = self._task_service.task_from_json(task_json)
 
         label = self._label_from_name(tag_name, is_force) if tag_name else None
         if label:
             self._api_client.add_label_to_task(task.id, label.id)
         return task
 
-    def clone_task(self, task_id: int, title):
+    def clone_task(self, task_id: int, title, is_clone_bucket):
         task_remote = self._api_client.get_task(task_id)
         task_remote.update({'id': None})
         task_remote.update({'title': title})
+        task_remote.update({'position': 0})
+        task_remote.update({'kanban_position': 0})
+        if is_clone_bucket:
+            task_remote.update({'bucket_id': 0})
 
         # make sure we do not send back the old reminder_dates
         task_remote.pop("reminder_dates", None)
         logger.debug('put task: %s', task_remote)
         task_json = self._api_client.put_task(task_remote['project_id'], task_remote)
         task = self._task_service.task_from_json(task_json)
 
+        for label in task_remote['labels']:
+            self._api_client.add_label_to_task(task.id, label['id'])
         return task
 
     def edit_task(self, task_id: int, args: dict):
         task_remote = self._api_client.get_task(task_id)
         tag_name = args.pop('tag') if args.get('tag') else None
         is_force = args.pop('force_create') if args.get('force_create') is not None else False
```

### Comparing `vja-2.0.0b3/vja/service_query.py` & `vja-2.0.0b4/vja/service_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/task_service.py` & `vja-2.0.0b4/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja/urgency.py` & `vja-2.0.0b4/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b3/vja.egg-info/PKG-INFO` & `vja-2.0.0b4/vja.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
@@ -41,14 +41,17 @@
           ```
           (If you cloned from git, you may copy the folder .vjacli to your `$HOME` directory instead.)
         - Adjust to your needs.
           `frontend_url` and `api_url` must point to your own Vikunja server.
           Especially, the api_url must be reachable from your client. This can be verified, for example
           by `curl https://mydomain.com/api/v1/info`
         
+        You may change the location of the configuration directory with an environment variable
+        like `VJA_CONFIGDIR=/not/my/home`
+        
         ### Description of configuration
         
         #### Required options
         
         | Section       | Option       | Description                                                 |
         |---------------|--------------|-------------------------------------------------------------|
         | [application] | api_url      | The service instance of Vikunja to which vja should connect |
```

