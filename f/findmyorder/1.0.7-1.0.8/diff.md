# Comparing `tmp/findmyorder-1.0.7.tar.gz` & `tmp/findmyorder-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.7.tar", max compression
+gzip compressed data, was "findmyorder-1.0.8.tar", max compression
```

## Comparing `findmyorder-1.0.7.tar` & `findmyorder-1.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-27 06:24:47.326810 findmyorder-1.0.7/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-27 06:24:47.326810 findmyorder-1.0.7/README.md
--rw-r--r--   0        0        0      106 2023-04-27 06:24:47.982813 findmyorder-1.0.7/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-27 06:24:47.326810 findmyorder-1.0.7/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-27 06:24:47.326810 findmyorder-1.0.7/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3422 2023-04-27 06:24:47.326810 findmyorder-1.0.7/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-27 06:24:47.982813 findmyorder-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-27 06:57:13.622135 findmyorder-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-27 06:57:13.622135 findmyorder-1.0.8/README.md
+-rw-r--r--   0        0        0      106 2023-04-27 06:57:14.362153 findmyorder-1.0.8/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3409 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-27 06:57:14.362153 findmyorder-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.8/PKG-INFO
```

### Comparing `findmyorder-1.0.7/LICENSE` & `findmyorder-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.7/README.md` & `findmyorder-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.7/findmyorder/config.py` & `findmyorder-1.0.8/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.7/findmyorder/main.py` & `findmyorder-1.0.8/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     def identify_order(self,mystring: str = None,):
       self.logger.debug(f"identify_order for {mystring}")
       try:
         #parsing
         action = oneOf("BUY SELL LONG SHORT")
         currency_pair = Word(alphas, exact=6)
         market = Optional(Word(alphas, exact=4))
-        leverage = Regex(r'Leverage: \w+ \((\d+(\.\d+)?X)\)')('leverage')
         percentage = Regex(r'\d+(\.\d+)?%')
-        quantity = Regex(r'\d+(\.\d+)?')('quantity')
+        # quantity = Regex(r'\d+(\.\d+)?')('quantity')
         # stop_loss = Regex(r'sl=\d+')['stop_loss']
         # take_profit1 = Regex(r'tp1=\d+')['take_profit1']
         # take_profit2 = Regex(r'tp2=\d+')['take_profit2']
+        # leverage = Regex(r'Leverage: \w+ \((\d+(\.\d+)?X)\)')
         # comment = Regex(r'comment=\w+')['comment']
 
         #order grammar
-        order_grammar = action('action') + currency_pair('currency_pair') + percentage('percentage') \
-                        + Optional(quantity)
+        order_grammar = action('action') + currency_pair('currency_pair') + percentage('percentage') 
+                        # + Optional(quantity)
                         # + Optional(stop_loss) 
                         # + Optional(take_profit1) 
                         # + Optional(take_profit2)  
                         # + Optional(comment)
         self.logger.debug(f"order_grammar  {order_grammar}")
         result = order_grammar.parseString(mystring)
         self.logger.debug(f"identify_order result {result}")
@@ -62,17 +62,17 @@
 
 
     def get_order(self,mystring: str = None,):
       try:
         self.logger.debug(f"get_order for {mystring}")
 
         if (self.search(mystring)):
-            # self.logger.info(msg=f"get_order found: {mystring}")
-            # parsed_order = self.identify_order(mystring)
-            # self.logger.info(msg=f"parsed_order results: {parsed_order}")
+            self.logger.info(msg=f"get_order found: {mystring}")
+            parsed_order = self.identify_order(mystring)
+            self.logger.info(msg=f"parsed_order results: {parsed_order}")
 
             # order_raw = mystring.split()
             # self.logger.info(msg=f"Order identified: {order_raw}")
 
             # order = {}
             # order['market'] = 'Any'
             # order['exchange'] = 'Any'
```

### Comparing `findmyorder-1.0.7/pyproject.toml` & `findmyorder-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.7"
+version = "1.0.8"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.0.7/PKG-INFO` & `findmyorder-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

