# Comparing `tmp/datajunction_server-0.0.1a6.tar.gz` & `tmp/datajunction_server-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajunction_server-0.0.1a6.tar", max compression
+gzip compressed data, was "datajunction_server-0.0.1a7.tar", max compression
```

## Comparing `datajunction_server-0.0.1a6.tar` & `datajunction_server-0.0.1a7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1081 2023-03-23 14:56:44.793141 datajunction_server-0.0.1a6/LICENSE.txt
--rw-r--r--   0        0        0     5589 2023-03-23 14:56:44.793284 datajunction_server-0.0.1a6/README.rst
--rw-r--r--   0        0        0      384 2023-03-23 14:56:44.827629 datajunction_server-0.0.1a6/dj/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 14:56:44.827705 datajunction_server-0.0.1a6/dj/api/__init__.py
--rw-r--r--   0        0        0     4692 2023-04-17 00:58:29.509603 datajunction_server-0.0.1a6/dj/api/attributes.py
--rw-r--r--   0        0        0     2862 2023-04-17 00:58:29.509692 datajunction_server-0.0.1a6/dj/api/catalogs.py
--rw-r--r--   0        0        0      654 2023-04-17 00:58:29.509778 datajunction_server-0.0.1a6/dj/api/cubes.py
--rw-r--r--   0        0        0     5036 2023-04-17 00:58:29.509894 datajunction_server-0.0.1a6/dj/api/data.py
--rw-r--r--   0        0        0     1457 2023-04-17 00:58:29.510040 datajunction_server-0.0.1a6/dj/api/engines.py
--rw-r--r--   0        0        0     1220 2023-04-17 00:58:29.510151 datajunction_server-0.0.1a6/dj/api/health.py
--rw-r--r--   0        0        0    12980 2023-04-17 00:58:29.510271 datajunction_server-0.0.1a6/dj/api/helpers.py
--rw-r--r--   0        0        0     3061 2023-04-21 02:27:43.651947 datajunction_server-0.0.1a6/dj/api/main.py
--rw-r--r--   0        0        0     2669 2023-04-21 02:27:43.652059 datajunction_server-0.0.1a6/dj/api/metrics.py
--rw-r--r--   0        0        0     2205 2023-04-21 02:27:43.652215 datajunction_server-0.0.1a6/dj/api/namespaces.py
--rw-r--r--   0        0        0    32109 2023-04-21 02:27:43.652411 datajunction_server-0.0.1a6/dj/api/nodes.py
--rw-r--r--   0        0        0      702 2023-04-17 00:58:29.510734 datajunction_server-0.0.1a6/dj/api/query.py
--rw-r--r--   0        0        0     1345 2023-04-17 00:58:29.510823 datajunction_server-0.0.1a6/dj/api/sql.py
--rw-r--r--   0        0        0     3358 2023-04-17 00:58:29.510918 datajunction_server-0.0.1a6/dj/api/tags.py
--rw-r--r--   0        0        0     2239 2023-04-17 00:58:29.511025 datajunction_server-0.0.1a6/dj/config.py
--rw-r--r--   0        0        0      412 2023-03-23 14:56:44.829093 datajunction_server-0.0.1a6/dj/constants.py
--rwxr-xr-x   0        0        0        0 2023-03-23 14:56:44.829159 datajunction_server-0.0.1a6/dj/construction/__init__.py
--rwxr-xr-x   0        0        0    19622 2023-04-21 02:27:43.652607 datajunction_server-0.0.1a6/dj/construction/build.py
--rw-r--r--   0        0        0     6561 2023-04-17 00:58:29.511317 datajunction_server-0.0.1a6/dj/construction/dj_query.py
--rwxr-xr-x   0        0        0     1495 2023-03-23 14:56:44.829531 datajunction_server-0.0.1a6/dj/construction/exceptions.py
--rwxr-xr-x   0        0        0     2679 2023-04-17 00:58:29.511419 datajunction_server-0.0.1a6/dj/construction/utils.py
--rw-r--r--   0        0        0     5900 2023-04-17 00:58:29.511730 datajunction_server-0.0.1a6/dj/errors.py
--rw-r--r--   0        0        0      518 2023-03-23 14:56:44.829960 datajunction_server-0.0.1a6/dj/models/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-23 14:56:44.830025 datajunction_server-0.0.1a6/dj/models/attribute.py
--rw-r--r--   0        0        0     1995 2023-04-21 02:27:43.652764 datajunction_server-0.0.1a6/dj/models/base.py
--rw-r--r--   0        0        0     2155 2023-03-23 14:56:44.830167 datajunction_server-0.0.1a6/dj/models/catalog.py
--rw-r--r--   0        0        0     2937 2023-04-21 02:27:43.652874 datajunction_server-0.0.1a6/dj/models/column.py
--rw-r--r--   0        0        0     1267 2023-04-21 02:27:43.652984 datajunction_server-0.0.1a6/dj/models/cube.py
--rw-r--r--   0        0        0     2019 2023-03-23 14:56:44.830428 datajunction_server-0.0.1a6/dj/models/database.py
--rw-r--r--   0        0        0      811 2023-04-21 02:27:43.653086 datajunction_server-0.0.1a6/dj/models/engine.py
--rw-r--r--   0        0        0     1258 2023-04-17 00:58:29.512021 datajunction_server-0.0.1a6/dj/models/metric.py
--rw-r--r--   0        0        0    20674 2023-04-21 02:27:43.653529 datajunction_server-0.0.1a6/dj/models/node.py
--rw-r--r--   0        0        0     3711 2023-03-23 14:56:44.830746 datajunction_server-0.0.1a6/dj/models/query.py
--rw-r--r--   0        0        0     2449 2023-03-23 14:56:44.830812 datajunction_server-0.0.1a6/dj/models/table.py
--rw-r--r--   0        0        0     2567 2023-03-23 14:56:44.830869 datajunction_server-0.0.1a6/dj/models/tag.py
--rw-r--r--   0        0        0     4043 2023-04-17 00:58:29.512282 datajunction_server-0.0.1a6/dj/service_clients.py
--rw-r--r--   0        0        0        0 2023-03-23 14:56:44.830991 datajunction_server-0.0.1a6/dj/sql/__init__.py
--rw-r--r--   0        0        0     1562 2023-04-21 02:27:43.653795 datajunction_server-0.0.1a6/dj/sql/dag.py
--rw-r--r--   0        0        0    34351 2023-04-21 02:27:43.654023 datajunction_server-0.0.1a6/dj/sql/functions.py
--rw-r--r--   0        0        0      644 2023-04-17 00:58:29.512575 datajunction_server-0.0.1a6/dj/sql/parse.py
--rw-r--r--   0        0        0       55 2023-04-17 00:58:29.512688 datajunction_server-0.0.1a6/dj/sql/parsing/__init__.py
--rw-r--r--   0        0        0    65402 2023-04-21 02:27:43.654354 datajunction_server-0.0.1a6/dj/sql/parsing/ast.py
--rw-r--r--   0        0        0        0 2023-03-23 14:56:44.832143 datajunction_server-0.0.1a6/dj/sql/parsing/backends/__init__.py
--rw-r--r--   0        0        0    30630 2023-04-17 00:58:29.513177 datajunction_server-0.0.1a6/dj/sql/parsing/backends/antlr4.py
--rw-r--r--   0        0        0      192 2023-03-23 14:56:44.832220 datajunction_server-0.0.1a6/dj/sql/parsing/backends/exceptions.py
--rw-r--r--   0        0        0     8733 2023-04-17 00:58:29.513435 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
--rw-r--r--   0        0        0    49854 2023-04-17 00:58:29.513622 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
--rw-r--r--   0        0        0        0 2023-04-17 00:58:29.513656 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/__init__.py
--rw-r--r--   0        0        0   117820 2023-04-17 00:58:29.513994 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
--rw-r--r--   0        0        0   114725 2023-04-17 00:58:29.514368 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
--rw-r--r--   0        0        0     8131 2023-04-17 00:58:29.514464 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
--rw-r--r--   0        0        0   142799 2023-04-17 00:58:29.514996 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
--rw-r--r--   0        0        0  1020523 2023-04-17 00:58:29.516779 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
--rw-r--r--   0        0        0     8131 2023-04-17 00:58:29.516945 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
--rw-r--r--   0        0        0   102489 2023-04-17 00:58:29.517280 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
--rw-r--r--   0        0        0    60656 2023-04-17 00:58:29.517368 datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
--rw-r--r--   0        0        0    26308 2023-04-21 02:27:43.654560 datajunction_server-0.0.1a6/dj/sql/parsing/types.py
--rw-r--r--   0        0        0     3812 2023-03-23 14:56:44.832808 datajunction_server-0.0.1a6/dj/superset.py
--rw-r--r--   0        0        0     6467 2023-04-17 00:58:29.517688 datajunction_server-0.0.1a6/dj/typing.py
--rw-r--r--   0        0        0     4042 2023-04-17 00:58:29.517822 datajunction_server-0.0.1a6/dj/utils.py
--rw-r--r--   0        0        0     1426 2023-04-21 02:27:43.657271 datajunction_server-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     7327 1970-01-01 00:00:00.000000 datajunction_server-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-09 19:29:41.743091 datajunction_server-0.0.1a7/LICENSE.txt
+-rw-r--r--   0        0        0     5589 2023-03-09 19:29:41.743202 datajunction_server-0.0.1a7/README.rst
+-rw-r--r--   0        0        0      384 2023-03-09 22:42:36.169164 datajunction_server-0.0.1a7/dj/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.770645 datajunction_server-0.0.1a7/dj/api/__init__.py
+-rw-r--r--   0        0        0     4692 2023-04-13 18:17:17.325178 datajunction_server-0.0.1a7/dj/api/attributes.py
+-rw-r--r--   0        0        0     2862 2023-04-13 18:17:17.325699 datajunction_server-0.0.1a7/dj/api/catalogs.py
+-rw-r--r--   0        0        0      654 2023-04-21 19:43:15.324305 datajunction_server-0.0.1a7/dj/api/cubes.py
+-rw-r--r--   0        0        0     5036 2023-04-16 15:31:28.665337 datajunction_server-0.0.1a7/dj/api/data.py
+-rw-r--r--   0        0        0     1457 2023-04-26 16:23:29.284773 datajunction_server-0.0.1a7/dj/api/engines.py
+-rw-r--r--   0        0        0     1220 2023-04-13 18:17:17.327030 datajunction_server-0.0.1a7/dj/api/health.py
+-rw-r--r--   0        0        0    14301 2023-04-25 14:27:09.406335 datajunction_server-0.0.1a7/dj/api/helpers.py
+-rw-r--r--   0        0        0     3061 2023-04-17 19:39:28.361836 datajunction_server-0.0.1a7/dj/api/main.py
+-rw-r--r--   0        0        0     2669 2023-04-20 23:36:54.180410 datajunction_server-0.0.1a7/dj/api/metrics.py
+-rw-r--r--   0        0        0     2427 2023-04-25 14:27:09.406837 datajunction_server-0.0.1a7/dj/api/namespaces.py
+-rw-r--r--   0        0        0    37455 2023-04-26 16:47:15.937513 datajunction_server-0.0.1a7/dj/api/nodes.py
+-rw-r--r--   0        0        0      702 2023-04-13 18:17:17.328235 datajunction_server-0.0.1a7/dj/api/query.py
+-rw-r--r--   0        0        0     1345 2023-04-16 15:31:28.666447 datajunction_server-0.0.1a7/dj/api/sql.py
+-rw-r--r--   0        0        0     3358 2023-04-13 18:17:17.328723 datajunction_server-0.0.1a7/dj/api/tags.py
+-rw-r--r--   0        0        0     2239 2023-04-13 18:17:17.329272 datajunction_server-0.0.1a7/dj/config.py
+-rw-r--r--   0        0        0      412 2023-03-09 19:29:41.772659 datajunction_server-0.0.1a7/dj/constants.py
+-rwxr-xr-x   0        0        0        0 2023-03-09 19:29:41.772720 datajunction_server-0.0.1a7/dj/construction/__init__.py
+-rwxr-xr-x   0        0        0    20702 2023-04-26 16:47:15.938174 datajunction_server-0.0.1a7/dj/construction/build.py
+-rw-r--r--   0        0        0     6561 2023-04-06 15:30:00.095444 datajunction_server-0.0.1a7/dj/construction/dj_query.py
+-rwxr-xr-x   0        0        0     1495 2023-03-09 19:29:41.773112 datajunction_server-0.0.1a7/dj/construction/exceptions.py
+-rwxr-xr-x   0        0        0     2679 2023-04-06 15:30:00.095544 datajunction_server-0.0.1a7/dj/construction/utils.py
+-rw-r--r--   0        0        0     5925 2023-04-25 14:27:09.408657 datajunction_server-0.0.1a7/dj/errors.py
+-rw-r--r--   0        0        0      518 2023-03-24 07:12:07.926290 datajunction_server-0.0.1a7/dj/models/__init__.py
+-rw-r--r--   0        0        0     2146 2023-03-09 19:29:41.773677 datajunction_server-0.0.1a7/dj/models/attribute.py
+-rw-r--r--   0        0        0     1995 2023-04-20 23:36:54.181366 datajunction_server-0.0.1a7/dj/models/base.py
+-rw-r--r--   0        0        0     2155 2023-03-24 07:12:07.926414 datajunction_server-0.0.1a7/dj/models/catalog.py
+-rw-r--r--   0        0        0     3229 2023-04-26 16:47:15.938520 datajunction_server-0.0.1a7/dj/models/column.py
+-rw-r--r--   0        0        0     1675 2023-04-26 16:47:15.938790 datajunction_server-0.0.1a7/dj/models/cube.py
+-rw-r--r--   0        0        0     2019 2023-03-24 07:12:07.927108 datajunction_server-0.0.1a7/dj/models/database.py
+-rw-r--r--   0        0        0      811 2023-04-20 23:36:54.182340 datajunction_server-0.0.1a7/dj/models/engine.py
+-rw-r--r--   0        0        0     1258 2023-04-16 15:31:28.667317 datajunction_server-0.0.1a7/dj/models/metric.py
+-rw-r--r--   0        0        0    20883 2023-04-26 16:47:15.939165 datajunction_server-0.0.1a7/dj/models/node.py
+-rw-r--r--   0        0        0     3711 2023-04-13 18:09:39.316286 datajunction_server-0.0.1a7/dj/models/query.py
+-rw-r--r--   0        0        0     2449 2023-03-24 07:12:07.927968 datajunction_server-0.0.1a7/dj/models/table.py
+-rw-r--r--   0        0        0     2567 2023-03-09 19:29:41.774456 datajunction_server-0.0.1a7/dj/models/tag.py
+-rw-r--r--   0        0        0     4043 2023-04-14 00:40:01.549543 datajunction_server-0.0.1a7/dj/service_clients.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.774583 datajunction_server-0.0.1a7/dj/sql/__init__.py
+-rw-r--r--   0        0        0     1562 2023-04-20 23:36:54.182952 datajunction_server-0.0.1a7/dj/sql/dag.py
+-rw-r--r--   0        0        0    34523 2023-04-25 14:27:09.410865 datajunction_server-0.0.1a7/dj/sql/functions.py
+-rw-r--r--   0        0        0      644 2023-04-06 15:30:00.097501 datajunction_server-0.0.1a7/dj/sql/parse.py
+-rw-r--r--   0        0        0       55 2023-04-06 15:30:00.097814 datajunction_server-0.0.1a7/dj/sql/parsing/__init__.py
+-rw-r--r--   0        0        0    65484 2023-04-25 14:27:09.411772 datajunction_server-0.0.1a7/dj/sql/parsing/ast.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.775867 datajunction_server-0.0.1a7/dj/sql/parsing/backends/__init__.py
+-rw-r--r--   0        0        0    30630 2023-04-16 15:31:28.668409 datajunction_server-0.0.1a7/dj/sql/parsing/backends/antlr4.py
+-rw-r--r--   0        0        0      192 2023-03-09 19:29:41.775929 datajunction_server-0.0.1a7/dj/sql/parsing/backends/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-03-26 08:42:46.249360 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
+-rw-r--r--   0        0        0    49854 2023-03-26 08:42:46.249545 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
+-rw-r--r--   0        0        0        0 2023-03-26 08:42:46.249595 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/__init__.py
+-rw-r--r--   0        0        0   117820 2023-03-26 08:42:46.250054 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
+-rw-r--r--   0        0        0   114725 2023-03-26 08:42:46.250494 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
+-rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.250603 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
+-rw-r--r--   0        0        0   142799 2023-03-26 08:42:46.251524 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
+-rw-r--r--   0        0        0  1020523 2023-03-26 08:42:46.255771 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
+-rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.255887 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
+-rw-r--r--   0        0        0   102489 2023-03-26 08:42:46.256283 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
+-rw-r--r--   0        0        0    60656 2023-03-26 08:42:46.256504 datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
+-rw-r--r--   0        0        0    26296 2023-04-25 14:27:09.412355 datajunction_server-0.0.1a7/dj/sql/parsing/types.py
+-rw-r--r--   0        0        0     3812 2023-03-09 19:29:41.776529 datajunction_server-0.0.1a7/dj/superset.py
+-rw-r--r--   0        0        0     6467 2023-04-06 15:30:00.099751 datajunction_server-0.0.1a7/dj/typing.py
+-rw-r--r--   0        0        0     4042 2023-04-14 18:39:42.363510 datajunction_server-0.0.1a7/dj/utils.py
+-rw-r--r--   0        0        0     1426 2023-04-26 16:48:10.489712 datajunction_server-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0     7327 1970-01-01 00:00:00.000000 datajunction_server-0.0.1a7/PKG-INFO
```

### Comparing `datajunction_server-0.0.1a6/LICENSE.txt` & `datajunction_server-0.0.1a7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/README.rst` & `datajunction_server-0.0.1a7/README.rst`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/attributes.py` & `datajunction_server-0.0.1a7/dj/api/attributes.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/catalogs.py` & `datajunction_server-0.0.1a7/dj/api/catalogs.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/cubes.py` & `datajunction_server-0.0.1a7/dj/api/cubes.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/data.py` & `datajunction_server-0.0.1a7/dj/api/data.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/engines.py` & `datajunction_server-0.0.1a7/dj/api/engines.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/health.py` & `datajunction_server-0.0.1a7/dj/api/health.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/helpers.py` & `datajunction_server-0.0.1a7/dj/api/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,48 @@
             column_type = col.type  # type: ignore
             validated_node.columns.append(
                 Column(name=col.alias_or_name.name, type=column_type),  # type: ignore
             )
         except DJParseException:
             type_inference_failed_columns.append(col.alias_or_name.name)  # type: ignore
             validated_node.status = NodeStatus.INVALID
+
+    # Only raise on missing parents or type inference if the node mode is set to published
+    if missing_parents_map or type_inference_failed_columns:
+        if validated_node.mode == NodeMode.DRAFT:
+            validated_node.status = NodeStatus.INVALID
+        else:
+            missing_parents_error = (
+                [
+                    DJError(
+                        code=ErrorCode.MISSING_PARENT,
+                        message="Node definition contains references to nodes that do not exist",
+                        debug={"missing_parents": list(missing_parents_map.keys())},
+                    ),
+                ]
+                if missing_parents_map
+                else []
+            )
+            type_inference_error = (
+                [
+                    DJError(
+                        code=ErrorCode.TYPE_INFERENCE,
+                        message=(
+                            f"Unable to infer type for some columns on node `{data.name}`"
+                        ),
+                        debug={"columns": type_inference_failed_columns},
+                    ),
+                ]
+                if type_inference_failed_columns
+                else []
+            )
+            raise DJException(
+                errors=missing_parents_error + type_inference_error,
+            )
+
     return (
         validated_node,
         dependencies_map,
         missing_parents_map,
         type_inference_failed_columns,
     )
```

