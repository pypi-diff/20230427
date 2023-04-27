# Comparing `tmp/domolibrary-0.1.7.tar.gz` & `tmp/domolibrary-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.7.tar", last modified: Wed Apr 26 18:27:21 2023, max compression
+gzip compressed data, was "domolibrary-0.1.8.tar", last modified: Wed Apr 26 19:37:21 2023, max compression
```

## Comparing `domolibrary-0.1.7.tar` & `domolibrary-0.1.8.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.131693 domolibrary-0.1.7/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.111693 domolibrary-0.1.7/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.7/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.111693 domolibrary-0.1.7/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.115693 domolibrary-0.1.7/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.7/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.7/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.7/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.7/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.7/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.7/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.7/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.119693 domolibrary-0.1.7/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.7/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.7/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.7/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.7/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.7/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.119693 domolibrary-0.1.7/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.7/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.7/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.7/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 18:27:21.127693 domolibrary-0.1.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.119693 domolibrary-0.1.7/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148101 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.123693 domolibrary-0.1.7/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18138 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.123693 domolibrary-0.1.7/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.123693 domolibrary-0.1.7/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.127693 domolibrary-0.1.7/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8286 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.127693 domolibrary-0.1.7/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 18:26:38.000000 domolibrary-0.1.7/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.119693 domolibrary-0.1.7/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.7/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 18:27:21.000000 domolibrary-0.1.7/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 18:27:17.000000 domolibrary-0.1.7/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 18:27:21.131693 domolibrary-0.1.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.7/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:27:21.127693 domolibrary-0.1.7/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.7/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.7/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.7/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.7/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.128456 domolibrary-0.1.8/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.004458 domolibrary-0.1.8/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.8/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.016457 domolibrary-0.1.8/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.060457 domolibrary-0.1.8/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.8/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.8/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.8/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.8/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.8/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.8/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.8/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.8/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.8/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 19:37:21.128456 domolibrary-0.1.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.8/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148101 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.088456 domolibrary-0.1.8/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18323 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.088456 domolibrary-0.1.8/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.092456 domolibrary-0.1.8/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.100456 domolibrary-0.1.8/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8346 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.100456 domolibrary-0.1.8/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.080457 domolibrary-0.1.8/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.8/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 19:37:15.000000 domolibrary-0.1.8/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 19:37:21.128456 domolibrary-0.1.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.124456 domolibrary-0.1.8/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.8/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.8/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.8/utils/upload_data.py
```

### Comparing `domolibrary-0.1.7/Automation/automation.py` & `domolibrary-0.1.8/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DataOcean/Transport.py` & `domolibrary-0.1.8/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.8/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.8/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DataOcean/cnfg_s3.py` & `domolibrary-0.1.8/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.8/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoAccount.py` & `domolibrary-0.1.8/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.8/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.8/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoApplication.py` & `domolibrary-0.1.8/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoAuth.py` & `domolibrary-0.1.8/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.8/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoCard.py` & `domolibrary-0.1.8/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoCertification.py` & `domolibrary-0.1.8/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.8/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.8/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoDataset.py` & `domolibrary-0.1.8/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoGrant.py` & `domolibrary-0.1.8/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoGroup.py` & `domolibrary-0.1.8/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.8/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoJob.py` & `domolibrary-0.1.8/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoLineage.py` & `domolibrary-0.1.8/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoPDP.py` & `domolibrary-0.1.8/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoPage.py` & `domolibrary-0.1.8/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoPublish.py` & `domolibrary-0.1.8/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoRole.py` & `domolibrary-0.1.8/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.8/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoStream.py` & `domolibrary-0.1.8/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoTag.py` & `domolibrary-0.1.8/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/DomoUser.py` & `domolibrary-0.1.8/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/get_data.py` & `domolibrary-0.1.8/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.8/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/LICENSE` & `domolibrary-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/PKG-INFO` & `domolibrary-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.7/README.md` & `domolibrary-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/_modidx.py` & `domolibrary-0.1.8/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.8/domolibrary/classes/DomoAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,14 +531,15 @@
         )
 
     return True
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 35
 @patch_to(DomoAccount)
 async def _is_group_ownership_beta(self, auth : dmda.DomoAuth):
+
     import domolibrary.classes.DomoBootstrap as dmbs
 
     domo_bsr = dmbs.DomoBootstrap(auth=auth or self.auth)
     domo_feature_ls = await domo_bsr.get_features()
 
     match_accounts_v2 = next(
         (domo_feature for domo_feature in domo_feature_ls if domo_feature.name == 'accounts-v2'), None)
@@ -547,62 +548,71 @@
 
 
 @patch_to(DomoAccount)
 async def share_account(
     self,
     user_id: int,
     auth: dmda.DomoAuth = None,
-    is_v2 :bool = None,
-    access_level: ShareAccount = None, # will default to Read
+    is_v2: bool = None,
+    access_level: ShareAccount = None,  # will default to Read
     debug_api: bool = False,
-    debug_prn:bool = False,
+    debug_prn: bool = False,
     session: httpx.AsyncClient = None,
 ):
     auth = auth or self.auth
 
