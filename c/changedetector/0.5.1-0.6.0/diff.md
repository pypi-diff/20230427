# Comparing `tmp/changedetector-0.5.1.tar.gz` & `tmp/changedetector-0.6.0.tar.gz`

## Comparing `changedetector-0.5.1.tar` & `changedetector-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/GLOBALS.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/__init__.py
--rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/detectchange.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/menu.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/versionControl.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/wrapperComponents.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/wro.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/wrs.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/wtch.py
--rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/scripts/detectchange.fish
--rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/scripts/detectchange.sh
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/TEST.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/attrDatas.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/requirements.txt
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/test.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/testfile.c
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/testfile.cpp
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/testfile.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/testfile.rb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/tests/testfile.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 changedetector-0.5.1/changedetector/themes/inquirer.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 changedetector-0.5.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.5.1/LICENCE
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 changedetector-0.5.1/README.md
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 changedetector-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 changedetector-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/GLOBALS.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/__init__.py
+-rw-r--r--   0        0        0    16477 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/detectchange.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/makeParser.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/menu.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/versionControl.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/wrapperComponents.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/wrm.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/wro.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/wrs.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/wtch.py
+-rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/scripts/detectchange.fish
+-rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/scripts/detectchange.sh
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/TEST.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/attrDatas.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/requirements.txt
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/test.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/testfile.c
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/testfile.cpp
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/testfile.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/testfile.rb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 changedetector-0.6.0/changedetector/tests/testfile.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 changedetector-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.0/LICENCE
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.0/README.md
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 changedetector-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 changedetector-0.6.0/PKG-INFO
```

### Comparing `changedetector-0.5.1/changedetector/__init__.py` & `changedetector-0.6.0/changedetector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "changedetector"
 __author__ = "LuxLuth"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 LuxLuth"
-__version__ = "0.5.1"
+__version__ = "0.6.0"
```

### Comparing `changedetector-0.5.1/changedetector/detectchange.py` & `changedetector-0.6.0/changedetector/detectchange.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import time
 import os
-import pathlib
 import sys
 from rich import print as rprint
 from rich.console import Console
 import typer
 
 from watchdog.observers import Observer
 from pyfiglet import Figlet
 
 # add the base directory to the path
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 from menu import menu
 from wrapperComponents import WrapperComponents as wp
+from makeParser import Parser
 
 # handlers
 from wrs import WrsHandler
 from wro import WroHandler
 from wtch import WatchForHandler
+from wrm import WrmHandler
 
 # Version Control
 from versionControl import VersionControl
 from GLOBALS import VARS as v
+import tomli
 
 
 class Entries:
     def __init__(self):
         self.entries = {}
         self.c = Console()
 
     def add(self, name: str, value):
         self.entries[name] = value
 
     def get(self, name: str) -> str | list | None | bool | int | list[str]:
-        return self.entries[name]
+        return self.entries.get(name, None)
 
     def makeMode(self):
         MODE = menu(
             "Choose the mode you want to use:",
             "select",
-            [("Watch and Run Self (WRS)", "wrs"), ("Watch and Run Other (WRO)", "wro")],
+            [("Watch and Run Self (WRS)", "wrs"), ("Watch and Run Other (WRO)", "wro"), ("Makefile", "mk")],
         )
         self.add("mode", MODE)
 
     def makeLang(self):
         self.language = menu(
             "Choose the language you want to use:",
             "select",
@@ -93,119 +95,161 @@
         except KeyboardInterrupt:
             rprint(
                 f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('KeyboardInterrupt')}"
             )
             sys.exit(1)
 
     def makePaths(self):
-        # Automatic detection of the working directory
-        BASE_DIR = pathlib.Path(__file__).parent.absolute().cwd()
+        BASE_DIR = os.getcwd()
         self.add("base_dir", BASE_DIR)
         try:
