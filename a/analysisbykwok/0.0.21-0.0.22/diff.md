# Comparing `tmp/analysisbykwok-0.0.21.tar.gz` & `tmp/analysisbykwok-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.21.tar", last modified: Thu Apr 27 07:32:47 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.22.tar", last modified: Thu Apr 27 07:53:22 2023, max compression
```

## Comparing `analysisbykwok-0.0.21.tar` & `analysisbykwok-0.0.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/
--rw-rw-rw-   0        0        0       62 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/analysisbykwok/
--rw-rw-rw-   0        0        0    17177 2023-04-27 07:29:35.000000 analysisbykwok-0.0.21/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-23 02:44:45.000000 analysisbykwok-0.0.21/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-04-27 07:32:04.000000 analysisbykwok-0.0.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/
+-rw-rw-rw-   0        0        0       62 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/analysisbykwok/
+-rw-rw-rw-   0        0        0    17172 2023-04-27 07:52:46.000000 analysisbykwok-0.0.22/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-27 07:52:55.000000 analysisbykwok-0.0.22/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-04-27 07:52:55.000000 analysisbykwok-0.0.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/setup.cfg
```

### Comparing `analysisbykwok-0.0.21/analysisbykwok/__init__.py` & `analysisbykwok-0.0.22/analysisbykwok/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,18 +287,17 @@
                 title = subject[-1][0].decode(str(subject[-1][1]))
             elif type(subject[-1][0]) == str:
                 title = subject[-1][0]
             # print("title:", title)
             get_att(msg, dir)
     def ProgressBar(i, sum, printvalue):
         sys.stdout.write('\r')
-        sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100 + 1), ((int(i / sum * 100))) * '■',
+        sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100), ((int(i / sum * 100))) * '■',
                                               (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
         sys.stdout.flush()
-
     def GetPlateSon(num):
         if num == '':
             res = requests.get(r'https://hq.stock.sohu.com/pl/pl-1631.html?uid=1681655630543283qgz&548285357286').text
             res = json.loads(
                 res.split('PEAK_ODIA(')[1].split(')</script>')[0].replace('\'pllist\',', '').replace('\'', '"'))
             info = ''
             for son in res:
```

