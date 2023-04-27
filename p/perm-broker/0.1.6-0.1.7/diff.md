# Comparing `tmp/perm_broker-0.1.6.tar.gz` & `tmp/perm_broker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perm_broker-0.1.6.tar", max compression
+gzip compressed data, was "perm_broker-0.1.7.tar", max compression
```

## Comparing `perm_broker-0.1.6.tar` & `perm_broker-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rwxr-xr-x   0        0        0        1 2021-04-08 04:00:01.000000 perm_broker-0.1.6/perm_broker/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/ops/__init__.py
--rwxr-xr-x   0        0        0     1648 2021-06-15 05:21:45.000000 perm_broker-0.1.6/perm_broker/auth/ops/common.py
--rwxr-xr-x   0        0        0     5365 2021-04-20 11:15:17.000000 perm_broker-0.1.6/perm_broker/auth/ops/dingtalk_auth.py
--rwxr-xr-x   0        0        0    10596 2021-04-19 01:53:59.000000 perm_broker-0.1.6/perm_broker/auth/ops/pass_auth.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/auth/views/__init__.py
--rwxr-xr-x   0        0        0     7560 2021-04-20 05:50:24.000000 perm_broker-0.1.6/perm_broker/auth/views/api.py
--rwxr-xr-x   0        0        0     1040 2023-03-23 09:17:00.769764 perm_broker-0.1.6/perm_broker/auth/views/debug_api.py
--rwxr-xr-x   0        0        0     3315 2021-04-19 01:54:39.000000 perm_broker-0.1.6/perm_broker/auth/views/web.py
--rwxr-xr-x   0        0        0     1733 2021-04-19 16:17:35.000000 perm_broker-0.1.6/perm_broker/backend/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:23:48.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/__init__.py
--rwxr-xr-x   0        0        0     1010 2021-04-18 08:50:15.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/helper.py
--rwxr-xr-x   0        0        0     7403 2021-04-09 02:02:58.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/models.py
--rwxr-xr-x   0        0        0     1992 2021-04-08 02:36:18.000000 perm_broker-0.1.6/perm_broker/backend/mongodb/util.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:24:06.000000 perm_broker-0.1.6/perm_broker/backend/mssql/__init__.py
--rwxr-xr-x   0        0        0     1796 2021-04-19 16:08:52.000000 perm_broker-0.1.6/perm_broker/backend/mssql/helper.py
--rwxr-xr-x   0        0        0     6835 2022-05-22 15:11:35.000000 perm_broker-0.1.6/perm_broker/backend/mssql/models.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:23:56.000000 perm_broker-0.1.6/perm_broker/backend/mysql/__init__.py
--rwxr-xr-x   0        0        0     1797 2021-06-22 09:36:15.000000 perm_broker-0.1.6/perm_broker/backend/mysql/helper.py
--rwxr-xr-x   0        0        0     6490 2022-05-22 15:12:34.000000 perm_broker-0.1.6/perm_broker/backend/mysql/models.py
--rwxr-xr-x   0        0        0      371 2021-04-19 01:51:20.000000 perm_broker-0.1.6/perm_broker/common/__init__.py
--rwxr-xr-x   0        0        0      790 2021-04-19 02:28:48.000000 perm_broker-0.1.6/perm_broker/common/conf.py
--rwxr-xr-x   0        0        0      336 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/common/event.py
--rwxr-xr-x   0        0        0      218 2021-04-19 01:51:00.000000 perm_broker-0.1.6/perm_broker/common/exceptions.py
--rwxr-xr-x   0        0        0       43 2021-04-09 02:02:20.000000 perm_broker-0.1.6/perm_broker/context.py
--rwxr-xr-x   0        0        0      160 2021-04-14 08:50:04.000000 perm_broker-0.1.6/perm_broker/default.py
--rwxr-xr-x   0        0        0     1092 2021-06-12 08:24:51.000000 perm_broker-0.1.6/perm_broker/entry.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/__init__.py
--rwxr-xr-x   0        0        0     1018 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/decr.py
--rwxr-xr-x   0        0        0     5027 2021-04-07 04:10:42.000000 perm_broker-0.1.6/perm_broker/perm/ops/perm_base.py
--rwxr-xr-x   0        0        0    16979 2021-04-18 13:55:34.000000 perm_broker-0.1.6/perm_broker/perm/ops/position.py
--rwxr-xr-x   0        0        0    10306 2021-06-15 07:27:43.000000 perm_broker-0.1.6/perm_broker/perm/ops/user_perm.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/perm/views/__init__.py
--rwxr-xr-x   0        0        0    27092 2023-04-19 01:34:21.916639 perm_broker-0.1.6/perm_broker/perm/views/api.py
--rwxr-xr-x   0        0        0     1840 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_login.html
--rwxr-xr-x   0        0        0     1564 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_login_mobile.html
--rwxr-xr-x   0        0        0      107 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/dingtalk_success.html
--rwxr-xr-x   0        0        0      248 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/templates/password_login.html
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/__init__.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/ops/__init__.py
--rwxr-xr-x   0        0        0     5725 2021-07-03 02:05:06.000000 perm_broker-0.1.6/perm_broker/user/ops/user_base.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/user/views/__init__.py
--rwxr-xr-x   0        0        0     6391 2021-04-19 01:30:12.000000 perm_broker-0.1.6/perm_broker/user/views/api.py
--rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/__init__.py
--rwxr-xr-x   0        0        0     2660 2021-06-23 00:32:57.000000 perm_broker-0.1.6/perm_broker/util/api_base.py
--rwxr-xr-x   0        0        0      198 2021-04-18 15:48:09.000000 perm_broker-0.1.6/perm_broker/util/cache_util.py
--rwxr-xr-x   0        0        0      355 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/chinese.py
--rwxr-xr-x   0        0        0     1992 2021-04-07 04:10:43.000000 perm_broker-0.1.6/perm_broker/util/db.py
--rwxr-xr-x   0        0        0      278 2023-04-19 01:39:57.575440 perm_broker-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 perm_broker-0.1.6/setup.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 perm_broker-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-04-08 04:00:01.000000 perm_broker-0.1.7/perm_broker/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/auth/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/auth/ops/__init__.py
+-rwxr-xr-x   0        0        0     1648 2021-06-15 05:21:45.000000 perm_broker-0.1.7/perm_broker/auth/ops/common.py
+-rwxr-xr-x   0        0        0     5365 2021-04-20 11:15:17.000000 perm_broker-0.1.7/perm_broker/auth/ops/dingtalk_auth.py
+-rwxr-xr-x   0        0        0    10596 2021-04-19 01:53:59.000000 perm_broker-0.1.7/perm_broker/auth/ops/pass_auth.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/auth/views/__init__.py
+-rwxr-xr-x   0        0        0     7560 2021-04-20 05:50:24.000000 perm_broker-0.1.7/perm_broker/auth/views/api.py
+-rwxr-xr-x   0        0        0     1040 2023-03-23 09:17:00.769764 perm_broker-0.1.7/perm_broker/auth/views/debug_api.py
+-rwxr-xr-x   0        0        0     3315 2021-04-19 01:54:39.000000 perm_broker-0.1.7/perm_broker/auth/views/web.py
+-rwxr-xr-x   0        0        0     1733 2021-04-19 16:17:35.000000 perm_broker-0.1.7/perm_broker/backend/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:23:48.000000 perm_broker-0.1.7/perm_broker/backend/mongodb/__init__.py
+-rwxr-xr-x   0        0        0     1010 2021-04-18 08:50:15.000000 perm_broker-0.1.7/perm_broker/backend/mongodb/helper.py
+-rwxr-xr-x   0        0        0     7403 2021-04-09 02:02:58.000000 perm_broker-0.1.7/perm_broker/backend/mongodb/models.py
+-rwxr-xr-x   0        0        0     1992 2021-04-08 02:36:18.000000 perm_broker-0.1.7/perm_broker/backend/mongodb/util.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:24:06.000000 perm_broker-0.1.7/perm_broker/backend/mssql/__init__.py
+-rwxr-xr-x   0        0        0     1796 2021-04-19 16:08:52.000000 perm_broker-0.1.7/perm_broker/backend/mssql/helper.py
+-rwxr-xr-x   0        0        0     6835 2022-05-22 15:11:35.000000 perm_broker-0.1.7/perm_broker/backend/mssql/models.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:23:56.000000 perm_broker-0.1.7/perm_broker/backend/mysql/__init__.py
+-rwxr-xr-x   0        0        0     1797 2021-06-22 09:36:15.000000 perm_broker-0.1.7/perm_broker/backend/mysql/helper.py
+-rwxr-xr-x   0        0        0     6586 2023-04-27 10:24:49.878552 perm_broker-0.1.7/perm_broker/backend/mysql/models.py
+-rwxr-xr-x   0        0        0      371 2021-04-19 01:51:20.000000 perm_broker-0.1.7/perm_broker/common/__init__.py
+-rwxr-xr-x   0        0        0      790 2021-04-19 02:28:48.000000 perm_broker-0.1.7/perm_broker/common/conf.py
+-rwxr-xr-x   0        0        0      336 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/common/event.py
+-rwxr-xr-x   0        0        0      218 2021-04-19 01:51:00.000000 perm_broker-0.1.7/perm_broker/common/exceptions.py
+-rwxr-xr-x   0        0        0       43 2021-04-09 02:02:20.000000 perm_broker-0.1.7/perm_broker/context.py
+-rwxr-xr-x   0        0        0      160 2021-04-14 08:50:04.000000 perm_broker-0.1.7/perm_broker/default.py
+-rwxr-xr-x   0        0        0     1092 2021-06-12 08:24:51.000000 perm_broker-0.1.7/perm_broker/entry.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/perm/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/perm/ops/__init__.py
+-rwxr-xr-x   0        0        0     1018 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/perm/ops/decr.py
+-rwxr-xr-x   0        0        0     5027 2021-04-07 04:10:42.000000 perm_broker-0.1.7/perm_broker/perm/ops/perm_base.py
+-rwxr-xr-x   0        0        0    16979 2021-04-18 13:55:34.000000 perm_broker-0.1.7/perm_broker/perm/ops/position.py
+-rwxr-xr-x   0        0        0    10306 2021-06-15 07:27:43.000000 perm_broker-0.1.7/perm_broker/perm/ops/user_perm.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/perm/views/__init__.py
+-rwxr-xr-x   0        0        0    27092 2023-04-19 01:34:21.916639 perm_broker-0.1.7/perm_broker/perm/views/api.py
+-rwxr-xr-x   0        0        0     1840 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/templates/dingtalk_login.html
+-rwxr-xr-x   0        0        0     1564 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/templates/dingtalk_login_mobile.html
+-rwxr-xr-x   0        0        0      107 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/templates/dingtalk_success.html
+-rwxr-xr-x   0        0        0      248 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/templates/password_login.html
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/user/__init__.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/user/ops/__init__.py
+-rwxr-xr-x   0        0        0     5725 2021-07-03 02:05:06.000000 perm_broker-0.1.7/perm_broker/user/ops/user_base.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/user/views/__init__.py
+-rwxr-xr-x   0        0        0     6391 2021-04-19 01:30:12.000000 perm_broker-0.1.7/perm_broker/user/views/api.py
+-rwxr-xr-x   0        0        0        1 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/util/__init__.py
+-rwxr-xr-x   0        0        0     2660 2021-06-23 00:32:57.000000 perm_broker-0.1.7/perm_broker/util/api_base.py
+-rwxr-xr-x   0        0        0      198 2021-04-18 15:48:09.000000 perm_broker-0.1.7/perm_broker/util/cache_util.py
+-rwxr-xr-x   0        0        0      355 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/util/chinese.py
+-rwxr-xr-x   0        0        0     1992 2021-04-07 04:10:43.000000 perm_broker-0.1.7/perm_broker/util/db.py
+-rwxr-xr-x   0        0        0      278 2023-04-27 10:30:03.461660 perm_broker-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 perm_broker-0.1.7/setup.py
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 perm_broker-0.1.7/PKG-INFO
```

### Comparing `perm_broker-0.1.6/perm_broker/auth/ops/common.py` & `perm_broker-0.1.7/perm_broker/auth/ops/common.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/auth/ops/dingtalk_auth.py` & `perm_broker-0.1.7/perm_broker/auth/ops/dingtalk_auth.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/auth/ops/pass_auth.py` & `perm_broker-0.1.7/perm_broker/auth/ops/pass_auth.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/auth/views/api.py` & `perm_broker-0.1.7/perm_broker/auth/views/api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/auth/views/debug_api.py` & `perm_broker-0.1.7/perm_broker/auth/views/debug_api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/auth/views/web.py` & `perm_broker-0.1.7/perm_broker/auth/views/web.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/__init__.py` & `perm_broker-0.1.7/perm_broker/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mongodb/helper.py` & `perm_broker-0.1.7/perm_broker/backend/mongodb/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mongodb/models.py` & `perm_broker-0.1.7/perm_broker/backend/mongodb/models.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mongodb/util.py` & `perm_broker-0.1.7/perm_broker/backend/mongodb/util.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mssql/helper.py` & `perm_broker-0.1.7/perm_broker/backend/mssql/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mssql/models.py` & `perm_broker-0.1.7/perm_broker/backend/mssql/models.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mysql/helper.py` & `perm_broker-0.1.7/perm_broker/backend/mysql/helper.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/backend/mysql/models.py` & `perm_broker-0.1.7/perm_broker/backend/mysql/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     return oid
 
 
 def model_save(self):
     try:
         if hasattr(self, 'lut'):
             self.lut = datetime.datetime.now()