-            if self.get("lang") == "python":
-                # print(python_files)
-                FILE = menu("Choose the file you want to run:", "file")
-            elif self.get("lang") == "ruby":
-                # print(ruby_files)
-                FILE = menu("Choose the file you want to run:", "file")
-
-            elif self.get("lang") == "c":
-                FILE = menu("Choose the file you want to run:", "file")
-
-            elif self.get("lang") == "c++":
-                # print(cpp_files)
-                FILE = menu("Choose the file you want to run:", "file")
+            if self.get("mode") != "mk":
+                if self.get("lang") == "python":
+                    # print(python_files)
+                    FILE = menu("Choose the file you want to run:", "file")
+                elif self.get("lang") == "ruby":
+                    # print(ruby_files)
+                    FILE = menu("Choose the file you want to run:", "file")
+
+                elif self.get("lang") == "c":
+                    FILE = menu("Choose the file you want to run:", "file")
+
+                elif self.get("lang") == "c++":
+                    # print(cpp_files)
+                    FILE = menu("Choose the file you want to run:", "file")
+
+                if self.get("mode") == "wro":
+                    # print(all_files)
+                    FILE_TO_WATCH = menu("Choose the file you want to watch:", "file")
+            else:
+                p = Parser()
+                cmds = p.parse()
+                if len(cmds) == 0:
+                    rprint(
+                        f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('No make command found')}"
+                    )
+                    sys.exit(1)
+                choices = [(c, c) for c in cmds]
+                MK_TO_RUN = menu("Choose the make command to run:", "select", choices)
+                self.add("mk_cmd", MK_TO_RUN)
 
-            if self.get("mode") == "wro":
-                # print(all_files)
                 FILE_TO_WATCH = menu("Choose the file you want to watch:", "file")
 
+                # sys.exit(0)
+
         except KeyboardInterrupt:
             rprint(
                 f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('KeyboardInterrupt')}"
             )
             sys.exit(1)
-        THE_FILE = os.path.join(self.get("base_dir"), f"{FILE}")
-        self.add("the_file", THE_FILE)
-        if self.get("mode") == "wro":
+        if self.get("mode") != "mk":
+            THE_FILE = os.path.join(self.get("base_dir"), f"{FILE}")
+            self.add("the_file", THE_FILE)
+        if self.get("mode") in ["wro", "mk"]:
             THE_FILE_TO_WATCH = os.path.join(self.get("base_dir"), f"{FILE_TO_WATCH}")
             self.add("the_file_to_watch", THE_FILE_TO_WATCH)
-        rprint(self.get("the_file"))
+        if self.get("mode") != "mk":
+            rprint(self.get("the_file"))
         # Check if the file's path is valid exist
-        if not os.path.exists(THE_FILE):
-            err = wp.textWrapBold(f"The file {THE_FILE} doesn't exist", "red")
-            rprint(f"❌ {err}")
-            sys.exit(1)
+        if self.get("mode") != "mk":
+            if not os.path.exists(THE_FILE):
+                err = wp.textWrapBold(f"The file {THE_FILE} doesn't exist", "red")
+                rprint(f"❌ {err}")
+                sys.exit(1)
 
         # Check if the file's path to watch is valid exist
-        if self.get("mode") == "wro" and not os.path.exists(THE_FILE_TO_WATCH):
+        if self.get("mode") in ["wro", "mk"] and not os.path.exists(THE_FILE_TO_WATCH):
             err = wp.textWrapBold(
                 f"The file {THE_FILE_TO_WATCH} doesn'tOUTPUT_FILE exist", "red"
             )
             rprint(f"❌ {err}")
             sys.exit(1)
 
+        self.make_command_list()
+
+    def make_command_list(self):
         if self.get("lang") in ["c++", "c"]:
             COMMAND_LIST = [self.get("cmd")]
             if self.get("flags")[0] != "":
                 COMMAND_LIST.extend(iter(self.get("flags")))
             COMMAND_LIST.append(self.get("the_file"))
             COMMAND_LIST.append(self.get("output_attr"))
             COMMAND_LIST.append(self.get("output_file"))
             self.add("command_list", COMMAND_LIST)
+        elif self.get("mode") == "mk":
+            COMMAND_LIST = ["make", self.get("mk_cmd")]
+            self.add("command_list", COMMAND_LIST)
         else:
             self.add("command_list", None)
 
     def make(self):
         self.makeMode()
