# Comparing `tmp/fookebox-1.0.0.tar.gz` & `tmp/fookebox-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fookebox-1.0.0.tar", last modified: Fri Apr 14 00:56:09 2023, max compression
+gzip compressed data, was "fookebox-1.0.1.tar", last modified: Thu Apr 27 00:51:30 2023, max compression
```

## Comparing `fookebox-1.0.0.tar` & `fookebox-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    34523 2023-04-14 00:54:11.000000 fookebox-1.0.0/COPYING
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-14 00:56:09.432418 fookebox-1.0.0/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)      886 2023-04-14 00:54:11.000000 fookebox-1.0.0/README.md
--rw-r--r--   0 stefan    (1027) stefan    (1027)       89 2023-04-14 00:54:11.000000 fookebox-1.0.0/pyproject.toml
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1735 2023-04-14 00:56:09.432418 fookebox-1.0.0/setup.cfg
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      720 2023-04-14 00:54:40.000000 fookebox-1.0.0/src/fookebox/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     4529 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/autoqueue.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1991 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/config.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/css/
--rw-r--r--   0 stefan    (1027) stefan    (1027)   121457 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/bootstrap.min.css
--rw-r--r--   0 stefan    (1027) stefan    (1027)   540434 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/bootstrap.min.css.map
--rw-r--r--   0 stefan    (1027) stefan    (1027)     6178 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/fookebox.css
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/fonts/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    20127 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 stefan    (1027) stefan    (1027)   108738 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 stefan    (1027) stefan    (1027)    45404 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 stefan    (1027) stefan    (1027)    23424 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 stefan    (1027) stefan    (1027)    18028 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3860 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fookebox.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    13514 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/handlers.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/de/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/de/LC_MESSAGES/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1106 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/i18n/de/LC_MESSAGES/fookebox.mo
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/js/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    39680 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/bootstrap.min.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)    13894 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/fookebox.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)      958 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/i18n-de.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)      832 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/i18n.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)    97163 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/jquery-1.12.4.min.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)   255084 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/jquery-ui.min.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1895 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/mpd.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/py.typed
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/templates/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     5302 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/templates/client.html
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox.egg-info/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1147 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)       52 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/entry_points.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)       87 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/requires.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        9 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/top_level.txt
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/tests/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    13312 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_auto_queue.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     4864 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_config.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    24552 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_handlers.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     6389 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_template.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.981438 fookebox-1.0.1/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    34523 2023-04-14 00:54:11.000000 fookebox-1.0.1/COPYING
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-27 00:51:30.981438 fookebox-1.0.1/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      886 2023-04-14 00:54:11.000000 fookebox-1.0.1/README.md
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       89 2023-04-14 00:54:11.000000 fookebox-1.0.1/pyproject.toml
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1751 2023-04-27 00:51:30.981438 fookebox-1.0.1/setup.cfg
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      956 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/__init__.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5945 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/autoqueue.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1991 2023-04-23 17:23:52.000000 fookebox-1.0.1/src/fookebox/config.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox/css/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   121457 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/css/bootstrap.min.css
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   540434 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/css/bootstrap.min.css.map
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     6178 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/css/fookebox.css
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox/fonts/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    20127 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   108738 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    45404 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    23424 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    18028 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2633 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/fookebox.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    12941 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/handlers.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox/i18n/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox/i18n/de/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.981438 fookebox-1.0.1/src/fookebox/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1106 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/i18n/de/LC_MESSAGES/fookebox.mo
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.981438 fookebox-1.0.1/src/fookebox/js/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    39680 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/js/bootstrap.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    14431 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/js/fookebox.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      961 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/js/i18n-de.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      861 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/js/i18n.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    97163 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/js/jquery-1.12.4.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   255084 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/js/jquery-ui.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5025 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/mpd.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/py.typed
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2622 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/tasks.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.981438 fookebox-1.0.1/src/fookebox/templates/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5302 2023-04-14 00:54:11.000000 fookebox-1.0.1/src/fookebox/templates/client.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2487 2023-04-27 00:51:03.000000 fookebox-1.0.1/src/fookebox/util.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.978104 fookebox-1.0.1/src/fookebox.egg-info/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1218 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       52 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/entry_points.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      102 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/requires.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        9 2023-04-27 00:51:30.000000 fookebox-1.0.1/src/fookebox.egg-info/top_level.txt
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-27 00:51:30.981438 fookebox-1.0.1/tests/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    18459 2023-04-27 00:51:03.000000 fookebox-1.0.1/tests/test_auto_queue.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5355 2023-04-27 00:51:03.000000 fookebox-1.0.1/tests/test_config.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    24420 2023-04-27 00:51:03.000000 fookebox-1.0.1/tests/test_handlers.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     8073 2023-04-27 00:51:03.000000 fookebox-1.0.1/tests/test_mpd_interface.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     7330 2023-04-27 00:51:03.000000 fookebox-1.0.1/tests/test_template.py
```

### Comparing `fookebox-1.0.0/COPYING` & `fookebox-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/PKG-INFO` & `fookebox-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fookebox
-Version: 1.0.0
+Version: 1.0.1
 Summary: A jukebox-style web-frontend to mpd
 Home-page: https://code.ott.net/fookebox/
 Author: Stefan Ott
 Author-email: stefan@ott.net
 Project-URL: Source, https://git.ott.net/fookebox/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `fookebox-1.0.0/README.md` & `fookebox-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/setup.cfg` & `fookebox-1.0.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	python-magic
 
 [options.extras_require]
 dev = 
 	build
 test = 
 	pytest
+	pytest-asyncio
 	pytest-cov
 	beautifulsoup4
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `fookebox-1.0.0/src/fookebox/__init__.py` & `fookebox-1.0.1/src/fookebox/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '1.0.0'
+"""
+fookebox
+========
+
+fookebox is a jukebox-style web-frontend to MPD.
+
+It can be used as a keyboard-less jukebox, as a powerful MPD control frontend
+or as anything in between.
+
+See https://code.ott.net/fookebox/ for more details.
+"""
+__version__ = '1.0.1'
```

### Comparing `fookebox-1.0.0/src/fookebox/config.py` & `fookebox-1.0.1/src/fookebox/config.py`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/css/bootstrap.min.css` & `fookebox-1.0.1/src/fookebox/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/css/bootstrap.min.css.map` & `fookebox-1.0.1/src/fookebox/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/css/fookebox.css` & `fookebox-1.0.1/src/fookebox/css/fookebox.css`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.eot` & `fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.svg` & `fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.ttf` & `fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff` & `fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff2` & `fookebox-1.0.1/src/fookebox/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/handlers.py` & `fookebox-1.0.1/src/fookebox/handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,85 +21,86 @@
 from importlib import resources
 import json
 
 import magic
 from mpd.base import CommandError
 from tornado import template
 from tornado.web import HTTPError, RequestHandler
+from tornado.websocket import WebSocketHandler
 
 import fookebox
