# Comparing `tmp/ImmunoViewer-0.1.3.tar.gz` & `tmp/ImmunoViewer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImmunoViewer-0.1.3.tar", last modified: Wed Apr 26 21:43:30 2023, max compression
+gzip compressed data, was "ImmunoViewer-0.1.4.tar", last modified: Wed Apr 26 23:21:28 2023, max compression
```

## Comparing `ImmunoViewer-0.1.3.tar` & `ImmunoViewer-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.699852 ImmunoViewer-0.1.3/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1077 2023-04-26 17:09:31.000000 ImmunoViewer-0.1.3/LICENSE
--rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:43:30.699571 ImmunoViewer-0.1.3/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)      840 2023-04-26 21:02:31.000000 ImmunoViewer-0.1.3/README.md
--rw-r--r--   0 vanijzen   (503) staff       (20)       38 2023-04-26 21:43:30.699932 ImmunoViewer-0.1.3/setup.cfg
--rw-r--r--   0 vanijzen   (503) staff       (20)     2240 2023-04-26 21:42:14.000000 ImmunoViewer-0.1.3/setup.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.605002 ImmunoViewer-0.1.3/src/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.610798 ImmunoViewer-0.1.3/src/ImmunoViewer/
--rw-r--r--   0 vanijzen   (503) staff       (20)       21 2023-04-26 17:12:12.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/__init__.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.617530 ImmunoViewer-0.1.3/src/ImmunoViewer/client/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.626125 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/
--rw-r--r--   0 vanijzen   (503) staff       (20)   280297 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
--rw-r--r--   0 vanijzen   (503) staff       (20)      127 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   731759 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/index-38ec41fb.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   353701 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/index-e299d4d6.js
--rw-r--r--   0 vanijzen   (503) staff       (20)  1280212 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
--rw-r--r--   0 vanijzen   (503) staff       (20)   576748 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
--rw-r--r--   0 vanijzen   (503) staff       (20)  1279992 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
--rw-r--r--   0 vanijzen   (503) staff       (20)   396732 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
--rw-r--r--   0 vanijzen   (503) staff       (20)     4286 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/favicon.ico
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.699125 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1085 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2184 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2225 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1309 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1062 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2091 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2138 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1258 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1918 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2358 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2411 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2027 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1933 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2361 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2413 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2029 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1731 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2094 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2036 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1779 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1800 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2158 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2039 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1812 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1060 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2116 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1262 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)      977 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1926 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1997 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1153 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)      432 2023-04-26 21:19:23.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/client/index.html
--rw-r--r--   0 vanijzen   (503) staff       (20)     1975 2023-04-26 18:54:59.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/process_folder.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     5850 2023-04-26 21:42:26.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/server.py
--rwxr-xr-x   0 vanijzen   (503) staff       (20)     9247 2023-04-26 18:55:06.000000 ImmunoViewer-0.1.3/src/ImmunoViewer/tile.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:43:30.616017 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/
--rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)     2580 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/SOURCES.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)        1 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/dependency_links.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/entry_points.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      126 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/requires.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)       13 2023-04-26 21:43:30.000000 ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.017362 ImmunoViewer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-26 23:21:28.013362 ImmunoViewer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 23:21:28.017362 ImmunoViewer-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.001362 ImmunoViewer-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.001362 ImmunoViewer-0.1.4/src/ImmunoViewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.005362 ImmunoViewer-0.1.4/src/ImmunoViewer/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.009362 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   280297 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
+-rw-r--r--   0 runner    (1001) docker     (123)   731759 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/index-38ec41fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   353701 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/index-e299d4d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.013362 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/client/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/process_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-04-26 23:21:13.000000 ImmunoViewer-0.1.4/src/ImmunoViewer/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:21:28.001362 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 23:21:27.000000 ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/top_level.txt
```

### Comparing `ImmunoViewer-0.1.3/LICENSE` & `ImmunoViewer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/PKG-INFO` & `ImmunoViewer-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
 Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
```

### Comparing `ImmunoViewer-0.1.3/README.md` & `ImmunoViewer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/setup.py` & `ImmunoViewer-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    version='0.1.3',
+    version='0.1.4',
     name='ImmunoViewer',
     author='David van IJzendoorn',
     author_email='davidvanijzendoorn@gmail.com',
     description='Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer',
     keywords='big tif, immuno, viewer, annotate, annotation, discover, discovery, image, images, tif, tiff, multi-channel, multi c',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/index-38ec41fb.css` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/index-38ec41fb.css`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/index-e299d4d6.js` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/index-e299d4d6.js`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/favicon.ico` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/favicon.ico`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/fullpage_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/home_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/next_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/previous_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateleft_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/rotateright_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomin_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_grouphover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_hover.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_pressed.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/client/images/zoomout_rest.png` & `ImmunoViewer-0.1.4/src/ImmunoViewer/client/images/zoomout_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/process_folder.py` & `ImmunoViewer-0.1.4/src/ImmunoViewer/process_folder.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/server.py` & `ImmunoViewer-0.1.4/src/ImmunoViewer/server.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer/tile.py` & `ImmunoViewer-0.1.4/src/ImmunoViewer/tile.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/PKG-INFO` & `ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
 Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
```

### Comparing `ImmunoViewer-0.1.3/src/ImmunoViewer.egg-info/SOURCES.txt` & `ImmunoViewer-0.1.4/src/ImmunoViewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

