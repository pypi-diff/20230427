# Comparing `tmp/obsutils-1.0.7.tar.gz` & `tmp/obsutils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsutils-1.0.7.tar", last modified: Tue Apr 25 11:01:08 2023, max compression
+gzip compressed data, was "obsutils-1.0.8.tar", last modified: Thu Apr 27 02:12:37 2023, max compression
```

## Comparing `obsutils-1.0.7.tar` & `obsutils-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.414178 obsutils-1.0.7/
--rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 11:01:08.414051 obsutils-1.0.7/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      167 2023-04-25 09:00:58.000000 obsutils-1.0.7/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.413053 obsutils-1.0.7/obsutils/
--rw-r--r--   0 chen       (501) staff       (20)       60 2023-04-25 08:51:54.000000 obsutils-1.0.7/obsutils/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     4876 2023-04-25 10:59:56.000000 obsutils-1.0.7/obsutils/file.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.413853 obsutils-1.0.7/obsutils.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      215 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)        9 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-25 11:01:08.414229 obsutils-1.0.7/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      688 2023-04-25 11:00:58.000000 obsutils-1.0.7/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-27 02:12:37.886759 obsutils-1.0.8/
+-rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-27 02:12:37.886636 obsutils-1.0.8/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      462 2023-04-25 11:04:10.000000 obsutils-1.0.8/README.md
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-27 02:12:37.885650 obsutils-1.0.8/obsutils/
+-rw-r--r--   0 chen       (501) staff       (20)       60 2023-04-25 08:51:54.000000 obsutils-1.0.8/obsutils/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     4638 2023-04-27 02:10:07.000000 obsutils-1.0.8/obsutils/file.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-27 02:12:37.886444 obsutils-1.0.8/obsutils.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-27 02:12:37.000000 obsutils-1.0.8/obsutils.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      215 2023-04-27 02:12:37.000000 obsutils-1.0.8/obsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-27 02:12:37.000000 obsutils-1.0.8/obsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-27 02:12:37.000000 obsutils-1.0.8/obsutils.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)        9 2023-04-27 02:12:37.000000 obsutils-1.0.8/obsutils.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-27 02:12:37.886804 obsutils-1.0.8/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      688 2023-04-27 02:12:35.000000 obsutils-1.0.8/setup.py
```

### Comparing `obsutils-1.0.7/obsutils/file.py` & `obsutils-1.0.8/obsutils/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 _obsClient = None
 _last_time = None
 
 logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-
-
 def init(ak, sk, server):
     global _AK, _SK, _server
     _AK = ak
     _SK = sk
     _server = server
     logger.info("init obsutil done")
 
+
 # 检查字符串是否为合法的obs路径
 # obs路径格式为：obs://bucketname/objectname
 def _is_obs_path(path):
     if path.startswith('obs://'):
         return True
     else:
         return False
@@ -52,17 +51,15 @@
 
     url = urlparse(obs_url)
     bucket_name = url.hostname
     try:
         resp = _obsClient.getObject(bucket_name, url.path[1:], loadStreamInMemory=True)
 
         if resp.status < 300:
-            logger.info('requestId:', resp.requestId)
-            # 获取对象内容
-            logger.info('size:', resp.body.size)
+
             return resp.body.buffer
 
         else:
             logger.info('errorCode:', resp.errorCode)
             logger.info('errorMessage:', resp.errorMessage)
     except:
         import traceback
@@ -86,18 +83,15 @@
     return decorator
 
 
 @_retry(times=5)
 def _download_one_file(bucketName, src, dest):
     resp = _obsClient.getObject(bucketName, src, downloadPath=dest,
                                 progressCallback=download_progress_callback)
-    if resp.status < 300:
-        logger.info('requestId:', resp.requestId)
-        logger.info('url:', resp.body.url)
-    else:
+    if resp.status >= 300:
         logger.info('errorCode:', resp.errorCode)
         logger.info('errorMessage:', resp.errorMessage)
 
 
 # 流式下载
 def _download_one_file_stream(bucketName, src):
     try:
```

### Comparing `obsutils-1.0.7/setup.py` & `obsutils-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if __name__ == '__main__':
     name = 'obsutils'
 
     requirements = ['esdk-obs-python']
 
     setup(
         name=name,
-        version='1.0.7',
+        version='1.0.8',
         description='hw modelarts obs utils',
         # long_description='',
         # author='Taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         # keywords='Serving Deep Learning Inference AI',
```

