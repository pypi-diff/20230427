# Comparing `tmp/sqlalchemy-iris-0.8.0.tar.gz` & `tmp/sqlalchemy-iris-0.8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-iris-0.8.0.tar", last modified: Tue Apr 25 16:06:16 2023, max compression
+gzip compressed data, was "sqlalchemy-iris-0.8.1b1.tar", last modified: Thu Apr 27 13:58:31 2023, max compression
```

## Comparing `sqlalchemy-iris-0.8.0.tar` & `sqlalchemy-iris-0.8.1b1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.548549 sqlalchemy-iris-0.8.0/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.552549 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    95424 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.552549 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.552549 sqlalchemy-iris-0.8.0/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.552549 sqlalchemy-iris-0.8.0/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.552549 sqlalchemy-iris-0.8.0/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-25 16:06:12.000000 sqlalchemy-iris-0.8.0/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/sqlalchemy_iris/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40685 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/information_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 16:06:16.000000 sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:06:16.556549 sqlalchemy-iris-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-25 16:05:56.000000 sqlalchemy-iris-0.8.0/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.160537 sqlalchemy-iris-0.8.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 13:58:31.160537 sqlalchemy-iris-0.8.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.148537 sqlalchemy-iris-0.8.1b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.152536 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    95597 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4687 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.152536 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.156537 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.156537 sqlalchemy-iris-0.8.1b1/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.156537 sqlalchemy-iris-0.8.1b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-27 13:58:25.000000 sqlalchemy-iris-0.8.1b1/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-27 13:58:31.160537 sqlalchemy-iris-0.8.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.156537 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48854 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/information_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.160537 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:58:31.000000 sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:31.160537 sqlalchemy-iris-0.8.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-27 13:58:02.000000 sqlalchemy-iris-0.8.1b1/tests/test_suite.py
```

### Comparing `sqlalchemy-iris-0.8.0/LICENSE` & `sqlalchemy-iris-0.8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/PKG-INFO` & `sqlalchemy-iris-0.8.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.8.0
+Version: 0.8.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.8.0/README.md` & `sqlalchemy-iris-0.8.1b1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_BufferWriter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_ConnectionInformation.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_ConnectionParameters.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_Constant.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_DBList.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_Device.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_GatewayContext.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_GatewayUtility.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRIS.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISConnection.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISEmbedded.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISGlobalNode.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISGlobalNodeView.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISIterator.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISList.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISNative.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISObject.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_IRISReference.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_InStream.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_LegacyIterator.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_ListReader.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_ListWriter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_LogFileStream.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_MessageHeader.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_OutStream.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_PrintStream.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_PythonGateway.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/_SharedMemorySocket.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/__init__.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Column.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_DBAPI.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -2196,33 +2196,36 @@
         values = [None if v == '' else '' if v == '\x00' else v for v in values]
         row = namedtuple('Row', [col.name for col in self._columns], rename=True)
 
         _types = {
             SQLType.BIGINT: int,
             SQLType.BINARY: bytes,
             SQLType.BIT: bool,
+            SQLType.FLOAT: float,
+            SQLType.NUMERIC: decimal.Decimal,
             SQLType.INTEGER: int,
             SQLType.VARCHAR: str,
             SQLType.LONGVARBINARY: IRISBinaryStream,
             SQLType.LONGVARCHAR: IRISStream,
         }
         
         if self._columns:
             for _column in self._columns:
                 value = values[_column.slotPosition - 1]
 
                 ctype = _column.type
                 value_type = _types[ctype] if ctype in _types else None
                 try:
-                    if type(value) == float:
-                        value = decimal.Decimal(str(value))
-                    elif not _column.tableName and not _column.schema:
-                        pass
+                    if not _column.tableName and not _column.schema:
+                        if type(value) == float:
+                            value = decimal.Decimal(str(value))
                     elif value is None or value_type is None:
                         pass
