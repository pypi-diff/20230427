# Comparing `tmp/tomcru-0.1.2.tar.gz` & `tmp/tomcru-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru-0.1.2.tar", max compression
+gzip compressed data, was "tomcru-0.1.3.tar", max compression
```

## Comparing `tomcru-0.1.2.tar` & `tomcru-0.1.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.1.2/LICENSE
--rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.1.2/README.md
--rw-r--r--   0        0        0      632 2023-04-27 01:58:27.516918 tomcru-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      561 2023-04-23 17:44:15.255606 tomcru-0.1.2/tomcru/__init__.py
--rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.1.2/tomcru/appbuilders/envmapping.py
--rw-r--r--   0        0        0     1390 2023-04-26 00:29:37.772660 tomcru-0.1.2/tomcru/appbuilders/faas/InjectableAppBase.py
--rw-r--r--   0        0        0     2952 2023-04-17 19:28:58.109580 tomcru-0.1.2/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/appbuilders/faas/sam_app/__init__.py
--rw-r--r--   0        0        0      846 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
--rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/appbuilders/faas/static_app/__init__.py
--rw-r--r--   0        0        0    10279 2023-04-27 00:36:09.185520 tomcru-0.1.2/tomcru/cfgparsers/BaseCfgParser.py
--rw-r--r--   0        0        0     3076 2023-04-26 23:45:03.858775 tomcru-0.1.2/tomcru/cfgparsers/EnvParser.py
--rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.1.2/tomcru/cfgparsers/MergeCfgParser.py
--rw-r--r--   0        0        0     4746 2023-04-27 01:54:56.413640 tomcru-0.1.2/tomcru/cfgparsers/SwaggerCfgParser.py
--rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.1.2/tomcru/cfgparsers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.1.2/tomcru/core/__init__.py
--rw-r--r--   0        0        0     3524 2023-04-19 21:58:50.454140 tomcru-0.1.2/tomcru/core/cfg/api.py
--rw-r--r--   0        0        0     1284 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/core/cfg/authorizers.py
--rw-r--r--   0        0        0     3605 2023-04-23 18:19:12.194283 tomcru-0.1.2/tomcru/core/cfg/integrations.py
--rw-r--r--   0        0        0     2081 2023-04-26 23:45:03.854775 tomcru-0.1.2/tomcru/core/cfg/proj.py
--rw-r--r--   0        0        0      563 2023-04-27 01:48:19.835005 tomcru-0.1.2/tomcru/core/modloader.py
--rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.1.2/tomcru/core/obj_store.py
--rw-r--r--   0        0        0     2948 2023-04-26 00:29:37.776660 tomcru-0.1.2/tomcru/core/project.py
--rw-r--r--   0        0        0     2252 2023-04-27 01:48:39.354937 tomcru-0.1.2/tomcru/core/servmgr.py
--rw-r--r--   0        0        0     3802 2023-04-25 11:22:05.331979 tomcru-0.1.2/tomcru/core/utils/MyMetaLoader.py
--rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.1.2/tomcru/core/utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.1.2/tomcru/core/utils/toml_custom.py
--rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.1.2/tomcru/core/utils/yaml_custom.py
--rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.1.2/tomcru/services/ServiceBase.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/__init__.py
--rw-r--r--   0        0        0     4838 2023-04-27 01:49:50.786690 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
--rw-r--r--   0        0        0     1511 2023-04-21 15:39:22.023408 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/apigw_hosted_utils.py
--rw-r--r--   0        0        0      851 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     2718 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     3203 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
--rw-r--r--   0        0        0      727 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
--rw-r--r--   0        0        0      287 2023-04-23 18:04:30.986605 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
--rw-r--r--   0        0        0     3663 2023-04-27 01:48:52.550891 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
--rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
--rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
--rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
--rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
--rw-r--r--   0        0        0     3872 2023-04-27 01:49:37.482736 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
--rw-r--r--   0        0        0     1918 2023-04-23 18:23:35.039805 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
--rw-r--r--   0        0        0     2613 2023-04-27 01:49:29.598764 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
--rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
--rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
--rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
--rw-r--r--   0        0        0     3070 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-18 00:10:51.017128 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
--rw-r--r--   0        0        0     3312 2023-04-19 01:27:07.459839 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
--rw-r--r--   0        0        0     3528 2023-04-18 00:10:51.013128 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
--rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
--rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
--rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.1.2/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
--rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.1.2/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-25 19:34:10.268617 tomcru-0.1.2/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/boto3_b/__init__.py
--rw-r--r--   0        0        0      802 2023-04-25 20:07:24.831399 tomcru-0.1.2/tomcru/services/aws/hosted/boto3_b/boto3.py
--rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/__init__.py
--rw-r--r--   0        0        0      289 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbSqlalchemyAdapter.py
--rw-r--r--   0        0        0     8044 2023-04-21 01:21:56.198102 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py
--rw-r--r--   0        0        0      697 2023-04-25 20:08:42.820346 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
--rw-r--r--   0        0        0     1133 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
--rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
--rw-r--r--   0        0        0     4076 2023-04-25 22:35:24.903552 tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
--rw-r--r--   0        0        0      779 2023-04-21 01:02:40.764855 tomcru-0.1.2/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py
--rw-r--r--   0        0        0     3363 2023-04-27 00:08:26.646256 tomcru-0.1.2/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/hosted/lambda_b/__init__.py
--rw-r--r--   0        0        0     2539 2023-04-27 00:16:39.812717 tomcru-0.1.2/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
--rw-r--r--   0        0        0      529 2023-04-25 22:30:36.985428 tomcru-0.1.2/tomcru/services/aws/hosted/s3_b/S3Service.py
--rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.1.2/tomcru/services/aws/hosted/s3_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/onpremise/__init__.py
--rw-r--r--   0        0        0     4097 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
--rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/onpremise/model_checker/__init__.py
--rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
--rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/onpremise/s3_static/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/SamTplBuilder.py
--rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/core.yaml
--rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/httpapi.yaml
--rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/integ_normal.yaml
--rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/integ_ws.yaml
--rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/lambda.yaml
--rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/layer.yaml
--rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/template.yaml
--rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/_junk/wsapi.yaml
--rw-r--r--   0        0        0     2120 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/lambda_b/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/params_b/ParametersBuilder.py
--rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/params_b/__init__.py
--rw-r--r--   0        0        0     2843 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
--rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-17 19:28:58.101580 tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
--rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
--rw-r--r--   0        0        0      861 2023-04-17 19:29:32.681461 tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
--rw-r--r--   0        0        0     2326 2023-04-17 18:29:36.252599 tomcru-0.1.2/tomcru/services/general/eme2swagger/Eme2Swagger.py
--rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.1.2/tomcru/services/general/eme2swagger/__init__.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.1.3/LICENSE
+-rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.1.3/README.md
+-rw-r--r--   0        0        0      632 2023-04-27 10:29:13.203529 tomcru-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      561 2023-04-23 17:44:15.255606 tomcru-0.1.3/tomcru/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.1.3/tomcru/appbuilders/envmapping.py
+-rw-r--r--   0        0        0     1416 2023-04-27 10:26:11.129112 tomcru-0.1.3/tomcru/appbuilders/faas/InjectableAppBase.py
+-rw-r--r--   0        0        0     2954 2023-04-27 10:14:15.984656 tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.1.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
+-rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/appbuilders/faas/static_app/__init__.py
+-rw-r--r--   0        0        0    10214 2023-04-27 10:27:22.520399 tomcru-0.1.3/tomcru/cfgparsers/BaseCfgParser.py
+-rw-r--r--   0        0        0     3076 2023-04-26 23:45:03.858775 tomcru-0.1.3/tomcru/cfgparsers/EnvParser.py
+-rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.1.3/tomcru/cfgparsers/MergeCfgParser.py
+-rw-r--r--   0        0        0     4746 2023-04-27 01:54:56.413640 tomcru-0.1.3/tomcru/cfgparsers/SwaggerCfgParser.py
+-rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.1.3/tomcru/cfgparsers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.1.3/tomcru/core/__init__.py
+-rw-r--r--   0        0        0     3524 2023-04-19 21:58:50.454140 tomcru-0.1.3/tomcru/core/cfg/api.py
+-rw-r--r--   0        0        0     1284 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/core/cfg/authorizers.py
+-rw-r--r--   0        0        0     3605 2023-04-23 18:19:12.194283 tomcru-0.1.3/tomcru/core/cfg/integrations.py
+-rw-r--r--   0        0        0     2081 2023-04-26 23:45:03.854775 tomcru-0.1.3/tomcru/core/cfg/proj.py
+-rw-r--r--   0        0        0      563 2023-04-27 01:48:19.835005 tomcru-0.1.3/tomcru/core/modloader.py
+-rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.1.3/tomcru/core/obj_store.py
+-rw-r--r--   0        0        0     2948 2023-04-27 10:13:31.952519 tomcru-0.1.3/tomcru/core/project.py
+-rw-r--r--   0        0        0     2252 2023-04-27 01:48:39.354937 tomcru-0.1.3/tomcru/core/servmgr.py
+-rw-r--r--   0        0        0     3802 2023-04-25 11:22:05.331979 tomcru-0.1.3/tomcru/core/utils/MyMetaLoader.py
+-rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.1.3/tomcru/core/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.1.3/tomcru/core/utils/toml_custom.py
+-rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/core/utils/yaml_custom.py
+-rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.1.3/tomcru/services/ServiceBase.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/__init__.py
+-rw-r--r--   0        0        0     4838 2023-04-27 01:49:50.786690 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
+-rw-r--r--   0        0        0     1511 2023-04-21 15:39:22.023408 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/apigw_hosted_utils.py
+-rw-r--r--   0        0        0      851 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     2718 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     3203 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
+-rw-r--r--   0        0        0      727 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
+-rw-r--r--   0        0        0      287 2023-04-23 18:04:30.986605 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
+-rw-r--r--   0        0        0     3663 2023-04-27 01:48:52.550891 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
+-rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
+-rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
+-rw-r--r--   0        0        0     3872 2023-04-27 01:49:37.482736 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0     1918 2023-04-23 18:23:35.039805 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
+-rw-r--r--   0        0        0     2613 2023-04-27 01:49:29.598764 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
+-rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
+-rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
+-rw-r--r--   0        0        0     3070 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-18 00:10:51.017128 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
+-rw-r--r--   0        0        0     3312 2023-04-19 01:27:07.459839 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
+-rw-r--r--   0        0        0     3528 2023-04-18 00:10:51.013128 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
+-rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
+-rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
+-rw-r--r--   0        0        0     1272 2023-04-25 19:34:10.268617 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/__init__.py
+-rw-r--r--   0        0        0      802 2023-04-25 20:07:24.831399 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/boto3.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbSqlalchemyAdapter.py
+-rw-r--r--   0        0        0     8044 2023-04-21 01:21:56.198102 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py
+-rw-r--r--   0        0        0      697 2023-04-27 10:20:48.798424 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
+-rw-r--r--   0        0        0     1133 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
+-rw-r--r--   0        0        0     4076 2023-04-25 22:35:24.903552 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
+-rw-r--r--   0        0        0      779 2023-04-21 01:02:40.764855 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py
+-rw-r--r--   0        0        0     3409 2023-04-27 10:26:11.121112 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/__init__.py
+-rw-r--r--   0        0        0     2553 2023-04-27 10:27:22.512399 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
+-rw-r--r--   0        0        0      529 2023-04-25 22:30:36.985428 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3Service.py
+-rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/__init__.py
+-rw-r--r--   0        0        0     4097 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
+-rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/__init__.py
+-rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
+-rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py
+-rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/core.yaml
+-rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/httpapi.yaml
+-rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_normal.yaml
+-rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_ws.yaml
+-rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/lambda.yaml
+-rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/layer.yaml
+-rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/template.yaml
+-rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/wsapi.yaml
+-rw-r--r--   0        0        0     2120 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/__init__.py
+-rw-r--r--   0        0        0     1363 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/params_b/__init__.py
+-rw-r--r--   0        0        0     2843 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
+-rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/__init__.py
+-rw-r--r--   0        0        0     1773 2023-04-17 19:28:58.101580 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
+-rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
+-rw-r--r--   0        0        0      861 2023-04-17 19:29:32.681461 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
+-rw-r--r--   0        0        0     2326 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/services/general/eme2swagger/Eme2Swagger.py
+-rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/services/general/eme2swagger/__init__.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.1.3/PKG-INFO
```

### Comparing `tomcru-0.1.2/LICENSE` & `tomcru-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/pyproject.toml` & `tomcru-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomcru"
-version = "0.1.2"
+version = "0.1.3"
 description = "Serverless app framework"
 authors = ["Rajmund Csombordi <rajmund.csombordi@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "tomcru"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tomcru-0.1.2/tomcru/__init__.py` & `tomcru-0.1.3/tomcru/__init__.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/appbuilders/envmapping.py` & `tomcru-0.1.3/tomcru/appbuilders/envmapping.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/appbuilders/faas/InjectableAppBase.py` & `tomcru-0.1.3/tomcru/appbuilders/faas/InjectableAppBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,32 @@
         self.p = proj
         self.env = env
         self.cfg = cfg
 
         self.inited = False
 
     def __enter__(self):
+        import traceback
         if not self.inited:
             self.p.srvmgr.load_services(self.env)
 
         for serv_id, service in self.p.srvmgr:
             if hasattr(service, 'inject_dependencies'):
                 service.inject_dependencies()
 
         if not self.inited:
+            self.inited = True
+
             for serv_id, service in sorted(self.p.srvmgr, key=lambda s: s[1].INIT_PRIORITY):
                 if hasattr(service, 'init'):
                     # todo: debug
                     print(f"Initializing service {serv_id}[ENV={self.env.env}]")
                     service.init()
                 else:
                     print(f"Skipping init on {serv_id}[ENV={self.env.env}]")
-            self.inited = True
 
         return self
 
     def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
         for serv_id, service in self.p.srvmgr:
             if hasattr(service, 'deject_dependencies'):
                 service.deject_dependencies()
```

### Comparing `tomcru-0.1.2/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py` & `tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.cfg = project.cfg
         self.apis = []
         #self.opts =
 
         self.param_builder = project.serv('aws:sam:params_b')
 
     def build_app(self, env):
-        self.p.env = env
+        # self.p.env = env
         lambda_builder = self.p.serv('aws:sam:lambda_b')
 
         sam_tpl: dict = self.build_app_stack(env)
 
         # buidl globals
         sam_tpl['Globals']['Function'] = lambda_builder.build_lambda_globals()
```

### Comparing `tomcru-0.1.2/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py` & `tomcru-0.1.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def get_object(self, srv, name=None):
         if name is None:
             srv, name = srv.split(':')
         objs = self.p.serv('aws:onpremise:obj_store')
         return objs.get(srv, name)
 
     def build_app(self, env):
-        self.p.env = env
+        # self.p.env = env
         builder = self.p.serv(self.api2builder['s3app'])
 
         return builder.build_app(env)
 
     def __enter__(self):
         return self
```

### Comparing `tomcru-0.1.2/tomcru/cfgparsers/BaseCfgParser.py` & `tomcru-0.1.3/tomcru/cfgparsers/BaseCfgParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
                     # handled by swagger cfg parser
                     swaggers.append(filepath)
                     continue
                 elif file.endswith('.toml'):
                     cfg = toml.load(filepath)
                 elif file.endswith('.yaml') or file.endswith('yml'):
                     cfg = yaml.load(filepath)
-                    print(123123, '!!!! yaml file !!!', cfg)
                 elif file.endswith('.json'):
                     with open(filepath) as fh:
                         cfg = json.load(fh)
                 else:
                     raise NotImplementedError(filepath)
 
                 if cfg:
@@ -107,15 +106,15 @@
         for api_name, cfg in apicfg.items():
             _api_type = cfg.get('type', 'http')
             cfg = {**cfg_all_, **cfg}
 
             if _api_type == 'rest':
                 raise NotImplementedError("HTTPv1 not supported")
 
-            print(f"Processing api: {api_name}")
+            #print(f"Parsing api: {api_name}")
 
             #cfg_api_ = self.cfg.apis.setdefault(api_name, TomcruApiDescriptor(api_name, _api_type))
             cfg_api_ = self.cfg.apis[api_name] = TomcruApiDescriptor(api_name, _api_type)
 
             # map ini to tomcru descriptor
             cfg_api_.swagger_enabled = cfg.get('swagger_enabled', False)
             cfg_api_.swagger_ui = cfg.get('swagger_ui', False)
@@ -144,15 +143,15 @@
         # _api_type = integration
         #
         cfg_api_ = self.cfg.apis[api_name] #.setdefault(api_name, TomcruApiDescriptor(api_name, _api_type))
 
         if not cfg_api_.enabled:
             return
 
-        print(f"Processing routes: {api_name}.{subkey}")
+        #print(f"Parsing routes: {api_name}.{subkey}")
         for endpoint, integ_opts in routes.items():
             # if endpoint.startswith('#'):
             #     # ignore comments
             #     continue
 
             # todo: maybe we want integ options to be dict instead of a list?
             if isinstance(integ_opts, dict):
```

### Comparing `tomcru-0.1.2/tomcru/cfgparsers/EnvParser.py` & `tomcru-0.1.3/tomcru/cfgparsers/EnvParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/cfgparsers/MergeCfgParser.py` & `tomcru-0.1.3/tomcru/cfgparsers/MergeCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/cfgparsers/SwaggerCfgParser.py` & `tomcru-0.1.3/tomcru/cfgparsers/SwaggerCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/cfg/api.py` & `tomcru-0.1.3/tomcru/core/cfg/api.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/cfg/authorizers.py` & `tomcru-0.1.3/tomcru/core/cfg/authorizers.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/cfg/integrations.py` & `tomcru-0.1.3/tomcru/core/cfg/integrations.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/cfg/proj.py` & `tomcru-0.1.3/tomcru/core/cfg/proj.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/modloader.py` & `tomcru-0.1.3/tomcru/core/modloader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/obj_store.py` & `tomcru-0.1.3/tomcru/core/obj_store.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/project.py` & `tomcru-0.1.3/tomcru/core/project.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/servmgr.py` & `tomcru-0.1.3/tomcru/core/servmgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/utils/MyMetaLoader.py` & `tomcru-0.1.3/tomcru/core/utils/MyMetaLoader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/utils/toml_custom.py` & `tomcru-0.1.3/tomcru/core/utils/toml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/core/utils/yaml_custom.py` & `tomcru-0.1.3/tomcru/core/utils/yaml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/ServiceBase.py` & `tomcru-0.1.3/tomcru/services/ServiceBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/apigw_hosted_utils.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/apigw_hosted_utils.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/boto3_b/boto3.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/boto3.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         _ctx_orig = dict(sys.modules)
 
         if not os.path.exists(_lambd_path) or not os.path.exists(os.path.join(_lambd_path, 'app.py')):
             raise IOError("Lambda path does not exists: " + _lambd_path+'/app.py')
 
         # load lambda function
         sys.path.append(_lambd_path)
-        #module = import_module(f"lambdas.{group}.{lamb}.app")
-        module = import_module(f"app")
+        sys.path.append(self.env.app_path)
+        module = import_module(f"lambdas.{group}.{lamb}.app")
+        sys.path.remove(self.env.app_path)
         sys.path.remove(_lambd_path)
 
         # restore loaded modules
         sys.modules.clear()
         sys.modules.update(_ctx_orig)
 
         fn = module.handler
```

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         # todo: apply meta tags & callback
 
     def put_object(self, Body: bytes | BinaryIO, Bucket, Key):
         _path = self.buckets[Bucket]['path']
 
         if isinstance(Body, bytes):
-            print("kuki")
+            raise NotImplementedError()
         else:
             with open(_path, 'b') as fh:
                 shutil.copyfileobj(Body, fh)
                 #fh.write(Body.read())
 
     def download_file(self, Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
         from_path = self._get_path(Bucket, Key)
```

### Comparing `tomcru-0.1.2/tomcru/services/aws/hosted/s3_b/S3Service.py` & `tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3Service.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py` & `tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/SamTplBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/core.yaml` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/core.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/httpapi.yaml` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/httpapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/integ_ws.yaml` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_ws.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/template.yaml` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/template.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/_junk/wsapi.yaml` & `tomcru-0.1.3/tomcru/services/aws/sam/_junk/wsapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/params_b/ParametersBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py` & `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py` & `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/tomcru/services/general/eme2swagger/Eme2Swagger.py` & `tomcru-0.1.3/tomcru/services/general/eme2swagger/Eme2Swagger.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.2/PKG-INFO` & `tomcru-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru
-Version: 0.1.2
+Version: 0.1.3
 Summary: Serverless app framework
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

