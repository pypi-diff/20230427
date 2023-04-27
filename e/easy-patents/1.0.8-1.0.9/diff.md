# Comparing `tmp/easy_patents-1.0.8.tar.gz` & `tmp/easy_patents-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_patents-1.0.8.tar", last modified: Sun Apr 23 09:31:49 2023, max compression
+gzip compressed data, was "dist/easy_patents-1.0.9.tar", last modified: Tue Apr 25 12:35:45 2023, max compression
```

## Comparing `easy_patents-1.0.8.tar` & `easy_patents-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents/config/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents/config/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents/sample/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents/sample/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 22:07:19.000000 easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      645 2023-04-21 08:16:33.000000 easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc
--rw-r--r--   0 root         (0) root         (0)      661 2023-04-21 22:07:19.000000 easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/sample/mail_notify.py
--rw-r--r--   0 root         (0) root         (0)    70294 2023-04-04 17:48:22.000000 easy_patents-1.0.8/easy_patents/sample/openai-0.27.4-py3-none-any.whl
--rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/sample/sample.py
--rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/sample/sample_check_due_date.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-04-21 13:10:49.000000 easy_patents-1.0.8/easy_patents/sample/sample_draft_apeal.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-21 22:04:19.000000 easy_patents-1.0.8/easy_patents/sample/sample_openai.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-21 22:41:07.000000 easy_patents-1.0.8/easy_patents/sample/sample_report_oa.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 08:11:06.000000 easy_patents-1.0.8/easy_patents/sample/sample_translate.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-04-21 11:02:27.000000 easy_patents-1.0.8/easy_patents/sample/sample_translate_oa.py
--rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/sample/sample_update_monitor_excel.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-04-23 09:31:13.000000 easy_patents-1.0.8/easy_patents/auth_info.py
--rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/delete_caches.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.8/easy_patents/errors.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-21 04:51:41.000000 easy_patents-1.0.8/easy_patents/get_apitoken.py
--rw-r--r--   0 root         (0) root         (0)    36126 2023-04-23 09:29:22.000000 easy_patents-1.0.8/easy_patents/get_info.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-04-23 07:12:37.000000 easy_patents-1.0.8/easy_patents/update_authinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 09:31:49.000000 easy_patents-1.0.8/easy_patents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-23 09:31:46.000000 easy_patents-1.0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 09:31:49.000000 easy_patents-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 09:31:49.000000 easy_patents-1.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents/config/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents/config/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents/sample/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents/sample/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 22:07:19.000000 easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      645 2023-04-21 08:16:33.000000 easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc
+-rw-r--r--   0 root         (0) root         (0)      661 2023-04-21 22:07:19.000000 easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/sample/mail_notify.py
+-rw-r--r--   0 root         (0) root         (0)    70294 2023-04-04 17:48:22.000000 easy_patents-1.0.9/easy_patents/sample/openai-0.27.4-py3-none-any.whl
+-rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/sample/sample.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/sample/sample_check_due_date.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-04-21 13:10:49.000000 easy_patents-1.0.9/easy_patents/sample/sample_draft_apeal.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-21 22:04:19.000000 easy_patents-1.0.9/easy_patents/sample/sample_openai.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-21 22:41:07.000000 easy_patents-1.0.9/easy_patents/sample/sample_report_oa.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 08:11:06.000000 easy_patents-1.0.9/easy_patents/sample/sample_translate.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-21 11:02:27.000000 easy_patents-1.0.9/easy_patents/sample/sample_translate_oa.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/sample/sample_update_monitor_excel.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-04-23 09:31:13.000000 easy_patents-1.0.9/easy_patents/auth_info.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/delete_caches.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.9/easy_patents/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-21 04:51:41.000000 easy_patents-1.0.9/easy_patents/get_apitoken.py
+-rw-r--r--   0 root         (0) root         (0)    36730 2023-04-25 12:35:17.000000 easy_patents-1.0.9/easy_patents/get_info.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-23 07:12:37.000000 easy_patents-1.0.9/easy_patents/update_authinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 12:35:45.000000 easy_patents-1.0.9/easy_patents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-25 12:35:40.000000 easy_patents-1.0.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-25 12:35:45.000000 easy_patents-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 12:35:45.000000 easy_patents-1.0.9/setup.cfg
```

### Comparing `easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc` & `easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc` & `easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc` & `easy_patents-1.0.9/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/mail_notify.py` & `easy_patents-1.0.9/easy_patents/sample/mail_notify.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/openai-0.27.4-py3-none-any.whl` & `easy_patents-1.0.9/easy_patents/sample/openai-0.27.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample.py` & `easy_patents-1.0.9/easy_patents/sample/sample.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_check_due_date.py` & `easy_patents-1.0.9/easy_patents/sample/sample_check_due_date.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_draft_apeal.py` & `easy_patents-1.0.9/easy_patents/sample/sample_draft_apeal.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_report_oa.py` & `easy_patents-1.0.9/easy_patents/sample/sample_report_oa.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_translate.py` & `easy_patents-1.0.9/easy_patents/sample/sample_translate.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_translate_oa.py` & `easy_patents-1.0.9/easy_patents/sample/sample_translate_oa.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/sample/sample_update_monitor_excel.py` & `easy_patents-1.0.9/easy_patents/sample/sample_update_monitor_excel.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/auth_info.py` & `easy_patents-1.0.9/easy_patents/auth_info.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/delete_caches.py` & `easy_patents-1.0.9/easy_patents/delete_caches.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/errors.py` & `easy_patents-1.0.9/easy_patents/errors.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/get_apitoken.py` & `easy_patents-1.0.9/easy_patents/get_apitoken.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents/get_info.py` & `easy_patents-1.0.9/easy_patents/get_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         取得したデータ
     '''
     # 通信失敗などで取得エラーがありうるので、RETRY回までリトライする
     for i in range(0, EASYPATENT_API_RETRY):
         accesstoken = EASYPATENT_AUTHINFO.get_accesstoken()
         header = {
             "Host": EASYPATENT_HOST,
-            "Authorization": "Bearer " + accesstoken
+            "Authorization": "Bearer " + accesstoken, 
+            "User-Agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.137 Safari/4E423F'
         }
         response = requests.get(url, headers=header)
         # jsonファイル以外の場合には取得は成功しているので、breakする
         if response.headers['content-type'] != "application/json":
             break
         response = response.json()
         status_code = response["result"]["statusCode"]
@@ -114,22 +115,22 @@
     >>> base_dir = os.path.dirname(__file__)
     >>> save_dir = os.path.join(base_dir, "tmp")
     >>> os.makedirs(save_dir, exist_ok=True)
 
     # ファイル名を指定しない場合、Content-Dispositionが使用される
     >>> save_path = save_to_file(info, save_dir)
     >>> save_path
-    'tmp/docContRefusalReason_2007035937.zip'
+    '/var/www/easy_patents/easy_patents/tmp/docContRefusalReason_2007035937.zip'
     >>> os.path.exists(save_path)
     True
 
     # ファイル名を指定すると、その名前で保存
     >>> save_path = save_to_file(info, save_dir, "test.zip")
     >>> save_path
-    'tmp/test.zip'
+    '/var/www/easy_patents/easy_patents/tmp/test.zip'
     >>> os.path.exists(save_path)
     True
     '''
     if filename is None:
         filename = response.headers['Content-Disposition'].split("=")[1]
     save_path = os.path.join(dirname, filename)
     with open(save_path, "wb") as f:
