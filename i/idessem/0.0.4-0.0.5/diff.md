# Comparing `tmp/idessem-0.0.4.tar.gz` & `tmp/idessem-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idessem-0.0.4.tar", last modified: Mon Mar  6 19:59:05 2023, max compression
+gzip compressed data, was "idessem-0.0.5.tar", last modified: Thu Apr 27 19:25:55 2023, max compression
```

## Comparing `idessem-0.0.4.tar` & `idessem-0.0.5.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.405641 idessem-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 19:57:16.000000 idessem-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-06 19:59:05.405641 idessem-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-06 19:57:16.000000 idessem-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.397642 idessem-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.397642 idessem-0.0.4/idessem/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.397642 idessem-0.0.4/idessem/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/avl_estatfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/log_matriz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/idessem/dessem/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/idessem/dessem/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/arquivos/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/avl_fpha1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/idessem/dessem/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/blocos/dataestudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/modelos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/dessem/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/idessem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.397642 idessem-0.0.4/idessem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-06 19:59:05.000000 idessem-0.0.4/idessem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-06 19:59:05.000000 idessem-0.0.4/idessem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:59:05.000000 idessem-0.0.4/idessem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-06 19:59:05.000000 idessem-0.0.4/idessem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 19:59:05.000000 idessem-0.0.4/idessem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 19:59:05.405641 idessem-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-06 19:57:16.000000 idessem-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/tests/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/dessem/test_polinjus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.401641 idessem-0.0.4/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:59:05.405641 idessem-0.0.4/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/arquivos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-03-06 19:57:16.000000 idessem-0.0.4/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.489013 idessem-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:23:24.000000 idessem-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 19:25:55.489013 idessem-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-27 19:23:24.000000 idessem-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/idessem/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.477012 idessem-0.0.5/idessem/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/log_matriz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/arquivos/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_fpha1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/dataestudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/idessem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:25:55.489013 idessem-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 19:23:24.000000 idessem-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.485013 idessem-0.0.5/tests/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_polinjus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.485013 idessem-0.0.5/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.489013 idessem-0.0.5/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/mock_open.py
```

### Comparing `idessem-0.0.4/LICENSE.md` & `idessem-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/PKG-INFO` & `idessem-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.4
+Version: 0.0.5
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.4/README.md` & `idessem-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/avl_altqueda.py` & `idessem-0.0.5/idessem/dessem/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/avl_desvfpha.py` & `idessem-0.0.5/idessem/dessem/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/avl_fpha1.py` & `idessem-0.0.5/idessem/dessem/avl_fpha1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from idessem.dessem.modelos.avl_fpha1 import TabelaAvlFpha1
+from idessem.dessem.modelos.avl_fpha1 import (
+    TabelaAvlFpha1,
+    TabelaAvlFpha1v1903,
+)
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
 
@@ -10,14 +13,18 @@
     """
     Armazena os dados referentes aos coeficientes da função de produção das usinas hidráulicas.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo AVL_FPHA1.
     """
 
     BLOCKS = [VersaoModelo, DataEstudo, TabelaAvlFpha1]
+    VERSIONS = {
+        "19.3": [VersaoModelo, DataEstudo, TabelaAvlFpha1v1903],
+        "19.3.1": [VersaoModelo, DataEstudo, TabelaAvlFpha1],
+    }
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="AVL_FPHA1.DAT"
     ) -> "AvlFpha1":
         return cls.read(diretorio, nome_arquivo)
```

### Comparing `idessem-0.0.4/idessem/dessem/hidr.py` & `idessem-0.0.5/idessem/dessem/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/log_matriz.py` & `idessem-0.0.5/idessem/dessem/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/arquivos/arquivocsv.py` & `idessem-0.0.5/idessem/dessem/modelos/arquivos/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/avl_altqueda.py` & `idessem-0.0.5/idessem/dessem/modelos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/avl_desvfpha.py` & `idessem-0.0.5/idessem/dessem/modelos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/avl_fpha1.py` & `idessem-0.0.5/idessem/dessem/modelos/log_matriz.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 from cfinterface.components.line import Line
 from idessem.dessem.modelos.blocos.tabelacsv import TabelaCSV
 
 
