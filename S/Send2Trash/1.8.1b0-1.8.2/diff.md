# Comparing `tmp/Send2Trash-1.8.1b0.tar.gz` & `tmp/Send2Trash-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Send2Trash-1.8.1b0.tar", last modified: Sat Aug 21 03:43:58 2021, max compression
+gzip compressed data, was "Send2Trash-1.8.2.tar", last modified: Thu Apr 27 05:30:25 2023, max compression
```

## Comparing `Send2Trash-1.8.1b0.tar` & `Send2Trash-1.8.2.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxrwxrwx   0        0        0        0 2021-08-21 03:43:58.954267 Send2Trash-1.8.1b0/
--rw-rw-rw-   0        0        0     3146 2021-08-21 03:39:54.000000 Send2Trash-1.8.1b0/CHANGES.rst
--rw-rw-rw-   0        0        0     1504 2020-06-12 02:48:22.000000 Send2Trash-1.8.1b0/LICENSE
--rw-rw-rw-   0        0        0       29 2020-06-12 02:48:22.000000 Send2Trash-1.8.1b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3669 2021-08-21 03:43:58.955267 Send2Trash-1.8.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2021-08-08 02:02:31.000000 Send2Trash-1.8.1b0/README.rst
-drwxrwxrwx   0        0        0        0 2021-08-21 03:43:58.935267 Send2Trash-1.8.1b0/Send2Trash.egg-info/
--rw-rw-rw-   0        0        0     3669 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-08-21 03:43:58.000000 Send2Trash-1.8.1b0/Send2Trash.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2021-08-17 23:49:42.000000 Send2Trash-1.8.1b0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2021-08-21 03:43:58.953267 Send2Trash-1.8.1b0/send2trash/
--rw-rw-rw-   0        0        0     2650 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/IFileOperationProgressSink.py
--rw-rw-rw-   0        0        0      762 2020-06-19 02:43:10.000000 Send2Trash-1.8.1b0/send2trash/__init__.py
--rw-rw-rw-   0        0        0      982 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/__main__.py
--rw-rw-rw-   0        0        0      622 2020-06-19 02:44:35.000000 Send2Trash-1.8.1b0/send2trash/compat.py
--rw-rw-rw-   0        0        0     1022 2021-03-02 05:40:13.000000 Send2Trash-1.8.1b0/send2trash/exceptions.py
--rw-rw-rw-   0        0        0      907 2021-08-08 02:22:46.000000 Send2Trash-1.8.1b0/send2trash/plat_gio.py
--rw-rw-rw-   0        0        0      821 2021-05-15 02:37:31.000000 Send2Trash-1.8.1b0/send2trash/plat_osx.py
--rw-rw-rw-   0        0        0     1881 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/plat_osx_ctypes.py
--rw-rw-rw-   0        0        0     1020 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/plat_osx_pyobjc.py
--rw-rw-rw-   0        0        0     7331 2021-08-21 03:24:35.000000 Send2Trash-1.8.1b0/send2trash/plat_other.py
--rw-rw-rw-   0        0        0      781 2020-06-19 02:43:23.000000 Send2Trash-1.8.1b0/send2trash/plat_win.py
--rw-rw-rw-   0        0        0     5158 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/plat_win_legacy.py
--rw-rw-rw-   0        0        0     2692 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/plat_win_modern.py
--rw-rw-rw-   0        0        0      530 2021-08-17 23:53:19.000000 Send2Trash-1.8.1b0/send2trash/util.py
--rw-rw-rw-   0        0        0     1551 2021-08-21 03:43:58.956266 Send2Trash-1.8.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.029613 Send2Trash-1.8.2/
+-rw-rw-rw-   0        0        0     3529 2023-04-27 05:22:55.000000 Send2Trash-1.8.2/CHANGES.rst
+-rw-rw-rw-   0        0        0     1504 2020-06-12 02:48:22.000000 Send2Trash-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0       29 2020-06-12 02:48:22.000000 Send2Trash-1.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3696 2023-04-27 05:30:25.029613 Send2Trash-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2339 2021-08-08 02:02:31.000000 Send2Trash-1.8.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.000226 Send2Trash-1.8.2/Send2Trash.egg-info/
+-rw-rw-rw-   0        0        0     3696 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      233 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 05:30:24.000000 Send2Trash-1.8.2/Send2Trash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2022-04-30 22:02:09.000000 Send2Trash-1.8.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.011755 Send2Trash-1.8.2/send2trash/
+-rw-rw-rw-   0        0        0      802 2022-06-01 06:46:22.000000 Send2Trash-1.8.2/send2trash/__init__.py
+-rw-rw-rw-   0        0        0      982 2021-08-17 23:53:19.000000 Send2Trash-1.8.2/send2trash/__main__.py
+-rw-rw-rw-   0        0        0      622 2020-06-19 02:44:35.000000 Send2Trash-1.8.2/send2trash/compat.py
+-rw-rw-rw-   0        0        0     1032 2022-06-01 05:15:58.000000 Send2Trash-1.8.2/send2trash/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.016085 Send2Trash-1.8.2/send2trash/mac/
+-rw-rw-rw-   0        0        0      836 2022-06-01 05:19:22.000000 Send2Trash-1.8.2/send2trash/mac/__init__.py
+-rw-rw-rw-   0        0        0     1901 2022-06-01 05:19:45.000000 Send2Trash-1.8.2/send2trash/mac/legacy.py
+-rw-rw-rw-   0        0        0     1040 2022-06-01 05:20:07.000000 Send2Trash-1.8.2/send2trash/mac/modern.py
+-rw-rw-rw-   0        0        0      927 2022-06-01 05:15:43.000000 Send2Trash-1.8.2/send2trash/plat_gio.py
+-rw-rw-rw-   0        0        0     7252 2022-06-01 05:15:31.000000 Send2Trash-1.8.2/send2trash/plat_other.py
+-rw-rw-rw-   0        0        0      530 2021-08-17 23:53:19.000000 Send2Trash-1.8.2/send2trash/util.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.022086 Send2Trash-1.8.2/send2trash/win/
+-rw-rw-rw-   0        0        0     1584 2021-08-21 20:02:34.000000 Send2Trash-1.8.2/send2trash/win/IFileOperationProgressSink.py
+-rw-rw-rw-   0        0        0      796 2022-06-01 05:17:11.000000 Send2Trash-1.8.2/send2trash/win/__init__.py
+-rw-rw-rw-   0        0        0     7288 2023-04-27 04:38:08.000000 Send2Trash-1.8.2/send2trash/win/legacy.py
+-rw-rw-rw-   0        0        0     2790 2022-07-27 03:50:06.000000 Send2Trash-1.8.2/send2trash/win/modern.py
+-rw-rw-rw-   0        0        0     1644 2023-04-27 05:30:25.031614 Send2Trash-1.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 05:30:25.028610 Send2Trash-1.8.2/tests/
+-rw-rw-rw-   0        0        0        0 2021-03-02 04:02:08.000000 Send2Trash-1.8.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     7240 2022-05-01 00:47:54.000000 Send2Trash-1.8.2/tests/test_plat_other.py
+-rw-rw-rw-   0        0        0     5804 2022-07-27 03:49:48.000000 Send2Trash-1.8.2/tests/test_plat_win.py
+-rw-rw-rw-   0        0        0     1227 2021-08-17 23:53:19.000000 Send2Trash-1.8.2/tests/test_script_main.py
```

### Comparing `Send2Trash-1.8.1b0/LICENSE` & `Send2Trash-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Send2Trash-1.8.1b0/PKG-INFO` & `Send2Trash-1.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: Send2Trash
-Version: 1.8.1b0
+Version: 1.8.2
 Summary: Send file to trash natively under Mac OS X, Windows and Linux
 Home-page: https://github.com/arsenetar/send2trash
 Author: Andrew Senetar
 Author-email: arsenetar@voltaicideas.net
 License: BSD License
 Project-URL: Bug Reports, https://github.com/arsenetar/send2trash/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: File Managers
 Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7
 Description-Content-Type: text/x-rst
 Provides-Extra: win32
 Provides-Extra: objc
 Provides-Extra: nativeLib
 License-File: LICENSE
