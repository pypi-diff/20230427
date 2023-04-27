# Comparing `tmp/devvio_util-1.4.0.tar.gz` & `tmp/devvio_util-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.4.0.tar", last modified: Thu Mar 23 14:16:50 2023, max compression
+gzip compressed data, was "devvio_util-1.4.2.tar", last modified: Thu Apr 27 17:02:14 2023, max compression
```

## Comparing `devvio_util-1.4.0.tar` & `devvio_util-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:16:50.684430 devvio_util-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-23 14:16:50.684430 devvio_util-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:16:43.000000 devvio_util-1.4.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:16:50.684430 devvio_util-1.4.0/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:16:43.000000 devvio_util-1.4.0/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-23 14:16:43.000000 devvio_util-1.4.0/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-03-23 14:16:43.000000 devvio_util-1.4.0/devvio_util/lib_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-23 14:16:43.000000 devvio_util-1.4.0/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:16:50.684430 devvio_util-1.4.0/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-23 14:16:50.000000 devvio_util-1.4.0/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-23 14:16:50.000000 devvio_util-1.4.0/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:16:50.000000 devvio_util-1.4.0/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:16:50.000000 devvio_util-1.4.0/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 14:16:50.000000 devvio_util-1.4.0/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:16:50.684430 devvio_util-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-23 14:16:43.000000 devvio_util-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.544627 devvio_util-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 17:02:14.544627 devvio_util-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:01.000000 devvio_util-1.4.2/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.540627 devvio_util-1.4.2/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/lib_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.540627 devvio_util-1.4.2/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:02:14.544627 devvio_util-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 17:02:01.000000 devvio_util-1.4.2/setup.py
```

### Comparing `devvio_util-1.4.0/devvio_util/psql_mixin.py` & `devvio_util-1.4.2/devvio_util/psql_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import psycopg2
 import time
 
 
 SQL_ATTEMPTS = 5
+
+
 class PsqlMixin:
     def __init__(self, *args, **kwargs):
         """
         :param logger: Logging object
         :param db_secrets: Dict passing DB credentials (db_host, db_user, db_pass, db_name, db_port)
         :param sql_attempts: Number of attempts the query must try before throwing a timeout exception
         """
         try:
             super().__init__(*args, **kwargs)  # forwards all unused arguments
         except Exception as e:
-            kwargs['logger'].debug('super().__init__() failed: {}'.format(e))
-        self._logger = kwargs['logger']
+            kwargs["logger"].debug("super().__init__() failed: {}".format(e))
+        self._logger = kwargs["logger"]
         self._conn_string = None
         self._conn = None
-        self._db_secrets = kwargs['db_secrets']
-        self._sql_attempts = kwargs.get('sql_attempts', SQL_ATTEMPTS)
+        self._db_secrets = kwargs["db_secrets"]
+        self._sql_attempts = kwargs.get("sql_attempts", SQL_ATTEMPTS)
 
     def set_conn_string(self):
         """
         Set the database connection string
         :return:
         :rtype:
         """
@@ -51,17 +53,20 @@
         :param kwargs:
         :return:
         """
         attempts = self._sql_attempts
         while attempts > 0:
             attempts = attempts - 1
             try:
+                n = len(self._conn.notices)
                 cursor = self._conn.cursor()
                 self._logger.debug(f"{args}")
                 cursor.execute(*args, **kwargs)
+                for notice in self._conn.notices[n:]:
+                    self._logger.info(f'{notice}.')
                 return cursor
             except psycopg2.OperationalError as e:
                 self._logger.exception(e)
                 self._logger.notice("psycopg2.OperationalError: {}".format(e))
                 time.sleep(0.2)
                 self.connect()
             except psycopg2.InterfaceError as e:
@@ -86,13 +91,13 @@
         """
         Rollback uncommitted updates.
         :return:
         """
         self._conn.rollback()
 
     def get_db_cred(self):
-        db_host = self._db_secrets.get('DEVV_DB_HOST')
-        db_user = self._db_secrets.get('DEVV_DB_USER')
-        db_pass = self._db_secrets.get('DEVV_DB_PASS')
-        db_name = self._db_secrets.get('DEVV_DB_NAME')
-        db_port = self._db_secrets.get('DEVV_DB_PORT')
-        return db_host, db_user, db_pass, db_name, db_port
+        db_host = self._db_secrets.get("DEVV_DB_HOST")
+        db_user = self._db_secrets.get("DEVV_DB_USER")
+        db_pass = self._db_secrets.get("DEVV_DB_PASS")
+        db_name = self._db_secrets.get("DEVV_DB_NAME")
+        db_port = self._db_secrets.get("DEVV_DB_PORT")
+        return db_host, db_user, db_pass, db_name, db_port
```

