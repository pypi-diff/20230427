# Comparing `tmp/drf-crud-proxy-0.3.1.tar.gz` & `tmp/drf-crud-proxy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-crud-proxy-0.3.1.tar", last modified: Wed May  5 07:14:11 2021, max compression
+gzip compressed data, was "drf-crud-proxy-0.4.0.tar", last modified: Thu Apr 27 20:35:34 2023, max compression
```

## Comparing `drf-crud-proxy-0.3.1.tar` & `drf-crud-proxy-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 atte      (1000) users      (985)        0 2021-05-05 07:14:11.720020 drf-crud-proxy-0.3.1/
--rw-r--r--   0 atte      (1000) users      (985)      182 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/MANIFEST.in
--rw-r--r--   0 atte      (1000) users      (985)     3811 2021-05-05 07:14:11.720020 drf-crud-proxy-0.3.1/PKG-INFO
--rw-r--r--   0 atte      (1000) users      (985)     2279 2021-05-05 07:07:35.000000 drf-crud-proxy-0.3.1/README.rst
-drwxr-xr-x   0 atte      (1000) users      (985)        0 2021-05-05 07:14:11.720020 drf-crud-proxy-0.3.1/drf_crud_proxy/
--rw-r--r--   0 atte      (1000) users      (985)      245 2021-05-05 07:03:18.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/__init__.py
--rw-r--r--   0 atte      (1000) users      (985)      101 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/apps.py
--rw-r--r--   0 atte      (1000) users      (985)     1174 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/generics.py
--rw-r--r--   0 atte      (1000) users      (985)     3305 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/mixins.py
--rw-r--r--   0 atte      (1000) users      (985)     3763 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/proxy.py
--rw-r--r--   0 atte      (1000) users      (985)      621 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy/viewsets.py
-drwxr-xr-x   0 atte      (1000) users      (985)        0 2021-05-05 07:14:11.720020 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/
--rw-r--r--   0 atte      (1000) users      (985)     3811 2021-05-05 07:14:11.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/PKG-INFO
--rw-r--r--   0 atte      (1000) users      (985)      410 2021-05-05 07:14:11.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 atte      (1000) users      (985)        1 2021-05-05 07:14:11.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 atte      (1000) users      (985)        1 2020-09-21 08:50:09.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/not-zip-safe
--rw-r--r--   0 atte      (1000) users      (985)       42 2021-05-05 07:14:11.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/requires.txt
--rw-r--r--   0 atte      (1000) users      (985)       27 2021-05-05 07:14:11.000000 drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/top_level.txt
--rw-r--r--   0 atte      (1000) users      (985)       38 2021-05-05 07:14:11.720020 drf-crud-proxy-0.3.1/setup.cfg
--rwxr-xr-x   0 atte      (1000) users      (985)     2001 2021-05-05 07:12:13.000000 drf-crud-proxy-0.3.1/setup.py
+drwxr-xr-x   0 atte      (1000) users      (985)        0 2023-04-27 20:35:34.984190 drf-crud-proxy-0.4.0/
+-rw-r--r--   0 atte      (1000) users      (985)     1073 2021-05-05 07:02:30.000000 drf-crud-proxy-0.4.0/LICENSE
+-rw-r--r--   0 atte      (1000) users      (985)      182 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/MANIFEST.in
+-rw-r--r--   0 atte      (1000) users      (985)     3365 2023-04-27 20:35:34.984190 drf-crud-proxy-0.4.0/PKG-INFO
+-rw-r--r--   0 atte      (1000) users      (985)     2257 2023-04-27 20:18:57.000000 drf-crud-proxy-0.4.0/README.rst
+drwxr-xr-x   0 atte      (1000) users      (985)        0 2023-04-27 20:35:34.980856 drf-crud-proxy-0.4.0/drf_crud_proxy/
+-rw-r--r--   0 atte      (1000) users      (985)      245 2023-04-27 20:29:37.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/__init__.py
+-rw-r--r--   0 atte      (1000) users      (985)      101 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/apps.py
+-rw-r--r--   0 atte      (1000) users      (985)     1174 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/generics.py
+-rw-r--r--   0 atte      (1000) users      (985)     3305 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/mixins.py
+-rw-r--r--   0 atte      (1000) users      (985)     3763 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/proxy.py
+-rw-r--r--   0 atte      (1000) users      (985)      621 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy/viewsets.py
+drwxr-xr-x   0 atte      (1000) users      (985)        0 2023-04-27 20:35:34.984190 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/
+-rw-r--r--   0 atte      (1000) users      (985)     3365 2023-04-27 20:35:34.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 atte      (1000) users      (985)      418 2023-04-27 20:35:34.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 atte      (1000) users      (985)        1 2023-04-27 20:35:34.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 atte      (1000) users      (985)        1 2020-09-21 08:50:09.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 atte      (1000) users      (985)       42 2023-04-27 20:35:34.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/requires.txt
+-rw-r--r--   0 atte      (1000) users      (985)       27 2023-04-27 20:35:34.000000 drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/top_level.txt
+-rw-r--r--   0 atte      (1000) users      (985)       38 2023-04-27 20:35:34.984190 drf-crud-proxy-0.4.0/setup.cfg
+-rwxr-xr-x   0 atte      (1000) users      (985)     2103 2023-04-27 20:35:15.000000 drf-crud-proxy-0.4.0/setup.py
```

### Comparing `drf-crud-proxy-0.3.1/PKG-INFO` & `drf-crud-proxy-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,93 @@
 Metadata-Version: 2.1
 Name: drf-crud-proxy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Separate serializers for parsing requests and returning responses in DRF
