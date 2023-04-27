# Comparing `tmp/gardener-cicd-dso-1.2038.0.tar.gz` & `tmp/gardener-cicd-dso-1.2039.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2038.0.tar", last modified: Mon Apr 24 11:38:25 2023, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2039.0.tar", last modified: Wed Apr 26 09:06:52 2023, max compression
```

## Comparing `gardener-cicd-dso-1.2038.0.tar` & `gardener-cicd-dso-1.2039.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    17856 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8057 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     6577 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-24 11:38:25.000000 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-24 11:38:25.000000 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:38:25.000000 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 11:38:25.000000 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-24 11:38:25.000000 gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:38:25.488708 gardener-cicd-dso-1.2038.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5756 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17050 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    11985 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/report.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    24726 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-24 11:38:25.492708 gardener-cicd-dso-1.2038.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-04-24 11:36:41.000000 gardener-cicd-dso-1.2038.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:52.961030 gardener-cicd-dso-1.2039.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-26 09:06:52.961030 gardener-cicd-dso-1.2039.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:52.957030 gardener-cicd-dso-1.2039.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    17856 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:52.957030 gardener-cicd-dso-1.2039.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8057 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:52.957030 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-26 09:06:52.000000 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-26 09:06:52.000000 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:06:52.000000 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-26 09:06:52.000000 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-26 09:06:52.000000 gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:52.961030 gardener-cicd-dso-1.2039.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5756 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17050 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    12151 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/report.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    24726 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-26 09:06:52.961030 gardener-cicd-dso-1.2039.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-04-26 08:39:59.000000 gardener-cicd-dso-1.2039.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2038.0/LICENSE.md` & `gardener-cicd-dso-1.2039.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/README.md` & `gardener-cicd-dso-1.2039.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/__init__.py` & `gardener-cicd-dso-1.2039.0/checkmarx/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/client.py` & `gardener-cicd-dso-1.2039.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/model.py` & `gardener-cicd-dso-1.2039.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/project.py` & `gardener-cicd-dso-1.2039.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2039.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/checkmarx/util.py` & `gardener-cicd-dso-1.2039.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/__init__.py` & `gardener-cicd-dso-1.2039.0/clamav/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/client.py` & `gardener-cicd-dso-1.2039.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2039.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/model.py` & `gardener-cicd-dso-1.2039.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/report.py` & `gardener-cicd-dso-1.2039.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/routes.py` & `gardener-cicd-dso-1.2039.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/scan.py` & `gardener-cicd-dso-1.2039.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/clamav/util.py` & `gardener-cicd-dso-1.2039.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2039.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/__init__.py` & `gardener-cicd-dso-1.2039.0/protecode/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/assessments.py` & `gardener-cicd-dso-1.2039.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/client.py` & `gardener-cicd-dso-1.2039.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/model.py` & `gardener-cicd-dso-1.2039.0/protecode/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import dataclasses
+import datetime
 import dso.labels
 import enum
 import traceback
 import typing
 
+import dateutil.parser
+
 import gci.componentmodel as cm
 
 import ci.util
 import dso.cvss
 import gci.componentmodel
 import github.compliance.model as gcm
 
@@ -266,14 +269,18 @@
 
     def reason(self):
         return self.raw['reason']
 
     def description(self):
         return self.raw.get('description')
 
+    @property
+    def modified(self) -> datetime.datetime:
+        return dateutil.parser.isoparse(self.raw.get('modified'))
+
     def applies_to_same_vulnerability_as(self, other) -> bool:
         if not isinstance(other, Triage):
             return False
         return self.vulnerability_id() == other.vulnerability_id()
 
     def __repr__(self):
         return (
```

### Comparing `gardener-cicd-dso-1.2038.0/protecode/report.py` & `gardener-cicd-dso-1.2039.0/protecode/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/rescore.py` & `gardener-cicd-dso-1.2039.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/scanning.py` & `gardener-cicd-dso-1.2039.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/protecode/util.py` & `gardener-cicd-dso-1.2039.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/setup.dso.py` & `gardener-cicd-dso-1.2039.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2038.0/setup.py` & `gardener-cicd-dso-1.2039.0/setup.py`

 * *Files identical despite different names*