-from .mpd import MPDContext
+from .mpd import IdleSocket, MPDContext, MPDSubscriber
 
 
 class ArtistHandler(RequestHandler):
     """
     A RequestHandler to load tracks by a particular artist.
 
     Methods
     -------
     get(artist):
         Load tracks of by particular artist.
     """
     # pylint: disable=abstract-method
-    def initialize(self, mpd: MPDContext):
+    def initialize(self, mpd: MPDContext) -> None:
         """Initialize the ArtistHandler object"""
         # pylint: disable=attribute-defined-outside-init
         self._mpd = mpd
 
-    def get(self, artist: str):
+    async def get(self, artist: str) -> None:
         """
         Returns tracks by a particular artist.
 
         Parameters
         ----------
         artist : str
             name of the artist
 
         Returns
         -------
         A list of tracks by the specified artist, wrapped in a dictionary under
         the 'tracks' key.
         """
-        with self._mpd as client:
-            hits = client.find('artist', artist)
+        async with self._mpd as client:
+            hits = await client.find('artist', artist)
 
         self.write({'tracks': hits})
 
 
 class GenreHandler(RequestHandler):
     """
     A RequestHandler to load tracks of a particular genre.
 
     Methods
     -------
     get(genre):
         Load tracks of a particular genre.
     """
     # pylint: disable=abstract-method
-    def initialize(self, mpd: MPDContext):
+    def initialize(self, mpd: MPDContext) -> None:
         """Initialize the GenreHandler object"""
         # pylint: disable=attribute-defined-outside-init
         self._mpd = mpd
 
-    def get(self, genre: str):
+    async def get(self, genre: str) -> None:
         """
         Returns tracks from a particular genre.
 
         Parameters
         ----------
         genre : str
             name of the genre
 
         Returns
         -------
         A list of tracks from the specified genre, wrapped in a dictionary
         under the 'tracks' key.
         """
-        with self._mpd as client:
-            hits = client.find('genre', genre)
+        async with self._mpd as client:
+            hits = await client.find('genre', genre)
 
         self.write({'tracks': hits})
 
 
 class ControlHandler(RequestHandler):
     """
     A RequestHandler to control MPD.
@@ -109,38 +110,34 @@
 
     Methods
     -------
     post():
         Send a command to MPD
     """
     # pylint: disable=abstract-method
-    def initialize(self, mpd: MPDContext, cfg: SectionProxy):
+    def initialize(self, mpd: MPDContext, cfg: SectionProxy) -> None:
         """Initialize the ControlHandler object"""
         # pylint: disable=attribute-defined-outside-init
         self._mpd = mpd
         self._cfg = cfg
 
-    def post(self):
+    async def post(self) -> None:
         """
         Send a command to MPD
 
         A JSON-encoded dictionary with the keyword 'action' and the MPD command
         as a value is expected in the POST body. Something like this:
 
             {'action': 'play'}
 
         Valid commands are play, pause, next, prev, volup, voldown and rebuild.
 
         Whether or not clients are allowed to send MPD commands can be
         configured using the 'enable_controls' config option.
 
-        Returns
-        -------
-        This method does not return anything.
-
         Exceptions
         ----------
         - If controls have been disabled, a HTTP 403 error is raised.
         - If the supplied JSON data is invalid, a HTTP 400 error is raised.
         - If an unknown command has been sent, a HTTP 400 error is raised.
         """
         if not self._cfg.getboolean('enable_controls'):
@@ -157,86 +154,81 @@
             'play': lambda client: client.play(),
             'pause': lambda client: client.pause(),
             'volup': lambda client: client.volume(+10),
             'voldown': lambda client: client.volume(-10),
             'rebuild': lambda client: client.update()
         }
 
-        action = data.get('action')
-        if action not in commands:
+        if (action := data.get('action')) in commands:
+            async with self._mpd as client:
+                await commands[action](client)
+        else:
             raise HTTPError(400, 'Invalid command')
 
-        with self._mpd as client:
-            commands[action](client)
-
 
 class CoverArtHandler(RequestHandler):
     """
     A RequestHandler that serves cover art.
 
     Methods
     -------
     get(filename):
         Get cover art for a file
     """
     # pylint: disable=abstract-method
-    def initialize(self, mpd: MPDContext, cfg: SectionProxy):
+    def initialize(self, mpd: MPDContext, cfg: SectionProxy) -> None:
         """Initialize the CoverArtHandler object"""
         # pylint: disable=attribute-defined-outside-init
         self._mpd = mpd
         self._cfg = cfg
 
-    def get(self, filename: str):
+    async def get(self, filename: str) -> None:
         """
         Returns cover art for a particular file.
 
         Parameters
         ----------
         filename : str
             name of the file
 
-        Returns
-        -------
-        Cover art for the specified file name.
-
         Exceptions
         ----------
         If no cover art is found, a HTTP 404 error is raised
         """
-        with self._mpd as client:
+        async with self._mpd as client:
             try:
-                albumart = client.albumart(filename)
+                albumart = await client.albumart(filename)
             except CommandError as exc:
                 raise HTTPError(404, 'Cover art not found') from exc
 
         data = albumart['binary']
         mime = magic.from_buffer(data, mime=True)
 
         self.write(data)
         self.set_header('content-type', mime)
 
 
-def _read_resource(dir_, filename):
+def _read_resource(dir_: str, filename: str) -> str:
     src = resources.files(fookebox).joinpath(dir_).joinpath(filename)
     with resources.as_file(src) as path:
         with open(path, 'r', encoding='utf-8') as file:
             return file.read()
 
 
-def _read_binary_resource(dir_, filename):
+def _read_binary_resource(dir_: str, filename: str) -> bytes:
     src = resources.files(fookebox).joinpath(dir_).joinpath(filename)
     with resources.as_file(src) as path:
         with open(path, 'rb') as file:
             return file.read()
 
 
 class CSSHandler(RequestHandler):
     """A RequestHandler that serves CSS files from the package resources."""
     # pylint: disable=abstract-method
-    def get(self, filename: str):
+    def get(self, filename: str) -> None:
         """
         Get the a CSS file from the package resources.
 
         Parameters
         ----------
         filename : str
             name of the file
@@ -249,15 +241,15 @@
         self.set_header('content-type', 'text/css')
         self.write(data)
 
 
 class FontHandler(RequestHandler):
     """A RequestHandler that serves fonts from the package resources."""
     # pylint: disable=abstract-method
-    def get(self, filename: str):
+    def get(self, filename: str) -> None:
         """
         Get the a font from the package resources.
 
         Parameters
         ----------
         filename : str
             name of the font file
@@ -272,42 +264,42 @@
         self.write(data)
         self.set_header('content-type', mime)
 
 
 class IndexHandler(RequestHandler):
     """A RequestHandler that serves the index HTML file."""
     # pylint: disable=abstract-method
-    def initialize(self, mpd: MPDContext, cfg: SectionProxy):
+    def initialize(self, mpd: MPDContext, cfg: SectionProxy) -> None:
         """Initialize the IndexHandler object"""
         # pylint: disable=attribute-defined-outside-init
         self.mpd = mpd
         self.cfg = cfg
 