@@ -82,9 +82,7 @@
 create a ``.Trash-$UID`` directory.
 
 For any other problem, ``OSError`` is raised.
 
 .. _PyGObject: https://wiki.gnome.org/PyGObject
 .. _GIO: https://developer.gnome.org/gio/
 .. _trash specifications from freedesktop.org: http://freedesktop.org/wiki/Specifications/trash-spec/
-
-
```

### Comparing `Send2Trash-1.8.1b0/README.rst` & `Send2Trash-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `Send2Trash-1.8.1b0/Send2Trash.egg-info/PKG-INFO` & `Send2Trash-1.8.2/Send2Trash.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: Send2Trash
-Version: 1.8.1b0
+Version: 1.8.2
 Summary: Send file to trash natively under Mac OS X, Windows and Linux
 Home-page: https://github.com/arsenetar/send2trash
 Author: Andrew Senetar
 Author-email: arsenetar@voltaicideas.net
 License: BSD License
 Project-URL: Bug Reports, https://github.com/arsenetar/send2trash/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: File Managers
 Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7
 Description-Content-Type: text/x-rst
 Provides-Extra: win32
 Provides-Extra: objc
 Provides-Extra: nativeLib
 License-File: LICENSE
@@ -82,9 +82,7 @@
 create a ``.Trash-$UID`` directory.
 
 For any other problem, ``OSError`` is raised.
 
 .. _PyGObject: https://wiki.gnome.org/PyGObject
 .. _GIO: https://developer.gnome.org/gio/
 .. _trash specifications from freedesktop.org: http://freedesktop.org/wiki/Specifications/trash-spec/
-
-
```