-class TabelaAvlFpha1(TabelaCSV):
+class TabelaLogMatriz(TabelaCSV):
     """
-    Bloco com as informações da tabela do arquivo AVL_FPHA1.
+    Bloco com as informações da tabela do arquivo LOG_MATRIZ.
     """
 
-    BEGIN_PATTERN = "-----;--------------;"
+    BEGIN_PATTERN = "----;------------;"
     LINE_MODEL = Line(
         [
+            IntegerField(size=4),
+            LiteralField(size=12),
+            IntegerField(size=9),
+            IntegerField(size=9),
+            IntegerField(size=9),
+            IntegerField(size=9),
+            IntegerField(size=9),
+            FloatField(size=9, decimal_digits=1),
+            FloatField(size=17, decimal_digits=3),
             IntegerField(size=5),
-            LiteralField(size=14),
-            IntegerField(size=7),
-            FloatField(size=9, decimal_digits=5),
-            FloatField(size=8, decimal_digits=2),
-            FloatField(size=12, decimal_digits=4),
-            FloatField(size=13, decimal_digits=6),
-            FloatField(size=13, decimal_digits=6),
-            FloatField(size=13, decimal_digits=6),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
-        "indice_usina",
-        "nome_usina",
-        "segmento_fpha",
-        "fator_correcao",
-        "vazao_lateral_media",
-        "rhs",
-        "coeficiente_volume_util",
-        "coeficiente_vazao_turbinada",
-        "coeficiente_vazao_lateral",
+        "iteracao",
+        "tipo",
+        "variaveis",
+        "variaveis_inteiras",
+        "restricoes",
+        "restricoes_inteiras",
+        "elementos",
+        "tempo_min",
+        "funcao_objetivo",
+        "status",
     ]
     END_PATTERN = ""
```

### Comparing `idessem-0.0.4/idessem/dessem/modelos/blocos/dataestudo.py` & `idessem-0.0.5/idessem/dessem/modelos/blocos/versaomodelo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from cfinterface.components.block import Block
-from cfinterface.components.datetimefield import DatetimeField
-from datetime import datetime
 from typing import IO
 
 
-class DataEstudo(Block):
+class VersaoModelo(Block):
     """
-    Bloco para ler a data base do estudo a partir da linha de
-    título do estudo existente no arquivo.
+    Bloco para ler a versão utilizada do modelo a partir da linha de
+    título do arquivo.
     """
 
-    BEGIN_PATTERN = r"Data do Caso:"
+    BEGIN_PATTERN = r"MODELO DESSEM"
     END_PATTERN = ""
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, DataEstudo):
+        if not isinstance(o, VersaoModelo):
             return False
         else:
-            if not all(
-                [type(self.data) == datetime, type(o.data) == datetime]
-            ):
+            if not all([type(self.data) == str, type(o.data) == str]):
                 return False
             return self.data == o.data
 
-    def read(self, file: IO):
+    def read(self, file: IO, *args, **kwargs):
         linha = file.readline()
-        dados = linha.split(DataEstudo.BEGIN_PATTERN)
-        campo = DatetimeField(size=10, starting_position=0, format="%d/%m/%Y")
-        self.data = campo.read(dados[1].strip())
+        self.data = linha.split("VERSAO")[1].split("-")[0].strip()
```

### Comparing `idessem-0.0.4/idessem/dessem/modelos/blocos/tabelacsv.py` & `idessem-0.0.5/idessem/dessem/modelos/blocos/tabelacsv.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 return False
             else:
                 return self.data.equals(o.data)
 
     def _monta_df(self, dados: dict) -> pd.DataFrame:
         return pd.DataFrame(data=dados, columns=self.__class__.COLUMN_NAMES)
 