-    def get(self):
+    async def get(self) -> None:
         """
         Load the index HTML file.
 
         The HTML file comes pre-loaded with all available artists and genres,
         rendered in the browser's preferred language (if available).
         """
-        with self.mpd as client:
-            artists = [x['artist'] for x in client.list('artist')]
-            genres = [x['genre'] for x in client.list('genre')]
+        async with self.mpd as client:
+            artists = [x['artist'] for x in await client.list('artist')]
+            genres = [x['genre'] for x in await client.list('genre')]
 
         markup = _read_resource('templates', 'client.html')
         tpl = template.Template(markup)
         output = tpl.generate(config=self.cfg, artists=artists, genres=genres,
                               locale=self.get_browser_locale())
         self.write(output)
 
 
 class JSHandler(RequestHandler):
     """A RequestHandler that serves JavaScript from the package resources."""
     # pylint: disable=abstract-method
-    def get(self, filename: str):
+    def get(self, filename: str) -> None:
         """
         Get the a JavaScript file from the package resources.
 
         Parameters
         ----------
         filename : str
             name of the file
@@ -324,55 +316,36 @@
 class QueueHandler(RequestHandler):
     # pylint: disable=abstract-method
     """
     A RequestHandler that allows clients to interact with MPD's queue.
 
     Methods
     -------
-    get():
-        Get the current queue
     post():
         Add an arbitrary number of tracks to the queue
     delete():
         Remove a track from the queue
     """
-    def initialize(self, mpd: MPDContext, cfg: SectionProxy):
+    def initialize(self, mpd: MPDContext, cfg: SectionProxy) -> None:
         # pylint: disable=attribute-defined-outside-init
         """Initialize the QueueHandler object"""
         self._mpd = mpd
         self._cfg = cfg
 
-    def get(self):
-        """
-        Returns the currently queued tracks.
-
-        This does not include the track that is being played at the moment.
-        """
-        with self._mpd as client:
-            queue = client.playlistinfo()
-            status = client.status()
-
-        index = int(status.get('song', 0))
-        self.write({'queue': queue[index+1:]})
-
-    def post(self):
+    async def post(self) -> None:
         """
         Add tracks to the queue.
 
         A JSON-encoded list of tracks to be added to the queue is read from the
         POST body. The tracks are then added, one by one, to the queue until
         there are no more tracks left or the queue is full.
 
         The queue size is determined from the max_queue_length configuration
         option.
 
-        Returns
-        -------
-        This method does not return anything.
-
         Exceptions
         ----------
         - If the queue limit has been exceeded, a HTTP 409 error is raised.
         - If the supplied JSON data is invalid, a HTTP 400 error is raised.
         """
         try:
             data = json.loads(self.request.body)
@@ -381,82 +354,65 @@
 
         dir_ = data.get('files', [])
         maxlen = self._cfg.getint('max_queue_length')
 
         if not isinstance(dir_, list):
             raise HTTPError(400, 'Invalid data')
 
-        with self._mpd as client:
+        async with self._mpd as client:
             for file in dir_:
-                playlist = client.playlist()[1:]
+                playlist = list(await client.playlist())[1:]
                 if len(playlist) >= maxlen:
                     raise HTTPError(409, 'Queue full')
-                client.add(file)
+                await client.add(file)
 
-            client.play()
+            await client.play()
 
-    def delete(self, position: int):
+    async def delete(self, position: str) -> None:
         """
         Remove a track from the queue.
 
         The queue position of the track to be removed is expected to be passed
         in the URL.
 
         Removing tracks from the queue can be allowed / disallowed using the
         'enable_song_removal' configuration option.
 
         Parameters
         ----------
         position : int
             position in the queue to remove
 
-        Returns
-        -------
-        This method does not return anything.
-
         Exceptions
         ----------
         - If removing items from the queue has been disabled, a HTTP 403 error
           is raised.
         - If the supplied position is not valid, a HTTP 400 error is raised.
         """
         if not self._cfg.get('enable_song_removal'):
             raise HTTPError(403)
 
-        with self._mpd as client:
+        async with self._mpd as client:
             try:
-                client.delete(position)
+                await client.delete(int(position))
             except CommandError as exc:
                 raise HTTPError(400, str(exc)) from exc
 
 
-class StatusHandler(RequestHandler):
+class SocketHandler(WebSocketHandler, MPDSubscriber):
     # pylint: disable=abstract-method
     """
