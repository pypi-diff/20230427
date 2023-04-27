# Comparing `tmp/mypy-boto3-kafka-1.26.122.tar.gz` & `tmp/mypy-boto3-kafka-1.26.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.26.122.tar", last modified: Thu Apr 27 19:33:40 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.26.60.tar", last modified: Mon Jan 30 21:06:23 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.26.122.tar` & `mypy-boto3-kafka-1.26.60.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.616081 mypy-boto3-kafka-1.26.122/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-04-27 19:33:40.616081 mypy-boto3-kafka-1.26.122/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.616081 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34826 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54484 2023-04-27 19:32:54.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54417 2023-04-27 19:32:53.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.616081 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 19:33:40.000000 mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:40.616081 mypy-boto3-kafka-1.26.122/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-27 19:32:52.000000 mypy-boto3-kafka-1.26.122/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.542472 mypy-boto3-kafka-1.26.60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-01-30 21:06:23.538471 mypy-boto3-kafka-1.26.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.534471 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45275 2023-01-30 21:06:02.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.538471 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:23.542472 mypy-boto3-kafka-1.26.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/setup.py
```

### Comparing `mypy-boto3-kafka-1.26.122/LICENSE` & `mypy-boto3-kafka-1.26.60/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-kafka-1.26.122/PKG-INFO` & `mypy-boto3-kafka-1.26.60/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.26.122
-Summary: Type annotations for boto3.Kafka 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.60
+Summary: Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,33 +279,28 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
-    "list_client_vpc_connections"
-)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -314,17 +309,14 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
-    "list_vpc_connections"
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -335,28 +327,24 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
-    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
-    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
-    UserIdentityTypeType,
-    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -381,87 +369,67 @@
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
-    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
     CreateConfigurationRequestRequestTypeDef,
-    CreateVpcConnectionRequestRequestTypeDef,
-    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeVpcConnectionRequestRequestTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetClusterPolicyRequestRequestTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     PaginatorConfigTypeDef,
-    ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersV2RequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
     ListNodesRequestRequestTypeDef,
     ListScramSecretsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVpcConnectionsRequestRequestTypeDef,
-    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PutClusterPolicyRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RejectClientVpcConnectionRequestRequestTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBootstrapBrokersResponseTypeDef,
-    GetClusterPolicyResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
@@ -471,63 +439,55 @@
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
-    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListNodesRequestListNodesPaginateTypeDef,
     ListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
