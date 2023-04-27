# Comparing `tmp/finflo-2.0.6.tar.gz` & `tmp/finflo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finflo-2.0.6.tar", last modified: Thu Apr  6 10:54:16 2023, max compression
+gzip compressed data, was "finflo-2.0.7.tar", last modified: Thu Apr 27 14:34:31 2023, max compression
```

## Comparing `finflo-2.0.6.tar` & `finflo-2.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:54:16.128700 finflo-2.0.6/
--rw-rw-rw-   0        0        0       19 2022-11-21 10:05:01.000000 finflo-2.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5488 2023-04-06 10:54:16.129702 finflo-2.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 10:54:16.057702 finflo-2.0.6/finflo/
--rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.6/finflo/__init__.py
--rw-rw-rw-   0        0        0     1230 2022-12-21 07:25:04.000000 finflo-2.0.6/finflo/admin.py
--rw-rw-rw-   0        0        0     8907 2023-03-12 17:35:11.000000 finflo-2.0.6/finflo/api.py
--rw-rw-rw-   0        0        0      205 2023-02-27 08:45:47.000000 finflo-2.0.6/finflo/apps.py
--rw-rw-rw-   0        0        0      386 2022-11-24 13:02:42.000000 finflo-2.0.6/finflo/base_enum.py
--rw-rw-rw-   0        0        0      301 2022-12-15 05:39:52.000000 finflo-2.0.6/finflo/compatability.py
--rw-rw-rw-   0        0        0     1035 2023-02-20 05:36:29.000000 finflo-2.0.6/finflo/exception.py
--rw-rw-rw-   0        0        0     1460 2023-03-31 06:16:55.000000 finflo-2.0.6/finflo/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:54:16.124702 finflo-2.0.6/finflo/migrations/
--rw-rw-rw-   0        0        0    11683 2023-02-28 10:13:58.000000 finflo-2.0.6/finflo/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1489 2023-02-28 10:26:38.000000 finflo-2.0.6/finflo/migrations/0002_remigrate.py
--rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.6/finflo/migrations/__init__.py
--rw-rw-rw-   0        0        0     8167 2023-04-06 10:52:40.000000 finflo-2.0.6/finflo/models.py
--rw-rw-rw-   0        0        0     4090 2023-02-21 05:58:43.000000 finflo-2.0.6/finflo/serializer.py
--rw-rw-rw-   0        0        0     2785 2023-03-24 10:04:31.000000 finflo-2.0.6/finflo/signals.py
--rw-rw-rw-   0        0        0        2 2023-03-06 12:26:54.000000 finflo-2.0.6/finflo/tests.py
--rw-rw-rw-   0        0        0    13841 2023-04-06 10:53:25.000000 finflo-2.0.6/finflo/transition.py
--rw-rw-rw-   0        0        0      907 2023-02-01 11:16:37.000000 finflo-2.0.6/finflo/urls.py
--rw-rw-rw-   0        0        0      293 2022-11-21 10:05:02.000000 finflo-2.0.6/finflo/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:54:16.106705 finflo-2.0.6/finflo.egg-info/
--rw-rw-rw-   0        0        0     5488 2023-04-06 10:54:14.000000 finflo-2.0.6/finflo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-04-06 10:54:15.000000 finflo-2.0.6/finflo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:54:14.000000 finflo-2.0.6/finflo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 10:54:15.000000 finflo-2.0.6/finflo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5089 2022-12-19 10:56:18.000000 finflo-2.0.6/readme.md
--rw-rw-rw-   0        0        0      421 2023-04-06 10:54:16.136709 finflo-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-03-26 08:52:21.000000 finflo-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.357445 finflo-2.0.7/
+-rw-rw-rw-   0        0        0       19 2022-11-21 10:05:01.000000 finflo-2.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5488 2023-04-27 14:34:31.358437 finflo-2.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.306440 finflo-2.0.7/finflo/
+-rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/__init__.py
+-rw-rw-rw-   0        0        0     1230 2022-12-21 07:25:04.000000 finflo-2.0.7/finflo/admin.py
+-rw-rw-rw-   0        0        0     8907 2023-03-12 17:35:11.000000 finflo-2.0.7/finflo/api.py
+-rw-rw-rw-   0        0        0      205 2023-02-27 08:45:47.000000 finflo-2.0.7/finflo/apps.py
+-rw-rw-rw-   0        0        0      386 2022-11-24 13:02:42.000000 finflo-2.0.7/finflo/base_enum.py
+-rw-rw-rw-   0        0        0      301 2022-12-15 05:39:52.000000 finflo-2.0.7/finflo/compatability.py
+-rw-rw-rw-   0        0        0     1035 2023-02-20 05:36:29.000000 finflo-2.0.7/finflo/exception.py
+-rw-rw-rw-   0        0        0     1460 2023-03-31 06:16:55.000000 finflo-2.0.7/finflo/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.354437 finflo-2.0.7/finflo/migrations/
+-rw-rw-rw-   0        0        0    11825 2023-04-27 14:33:17.000000 finflo-2.0.7/finflo/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1489 2023-02-28 10:26:38.000000 finflo-2.0.7/finflo/migrations/0002_remigrate.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/migrations/__init__.py
+-rw-rw-rw-   0        0        0     8277 2023-04-27 14:32:20.000000 finflo-2.0.7/finflo/models.py
+-rw-rw-rw-   0        0        0     4090 2023-02-21 05:58:43.000000 finflo-2.0.7/finflo/serializer.py
+-rw-rw-rw-   0        0        0     2785 2023-03-24 10:04:31.000000 finflo-2.0.7/finflo/signals.py
+-rw-rw-rw-   0        0        0        2 2023-03-06 12:26:54.000000 finflo-2.0.7/finflo/tests.py
+-rw-rw-rw-   0        0        0    13841 2023-04-06 10:53:25.000000 finflo-2.0.7/finflo/transition.py
+-rw-rw-rw-   0        0        0      907 2023-02-01 11:16:37.000000 finflo-2.0.7/finflo/urls.py
+-rw-rw-rw-   0        0        0      293 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.335443 finflo-2.0.7/finflo.egg-info/
+-rw-rw-rw-   0        0        0     5488 2023-04-27 14:34:29.000000 finflo-2.0.7/finflo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-04-27 14:34:31.000000 finflo-2.0.7/finflo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:34:29.000000 finflo-2.0.7/finflo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 14:34:30.000000 finflo-2.0.7/finflo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5089 2022-12-19 10:56:18.000000 finflo-2.0.7/readme.md
+-rw-rw-rw-   0        0        0      421 2023-04-27 14:34:31.365444 finflo-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-03-26 08:52:21.000000 finflo-2.0.7/setup.py
```

### Comparing `finflo-2.0.6/PKG-INFO` & `finflo-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finflo
-Version: 2.0.6
+Version: 2.0.7
 Author: AnandRaj
 Author-email: anandrajb@venzotechnologies.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finflo-2.0.6/finflo/admin.py` & `finflo-2.0.7/finflo/admin.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/api.py` & `finflo-2.0.7/finflo/api.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/exception.py` & `finflo-2.0.7/finflo/exception.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/middleware.py` & `finflo-2.0.7/finflo/middleware.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/migrations/0001_initial.py` & `finflo-2.0.7/finflo/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
             },
         ),
         migrations.CreateModel(
             name='workflowitems',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_date', models.DateTimeField(auto_now_add=True)),
+                ('modified_at', models.DateTimeField(auto_now=True)),
                 ('initial_state', models.CharField(default='DRAFT', max_length=50)),
                 ('interim_state', models.CharField(default='DRAFT', max_length=50)),
                 ('final_state', models.CharField(default='DRAFT', max_length=50)),
                 ('next_available_transitions', models.JSONField(blank=True, null=True)),
                 ('action', models.CharField(blank=True, default='DRAFT', max_length=25, null=True)),
                 ('subaction', models.CharField(blank=True, max_length=55, null=True)),
                 ('previous_action', models.CharField(blank=True, max_length=55, null=True)),
@@ -173,14 +174,15 @@
                 ('interim_state', models.CharField(default='DRAFT', max_length=50)),
                 ('final_state', models.CharField(default='DRAFT', max_length=50)),
                 ('is_read', models.BooleanField(blank=True, default=True, null=True)),
                 ('record_datas', models.JSONField(blank=True, null=True)),
                 ('final_value', models.BooleanField(blank=True, default=False, null=True)),
                 ('comments', models.CharField(blank=True, max_length=500, null=True)),
                 ('created_date', models.DateTimeField(auto_now_add=True)),
+                ('modified_at', models.DateTimeField(auto_now=True)),
                 ('model_type', models.CharField(blank=True, max_length=55, null=True)),
                 ('event_user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL)),
                 ('from_party', models.CharField(max_length = 500 , blank = True , null = True )),
                 ('to_party', models.CharField(max_length = 500 , blank = True , null = True )),
                 ('workflowitems', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='WorkFlowEvents', to='finflo.workflowitems')),
             ],
             options={
```

### Comparing `finflo-2.0.6/finflo/migrations/0002_remigrate.py` & `finflo-2.0.7/finflo/migrations/0002_remigrate.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/models.py` & `finflo-2.0.7/finflo/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         verbose_name_plural = "3. Action"
         unique_together = ('description', 'model' ) 
  
 
 class workflowitems(models.Model):
     
     created_date = models.DateTimeField(auto_now_add=True)
+    modified_at = models.DateTimeField(auto_now=True)
     transitionmanager = models.OneToOneField(TransitionManager, on_delete=models.CASCADE,blank=True, null=True )
     initial_state  = models.CharField(max_length=50,default = Values.DRAFT.value)
     interim_state = models.CharField(max_length=50,default = Values.DRAFT.value)
     final_state = models.CharField(max_length=50,default = Values.DRAFT.value) 
     event_user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.SET_NULL , blank=True, null=True)
     next_available_transitions =  models.JSONField(blank=True, null=True)
     from_party = models.CharField(max_length = 500  , blank = True , null = True )