-        self.makeLang()
-        self.makeCommand()
-        self.makePaths()
+        if self.get("mode") != "mk":
+            self.makeLang()
+            self.makeCommand()
+            self.makePaths()
+        else:
+            self.makePaths()
 
     def __str__(self):
         return str(self.entries)
 
     def __repr__(self):
         return str(self.entries)
 
 
 class BeautifulOutput:
     def __init__(self, e: Entries = None) -> None:
         self.lang = e.get("lang") if e else None
+        self.mode = e.get("mode") if e else None
         self.the_file = e.get("the_file") if e else None
+        self.the_file_to_watch = e.get("the_file_to_watch") if e else None
+
 
     def _start(self):
         os.system("cls" if os.name == "nt" else "clear")
         f = Figlet(font="colossal", width=80)
         print(f.renderText("Change"))
         print(f.renderText("Detect"))
 
     def _out(self, lang: str):
         if v.verbose:
             custom_fig = Figlet(font="colossal")
             print(custom_fig.renderText(lang))
-            rprint(
-                f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
-            )
+            if self.mode != "mk":
+                rprint(
+                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
+                )
+            else:
+                rprint(
+                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file_to_watch)}"
+                )
         else:
-            rprint(
-                f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
-            )
+            if self.mode != "mk":
+                rprint(
+                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
+                )
+            else:
+                rprint(
+                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file_to_watch)}"
+                )
 
     def _run(self):
         # clear the terminal
         os.system("cls" if os.name == "nt" else "clear")
         if self.lang in ["ruby", "rb"]:
             self._out("Ruby")
         elif self.lang in ["python", "py", "python3"]:
             self._out("Python")
         elif self.lang in ["c++", "cpp"]:
             self._out("C++")
         elif self.lang == "c":
             self._out("C")
+        elif self.mode == "mk":
+            self._out("Makefile")
 
     def __str__(self):
         return f"BeautifulOutput({self.lang}, {self.the_file})"
 
 
 class _Watcher:
     def __init__(self, handler_type: WrsHandler, dir_to_watch: str = os.getcwd()):
@@ -260,37 +304,135 @@
                 command_list=e.get("command_list"),
                 language=e.get("lang"),
                 base_dir=e.get("base_dir"),
                 cmd=e.get("cmd"),
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRS)", "green")
-        else:
+        elif e.get("mode") == "wro":
             wh = WroHandler(
                 the_file=e.get("the_file"),
                 the_file_to_watch=e.get("the_file_to_watch"),
                 command_list=e.get("command_list"),
                 language=e.get("lang"),
                 base_dir=e.get("base_dir"),
                 cmd=e.get("cmd"),
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRO)", "green")
+        else:
+            wh = WrmHandler(
+                the_file_to_watch=e.get("the_file_to_watch"),
+                command_list=e.get("command_list")
+            )
+            BeautifulOutput(e)._run()
+            mode = wp.textWrapBold("(MAKEFILE)", "green")
+
         w = _Watcher(wh, e.get("base_dir"))
         print(" ")
         rprint(f"Watching in {mode} mode...")
         print(" ")
         w.run()
     except KeyboardInterrupt:
         # pipe the error number to the shell
         rprint(
             f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('Keyboard Interrupt')}"
         )
         sys.exit(0)
 
