# Comparing `tmp/PYB11Generator-2.0.3.tar.gz` & `tmp/PYB11Generator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/usr/WS2/owen/projects/PYB11Generator/dist/.tmp-ib1fdt6q/PYB11Generator-2.0.3.tar", last modified: Thu Mar 30 17:06:42 2023, max compression
+gzip compressed data, was "dist/PYB11Generator-2.1.0.tar", last modified: Thu Apr 27 18:26:34 2023, max compression
```

## Comparing `PYB11Generator-2.0.3.tar` & `PYB11Generator-2.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:42.000000 PYB11Generator-2.0.3/
--rw-------   0 owen      (5769) owen      (5769)       48 2019-08-20 18:11:30.000000 PYB11Generator-2.0.3/.gitignore
--rw-------   0 owen      (5769) owen      (5769)      113 2023-03-28 23:44:28.000000 PYB11Generator-2.0.3/.gitmodules
--rw-------   0 owen      (5769) owen      (5769)     1487 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)     1542 2019-02-21 18:49:03.000000 PYB11Generator-2.0.3/LICENSE
--rw-------   0 owen      (5769) owen      (5769)      111 2023-03-23 22:49:20.000000 PYB11Generator-2.0.3/MANIFEST.in
--rw-------   0 owen      (5769) owen      (5769)     1167 2019-02-21 18:47:19.000000 PYB11Generator-2.0.3/NOTICE
--rw-------   0 owen      (5769) owen      (5769)     2826 2023-03-30 17:06:42.000000 PYB11Generator-2.0.3/PKG-INFO
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/PYB11Generator/
--rw-------   0 owen      (5769) owen      (5769)     3095 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11ClassAttribute.py
--rw-------   0 owen      (5769) owen      (5769)     7712 2021-10-26 20:13:37.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11Decorators.py
--rw-------   0 owen      (5769) owen      (5769)     3503 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11Publicist.py
--rw-------   0 owen      (5769) owen      (5769)     3382 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11STLmethods.py
--rw-------   0 owen      (5769) owen      (5769)    10914 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11Trampoline.py
--rw-------   0 owen      (5769) owen      (5769)     1430 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11attr.py
--rw-------   0 owen      (5769) owen      (5769)    26552 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11class.py
--rw-------   0 owen      (5769) owen      (5769)     3018 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11enum.py
--rw-------   0 owen      (5769) owen      (5769)     7082 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11function.py
--rw-------   0 owen      (5769) owen      (5769)     7091 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11property.py
--rw-------   0 owen      (5769) owen      (5769)    18670 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/PYB11Generator/PYB11utils.py
--rw-------   0 owen      (5769) owen      (5769)     4426 2023-03-23 22:49:20.000000 PYB11Generator-2.0.3/PYB11Generator/__init__.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/
--rw-------   0 owen      (5769) owen      (5769)     2826 2023-03-30 17:06:39.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/PKG-INFO
--rw-------   0 owen      (5769) owen      (5769)     1759 2023-03-30 17:06:40.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/SOURCES.txt
--rw-------   0 owen      (5769) owen      (5769)        1 2023-03-30 17:06:39.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/dependency_links.txt
--rw-------   0 owen      (5769) owen      (5769)       19 2023-03-30 17:06:39.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/requires.txt
--rw-------   0 owen      (5769) owen      (5769)       15 2023-03-30 17:06:39.000000 PYB11Generator-2.0.3/PYB11Generator.egg-info/top_level.txt
--rw-------   0 owen      (5769) owen      (5769)     2074 2019-02-21 19:28:27.000000 PYB11Generator-2.0.3/README.md
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/cmake/
--rw-------   0 owen      (5769) owen      (5769)     8843 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/cmake/FindSphinx.cmake
--rw-------   0 owen      (5769) owen      (5769)     9748 2023-03-23 22:49:21.000000 PYB11Generator-2.0.3/cmake/PYB11Generator.cmake
--rw-------   0 owen      (5769) owen      (5769)     2961 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/cmake/add_sphinx_target.cmake
--rw-------   0 owen      (5769) owen      (5769)      927 2023-03-23 22:49:21.000000 PYB11Generator-2.0.3/cmake/generate_cpp.py
--rw-------   0 owen      (5769) owen      (5769)      980 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/cmake/moduleCheck.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/docs/
--rw-------   0 owen      (5769) owen      (5769)       26 2019-02-21 18:18:02.000000 PYB11Generator-2.0.3/docs/.gitignore
--rw-------   0 owen      (5769) owen      (5769)      826 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)      580 2019-02-21 18:18:01.000000 PYB11Generator-2.0.3/docs/Makefile
--rw-------   0 owen      (5769) owen      (5769)     6551 2019-02-21 18:22:50.000000 PYB11Generator-2.0.3/docs/PYB11decorators.rst
--rw-------   0 owen      (5769) owen      (5769)    10638 2023-03-23 22:49:21.000000 PYB11Generator-2.0.3/docs/PYB11functions.rst
--rw-------   0 owen      (5769) owen      (5769)     5560 2019-05-06 18:54:55.000000 PYB11Generator-2.0.3/docs/PYB11variables.rst
--rw-------   0 owen      (5769) owen      (5769)    34756 2019-03-06 23:49:23.000000 PYB11Generator-2.0.3/docs/classes.rst
--rw-------   0 owen      (5769) owen      (5769)     4687 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/cmake.rst
--rw-------   0 owen      (5769) owen      (5769)     7017 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/complications.rst
--rw-------   0 owen      (5769) owen      (5769)     5886 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/conf.py
--rw-------   0 owen      (5769) owen      (5769)     1387 2019-02-21 18:18:02.000000 PYB11Generator-2.0.3/docs/enums.rst
--rw-------   0 owen      (5769) owen      (5769)    12857 2019-03-04 22:39:16.000000 PYB11Generator-2.0.3/docs/functions.rst
--rw-------   0 owen      (5769) owen      (5769)     1974 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/index.rst
--rw-------   0 owen      (5769) owen      (5769)     7335 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/docs/intro.rst
--rw-------   0 owen      (5769) owen      (5769)      787 2019-02-21 18:18:01.000000 PYB11Generator-2.0.3/docs/make.bat
--rw-------   0 owen      (5769) owen      (5769)     6141 2019-02-21 18:18:02.000000 PYB11Generator-2.0.3/docs/memory.rst
--rw-------   0 owen      (5769) owen      (5769)     6149 2019-02-21 18:18:02.000000 PYB11Generator-2.0.3/docs/pybind11_objects.inv
--rw-------   0 owen      (5769) owen      (5769)    31044 2019-02-21 18:18:02.000000 PYB11Generator-2.0.3/docs/pybind11_objects.txt
--rw-------   0 owen      (5769) owen      (5769)     3179 2019-02-21 18:18:01.000000 PYB11Generator-2.0.3/docs/stl.rst
--rw-------   0 owen      (5769) owen      (5769)      793 2023-03-30 16:56:52.000000 PYB11Generator-2.0.3/pyproject.toml
--rw-------   0 owen      (5769) owen      (5769)       38 2023-03-30 17:06:42.000000 PYB11Generator-2.0.3/setup.cfg
--rw-------   0 owen      (5769) owen      (5769)     1412 2023-03-30 16:56:50.000000 PYB11Generator-2.0.3/setup.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:40.000000 PYB11Generator-2.0.3/tests/
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/tests/cross_module/
--rw-------   0 owen      (5769) owen      (5769)      201 2018-12-05 23:53:49.000000 PYB11Generator-2.0.3/tests/cross_module/A.hh
--rw-------   0 owen      (5769) owen      (5769)      225 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/tests/cross_module/A_PYB11.py
--rw-------   0 owen      (5769) owen      (5769)      257 2018-12-05 23:55:12.000000 PYB11Generator-2.0.3/tests/cross_module/B.hh
--rw-------   0 owen      (5769) owen      (5769)      234 2023-01-21 00:52:30.000000 PYB11Generator-2.0.3/tests/cross_module/B_PYB11.py
--rw-------   0 owen      (5769) owen      (5769)      160 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/cross_module/CMakeLists.txt
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/tests/inheritance/
--rw-------   0 owen      (5769) owen      (5769)      312 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inheritance/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)     1667 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inheritance/change_templates_PYB11.py
--rw-------   0 owen      (5769) owen      (5769)      890 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inheritance/inherit_base_virtual_methods_PYB11.py
--rw-------   0 owen      (5769) owen      (5769)     1533 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inheritance/nontemplate_inherit_from_template_PYB11.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:41.000000 PYB11Generator-2.0.3/tests/inject/
--rw-------   0 owen      (5769) owen      (5769)       84 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inject/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)      586 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/inject/inject_test_PYB11.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:42.000000 PYB11Generator-2.0.3/tests/numpy/
--rw-------   0 owen      (5769) owen      (5769)       41 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/numpy/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)      271 2019-05-06 18:54:56.000000 PYB11Generator-2.0.3/tests/numpy/my_array.hh
--rw-------   0 owen      (5769) owen      (5769)      780 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/numpy/test_np_array_PYB11.py
-drwx------   0 owen      (5769) owen      (5769)        0 2023-03-30 17:06:42.000000 PYB11Generator-2.0.3/tests/protected/
--rw-------   0 owen      (5769) owen      (5769)      422 2019-03-11 21:35:32.000000 PYB11Generator-2.0.3/tests/protected/A.py
--rw-------   0 owen      (5769) owen      (5769)      436 2019-03-11 21:35:42.000000 PYB11Generator-2.0.3/tests/protected/B.py
--rw-------   0 owen      (5769) owen      (5769)       88 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/protected/CMakeLists.txt
--rw-------   0 owen      (5769) owen      (5769)      556 2019-03-11 21:34:13.000000 PYB11Generator-2.0.3/tests/protected/protected.hh
--rw-------   0 owen      (5769) owen      (5769)      153 2023-01-21 00:52:31.000000 PYB11Generator-2.0.3/tests/protected/protected_PYB11.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/
+-rw-------   0 owen      (5769) owen      (5769)       48 2019-08-20 18:11:30.000000 PYB11Generator-2.1.0/.gitignore
+-rw-------   0 owen      (5769) owen      (5769)      113 2023-03-28 23:44:28.000000 PYB11Generator-2.1.0/.gitmodules
+-rw-------   0 owen      (5769) owen      (5769)     1487 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)     1542 2019-02-21 18:49:03.000000 PYB11Generator-2.1.0/LICENSE
+-rw-------   0 owen      (5769) owen      (5769)      111 2023-03-23 22:49:20.000000 PYB11Generator-2.1.0/MANIFEST.in
+-rw-------   0 owen      (5769) owen      (5769)     1167 2019-02-21 18:47:19.000000 PYB11Generator-2.1.0/NOTICE
+-rw-------   0 owen      (5769) owen      (5769)     2758 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/PKG-INFO
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:33.000000 PYB11Generator-2.1.0/PYB11Generator/
+-rw-------   0 owen      (5769) owen      (5769)     3095 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11ClassAttribute.py
+-rw-------   0 owen      (5769) owen      (5769)     7957 2023-04-26 23:27:12.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11Decorators.py
+-rw-------   0 owen      (5769) owen      (5769)     3503 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11Publicist.py
+-rw-------   0 owen      (5769) owen      (5769)     3382 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11STLmethods.py
+-rw-------   0 owen      (5769) owen      (5769)    10914 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11Trampoline.py
+-rw-------   0 owen      (5769) owen      (5769)     1430 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11attr.py
+-rw-------   0 owen      (5769) owen      (5769)    26934 2023-04-26 23:27:13.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11class.py
+-rw-------   0 owen      (5769) owen      (5769)     3018 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11enum.py
+-rw-------   0 owen      (5769) owen      (5769)     7082 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11function.py
+-rw-------   0 owen      (5769) owen      (5769)     7091 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11property.py
+-rw-------   0 owen      (5769) owen      (5769)    18712 2023-04-26 23:27:13.000000 PYB11Generator-2.1.0/PYB11Generator/PYB11utils.py
+-rw-------   0 owen      (5769) owen      (5769)     4426 2023-03-23 22:49:20.000000 PYB11Generator-2.1.0/PYB11Generator/__init__.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/
+-rw-------   0 owen      (5769) owen      (5769)     2758 2023-04-27 18:26:32.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/PKG-INFO
+-rw-------   0 owen      (5769) owen      (5769)     1759 2023-04-27 18:26:33.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/SOURCES.txt
+-rw-------   0 owen      (5769) owen      (5769)        1 2023-04-27 18:26:32.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/dependency_links.txt
+-rw-------   0 owen      (5769) owen      (5769)       19 2023-04-27 18:26:32.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/requires.txt
+-rw-------   0 owen      (5769) owen      (5769)       15 2023-04-27 18:26:32.000000 PYB11Generator-2.1.0/PYB11Generator.egg-info/top_level.txt
+-rw-------   0 owen      (5769) owen      (5769)     2074 2019-02-21 19:28:27.000000 PYB11Generator-2.1.0/README.md
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/cmake/
+-rw-------   0 owen      (5769) owen      (5769)     8843 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/cmake/FindSphinx.cmake
+-rw-------   0 owen      (5769) owen      (5769)     9748 2023-03-23 22:49:21.000000 PYB11Generator-2.1.0/cmake/PYB11Generator.cmake
+-rw-------   0 owen      (5769) owen      (5769)     2961 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/cmake/add_sphinx_target.cmake
+-rw-------   0 owen      (5769) owen      (5769)      927 2023-03-23 22:49:21.000000 PYB11Generator-2.1.0/cmake/generate_cpp.py
+-rw-------   0 owen      (5769) owen      (5769)      980 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/cmake/moduleCheck.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/docs/
+-rw-------   0 owen      (5769) owen      (5769)       26 2019-02-21 18:18:02.000000 PYB11Generator-2.1.0/docs/.gitignore
+-rw-------   0 owen      (5769) owen      (5769)      826 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)      580 2019-02-21 18:18:01.000000 PYB11Generator-2.1.0/docs/Makefile
+-rw-------   0 owen      (5769) owen      (5769)     6899 2023-04-26 23:27:13.000000 PYB11Generator-2.1.0/docs/PYB11decorators.rst
+-rw-------   0 owen      (5769) owen      (5769)    10638 2023-03-23 22:49:21.000000 PYB11Generator-2.1.0/docs/PYB11functions.rst
+-rw-------   0 owen      (5769) owen      (5769)     5560 2019-05-06 18:54:55.000000 PYB11Generator-2.1.0/docs/PYB11variables.rst
+-rw-------   0 owen      (5769) owen      (5769)    35574 2023-04-26 23:27:13.000000 PYB11Generator-2.1.0/docs/classes.rst
+-rw-------   0 owen      (5769) owen      (5769)     4687 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/cmake.rst
+-rw-------   0 owen      (5769) owen      (5769)     7017 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/complications.rst
+-rw-------   0 owen      (5769) owen      (5769)     5886 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/conf.py
+-rw-------   0 owen      (5769) owen      (5769)     1387 2019-02-21 18:18:02.000000 PYB11Generator-2.1.0/docs/enums.rst
+-rw-------   0 owen      (5769) owen      (5769)    12857 2019-03-04 22:39:16.000000 PYB11Generator-2.1.0/docs/functions.rst
+-rw-------   0 owen      (5769) owen      (5769)     1974 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/index.rst
+-rw-------   0 owen      (5769) owen      (5769)     7335 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/docs/intro.rst
+-rw-------   0 owen      (5769) owen      (5769)      787 2019-02-21 18:18:01.000000 PYB11Generator-2.1.0/docs/make.bat
+-rw-------   0 owen      (5769) owen      (5769)     6141 2019-02-21 18:18:02.000000 PYB11Generator-2.1.0/docs/memory.rst
+-rw-------   0 owen      (5769) owen      (5769)     6149 2019-02-21 18:18:02.000000 PYB11Generator-2.1.0/docs/pybind11_objects.inv
+-rw-------   0 owen      (5769) owen      (5769)    31044 2019-02-21 18:18:02.000000 PYB11Generator-2.1.0/docs/pybind11_objects.txt
+-rw-------   0 owen      (5769) owen      (5769)     3179 2019-02-21 18:18:01.000000 PYB11Generator-2.1.0/docs/stl.rst
+-rw-------   0 owen      (5769) owen      (5769)      793 2023-04-27 16:48:21.000000 PYB11Generator-2.1.0/pyproject.toml
+-rw-------   0 owen      (5769) owen      (5769)       38 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/setup.cfg
+-rw-------   0 owen      (5769) owen      (5769)     1412 2023-04-27 16:48:30.000000 PYB11Generator-2.1.0/setup.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:33.000000 PYB11Generator-2.1.0/tests/
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/tests/cross_module/
+-rw-------   0 owen      (5769) owen      (5769)      201 2018-12-05 23:53:49.000000 PYB11Generator-2.1.0/tests/cross_module/A.hh
+-rw-------   0 owen      (5769) owen      (5769)      225 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/tests/cross_module/A_PYB11.py
+-rw-------   0 owen      (5769) owen      (5769)      257 2018-12-05 23:55:12.000000 PYB11Generator-2.1.0/tests/cross_module/B.hh
+-rw-------   0 owen      (5769) owen      (5769)      234 2023-01-21 00:52:30.000000 PYB11Generator-2.1.0/tests/cross_module/B_PYB11.py
+-rw-------   0 owen      (5769) owen      (5769)      160 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/cross_module/CMakeLists.txt
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/tests/inheritance/
+-rw-------   0 owen      (5769) owen      (5769)      312 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inheritance/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)     1667 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inheritance/change_templates_PYB11.py
+-rw-------   0 owen      (5769) owen      (5769)      890 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inheritance/inherit_base_virtual_methods_PYB11.py
+-rw-------   0 owen      (5769) owen      (5769)     1533 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inheritance/nontemplate_inherit_from_template_PYB11.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/tests/inject/
+-rw-------   0 owen      (5769) owen      (5769)       84 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inject/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)      586 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/inject/inject_test_PYB11.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/tests/numpy/
+-rw-------   0 owen      (5769) owen      (5769)       41 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/numpy/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)      271 2019-05-06 18:54:56.000000 PYB11Generator-2.1.0/tests/numpy/my_array.hh
+-rw-------   0 owen      (5769) owen      (5769)      780 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/numpy/test_np_array_PYB11.py
+drwx------   0 owen      (5769) owen      (5769)        0 2023-04-27 18:26:34.000000 PYB11Generator-2.1.0/tests/protected/
+-rw-------   0 owen      (5769) owen      (5769)      422 2019-03-11 21:35:32.000000 PYB11Generator-2.1.0/tests/protected/A.py
+-rw-------   0 owen      (5769) owen      (5769)      436 2019-03-11 21:35:42.000000 PYB11Generator-2.1.0/tests/protected/B.py
+-rw-------   0 owen      (5769) owen      (5769)       88 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/protected/CMakeLists.txt
+-rw-------   0 owen      (5769) owen      (5769)      556 2019-03-11 21:34:13.000000 PYB11Generator-2.1.0/tests/protected/protected.hh
+-rw-------   0 owen      (5769) owen      (5769)      153 2023-01-21 00:52:31.000000 PYB11Generator-2.1.0/tests/protected/protected_PYB11.py
```

### Comparing `PYB11Generator-2.0.3/CMakeLists.txt` & `PYB11Generator-2.1.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/LICENSE` & `PYB11Generator-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/NOTICE` & `PYB11Generator-2.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PKG-INFO` & `PYB11Generator-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: PYB11Generator
-Version: 2.0.3
-Summary: PYB11Generator is a code generation tool which generates pybind11 code for binding C++ to Python. Documentation is available at https://pyb11generator.readthedocs.io/
+Version: 2.1.0
+Summary: A code generator for the pybind11 C++ <-> Python language binding tool
 Home-page: https://github.com/jmikeowen/PYB11Generator
 Author: J. Michael Owen