-    def read(self, file: IO):
+    def read(self, file: IO, *args, **kwargs):
         if len(self.__class__.LINE_MODEL.fields) != len(
             self.__class__.COLUMN_NAMES
         ):
             n_linha = len(self.__class__.LINE_MODEL.fields)
             n_cols = len(self.__class__.COLUMN_NAMES)
             raise RuntimeError(
                 f"Número de colunas ({n_cols}) diferente do"
@@ -49,13 +49,13 @@
                 break
             elif len(linha) < 3:
                 return
         # Lê a tabela
         dados: Dict[str, list] = {c: [] for c in self.__class__.COLUMN_NAMES}
         while True:
             linha = file.readline()
-            if len(linha) < 3:
+            if (len(linha) < 3) or self.__class__.BEGIN_PATTERN in linha:
                 self.data = self._monta_df(dados)
                 return
             dados_linha = self.__class__.LINE_MODEL.read(linha)
             for i, c in enumerate(self.__class__.COLUMN_NAMES):
                 dados[c].append(dados_linha[i])
```

### Comparing `idessem-0.0.4/idessem/dessem/modelos/hidr.py` & `idessem-0.0.5/idessem/dessem/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/log_matriz.py` & `idessem-0.0.5/idessem/dessem/modelos/avl_fpha1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,72 @@
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 from cfinterface.components.line import Line
 from idessem.dessem.modelos.blocos.tabelacsv import TabelaCSV
 
 
-class TabelaLogMatriz(TabelaCSV):
+class TabelaAvlFpha1(TabelaCSV):
     """
-    Bloco com as informações da tabela do arquivo LOG_MATRIZ.
+    Bloco com as informações da tabela do arquivo AVL_FPHA1.
     """
 
-    BEGIN_PATTERN = "----;------------;"
+    BEGIN_PATTERN = "-----;--------------;"
     LINE_MODEL = Line(
         [
-            IntegerField(size=4),
-            LiteralField(size=12),
-            IntegerField(size=9),
-            IntegerField(size=9),
-            IntegerField(size=9),
-            IntegerField(size=9),
-            IntegerField(size=9),
-            FloatField(size=9, decimal_digits=1),
-            FloatField(size=17, decimal_digits=3),
             IntegerField(size=5),
+            LiteralField(size=14),
+            IntegerField(size=7),
+            FloatField(size=9, decimal_digits=5),
+            FloatField(size=8, decimal_digits=2),
+            FloatField(size=12, decimal_digits=4),
+            FloatField(size=13, decimal_digits=6),
+            FloatField(size=13, decimal_digits=6),
+            FloatField(size=13, decimal_digits=6),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
-        "iteracao",
-        "tipo",
-        "variaveis",
-        "variaveis_inteiras",
-        "restricoes",
-        "restricoes_inteiras",
-        "elementos",
-        "tempo_min",
-        "funcao_objetivo",
-        "status",
+        "indice_usina",
+        "nome_usina",
+        "segmento_fpha",
+        "fator_correcao",
+        "vazao_lateral_media",
+        "rhs",
+        "coeficiente_volume_util",
+        "coeficiente_vazao_turbinada",
+        "coeficiente_vazao_lateral",
     ]
-    END_PATTERN = ""
+    END_PATTERN = "-----;--------------;"
+
+
+class TabelaAvlFpha1v1903(TabelaCSV):
+    """
+    Bloco com as informações da tabela do arquivo AVL_FPHA1.
+    Válido a partir da versão 19.3.
+    """
+
+    BEGIN_PATTERN = "-----;--------------;"
+    LINE_MODEL = Line(
+        [
+            IntegerField(size=5),
+            LiteralField(size=14),
+            IntegerField(size=7),
+            FloatField(size=9, decimal_digits=5),
+            FloatField(size=12, decimal_digits=4),
+            FloatField(size=13, decimal_digits=6),
+            FloatField(size=13, decimal_digits=6),
+            FloatField(size=13, decimal_digits=6),
+        ],
+        delimiter=";",
+    )
+    COLUMN_NAMES = [
+        "indice_usina",
+        "nome_usina",
+        "segmento_fpha",
+        "fator_correcao",
+        "rhs",
+        "coeficiente_volume_util",
+        "coeficiente_vazao_turbinada",
+        "coeficiente_vazao_lateral",
+    ]
+    END_PATTERN = "-----;--------------;"
```

### Comparing `idessem-0.0.4/idessem/dessem/modelos/pdo_eco_usih.py` & `idessem-0.0.5/idessem/dessem/modelos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/pdo_hidr.py` & `idessem-0.0.5/idessem/dessem/modelos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/pdo_oper_uct.py` & `idessem-0.0.5/idessem/dessem/modelos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/pdo_sist.py` & `idessem-0.0.5/idessem/dessem/modelos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/modelos/polinjus.py` & `idessem-0.0.5/idessem/dessem/modelos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/pdo_eco_usih.py` & `idessem-0.0.5/idessem/dessem/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/pdo_hidr.py` & `idessem-0.0.5/idessem/dessem/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/pdo_oper_uct.py` & `idessem-0.0.5/idessem/dessem/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/pdo_sist.py` & `idessem-0.0.5/idessem/dessem/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem/dessem/polinjus.py` & `idessem-0.0.5/idessem/dessem/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/idessem.egg-info/PKG-INFO` & `idessem-0.0.5/idessem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.4
+Version: 0.0.5
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.4/idessem.egg-info/SOURCES.txt` & `idessem-0.0.5/idessem.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 idessem/dessem/avl_altqueda.py
 idessem/dessem/avl_desvfpha.py
 idessem/dessem/avl_estatfpha.py
 idessem/dessem/avl_fpha1.py
 idessem/dessem/des_log_relato.py
 idessem/dessem/hidr.py
 idessem/dessem/log_matriz.py
+idessem/dessem/operut.py
 idessem/dessem/pdo_eco_usih.py
 idessem/dessem/pdo_hidr.py
 idessem/dessem/pdo_oper_uct.py
 idessem/dessem/pdo_sist.py
 idessem/dessem/polinjus.py
 idessem/dessem/modelos/__init__.py
 idessem/dessem/modelos/avl_altqueda.py
 idessem/dessem/modelos/avl_desvfpha.py
 idessem/dessem/modelos/avl_fpha1.py
+idessem/dessem/modelos/des_log_relato.py
 idessem/dessem/modelos/hidr.py
 idessem/dessem/modelos/log_matriz.py
+idessem/dessem/modelos/operut.py
 idessem/dessem/modelos/pdo_eco_usih.py
 idessem/dessem/modelos/pdo_hidr.py
 idessem/dessem/modelos/pdo_oper_uct.py
 idessem/dessem/modelos/pdo_sist.py
 idessem/dessem/modelos/polinjus.py
 idessem/dessem/modelos/arquivos/__init__.py
 idessem/dessem/modelos/arquivos/arquivocsv.py
@@ -41,27 +44,30 @@
 idessem/dessem/modelos/blocos/tabelacsv.py
 idessem/dessem/modelos/blocos/versaomodelo.py
 tests/__init__.py
 tests/dessem/__init__.py
 tests/dessem/test_avl_altqueda.py
 tests/dessem/test_avl_desvfpha.py
 tests/dessem/test_avl_fpha1.py
+tests/dessem/test_des_log_relato.py
 tests/dessem/test_hidr.py
 tests/dessem/test_log_matriz.py
+tests/dessem/test_operut.py
 tests/dessem/test_pdo_eco_usih.py
 tests/dessem/test_pdo_hidr.py
 tests/dessem/test_pdo_oper_uct.py
 tests/dessem/test_pdo_sist.py
 tests/dessem/test_polinjus.py
 tests/mocks/__init__.py
 tests/mocks/mock_open.py
 tests/mocks/arquivos/__init__.py
 tests/mocks/arquivos/avl_altqueda.py
 tests/mocks/arquivos/avl_desvfpha.py
 tests/mocks/arquivos/avl_fpha1.py
 tests/mocks/arquivos/des_log_relato.py
 tests/mocks/arquivos/log_matriz.py
+tests/mocks/arquivos/operut.py
 tests/mocks/arquivos/pdo_eco_usih.py
 tests/mocks/arquivos/pdo_hidr.py
 tests/mocks/arquivos/pdo_oper_uct.py
 tests/mocks/arquivos/pdo_sist.py
 tests/mocks/arquivos/polinjus.py
```

### Comparing `idessem-0.0.4/setup.py` & `idessem-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_avl_altqueda.py` & `idessem-0.0.5/tests/dessem/test_avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_avl_desvfpha.py` & `idessem-0.0.5/tests/dessem/test_avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_avl_fpha1.py` & `idessem-0.0.5/tests/dessem/test_pdo_sist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,73 @@
-from idessem.dessem.avl_fpha1 import AvlFpha1
-
+from idessem.dessem.pdo_sist import PdoSist
+import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.avl_fpha1 import MockAvlFpha1
+from tests.mocks.arquivos.pdo_sist import MockPdoSist
 
 
-def test_atributos_encontrados_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_atributos_encontrados_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = PdoSist.le_arquivo("")
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
-def test_versao_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_versao_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = PdoSist.le_arquivo("")
         assert log.versao == "19.3"
 
 
-def test_data_estudo_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_data_estudo_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = PdoSist.le_arquivo("")
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
-def test_tabela_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_tabela_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
-        assert log.tabela.at[0, "indice_usina"] == 1
-        assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
-        assert log.tabela.at[0, "segmento_fpha"] == 1
-        assert log.tabela.at[0, "fator_correcao"] == 1.0
-        assert log.tabela.at[0, "vazao_lateral_media"] == 0
-        assert log.tabela.at[0, "rhs"] == -11.8461
-        assert log.tabela.at[0, "coeficiente_volume_util"] == 0.020604
-        assert log.tabela.at[0, "coeficiente_vazao_turbinada"] == 0.224440
-        assert log.tabela.at[0, "coeficiente_vazao_lateral"] == 0.0
+        log = PdoSist.le_arquivo("")
+        assert log.tabela.at[0, "estagio"] == 1
+        assert log.tabela.at[0, "patamar"] == "LEVE"
+        assert log.tabela.at[0, "submercado"] == "SE"
+        assert log.tabela.at[0, "cmo"] == 71.48
+        assert log.tabela.at[0, "demanda"] == 36935.91
+        assert log.tabela.at[0, "perdas"] == "-"
+        assert log.tabela.at[0, "geracao_pequenas_usinas"] == 0.0
+        assert log.tabela.at[0, "geracao_fixa_barra"] == 0.0
+        assert log.tabela.at[0, "geracao_renovavel"] == 5006.00
+        assert log.tabela.at[0, "geracao_hidraulica"] == 27152.97
+        assert log.tabela.at[0, "geracao_termica"] == 2555.95
+        assert log.tabela.at[0, "consumo_elevatorias"] == 108.62
+        assert log.tabela.at[0, "importacao"] == 6479.64
+        assert log.tabela.at[0, "exportacao"] == 6079.64
+        assert log.tabela.at[0, "corte_carga"] == 0.0
+        assert log.tabela.at[0, "saldo"] == -3461.61
+        assert log.tabela.at[0, "recebimento"] == 3461.61
+        assert log.tabela.at[0, "geracao_termica_minima"] == 2555.95
+        assert log.tabela.at[0, "geracao_termica_maxima"] == 9489.79
+        assert log.tabela.at[0, "energia_armazenada"] == 122020.78
 
 
-def test_eq_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_eq_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = PdoSist.le_arquivo("")
+        log2 = PdoSist.le_arquivo("")
         assert log1 == log2
 
 
-def test_neq_avl_fpha1():
-    m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
+def test_neq_pdo_sist():
+    m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = PdoSist.le_arquivo("")
+        log2 = PdoSist.le_arquivo("")
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.4/tests/dessem/test_hidr.py` & `idessem-0.0.5/tests/dessem/test_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_log_matriz.py` & `idessem-0.0.5/tests/dessem/test_log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_pdo_eco_usih.py` & `idessem-0.0.5/tests/dessem/test_pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_pdo_hidr.py` & `idessem-0.0.5/tests/dessem/test_pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_pdo_oper_uct.py` & `idessem-0.0.5/tests/dessem/test_pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/dessem/test_polinjus.py` & `idessem-0.0.5/tests/dessem/test_polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/avl_altqueda.py` & `idessem-0.0.5/tests/mocks/arquivos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/avl_desvfpha.py` & `idessem-0.0.5/tests/mocks/arquivos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/log_matriz.py` & `idessem-0.0.5/tests/mocks/arquivos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/pdo_eco_usih.py` & `idessem-0.0.5/tests/mocks/arquivos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/pdo_hidr.py` & `idessem-0.0.5/tests/mocks/arquivos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/pdo_oper_uct.py` & `idessem-0.0.5/tests/mocks/arquivos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/pdo_sist.py` & `idessem-0.0.5/tests/mocks/arquivos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/arquivos/polinjus.py` & `idessem-0.0.5/tests/mocks/arquivos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.4/tests/mocks/mock_open.py` & `idessem-0.0.5/tests/mocks/mock_open.py`

 * *Files identical despite different names*