@@ -267,20 +268,20 @@
     --------
     >>> make_url("app_progress", "特願２０２０－８５２４")
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/2020008524'
     >>> make_url("app_progress", "特願２０２０－８５２４", convert=False)
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/特願２０２０－８５２４'
     >>> make_url("app_progress", "特願２０２０－８５２４", seed="test")
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/test/2020008524'
-    >>> make_url("app_progress", "特願２０２０－８５２４", seed="test", law="design")
+    >>> make_url("app_progress", "意願２０２０－８５２４", seed="test", law="design")
     'https://ip-data.jpo.go.jp/api/design/v1/app_progress/test/2020008524'
     '''
     base_url = "https://ip-data.jpo.go.jp/api"
     if convert:
-        key = convert_key(key)
+        key = convert_key(key, law)
     if seed:
         url = "%s/%s/v1/%s/%s/%s" % (base_url, law, api_name, seed, key)
     else:
         url = "%s/%s/v1/%s/%s" % (base_url, law, api_name, key)
     return url
 
 
@@ -338,15 +339,15 @@
         解凍後のファイルが格納されたディレクトリパス
 
     Examples
     --------
     >>> url = make_url("app_doc_cont_refusal_reason", "2007035937", law="patent")
     >>> info = get_api_info(url)
     >>> unzip_and_save(info, "app_doc_cont_refusal_reason", "2007035937", law="patent")
-    'data/patent/2007035937/app_doc_cont_refusal_reason'
+    '/var/www/easy_patents/easy_patents/data/patent/2007035937/app_doc_cont_refusal_reason'
     '''
     # zipファイルの保存
     zip_dir = make_dir_path(api_type, key, law, file_type="zip")
     zip_path = save_to_file(response, zip_dir, zip_file_name)
 
     # zipファイルの解凍
     file_dir = make_dir_path(api_type, key, law, file_type="xml")
@@ -384,17 +385,17 @@
     str
         ディレクトリ名
 
     Examples
     --------
     >>> key = "2020008423"
     >>> get_unzip_data("app_doc_cont_refusal_reason_decision", key)