+                    elif value_type is decimal.Decimal:
+                        value = decimal.Decimal(str(value))
                     elif issubclass(value_type, IRISStream):
                         stream = value_type(self._connection, value, embedded=True)
                         value = stream.fetch()
                     elif not isinstance(value, value_type):
                         value = value_type(value)
                 except Exception as ex:
                     raise ex
```

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Descriptor.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_IRISStream.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Message.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_Parameter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,16 @@
             int: lambda v : v,
             float: lambda v : v,
             decimal.Decimal: lambda v : v,
         }
         func = _set_switcher[type(self.__value)] if type(self.__value) in _set_switcher else (lambda v : str(v))
         value = func(self.__value)
         if self.mode == ParameterMode.REPLACED_LITERAL:
-            try:
+            if isinstance(value, str) and value.isdigit():
                 value = int(value)
-            except:
-                try:
-                    value = float(value)
-                except:
-                    pass
         return value
 
     def _copy_cached_info(self, desc, copy_replaced):
         self.type = desc.type
         self.precision = desc.precision
         self.scale = desc.scale
         self.nullable = desc.nullable
```

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_ParameterCollection.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_ResultSetRow.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/_SQLType.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_PreParser.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_Scanner.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_Token.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/dbapi/preparser/_TokenList.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessHost.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessOperation.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessProcess.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_BusinessService.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_Common.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_Director.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISBusinessService.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_IRISOutboundAdapter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_InboundAdapter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/_OutboundAdapter.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/intersystems_iris/pex/__init__.py` & `sqlalchemy-iris-0.8.1b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/iris/__init__.py` & `sqlalchemy-iris-0.8.1b1/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/iris/irisbuiltins.py` & `sqlalchemy-iris-0.8.1b1/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/iris/irisloader.py` & `sqlalchemy-iris-0.8.1b1/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/irisnative/_IRISNative.py` & `sqlalchemy-iris-0.8.1b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/setup.cfg` & `sqlalchemy-iris-0.8.1b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy-iris
-version = 0.8.0
+version = 0.8.1b1
 description = InterSystems IRIS for SQLAlchemy
 long_description = file: README.md
 url = https://github.com/caretdev/sqlalchemy-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 long_description_content_type = text/markdown
