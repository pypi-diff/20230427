# Comparing `tmp/apis_bibsonomy-0.4.1.tar.gz` & `tmp/apis_bibsonomy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apis_bibsonomy-0.4.1.tar", max compression
+gzip compressed data, was "apis_bibsonomy-0.5.0.tar", max compression
```

## Comparing `apis_bibsonomy-0.4.1.tar` & `apis_bibsonomy-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0     1141 2023-04-04 15:02:10.548468 apis_bibsonomy-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0       22 2023-04-04 15:02:33.520733 apis_bibsonomy-0.4.1/apis_bibsonomy/__init__.py
--rw-r--r--   0        0        0     6140 2023-04-04 15:02:10.548468 apis_bibsonomy-0.4.1/apis_bibsonomy/api_views.py
--rw-r--r--   0        0        0       96 2023-04-04 15:02:10.548468 apis_bibsonomy-0.4.1/apis_bibsonomy/apps.py
--rw-r--r--   0        0        0     3778 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/autocompletes.py
--rw-r--r--   0        0        0        0 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/fields.py
--rw-r--r--   0        0        0     1707 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/forms.py
--rw-r--r--   0        0        0     1157 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/0001_initial.py
--rw-r--r--   0        0        0      484 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/0002_reference_folio.py
--rw-r--r--   0        0        0      704 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/0003_auto_20230202_0953.py
--rw-r--r--   0        0        0        0 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/__init__.py
--rw-r--r--   0        0        0      899 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/models.py
--rw-r--r--   0        0        0      107 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/static/apis_bibsonomy/css/apis_bibsonomy.css
--rw-r--r--   0        0        0     4933 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js
--rw-r--r--   0        0        0   116169 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js
--rw-r--r--   0        0        0      761 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html
--rw-r--r--   0        0        0      214 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/templates/apis_bibsonomy/form_tag.html
--rw-r--r--   0        0        0        0 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/templatetags/__init__.py
--rw-r--r--   0        0        0      774 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/templatetags/bibsonomy_templatetags.py
--rw-r--r--   0        0        0      326 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/urls.py
--rw-r--r--   0        0        0     2169 2023-04-04 15:02:10.552468 apis_bibsonomy-0.4.1/apis_bibsonomy/utils.py
--rw-r--r--   0        0        0      352 2023-04-04 15:02:33.464730 apis_bibsonomy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 apis_bibsonomy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0       22 2023-04-27 10:57:53.520555 apis_bibsonomy-0.5.0/apis_bibsonomy/__init__.py
+-rw-r--r--   0        0        0     6140 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/api_views.py
+-rw-r--r--   0        0        0      150 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/apps.py
+-rw-r--r--   0        0        0     3778 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/autocompletes.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/fields.py
+-rw-r--r--   0        0        0     1707 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/forms.py
+-rw-r--r--   0        0        0     1157 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/0001_initial.py
+-rw-r--r--   0        0        0      484 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/0002_reference_folio.py
+-rw-r--r--   0        0        0      704 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/0003_auto_20230202_0953.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/__init__.py
+-rw-r--r--   0        0        0     1370 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/models.py
+-rw-r--r--   0        0        0      107 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/static/apis_bibsonomy/css/apis_bibsonomy.css
+-rw-r--r--   0        0        0     4933 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js
+-rw-r--r--   0        0        0   116169 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js
+-rw-r--r--   0        0        0      761 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html
+-rw-r--r--   0        0        0      214 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/form_tag.html
+-rw-r--r--   0        0        0     1028 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/reference_confirm_delete.html
+-rw-r--r--   0        0        0      675 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/reference_detail.html
+-rw-r--r--   0        0        0      365 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/reference_list.html
+-rw-r--r--   0        0        0      394 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templates/base.html
+-rw-r--r--   0        0        0        0 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templatetags/__init__.py
+-rw-r--r--   0        0        0      774 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/templatetags/bibsonomy_templatetags.py
+-rw-r--r--   0        0        0      659 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/urls.py
+-rw-r--r--   0        0        0     2169 2023-04-27 10:57:26.580204 apis_bibsonomy-0.5.0/apis_bibsonomy/utils.py
+-rw-r--r--   0        0        0     1485 2023-04-27 10:57:26.584204 apis_bibsonomy-0.5.0/apis_bibsonomy/views.py
+-rw-r--r--   0        0        0      352 2023-04-27 10:57:53.460554 apis_bibsonomy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 apis_bibsonomy-0.5.0/PKG-INFO
```

### Comparing `apis_bibsonomy-0.4.1/LICENSE.txt` & `apis_bibsonomy-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/api_views.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/api_views.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/autocompletes.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/autocompletes.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/forms.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/forms.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/0001_initial.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/migrations/0003_auto_20230202_0953.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/migrations/0003_auto_20230202_0953.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js` & `apis_bibsonomy-0.5.0/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js` & `apis_bibsonomy-0.5.0/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html` & `apis_bibsonomy-0.5.0/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/templatetags/bibsonomy_templatetags.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/templatetags/bibsonomy_templatetags.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/apis_bibsonomy/utils.py` & `apis_bibsonomy-0.5.0/apis_bibsonomy/utils.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.4.1/PKG-INFO` & `apis_bibsonomy-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apis-bibsonomy
-Version: 0.4.1
+Version: 0.5.0
 Summary: Bibsonomy/Zotero plugin for managing refernces in APIS framework
 License: MIT
 Author: Matthias Schlögl
 Author-email: m.schloegl@gmail.com
 Requires-Python: >=3.6,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