+    
     if isinstance(auth, dmda.DomoFullAuth) and is_v2 is None:
         is_v2 = await self._is_group_ownership_beta(auth)
-    
+
     if debug_prn:
-        print( f"ℹ️ - {auth.domo_instance} - {'is' if is_v2 else 'is not'} v2_group_ownership")
+        print(
+            f"ℹ️ - {auth.domo_instance} - {'is' if is_v2 else 'is not'} v2_group_ownership")
 
     if is_v2 is None:
         raise Exception(
             """🛑 ERROR must pass `is_v2` bool to share_accounts function IF NOT pass `dmda.DomoFullAuth`.
 the group management v2 API has a different body.  
 Alternatively pass a full auth object to auto check the bootstrap.
 """)
+    
+    res = None
 
     if is_v2:
         share_payload = account_routes.generate_share_account_payload_v2(
             user_id=user_id, access_level=access_level or ShareAccount_V2_AccessLevel.CAN_VIEW
         )
 
-        return await account_routes.share_account_v2(
+        res = await account_routes.share_account_v2(
             auth=auth,
             account_id=self.id,
             share_payload=share_payload,
             debug_api=debug_api,
             session=session,
         )
 
-    share_payload = account_routes.generate_share_account_payload_v1(
-        user_id=user_id, access_level=access_level or ShareAccount_V1_AccessLevel.CAN_VIEW
-    )
-
-    res = await account_routes.share_account_v1(
-        auth=auth,
-        account_id=self.id,
-        share_payload=share_payload,
-        debug_api=debug_api,
-        session=session,
-    )
+    else:
+        share_payload = account_routes.generate_share_account_payload_v1(
+            user_id=user_id, access_level=access_level or ShareAccount_V1_AccessLevel.CAN_VIEW
+        )
+
+        res = await account_routes.share_account_v1(
+            auth=auth,
+            account_id=self.id,
+            share_payload=share_payload,
+            debug_api=debug_api,
+            session=session,
+        )
 
     if res.status == 500 and res.response == 'Internal Server Error':
         res.response = f'ℹ️ - {res.response + "| User may own account."}'
+
+    if res.status == 200:
+        res.response = f"shared {self.id} - {self.name} with {user_id}"
+
     return res
 
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 38
 @dataclass
 class DomoAccounts:
     auth: dmda.DomoAuth
```

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.8/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.8/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.8/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.8/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.8/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.8/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.8/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.8/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.8/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.8/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.8/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.8/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.8/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.8/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/client/DomoError.py` & `domolibrary-0.1.8/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/client/Logger.py` & `domolibrary-0.1.8/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.8/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/client/get_data.py` & `domolibrary-0.1.8/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.8/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.8/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/account.py` & `domolibrary-0.1.8/domolibrary/routes/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         url=url,
         method='PUT',
         body=share_payload,
         debug_api=debug_api,
         session=session
     )
 
-
+#v1 may have been deprecated.  used to be tied to group beta
 async def share_account_v1(auth: dmda.DomoAuth,
                            account_id: str,
                            share_payload: dict,
                            debug_api: bool = False,
                            session: httpx.AsyncClient = None
                            ):
```

### Comparing `domolibrary-0.1.7/domolibrary/routes/activity_log.py` & `domolibrary-0.1.8/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.8/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/card.py` & `domolibrary-0.1.8/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/datacenter.py` & `domolibrary-0.1.8/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/dataflow.py` & `domolibrary-0.1.8/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/dataset.py` & `domolibrary-0.1.8/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/grant.py` & `domolibrary-0.1.8/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/group.py` & `domolibrary-0.1.8/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/instance_config.py` & `domolibrary-0.1.8/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/page.py` & `domolibrary-0.1.8/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/pdp.py` & `domolibrary-0.1.8/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/publish.py` & `domolibrary-0.1.8/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/role.py` & `domolibrary-0.1.8/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/routes/user.py` & `domolibrary-0.1.8/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/utils/DictDot.py` & `domolibrary-0.1.8/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.8/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/utils/convert.py` & `domolibrary-0.1.8/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.8/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary/utils/upload_data.py` & `domolibrary-0.1.8/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.8/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.7/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.8/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/settings.ini` & `domolibrary-0.1.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.07
+version = 0.1.08
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.7/setup.py` & `domolibrary-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/Base.py` & `domolibrary-0.1.8/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/DictDot.py` & `domolibrary-0.1.8/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/Exceptions.py` & `domolibrary-0.1.8/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/LoggerClass.py` & `domolibrary-0.1.8/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/chunk_execution.py` & `domolibrary-0.1.8/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/consol_get_creds.py` & `domolibrary-0.1.8/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/convert.py` & `domolibrary-0.1.8/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.8/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.7/utils/upload_data.py` & `domolibrary-0.1.8/utils/upload_data.py`

 * *Files identical despite different names*

