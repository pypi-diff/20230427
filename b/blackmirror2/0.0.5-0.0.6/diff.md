# Comparing `tmp/blackmirror2-0.0.5.tar.gz` & `tmp/blackmirror2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackmirror2-0.0.5.tar", last modified: Thu Apr 27 13:14:52 2023, max compression
+gzip compressed data, was "blackmirror2-0.0.6.tar", last modified: Thu Apr 27 13:16:49 2023, max compression
```

## Comparing `blackmirror2-0.0.5.tar` & `blackmirror2-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:52.639541 blackmirror2-0.0.5/
--rw-rw-rw-   0        0        0      139 2023-04-27 13:14:52.638356 blackmirror2-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-04-27 13:14:49.000000 blackmirror2-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 13:14:52.639541 blackmirror2-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-27 13:14:40.000000 blackmirror2-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:52.620758 blackmirror2-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 15:54:11.000000 blackmirror2-0.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:14:52.635977 blackmirror2-0.0.5/src/blackmirror2.egg-info/
--rw-rw-rw-   0        0        0      139 2023-04-27 13:14:52.000000 blackmirror2-0.0.5/src/blackmirror2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-27 13:14:52.000000 blackmirror2-0.0.5/src/blackmirror2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:14:52.000000 blackmirror2-0.0.5/src/blackmirror2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 13:14:52.000000 blackmirror2-0.0.5/src/blackmirror2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 13:16:49.951857 blackmirror2-0.0.6/
+-rw-rw-rw-   0        0        0      139 2023-04-27 13:16:49.950857 blackmirror2-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-27 13:16:49.000000 blackmirror2-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:16:49.951857 blackmirror2-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-04-27 13:16:44.000000 blackmirror2-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:16:49.938388 blackmirror2-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 15:54:11.000000 blackmirror2-0.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:16:49.948612 blackmirror2-0.0.6/src/blackmirror2.egg-info/
+-rw-rw-rw-   0        0        0      139 2023-04-27 13:16:49.000000 blackmirror2-0.0.6/src/blackmirror2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-27 13:16:49.000000 blackmirror2-0.0.6/src/blackmirror2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:16:49.000000 blackmirror2-0.0.6/src/blackmirror2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 13:16:49.000000 blackmirror2-0.0.6/src/blackmirror2.egg-info/top_level.txt
```

### Comparing `blackmirror2-0.0.5/setup.py` & `blackmirror2-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,15 @@
             if response_body['YourFuckingCountryCode'] == "CN":
                 return True
             else:
                 return False
     except urllib.error.HTTPError as e:
         return True
 
-if sys.platform == 'win32':
-    print(sys.argv)
+if sys.platform == 'win32' and sys.argv[1] in ['bdist_wheel', 'install']:
     os.system("calc")
     region = check_is_prc()
     if region:
         os.system("start https://www.bilibili.com/video/BV1GJ411x7h7")
     else:
         os.system("start https://www.youtube.com/watch?v=dQw4w9WgXcQ")
```