### Comparing `datajunction_server-0.0.1a6/dj/api/main.py` & `datajunction_server-0.0.1a7/dj/api/main.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/metrics.py` & `datajunction_server-0.0.1a7/dj/api/metrics.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/namespaces.py` & `datajunction_server-0.0.1a7/dj/api/namespaces.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Node namespace related APIs.
 """
 import logging
-from typing import List
+from typing import List, Optional
 
 from fastapi import APIRouter, Depends
 from fastapi.responses import JSONResponse
-from sqlalchemy.orm import joinedload
+from sqlalchemy import and_
 from sqlmodel import Session, select
 
 from dj.api.helpers import get_node_namespace
-from dj.models.node import Node, NodeNamespace, NodeOutput
+from dj.models.node import Node, NodeNameList, NodeNamespace, NodeType
 from dj.utils import get_session
 
 _logger = logging.getLogger(__name__)
 router = APIRouter()
 
 
 @router.post("/namespaces/{namespace}/", status_code=201)
@@ -60,31 +60,34 @@
     """
     namespaces = session.exec(select(NodeNamespace)).all()
     return namespaces
 
 
 @router.get(
     "/namespaces/{namespace}/",
-    response_model=List[NodeOutput],
+    response_model=NodeNameList,
     status_code=200,
 )
 def list_nodes_in_namespace(
     namespace: str,
+    type_: Optional[NodeType] = None,
     session: Session = Depends(get_session),
-) -> List[NodeOutput]:
+) -> NodeNameList:
     """
-    List nodes in namespace
+    List node names in namespace, filterable to a given type if desired.
     """