### Comparing `Send2Trash-1.8.1b0/send2trash/__init__.py` & `Send2Trash-1.8.2/send2trash/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # This software is licensed under the "BSD" License as described in the "LICENSE" file,
 # which should be included with this package. The terms are also available at
 # http://www.hardcoded.net/licenses/bsd_license
 
 import sys
 
-from .exceptions import TrashPermissionError  # noqa: F401
+from send2trash.exceptions import TrashPermissionError  # noqa: F401
 
 if sys.platform == "darwin":
-    from .plat_osx import send2trash
+    from send2trash.mac import send2trash
 elif sys.platform == "win32":
-    from .plat_win import send2trash
+    from send2trash.win import send2trash
 else:
     try:
         # If we can use gio, let's use it
-        from .plat_gio import send2trash
+        from send2trash.plat_gio import send2trash
     except ImportError:
         # Oh well, let's fallback to our own Freedesktop trash implementation
-        from .plat_other import send2trash  # noqa: F401
+        from send2trash.plat_other import send2trash  # noqa: F401
```

### Comparing `Send2Trash-1.8.1b0/send2trash/__main__.py` & `Send2Trash-1.8.2/send2trash/__main__.py`

 * *Files identical despite different names*

### Comparing `Send2Trash-1.8.1b0/send2trash/compat.py` & `Send2Trash-1.8.2/send2trash/compat.py`

 * *Files identical despite different names*

### Comparing `Send2Trash-1.8.1b0/send2trash/exceptions.py` & `Send2Trash-1.8.2/send2trash/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import errno
-from .compat import PY3
+from send2trash.compat import PY3
 
 if PY3:
     _permission_error = PermissionError  # noqa: F821
 else:
     _permission_error = OSError
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_gio.py` & `Send2Trash-1.8.2/send2trash/plat_gio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2017 Virgil Dupras
 
 # This software is licensed under the "BSD" License as described in the "LICENSE" file,
 # which should be included with this package. The terms are also available at
 # http://www.hardcoded.net/licenses/bsd_license
 
 from gi.repository import GObject, Gio
-from .exceptions import TrashPermissionError
-from .util import preprocess_paths
+from send2trash.exceptions import TrashPermissionError
+from send2trash.util import preprocess_paths
 
 
 def send2trash(paths):
     paths = preprocess_paths(paths)
     for path in paths:
         try:
             f = Gio.File.new_for_path(path)
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_osx_ctypes.py` & `Send2Trash-1.8.2/send2trash/mac/legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # http://www.hardcoded.net/licenses/bsd_license
 
 from __future__ import unicode_literals
 
 from ctypes import cdll, byref, Structure, c_char, c_char_p
 from ctypes.util import find_library
 