-    'data/patent/2020008423/app_doc_cont_refusal_reason_decision'
+    '/var/www/easy_patents/easy_patents/data/patent/2020008423/app_doc_cont_refusal_reason_decision'
     '''
-    key = convert_key(key)
+    key = convert_key(key, law)
     file_dir = make_dir_path(api_type, key, law, file_type="xml")
     now = datetime.datetime.now()
     expire_date = now - datetime.timedelta(days=reget_date)
     latest_file = get_latest_file(file_dir)
     if latest_file:
         file_timestamp = os.path.getctime(latest_file)
         create_date = datetime.datetime.fromtimestamp(file_timestamp)
@@ -402,15 +403,15 @@
             return file_dir
 
     url = make_url(api_type, key, law=law)
     response = get_api_info(url)
     return unzip_and_save(response, api_type, key, law)
 
 
-def get_json_path(dir_name, law="patent", non_exist_ok=True):
+def get_json_path(dir_name, non_exist_ok=True):
     '''
     指定されたディレクトリにあるjsonパスを返す
     
     Parameters
     ----------
     dir_name: str
         ディレクトリ名
@@ -538,15 +539,15 @@
     #json_data = func(key)
     if api_type in ["application_reference", "publication_reference","registration_reference"]:
         seed, _ = api_type.split("_")
         url = make_url("case_number_reference", key, seed=seed, law=law)
     elif api_type in ["international_application", "international_publication"]:
         url = make_url("pct_national_phase_application_number", key, seed=api_type, law=law)
     else:
-        url = make_url(api_type, key, law=law)
+        url = make_url(api_type, key, law=law, convert=convert)
     json_data = get_api_info(url)
     
     # 次回以降の処理のために保存
     save_json(json_data, json_dir)
     return json_data
 
 
@@ -868,19 +869,19 @@
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_opinion_amendment("2020008423")
-    'data/patent/2020008423/app_doc_cont_opinion_amendment'
+    '/var/www/easy_patents/easy_patents/data/patent/2020008423/app_doc_cont_opinion_amendment'
     >>> app_doc_cont_opinion_amendment("2020021161", law="design")
-    'data/design/2020021161/app_doc_cont_opinion_amendment'
+    '/var/www/easy_patents/easy_patents/data/design/2020021161/app_doc_cont_opinion_amendment'
     >>> app_doc_cont_opinion_amendment("2018039075", law="trademark")
-    'data/trademark/2018039075/app_doc_cont_opinion_amendment'
+    '/var/www/easy_patents/easy_patents/data/trademark/2018039075/app_doc_cont_opinion_amendment'
     '''
     return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
 def app_doc_cont_refusal_reason_decision(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に対応する実体審査における発送書類の実体ファイル（拒絶理由通知書、特許査定、拒絶査定、補正の却下の決定）のxmlファイルの格納ディレクトリを返す
@@ -900,19 +901,19 @@
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_refusal_reason_decision("2020008423")
-    'data/patent/2020008423/app_doc_cont_refusal_reason_decision'
+    '/var/www/easy_patents/easy_patents/data/patent/2020008423/app_doc_cont_refusal_reason_decision'
     >>> app_doc_cont_refusal_reason_decision("2020009549", law="design")
-    'data/design/2020009549/app_doc_cont_refusal_reason_decision'
+    '/var/www/easy_patents/easy_patents/data/design/2020009549/app_doc_cont_refusal_reason_decision'
     >>> app_doc_cont_refusal_reason_decision("2021010720", law="trademark")
-    'data/trademark/2021010720/app_doc_cont_refusal_reason_decision'
+    '/var/www/easy_patents/easy_patents/data/trademark/2021010720/app_doc_cont_refusal_reason_decision'
     '''
     return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
 def app_doc_cont_refusal_reason(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に対応する拒絶理由通知書のZIPファイルをダウンロードする。
@@ -932,19 +933,19 @@
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_refusal_reason("2007035937")
-    'data/patent/2007035937/app_doc_cont_refusal_reason'
+    '/var/www/easy_patents/easy_patents/data/patent/2007035937/app_doc_cont_refusal_reason'
     >>> app_doc_cont_refusal_reason("2020009549", law="design")
-    'data/design/2020009549/app_doc_cont_refusal_reason'
+    '/var/www/easy_patents/easy_patents/data/design/2020009549/app_doc_cont_refusal_reason'
     >>> app_doc_cont_refusal_reason("2021010720", law="trademark")
-    'data/trademark/2021010720/app_doc_cont_refusal_reason'
+    '/var/www/easy_patents/easy_patents/data/trademark/2021010720/app_doc_cont_refusal_reason'
     '''
     return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
 def cite_doc_info(case_number, reget_date=1):
     '''
     指定された特許出願番号に紐づく引用文献情報を取得する。
```

### Comparing `easy_patents-1.0.8/easy_patents/update_authinfo.py` & `easy_patents-1.0.9/easy_patents/update_authinfo.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.8/easy_patents.egg-info/SOURCES.txt` & `easy_patents-1.0.9/easy_patents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