@@ -182,14 +183,15 @@
     to_party = models.CharField(max_length = 500  , blank = True , null = True )
     event_user = models.ForeignKey(settings.AUTH_USER_MODEL,  on_delete=models.SET_NULL , blank=True, null=True)
     is_read = models.BooleanField(default=True,blank=True, null=True)
     record_datas = models.JSONField(blank=True, null=True)
     final_value = models.BooleanField(default=False,blank=True, null=True)
     comments = models.CharField(max_length=500,blank=True, null=True)
     created_date = models.DateTimeField(auto_now_add=True)
+    modified_at = models.DateTimeField(auto_now=True)
     model_type = models.CharField(max_length=55, blank=True, null=True)
     
     
     class Meta:
         verbose_name_plural = "8. WorkFlowEvent"
         ordering = ['id']
```

### Comparing `finflo-2.0.6/finflo/serializer.py` & `finflo-2.0.7/finflo/serializer.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/signals.py` & `finflo-2.0.7/finflo/signals.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/transition.py` & `finflo-2.0.7/finflo/transition.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo/urls.py` & `finflo-2.0.7/finflo/urls.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/finflo.egg-info/PKG-INFO` & `finflo-2.0.7/finflo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finflo
-Version: 2.0.6
+Version: 2.0.7
 Author: AnandRaj
 Author-email: anandrajb@venzotechnologies.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finflo-2.0.6/finflo.egg-info/SOURCES.txt` & `finflo-2.0.7/finflo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finflo-2.0.6/readme.md` & `finflo-2.0.7/readme.md`

 * *Files identical despite different names*