-from .compat import binary_type
-from .util import preprocess_paths
+from send2trash.compat import binary_type
+from send2trash.util import preprocess_paths
 
 Foundation = cdll.LoadLibrary(find_library("Foundation"))
 CoreServices = cdll.LoadLibrary(find_library("CoreServices"))
 
 GetMacOSStatusCommentString = Foundation.GetMacOSStatusCommentString
 GetMacOSStatusCommentString.restype = c_char_p
 FSPathMakeRefWithOptions = CoreServices.FSPathMakeRefWithOptions
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_osx_pyobjc.py` & `Send2Trash-1.8.2/send2trash/mac/modern.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2017 Virgil Dupras
 
 # This software is licensed under the "BSD" License as described in the "LICENSE" file,
 # which should be included with this package. The terms are also available at
 # http://www.hardcoded.net/licenses/bsd_license
 
 from Foundation import NSFileManager, NSURL
-from .compat import text_type
-from .util import preprocess_paths
+from send2trash.compat import text_type
+from send2trash.util import preprocess_paths
 
 
 def check_op_result(op_result):
     # First value will be false on failure
     if not op_result[0]:
         # Error is in third value, localized failure reason matchs ctypes version
         raise OSError(op_result[2].localizedFailureReason())
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_other.py` & `Send2Trash-1.8.2/send2trash/plat_other.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 try:
     from urllib.parse import quote
 except ImportError:
     # Python 2
     from urllib import quote
 
-from .compat import text_type, environb
-from .util import preprocess_paths
-from .exceptions import TrashPermissionError
+from send2trash.compat import text_type, environb
+from send2trash.util import preprocess_paths
+from send2trash.exceptions import TrashPermissionError
 
 try:
     fsencode = os.fsencode  # Python 3
     fsdecode = os.fsdecode
 except AttributeError:
 
     def fsencode(u):  # Python 2
@@ -178,34 +178,31 @@
 def send2trash(paths):
     paths = preprocess_paths(paths)
     for path in paths:
         if isinstance(path, text_type):
             path_b = fsencode(path)
         elif isinstance(path, bytes):
             path_b = path
-        elif hasattr(path, "__fspath__"):
-            # Python 3.6 PathLike protocol
-            return send2trash(path.__fspath__())
         else:
             raise TypeError("str, bytes or PathLike expected, not %r" % type(path))
 
         if not op.exists(path_b):
-            raise OSError("File not found: %s" % path)
+            raise OSError(errno.ENOENT, "File not found: %s" % path)
         # ...should check whether the user has the necessary permissions to delete
         # it, before starting the trashing operation itself. [2]
         if not os.access(path_b, os.W_OK):
-            raise OSError("Permission denied: %s" % path)
-        # if the file to be trashed is on the same device as HOMETRASH we
-        # want to move it there.
-        path_dev = get_dev(path_b)
+            raise OSError(errno.EACCES, "Permission denied: %s" % path)
 
+        path_dev = get_dev(path_b)
         # If XDG_DATA_HOME or HOMETRASH do not yet exist we need to stat the
         # home directory, and these paths will be created further on if needed.
         trash_dev = get_dev(op.expanduser(b"~"))
 
+        # if the file to be trashed is on the same device as HOMETRASH we
+        # want to move it there.
         if path_dev == trash_dev:
             topdir = XDG_DATA_HOME
             dest_trash = HOMETRASH_B
         else:
             topdir = find_mount_point(path_b)
             trash_dev = get_dev(topdir)
             if trash_dev != path_dev:
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_win.py` & `Send2Trash-1.8.2/send2trash/win/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 from __future__ import unicode_literals
 from platform import version
 
 # if windows is vista or newer and pywin32 is available use IFileOperation
 if int(version().split(".", 1)[0]) >= 6:
     try:
         # Attempt to use pywin32 to use IFileOperation
-        from .plat_win_modern import send2trash
+        from send2trash.win.modern import send2trash
     except ImportError:
         # use SHFileOperation as fallback