-Home-page: https://github.com/attevaltonen/drf-crud-proxy
-Author: attevaltonen
-Author-email: atte.hj.valtonen@gmail.com
+Home-page: https://github.com/attevaltojarvi/drf-crud-proxy
+Author: attevaltojarvi
+Author-email: atte.valtojarvi@gmail.com
 License: MIT
-Description: DRF CRUD Proxy
-        ==============
-        
-        This package provides extended Django REST Framework generic views and viewsets that provide the possibility to specify
-        different serializers for reading the incoming request and presenting the response.
-        
-        This is super handy in situations where you want to, for example, let the user send a ForeignKey attribute,
-        but present the related object alongside the response instead of only the database ID.
-        
-        Requirements
-        ------------
-        
-        - Python 3.6, 3.7, 3.8 and 3.9 (probably older versions as well)
-        - Django 2.2, 3.0, 3.1 and 3.2 (basically works with older versions as well, but they're EOL)
-        - Django REST Framework 3.8 or newer (probably works on any 3.x version)
-        
-        Installation
-        ------------
-        
-        .. code::
-        
-          pip install drf-crud-proxy
-        
-        Usage
-        -----
-        
-        Import the generic views and subclass your own views from them. Specify ``request_serializer_class`` and/or
-        ``response_serializer_class`` to the view (both default to DRF's own ``serializer_class`` attribute).
-        
-        .. code:: python
-        
-          # api/views.py
-        
-          from drf_crud_proxy import generics
-          from app.models import MyModel
-          from api.serializers import MyModelCreateSerializer, MyModelSerializer
-        
-        
-          class MyModelListCreateView(generics.ProxiedListCreateAPIView):
-              queryset = MyModel.objects.all()
-              request_serializer_class = MyModelCreateSerializer
-              response_serializer_class = MyModelSerializer
-        
-        The incoming request is handled with ``MyModelCreateSerializer`` and the response with ``MyModelSerializer``.
-        
-        If you want to customize the data on either situation, override ``get_request_data`` and/or ``get_response_data``
-        methods in the view.
-        
-        The package also supports the so-called ``PUT-as-create`` behavior that was removed from DRF in its 3.0 release. Note that
-        the user has to have model permissions for the corresponding create behavior (``POST`` request).
-        
-        **NOTE**: The ``PUT-as-create`` functionality doesn't have tests (yet).
-        
-        License
-        -------
-        
-        MIT
-        
-        Inspiration
-        -----------
-        
-        This functionality in DRF is something I've needed in numerous Django projects, so hopefully this will help someone else
-        too :)
-        
-        This package has been built on top of the ideas presented by the great vintasoftware's ``drf-rw-serializers`` (https://github.com/vintasoftware/drf-rw-serializers) package. Thanks!
-        
 Keywords: Django REST Framework,Serializers,REST,API,Django
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Finnish
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+DRF CRUD Proxy
+==============
+
+This package provides extended Django REST Framework generic views and viewsets that provide the possibility to specify
+different serializers for reading the incoming request and presenting the response.
+
+This is super handy in situations where you want to, for example, let the user send a ForeignKey attribute,
+but present the related object alongside the response instead of only the database ID.
+
+Requirements
+------------
+
+- Python 3.6, 3.7, 3.8, 3.9, 3.10 and 3.11
+- Django 3.2, 4.0, 4.1 and 4.2 (basically works with older versions as well, but they're EOL)
+- Django REST Framework 3.8 or newer (probably works on any 3.x version)
+
+Installation
+------------
+
+.. code::
+
+  pip install drf-crud-proxy
+
+Usage
+-----
+
+Import the generic views and subclass your own views from them. Specify ``request_serializer_class`` and/or
+``response_serializer_class`` to the view (both default to DRF's own ``serializer_class`` attribute).
+
+.. code:: python
+
+  # api/views.py
+
+  from drf_crud_proxy import generics
+  from app.models import MyModel
+  from api.serializers import MyModelCreateSerializer, MyModelSerializer
+
+
+  class MyModelListCreateView(generics.ProxiedListCreateAPIView):
+      queryset = MyModel.objects.all()
+      request_serializer_class = MyModelCreateSerializer
+      response_serializer_class = MyModelSerializer
+
+The incoming request is handled with ``MyModelCreateSerializer`` and the response with ``MyModelSerializer``.
+
+If you want to customize the data on either situation, override ``get_request_data`` and/or ``get_response_data``
+methods in the view.
+
+The package also supports the so-called ``PUT-as-create`` behavior that was removed from DRF in its 3.0 release. Note that
+the user has to have model permissions for the corresponding create behavior (``POST`` request).
+
+**NOTE**: The ``PUT-as-create`` functionality doesn't have tests (yet).
+
+License
+-------
+
+MIT
+
+Inspiration
+-----------
+
+This functionality in DRF is something I've needed in numerous Django projects, so hopefully this will help someone else
+too :)
+
+This package has been built on top of the ideas presented by the great vintasoftware's ``drf-rw-serializers`` (https://github.com/vintasoftware/drf-rw-serializers) package. Thanks!
```

### Comparing `drf-crud-proxy-0.3.1/README.rst` & `drf-crud-proxy-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 This is super handy in situations where you want to, for example, let the user send a ForeignKey attribute,
 but present the related object alongside the response instead of only the database ID.
 
 Requirements
 ------------
 
-- Python 3.6, 3.7, 3.8 and 3.9 (probably older versions as well)
-- Django 2.2, 3.0, 3.1 and 3.2 (basically works with older versions as well, but they're EOL)
+- Python 3.6, 3.7, 3.8, 3.9, 3.10 and 3.11
+- Django 3.2, 4.0, 4.1 and 4.2 (basically works with older versions as well, but they're EOL)
 - Django REST Framework 3.8 or newer (probably works on any 3.x version)
 
 Installation
 ------------
 
 .. code::
```

### Comparing `drf-crud-proxy-0.3.1/drf_crud_proxy/generics.py` & `drf-crud-proxy-0.4.0/drf_crud_proxy/generics.py`

 * *Files identical despite different names*

### Comparing `drf-crud-proxy-0.3.1/drf_crud_proxy/mixins.py` & `drf-crud-proxy-0.4.0/drf_crud_proxy/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-crud-proxy-0.3.1/drf_crud_proxy/proxy.py` & `drf-crud-proxy-0.4.0/drf_crud_proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `drf-crud-proxy-0.3.1/drf_crud_proxy/viewsets.py` & `drf-crud-proxy-0.4.0/drf_crud_proxy/viewsets.py`

 * *Files identical despite different names*

### Comparing `drf-crud-proxy-0.3.1/drf_crud_proxy.egg-info/PKG-INFO` & `drf-crud-proxy-0.4.0/drf_crud_proxy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,93 @@
 Metadata-Version: 2.1
 Name: drf-crud-proxy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Separate serializers for parsing requests and returning responses in DRF
-Home-page: https://github.com/attevaltonen/drf-crud-proxy
-Author: attevaltonen
-Author-email: atte.hj.valtonen@gmail.com
+Home-page: https://github.com/attevaltojarvi/drf-crud-proxy
+Author: attevaltojarvi
+Author-email: atte.valtojarvi@gmail.com
 License: MIT
-Description: DRF CRUD Proxy
-        ==============
-        
-        This package provides extended Django REST Framework generic views and viewsets that provide the possibility to specify
-        different serializers for reading the incoming request and presenting the response.
-        
-        This is super handy in situations where you want to, for example, let the user send a ForeignKey attribute,
-        but present the related object alongside the response instead of only the database ID.
-        
-        Requirements
-        ------------
-        
-        - Python 3.6, 3.7, 3.8 and 3.9 (probably older versions as well)
-        - Django 2.2, 3.0, 3.1 and 3.2 (basically works with older versions as well, but they're EOL)
-        - Django REST Framework 3.8 or newer (probably works on any 3.x version)
-        
-        Installation
-        ------------
-        
-        .. code::
-        
-          pip install drf-crud-proxy
-        
-        Usage
-        -----
-        
-        Import the generic views and subclass your own views from them. Specify ``request_serializer_class`` and/or
-        ``response_serializer_class`` to the view (both default to DRF's own ``serializer_class`` attribute).
-        
-        .. code:: python
-        
-          # api/views.py
-        
-          from drf_crud_proxy import generics
-          from app.models import MyModel
-          from api.serializers import MyModelCreateSerializer, MyModelSerializer
-        
-        
-          class MyModelListCreateView(generics.ProxiedListCreateAPIView):
-              queryset = MyModel.objects.all()
-              request_serializer_class = MyModelCreateSerializer
-              response_serializer_class = MyModelSerializer
-        
-        The incoming request is handled with ``MyModelCreateSerializer`` and the response with ``MyModelSerializer``.
-        
-        If you want to customize the data on either situation, override ``get_request_data`` and/or ``get_response_data``
-        methods in the view.
-        
-        The package also supports the so-called ``PUT-as-create`` behavior that was removed from DRF in its 3.0 release. Note that
-        the user has to have model permissions for the corresponding create behavior (``POST`` request).
-        
-        **NOTE**: The ``PUT-as-create`` functionality doesn't have tests (yet).
-        
-        License
-        -------
-        
-        MIT
-        
-        Inspiration
-        -----------
-        
-        This functionality in DRF is something I've needed in numerous Django projects, so hopefully this will help someone else
-        too :)
-        
-        This package has been built on top of the ideas presented by the great vintasoftware's ``drf-rw-serializers`` (https://github.com/vintasoftware/drf-rw-serializers) package. Thanks!
-        
 Keywords: Django REST Framework,Serializers,REST,API,Django
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Finnish
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+DRF CRUD Proxy
+==============
+
+This package provides extended Django REST Framework generic views and viewsets that provide the possibility to specify
+different serializers for reading the incoming request and presenting the response.
+
+This is super handy in situations where you want to, for example, let the user send a ForeignKey attribute,
+but present the related object alongside the response instead of only the database ID.
+
+Requirements
+------------
+
+- Python 3.6, 3.7, 3.8, 3.9, 3.10 and 3.11
+- Django 3.2, 4.0, 4.1 and 4.2 (basically works with older versions as well, but they're EOL)
+- Django REST Framework 3.8 or newer (probably works on any 3.x version)
+
+Installation
+------------
+
+.. code::
+
+  pip install drf-crud-proxy
+
+Usage
+-----
+
+Import the generic views and subclass your own views from them. Specify ``request_serializer_class`` and/or
+``response_serializer_class`` to the view (both default to DRF's own ``serializer_class`` attribute).
+
+.. code:: python
+
+  # api/views.py
+
+  from drf_crud_proxy import generics
+  from app.models import MyModel
+  from api.serializers import MyModelCreateSerializer, MyModelSerializer
+
+
+  class MyModelListCreateView(generics.ProxiedListCreateAPIView):
+      queryset = MyModel.objects.all()
+      request_serializer_class = MyModelCreateSerializer
+      response_serializer_class = MyModelSerializer
+
+The incoming request is handled with ``MyModelCreateSerializer`` and the response with ``MyModelSerializer``.
+
+If you want to customize the data on either situation, override ``get_request_data`` and/or ``get_response_data``
+methods in the view.
+
+The package also supports the so-called ``PUT-as-create`` behavior that was removed from DRF in its 3.0 release. Note that
+the user has to have model permissions for the corresponding create behavior (``POST`` request).
+
+**NOTE**: The ``PUT-as-create`` functionality doesn't have tests (yet).
+
+License
+-------
+
+MIT
+
+Inspiration
+-----------
+
+This functionality in DRF is something I've needed in numerous Django projects, so hopefully this will help someone else
+too :)
+
+This package has been built on top of the ideas presented by the great vintasoftware's ``drf-rw-serializers`` (https://github.com/vintasoftware/drf-rw-serializers) package. Thanks!
```

### Comparing `drf-crud-proxy-0.3.1/setup.py` & `drf-crud-proxy-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,37 +28,39 @@
 
 setup(
     name="drf-crud-proxy",
     version=VERSION,
     description="Separate serializers for parsing requests and returning responses in DRF",
     long_description=README,
     long_description_content_type="text/x-rst",
-    author="attevaltonen",
-    author_email="atte.hj.valtonen@gmail.com",
-    url="https://github.com/attevaltonen/drf-crud-proxy",
+    author="attevaltojarvi",
+    author_email="atte.valtojarvi@gmail.com",
+    url="https://github.com/attevaltojarvi/drf-crud-proxy",
     packages=find_packages(exclude=("example_app", "test_utils", "tests")),
     include_package_data=True,
     install_requires=[
-        "Django>=2.2,<3.3",
+        "Django>=3.2,<5.0",
         "djangorestframework>=3.8"
     ],
     license="MIT",
     zip_safe=False,
     keywords="Django REST Framework, Serializers, REST, API, Django",
     test_suite="tox",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: Finnish",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9"
-    ],
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
+    ]
 )
```

