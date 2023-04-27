# Comparing `tmp/datatable-faker-0.1.4.tar.gz` & `tmp/datatable-faker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-faker-0.1.4.tar", last modified: Thu Apr 27 07:03:16 2023, max compression
+gzip compressed data, was "datatable-faker-0.1.5.tar", last modified: Thu Apr 27 07:20:57 2023, max compression
```

## Comparing `datatable-faker-0.1.4.tar` & `datatable-faker-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/
--rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.4/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      982 2023-04-27 07:01:46.000000 datatable-faker-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/datatable_faker/
--rw-rw-r--   0 root         (0) root         (0)     4964 2023-04-27 06:59:33.000000 datatable-faker-0.1.4/src/datatable_faker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1410 2023-04-26 05:03:55.000000 datatable-faker-0.1.4/src/datatable_faker/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/datatable_faker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      302 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/
+-rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.5/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      982 2023-04-27 07:20:46.000000 datatable-faker-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/src/datatable_faker/
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-04-27 07:20:35.000000 datatable-faker-0.1.5/src/datatable_faker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-04-26 05:03:55.000000 datatable-faker-0.1.5/src/datatable_faker/check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:20:57.329018 datatable-faker-0.1.5/src/datatable_faker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:20:57.000000 datatable-faker-0.1.5/src/datatable_faker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-27 07:20:57.000000 datatable-faker-0.1.5/src/datatable_faker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:20:57.000000 datatable-faker-0.1.5/src/datatable_faker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 07:20:57.000000 datatable-faker-0.1.5/src/datatable_faker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 07:20:57.000000 datatable-faker-0.1.5/src/datatable_faker.egg-info/top_level.txt
```

### Comparing `datatable-faker-0.1.4/LICENSE` & `datatable-faker-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.4/PKG-INFO` & `datatable-faker-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datatable-faker-0.1.4/README.rst` & `datatable-faker-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.4/setup.py` & `datatable-faker-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="datatable-faker",
     author="Prince Roshan",
-    version='0.1.4',
+    version='0.1.5',
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/Agent-Hellboy/datatable-faker",
     description="Library to generate fake datatable for unittest ",
     long_description=read("README.rst"),
     license="MIT",
     package_dir={'': 'src'},
     packages=['datatable_faker'],
```

### Comparing `datatable-faker-0.1.4/src/datatable_faker/__init__.py` & `datatable-faker-0.1.5/src/datatable_faker/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,47 +50,47 @@
         elif field_type is float:
             fake_data[field.name] = fake.pyfloat()
         elif field_type is str:
             fake_data[field.name] = fake.word()
         elif field_type is bool:
             fake_data[field.name] = fake.boolean()
         elif issubclass(field_type, BaseModel):
-            fake_data[field.name] = generate_fake_data(field_type)
+            fake_data[field.name] = generate_fake_dataa_from_pydentic(field_type)
         elif field_type is List[int]:
             fake_data[field.name] = [fake.random_int() for _ in range(3)]
         elif field_type is List[float]:
             fake_data[field.name] = [fake.pyfloat() for _ in range(3)]
         elif field_type is List[str]:
             fake_data[field.name] = [fake.word() for _ in range(3)]
         elif field_type is List[bool]:
             fake_data[field.name] = [fake.boolean() for _ in range(3)]
         elif field_type.__origin__ is list:
             inner_type = field_type.__args__[0]
-            fake_data[field.name] = [generate_fake_data(inner_type) for _ in range(3)]
+            fake_data[field.name] = [generate_fake_data_from_pydentic(inner_type) for _ in range(3)]
         elif field_type is Dict[str, int]:
             fake_data[field.name] = {fake.word(): fake.random_int() for _ in range(3)}
         elif field_type is Dict[str, float]:
             fake_data[field.name] = {fake.word(): fake.pyfloat() for _ in range(3)}
         elif field_type is Dict[str, str]:
             fake_data[field.name] = {fake.word(): fake.word() for _ in range(3)}
         elif field_type is Dict[str, bool]:
             fake_data[field.name] = {fake.word(): fake.boolean() for _ in range(3)}
         elif field_type.__origin__ is dict:
             key_type, value_type = field_type.__args__
-            fake_data[field.name] = {generate_fake_data(key_type): generate_fake_data(value_type) for _ in range(3)}
+            fake_data[field.name] = {generate_fake_data_from_pydentic(key_type): generate_fake_data_from_pydentic(value_type) for _ in range(3)}
         elif field_type is Tuple[int, str]:
             fake_data[field.name] = (fake.random_int(), fake.word())
         elif field_type is Tuple[int, str, bool]:
             fake_data[field.name] = (fake.random_int(), fake.word(), fake.boolean())
         elif field_type is Tuple[int, str, bool, float]:
             fake_data[field.name] = (fake.random_int(), fake.word(), fake.boolean(), fake.pyfloat())
         elif field_type.__origin__ is tuple:
             inner_types = field_type.__args__
-            fake_data[field.name] = tuple(generate_fake_data(inner_type) for inner_type in inner_types)
+            fake_data[field.name] = tuple(generate_fake_data_from_pydentic(inner_type) for inner_type in inner_types)
         elif field_type is Union[int, str]:
             fake_data[field.name] = fake.random_element([fake.random_int(), fake.word()])
         elif field_type is Optional[int]:
             fake_data[field.name] = fake.random_element([fake.random_int(), None])
         elif field_type.__origin__ is Union:
             inner_types = field_type.__args__
-            fake_data[field.name] = fake.random_element([generate_fake_data(inner_type) for inner_type in inner_types])
-    return model_class(**fake_data)
+            fake_data[field.name] = fake.random_element([generate_fake_data_from_pydentic(inner_type) for inner_type in inner_types])
+    return model_class(**fake_data)
```

### Comparing `datatable-faker-0.1.4/src/datatable_faker/check.py` & `datatable-faker-0.1.5/src/datatable_faker/check.py`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.4/src/datatable_faker.egg-info/PKG-INFO` & `datatable-faker-0.1.5/src/datatable_faker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
```