-Author-email: "J. Michael Owen" <mikeowen@llnl.gov>
-Project-URL: Homepage, https://github.com/LLNL/PYB11Generator
-Project-URL: Bug Tracker, https://github.com/LLNL/PYB11Generator/issues
+Author-email: mikeowen@llnl.gov
+License: UNKNOWN
+Description: PYB11Generator
+        ==============
+        
+        PYB11Generator is a python based code generator that creates [pybind11](https://github.com/pybind/pybind11) code for binding C++ libraries as extensions in Python. PYB11Generator parses input that is very close to writing the desired interface in native python, turning this into the corresponding pybind11 C++ code.
+        
+        Note, since PYB11Generator blindly generates C++ pybind11 code, it is essential to understand the pybind11 package itself as well!  In other words, be sure to read and understand the [pybind11 documentation](https://pybind11.readthedocs.io/en/stable/) before trying to go too far with PYB11Generator.  The purpose of PYB11Generator is to reduce the burden of writing and maintaining redundant code when working with pybind11 (such as the [trampoline classes](https://pybind11.readthedocs.io/en/stable/advanced/classes.html#overriding-virtual-functions-in-python)), and provide a natural syntax for those already familiar with writing interfaces in Python.  However, since the generated pybind11 code produced by PYB11Generator is what is actually compiled by a C++ compiler to create the corresponding python package, any errors reported by the compiler will refer to this generated code, and require understanding pybind11 itself to properly interpret.
+        
+        Documentation
+        -------------
+        
+        PYB11Generator is documented at [readthedocs](https://pyb11generator.readthedocs.io/en/latest/).
+        
+        Note the source for this documentation is embedded in the PYB11Generator repository under docs/.
+        
+        Contributions
+        -------------
+        
+        Although a great deal of the functionality of pybind11 is available via PYB11Generator, there are certainly missing pieces and improvements that can be made.  Contributions are welcome, and should be provided as pull requests to the main repository.  Note all contributions must be provided under the same license for distribution (in this case the BSD license).
+        
+        License
+        -------
+        
+        PYB11Generator is released under the [BSD license](https://github.com/jmikeowen/PYB11Generator/blob/master/LICENSE).
+        
+        LLNL-CODE-767799
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
-PYB11Generator
-==============
-
-PYB11Generator is a python based code generator that creates [pybind11](https://github.com/pybind/pybind11) code for binding C++ libraries as extensions in Python. PYB11Generator parses input that is very close to writing the desired interface in native python, turning this into the corresponding pybind11 C++ code.
-
-Note, since PYB11Generator blindly generates C++ pybind11 code, it is essential to understand the pybind11 package itself as well!  In other words, be sure to read and understand the [pybind11 documentation](https://pybind11.readthedocs.io/en/stable/) before trying to go too far with PYB11Generator.  The purpose of PYB11Generator is to reduce the burden of writing and maintaining redundant code when working with pybind11 (such as the [trampoline classes](https://pybind11.readthedocs.io/en/stable/advanced/classes.html#overriding-virtual-functions-in-python)), and provide a natural syntax for those already familiar with writing interfaces in Python.  However, since the generated pybind11 code produced by PYB11Generator is what is actually compiled by a C++ compiler to create the corresponding python package, any errors reported by the compiler will refer to this generated code, and require understanding pybind11 itself to properly interpret.
-
-Documentation
--------------
-
-PYB11Generator is documented at [readthedocs](https://pyb11generator.readthedocs.io/en/latest/).
-
-Note the source for this documentation is embedded in the PYB11Generator repository under docs/.
-
-Contributions
--------------
-
-Although a great deal of the functionality of pybind11 is available via PYB11Generator, there are certainly missing pieces and improvements that can be made.  Contributions are welcome, and should be provided as pull requests to the main repository.  Note all contributions must be provided under the same license for distribution (in this case the BSD license).
-
-License
--------
-
-PYB11Generator is released under the [BSD license](https://github.com/jmikeowen/PYB11Generator/blob/master/LICENSE).
-
-LLNL-CODE-767799
```

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11ClassAttribute.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11ClassAttribute.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11Decorators.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11Decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,7 +213,14 @@
         self.val = x
         return
     def __call__(self, thing):
         if not hasattr(thing, "PYB11module"):
             thing.PYB11module = {}
         thing.PYB11module[thing] = self.val
         return thing
+
+#-------------------------------------------------------------------------------
+# operator (method)
+#-------------------------------------------------------------------------------
+def PYB11operator(f):
+    f.PYB11operator = True
+    return f
```

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11Publicist.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11Publicist.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11STLmethods.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11STLmethods.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11Trampoline.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11Trampoline.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11attr.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11attr.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11class.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11class.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,20 @@
         ss(", py::keep_alive<%i, %i>()" % methattrs["keepalive"])
 
     # Write the doc string
     doc = inspect.getdoc(meth)
     if doc:
         ss(", ")
         PYB11docstring(doc, ss)
+
+    # Is this an operator method?
+    if methattrs["operator"]:
+        ss(", py::is_operator()")
+        
+    # Done
     ss(");\n")
 
 #-------------------------------------------------------------------------------
 # PYB11generateClass
 #
 # Bind the methods for the given class
 #-------------------------------------------------------------------------------
@@ -357,33 +363,36 @@
     special_operators =  {"__init__": (ignore, ""),
 
                           "__call__": (call_operator, ""),
 
                           "__add__" : (binary_operator, "+"),
                           "__sub__" : (binary_operator, "-"),
                           "__mul__" : (binary_operator, "*"),
-                          "__div__" : (binary_operator, "/"),
+                          "__truediv__" : (binary_operator, "/"),
+                          "__floordiv__" : (binary_operator, "//"),
                           "__mod__" : (binary_operator, "%"),
                           "__and__" : (binary_operator, "&"),
                           "__xor__" : (binary_operator, "^"),
                           "__or__"  : (binary_operator, "|"),
                           
                           "__radd__" : (reverse_binary_operator, "+"),
                           "__rsub__" : (reverse_binary_operator, "-"),
                           "__rmul__" : (reverse_binary_operator, "*"),
-                          "__rdiv__" : (reverse_binary_operator, "/"),
+                          "__rtruediv__" : (reverse_binary_operator, "/"),
+                          "__rfloordiv__" : (reverse_binary_operator, "//"),
                           "__rmod__" : (reverse_binary_operator, "%"),
                           "__rand__" : (reverse_binary_operator, "&"),
                           "__rxor__" : (reverse_binary_operator, "^"),
                           "__ror__"  : (reverse_binary_operator, "|"),
                           
                           "__iadd__" : (binary_operator, "+="),
                           "__isub__" : (binary_operator, "-="),
                           "__imul__" : (binary_operator, "*="),
-                          "__idiv__" : (binary_operator, "/="),
+                          "__itruediv__" : (binary_operator, "/="),
+                          "__ifloordiv__" : (binary_operator, "//="),
                           "__imod__" : (binary_operator, "%="),
                           "__iand__" : (binary_operator, "&="),
                           "__ixor__" : (binary_operator, "^="),
                           "__ior__"  : (binary_operator, "|="),
 
                           "__neg__"    : (unary_operator, "-"),
                           "__invert__" : (unary_operator, "~"),
@@ -476,15 +485,15 @@
     # Bind special operators.
     ss("\n    // Operators\n")
     kills = []
     for i, (mname, meth) in enumerate(allmethods):
         methattrs = PYB11attrs(meth)
         methattrs["returnType"] = eval("klassinst." + mname + "()")
         args = PYB11parseArgs(meth)
-        if methattrs["pyname"] in special_operators:
+        if methattrs["pyname"] in special_operators and not methattrs["implementation"]:
             func, op = special_operators[methattrs["pyname"]]
             func(meth, methattrs, args, op)
             kills.append(i)
     for i in reversed(kills):
         del allmethods[i]
 
     # Bind the remaining methods of the class.
```

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11enum.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11enum.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11function.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11function.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11property.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11property.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator/PYB11utils.py` & `PYB11Generator-2.1.0/PYB11Generator/PYB11utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,16 @@
          "noconvert"             : False,
          "implementation"        : None,
          "returnpolicy"          : None,
          "keepalive"             : None,
          "call_guard"            : None,
          "template"              : (),
          "template_dict"         : {},
-         "module"                : {}}
+         "module"                : {},
+         "operator"              : False}
     for key in d:
         if hasattr(obj, "PYB11" + key):
             d[key] = eval("obj.PYB11%s" % key)
     safeexts= PYB11cppname_exts(d["template"])
     d["full_cppname"] = d["cppname"] + safeexts[0]
     d["mangle_cppname"] = d["cppname"] + safeexts[1]
     return d
```

### Comparing `PYB11Generator-2.0.3/PYB11Generator/__init__.py` & `PYB11Generator-2.1.0/PYB11Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/PYB11Generator.egg-info/PKG-INFO` & `PYB11Generator-2.1.0/PYB11Generator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: PYB11Generator
-Version: 2.0.3
-Summary: PYB11Generator is a code generation tool which generates pybind11 code for binding C++ to Python. Documentation is available at https://pyb11generator.readthedocs.io/
+Version: 2.1.0
+Summary: A code generator for the pybind11 C++ <-> Python language binding tool
 Home-page: https://github.com/jmikeowen/PYB11Generator
 Author: J. Michael Owen
-Author-email: "J. Michael Owen" <mikeowen@llnl.gov>
-Project-URL: Homepage, https://github.com/LLNL/PYB11Generator
-Project-URL: Bug Tracker, https://github.com/LLNL/PYB11Generator/issues
+Author-email: mikeowen@llnl.gov
+License: UNKNOWN
+Description: PYB11Generator
+        ==============
+        
+        PYB11Generator is a python based code generator that creates [pybind11](https://github.com/pybind/pybind11) code for binding C++ libraries as extensions in Python. PYB11Generator parses input that is very close to writing the desired interface in native python, turning this into the corresponding pybind11 C++ code.
+        
+        Note, since PYB11Generator blindly generates C++ pybind11 code, it is essential to understand the pybind11 package itself as well!  In other words, be sure to read and understand the [pybind11 documentation](https://pybind11.readthedocs.io/en/stable/) before trying to go too far with PYB11Generator.  The purpose of PYB11Generator is to reduce the burden of writing and maintaining redundant code when working with pybind11 (such as the [trampoline classes](https://pybind11.readthedocs.io/en/stable/advanced/classes.html#overriding-virtual-functions-in-python)), and provide a natural syntax for those already familiar with writing interfaces in Python.  However, since the generated pybind11 code produced by PYB11Generator is what is actually compiled by a C++ compiler to create the corresponding python package, any errors reported by the compiler will refer to this generated code, and require understanding pybind11 itself to properly interpret.
+        
+        Documentation
+        -------------
+        
+        PYB11Generator is documented at [readthedocs](https://pyb11generator.readthedocs.io/en/latest/).
+        
+        Note the source for this documentation is embedded in the PYB11Generator repository under docs/.
+        
+        Contributions
+        -------------
+        
+        Although a great deal of the functionality of pybind11 is available via PYB11Generator, there are certainly missing pieces and improvements that can be made.  Contributions are welcome, and should be provided as pull requests to the main repository.  Note all contributions must be provided under the same license for distribution (in this case the BSD license).
+        
+        License
+        -------
+        
+        PYB11Generator is released under the [BSD license](https://github.com/jmikeowen/PYB11Generator/blob/master/LICENSE).
+        
+        LLNL-CODE-767799
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
-PYB11Generator
-==============
-
-PYB11Generator is a python based code generator that creates [pybind11](https://github.com/pybind/pybind11) code for binding C++ libraries as extensions in Python. PYB11Generator parses input that is very close to writing the desired interface in native python, turning this into the corresponding pybind11 C++ code.
-
-Note, since PYB11Generator blindly generates C++ pybind11 code, it is essential to understand the pybind11 package itself as well!  In other words, be sure to read and understand the [pybind11 documentation](https://pybind11.readthedocs.io/en/stable/) before trying to go too far with PYB11Generator.  The purpose of PYB11Generator is to reduce the burden of writing and maintaining redundant code when working with pybind11 (such as the [trampoline classes](https://pybind11.readthedocs.io/en/stable/advanced/classes.html#overriding-virtual-functions-in-python)), and provide a natural syntax for those already familiar with writing interfaces in Python.  However, since the generated pybind11 code produced by PYB11Generator is what is actually compiled by a C++ compiler to create the corresponding python package, any errors reported by the compiler will refer to this generated code, and require understanding pybind11 itself to properly interpret.
-
-Documentation
--------------
-
-PYB11Generator is documented at [readthedocs](https://pyb11generator.readthedocs.io/en/latest/).
-
-Note the source for this documentation is embedded in the PYB11Generator repository under docs/.
-
-Contributions
--------------
-
-Although a great deal of the functionality of pybind11 is available via PYB11Generator, there are certainly missing pieces and improvements that can be made.  Contributions are welcome, and should be provided as pull requests to the main repository.  Note all contributions must be provided under the same license for distribution (in this case the BSD license).
-
-License
--------
-
-PYB11Generator is released under the [BSD license](https://github.com/jmikeowen/PYB11Generator/blob/master/LICENSE).
-
-LLNL-CODE-767799
```

### Comparing `PYB11Generator-2.0.3/PYB11Generator.egg-info/SOURCES.txt` & `PYB11Generator-2.1.0/PYB11Generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/README.md` & `PYB11Generator-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/cmake/FindSphinx.cmake` & `PYB11Generator-2.1.0/cmake/FindSphinx.cmake`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/cmake/PYB11Generator.cmake` & `PYB11Generator-2.1.0/cmake/PYB11Generator.cmake`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/cmake/add_sphinx_target.cmake` & `PYB11Generator-2.1.0/cmake/add_sphinx_target.cmake`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/cmake/generate_cpp.py` & `PYB11Generator-2.1.0/cmake/generate_cpp.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/cmake/moduleCheck.py` & `PYB11Generator-2.1.0/cmake/moduleCheck.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/CMakeLists.txt` & `PYB11Generator-2.1.0/docs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/Makefile` & `PYB11Generator-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/PYB11decorators.rst` & `PYB11Generator-2.1.0/docs/PYB11decorators.rst`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 
 .. #############################################################################
 .. decorator:: PYB11static
 
   Mark a class method as static.
 
 .. #############################################################################
+.. decorator:: PYB11operator
+
+  Mark a class method as an operator.  See `pybind11 discussion of py::is_operator in the discussion of operator overloading<https://pybind11.readthedocs.io/en/stable/advanced/classes.html?highlight=is_operator#operator-overloading>`_.
+
+.. #############################################################################
 .. decorator:: PYB11noconvert
 
   Applies ``py::noconvert`` to all the arguments of a method to prevent automatic conversion.  See `pybind11 discussion of py:: <https://pybind11.readthedocs.io/en/stable/advanced/functions.html?highlight=noconvert#non-converting-arguments>`_.
 
 .. #############################################################################
 .. decorator:: PYB11implementation("val")
```

### Comparing `PYB11Generator-2.0.3/docs/PYB11functions.rst` & `PYB11Generator-2.1.0/docs/PYB11functions.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/PYB11variables.rst` & `PYB11Generator-2.1.0/docs/PYB11variables.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/classes.rst` & `PYB11Generator-2.1.0/docs/classes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -320,21 +320,21 @@
 
 .. _class-operators:
 
 -----------------------------------
 Special class operators and methods
 -----------------------------------
 
-Python has a number of `special methods for classes <https://docs.python.org/2/reference/datamodel.html#special-method-names>`_, such as ``__len__``, ``__add__``, etc., which allow the object behavior to be controlled for operations such as +, +=, ``len()``, and so forth.  pybind11 supports `these operators <https://pybind11.readthedocs.io/en/stable/advanced/classes.html#operator-overloading>`_, so naturally PYB11Generator does as well.  In keeping with PYB11Generators interface, these are specified by providing these special method names in your Python class description.
+Python has a number of `special methods for classes <https://docs.python.org/3/reference/datamodel.html#special-method-names>`_, such as ``__len__``, ``__add__``, etc., which allow the object behavior to be controlled for operations such as +, +=, ``len()``, and so forth.  pybind11 supports `these operators <https://pybind11.readthedocs.io/en/stable/advanced/classes.html#operator-overloading>`_, so naturally PYB11Generator does as well.  In keeping with PYB11Generators interface, these are specified by providing these special method names in your Python class description.
 
 Numeric operators
 -----------------
 
-The numeric operators supported by PYB11Generator are ``__add__``, ``__sub__``, ``__mul__``, ``__div__``, ``__mod__``, ``__and__``, ``__xor__``, ``__or__``, ``__radd__``, ``__rsub__``, ``__rmul__``, ``__rdiv__``, ``__rmod__``, ``__rand__``, ``__rxor__``, ``__ror__``, 
-``__iadd__``, ``__isub__``, ``__imul__``, ``__idiv__``, ``__imod__``, ``__iand__``, ``__ixor__``, ``__ior__``, ``__neg__``, and ``__invert__``.  Python descriptions of these methods are available `here <https://docs.python.org/2/reference/datamodel.html#emulating-numeric-types>`_.
+The numeric operators supported by PYB11Generator are ``__add__``, ``__sub__``, ``__mul__``, ``__truediv__``, ``__floordiv__``, ``__mod__``, ``__and__``, ``__xor__``, ``__or__``, ``__radd__``, ``__rsub__``, ``__rmul__``, ``__rtruediv__``, ``__rfloordiv__``, ``__rmod__``, ``__rand__``, ``__rxor__``, ``__ror__``, 
+``__iadd__``, ``__isub__``, ``__imul__``, ``__itruediv__``, ``__ifloordiv__``, ``__imod__``, ``__iand__``, ``__ixor__``, ``__ior__``, ``__neg__``, and ``__invert__``.  Python descriptions of these methods are available `here <https://docs.python.org/3/reference/datamodel.html#emulating-numeric-types>`_.
 
 In the common case for binary operators where the argument is of the same type as the class we're binding, we can omit the the argument specification and return type.  However, in the case where the binary operator accepts a different C++ type, we need to specify this argument type in the usual PYB11 syntax for arguments and return types.
 
 It is also important to remember that Python does not allow us to define a method name more than once in a class, so if we have overloaded C++ math operators (say ``operator+`` can accept more than one type), we must give each binding a unique name, but then use decorators such as ``@PYB11pyname`` to force the special operator name for the method.
 
 As an example, consider the following C++ class which supports addition with itself or a ``double``, multiplication by a ``double``, and the unary negative operator:
 
@@ -378,18 +378,29 @@
       def __imul__(self, rhs="const double"):
           return "Vector3d&"
 
       def __mul__(self, rhs="const double"):
           return "Vector3d"
     
 
+.. Note::
+
+   In some instances it is necessary to explicitly specify how to handle such operator calls.  For instance in the previous example if we needed to provide a multiplication method with a right-hand side type that is not default constructable, we can explicitly provide the implementation using a C++ lambda function and specify the method is an operator using the ``@PYB11operator`` decorator.  In our Vector3d example above for instance this could become::
+
+     class Vector3d:
+
+         @PYB11implementation("[](const Vector3d& self, const my_nonconstructable_type&) { return self * my_nonconstructable_type; }")
+         @PYB11operator
+         def __mul__(self, rhs="const my_nonconstructable_type&"):
+             return "Vector3d"
+
 Comparison operators
 --------------------
 
-The `comparison operators <https://docs.python.org/2/reference/datamodel.html#object.__lt__>`_ supported are ``__lt__``, ``__le__``, ``__eq__``, ``__ne__``, ``__gt__``, and ``__ge__``.  Usage of these methods (naturally all binary operators in this case) follow the same pattern as the numeric binary operators.  As an example, suppose our ``Vector3d`` class in the previous example also defined comparisons with with either ``Vector3d`` or ``double``:
+The `comparison operators <https://docs.python.org/3/reference/datamodel.html#object.__lt__>`_ supported are ``__lt__``, ``__le__``, ``__eq__``, ``__ne__``, ``__gt__``, and ``__ge__``.  Usage of these methods (naturally all binary operators in this case) follow the same pattern as the numeric binary operators.  As an example, suppose our ``Vector3d`` class in the previous example also defined comparisons with with either ``Vector3d`` or ``double``:
 
 .. code-block:: cpp
 
   class Vector3d {
   public:
     bool operator==(const Vector3d& rhs) const;
     bool operator!=(const Vector3d& rhs) const;
@@ -448,15 +459,15 @@
 PYB11Generator automatically associates ``__call__`` with the C++ method ``operator()``, unless overridden with something like ``@PYB11implementation``.
 
 .. _class-misc-operators:
 
 Miscellaneous operators
 -----------------------
 
-Another pair other useful operators supported are ``__repr__`` and ``__str__``.  These are used to create string representations of objects for slightly different purposes, as explained in the official `Python documentation <https://docs.python.org/2/reference/datamodel.html#object.__repr__>`_ -- essentially ``__repr__`` should return a string representation of the object such that it could be reconstructed, vs. ``__str__`` which should produce a human friendly string.
+Another pair other useful operators supported are ``__repr__`` and ``__str__``.  These are used to create string representations of objects for slightly different purposes, as explained in the official `Python documentation <https://docs.python.org/3/reference/datamodel.html#object.__repr__>`_ -- essentially ``__repr__`` should return a string representation of the object such that it could be reconstructed, vs. ``__str__`` which should produce a human friendly string.
 
 Any function or method that produces such strings is fine to bind to these names (often via renaming such as ``@PYB11pyname("__str__")``), but a very common pattern is to use lambda functions with the :func:`PYB11implementation` decorator to implement these methods directly in the binding code.  As one example, we might bind useful versions of these operators for the example C++ class ``Vector3d`` above as::
 
   class Vector3d:
 
       @PYB11implementation("[](const Vector3d& self) -> std::string { return "[" + self.x + ", " + self.y + ", " + self.z + "]" }")
       def __repr__(self):
@@ -467,15 +478,15 @@
           return "std::string"
 
 Sequence methods
 ----------------
 
 Probably the first thing to point out here is this section is *not* necessary for handling STL containers: pybind11 has built-in support for :ref:`pybind11:stl_bind`, which PYB11Generator provides convenient wrappers for.  In fact, so long as implicit copying of STL containers through the Python-C++ interface is acceptable, nothing need be done with STL containers at all -- they will automatically be handled by pybind11 transparently.
 
-Binding the Python sequence methods for your own C++ types can at times be a complicated process, and there is not necessarily a single solution that fits all cases.  There are `several methods <https://docs.python.org/2/reference/datamodel.html#emulating-container-types>`_ in Python you can override to provide sequence information: ``__len__``, ``__getitem__``, ``__setitem__``, ``__getslice__``, ``__setslice__``, ``__iter__``, etc.  PYB11Generator allows all these methods to be used via pybind11, but it definitely behooves the interested user to thoroughly understand the `pybind11 <https://pybind11.readthedocs.io/en/stable/advanced/misc.html#binding-sequence-data-types-iterators-the-slicing-protocol-etc>`_ and `Python <https://docs.python.org/2/reference/datamodel.html#emulating-container-types>`_ documentation on this subject.  It will often require writing some lightweight interstitial code to translate C++ container information to Python and back, for which lambda functions and the :py:func:`PYB11implementation` decorator are handy.
+Binding the Python sequence methods for your own C++ types can at times be a complicated process, and there is not necessarily a single solution that fits all cases.  There are `several methods <https://docs.python.org/3/reference/datamodel.html#emulating-container-types>`_ in Python you can override to provide sequence information: ``__len__``, ``__getitem__``, ``__setitem__``, ``__getslice__``, ``__setslice__``, ``__iter__``, etc.  PYB11Generator allows all these methods to be used via pybind11, but it definitely behooves the interested user to thoroughly understand the `pybind11 <https://pybind11.readthedocs.io/en/stable/advanced/misc.html#binding-sequence-data-types-iterators-the-slicing-protocol-etc>`_ and `Python <https://docs.python.org/3/reference/datamodel.html#emulating-container-types>`_ documentation on this subject.  It will often require writing some lightweight interstitial code to translate C++ container information to Python and back, for which lambda functions and the :py:func:`PYB11implementation` decorator are handy.
 
 As the bare beginning of an example, here is a version of one of the pybind11 test C++ sequence classes (stripped to just the interface) drawn from the ``pybind11/tests/test_sequences_and_iterators.cpp`` test code:
 
 .. code-block:: cpp
 
   class Sequence {
     public:
```

### Comparing `PYB11Generator-2.0.3/docs/cmake.rst` & `PYB11Generator-2.1.0/docs/cmake.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/complications.rst` & `PYB11Generator-2.1.0/docs/complications.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/conf.py` & `PYB11Generator-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/enums.rst` & `PYB11Generator-2.1.0/docs/enums.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/functions.rst` & `PYB11Generator-2.1.0/docs/functions.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/index.rst` & `PYB11Generator-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/intro.rst` & `PYB11Generator-2.1.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/make.bat` & `PYB11Generator-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/memory.rst` & `PYB11Generator-2.1.0/docs/memory.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/pybind11_objects.inv` & `PYB11Generator-2.1.0/docs/pybind11_objects.inv`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/pybind11_objects.txt` & `PYB11Generator-2.1.0/docs/pybind11_objects.txt`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/docs/stl.rst` & `PYB11Generator-2.1.0/docs/stl.rst`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/pyproject.toml` & `PYB11Generator-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["pybind11", "decorator"]
 #dynamic = ["version"]
-version = "2.0.3"
+version = "2.1.0"
 
 [project.urls]
 "Homepage" = "https://github.com/LLNL/PYB11Generator"
 "Bug Tracker" = "https://github.com/LLNL/PYB11Generator/issues"
```

### Comparing `PYB11Generator-2.0.3/setup.py` & `PYB11Generator-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Must have a separator
 if base and not base.endswith("/"):
     base += "/"
 
 setuptools.setup(
     name = "PYB11Generator",
-    version = "2.0.3",
+    version = "2.1.0",
     author = "J. Michael Owen",
     author_email = "mikeowen@llnl.gov",
     description = "A code generator for the pybind11 C++ <-> Python language binding tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/jmikeowen/PYB11Generator",
     include_package_data = True,
```

### Comparing `PYB11Generator-2.0.3/tests/inheritance/change_templates_PYB11.py` & `PYB11Generator-2.1.0/tests/inheritance/change_templates_PYB11.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/tests/inheritance/inherit_base_virtual_methods_PYB11.py` & `PYB11Generator-2.1.0/tests/inheritance/inherit_base_virtual_methods_PYB11.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/tests/inheritance/nontemplate_inherit_from_template_PYB11.py` & `PYB11Generator-2.1.0/tests/inheritance/nontemplate_inherit_from_template_PYB11.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/tests/inject/inject_test_PYB11.py` & `PYB11Generator-2.1.0/tests/inject/inject_test_PYB11.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/tests/numpy/test_np_array_PYB11.py` & `PYB11Generator-2.1.0/tests/numpy/test_np_array_PYB11.py`

 * *Files identical despite different names*

### Comparing `PYB11Generator-2.0.3/tests/protected/protected.hh` & `PYB11Generator-2.1.0/tests/protected/protected.hh`

 * *Files identical despite different names*