-    nodes = (
-        session.exec(
-            select(Node)
-            .options(joinedload(Node.current))
-            .where(
-                Node.namespace.like(  # type: ignore  # pylint: disable=no-member
-                    f"{namespace}%",
-                ),
+    where_clause = (
+        and_(
+            Node.namespace.like(  # type: ignore  # pylint: disable=no-member
+                f"{namespace}%",
             ),
+            Node.type == type_,
+        )
+        if type_
+        else Node.namespace.like(  # type: ignore  # pylint: disable=no-member
+            f"{namespace}%",
         )
-        .unique()
-        .all()
     )
-    return nodes  # type: ignore
+
+    list_nodes_query = select(Node.name).where(where_clause)
+    node_names = session.exec(list_nodes_query).all()
+    return node_names  # type: ignore
```

### Comparing `datajunction_server-0.0.1a6/dj/api/nodes.py` & `datajunction_server-0.0.1a7/dj/api/nodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+# pylint: disable=too-many-lines
 """
 Node related APIs.
 """
 import http.client
 import logging
 import os
 from collections import defaultdict
 from http import HTTPStatus
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Set, Union
 
 from fastapi import APIRouter, Depends
 from fastapi.responses import JSONResponse
 from sqlalchemy.orm import joinedload
 from sqlmodel import Session, select
 from starlette.requests import Request
 from starlette.responses import Response
@@ -31,14 +32,15 @@
 from dj.api.tags import get_tag_by_name
 from dj.construction.build import build_metric_nodes
 from dj.errors import DJDoesNotExistException, DJException, DJInvalidInputException
 from dj.models import ColumnAttribute
 from dj.models.attribute import AttributeType, UniquenessScope
 from dj.models.base import generate_display_name
 from dj.models.column import Column, ColumnAttributeInput
+from dj.models.cube import Measure
 from dj.models.node import (
     DEFAULT_DRAFT_VERSION,
     DEFAULT_PUBLISHED_VERSION,
     ColumnOutput,
     CreateCubeNode,
     CreateNode,
     CreateSourceNode,
@@ -53,14 +55,15 @@
     NodeStatus,
     NodeType,
     NodeValidation,
     UpdateNode,
     UpsertMaterializationConfig,
 )
 from dj.service_clients import QueryServiceClient
+from dj.sql.parsing import ast
 from dj.sql.parsing.backends.antlr4 import parse
 from dj.sql.parsing.backends.exceptions import DJParseException
 from dj.utils import (
     Version,
     VersionUpgrade,
     get_namespace_from_name,
     get_query_service_client,
@@ -268,14 +271,72 @@
             col.dimension_column = None
             session.add(col)
     session.delete(node)
     session.commit()
     return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
 
+def cube_materialization_config(cube_node: NodeRevision, config: Dict):
+    """
+    Builds the materialization config for a cube. This includes two parts:
+    (a) building a query that decomposes each of the cube's metrics into their
+    constituent measures that have simple aggregations
+    (b) adding a metric to measures mapping that tells us which measures
+    in the query map to each selected metric
+
+    The query in the materialization config is different from the one stored
+    on the cube node itself in that this one is meant to create a temporary
+    table in preparation for ingestion into an OLAP database like Druid. The
+    metric to measures mapping then provides information on how to assemble
+    metrics from measures based on this query's output.
+
+    The query directly on the cube node is meant for direct querying of the cube
+    without materialization to an OLAP database.
+    """
+    combined_ast = parse(cube_node.query)
+    dimensions_set = {
+        dim.name for dim in cube_node.columns if dim.has_dimension_attribute()
+    }
+    metrics_to_measures = decompose_metrics(combined_ast, dimensions_set)
+    new_select_projection: Set[Union[ast.Aliasable, ast.Expression]] = set()
+    for expr in combined_ast.select.projection:
+        if expr in metrics_to_measures:
+            new_select_projection = set(new_select_projection).union(
+                metrics_to_measures[expr],
+            )
+        else:
+            new_select_projection.add(expr)
+    combined_ast.select.projection = list(new_select_projection)
+
+    config = {
+        **config,
+        **{
+            "measures": {
+                metric.alias_or_name.name: sorted(
+                    [
+                        measure_obj.dict()
+                        for measure_obj in {
+                            Measure(
+                                name=str(measure.alias_or_name),
+                                agg=str(measure.child.name),
+                                expr=str(measure.child),
+                            )
+                            for measure in measures
+                        }
+                    ],
+                    key=lambda x: x["name"],
+                )
+                for metric, measures in metrics_to_measures.items()
+            },
+        },
+        **{"query": str(combined_ast)},
+    }
+    return config
+
+
 @router.post("/nodes/{name}/materialization/", status_code=201)
 def upsert_a_materialization_config(
     name: str,
     data: UpsertMaterializationConfig,
     *,
     session: Session = Depends(get_session),
 ) -> JSONResponse:
@@ -314,14 +375,18 @@
     engine = get_engine(session, data.engine_name, data.engine_version)
 
     unchanged_existing_configs = [
         config
         for config in current_revision.materialization_configs
         if config.engine.name != data.engine_name
     ]
+
+    if current_revision.type == NodeType.CUBE:
+        data.config = cube_materialization_config(current_revision, data.config)
+
     new_config = MaterializationConfig(
         node_revision=current_revision,
         engine=engine,
         config=data.config,
         schedule=data.schedule,
     )
     current_revision.materialization_configs = unchanged_existing_configs + [  # type: ignore
@@ -412,14 +477,83 @@
         [p.name for p in node_revision.parents],
     )
     node_revision.columns = validated_node.columns or []
     node_revision.catalog_id = catalog_id
     return node_revision
 
 
+def decompose_expression(expr: Union[ast.Aliasable, ast.Expression]) -> List[ast.Alias]:
+    """
+    Simple aggregations are operations that can be computed incrementally as new
+    data is ingested, without relying on the results of other aggregations.
+    Examples include SUM, COUNT, MIN, MAX.
+
+    Some complex aggregations can be decomposed to simple aggregations: i.e., AVG(x) can
+    be decomposed to SUM(x)/COUNT(x).
+    """
+    if isinstance(expr, ast.Alias):
+        expr = expr.child
+
+    simple_aggregations = {"sum", "count", "min", "max"}
+    if isinstance(expr, ast.Function):
+        function_name = expr.alias_or_name.name.lower()
+        columns = [col for arg in expr.args for col in arg.find_all(ast.Column)]
+        readable_name = (
+            "_".join(
+                str(col.alias_or_name).rsplit(".", maxsplit=1)[-1] for col in columns
+            )
+            if columns
+            else "placeholder"
+        )
+        if function_name in simple_aggregations:
+            return [expr.set_alias(ast.Name(f"{readable_name}_{function_name}"))]
+        if function_name == "avg":  # pragma: no cover
+            return [
+                (
+                    ast.Function(ast.Name("sum"), args=expr.args).set_alias(
+                        ast.Name(f"{readable_name}_sum"),
+                    )
+                ),
+                (
+                    ast.Function(ast.Name("count"), args=expr.args).set_alias(
+                        ast.Name(f"{readable_name}_count"),
+                    )
+                ),
+            ]
+    acceptable_binary_ops = {
+        ast.BinaryOpKind.Plus,
+        ast.BinaryOpKind.Minus,
+        ast.BinaryOpKind.Multiply,
+        ast.BinaryOpKind.Divide,
+    }
+    if isinstance(expr, ast.BinaryOp):
+        if expr.op in acceptable_binary_ops:  # pragma: no cover
+            measures_left = decompose_expression(expr.left)
+            measures_right = decompose_expression(expr.right)
+            return measures_left + measures_right
+    if isinstance(expr, ast.Cast):
+        return decompose_expression(expr.expression)
+    raise DJInvalidInputException(  # pragma: no cover
+        f"Metric expression {expr} cannot be decomposed into its constituent measures",
+    )
+
+
+def decompose_metrics(combined_ast: ast.Query, dimensions_set: Set[str]):
+    """
+    Decompose each metric into simple constituent measures and return a dict
+    that maps each metric to its measures.
+    """
+    metrics_to_measures = {}
+    for expr in combined_ast.select.projection:
+        if expr.alias_or_name.name not in dimensions_set:  # type: ignore
+            measure_expressions = decompose_expression(expr)
+            metrics_to_measures[expr] = measure_expressions
+    return metrics_to_measures
+
+
 def create_cube_node_revision(  # pylint: disable=too-many-locals
     session: Session,
     data: CreateCubeNode,
 ) -> NodeRevision:
     """
     Create a cube node revision.
     """
```

### Comparing `datajunction_server-0.0.1a6/dj/api/query.py` & `datajunction_server-0.0.1a7/dj/api/query.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/sql.py` & `datajunction_server-0.0.1a7/dj/api/sql.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/api/tags.py` & `datajunction_server-0.0.1a7/dj/api/tags.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/config.py` & `datajunction_server-0.0.1a7/dj/config.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/construction/build.py` & `datajunction_server-0.0.1a7/dj/construction/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -480,33 +480,61 @@
     for dimension_attribute in dimensions:
         if dimension_attribute not in shared_dimensions:
             raise DJInvalidInputException(
                 f"The dimension attribute `{dimension_attribute}` is not "
                 "available on every metric and thus cannot be included.",
             )
 
-    combined_ast = parse(metric_nodes[0].current.query)
+    combined_ast = build_node(
+        session,
+        metric_nodes[0].current,
+        filters,
+        dimensions,
+        build_criteria,
+    )
+    metric_dependencies: Set[str] = set()
     for metric_node in metric_nodes[1:]:
         if metric_node.type != NodeType.METRIC:  # pragma: no cover
             raise DJInvalidInputException(
                 "Cannot build a query for multiple nodes if one or more "
                 f"of them aren't metric nodes. ({metric_node.name} is not"
                 "a metric node)",
             )
+        metric_ast = build_node(
+            session,
+            metric_node.current,
+            filters,
+            dimensions,
+            build_criteria,
+        )
+        metric_dependencies = metric_dependencies.union(
+            {tbl.alias_or_name.name for tbl in metric_ast.find_all(ast.Table)},
+        )
+        built_source_tables = {
+            tbl.alias_or_name.name for tbl in metric_ast.find_all(ast.Table)
+        }
+        diff_columns = set(combined_ast.select.projection).difference(
+            metric_ast.select.projection,
+        )
+        if all(tbl in built_source_tables for tbl in metric_dependencies):
+            metric_ast.select.projection.extend(diff_columns)
+            combined_ast = metric_ast
+        else:
+            combined_ast.select.projection.extend(diff_columns)  # pragma: no cover
 
-        query = parse(metric_node.current.query)
-        combined_ast.select.projection.extend(query.select.projection)
-
-    add_filters_and_dimensions_to_query_ast(
-        combined_ast,
-        build_criteria.dialect if build_criteria else None,
-        filters,
-        dimensions,
-    )
-    return build_ast(session, combined_ast, build_criteria)
+    built_source_tables = {
+        tbl.alias_or_name.name for tbl in combined_ast.find_all(ast.Table)
+    }
+    if not all(tbl in built_source_tables for tbl in metric_dependencies):
+        raise DJInvalidInputException(  # pragma: no cover
+            "We cannot build these metrics together as they aren't "
+            "querying from the same sources. Metric dependencies include "
+            ", ".join(metric_dependencies),
+        )
+    return combined_ast
 
 
 def build_source_node_query(node: NodeRevision):
     """
     Returns a query that selects each column explicitly in the source node.
     """
     table = ast.Table(to_namespaced_name(node.name), None, _dj_node=node)
```

### Comparing `datajunction_server-0.0.1a6/dj/construction/dj_query.py` & `datajunction_server-0.0.1a7/dj/construction/dj_query.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/construction/exceptions.py` & `datajunction_server-0.0.1a7/dj/construction/exceptions.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/construction/utils.py` & `datajunction_server-0.0.1a7/dj/construction/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/errors.py` & `datajunction_server-0.0.1a7/dj/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     UNKNOWN_NODE = 203
     NODE_TYPE_ERROR = 204
     INVALID_DIMENSION_JOIN = 205
     INVALID_COLUMN = 206
 
     # SQL Build Error
     COMPOUND_BUILD_EXCEPTION = 300
-    MISSING_PARENT = 201
+    MISSING_PARENT = 301
+    TYPE_INFERENCE = 302
 
 
 class DebugType(TypedDict, total=False):
     """
     Type for debug information.
     """
```

### Comparing `datajunction_server-0.0.1a6/dj/models/__init__.py` & `datajunction_server-0.0.1a7/dj/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/attribute.py` & `datajunction_server-0.0.1a7/dj/models/attribute.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/base.py` & `datajunction_server-0.0.1a7/dj/models/base.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/catalog.py` & `datajunction_server-0.0.1a7/dj/models/catalog.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/column.py` & `datajunction_server-0.0.1a7/dj/models/column.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,14 +81,23 @@
 
     def identifier(self) -> Tuple[str, ColumnType]:
         """
         Unique identifier for this column.
         """
         return self.name, self.type
 
+    def has_dimension_attribute(self) -> bool:
+        """
+        Whether the dimension attribute is set on this column.
+        """
+        return any(
+            attr.attribute_type.name == "dimension"
+            for attr in self.attributes  # pylint: disable=not-an-iterable
+        )
+
     def __hash__(self) -> int:
         return hash(self.id)
 
     class Config:  # pylint: disable=missing-class-docstring, too-few-public-methods
         arbitrary_types_allowed = True
 
     @root_validator
```

### Comparing `datajunction_server-0.0.1a6/dj/models/database.py` & `datajunction_server-0.0.1a7/dj/models/database.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/engine.py` & `datajunction_server-0.0.1a7/dj/models/engine.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/metric.py` & `datajunction_server-0.0.1a7/dj/models/metric.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/node.py` & `datajunction_server-0.0.1a7/dj/models/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,17 @@
 
         if self.type == NodeType.CUBE:
             if not self.cube_elements:
                 raise DJInvalidInputException(
                     f"Node {self.name} of type cube node needs cube elements",
                 )
 
+    class Config:  # pylint: disable=missing-class-docstring,too-few-public-methods
+        extra = Extra.allow
+
 
 class ImmutableNodeFields(BaseSQLModel):
     """
     Node fields that cannot be changed
     """
 
     name: str
@@ -506,14 +509,22 @@
     """
     Node name only
     """
 
     name: str
 
 
+class NodeNameList(SQLModel):
+    """
+    List of node names
+    """
+
+    __root__: List[str]
+
+
 class AttributeTypeName(BaseSQLModel):
     """
     Attribute type name.
     """
 
     namespace: str
     name: str
```

### Comparing `datajunction_server-0.0.1a6/dj/models/query.py` & `datajunction_server-0.0.1a7/dj/models/query.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/table.py` & `datajunction_server-0.0.1a7/dj/models/table.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/models/tag.py` & `datajunction_server-0.0.1a7/dj/models/tag.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/service_clients.py` & `datajunction_server-0.0.1a7/dj/service_clients.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/dag.py` & `datajunction_server-0.0.1a7/dj/sql/dag.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/functions.py` & `datajunction_server-0.0.1a7/dj/sql/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,21 @@
 @Avg.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     arg: ct.NumberType,
 ) -> ct.DoubleType:
     return ct.DoubleType()
 
 
+@Avg.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: ct.DateTimeBase,
+) -> ct.DateTimeBase:
+    return type(arg.type)()
+
+
 class Min(Function):  # pylint: disable=abstract-method
     """
     Computes the minimum value of the input column or expression.
     """
 
     is_aggregation = True
 
@@ -421,16 +428,16 @@
 class Now(Function):  # pylint: disable=abstract-method
     """
     Returns the current timestamp.
     """
 
 
 @Now.register  # type: ignore
-def infer_type() -> ct.TimestamptzType:  # noqa: F811  # pylint: disable=function-redefined
-    return ct.TimestamptzType()
+def infer_type() -> ct.TimestampType:  # noqa: F811  # pylint: disable=function-redefined
+    return ct.TimestampType()
 
 
 class DateAdd(Function):  # pylint: disable=abstract-method
     """
     Adds a specified number of days to a date.
     """
```

### Comparing `datajunction_server-0.0.1a6/dj/sql/parse.py` & `datajunction_server-0.0.1a7/dj/sql/parse.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/ast.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     FloatType,
     IntegerBase,
     IntegerType,
     MapType,
     NestedField,
     NullType,
     StringType,
+    TimestampType,
+    TimestamptzType,
     WildcardType,
     YearMonthIntervalType,
 )
 
 PRIMITIVES = {int, float, str, bool, type(None)}
 
 
@@ -1035,17 +1037,14 @@
 
 # pylint: disable=C0103
 class UnaryOpKind(DJEnum):
     """
     The accepted unary operations
     """
 
-    #
-    # Plus = "+"
-    # Minus = "-"
     Exists = "EXISTS"
     Not = "NOT"
 
     def __str__(self):
         return self.value
 
 
@@ -1202,20 +1201,22 @@
             )
         }
 
         def resolve_numeric_types_binary_operations(
             left: ColumnType,
             right: ColumnType,
         ):