-        from .plat_win_legacy import send2trash
+        from send2trash.win.legacy import send2trash
 else:
     # use SHFileOperation as fallback
-    from .plat_win_legacy import send2trash  # noqa: F401
+    from send2trash.win.legacy import send2trash  # noqa: F401
```

### Comparing `Send2Trash-1.8.1b0/send2trash/plat_win_modern.py` & `Send2Trash-1.8.2/send2trash/win/modern.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,51 +2,56 @@
 
 # This software is licensed under the "BSD" License as described in the "LICENSE" file,
 # which should be included with this package. The terms are also available at
 # http://www.hardcoded.net/licenses/bsd_license
 
 from __future__ import unicode_literals
 import os.path as op
-from .compat import text_type
-from .util import preprocess_paths
+from send2trash.compat import text_type
+from send2trash.util import preprocess_paths
 from platform import version
 import pythoncom
 import pywintypes
 from win32com.shell import shell, shellcon
-from .IFileOperationProgressSink import CreateSink
+from send2trash.win.IFileOperationProgressSink import create_sink
 
 
 def send2trash(paths):
     paths = preprocess_paths(paths)
+    if not paths:
+        return
     # convert data type
     paths = [text_type(path, "mbcs") if not isinstance(path, text_type) else path for path in paths]
     # convert to full paths
     paths = [op.abspath(path) if not op.isabs(path) else path for path in paths]
     # remove the leading \\?\ if present
     paths = [path[4:] if path.startswith("\\\\?\\") else path for path in paths]
     # Need to initialize the com before using
     pythoncom.CoInitialize()
     # create instance of file operation object
     fileop = pythoncom.CoCreateInstance(
-        shell.CLSID_FileOperation, None, pythoncom.CLSCTX_ALL, shell.IID_IFileOperation,
+        shell.CLSID_FileOperation,
+        None,
+        pythoncom.CLSCTX_ALL,
+        shell.IID_IFileOperation,
     )
     # default flags to use
     flags = shellcon.FOF_NOCONFIRMATION | shellcon.FOF_NOERRORUI | shellcon.FOF_SILENT | shellcon.FOFX_EARLYFAILURE
     # determine rest of the flags based on OS version
     # use newer recommended flags if available
     if int(version().split(".", 1)[0]) >= 8:
         flags |= 0x20000000 | 0x00080000  # FOFX_ADDUNDORECORD win 8+  # FOFX_RECYCLEONDELETE win 8+
     else:
         flags |= shellcon.FOF_ALLOWUNDO
     # set the flags
     fileop.SetOperationFlags(flags)
     # actually try to perform the operation, this section may throw a
     # pywintypes.com_error which does not seem to create as nice of an
     # error as OSError so wrapping with try to convert
-    sink = CreateSink()
+    sink = create_sink()
     try:
         for path in paths:
             item = shell.SHCreateItemFromParsingName(path, None, shell.IID_IShellItem)
             fileop.DeleteItem(item, sink)
         result = fileop.PerformOperations()
         aborted = fileop.GetAnyOperationsAborted()
         # if non-zero result or aborted throw an exception
