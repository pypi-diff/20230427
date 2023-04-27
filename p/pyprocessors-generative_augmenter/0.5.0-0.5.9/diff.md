# Comparing `tmp/pyprocessors-generative_augmenter-0.5.0.tar.gz` & `tmp/pyprocessors-generative_augmenter-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-generative_augmenter-0.5.0.tar", last modified: Thu Apr 27 10:00:39 2023, max compression
+gzip compressed data, was "pyprocessors-generative_augmenter-0.5.9.tar", last modified: Thu Apr 27 11:12:50 2023, max compression
```

## Comparing `pyprocessors-generative_augmenter-0.5.0.tar` & `pyprocessors-generative_augmenter-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       97 2021-04-14 09:32:17.791141 pyprocessors-generative_augmenter-0.5.0/.dockerignore
--rw-r--r--   0        0        0      147 2021-04-16 09:33:20.914449 pyprocessors-generative_augmenter-0.5.0/.gitignore
--rwxr-xr-x   0        0        0        0 2023-04-27 09:59:23.728678 pyprocessors-generative_augmenter-0.5.0/.tox/.package.lock
--rw-r--r--   0        0        0      448 2021-04-14 09:32:17.791141 pyprocessors-generative_augmenter-0.5.0/Dockerfile
--rw-r--r--   0        0        0    10238 2023-04-26 15:18:15.181175 pyprocessors-generative_augmenter-0.5.0/Jenkinsfile
--rw-r--r--   0        0        0      380 2022-02-22 13:26:31.568419 pyprocessors-generative_augmenter-0.5.0/README.md
--rw-r--r--   0        0        0     1559 2022-04-08 12:08:36.518352 pyprocessors-generative_augmenter-0.5.0/bumpversion.py
--rw-r--r--   0        0        0       58 2023-04-27 09:55:33.498031 pyprocessors-generative_augmenter-0.5.0/pyprocessors_generative_augmenter/__init__.py
--rw-r--r--   0        0        0     5857 2023-04-27 09:59:15.520722 pyprocessors-generative_augmenter-0.5.0/pyprocessors_generative_augmenter/generative_augmenter.py
--rw-r--r--   0        0        0     2593 2023-04-26 16:52:11.758142 pyprocessors-generative_augmenter-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-03-25 07:15:30.426146 pyprocessors-generative_augmenter-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     9161 2023-04-27 09:40:25.455367 pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs.json
--rw-r--r--   0        0        0     6757 2023-04-27 09:35:53.688000 pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0     7931 2023-04-27 09:59:31.128639 pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_preserve_entities_augmented.json
--rw-r--r--   0        0        0     6713 2023-04-27 09:37:02.059000 pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0     8111 2023-04-27 09:59:31.132639 pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_substitute_entities_augmented.json
--rw-r--r--   0        0        0     1379 2023-04-27 09:39:13.195552 pyprocessors-generative_augmenter-0.5.0/tests/test_generative_augmenter.py
--rw-r--r--   0        0        0      951 2023-02-15 16:25:11.973559 pyprocessors-generative_augmenter-0.5.0/tox.ini
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.0/setup.py
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      167 2023-04-27 11:04:50.634861 pyprocessors-generative_augmenter-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10240 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       54 2023-04-27 11:12:49.262433 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/__init__.py
+-rw-r--r--   0        0        0     5857 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py
+-rw-r--r--   0        0        0     2593 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0     9161 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json
+-rw-r--r--   0        0        0     6757 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities.json
+-rw-r--r--   0        0        0     7931 2023-04-27 11:12:46.257354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities_augmented.json
+-rw-r--r--   0        0        0     6713 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities.json
+-rw-r--r--   0        0        0     8111 2023-04-27 11:12:46.260354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities_augmented.json
+-rw-r--r--   0        0        0     1379 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tests/test_generative_augmenter.py
+-rw-r--r--   0        0        0      951 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/setup.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/PKG-INFO
```

### Comparing `pyprocessors-generative_augmenter-0.5.0/Jenkinsfile` & `pyprocessors-generative_augmenter-0.5.9/Jenkinsfile`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
           }
           steps {
             script {
               println("attempt to publish ${env.JOB_NAME} with version: ${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}")
 
               // push updates of file __init__.py
               withCredentials([gitUsernamePassword(credentialsId: 'bitbucket-user', gitToolName: 'git-tool')]) {
-                sh "echo '\"\"\"GenerativeazA$$ processor\"\"\"' > pyprocessors_generative_augmenter/__init__.py"
+                sh "echo '\"\"\"GenerativeazA\$\$ processor\"\"\"' > pyprocessors_generative_augmenter/__init__.py"
                 sh "echo '__version__ = \"${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}\"' >> pyprocessors_generative_augmenter/__init__.py"
                 sh 'git commit pyprocessors_generative_augmenter/__init__.py -m "[Jenkins CI] Commit on version files" || echo "No changes to commit"'
                 sh 'git push'
               }
             }
           }
         }
```

### Comparing `pyprocessors-generative_augmenter-0.5.0/bumpversion.py` & `pyprocessors-generative_augmenter-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/pyprocessors_generative_augmenter/generative_augmenter.py` & `pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/pyproject.toml` & `pyprocessors-generative_augmenter-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_preserve_entities.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_preserve_entities_augmented.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities_augmented.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_substitute_entities.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/data/jinjadocs_substitute_entities_augmented.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities_augmented.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tests/test_generative_augmenter.py` & `pyprocessors-generative_augmenter-0.5.9/tests/test_generative_augmenter.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/tox.ini` & `pyprocessors-generative_augmenter-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.0/setup.py` & `pyprocessors-generative_augmenter-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['generative_augmenter = '
                           'pyprocessors_generative_augmenter.generative_augmenter:GenerativeAugmenterProcessor']}
 
 setup(name='pyprocessors-generative_augmenter',
-      version='0.5.0',
-      description='GenerativeAugmenter processor',
+      version='0.5.9',
+      description='GenerativeazA$$ processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
       extras_require=extras_require,
```

### Comparing `pyprocessors-generative_augmenter-0.5.0/PKG-INFO` & `pyprocessors-generative_augmenter-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyprocessors-generative_augmenter
-Version: 0.5.0
-Summary: GenerativeAugmenter processor
+Version: 0.5.9
+Summary: GenerativeazA$$ processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

