# Comparing `tmp/dhosting_api-0.1.tar.gz` & `tmp/dhosting_api-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhosting_api-0.1.tar", last modified: Wed Apr 26 06:25:25 2023, max compression
+gzip compressed data, was "dhosting_api-1.0.tar", last modified: Thu Apr 27 07:00:07 2023, max compression
```

## Comparing `dhosting_api-0.1.tar` & `dhosting_api-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/
--rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-26 06:25:25.126963 dhosting_api-0.1/PKG-INFO
--rw-rw-r--   0 maks      (1000) maks      (1000)      552 2023-04-25 13:32:50.000000 dhosting_api-0.1/README.rst
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/dhosting/
--rw-rw-r--   0 maks      (1000) maks      (1000)        0 2023-04-19 07:56:05.000000 dhosting_api-0.1/dhosting/__init__.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     2757 2023-04-25 11:34:03.000000 dhosting_api-0.1/dhosting/adapter.py
--rw-rw-r--   0 maks      (1000) maks      (1000)      830 2023-04-19 12:47:28.000000 dhosting_api-0.1/dhosting/base_email.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     4397 2023-04-25 12:19:42.000000 dhosting_api-0.1/dhosting/connection.py
--rw-rw-r--   0 maks      (1000) maks      (1000)      564 2023-04-21 06:23:02.000000 dhosting_api-0.1/dhosting/exceptions.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     2971 2023-04-25 11:55:46.000000 dhosting_api-0.1/dhosting/utils.py
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/dhosting_api.egg-info/
--rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/PKG-INFO
--rw-rw-r--   0 maks      (1000) maks      (1000)      326 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/SOURCES.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)        1 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/dependency_links.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)       16 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/requires.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)        9 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/top_level.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)       38 2023-04-26 06:25:25.126963 dhosting_api-0.1/setup.cfg
--rw-rw-r--   0 maks      (1000) maks      (1000)      478 2023-04-25 13:49:58.000000 dhosting_api-0.1/setup.py
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-27 07:00:07.570853 dhosting_api-1.0/
+-rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-27 07:00:07.566853 dhosting_api-1.0/PKG-INFO
+-rw-rw-r--   0 maks      (1000) maks      (1000)      552 2023-04-26 08:08:44.000000 dhosting_api-1.0/README.rst
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-27 07:00:07.566853 dhosting_api-1.0/dhosting_api/
+-rw-rw-r--   0 maks      (1000) maks      (1000)        0 2023-04-26 08:08:44.000000 dhosting_api-1.0/dhosting_api/__init__.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     2851 2023-04-27 06:41:29.000000 dhosting_api-1.0/dhosting_api/adapter.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)      830 2023-04-26 08:08:44.000000 dhosting_api-1.0/dhosting_api/base_email.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     4815 2023-04-27 06:42:34.000000 dhosting_api-1.0/dhosting_api/connection.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)      615 2023-04-27 06:41:09.000000 dhosting_api-1.0/dhosting_api/exceptions.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     2971 2023-04-26 08:08:44.000000 dhosting_api-1.0/dhosting_api/utils.py
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-27 07:00:07.566853 dhosting_api-1.0/dhosting_api.egg-info/
+-rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-27 07:00:07.000000 dhosting_api-1.0/dhosting_api.egg-info/PKG-INFO
+-rw-rw-r--   0 maks      (1000) maks      (1000)      350 2023-04-27 07:00:07.000000 dhosting_api-1.0/dhosting_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)        1 2023-04-27 07:00:07.000000 dhosting_api-1.0/dhosting_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       16 2023-04-27 07:00:07.000000 dhosting_api-1.0/dhosting_api.egg-info/requires.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       13 2023-04-27 07:00:07.000000 dhosting_api-1.0/dhosting_api.egg-info/top_level.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       38 2023-04-27 07:00:07.570853 dhosting_api-1.0/setup.cfg
+-rw-rw-r--   0 maks      (1000) maks      (1000)      482 2023-04-27 06:59:53.000000 dhosting_api-1.0/setup.py
```

### Comparing `dhosting_api-0.1/PKG-INFO` & `dhosting_api-1.0/dhosting_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dhosting_api
-Version: 0.1
+Name: dhosting-api
+Version: 1.0
 Summary: Package to connect with dhosting_api
 Author: Maks Galbierczyk
 Author-email: maksymilian.galbierczyk@apz.pl
 License: MIT
 
 Package to communicate with DhostingApi
 ===============================================================================
```

### Comparing `dhosting_api-0.1/README.rst` & `dhosting_api-1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/adapter.py` & `dhosting_api-1.0/dhosting_api/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         if endpoint == '/email/getMailboxList':
             if error_number == 120458:
                 raise exceptions.BadDomainName
             else:
                 self._generic_exception(response)
 
         if endpoint == '/emailAlias/createAlias':
+            if error_number == 130420:
+                raise exceptions.AliasAddedToSameEmail
             if error_number == 130440:
                 raise exceptions.AliasAlreadyExist
 
         if error_number == 120450:
             raise exceptions.MailboxDoesntExist
         elif error_number == 120460:
             raise exceptions.OperationError
```

### Comparing `dhosting_api-0.1/dhosting/base_email.py` & `dhosting_api-1.0/dhosting_api/base_email.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/connection.py` & `dhosting_api-1.0/dhosting_api/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,18 +89,35 @@
     def get_mailbox_quota(self, email):
         return self.get_mailbox_information(email)['quota']['limit_skrzynki_mb']
 
     def get_mailbox(self, email):
         return Mailbox(email)
 
     def generate_password(self, n):
-        alphabet = string.ascii_letters + string.digits + '!@^&*()_+<>'
-        pwd = ''
-        for i in range(n):
-            pwd += ''.join(secrets.choice(alphabet))
+        if n < 8:
+            n = 8
+        alphabet = '!@^&*()_+<>#$%-='
+        pwd = []
+        for i in range(0, 2):
+            pwd += secrets.choice(alphabet)
+
+        alphabet = string.digits
+        for i in range(0, 2):
+            pwd += secrets.choice(alphabet)
+
+        alphabet = string.ascii_letters.lower()
+        for i in range(0, 2):
+            pwd += secrets.choice(alphabet)
+
+        alphabet = string.ascii_letters
+        for i in range(0, n - 6):
+            pwd += secrets.choice(alphabet)
+
+        secrets.SystemRandom().shuffle(pwd)
+        pwd = ''.join(pwd)
         return pwd
 
     def check_limit(self, limit):
         if limit < 10:
             return True
         elif limit == -1:
             return True
```

### Comparing `dhosting_api-0.1/dhosting/exceptions.py` & `dhosting_api-1.0/dhosting_api/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,7 +41,11 @@
 class DisallowedMarks(Exception):
     pass
 
 
 class AliasAlreadyExist(Exception):
     pass
 
+
+class AliasAddedToSameEmail(Exception):
+    pass
+
```

### Comparing `dhosting_api-0.1/dhosting/utils.py` & `dhosting_api-1.0/dhosting_api/utils.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting_api.egg-info/PKG-INFO` & `dhosting_api-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dhosting-api
-Version: 0.1
+Name: dhosting_api
+Version: 1.0
 Summary: Package to connect with dhosting_api
 Author: Maks Galbierczyk
 Author-email: maksymilian.galbierczyk@apz.pl
 License: MIT
 
 Package to communicate with DhostingApi
 ===============================================================================
```