```

### Comparing `Send2Trash-1.8.1b0/send2trash/util.py` & `Send2Trash-1.8.2/send2trash/util.py`

 * *Files identical despite different names*

### Comparing `Send2Trash-1.8.1b0/setup.cfg` & `Send2Trash-1.8.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 656e 6432 5472 6173 680d 0a76   = Send2Trash..v
-00000020: 6572 7369 6f6e 203d 2031 2e38 2e31 6230  ersion = 1.8.1b0
-00000030: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000040: 6769 7468 7562 2e63 6f6d 2f61 7273 656e  github.com/arsen
-00000050: 6574 6172 2f73 656e 6432 7472 6173 680d  etar/send2trash.
-00000060: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000070: 0d0a 0942 7567 2052 6570 6f72 7473 203d  ...Bug Reports =
-00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000090: 636f 6d2f 6172 7365 6e65 7461 722f 7365  com/arsenetar/se
-000000a0: 6e64 3274 7261 7368 2f69 7373 7565 730d  nd2trash/issues.
-000000b0: 0a61 7574 686f 7220 3d20 416e 6472 6577  .author = Andrew
-000000c0: 2053 656e 6574 6172 0d0a 6175 7468 6f72   Senetar..author
-000000d0: 5f65 6d61 696c 203d 2061 7273 656e 6574  _email = arsenet
-000000e0: 6172 4076 6f6c 7461 6963 6964 6561 732e  ar@voltaicideas.
-000000f0: 6e65 740d 0a6c 6963 656e 7365 203d 2042  net..license = B
-00000100: 5344 204c 6963 656e 7365 0d0a 6c69 6365  SD License..lice
-00000110: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
-00000120: 4e53 450d 0a64 6573 6372 6970 7469 6f6e  NSE..description
-00000130: 203d 2053 656e 6420 6669 6c65 2074 6f20   = Send file to 
-00000140: 7472 6173 6820 6e61 7469 7665 6c79 2075  trash natively u
-00000150: 6e64 6572 204d 6163 204f 5320 582c 2057  nder Mac OS X, W
-00000160: 696e 646f 7773 2061 6e64 204c 696e 7578  indows and Linux
-00000170: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000180: 6f6e 203d 2066 696c 653a 5245 4144 4d45  on = file:README
-00000190: 2e72 7374 0d0a 6c6f 6e67 5f64 6573 6372  .rst..long_descr
-000001a0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000001b0: 7970 6520 3d20 7465 7874 2f78 2d72 7374  ype = text/x-rst
-000001c0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000001d0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-000001e0: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
-000001f0: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
-00000200: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-00000210: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-00000220: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000230: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
-00000240: 4420 4c69 6365 6e73 650d 0a09 4f70 6572  D License...Oper
-00000250: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000260: 4d61 634f 5320 3a3a 204d 6163 4f53 2058  MacOS :: MacOS X
-00000270: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000280: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
-00000290: 203a 3a20 5769 6e64 6f77 730d 0a09 4f70   :: Windows...Op
-000002a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000002b0: 3a20 504f 5349 580d 0a09 5072 6f67 7261  : POSIX...Progra
-000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002d0: 3a20 5079 7468 6f6e 203a 3a20 322e 370d  : Python :: 2.7.
-000002e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000300: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
-00000310: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000320: 5079 7468 6f6e 203a 3a20 332e 350d 0a09  Python :: 3.5...
-00000330: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000340: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000350: 3a20 332e 360d 0a09 5072 6f67 7261 6d6d  : 3.6...Programm
-00000360: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000370: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
-00000380: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000390: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003a0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
-000003b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003c0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-000003d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003f0: 3a20 332e 3130 0d0a 0954 6f70 6963 203a  : 3.10...Topic :
-00000400: 3a20 4465 736b 746f 7020 456e 7669 726f  : Desktop Enviro
-00000410: 6e6d 656e 7420 3a3a 2046 696c 6520 4d61  nment :: File Ma
-00000420: 6e61 6765 7273 0d0a 0d0a 5b6f 7074 696f  nagers....[optio
-00000430: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-00000440: 7365 6e64 3274 7261 7368 0d0a 7465 7374  send2trash..test
-00000450: 735f 7265 7175 6972 6520 3d20 7079 7465  s_require = pyte
-00000460: 7374 0d0a 7079 7468 6f6e 5f72 6571 7569  st..python_requi
-00000470: 7265 7320 3d20 3e3d 322e 372c 2021 3d33  res = >=2.7, !=3
-00000480: 2e30 2e2a 2c20 213d 332e 312e 2a2c 2021  .0.*, !=3.1.*, !
-00000490: 3d33 2e32 2e2a 2c20 213d 332e 332e 2a2c  =3.2.*, !=3.3.*,
-000004a0: 2021 3d33 2e34 2e2a 0d0a 0d0a 5b6f 7074   !=3.4.*....[opt
-000004b0: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
-000004c0: 6972 655d 0d0a 7769 6e33 3220 3d20 7079  ire]..win32 = py
-000004d0: 7769 6e33 323b 2073 7973 5f70 6c61 7466  win32; sys_platf
-000004e0: 6f72 6d20 3d3d 2022 7769 6e33 3222 0d0a  orm == "win32"..
-000004f0: 6f62 6a63 203d 2070 796f 626a 632d 6672  objc = pyobjc-fr
-00000500: 616d 6577 6f72 6b2d 436f 636f 613b 2073  amework-Cocoa; s
-00000510: 7973 5f70 6c61 7466 6f72 6d20 3d3d 2022  ys_platform == "
-00000520: 6461 7277 696e 220d 0a6e 6174 6976 656c  darwin"..nativel
-00000530: 6962 203d 200d 0a09 7079 7769 6e33 323b  ib = ...pywin32;
-00000540: 2073 7973 5f70 6c61 7466 6f72 6d20 3d3d   sys_platform ==
-00000550: 2022 7769 6e33 3222 0d0a 0970 796f 626a   "win32"...pyobj
-00000560: 632d 6672 616d 6577 6f72 6b2d 436f 636f  c-framework-Coco
-00000570: 613b 2073 7973 5f70 6c61 7466 6f72 6d20  a; sys_platform 
-00000580: 3d3d 2022 6461 7277 696e 220d 0a0d 0a5b  == "darwin"....[
-00000590: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-000005a0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000005b0: 6372 6970 7473 203d 200d 0a09 7365 6e64  cripts = ...send
-000005c0: 3274 7261 7368 203d 2073 656e 6432 7472  2trash = send2tr
-000005d0: 6173 682e 5f5f 6d61 696e 5f5f 3a6d 6169  ash.__main__:mai
-000005e0: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
-000005f0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000600: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 6572 7369 6f6e 203d 2031 2e38 2e32 0d0a  ersion = 1.8.2..
+00000030: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000040: 7468 7562 2e63 6f6d 2f61 7273 656e 6574  thub.com/arsenet
+00000050: 6172 2f73 656e 6432 7472 6173 680d 0a70  ar/send2trash..p
+00000060: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000070: 0942 7567 2052 6570 6f72 7473 203d 2068  .Bug Reports = h
+00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000090: 6d2f 6172 7365 6e65 7461 722f 7365 6e64  m/arsenetar/send
+000000a0: 3274 7261 7368 2f69 7373 7565 730d 0a61  2trash/issues..a
+000000b0: 7574 686f 7220 3d20 416e 6472 6577 2053  uthor = Andrew S
+000000c0: 656e 6574 6172 0d0a 6175 7468 6f72 5f65  enetar..author_e
+000000d0: 6d61 696c 203d 2061 7273 656e 6574 6172  mail = arsenetar
+000000e0: 4076 6f6c 7461 6963 6964 6561 732e 6e65  @voltaicideas.ne
+000000f0: 740d 0a6c 6963 656e 7365 203d 2042 5344  t..license = BSD
+00000100: 204c 6963 656e 7365 0d0a 6c69 6365 6e73   License..licens
+00000110: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
+00000120: 450d 0a64 6573 6372 6970 7469 6f6e 203d  E..description =
+00000130: 2053 656e 6420 6669 6c65 2074 6f20 7472   Send file to tr
+00000140: 6173 6820 6e61 7469 7665 6c79 2075 6e64  ash natively und
+00000150: 6572 204d 6163 204f 5320 582c 2057 696e  er Mac OS X, Win
+00000160: 646f 7773 2061 6e64 204c 696e 7578 0d0a  dows and Linux..
+00000170: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000180: 203d 2066 696c 653a 5245 4144 4d45 2e72   = file:README.r
+00000190: 7374 0d0a 6c6f 6e67 5f64 6573 6372 6970  st..long_descrip
+000001a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000001b0: 6520 3d20 7465 7874 2f78 2d72 7374 0d0a  e = text/x-rst..
+000001c0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+000001d0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+000001e0: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+000001f0: 6374 696f 6e2f 5374 6162 6c65 0d0a 0949  ction/Stable...I
+00000200: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000210: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+00000220: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000230: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
+00000240: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000250: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+00000260: 634f 5320 3a3a 204d 6163 4f53 2058 0d0a  cOS :: MacOS X..
+00000270: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000280: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
+00000290: 3a20 5769 6e64 6f77 730d 0a09 4f70 6572  : Windows...Oper
+000002a0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000002b0: 504f 5349 580d 0a09 5072 6f67 7261 6d6d  POSIX...Programm
+000002c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002d0: 5079 7468 6f6e 203a 3a20 322e 370d 0a09  Python :: 2.7...
+000002e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000300: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+00000310: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000320: 7468 6f6e 203a 3a20 332e 350d 0a09 5072  thon :: 3.5...Pr
+00000330: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000340: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000350: 332e 360d 0a09 5072 6f67 7261 6d6d 696e  3.6...Programmin
+00000360: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000370: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
+00000380: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000390: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003a0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+000003b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003c0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
+000003d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000003e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000003f0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
+00000400: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000410: 7974 686f 6e20 3a3a 2033 2e31 310d 0a09  ython :: 3.11...
+00000420: 546f 7069 6320 3a3a 2044 6573 6b74 6f70  Topic :: Desktop
+00000430: 2045 6e76 6972 6f6e 6d65 6e74 203a 3a20   Environment :: 
+00000440: 4669 6c65 204d 616e 6167 6572 730d 0a0d  File Managers...
+00000450: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+00000460: 6167 6573 203d 2066 696e 643a 0d0a 7465  ages = find:..te
+00000470: 7374 735f 7265 7175 6972 6520 3d20 7079  sts_require = py
+00000480: 7465 7374 0d0a 7079 7468 6f6e 5f72 6571  test..python_req
+00000490: 7569 7265 7320 3d20 3e3d 322e 372c 2021  uires = >=2.7, !
+000004a0: 3d33 2e30 2e2a 2c20 213d 332e 312e 2a2c  =3.0.*, !=3.1.*,
+000004b0: 2021 3d33 2e32 2e2a 2c20 213d 332e 332e   !=3.2.*, !=3.3.
+000004c0: 2a2c 2021 3d33 2e34 2e2a 0d0a 0d0a 5b6f  *, !=3.4.*....[o
+000004d0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000004e0: 6669 6e64 5d0d 0a69 6e63 6c75 6465 203d  find]..include =
+000004f0: 200d 0a09 7365 6e64 3274 7261 7368 2a0d   ...send2trash*.
+00000500: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
+00000510: 6173 5f72 6571 7569 7265 5d0d 0a77 696e  as_require]..win
+00000520: 3332 203d 200d 0a09 7079 7769 6e33 323b  32 = ...pywin32;
+00000530: 2073 7973 5f70 6c61 7466 6f72 6d20 3d3d   sys_platform ==
+00000540: 2022 7769 6e33 3222 0d0a 6f62 6a63 203d   "win32"..objc =
+00000550: 200d 0a09 7079 6f62 6a63 2d66 7261 6d65   ...pyobjc-frame
+00000560: 776f 726b 2d43 6f63 6f61 3b20 7379 735f  work-Cocoa; sys_
+00000570: 706c 6174 666f 726d 203d 3d20 2264 6172  platform == "dar
+00000580: 7769 6e22 0d0a 6e61 7469 7665 4c69 6220  win"..nativeLib 
+00000590: 3d20 0d0a 0970 7977 696e 3332 3b20 7379  = ...pywin32; sy
+000005a0: 735f 706c 6174 666f 726d 203d 3d20 2277  s_platform == "w
+000005b0: 696e 3332 220d 0a09 7079 6f62 6a63 2d66  in32"...pyobjc-f
+000005c0: 7261 6d65 776f 726b 2d43 6f63 6f61 3b20  ramework-Cocoa; 
+000005d0: 7379 735f 706c 6174 666f 726d 203d 3d20  sys_platform == 
+000005e0: 2264 6172 7769 6e22 0d0a 0d0a 5b6f 7074  "darwin"....[opt
+000005f0: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
+00000600: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
+00000610: 7074 7320 3d20 0d0a 0973 656e 6432 7472  pts = ...send2tr
+00000620: 6173 6820 3d20 7365 6e64 3274 7261 7368  ash = send2trash
+00000630: 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e 0d0a  .__main__:main..
+00000640: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000650: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000660: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