```

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/__init__.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/base.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,61 @@
 from sqlalchemy.sql.functions import ReturnTypeFromArgs
 from sqlalchemy.sql import expression
 from sqlalchemy.sql import schema
 from sqlalchemy import sql, text
 from sqlalchemy import util
 from sqlalchemy import types as sqltypes
 
+from sqlalchemy import __version__ as sqlalchemy_version
+
+if sqlalchemy_version.startswith("2."):
+    from sqlalchemy.engine import ObjectKind
+    from sqlalchemy.engine import ObjectScope
+    from sqlalchemy.engine.reflection import ReflectionDefaults
+else:
+    from enum import Flag
+
+    class ObjectKind(Flag):
+        TABLE = 1
+        VIEW = 2
+        ANY = TABLE | VIEW
+
+    class ObjectScope(Flag):
+        DEFAULT = 1
+        TEMPORARY = 2
+        ANY = DEFAULT | TEMPORARY
+
+    class ReflectionDefaults:
+        @classmethod
+        def columns(cls):
+            return []
+
+        @classmethod
+        def pk_constraint(cls):
+            return {
+                "name": None,
+                "constrained_columns": [],
+            }
+
+        @classmethod
+        def foreign_keys(cls):
+            return []
+
+        @classmethod
+        def indexes(cls):
+            return []
+
+        @classmethod
+        def unique_constraints(cls):
+            return []
+
+        @classmethod
+        def check_constraints(cls):
+            return []
+
 from sqlalchemy.types import BIGINT
 from sqlalchemy.types import VARCHAR
 from sqlalchemy.types import INTEGER
 from sqlalchemy.types import DATE
 from sqlalchemy.types import TIMESTAMP
 from sqlalchemy.types import TIME
 from sqlalchemy.types import NUMERIC
@@ -346,15 +393,15 @@
 
     def limit_clause(self, select, **kw):
         return ""
 
     def fetch_clause(self, select, **kw):
         return ""
 
-    def visit_empty_set_expr(self, type_):
+    def visit_empty_set_expr(self, type_, **kw):
         return "SELECT 1 WHERE 1!=1"
 
     def _get_limit_or_fetch(self, select):
         if select._fetch_clause is None:
             return select._limit_clause
         else:
             return select._fetch_clause
@@ -508,16 +555,16 @@
 
     def visit_column(self, column, within_columns_clause=False, **kwargs):
         text = super().visit_column(
             column, within_columns_clause=within_columns_clause, **kwargs
         )
         if within_columns_clause:
             return text
-        if isinstance(column.type, sqltypes.Text):
-            text = "CONVERT(VARCHAR, %s)" % (text,)
+        # if isinstance(column.type, sqltypes.Text):
+        #     text = "CONVERT(VARCHAR, %s)" % (text,)
         return text
 
     def visit_concat_op_binary(self, binary, operator, **kw):
         return "STRING(%s, %s)" % (
             self.process(binary.left, **kw),
             self.process(binary.right, **kw),
         )
@@ -541,23 +588,29 @@
             x += clause.value._compiler_dispatch(self, **kwargs) + " "
         for cond, result in clause.whens:
             x += (
                 "WHEN "
                 + cond._compiler_dispatch(self, **kwargs)
                 + " THEN "
                 # Explicit CAST required on 2023.1
-                + (self.visit_cast(sql.cast(result, result.type), **kwargs)
-                    if isinstance(result, sql.elements.BindParameter) else result._compiler_dispatch(self, **kwargs))
+                + (
+                    self.visit_cast(sql.cast(result, result.type), **kwargs)
+                    if isinstance(result, sql.elements.BindParameter)
+                    else result._compiler_dispatch(self, **kwargs)
+                )
                 + " "
             )
         if clause.else_ is not None:
             x += (
-                "ELSE " 
-                + (self.visit_cast(sql.cast(clause.else_, clause.else_.type), **kwargs)
-                    if isinstance(clause.else_, sql.elements.BindParameter) else clause.else_._compiler_dispatch(self, **kwargs))
+                "ELSE "
+                + (
+                    self.visit_cast(sql.cast(clause.else_, clause.else_.type), **kwargs)
+                    if isinstance(clause.else_, sql.elements.BindParameter)
+                    else clause.else_._compiler_dispatch(self, **kwargs)
+                )
                 + " "
             )
         x += "END"
         return x
 
 
 class IRISDDLCompiler(sql.compiler.DDLCompiler):
@@ -638,24 +691,30 @@
         index = create.element
         preparer = self.preparer
 
         # handle other included columns
         includeclause = index.dialect_options["iris"]["include"]
         if includeclause:
             inclusions = [
-                index.table.c[col] if isinstance(col, util.string_types) else col
+                index.table.c[col] if isinstance(col, str) else col
                 for col in includeclause
             ]
 
             text += " WITH DATA (%s)" % ", ".join(
                 [preparer.quote(c.name) for c in inclusions]
             )
 
         return text
 
+    def visit_drop_index(self, drop, **kw):
+        return "DROP INDEX %s ON %s" % (
+            self._prepared_index_name(drop.element, include_schema=False),
+            self.preparer.format_table(drop.element.table),
+        )
+
 
 class IRISTypeCompiler(compiler.GenericTypeCompiler):
     def visit_BOOLEAN(self, type_, **kw):
         return self.visit_BIT(type_)
 
     def visit_BIT(self, type_, **kw):
         return "BIT"
@@ -749,14 +808,16 @@
     supports_native_boolean = True
     non_native_boolean_check_constraint = False
 
     supports_multivalues_insert = True
 
     supports_sequences = False
 
+    div_is_floordiv = False
+
     postfetch_lastrowid = True
     supports_simple_order_by_label = False
     supports_empty_insert = False
     supports_is_distinct_from = False
 
     colspecs = colspecs
 
@@ -887,15 +948,15 @@
         opts["password"] = url.password if url.password else ""
 
         opts["autoCommit"] = False
 
         opts["embedded"] = self.embedded
         if opts["hostname"] and "@" in opts["hostname"]:
             _h = opts["hostname"].split("@")
-            opts["password"] += "@" + _h[0: len(_h) - 1].join("@")
+            opts["password"] += "@" + _h[0 : len(_h) - 1].join("@")
             opts["hostname"] = _h[len(_h) - 1]
 
         return ([], opts)
 
     _debug_queries = False
     # _debug_queries = True
 
@@ -982,53 +1043,135 @@
             )
             .order_by(tables.c.table_name)
         )
         table_names = [r[0] for r in connection.execute(s)]
         return table_names
 
     @reflection.cache
+    def get_temp_table_names(self, connection, dblink=None, **kw):
+        tables = ischema.tables
+        s = (
+            sql.select(tables.c.table_name)
+            .where(
+                sql.and_(
+                    tables.c.table_schema == self.default_schema_name,
+                    tables.c.table_type == "GLOBAL TEMPORARY",
+                )
+            )
+            .order_by(tables.c.table_name)
+        )
+        table_names = [r[0] for r in connection.execute(s)]
+        return table_names
+
+    @reflection.cache
     def has_table(self, connection, table_name, schema=None, **kw):
         self._ensure_has_table_connection(connection)
         tables = ischema.tables
         schema_name = self.get_schema(schema)
 
         s = sql.select(func.count()).where(
             sql.and_(
                 tables.c.table_schema == str(schema_name),
                 tables.c.table_name == str(table_name),
             )
         )
         return bool(connection.execute(s).scalar())
 
+    def _default_or_error(self, connection, tablename, schema, method, **kw):
+        if self.has_table(connection, tablename, schema, **kw):
+            return method()
+        else:
+            raise exc.NoSuchTableError(f"{schema}.{tablename}")
+
+    def _get_all_objects(self, connection, schema, filter_names, scope, kind, **kw):
+        self._ensure_has_table_connection(connection)
+        tables = ischema.tables
+        schema_name = self.get_schema(schema)
+
+        s = (
+            sql.select(
+                tables.c.table_name,
+            )
+            .select_from(tables)
+            .where(
+                tables.c.table_schema == str(schema_name),
+            )
+        )
+
+        table_types = []
+        if ObjectScope.TEMPORARY in scope and ObjectKind.TABLE in kind:
+            table_types.append("GLOBAL TEMPORARY")
+        if ObjectScope.DEFAULT in scope and ObjectKind.VIEW in kind:
+            table_types.append("VIEW")
+        if ObjectScope.DEFAULT in scope and ObjectKind.TABLE in kind:
+            table_types.append("BASE TABLE")
+
+        if not table_types:
+            return []
+        s = s.where(tables.c.table_type.in_(table_types))
+
+        if filter_names:
+            s = s.where(tables.c.table_name.in_([str(name) for name in filter_names]))
+
+        result = connection.execute(s).scalars()
+        return result.all()
+
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, unique=False, **kw):
+        data = self.get_multi_indexes(
+            connection,
+            schema=schema,
+            filter_names=[table_name],
+            scope=ObjectScope.ANY,
+            kind=ObjectKind.ANY,
+            unique=unique,
+            **kw,
+        )
+        return self._value_or_raise(data, table_name, schema)
+
+    def get_multi_indexes(
+        self, connection, schema, filter_names, scope, kind, unique=False, **kw
+    ):
         schema_name = self.get_schema(schema)
         indexes = ischema.indexes
         tables = ischema.tables
         index_def = ischema.index_definition
 
+        all_objects = self._get_all_objects(
+            connection, schema, filter_names, scope, kind
+        )
+        if not all_objects:
+            return util.defaultdict(list)
+
         s = (
             sql.select(
+                indexes.c.table_name,
                 indexes.c.index_name,
                 indexes.c.column_name,
                 indexes.c.primary_key,
                 indexes.c.non_unique,
                 indexes.c.asc_or_desc,
             )
             .select_from(indexes)
             .where(
                 sql.and_(
                     indexes.c.table_schema == str(schema_name),
-                    indexes.c.table_name == str(table_name),
+                    indexes.c.table_name.in_(all_objects),
                     indexes.c.primary_key == sql.false(),
-                    (indexes.c.non_unique == sql.true()) if not unique else (1 == 1),
                 )
             )
-            .order_by(indexes.c.ordinal_position)
+            .order_by(
+                indexes.c.table_name,
+                indexes.c.index_name,
+                indexes.c.ordinal_position,
+            )
         )
+        if unique:
+            s = s.where(indexes.c.non_unique != sql.true())
+
         if self._dictionary_access:
             s = s.add_columns(
                 index_def.c.Data,
             ).outerjoin(
                 index_def,
                 sql.and_(
                     index_def.c.SqlName == indexes.c.index_name,
@@ -1042,105 +1185,212 @@
                 ),
             )
         else:
             s = s.add_columns(None)
 
         rs = connection.execute(s)
 
+        flat_indexes = util.defaultdict(dict)
+        default = ReflectionDefaults.indexes
+
         indexes = util.defaultdict(dict)
+        for table_name in all_objects:
+            indexes[(schema, table_name)] = default()
+
         for row in rs:
             (
+                idxtable,
                 idxname,
                 colname,
                 _,
                 nuniq,
                 _,
                 include,
             ) = row
 
-            indexrec = indexes[idxname]
+            if (schema, idxtable) not in indexes:
+                continue
+
+            indexrec = flat_indexes[(schema, idxtable, idxname)]
             if "name" not in indexrec:
                 indexrec["name"] = self.normalize_name(idxname)
                 indexrec["column_names"] = []
-                indexrec["unique"] = not nuniq
+                if not unique:
+                    indexrec["unique"] = not nuniq
+                else:
+                    indexrec["duplicates_index"] = idxname
 
             indexrec["column_names"].append(self.normalize_name(colname))
             include = include.split(",") if include else []
-            indexrec["include_columns"] = include
+            if not unique or include:
+                indexrec["include_columns"] = include
             if include:
                 indexrec["dialect_options"] = {"iris_include": include}
 
-        indexes = list(indexes.values())
+        for schema, idxtable, idxname in flat_indexes:
+            indexes[(schema, idxtable)].append(
+                flat_indexes[(schema, idxtable, idxname)]
+            )
+
         return indexes
 
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
+        data = self.get_multi_pk_constraint(
+            connection,
+            schema,
+            filter_names=[table_name],
+            scope=ObjectScope.ANY,
+            kind=ObjectKind.ANY,
+            **kw,
+        )
+        return self._value_or_raise(data, table_name, schema)
+
+    def get_multi_pk_constraint(
+        self,
+        connection,
+        schema,
+        filter_names,
+        scope,
+        kind,
+        **kw,
+    ):
         schema_name = self.get_schema(schema)
         key_constraints = ischema.key_constraints
         constraints = ischema.constraints
 
+        all_objects = self._get_all_objects(
+            connection, schema, filter_names, scope, kind
+        )
+        if not all_objects:
+            return util.defaultdict(list)
+
         s = (
             sql.select(
+                key_constraints.c.table_name,
                 key_constraints.c.constraint_name,
                 key_constraints.c.column_name,
             )
             .join(
                 constraints,
                 sql.and_(
                     key_constraints.c.constraint_name == constraints.c.constraint_name,
                     key_constraints.c.table_schema == constraints.c.table_schema,
                 ),
             )
             .where(
                 sql.and_(
                     key_constraints.c.table_schema == str(schema_name),
-                    key_constraints.c.table_name == str(table_name),
+                    key_constraints.c.table_name.in_(all_objects),
                     constraints.c.constraint_type == "PRIMARY KEY",
                 )
             )
-            .order_by(key_constraints.c.ordinal_position)
+            .order_by(
+                key_constraints.c.table_name,
+                key_constraints.c.constraint_name,
+                key_constraints.c.ordinal_position,
+            )
         )
 
         rs = connection.execute(s)
 
+        primary_keys = util.defaultdict(dict)
+        default = ReflectionDefaults.pk_constraint
+
         constraint_name = None
-        pkfields = []
         for row in rs:
             (
+                table_name,
                 name,
                 colname,
             ) = row
             constraint_name = self.normalize_name(name)
-            pkfields.append(self.normalize_name(colname))
 
-        if pkfields:
-            return {
-                "constrained_columns": pkfields,
-                "name": constraint_name,
-            }
+            table_pk = primary_keys[(schema, table_name)]
+            if not table_pk:
+                table_pk["name"] = constraint_name
+                table_pk["constrained_columns"] = [colname]
+            else:
+                table_pk["constrained_columns"].append(colname)
 
-        return None
+        return (
+            (key, primary_keys[key] if key in primary_keys else default())
+            for key in (
+                (schema, self.normalize_name(obj_name)) for obj_name in all_objects
+            )
+        )
+
+    def _value_or_raise(self, data, table, schema):
+        table = self.normalize_name(str(table))
+        try:
+            return dict(data)[(schema, table)]
+        except KeyError:
+            raise exc.NoSuchTableError(
+                f"{schema}.{table}" if schema else table
+            ) from None
 
     @reflection.cache
     def get_unique_constraints(self, connection, table_name, schema=None, **kw):
-        indexes = self.get_indexes(connection, table_name, schema, unique=True, **kw)
-        return [
-            {"name": i["name"], "column_names": i["column_names"]}
-            for i in indexes
-            if i["unique"]
-        ]
+        data = self.get_multi_unique_constraints(
+            connection,
+            schema=schema,
+            filter_names=[table_name],
+            scope=ObjectScope.ANY,
+            kind=ObjectKind.ANY,
+            **kw,
+        )
+        return self._value_or_raise(data, table_name, schema)
+
+    def get_multi_unique_constraints(
+        self,
+        connection,
+        schema,
+        filter_names,
+        scope,
+        kind,
+        **kw,
+    ):
+        return self.get_multi_indexes(
+            connection, schema, filter_names, scope, kind, unique=True, **kw
+        )
 
     @reflection.cache
     def get_foreign_keys(self, connection, table_name, schema=None, **kw):
+        data = self.get_multi_foreign_keys(
+            connection,
+            schema,
+            filter_names=[table_name],
+            scope=ObjectScope.ANY,
+            kind=ObjectKind.ANY,
+            **kw,
+        )
+        return self._value_or_raise(data, table_name, schema)
+
+    def get_multi_foreign_keys(
+        self,
+        connection,
+        schema,
+        filter_names,
+        scope,
+        kind,
+        **kw,
+    ):
         schema_name = self.get_schema(schema)
         ref_constraints = ischema.ref_constraints
         key_constraints = ischema.key_constraints
         key_constraints_ref = aliased(ischema.key_constraints)
 
+        all_objects = self._get_all_objects(
+            connection, schema, filter_names, scope, kind
+        )
+        if not all_objects:
+            return util.defaultdict(list)
+
         s = (
             sql.select(
+                key_constraints.c.table_name,
                 key_constraints.c.constraint_name,
                 key_constraints.c.column_name,
                 key_constraints_ref.c.table_schema,
                 key_constraints_ref.c.table_name,
                 key_constraints_ref.c.column_name,
                 ref_constraints.c.match_option,
                 ref_constraints.c.update_rule,
@@ -1165,102 +1415,127 @@
                     key_constraints_ref.c.ordinal_position
                     == key_constraints.c.ordinal_position,
                 ),
             )
             .where(
                 sql.and_(
                     key_constraints.c.table_schema == str(schema_name),
-                    key_constraints.c.table_name == str(table_name),
+                    key_constraints.c.table_name.in_(all_objects),
                 )
             )
-            .order_by(key_constraints_ref.c.ordinal_position)
+            .order_by(
+                key_constraints.c.constraint_name,
+                key_constraints.c.ordinal_position,
+            )
         )
 
         rs = connection.execute(s)
 
-        fkeys = []
-
-        def fkey_rec():
-            return {
-                "name": None,
-                "constrained_columns": [],
-                "referred_schema": None,
-                "referred_table": None,
-                "referred_columns": [],
-                "options": {},
-            }
-
-        fkeys = util.defaultdict(fkey_rec)
+        fkeys = util.defaultdict(dict)
 
         for row in rs:
             (
+                table_name,
                 rfknm,
                 scol,
                 rschema,
                 rtbl,
                 rcol,
                 _,  # match rule
                 fkuprule,
                 fkdelrule,
             ) = row
 
-            rec = fkeys[rfknm]
-            rec["name"] = rfknm
+            table_fkey = fkeys[(schema, table_name)]
+
+            if rfknm not in table_fkey:
+                table_fkey[rfknm] = fkey = {
+                    "name": rfknm,
+                    "constrained_columns": [],
+                    "referred_schema": rschema
+                    if rschema != self.default_schema_name
+                    else None,
+                    "referred_table": rtbl,
+                    "referred_columns": [],
+                    "options": {},
+                }
+            else:
+                fkey = table_fkey[rfknm]
 
             if fkuprule != "NO ACTION":
-                rec["options"]["onupdate"] = fkuprule
+                fkey["options"]["onupdate"] = fkuprule
 
             if fkdelrule != "NO ACTION":
-                rec["options"]["ondelete"] = fkdelrule
-
-            if not rec["referred_table"]:
-                rec["referred_table"] = rtbl
-                if rschema != "SQLUser":
-                    rec["referred_schema"] = rschema
+                fkey["options"]["ondelete"] = fkdelrule
 
-            local_cols, remote_cols = (
-                rec["constrained_columns"],
-                rec["referred_columns"],
-            )
-
-            local_cols.append(scol)
-            remote_cols.append(rcol)
+            fkey["constrained_columns"].append(scol)
+            fkey["referred_columns"].append(rcol)
 
-        if fkeys:
-            return list(fkeys.values())
+        default = ReflectionDefaults.foreign_keys
 
-        return []
+        return (
+            (key, list(fkeys[key].values()) if key in fkeys else default())
+            for key in (
+                (schema, self.normalize_name(obj_name)) for obj_name in all_objects
+            )
+        )
 
     def get_columns(self, connection, table_name, schema=None, **kw):
+        data = self.get_multi_columns(
+            connection,
+            schema,
+            filter_names=[table_name],
+            scope=ObjectScope.ANY,
+            kind=ObjectKind.ANY,
+            **kw,
+        )
+        return self._value_or_raise(data, table_name, schema)
+
+    def get_multi_columns(
+        self,
+        connection,
+        schema,
+        filter_names,
+        scope,
+        kind,
+        **kw,
+    ):
         schema_name = self.get_schema(schema)
         tables = ischema.tables
         columns = ischema.columns
         property = ischema.property_definition
 
-        whereclause = sql.and_(
-            columns.c.table_name == str(table_name),
-            columns.c.table_schema == str(schema_name),
+        all_objects = self._get_all_objects(
+            connection, schema, filter_names, scope, kind
         )
+        if not all_objects:
+            return util.defaultdict(list)
 
         s = (
             sql.select(
+                columns.c.table_name,
                 columns.c.column_name,
                 columns.c.data_type,
                 columns.c.is_nullable,
                 columns.c.character_maximum_length,
                 columns.c.numeric_precision,
                 columns.c.numeric_scale,
                 columns.c.column_default,
                 columns.c.collation_name,
                 columns.c.auto_increment,
             )
             .select_from(columns)
-            .where(whereclause)
+            .where(
+                columns.c.table_schema == str(schema_name),
+            )
             .order_by(columns.c.ordinal_position)
         )
+        if all_objects:
+            s = s.where(columns.c.table_name.in_(all_objects))
+
         if self._dictionary_access:
             s = s.add_columns(
                 property.c.SqlComputeCode,
                 property.c.Calculated,
                 property.c.Transient,
             ).outerjoin(
                 property,
@@ -1274,16 +1549,18 @@
                     )
                     .scalar_subquery(),
                 ),
             )
 
         c = connection.execution_options(future_result=True).execute(s)
 
-        cols = []
+        cols = util.defaultdict(list)
+
         for row in c.mappings():
+            table_name = row[columns.c.table_name]
             name = row[columns.c.column_name]
             type_ = row[columns.c.data_type].upper()
             nullable = row[columns.c.is_nullable]
             charlen = row[columns.c.character_maximum_length]
             numericprec = row[columns.c.numeric_precision]
             numericscale = row[columns.c.numeric_scale]
             default = row[columns.c.column_default]
@@ -1338,15 +1615,15 @@
                 sqltext = sqltext.split(" = ")[1]
                 sqltext = re.sub(r"{(\b\w+\b)}", r"\g<1>", sqltext)
                 persisted = not calculated and not transient
                 cdict["computed"] = {
                     "sqltext": sqltext,
                     "persisted": persisted,
                 }
-            cols.append(cdict)
+            cols[(schema, table_name)].append(cdict)
 
         return cols
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         schema_name = self.get_schema(schema)
         views = ischema.views
@@ -1370,8 +1647,8 @@
                 views.c.table_schema == str(schema_name),
                 views.c.table_name == str(view_name),
             )
         ).scalar()
 
         if view_def:
             return view_def
-        return None
+        raise exc.NoSuchTableError(f"{schema}.{view_name}")
```

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/embedded.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/embedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/information_schema.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/information_schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/requirements.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from sqlalchemy.testing.requirements import SuiteRequirements
 
 from sqlalchemy.testing import exclusions
 
 
 class Requirements(SuiteRequirements):
     @property
