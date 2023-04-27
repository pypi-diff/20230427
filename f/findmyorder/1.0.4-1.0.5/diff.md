# Comparing `tmp/findmyorder-1.0.4.tar.gz` & `tmp/findmyorder-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.4.tar", max compression
+gzip compressed data, was "findmyorder-1.0.5.tar", max compression
```

## Comparing `findmyorder-1.0.4.tar` & `findmyorder-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-26 20:37:37.263603 findmyorder-1.0.4/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-26 20:37:37.263603 findmyorder-1.0.4/README.md
--rw-r--r--   0        0        0      106 2023-04-26 20:37:38.483613 findmyorder-1.0.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3153 2023-04-26 20:37:37.263603 findmyorder-1.0.4/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-26 20:37:38.483613 findmyorder-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-26 21:17:25.450977 findmyorder-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-26 21:17:25.450977 findmyorder-1.0.5/README.md
+-rw-r--r--   0        0        0      106 2023-04-26 21:17:26.514984 findmyorder-1.0.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-26 21:17:25.450977 findmyorder-1.0.5/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-26 21:17:25.450977 findmyorder-1.0.5/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3164 2023-04-26 21:17:25.450977 findmyorder-1.0.5/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-26 21:17:26.514984 findmyorder-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.5/PKG-INFO
```

### Comparing `findmyorder-1.0.4/LICENSE` & `findmyorder-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.4/README.md` & `findmyorder-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.4/findmyorder/config.py` & `findmyorder-1.0.5/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.4/findmyorder/main.py` & `findmyorder-1.0.5/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,10 +81,10 @@
             # order['stoploss'] = 1000
             # order['takeprofit'] = {'tp1':1, 'tp2':10, 'tp3':100, 'tp4':1000, 'tp5':1000}
             # order['comments'] = 'findmyorder'
             
             return parsed_order
 
       except Exception as e:
-          self.logger.debug(f"error {e}")
-          return
+          self.logger.debug(f"error get order {e}")
+          #return
```

### Comparing `findmyorder-1.0.4/pyproject.toml` & `findmyorder-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.4"
+version = "1.0.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.0.4/PKG-INFO` & `findmyorder-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