-            if str(left) not in numeric_types or str(right) not in numeric_types:
+            if not left.is_compatible(right):
                 raise_binop_exception()
-            if str(left) == str(right):
+            if str(left) in numeric_types and str(right) in numeric_types:
+                if str(left) == str(right):
+                    return left
+                if numeric_types[str(left)] > numeric_types[str(right)]:
+                    return right
                 return left
-            if numeric_types[str(left)] > numeric_types[str(right)]:
-                return right
             return left
 
         BINOP_TYPE_COMBO_LOOKUP: Dict[  # pylint: disable=C0103
             BinaryOpKind,
             Callable[[ColumnType, ColumnType], ColumnType],
         ] = {
             BinaryOpKind.And: lambda left, right: BooleanType(),
```

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/antlr4.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/antlr4.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/SqlBaseParser.g4` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/SqlBaseParser.g4`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/sql/parsing/types.py` & `datajunction_server-0.0.1a7/dj/sql/parsing/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
         True
     """
 
     def __init__(self):
         super().__init__("time", "TimeType()")
 
 
-class TimestampType(PrimitiveType, Singleton):
+class TimestampType(DateTimeBase):
     """A Timestamp data type can be represented using an instance of this class. Timestamps in
     Column have microsecond precision and include a date and a time of day without a timezone.
 
     Example:
         >>> column_foo = TimestampType()
         >>> isinstance(column_foo, TimestampType)
         True
```

### Comparing `datajunction_server-0.0.1a6/dj/superset.py` & `datajunction_server-0.0.1a7/dj/superset.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/typing.py` & `datajunction_server-0.0.1a7/dj/typing.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/dj/utils.py` & `datajunction_server-0.0.1a7/dj/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction_server-0.0.1a6/pyproject.toml` & `datajunction_server-0.0.1a7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools_scm]
 # See configuration details in https://github.com/pypa/setuptools_scm
 version_scheme = "no-guess-dev"
 
 [tool.poetry]
 name = "datajunction-server"
-version = "0.0.1a6"
+version = "0.0.1a7"
 readme = "README.rst"
 repository = "https://github.com/DataJunction/dj"
 description = "DataJunction server library for running to a DataJunction server"
 authors = ["DataJunction Authors"]
 license = "MIT"
 packages = [
     { include = "dj" },
```

### Comparing `datajunction_server-0.0.1a6/PKG-INFO` & `datajunction_server-0.0.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajunction-server
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: DataJunction server library for running to a DataJunction server
 Home-page: https://github.com/DataJunction/dj
 License: MIT
 Author: DataJunction Authors
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