-    VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityTypeDef,
-    ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
+    UpdateSecurityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -547,42 +507,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-kafka-1.26.122/README.md` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kafka
+Version: 1.26.60
+Summary: Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,33 +279,28 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
-    "list_client_vpc_connections"
-)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -282,17 +309,14 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
-    "list_vpc_connections"
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -303,28 +327,24 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
-    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
-    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
-    UserIdentityTypeType,
-    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -349,87 +369,67 @@
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
-    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
     CreateConfigurationRequestRequestTypeDef,
-    CreateVpcConnectionRequestRequestTypeDef,
-    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeVpcConnectionRequestRequestTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetClusterPolicyRequestRequestTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     PaginatorConfigTypeDef,
-    ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersV2RequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
     ListNodesRequestRequestTypeDef,
     ListScramSecretsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVpcConnectionsRequestRequestTypeDef,
-    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PutClusterPolicyRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RejectClientVpcConnectionRequestRequestTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBootstrapBrokersResponseTypeDef,
-    GetClusterPolicyResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
@@ -439,63 +439,55 @@
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
-    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListNodesRequestListNodesPaginateTypeDef,
     ListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
-    VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityTypeDef,
-    ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
+    UpdateSecurityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -515,42 +507,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,65 +4,57 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
-        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
-        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
-    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 
 Client = KafkaClient
 
 
 __all__ = (
     "Client",
     "KafkaClient",
-    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
-    "ListVpcConnectionsPaginator",
 )
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,64 +4,56 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
-        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
-        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
-    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 
 Client = KafkaClient
 
 __all__ = (
     "Client",
     "KafkaClient",
-    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
-    "ListVpcConnectionsPaginator",
 )
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.26.122\nVersion:         1.26.122\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Kafka 1.26.60\nVersion:         1.26.60\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.122")
+    print("1.26.60")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,67 +17,58 @@
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
-    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
-    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     LoggingInfoTypeDef,
     OpenMonitoringInfoTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedThroughputTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     ServerlessRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
@@ -219,67 +210,33 @@
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_configuration)
         """
 
-    def create_vpc_connection(
-        self,
-        *,
-        TargetClusterArn: str,
-        Authentication: str,
-        VpcId: str,
-        ClientSubnets: Sequence[str],
-        SecurityGroups: Sequence[str],
-        Tags: Mapping[str, str] = ...
-    ) -> CreateVpcConnectionResponseTypeDef:
-        """
-        Creates a new MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_vpc_connection)
-        """
-
     def delete_cluster(
         self, *, ClusterArn: str, CurrentVersion: str = ...
     ) -> DeleteClusterResponseTypeDef:
         """
         Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster)
         """
 
-    def delete_cluster_policy(self, *, ClusterArn: str) -> Dict[str, Any]:
-        """
-        Deletes the MSK cluster policy specified by the Amazon Resource Name (ARN) in
-        the request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster_policy)
-        """
-
     def delete_configuration(self, *, Arn: str) -> DeleteConfigurationResponseTypeDef:
         """
         Deletes an MSK Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_configuration)
         """
 
-    def delete_vpc_connection(self, *, Arn: str) -> DeleteVpcConnectionResponseTypeDef:
-        """
-        Deletes a MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_vpc_connection)
-        """
-
     def describe_cluster(self, *, ClusterArn: str) -> DescribeClusterResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster)
@@ -318,22 +275,14 @@
         """
         Returns a description of this revision of the configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_configuration_revision)
         """
 
-    def describe_vpc_connection(self, *, Arn: str) -> DescribeVpcConnectionResponseTypeDef:
-        """
-        Returns a description of this MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_vpc_connection)
-        """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -348,43 +297,24 @@
         """
         A list of brokers that a client application can use to bootstrap.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_bootstrap_brokers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_bootstrap_brokers)
         """
 
-    def get_cluster_policy(self, *, ClusterArn: str) -> GetClusterPolicyResponseTypeDef:
-        """
-        Get the MSK cluster policy specified by the Amazon Resource Name (ARN) in the
-        request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_cluster_policy)
-        """
-
     def get_compatible_kafka_versions(
         self, *, ClusterArn: str = ...
     ) -> GetCompatibleKafkaVersionsResponseTypeDef:
         """
         Gets the Apache Kafka versions to which you can update the MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_compatible_kafka_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_compatible_kafka_versions)
         """
 
-    def list_client_vpc_connections(
-        self, *, ClusterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListClientVpcConnectionsResponseTypeDef:
-        """
-        Returns a list of all the VPC connections in this Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_client_vpc_connections)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_client_vpc_connections)
-        """
-
     def list_cluster_operations(
         self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterOperationsResponseTypeDef:
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
@@ -471,55 +401,24 @@
         """
         Returns a list of the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_tags_for_resource)
         """
 
-    def list_vpc_connections(
-        self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVpcConnectionsResponseTypeDef:
-        """
-        Returns a list of all the VPC connections in this Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_vpc_connections)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_vpc_connections)
-        """
-
-    def put_cluster_policy(
-        self, *, ClusterArn: str, Policy: str, CurrentVersion: str = ...
-    ) -> PutClusterPolicyResponseTypeDef:
-        """
-        Creates or updates the MSK cluster policy specified by the cluster Amazon
-        Resource Name (ARN) in the request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.put_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#put_cluster_policy)
-        """
-
     def reboot_broker(
         self, *, BrokerIds: Sequence[str], ClusterArn: str
     ) -> RebootBrokerResponseTypeDef:
         """
         Reboots brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reboot_broker)
         """
 
-    def reject_client_vpc_connection(
-        self, *, VpcConnectionArn: str, ClusterArn: str = ...
-    ) -> Dict[str, Any]:
-        """
-        Returns empty response.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reject_client_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reject_client_vpc_connection)
-        """
-
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to the specified MSK resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.tag_resource)
@@ -665,23 +564,14 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_storage)
         """
 
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_client_vpc_connections"]
-    ) -> ListClientVpcConnectionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
 
@@ -737,16 +627,7 @@
     def get_paginator(
         self, operation_name: Literal["list_scram_secrets"]
     ) -> ListScramSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
-
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_vpc_connections"]
-    ) -> ListVpcConnectionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
-        """
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -17,67 +17,58 @@
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
-    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
-    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     LoggingInfoTypeDef,
     OpenMonitoringInfoTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedThroughputTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     ServerlessRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
@@ -207,62 +198,31 @@
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_configuration)
         """
-    def create_vpc_connection(
-        self,
-        *,
-        TargetClusterArn: str,
-        Authentication: str,
-        VpcId: str,
-        ClientSubnets: Sequence[str],
-        SecurityGroups: Sequence[str],
-        Tags: Mapping[str, str] = ...
-    ) -> CreateVpcConnectionResponseTypeDef:
-        """
-        Creates a new MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_vpc_connection)
-        """
     def delete_cluster(
         self, *, ClusterArn: str, CurrentVersion: str = ...
     ) -> DeleteClusterResponseTypeDef:
         """
         Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster)
         """
-    def delete_cluster_policy(self, *, ClusterArn: str) -> Dict[str, Any]:
-        """
-        Deletes the MSK cluster policy specified by the Amazon Resource Name (ARN) in
-        the request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster_policy)
-        """
     def delete_configuration(self, *, Arn: str) -> DeleteConfigurationResponseTypeDef:
         """
         Deletes an MSK Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_configuration)
         """
-    def delete_vpc_connection(self, *, Arn: str) -> DeleteVpcConnectionResponseTypeDef:
-        """
-        Deletes a MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_vpc_connection)
-        """
     def describe_cluster(self, *, ClusterArn: str) -> DescribeClusterResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster)
@@ -296,21 +256,14 @@
     ) -> DescribeConfigurationRevisionResponseTypeDef:
         """
         Returns a description of this revision of the configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_configuration_revision)
         """
-    def describe_vpc_connection(self, *, Arn: str) -> DescribeVpcConnectionResponseTypeDef:
-        """
-        Returns a description of this MSK VPC connection.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_vpc_connection)
-        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -323,40 +276,23 @@
     def get_bootstrap_brokers(self, *, ClusterArn: str) -> GetBootstrapBrokersResponseTypeDef:
         """
         A list of brokers that a client application can use to bootstrap.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_bootstrap_brokers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_bootstrap_brokers)
         """
-    def get_cluster_policy(self, *, ClusterArn: str) -> GetClusterPolicyResponseTypeDef:
-        """
-        Get the MSK cluster policy specified by the Amazon Resource Name (ARN) in the
-        request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_cluster_policy)
-        """
     def get_compatible_kafka_versions(
         self, *, ClusterArn: str = ...
     ) -> GetCompatibleKafkaVersionsResponseTypeDef:
         """
         Gets the Apache Kafka versions to which you can update the MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_compatible_kafka_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_compatible_kafka_versions)
         """
-    def list_client_vpc_connections(
-        self, *, ClusterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListClientVpcConnectionsResponseTypeDef:
-        """
-        Returns a list of all the VPC connections in this Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_client_vpc_connections)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_client_vpc_connections)
-        """
     def list_cluster_operations(
         self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterOperationsResponseTypeDef:
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
@@ -434,51 +370,23 @@
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_tags_for_resource)
         """
-    def list_vpc_connections(
-        self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVpcConnectionsResponseTypeDef:
-        """
-        Returns a list of all the VPC connections in this Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_vpc_connections)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_vpc_connections)
-        """
-    def put_cluster_policy(
-        self, *, ClusterArn: str, Policy: str, CurrentVersion: str = ...
-    ) -> PutClusterPolicyResponseTypeDef:
-        """
-        Creates or updates the MSK cluster policy specified by the cluster Amazon
-        Resource Name (ARN) in the request.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.put_cluster_policy)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#put_cluster_policy)
-        """
     def reboot_broker(
         self, *, BrokerIds: Sequence[str], ClusterArn: str
     ) -> RebootBrokerResponseTypeDef:
         """
         Reboots brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reboot_broker)
         """
-    def reject_client_vpc_connection(
-        self, *, VpcConnectionArn: str, ClusterArn: str = ...
-    ) -> Dict[str, Any]:
-        """
-        Returns empty response.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reject_client_vpc_connection)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reject_client_vpc_connection)
-        """
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to the specified MSK resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.tag_resource)
@@ -612,22 +520,14 @@
         Updates cluster broker volume size (or) sets cluster storage mode to TIERED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_storage)
         """
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_client_vpc_connections"]
-    ) -> ListClientVpcConnectionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
-        """
-    @overload
-    def get_paginator(
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
     @overload
@@ -676,15 +576,7 @@
     def get_paginator(
         self, operation_name: Literal["list_scram_secrets"]
     ) -> ListScramSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_vpc_connections"]
-    ) -> ListVpcConnectionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
-        """
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,45 +14,39 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BrokerAZDistributionType",
     "ClientBrokerType",
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
-    "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
-    "ListVpcConnectionsPaginatorName",
     "NodeTypeType",
     "StorageModeType",
-    "UserIdentityTypeType",
-    "VpcConnectionStateType",
     "KafkaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BrokerAZDistributionType = Literal["DEFAULT"]
 ClientBrokerType = Literal["PLAINTEXT", "TLS", "TLS_PLAINTEXT"]
 ClusterStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETING",
     "FAILED",
@@ -63,37 +57,24 @@
 ]
 ClusterTypeType = Literal["PROVISIONED", "SERVERLESS"]
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
-ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
-ListVpcConnectionsPaginatorName = Literal["list_vpc_connections"]
 NodeTypeType = Literal["BROKER"]
 StorageModeType = Literal["LOCAL", "TIERED"]
-UserIdentityTypeType = Literal["AWSACCOUNT", "AWSSERVICE"]
-VpcConnectionStateType = Literal[
-    "AVAILABLE",
-    "CREATING",
-    "DEACTIVATING",
-    "DELETING",
-    "FAILED",
-    "INACTIVE",
-    "REJECTED",
-    "REJECTING",
-]
 KafkaServiceName = Literal["kafka"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -141,15 +122,14 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -235,15 +215,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -254,15 +233,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -324,15 +302,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -414,20 +391,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -446,46 +421,40 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_client_vpc_connections",
     "list_cluster_operations",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
-    "list_vpc_connections",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,43 +14,41 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BrokerAZDistributionType",
     "ClientBrokerType",
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
-    "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
-    "ListVpcConnectionsPaginatorName",
     "NodeTypeType",
     "StorageModeType",
-    "UserIdentityTypeType",
-    "VpcConnectionStateType",
     "KafkaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 BrokerAZDistributionType = Literal["DEFAULT"]
 ClientBrokerType = Literal["PLAINTEXT", "TLS", "TLS_PLAINTEXT"]
 ClusterStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETING",
     "FAILED",
@@ -61,37 +59,24 @@
 ]
 ClusterTypeType = Literal["PROVISIONED", "SERVERLESS"]
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
-ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
-ListVpcConnectionsPaginatorName = Literal["list_vpc_connections"]
 NodeTypeType = Literal["BROKER"]
 StorageModeType = Literal["LOCAL", "TIERED"]
-UserIdentityTypeType = Literal["AWSACCOUNT", "AWSSERVICE"]
-VpcConnectionStateType = Literal[
-    "AVAILABLE",
-    "CREATING",
-    "DEACTIVATING",
-    "DELETING",
-    "FAILED",
-    "INACTIVE",
-    "REJECTED",
-    "REJECTING",
-]
 KafkaServiceName = Literal["kafka"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -139,15 +124,14 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -233,15 +217,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -252,15 +235,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -322,15 +304,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -412,20 +393,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -444,46 +423,40 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_client_vpc_connections",
     "list_cluster_operations",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
-    "list_vpc_connections",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,98 +6,75 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
-        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
-        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
-    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
-    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
-    "ListVpcConnectionsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
 
-class ListClientVpcConnectionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
-    """
-
-    def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
-        """
-
-
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
@@ -212,22 +189,7 @@
     def paginate(
         self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
-
-
-class ListVpcConnectionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
-    """
-
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
-        """
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -6,94 +6,72 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
-        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
-        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
-    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
-    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
-    "ListVpcConnectionsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-class ListClientVpcConnectionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
-    """
-
-    def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
-        """
-
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
@@ -201,21 +179,7 @@
     def paginate(
         self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
-
-class ListVpcConnectionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
-    """
-
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
-        """
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     StorageModeType,
-    UserIdentityTypeType,
-    VpcConnectionStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -47,87 +45,67 @@
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
-    "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
-    "CreateVpcConnectionRequestRequestTypeDef",
-    "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
-    "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeVpcConnectionRequestRequestTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
-    "GetClusterPolicyRequestRequestTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
-    "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersV2RequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
     "ListNodesRequestRequestTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVpcConnectionsRequestRequestTypeDef",
-    "VpcConnectionTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
-    "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "RejectClientVpcConnectionRequestRequestTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
-    "UserIdentityTypeDef",
-    "VpcConnectivityTlsTypeDef",
-    "VpcConnectivityIamTypeDef",
-    "VpcConnectivityScramTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
-    "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeleteConfigurationResponseTypeDef",
-    "DeleteVpcConnectionResponseTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
-    "DescribeVpcConnectionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBootstrapBrokersResponseTypeDef",
-    "GetClusterPolicyResponseTypeDef",
     "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConnectivityResponseTypeDef",
@@ -137,63 +115,55 @@
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
-    "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
+    "ConnectivityInfoTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
-    "VpcConnectionInfoTypeDef",
-    "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "UpdateConnectivityRequestRequestTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationTypeDef",
-    "VpcConnectivityClientAuthenticationTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "UpdateSecurityRequestRequestTypeDef",
-    "VpcConnectivityTypeDef",
-    "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
-    "UpdateConnectivityRequestRequestTypeDef",
+    "UpdateSecurityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
@@ -332,38 +302,14 @@
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-_RequiredClientVpcConnectionTypeDef = TypedDict(
-    "_RequiredClientVpcConnectionTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-_OptionalClientVpcConnectionTypeDef = TypedDict(
-    "_OptionalClientVpcConnectionTypeDef",
-    {
-        "Authentication": str,
-        "CreationTime": datetime,
-        "State": VpcConnectionStateType,
-        "Owner": str,
-    },
-    total=False,
-)
-
-
-class ClientVpcConnectionTypeDef(
-    _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
-):
-    pass
-
-
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -453,47 +399,14 @@
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcConnectionRequestRequestTypeDef",
-    {
-        "TargetClusterArn": str,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": Sequence[str],
-        "SecurityGroups": Sequence[str],
-    },
-)
-_OptionalCreateVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcConnectionRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateVpcConnectionRequestRequestTypeDef(
-    _RequiredCreateVpcConnectionRequestRequestTypeDef,
-    _OptionalCreateVpcConnectionRequestRequestTypeDef,
-):
-    pass
-
-
-DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
-    "DeleteClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-
 _RequiredDeleteClusterRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalDeleteClusterRequestRequestTypeDef = TypedDict(
@@ -514,21 +427,14 @@
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
-    "DeleteVpcConnectionRequestRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
@@ -557,21 +463,14 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
-DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
-    "DescribeVpcConnectionRequestRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
@@ -587,21 +486,14 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetClusterPolicyRequestRequestTypeDef = TypedDict(
-    "GetClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
@@ -643,24 +535,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
-    "ListClientVpcConnectionsRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -789,46 +671,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListVpcConnectionsRequestRequestTypeDef = TypedDict(
-    "ListVpcConnectionsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredVpcConnectionTypeDef = TypedDict(
-    "_RequiredVpcConnectionTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-    },
-)
-_OptionalVpcConnectionTypeDef = TypedDict(
-    "_OptionalVpcConnectionTypeDef",
-    {
-        "CreationTime": datetime,
-        "Authentication": str,
-        "VpcId": str,
-        "State": VpcConnectionStateType,
-    },
-    total=False,
-)
-
-
-class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
-    pass
-
-
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -847,66 +697,22 @@
         "Endpoints": List[str],
         "ZookeeperId": float,
         "ZookeeperVersion": str,
     },
     total=False,
 )
 
-_RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "Policy": str,
-    },
-)
-_OptionalPutClusterPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutClusterPolicyRequestRequestTypeDef",
-    {
-        "CurrentVersion": str,
-    },
-    total=False,
-)
-
-
-class PutClusterPolicyRequestRequestTypeDef(
-    _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
-):
-    pass
-
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
 
-_RequiredRejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredRejectClientVpcConnectionRequestRequestTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-_OptionalRejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalRejectClientVpcConnectionRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-    total=False,
-)
-
-
-class RejectClientVpcConnectionRequestRequestTypeDef(
-    _RequiredRejectClientVpcConnectionRequestRequestTypeDef,
-    _OptionalRejectClientVpcConnectionRequestRequestTypeDef,
-):
-    pass
-
-
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -983,47 +789,14 @@
 class UpdateConfigurationRequestRequestTypeDef(
     _RequiredUpdateConfigurationRequestRequestTypeDef,
     _OptionalUpdateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-UserIdentityTypeDef = TypedDict(
-    "UserIdentityTypeDef",
-    {
-        "Type": UserIdentityTypeType,
-        "PrincipalId": str,
-    },
-    total=False,
-)
-
-VpcConnectivityTlsTypeDef = TypedDict(
-    "VpcConnectivityTlsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-VpcConnectivityIamTypeDef = TypedDict(
-    "VpcConnectivityIamTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-VpcConnectivityScramTypeDef = TypedDict(
-    "VpcConnectivityScramTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterName": str,
         "State": ClusterStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1037,29 +810,14 @@
         "ClusterName": str,
         "State": ClusterStateType,
         "ClusterType": ClusterTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVpcConnectionResponseTypeDef = TypedDict(
-    "CreateVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "ClusterArn": str,
         "State": ClusterStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1070,51 +828,26 @@
     {
         "Arn": str,
         "State": ConfigurationStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteVpcConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeConfigurationRevisionResponseTypeDef = TypedDict(
     "DescribeConfigurationRevisionResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "Revision": int,
         "ServerProperties": bytes,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeVpcConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "Subnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1124,26 +857,14 @@
         "BootstrapBrokerString": str,
         "BootstrapBrokerStringTls": str,
         "BootstrapBrokerStringSaslScram": str,
         "BootstrapBrokerStringSaslIam": str,
         "BootstrapBrokerStringPublicTls": str,
         "BootstrapBrokerStringPublicSaslScram": str,
         "BootstrapBrokerStringPublicSaslIam": str,
-        "BootstrapBrokerStringVpcConnectivityTls": str,
-        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
-        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetClusterPolicyResponseTypeDef = TypedDict(
-    "GetClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScramSecretsResponseTypeDef = TypedDict(
     "ListScramSecretsResponseTypeDef",
     {
@@ -1157,22 +878,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutClusterPolicyResponseTypeDef = TypedDict(
-    "PutClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RebootBrokerResponseTypeDef = TypedDict(
     "RebootBrokerResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1351,23 +1064,14 @@
         "ClientVpcIpAddress": str,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "Endpoints": List[str],
     },
     total=False,
 )
 
-ListClientVpcConnectionsResponseTypeDef = TypedDict(
-    "ListClientVpcConnectionsResponseTypeDef",
-    {
-        "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
@@ -1467,14 +1171,22 @@
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConnectivityInfoTypeDef = TypedDict(
+    "ConnectivityInfoTypeDef",
+    {
+        "PublicAccess": PublicAccessTypeDef,
+    },
+    total=False,
+)
+
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
@@ -1493,23 +1205,14 @@
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
@@ -1625,31 +1328,14 @@
 class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
     _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
     _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
 ):
     pass
 
 
-ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVpcConnectionsResponseTypeDef = TypedDict(
-    "ListVpcConnectionsResponseTypeDef",
-    {
-        "VpcConnections": List[VpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1669,34 +1355,14 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
-VpcConnectionInfoTypeDef = TypedDict(
-    "VpcConnectionInfoTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "Owner": str,
-        "UserIdentity": UserIdentityTypeDef,
-        "CreationTime": datetime,
-    },
-    total=False,
-)
-
-VpcConnectivitySaslTypeDef = TypedDict(
-    "VpcConnectivitySaslTypeDef",
-    {
-        "Scram": VpcConnectivityScramTypeDef,
-        "Iam": VpcConnectivityIamTypeDef,
-    },
-    total=False,
-)
-
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1735,14 +1401,23 @@
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateConnectivityRequestRequestTypeDef = TypedDict(
+    "UpdateConnectivityRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "CurrentVersion": str,
+    },
+)
+
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
@@ -1767,23 +1442,39 @@
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-VpcConnectivityClientAuthenticationTypeDef = TypedDict(
-    "VpcConnectivityClientAuthenticationTypeDef",
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
+    {
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
     {
-        "Sasl": VpcConnectivitySaslTypeDef,
-        "Tls": VpcConnectivityTlsTypeDef,
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
     },
     total=False,
 )
 
+
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
+
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1849,80 +1540,14 @@
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-    },
-)
-_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSecurityRequestRequestTypeDef(
-    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
-):
-    pass
-
-
-VpcConnectivityTypeDef = TypedDict(
-    "VpcConnectivityTypeDef",
-    {
-        "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
-    },
-    total=False,
-)
-
-ConnectivityInfoTypeDef = TypedDict(
-    "ConnectivityInfoTypeDef",
-    {
-        "PublicAccess": PublicAccessTypeDef,
-        "VpcConnectivity": VpcConnectivityTypeDef,
-    },
-    total=False,
-)
-
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
-    {
-        "ClientSubnets": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": Sequence[str],
-    },
-    total=False,
-)
-
-
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
-):
-    pass
-
-
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -1934,22 +1559,36 @@
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-UpdateConnectivityRequestRequestTypeDef = TypedDict(
-    "UpdateConnectivityRequestRequestTypeDef",
+_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
+_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSecurityRequestRequestTypeDef(
+    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
+):
+    pass
+
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationTypeDef,
@@ -2071,15 +1710,14 @@
         "ErrorInfo": ErrorInfoTypeDef,
         "OperationArn": str,
         "OperationState": str,
         "OperationSteps": List[ClusterOperationStepTypeDef],
         "OperationType": str,
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     StorageModeType,
-    UserIdentityTypeType,
-    VpcConnectionStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -46,87 +44,67 @@
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
-    "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
-    "CreateVpcConnectionRequestRequestTypeDef",
-    "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
-    "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeVpcConnectionRequestRequestTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
-    "GetClusterPolicyRequestRequestTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
-    "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersV2RequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
     "ListNodesRequestRequestTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVpcConnectionsRequestRequestTypeDef",
-    "VpcConnectionTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
-    "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "RejectClientVpcConnectionRequestRequestTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
-    "UserIdentityTypeDef",
-    "VpcConnectivityTlsTypeDef",
-    "VpcConnectivityIamTypeDef",
-    "VpcConnectivityScramTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
-    "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeleteConfigurationResponseTypeDef",
-    "DeleteVpcConnectionResponseTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
-    "DescribeVpcConnectionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBootstrapBrokersResponseTypeDef",
-    "GetClusterPolicyResponseTypeDef",
     "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConnectivityResponseTypeDef",
@@ -136,63 +114,55 @@
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
-    "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
+    "ConnectivityInfoTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
-    "VpcConnectionInfoTypeDef",
-    "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "UpdateConnectivityRequestRequestTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationTypeDef",
-    "VpcConnectivityClientAuthenticationTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "UpdateSecurityRequestRequestTypeDef",
-    "VpcConnectivityTypeDef",
-    "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
-    "UpdateConnectivityRequestRequestTypeDef",
+    "UpdateSecurityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
@@ -325,36 +295,14 @@
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-_RequiredClientVpcConnectionTypeDef = TypedDict(
-    "_RequiredClientVpcConnectionTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-_OptionalClientVpcConnectionTypeDef = TypedDict(
-    "_OptionalClientVpcConnectionTypeDef",
-    {
-        "Authentication": str,
-        "CreationTime": datetime,
-        "State": VpcConnectionStateType,
-        "Owner": str,
-    },
-    total=False,
-)
-
-class ClientVpcConnectionTypeDef(
-    _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
-):
-    pass
-
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -440,45 +388,14 @@
 
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcConnectionRequestRequestTypeDef",
-    {
-        "TargetClusterArn": str,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": Sequence[str],
-        "SecurityGroups": Sequence[str],
-    },
-)
-_OptionalCreateVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcConnectionRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateVpcConnectionRequestRequestTypeDef(
-    _RequiredCreateVpcConnectionRequestRequestTypeDef,
-    _OptionalCreateVpcConnectionRequestRequestTypeDef,
-):
-    pass
-
-DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
-    "DeleteClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-
 _RequiredDeleteClusterRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalDeleteClusterRequestRequestTypeDef = TypedDict(
@@ -497,21 +414,14 @@
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
-    "DeleteVpcConnectionRequestRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
@@ -540,21 +450,14 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
-DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
-    "DescribeVpcConnectionRequestRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
@@ -570,21 +473,14 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetClusterPolicyRequestRequestTypeDef = TypedDict(
-    "GetClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
@@ -626,24 +522,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
-    "ListClientVpcConnectionsRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -764,44 +650,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListVpcConnectionsRequestRequestTypeDef = TypedDict(
-    "ListVpcConnectionsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredVpcConnectionTypeDef = TypedDict(
-    "_RequiredVpcConnectionTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-    },
-)
-_OptionalVpcConnectionTypeDef = TypedDict(
-    "_OptionalVpcConnectionTypeDef",
-    {
-        "CreationTime": datetime,
-        "Authentication": str,
-        "VpcId": str,
-        "State": VpcConnectionStateType,
-    },
-    total=False,
-)
-
-class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
-    pass
-
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -820,62 +676,22 @@
         "Endpoints": List[str],
         "ZookeeperId": float,
         "ZookeeperVersion": str,
     },
     total=False,
 )
 
-_RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutClusterPolicyRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "Policy": str,
-    },
-)
-_OptionalPutClusterPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutClusterPolicyRequestRequestTypeDef",
-    {
-        "CurrentVersion": str,
-    },
-    total=False,
-)
-
-class PutClusterPolicyRequestRequestTypeDef(
-    _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
-):
-    pass
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
 
-_RequiredRejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredRejectClientVpcConnectionRequestRequestTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-_OptionalRejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalRejectClientVpcConnectionRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-    },
-    total=False,
-)
-
-class RejectClientVpcConnectionRequestRequestTypeDef(
-    _RequiredRejectClientVpcConnectionRequestRequestTypeDef,
-    _OptionalRejectClientVpcConnectionRequestRequestTypeDef,
-):
-    pass
-
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -948,47 +764,14 @@
 
 class UpdateConfigurationRequestRequestTypeDef(
     _RequiredUpdateConfigurationRequestRequestTypeDef,
     _OptionalUpdateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-UserIdentityTypeDef = TypedDict(
-    "UserIdentityTypeDef",
-    {
-        "Type": UserIdentityTypeType,
-        "PrincipalId": str,
-    },
-    total=False,
-)
-
-VpcConnectivityTlsTypeDef = TypedDict(
-    "VpcConnectivityTlsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-VpcConnectivityIamTypeDef = TypedDict(
-    "VpcConnectivityIamTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-VpcConnectivityScramTypeDef = TypedDict(
-    "VpcConnectivityScramTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterName": str,
         "State": ClusterStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1002,29 +785,14 @@
         "ClusterName": str,
         "State": ClusterStateType,
         "ClusterType": ClusterTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVpcConnectionResponseTypeDef = TypedDict(
-    "CreateVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "ClusterArn": str,
         "State": ClusterStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1035,51 +803,26 @@
     {
         "Arn": str,
         "State": ConfigurationStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteVpcConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeConfigurationRevisionResponseTypeDef = TypedDict(
     "DescribeConfigurationRevisionResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "Revision": int,
         "ServerProperties": bytes,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeVpcConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "Subnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1089,26 +832,14 @@
         "BootstrapBrokerString": str,
         "BootstrapBrokerStringTls": str,
         "BootstrapBrokerStringSaslScram": str,
         "BootstrapBrokerStringSaslIam": str,
         "BootstrapBrokerStringPublicTls": str,
         "BootstrapBrokerStringPublicSaslScram": str,
         "BootstrapBrokerStringPublicSaslIam": str,
-        "BootstrapBrokerStringVpcConnectivityTls": str,
-        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
-        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetClusterPolicyResponseTypeDef = TypedDict(
-    "GetClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScramSecretsResponseTypeDef = TypedDict(
     "ListScramSecretsResponseTypeDef",
     {
@@ -1122,22 +853,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutClusterPolicyResponseTypeDef = TypedDict(
-    "PutClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RebootBrokerResponseTypeDef = TypedDict(
     "RebootBrokerResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1312,23 +1035,14 @@
         "ClientVpcIpAddress": str,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "Endpoints": List[str],
     },
     total=False,
 )
 
-ListClientVpcConnectionsResponseTypeDef = TypedDict(
-    "ListClientVpcConnectionsResponseTypeDef",
-    {
-        "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
@@ -1426,14 +1140,22 @@
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConnectivityInfoTypeDef = TypedDict(
+    "ConnectivityInfoTypeDef",
+    {
+        "PublicAccess": PublicAccessTypeDef,
+    },
+    total=False,
+)
+
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
@@ -1452,23 +1174,14 @@
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
@@ -1576,31 +1289,14 @@
 
 class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
     _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
     _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
 ):
     pass
 
-ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVpcConnectionsResponseTypeDef = TypedDict(
-    "ListVpcConnectionsResponseTypeDef",
-    {
-        "VpcConnections": List[VpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1620,34 +1316,14 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
-VpcConnectionInfoTypeDef = TypedDict(
-    "VpcConnectionInfoTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "Owner": str,
-        "UserIdentity": UserIdentityTypeDef,
-        "CreationTime": datetime,
-    },
-    total=False,
-)
-
-VpcConnectivitySaslTypeDef = TypedDict(
-    "VpcConnectivitySaslTypeDef",
-    {
-        "Scram": VpcConnectivityScramTypeDef,
-        "Iam": VpcConnectivityIamTypeDef,
-    },
-    total=False,
-)
-
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1686,14 +1362,23 @@
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateConnectivityRequestRequestTypeDef = TypedDict(
+    "UpdateConnectivityRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "CurrentVersion": str,
+    },
+)
+
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
@@ -1718,23 +1403,37 @@
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-VpcConnectivityClientAuthenticationTypeDef = TypedDict(
-    "VpcConnectivityClientAuthenticationTypeDef",
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
     {
-        "Sasl": VpcConnectivitySaslTypeDef,
-        "Tls": VpcConnectivityTlsTypeDef,
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
+    {
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
     },
     total=False,
 )
 
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1794,76 +1493,14 @@
 )
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-    },
-)
-_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSecurityRequestRequestTypeDef(
-    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
-):
-    pass
-
-VpcConnectivityTypeDef = TypedDict(
-    "VpcConnectivityTypeDef",
-    {
-        "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
-    },
-    total=False,
-)
-
-ConnectivityInfoTypeDef = TypedDict(
-    "ConnectivityInfoTypeDef",
-    {
-        "PublicAccess": PublicAccessTypeDef,
-        "VpcConnectivity": VpcConnectivityTypeDef,
-    },
-    total=False,
-)
-
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
-    {
-        "ClientSubnets": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": Sequence[str],
-    },
-    total=False,
-)
-
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
-):
-    pass
-
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -1875,22 +1512,34 @@
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-UpdateConnectivityRequestRequestTypeDef = TypedDict(
-    "UpdateConnectivityRequestRequestTypeDef",
+_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
+_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSecurityRequestRequestTypeDef(
+    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
+):
+    pass
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationTypeDef,
@@ -2006,15 +1655,14 @@
         "ErrorInfo": ErrorInfoTypeDef,
         "OperationArn": str,
         "OperationState": str,
         "OperationSteps": List[ClusterOperationStepTypeDef],
         "OperationType": str,
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.26.60/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kafka
-Version: 1.26.122
-Summary: Type annotations for boto3.Kafka 1.26.122 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,33 +247,28 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
-    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
-    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
-list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
-    "list_client_vpc_connections"
-)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -314,17 +277,14 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
-list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
-    "list_vpc_connections"
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -335,28 +295,24 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
-    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
-    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
-    UserIdentityTypeType,
-    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -381,87 +337,67 @@
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
-    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
     CreateConfigurationRequestRequestTypeDef,
-    CreateVpcConnectionRequestRequestTypeDef,
-    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeVpcConnectionRequestRequestTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetClusterPolicyRequestRequestTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     PaginatorConfigTypeDef,
-    ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersV2RequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
     ListNodesRequestRequestTypeDef,
     ListScramSecretsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVpcConnectionsRequestRequestTypeDef,
-    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PutClusterPolicyRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RejectClientVpcConnectionRequestRequestTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBootstrapBrokersResponseTypeDef,
-    GetClusterPolicyResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
@@ -471,63 +407,55 @@
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
-    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListNodesRequestListNodesPaginateTypeDef,
     ListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
-    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
-    VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityTypeDef,
-    ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
+    UpdateSecurityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -547,42 +475,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-kafka-1.26.122/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.26.122/setup.py` & `mypy-boto3-kafka-1.26.60/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-kafka.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.26.122",
+    version="1.26.60",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.26.122 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