+    def array_type(self):
+        return exclusions.closed()
+
+    @property
+    def uuid_data_type(self):
+        return exclusions.closed()
+
+    @property
     def check_constraints(self):
         """Target database must support check constraints."""
 
         return exclusions.closed()
 
     @property
     def views(self):
@@ -210,7 +218,24 @@
         return {"default": default, "supported": levels}
 
     @property
     def regexp_match(self):
         """backend supports the regexp_match operator."""
         # InterSystems use own format for %MATCHES and %PATTERN, it does not support Regular Expressions
         return exclusions.closed()
+
+    @property
+    def unique_constraints_reflect_as_index(self):
+        """Target database reflects unique constraints as indexes."""
+
+        return exclusions.open()
+
+    @property
+    def temp_table_names(self):
+        """target dialect supports listing of temporary table names"""
+        return exclusions.open()
+
+    @property
+    def unique_index_reflect_as_unique_constraints(self):
+        """Target database reflects unique indexes as unique constrains."""
+
+        return exclusions.open()
```

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris/types.py` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/PKG-INFO` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.8.0
+Version: 0.8.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.8.0/sqlalchemy_iris.egg-info/SOURCES.txt` & `sqlalchemy-iris-0.8.1b1/sqlalchemy_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.8.0/tests/test_suite.py` & `sqlalchemy-iris-0.8.1b1/tests/test_suite.py`

 * *Files identical despite different names*