-    A RequestHandler that returns the current MPD status.
-
-    Methods
-    -------
-    get():
-        Get the current status
+    A WebSocketHandler for clients that wish to receive status updates.
     """
-    def initialize(self, mpd: MPDContext):
+    def initialize(self, idle: IdleSocket) -> None:
         # pylint: disable=attribute-defined-outside-init
-        """Initialize the StatusHandler object"""
-        self._mpd = mpd
+        """Initialize the SocketHandler object"""
+        self._idle = idle
 
-    def get(self):
-        """
-        Returns the current MPD status.
-
-        This includes the currently playing song as well as the length of the
-        queue.
-        """
-        with self._mpd as client:
-            status = client.status()
-            status.update(client.currentsong())
-            status.update({'queueLength': len(client.playlist())})
+    def open(self, *args: str, **kwargs: str) -> None:
+        self._idle.subscribe(self)
 
-        if 'pos' in status:
-            status['queueLength'] -= int(status['pos'])+1
+    def on_close(self) -> None:
+        self._idle.unsubscribe(self)
 
-        self.write(status)
+    async def update(self, message: dict) -> None:
+        self.write_message(json.dumps(message))
```

### Comparing `fookebox-1.0.0/src/fookebox/i18n/de/LC_MESSAGES/fookebox.mo` & `fookebox-1.0.1/src/fookebox/i18n/de/LC_MESSAGES/fookebox.mo`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/js/bootstrap.min.js` & `fookebox-1.0.1/src/fookebox/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/js/fookebox.js` & `fookebox-1.0.1/src/fookebox/js/fookebox.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU Affero General Public License for more details.
  *
  * You should have received a copy of the GNU Affero General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-/* HTML elements */
+/* global _ */
 
 function PlayAlbumButton(album) {
     var div = document.createElement("div");
     div.classList.add("pull-right");
 
     var button = document.createElement("button");
     button.classList.add("btn");
@@ -33,16 +33,16 @@
     span.classList.add("glyphicon");
     span.classList.add("glyphicon-play");
     button.append(span);
 
     var text = " " + _("Play album");
     button.append(text);
 
-    div.onclick = function(event) {
-        album.play()
+    div.onclick = function() {
+        album.play();
     };
 
     return div;
 }
 
 function AlbumHeader(album, enablePlayAlbum) {
     var div = document.createElement("div");
@@ -79,26 +79,26 @@
 
     var list = document.createElement("ul");
     list.classList.add("list-unstyled");
     body.append(list);
 
     for (var i = 0; i < tracks.length; i++) {
         var track = tracks[i];
-        list.append(new Track(track, jukebox))
+        list.append(new Track(track, jukebox));
     }
 
     return body;
 }
 
 function Track(t, jukebox) {
     var li = document.createElement("li");
 
     var link = document.createElement("a");
     link.href = "#";
-    link.innerHTML = `${t.track} &ndash; ${t.artist} &ndash; ${t.title}`
+    link.innerHTML = `${t.track} &ndash; ${t.artist} &ndash; ${t.title}`;
     li.append(link);
 
     link.onclick = function(event) {
         event.preventDefault();
         jukebox.play([t]);
     };
 
@@ -127,33 +127,31 @@
 
 AlbumCover.prototype.load = function(target) {
     const file = encodeRFC3986URIComponent(this.album.tracks[0].file);
     const url = `cover/${file}`;
 
     const req = $.ajax(url);
 
-    req.done(function(data) {
+    req.done(function() {
         target.style.backgroundImage = `url(${url})`;
     });
-    req.fail(function(data) {
+    req.fail(function() {
         target.classList.add("no-cover");
     });
-}
-
-/* End of HTML elements */
+};
 
 function WindowHandler(jukebox) {
     this.jukebox = jukebox;
     this.skipval = null;
 
     $(window).on("hashchange", $.proxy(this.loadhash, this));
     this.loadhash(this);
 }
 
-WindowHandler.prototype.loadhash = function(e) {
+WindowHandler.prototype.loadhash = function() {
     var hash = window.location.hash;
 
     if (!hash) {
         this.jukebox.showSearch();
         return;
     }
 
@@ -173,43 +171,38 @@
 
     this.jukebox.showItems(key, val);
 
     if (key == 'artist')
         $('#showArtists').tab('show');
     else if (key == 'genre')
         $('#showGenres').tab('show');
-}
+};
 
 WindowHandler.prototype.skip = function(val) {
     this.skipval = val;
-}
+};
 
 function QueueView() {
     var getMaxLength = function() {
         return $('#queue').find('li').length;
-    }
+    };
 
     var getCurrentLength = function() {
         return $('#queue').find('li:not(.disabled)').length;
-    }
+    };
 
     Object.defineProperty(this, 'maxLength', {
         get: getMaxLength
     });
 
     Object.defineProperty(this, 'currentLength', {
         get: getCurrentLength
     });
 }
 
-QueueView.prototype.update = function() {
-    var req = $.get('queue');
-    req.done($.proxy(this.load, this));
-}
-
 QueueView.prototype.updateLabel = function(flash) {
     var len = this.currentLength;
     var qlen = this.maxLength;
     var label = $('#queueStatus');
 
     if (len == qlen) {
         label.text(_('full'));
@@ -227,35 +220,31 @@
         label.removeClass('label-warning');
         label.addClass('label-info');
     }
 
     if (flash) {
         this.pulsate();
     }
-}
+};
 
 QueueView.prototype.pulsate = function() {
     var label = $('#queueStatus');
     label.hide();
     label.show('highlight');
-}
+};
 
 QueueView.prototype.delete = function(i) {
-    return function(event) {
-        var req = $.ajax("queue/" + (i + 1), {
+    return function() {
+        $.ajax("queue/" + (i + 1), {
             "type": "DELETE",
         });
 
-        req.done($.proxy(function() {
-            this.update();
-        }, this));
-
         return false;
     }.bind(this);
-}
+};
 
 QueueView.prototype.load = function(data) {
     if (!("queue" in data)) {
         return;
     }
 
     var len = data.queue.length;
@@ -268,61 +257,61 @@
 
         link.off("click");
 
         if (i >= len) {
             el.addClass("disabled");
             link.find(".artist").text("");
             link.find(".title").text("");
-            link.click(function(event) {
-                return false
+            link.click(function() {
+                return false;
             });
             continue;
         }
 
         var track = data.queue[i];
         link.find(".artist").text(track.artist);
         link.find(".title").text(track.title);
         el.removeClass("disabled");
 
         if (el.find("span.controls").length > 0) {
             link.click(this.delete(i));
         } else {
-            link.click(function(event) {
-                return false
+            link.click(function() {
+                return false;
             });
         }
     }
 
     this.updateLabel(len != prevlen);
-}
+};
 
 function AlbumList() {
     this.albums = new Object();
 }
 
 AlbumList.prototype.contains = function(album) {
     return (album.hash() in this.albums);
-}
+};
 
 AlbumList.prototype.add = function(album) {
     this.albums[album.hash()] = album;
-}
+};
 
 AlbumList.prototype.get = function(album) {
     return this.albums[album.hash()];
-}
+};
 
 AlbumList.prototype.sortAll = function() {
     for (var key in this.albums) {
         var album = this.albums[key];
         album.sort(function(a, b) {
             return Number(a.track) - Number(b.track);
         });
     }
-}
+};
 
 AlbumList.prototype.render = function() {
     var queueAlbums = false;
     var albums = new Array();
     var body = $("body");
 
     if (body.attr("queue-albums")) {
@@ -336,66 +325,66 @@
     albums.sort(function(a, b) {
         return a.name > b.name;
     });
 
     $(albums).each(function(i, album) {
         album.render(queueAlbums);
     });
-}
+};
 
 function Album(jukebox, path, name) {
     this.jukebox = jukebox;
     this.path = path;
     this.name = name;
     this.artist = '';
     this.tracks = new Array();
 }
 
 Album.prototype.hash = function() {
     return btoa(escape('' + this.name + this.path));
-}
+};
 
 Album.prototype.add = function(track) {
     this.tracks.push(track);
 
     if (this.artist == '') {
         this.artist = track.artist;
     } else if ((this.artist.indexOf(track.artist) < 0) &&
         (track.artist.indexOf(this.artist) < 0)) {
         this.artist = _('Various artists');
     }
-}
+};
 
 Album.prototype.sort = function(f) {
     this.tracks.sort(f);
-}
+};
 
-Album.prototype.play = function(f) {
+Album.prototype.play = function() {
     this.jukebox.play(this.tracks);
-}
+};
 
 Album.prototype.render = function(enablePlayAlbum) {
     $('#result').append(new AlbumHeader(this, enablePlayAlbum));
     $('#result').append(new TrackList(this.tracks, this.jukebox));
-}
+};
 
 function SearchResult(jukebox, tracks) {
     this.tracks = tracks;
     this.jukebox = jukebox;
     this.albums = new AlbumList();
 
     function tracknum(input) {
         if ((input == '') || !input)
             return '00';
         else if (input.indexOf('/') >= 0)
             return tracknum(input.replace(/\/.*/, ''));
         else if (input.length < 2)
             return '0' + input;
         else
-            return input
+            return input;
     }
 
     function mkstring(input, type) {
         if (typeof input == "string") {
             return input;
         } else if (typeof input == "object") {
             if (input.length > 0)
@@ -432,67 +421,104 @@
         }
 
         album = this.albums.get(album);
         album.add(track);
     }, this));
 
     this.albums.sortAll();
-}
+};
 
 SearchResult.prototype.show = function() {
     $('#result').empty();
     this.albums.render();
+};
+
+function FookeboxSocket() {
+    const hostname = window.location.hostname;
+    const port = window.location.port;
+    this._url = `ws://${hostname}:${port}/socket`;
 }
 
+FookeboxSocket.prototype.listen = function(client) {
+    this._sock = new WebSocket(this._url);
+    this._sock.addEventListener('close', () => {
+        setTimeout(this.listen.bind(this), 1000, client);
+        console.log('Connection lost, reconnecting');
+    });
+    this._sock.addEventListener('message', (event) => {
+        var data = JSON.parse(event.data);
+        client.notify(data);
+    });
+};
+
 function Jukebox() {
     this.queue = new QueueView();
-    this.queue.update();
+    this._state = 'stop';
 }
 
 Jukebox.prototype.showSearch = function() {
     $('.navbar-toggle').removeClass('hidden-xs');
     $('.sidebar').removeClass('hidden-xs');
     $('.main').addClass('hidden-xs');
-}
+};
 
 Jukebox.prototype.showResult = function() {
     $('.navbar-toggle').addClass('hidden-xs');
     $('.sidebar').addClass('hidden-xs');
     $('.main').removeClass('hidden-xs');
     window.scrollTo(0, 0);
     $('.main').scrollTop(0);
-}
+};
 
 Jukebox.prototype.sync = function() {
-    window.setTimeout($.proxy(this.sync, this), 1000);
+    const sock = new FookeboxSocket();
+    sock.listen(this);
+};
+
+Jukebox.prototype.notify = function(data) {
+    const status = data.status;
+    if (status) {
+        if (status.state) {
+            this._state = status.state;
+        }
+    }
 
-    var req = $.get('status');
-    req.done($.proxy(function(data) {
+    let playlist = data.playlistinfo;
+
+    if (playlist) {
+        const queue = playlist.splice(1);
+        this.updatePlayer(playlist.pop());
+        this.queue.load({
+            'queue': queue
+        });
+    }
+};
+
+Jukebox.prototype.updatePlayer = function(data) {
+    if (data) {
         if ('artist' in data) {
             $('.currentArtist').text(data.artist);
-        } else if (data.state == 'play') {
+        } else if (this._state == 'play') {
             $('.currentArtist').text(_('Unknown artist'));
         } else {
             $('.currentArtist').empty();
         }
 
         if ('title' in data) {
             $('.currentTitle').text(data.title);
-        } else if (data.state == 'play') {
+        } else if (this._state == 'play') {
             $('.currentTitle').text(_('Unnamed track'));
         } else {
             $('.currentTitle').empty();
         }
-
-        if ('queueLength' in data) {
-            if (data.queueLength != this.queue.currentLength)
-                this.queue.update();
-        }
-    }, this));
-}
+    } else {
+        $('.currentArtist').empty();
+        $('.currentTitle').empty();
+    }
+};
 
 Jukebox.prototype.showItems = function(type, name) {
     const name_encoded = encodeRFC3986URIComponent(name);
     const req = $.getJSON(type + "/" + name_encoded);
 
     const well = $('<div class="well"></div>');
     well.text(_("Loading, please wait..."));
@@ -509,65 +535,61 @@
         const result = new SearchResult(this, data.tracks);
         result.show();
     }, this));
 
     req.fail(function() {
         console.error("failed");
     });
-}
+};
 
 Jukebox.prototype.play = function(tracks) {
     var files = tracks.map(function(obj) {
-        return obj.file
+        return obj.file;
     });
 
     var req = $.ajax("queue", {
         "data": JSON.stringify({
             "files": files
         }),
         "type": "POST",
         "processData": false,
         "contentType": "application/json"
     });
 
-    req.done($.proxy(function() {
-        this.queue.update();
-    }, this));
-
     req.error($.proxy(function(data) {
         switch (data.status) {
             case 409:
                 this.queue.pulsate();
                 break;
             default:
                 console.error(data);
         }
     }, this));
-}
+};
 
 Jukebox.prototype.showGenre = function(name) {
     this.showItems('genre', name);
-}
+};
 
 Jukebox.prototype.showArtist = function(name) {
     this.showItems('artist', name);
-}
+};
 
 Jukebox.prototype.control = function(action) {
     var data = {
         'action': action
     };
 
     $.ajax({
         url: 'control',
         type: 'POST',
         data: JSON.stringify(data),
         contentType: 'application/json; charset=utf-8'
     });
-}
+};
 
 $(document).ready(function() {
     function filter(list) {
         return function(event) {
             var el = $(event.currentTarget);
             var val = el.val().toLowerCase();
 
@@ -576,34 +598,34 @@
                 var text = link.text().toLowerCase();
 
                 if (text.indexOf(val) > -1)
                     link.show();
                 else
                     link.hide();
             });
-        }
-    };
+        };
+    }
 
     function noop(event) {
         event.preventDefault();
-    };
+    }
 
     function show(hashPrefix, showFunc) {
         return function(event) {
             event.preventDefault();
 
             const target = $(event.target);
             const val = target.data('value');
             const hash = hashPrefix + encodeRFC3986URIComponent(val);
             wh.skip(hash);
             window.location.hash = hash;
 
             showFunc(val);
         };
-    };
+    }
 
     var jukebox = new Jukebox();
     jukebox.sync();
 
     var wh = new WindowHandler(jukebox);
 
     $('#artistSearch').keyup(filter($('li.artist')));
```

### Comparing `fookebox-1.0.0/src/fookebox/js/i18n-de.js` & `fookebox-1.0.1/src/fookebox/js/i18n-de.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU Affero General Public License for more details.
  *
  * You should have received a copy of the GNU Affero General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-var i18n = {
+window.i18n = {
     'Unknown artist': 'Unbekannter Künstler',
     'Unnamed track': 'Unbekanntes Stück',
     'Various artists': 'Verschiedene Künstler',
     'empty': 'leer',
     'full': 'voll',
     'Play album': 'Album abspielen'
 };
```

### Comparing `fookebox-1.0.0/src/fookebox/js/i18n.js` & `fookebox-1.0.1/src/fookebox/js/i18n.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -13,13 +13,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU Affero General Public License for more details.
  *
  * You should have received a copy of the GNU Affero General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-function _(s) {
+/* global i18n */
+
+window._ = function(s) {
     if (typeof(i18n) != 'undefined' && i18n[s]) {
         return i18n[s];
     }
     return s;
-}
+};
```

### Comparing `fookebox-1.0.0/src/fookebox/js/jquery-1.12.4.min.js` & `fookebox-1.0.1/src/fookebox/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/js/jquery-ui.min.js` & `fookebox-1.0.1/src/fookebox/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox/templates/client.html` & `fookebox-1.0.1/src/fookebox/templates/client.html`

 * *Files identical despite different names*

### Comparing `fookebox-1.0.0/src/fookebox.egg-info/PKG-INFO` & `fookebox-1.0.1/src/fookebox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fookebox
-Version: 1.0.0
+Version: 1.0.1
 Summary: A jukebox-style web-frontend to mpd
 Home-page: https://code.ott.net/fookebox/
 Author: Stefan Ott
 Author-email: stefan@ott.net
 Project-URL: Source, https://git.ott.net/fookebox/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `fookebox-1.0.0/src/fookebox.egg-info/SOURCES.txt` & `fookebox-1.0.1/src/fookebox.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 src/fookebox/__init__.py
 src/fookebox/autoqueue.py
 src/fookebox/config.py
 src/fookebox/fookebox.py
 src/fookebox/handlers.py
 src/fookebox/mpd.py
 src/fookebox/py.typed
+src/fookebox/tasks.py
+src/fookebox/util.py
 src/fookebox.egg-info/PKG-INFO
 src/fookebox.egg-info/SOURCES.txt
 src/fookebox.egg-info/dependency_links.txt
 src/fookebox.egg-info/entry_points.txt
 src/fookebox.egg-info/requires.txt
 src/fookebox.egg-info/top_level.txt
 src/fookebox/css/bootstrap.min.css
@@ -30,8 +32,9 @@
 src/fookebox/js/i18n.js
 src/fookebox/js/jquery-1.12.4.min.js
 src/fookebox/js/jquery-ui.min.js
 src/fookebox/templates/client.html
 tests/test_auto_queue.py
 tests/test_config.py
 tests/test_handlers.py
+tests/test_mpd_interface.py
 tests/test_template.py
```

### Comparing `fookebox-1.0.0/tests/test_config.py` & `fookebox-1.0.1/tests/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,108 @@
 """
 Test the configuration loader.
 
 The loader is responsible for loading the fookebox configuration file and for
 providing reasonable default values.
 """
+
+from unittest import TestCase
 from fookebox.config import load_config, default_config
 
 
-class TestConfigLoader:
+class TestConfigLoader(TestCase):
     # pylint: disable=missing-class-docstring
-    def test_load_empty_config(self):
+    def test_load_empty_config(self) -> None:
         """Load an empty configuration file. All values should be set."""
         cfg = load_config('tests/fixtures/config-empty.ini')
 
-        assert cfg.get('site_name') == "fookebox"
-        assert cfg.getint('listen_port') == 8888
-        assert cfg.get('mpd_host') == "localhost"
-        assert cfg.getint('mpd_port') == 6600
-        assert cfg.get('mpd_pass') is None
-        assert cfg.getint('max_queue_length') == 5
-        assert cfg.getboolean('auto_queue') is True
-        assert cfg.getint('auto_queue_time_left') == 3
-        assert cfg.get('auto_queue_playlist') is None
-        assert cfg.get('auto_queue_genre') is None
-        assert cfg.getboolean('show_search') is True
-        assert cfg.getboolean('enable_controls') is True
-        assert cfg.getboolean('enable_song_removal') is True
-        assert cfg.getboolean('enable_queue_album') is True
+        self.assertEqual(cfg.get('site_name'), "fookebox")
+        self.assertEqual(cfg.getint('listen_port'), 8888)
+        self.assertEqual(cfg.get('mpd_host'), "localhost")
+        self.assertEqual(cfg.getint('mpd_port'), 6600)
+        self.assertIsNone(cfg.get('mpd_pass'))
+        self.assertEqual(cfg.getint('max_queue_length'), 5)
+        self.assertTrue(cfg.getboolean('auto_queue'))
+        self.assertEqual(cfg.getint('auto_queue_time_left'), 3)
+        self.assertIsNone(cfg.get('auto_queue_playlist'))
+        self.assertIsNone(cfg.get('auto_queue_genre'))
+        self.assertTrue(cfg.getboolean('show_search'))
+        self.assertTrue(cfg.getboolean('enable_controls'))
+        self.assertTrue(cfg.getboolean('enable_song_removal'))
+        self.assertTrue(cfg.getboolean('enable_queue_album'))
 
-    def test_load_config_without_fookebox_section(self):
+    def test_load_config_without_fookebox_section(self) -> None:
         """Load a configuration file without a fookebox section.
            All values should be set."""
         cfg = load_config('tests/fixtures/config-no-fookebox-section.ini')
 
-        assert cfg.get('site_name') == "fookebox"
-        assert cfg.getint('listen_port') == 8888
-        assert cfg.get('mpd_host') == "localhost"
-        assert cfg.getint('mpd_port') == 6600
-        assert cfg.get('mpd_pass') is None
-        assert cfg.getint('max_queue_length') == 5
-        assert cfg.getboolean('auto_queue') is True
-        assert cfg.getint('auto_queue_time_left') == 3
-        assert cfg.get('auto_queue_playlist') is None
-        assert cfg.get('auto_queue_genre') is None
-        assert cfg.getboolean('show_search') is True
-        assert cfg.getboolean('enable_controls') is True
-        assert cfg.getboolean('enable_song_removal') is True
-        assert cfg.getboolean('enable_queue_album') is True
+        self.assertEqual(cfg.get('site_name'), "fookebox")
+        self.assertEqual(cfg.getint('listen_port'), 8888)
+        self.assertEqual(cfg.get('mpd_host'), "localhost")
+        self.assertEqual(cfg.getint('mpd_port'), 6600)
+        self.assertIsNone(cfg.get('mpd_pass'))
+        self.assertEqual(cfg.getint('max_queue_length'), 5)
+        self.assertTrue(cfg.getboolean('auto_queue'))
+        self.assertEqual(cfg.getint('auto_queue_time_left'), 3)
+        self.assertIsNone(cfg.get('auto_queue_playlist'))
+        self.assertIsNone(cfg.get('auto_queue_genre'))
+        self.assertTrue(cfg.getboolean('show_search'))
+        self.assertTrue(cfg.getboolean('enable_controls'))
+        self.assertTrue(cfg.getboolean('enable_song_removal'))
+        self.assertTrue(cfg.getboolean('enable_queue_album'))
 
-    def test_load_default_config(self):
+    def test_load_default_config(self) -> None:
         """Load default settings"""
         cfg = default_config()
 
-        assert cfg.get('site_name') == "fookebox"
-        assert cfg.getint('listen_port') == 8888
-        assert cfg.get('mpd_host') == "localhost"
-        assert cfg.getint('mpd_port') == 6600
-        assert cfg.get('mpd_pass') is None
-        assert cfg.getint('max_queue_length') == 5
-        assert cfg.getboolean('auto_queue') is True
-        assert cfg.getint('auto_queue_time_left') == 3
-        assert cfg.get('auto_queue_playlist') is None
-        assert cfg.get('auto_queue_genre') is None
-        assert cfg.getboolean('show_search') is True
-        assert cfg.getboolean('enable_controls') is True
-        assert cfg.getboolean('enable_song_removal') is True
-        assert cfg.getboolean('enable_queue_album') is True
+        self.assertEqual(cfg.get('site_name'), "fookebox")
+        self.assertEqual(cfg.getint('listen_port'), 8888)
+        self.assertEqual(cfg.get('mpd_host'), "localhost")
+        self.assertEqual(cfg.getint('mpd_port'), 6600)
+        self.assertIsNone(cfg.get('mpd_pass'))
+        self.assertEqual(cfg.getint('max_queue_length'), 5)
+        self.assertTrue(cfg.getboolean('auto_queue'))
+        self.assertEqual(cfg.getint('auto_queue_time_left'), 3)
+        self.assertIsNone(cfg.get('auto_queue_playlist'))
+        self.assertIsNone(cfg.get('auto_queue_genre'))
+        self.assertTrue(cfg.getboolean('show_search'))
+        self.assertTrue(cfg.getboolean('enable_controls'))
+        self.assertTrue(cfg.getboolean('enable_song_removal'))
+        self.assertTrue(cfg.getboolean('enable_queue_album'))
 
-    def test_load_some_config(self):
+    def test_load_some_config(self) -> None:
         """Load a configuration file. All values should be set."""
         cfg = load_config('tests/fixtures/config-example-1.ini')
 
-        assert cfg.get('site_name') == "test site 1"
-        assert cfg.getint('listen_port') == 8889
-        assert cfg.get('mpd_host') == "test host"
-        assert cfg.getint('mpd_port') == 612
-        assert cfg.get('mpd_pass') == "test password"
-        assert cfg.getint('max_queue_length') == 7
-        assert cfg.getboolean('auto_queue') is True
-        assert cfg.getint('auto_queue_time_left') == 19
-        assert cfg.get('auto_queue_playlist') == "idle"
-        assert cfg.get('auto_queue_genre') == "Jazz"
-        assert cfg.getboolean('show_search') is True
-        assert cfg.getboolean('enable_controls') is True
-        assert cfg.getboolean('enable_song_removal') is True
-        assert cfg.getboolean('enable_queue_album') is True
+        self.assertEqual(cfg.get('site_name'), "test site 1")
+        self.assertEqual(cfg.getint('listen_port'), 8889)
+        self.assertEqual(cfg.get('mpd_host'), "test host")
+        self.assertEqual(cfg.getint('mpd_port'), 612)
+        self.assertEqual(cfg.get('mpd_pass'), "test password")
+        self.assertEqual(cfg.getint('max_queue_length'), 7)
+        self.assertTrue(cfg.getboolean('auto_queue'))
+        self.assertEqual(cfg.getint('auto_queue_time_left'), 19)
+        self.assertEqual(cfg.get('auto_queue_playlist'), "idle")
+        self.assertEqual(cfg.get('auto_queue_genre'), "Jazz")
+        self.assertTrue(cfg.getboolean('show_search'))
+        self.assertTrue(cfg.getboolean('enable_controls'))
+        self.assertTrue(cfg.getboolean('enable_song_removal'))
+        self.assertTrue(cfg.getboolean('enable_queue_album'))
 
-    def test_load_other_config(self):
+    def test_load_other_config(self) -> None:
         """Load a different configuration file. All values should be set."""
         cfg = load_config('tests/fixtures/config-example-2.ini')
 
-        assert cfg.get('site_name') == "test site 2"
-        assert cfg.getint('listen_port') == 8890
-        assert cfg.get('mpd_host') == "mpd host"
-        assert cfg.getint('mpd_port') == 613
-        assert cfg.get('mpd_pass') == "password"
-        assert cfg.getint('max_queue_length') == 6
-        assert cfg.getboolean('auto_queue') is False
-        assert cfg.getint('auto_queue_time_left') == 20
-        assert cfg.get('auto_queue_playlist') == "playlist"
-        assert cfg.get('auto_queue_genre') == "Rock & Roll"
-        assert cfg.getboolean('show_search') is False
-        assert cfg.getboolean('enable_controls') is False
-        assert cfg.getboolean('enable_song_removal') is False
-        assert cfg.getboolean('enable_queue_album') is False
+        self.assertEqual(cfg.get('site_name'), "test site 2")
+        self.assertEqual(cfg.getint('listen_port'), 8890)
+        self.assertEqual(cfg.get('mpd_host'), "mpd host")
+        self.assertEqual(cfg.getint('mpd_port'), 613)
+        self.assertEqual(cfg.get('mpd_pass'), "password")
+        self.assertEqual(cfg.getint('max_queue_length'), 6)
+        self.assertFalse(cfg.getboolean('auto_queue'))
+        self.assertEqual(cfg.getint('auto_queue_time_left'), 20)
+        self.assertEqual(cfg.get('auto_queue_playlist'), "playlist")
+        self.assertEqual(cfg.get('auto_queue_genre'), "Rock & Roll")
+        self.assertFalse(cfg.getboolean('show_search'))
+        self.assertFalse(cfg.getboolean('enable_controls'))
+        self.assertFalse(cfg.getboolean('enable_song_removal'))
+        self.assertFalse(cfg.getboolean('enable_queue_album'))
```

### Comparing `fookebox-1.0.0/tests/test_template.py` & `fookebox-1.0.1/tests/test_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,175 +1,188 @@
 """
 Test the page template. Make sure it handles translations and configuration
 settings correctly.
 """
 from importlib import resources
+from typing import Optional, Union
+from unittest import TestCase
 
 from bs4 import BeautifulSoup
 from tornado import locale
 from tornado.template import Template
 
 import fookebox
 
 from tests.common import ConfigWrapper
 
 
-def _load_resource(dir_, filename):
+def _load_resource(dir_: str, filename: str) -> str:
     res = resources.files(fookebox).joinpath(dir_)
     with resources.as_file(res) as path:
-        src = resources.files(fookebox).joinpath(path).joinpath(filename)
+        src = resources.files(fookebox).joinpath(str(path)).joinpath(filename)
         with resources.as_file(src) as path:
             with open(path, 'r', encoding='utf-8') as file:
                 return file.read()
 
 
 class MockLocale:
     # pylint: disable=too-few-public-methods
     """
     This class is used as a basic no-op locale mock in tests where the locale
     does not matter.
     """
-    def __init__(self, code="xx"):
+    def __init__(self, code: str = "xx"):
         self.code = code
 
-    def translate(self, val):
+    @staticmethod
+    def translate(val: str) -> str:
         # pylint: disable=missing-function-docstring
         return val
 
 
-class TestTemplate:
+class TestTemplate(TestCase):
     """
     Here we test the page template. The template can show/hide different
     controls based on the configuration.
     """
-    def render(self, *, cfg, loc=MockLocale(), artists=None, genres=None):
+    @staticmethod
+    def render(cfg: ConfigWrapper,
+               loc: Union[locale.Locale, MockLocale] = MockLocale(),
+               artists: Optional[list[str]] = None,
+               genres: Optional[list[str]] = None) -> BeautifulSoup:
         """Render the page template. This is used by other tests"""
         markup = _load_resource('templates', 'client.html')
         template = Template(markup)
 
         artists = artists or []
         genres = genres or []
 
         html = template.generate(config=cfg, locale=loc, artists=artists,
                                  genres=genres)
         return BeautifulSoup(html, 'html.parser')
 
-    def test_show_search(self):
+    def test_show_search(self) -> None:
         """Show the search form if 'show_search' has been enabled"""
         config = ConfigWrapper()
         config.set('show_search', True)
         soup = self.render(cfg=config)
 
-        assert soup.find("form", {"id": "artistSearchForm"}) is not None
-        assert soup.find("form", {"id": "genreSearchForm"}) is not None
+        self.assertIsNotNone(soup.find("form", {"id": "artistSearchForm"}))
+        self.assertIsNotNone(soup.find("form", {"id": "genreSearchForm"}))
 
-    def test_hide_search(self):
+    def test_hide_search(self) -> None:
         """Hide the search form if 'show_search' has not been enabled"""
         config = ConfigWrapper()
         config.set('show_search', False)
         soup = self.render(cfg=config)
 
-        assert soup.find("form", {"id": "artistSearchForm"}) is None
-        assert soup.find("form", {"id": "genreSearchForm"}) is None
+        self.assertIsNone(soup.find("form", {"id": "artistSearchForm"}))
+        self.assertIsNone(soup.find("form", {"id": "genreSearchForm"}))
 
-    def test_site_name(self):
+    def test_site_name(self) -> None:
         """Use the site_name as page title"""
         config = ConfigWrapper()
         config.set('site_name', 'test 51')
         soup = self.render(cfg=config)
-        assert soup.find("title").text == "test 51"
+        title = soup.find('title')
+        self.assertEqual(title.text, 'test 51')                 # type: ignore
 
         config.set('site_name', 'other test')
         soup = self.render(cfg=config)
-        assert soup.find("title").text == "other test"
+        title = soup.find('title')
+        self.assertEqual(title.text, 'other test')              # type: ignore
 
-    def test_enable_controls(self):
+    def test_enable_controls(self) -> None:
         """Show the control panel controls have been enabled"""
         config = ConfigWrapper()
         config.set('enable_controls', True)
         soup = self.render(cfg=config)
-        assert soup.find("div", {"id": "controls"}) is not None
+        self.assertIsNotNone(soup.find("div", {"id": "controls"}))
 
-    def test_disable_controls(self):
+    def test_disable_controls(self) -> None:
         """Hide the control panel controls have not been enabled"""
         config = ConfigWrapper()
         config.set('enable_controls', False)
         soup = self.render(cfg=config)
-        assert soup.find("div", {"id": "controls"}) is None
+        self.assertIsNone(soup.find("div", {"id": "controls"}))
 
-    def test_locale_de(self):
+    def test_locale_de(self) -> None:
         """Use the German translation"""
         res = resources.files(fookebox).joinpath('i18n')
         with resources.as_file(res) as dir_:
             locale.load_gettext_translations(str(dir_), domain='fookebox')
 
         soup = self.render(loc=locale.get('de'), cfg=ConfigWrapper())
         link = soup.find("a", {"id": "showArtists"})
-        assert link.text == "Künstler"
+        self.assertEqual(link.text, 'Künstler')                 # type: ignore
 
-    def test_locale_en(self):
+    def test_locale_en(self) -> None:
         """Use the English language version"""
         res = resources.files(fookebox).joinpath('i18n')
         with resources.as_file(res) as dir_:
             locale.load_gettext_translations(str(dir_), domain='fookebox')
 
         soup = self.render(loc=locale.get('en'), cfg=ConfigWrapper())
         link = soup.find("a", {"id": "showArtists"})
-        assert link.text == "Artists"
+        self.assertEqual(link.text, 'Artists')                  # type: ignore
 
-    def test_locale_fallback_unknown(self):
+    def test_locale_fallback_unknown(self) -> None:
         """Use English as a fallback for unknown languages"""
         res = resources.files(fookebox).joinpath('i18n')
         with resources.as_file(res) as dir_:
             locale.load_gettext_translations(str(dir_), domain='fookebox')
 
         soup = self.render(loc=locale.get('fr'), cfg=ConfigWrapper())
         link = soup.find("a", {"id": "showArtists"})
-        assert link.text == "Artists"
+        self.assertEqual(link.text, 'Artists')                  # type: ignore
 
-    def test_enable_song_removal(self):
+    def test_enable_song_removal(self) -> None:
         """Show the song removal links if song removal has been enabled"""
         config = ConfigWrapper()
         config.set('enable_song_removal', True)
 
         soup = self.render(cfg=config)
         queue = soup.find("ul", {"id": "queue"})
-        assert queue.find("span", {"class": "controls"}) is not None
+        controls = queue.find("span", {"class": "controls"})    # type: ignore
+        self.assertIsNotNone(controls)
 
-    def test_disable_song_removal(self):
+    def test_disable_song_removal(self) -> None:
         """Hide the song removal links if song removal has not been enabled"""
         config = ConfigWrapper()
         config.set('enable_song_removal', False)
 
         soup = self.render(cfg=config)
         queue = soup.find("ul", {"id": "queue"})
-        assert queue.find("span", {"class": "controls"}) is None
+        controls = queue.find("span", {"class": "controls"})    # type: ignore
+        self.assertIsNone(controls)
 
-    def test_disable_queue_album(self):
+    def test_disable_queue_album(self) -> None:
         """Show the links to queue whole albums if enabled"""
         config = ConfigWrapper()
         config.set('enable_queue_album', False)
 
         soup = self.render(cfg=config)
         body = soup.find("body")
-        assert body.get("queue-albums") is None
+        self.assertIsNone(body.get("queue-albums"))             # type: ignore
 
-    def test_enable_queue_album(self):
+    def test_enable_queue_album(self) -> None:
         """Hide the links to queue whole albums if not enabled"""
         config = ConfigWrapper()
         config.set('enable_queue_album', True)
 
         soup = self.render(cfg=config)
         body = soup.find("body")
-        assert body.get("queue-albums") == "True"
+        self.assertEqual(body.get("queue-albums"), "True")      # type: ignore
 
-    def test_artists(self):
+    def test_artists(self) -> None:
         """Include the list of artists in the page"""
         soup = self.render(cfg=ConfigWrapper(), artists=['The KLF', 'Cher'])
         body = soup.find('body')
-        assert len(body.find_all('li', {'class': 'artist'})) == 2
+        artists = body.find_all('li', {'class': 'artist'})      # type: ignore
+        self.assertEqual(len(artists), 2)
 
-    def test_genres(self):
+    def test_genres(self) -> None:
         """Include the list of genres in the page"""
         soup = self.render(cfg=ConfigWrapper(), genres=['Jazz', 'Funk', 'IDM'])
         body = soup.find('body')
-        assert len(body.find_all('li', {'class': 'genre'})) == 3
+        genres = body.find_all('li', {'class': 'genre'})        # type: ignore
+        self.assertEqual(len(genres), 3)
```