+def make_path(base_dir: str, file: str) -> str:
+    if file == None:
+        return None
+    if file.startswith(f".{os.sep}"):
+        file = file[2:]
+    return os.path.join(base_dir, file)
+
+def cfg_activate() -> None:
+    """
+    CFG ACTIVATE
+    ------------
+    SAME AS ACTIVATE BUT IT READS THE CONFIG FILE (.detectchange) => a toml file
+    """
+    base_dir = os.getcwd()
+    config_file = os.path.join(base_dir, ".detectchange")
+    if not os.path.exists(config_file):
+        rprint(
+            f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('No config file found')}"
+        )
+        sys.exit(1)
+    with open(".detectchange", "rb") as f:
+        config = tomli.load(f)
+
+    mode = config.get("mode", "wrs")
+    lang = config.get("lang", "python")
+    the_file = make_path(os.getcwd(), config.get("file", "main.py"))
+    the_file_to_watch = make_path(os.getcwd(), config.get("file_to_watch", None))
+    verbose = config.get("verbose", False)
+    if lang in ["python", "py", "python3"]:
+        cmd = config.get("cmd", ["py", "python3"])
+    elif lang in ["ruby", "rb"]:
+        cmd = config.get("cmd", ["ruby", "ruby"])
+    c = config.get("c", {})
+    if lang in ["c", "c++", "cpp"]:
+        cmd = c.get("cc", None)
+    flags = c.get("cflags", " ").split(" ")
+    output_attr = c.get("output_attr", "-o")
+    output_file = make_path(os.getcwd(), c.get("output", "a.out"))
+    if cmd is None and lang in ["c", "c++", "cpp"]:
+        rprint(
+            f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('No C compiler found')}"
+        )
+        sys.exit(1)
+
+    try:
+        e = Entries()
+        e.add("mode", mode)
+        e.add("lang", lang)
+        e.add("the_file", the_file)
+        e.add("the_file_to_watch", the_file_to_watch)
+        e.add("base_dir", base_dir)
+        e.add("cmd", cmd)
+        e.add("flags", flags)
+        e.add("output_attr", output_attr)
+        e.add("output_file", output_file)
+        e.make_command_list()
+        v.verbose = verbose
+        if mode == "wrs":
+            wh = WrsHandler(
+                the_file=the_file,
+                command_list=e.get("command_list"),
+                language=lang,
+                base_dir=base_dir,
+                cmd=cmd,
+            )
+            BeautifulOutput(e)._run()
+            mode = wp.textWrapBold("(WRS)", "green")
+        else:
+            wh = WroHandler(
+                the_file=the_file,
+                the_file_to_watch=the_file_to_watch,
+                command_list=e.get("command_list"),
+                language=lang,
+                base_dir=base_dir,
+                cmd=cmd,
+            )
+            BeautifulOutput(e)._run()
+            mode = wp.textWrapBold("(WRO)", "green")
+        w = _Watcher(wh, base_dir)
+        print(" ")
+        rprint(f"Watching in {mode} mode...")
+        print(" ")
+        w.run()
+    except KeyboardInterrupt:
+        # pipe the error number to the shell
+        rprint(
+            f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('Keyboard Interrupt')}"
+        )
+        sys.exit(0)
+
 
 def watchFor(ms: int):
     """
     WATCH FOR
     ---------
     Watch for changes in the currentdir and return a json
     """
@@ -327,18 +469,32 @@
 
 
 @app.command(
     help="Watch for changes in the current directory and execute the program chosen",
     name="watch",
 )
 def run(
-    verbose: bool = typer.Option(False, "--verbose", "-v"),
+    verbose: bool = typer.Option(
+        False,
+        "--verbose",
+        "-v",
+        help="Activate verbose. In this case, the program notify any change"
+    ),
+    config: bool = typer.Option(
+        False,
+        "--config",
+        "-c",
+        help="Use the `.detectchange` config file when you launch the program with this flag"
+    ),
 ):
     if verbose:
         v.verbose = True
     else:
         v.verbose = False
-    activate()
+    if config:
+        cfg_activate()
+    else:
+        activate()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `changedetector-0.5.1/changedetector/menu.py` & `changedetector-0.6.0/changedetector/menu.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/versionControl.py` & `changedetector-0.6.0/changedetector/versionControl.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/wrapperComponents.py` & `changedetector-0.6.0/changedetector/wrapperComponents.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/wro.py` & `changedetector-0.6.0/changedetector/wro.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/wrs.py` & `changedetector-0.6.0/changedetector/wrs.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/wtch.py` & `changedetector-0.6.0/changedetector/wtch.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/scripts/detectchange.fish` & `changedetector-0.6.0/changedetector/scripts/detectchange.fish`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/scripts/detectchange.sh` & `changedetector-0.6.0/changedetector/scripts/detectchange.sh`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/tests/TEST.md` & `changedetector-0.6.0/changedetector/tests/TEST.md`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/tests/attrDatas.py` & `changedetector-0.6.0/changedetector/tests/attrDatas.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/tests/test.py` & `changedetector-0.6.0/changedetector/tests/test.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/changedetector/tests/testfile.py` & `changedetector-0.6.0/changedetector/tests/testfile.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/LICENCE` & `changedetector-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `changedetector-0.5.1/pyproject.toml` & `changedetector-0.6.0/pyproject.toml`

 * *Files identical despite different names*