+        elif hasattr(self, 'info'):
+            self.info['lut'] = str(datetime.datetime.now())
         session.add(self)
         session.commit()
     except Exception as e:
         session.close()
 
 Base.save = model_save
```

### Comparing `perm_broker-0.1.6/perm_broker/common/conf.py` & `perm_broker-0.1.7/perm_broker/common/conf.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/entry.py` & `perm_broker-0.1.7/perm_broker/entry.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/perm/ops/decr.py` & `perm_broker-0.1.7/perm_broker/perm/ops/decr.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/perm/ops/perm_base.py` & `perm_broker-0.1.7/perm_broker/perm/ops/perm_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/perm/ops/position.py` & `perm_broker-0.1.7/perm_broker/perm/ops/position.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/perm/ops/user_perm.py` & `perm_broker-0.1.7/perm_broker/perm/ops/user_perm.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/perm/views/api.py` & `perm_broker-0.1.7/perm_broker/perm/views/api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/templates/dingtalk_login.html` & `perm_broker-0.1.7/perm_broker/templates/dingtalk_login.html`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/templates/dingtalk_login_mobile.html` & `perm_broker-0.1.7/perm_broker/templates/dingtalk_login_mobile.html`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/user/ops/user_base.py` & `perm_broker-0.1.7/perm_broker/user/ops/user_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/user/views/api.py` & `perm_broker-0.1.7/perm_broker/user/views/api.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/util/api_base.py` & `perm_broker-0.1.7/perm_broker/util/api_base.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/perm_broker/util/db.py` & `perm_broker-0.1.7/perm_broker/util/db.py`

 * *Files identical despite different names*

### Comparing `perm_broker-0.1.6/setup.py` & `perm_broker-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'perm_broker.util']
 
 package_data = \
 {'': ['*'], 'perm_broker': ['templates/*']}
 
 setup_kwargs = {
     'name': 'perm-broker',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': 'None',
     'author': 'Gongziting Tech Ltd.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

