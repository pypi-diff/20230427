# Comparing `tmp/aa_industry-0.2.1.tar.gz` & `tmp/aa_industry-0.2.2.tar.gz`

## Comparing `aa_industry-0.2.1.tar` & `aa_industry-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/admin.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/app_settings.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/apps.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/auth_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/forms.py
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/helper.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/models.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/tasks.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/tests.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/urls.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/views.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/migrations/0001_initial.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/migrations/0002_delete_usertoken.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/migrations/0003_auto_20220601_1747.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/migrations/0004_usercharacters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/migrations/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_Copying.png
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_Invention.png
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_Manufacturing.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_Reaction.png
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_ResearchMaterial.png
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/Icon_ReverseEngineering.png
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/copying.png
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/invention.png
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/manufacturing.png
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/reaction.png
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/researchMaterial.png
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/static/industry/images/researchTime.png
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/base.html
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/corp_jobs_list_snippet.html
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/index.html
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/jobs_list_snippet.html
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/registered_characters.html
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templates/industry/usertoken_confirm_delete.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templatetags/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 aa_industry-0.2.1/industry/templatetags/character_portrait.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 aa_industry-0.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_industry-0.2.1/LICENSE
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 aa_industry-0.2.1/README.md
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 aa_industry-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 aa_industry-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/__init__.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/admin.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/app_settings.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/apps.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/auth_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/forms.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/helper.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/models.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/tasks.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/tests.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/urls.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/views.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/migrations/0001_initial.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/migrations/0002_delete_usertoken.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/migrations/0003_auto_20220601_1747.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/migrations/0004_usercharacters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/migrations/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_Copying.png
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_Invention.png
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_Manufacturing.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_Reaction.png
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_ResearchMaterial.png
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/Icon_ReverseEngineering.png
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/copying.png
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/invention.png
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/manufacturing.png
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/reaction.png
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/researchMaterial.png
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/static/industry/images/researchTime.png
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/base.html
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/corp_jobs_list_snippet.html
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/index.html
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/jobs_list_snippet.html
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/registered_characters.html
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templates/industry/usertoken_confirm_delete.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templatetags/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 aa_industry-0.2.2/industry/templatetags/character_portrait.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 aa_industry-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_industry-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 aa_industry-0.2.2/README.md
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 aa_industry-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 aa_industry-0.2.2/PKG-INFO
```

### Comparing `aa_industry-0.2.1/industry/auth_hooks.py` & `aa_industry-0.2.2/industry/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/helper.py` & `aa_industry-0.2.2/industry/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     cache_corporation_id.clear()
 
     for j in jobs:
         job_details = dict()
         job_details['is_corp_job'] = is_corp
         job_details['job_id'] = j.get('job_id')
 
-        # a = EveEntity.objects.get_or_create_esi(id=j.get('blueprint_type_id'))[0]
-        a = EveEntity.objects.get_or_create_esi(id=j.get('blueprint_id'))[0]
+        a = EveEntity.objects.get_or_create_esi(id=j.get('blueprint_type_id'))[0]
         job_details['blueprint_name'] = a.name
         job_details['blueprint_id'] = a.id
 
         job_details['activity_id'] = _get_activity_by_id(j.get('activity_id'))
 
         job_details['duration'] = _secondsToTime(j.get('duration'))
         job_details['start_date'] = _fromStrToDate(j.get('start_date'))
```

### Comparing `aa_industry-0.2.1/industry/models.py` & `aa_industry-0.2.2/industry/models.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/tests.py` & `aa_industry-0.2.2/industry/tests.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/views.py` & `aa_industry-0.2.2/industry/views.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/migrations/0001_initial.py` & `aa_industry-0.2.2/industry/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/migrations/0003_auto_20220601_1747.py` & `aa_industry-0.2.2/industry/migrations/0003_auto_20220601_1747.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/migrations/0004_usercharacters.py` & `aa_industry-0.2.2/industry/migrations/0004_usercharacters.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/Icon_Copying.png` & `aa_industry-0.2.2/industry/static/industry/images/Icon_Copying.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/Icon_Invention.png` & `aa_industry-0.2.2/industry/static/industry/images/Icon_Invention.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/Icon_Manufacturing.png` & `aa_industry-0.2.2/industry/static/industry/images/Icon_Manufacturing.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/Icon_ResearchMaterial.png` & `aa_industry-0.2.2/industry/static/industry/images/Icon_ResearchMaterial.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/Icon_ReverseEngineering.png` & `aa_industry-0.2.2/industry/static/industry/images/Icon_ReverseEngineering.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/copying.png` & `aa_industry-0.2.2/industry/static/industry/images/copying.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/invention.png` & `aa_industry-0.2.2/industry/static/industry/images/invention.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/manufacturing.png` & `aa_industry-0.2.2/industry/static/industry/images/manufacturing.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/researchMaterial.png` & `aa_industry-0.2.2/industry/static/industry/images/researchMaterial.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/static/industry/images/researchTime.png` & `aa_industry-0.2.2/industry/static/industry/images/researchTime.png`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templates/industry/corp_jobs_list_snippet.html` & `aa_industry-0.2.2/industry/templates/industry/corp_jobs_list_snippet.html`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templates/industry/index.html` & `aa_industry-0.2.2/industry/templates/industry/index.html`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templates/industry/jobs_list_snippet.html` & `aa_industry-0.2.2/industry/templates/industry/jobs_list_snippet.html`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templates/industry/registered_characters.html` & `aa_industry-0.2.2/industry/templates/industry/registered_characters.html`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templates/industry/usertoken_confirm_delete.html` & `aa_industry-0.2.2/industry/templates/industry/usertoken_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/industry/templatetags/character_portrait.py` & `aa_industry-0.2.2/industry/templatetags/character_portrait.py`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/LICENSE` & `aa_industry-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/README.md` & `aa_industry-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/pyproject.toml` & `aa_industry-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_industry-0.2.1/PKG-INFO` & `aa_industry-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-industry
-Version: 0.2.1
+Version: 0.2.2
 Summary: Industry plugin app for Alliance Auth.
 Project-URL: Homepage, https://github.com/aechiara/aa-industry
 Project-URL: Documentation, https://github.com/aechiara/aa-industry
 Project-URL: Source, https://github.com/aechiara/aa-industry
 Project-URL: Changelog, https://github.com/aechiara/aa-industry
 Project-URL: Tracker, https://github.com/aechiara/aa-industry/issues
 Author-email: AlexBR Plasmodio <aechiara@gmail.com>
```

