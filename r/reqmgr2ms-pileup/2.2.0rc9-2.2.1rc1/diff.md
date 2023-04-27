# Comparing `tmp/reqmgr2ms-pileup-2.2.0rc9.tar.gz` & `tmp/reqmgr2ms-pileup-2.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqmgr2ms-pileup-2.2.0rc9.tar", last modified: Wed Apr 12 16:18:16 2023, max compression
+gzip compressed data, was "reqmgr2ms-pileup-2.2.1rc1.tar", last modified: Tue Apr 25 21:48:32 2023, max compression
```

## Comparing `reqmgr2ms-pileup-2.2.0rc9.tar` & `reqmgr2ms-pileup-2.2.1rc1.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.273743 reqmgr2ms-pileup-2.2.0rc9/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.273743 reqmgr2ms-pileup-2.2.0rc9/bin/HWMon/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23048 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/HWMon/wmcore-SysStat
--rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/acdcserver-tools
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.277742 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/ParseSpecCmsswdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/checkDsetFileCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/checkStuckLQE.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/createPileupObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/drainAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/getWQStatusByWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/mongoInit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/parseUnifiedCampaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/setrequeststatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/summaryWMStatsFailures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/updateTotalStats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/workflowCompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/attempt-to-patch.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3324 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/buildrelease.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/check-ACDC-parentage
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/check-phedex-dbs-status
--rwxr-xr-x   0 runner    (1001) docker     (123)     7262 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/check-request-wq-status
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/clean-oracle
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/combineMinifyWMStats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/couch-thrash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/couch_archiver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/create-iam-token.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/createStoreResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/dbsbuffer-file-fix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5982 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/deploy-rpm-to-jenkins.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4803 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/fix-dbs-parentage
--rwxr-xr-x   0 runner    (1001) docker     (123)     1623 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/inject-to-config-cache
--rwxr-xr-x   0 runner    (1001) docker     (123)     2939 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/kill-workflow-in-agent
--rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/kill-workflow-in-global
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/make-local-clones.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/outputmodules-from-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/patchComponent.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6550 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/paused-jobs
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/purgeDeletedCouchDoc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/reqmgr-put-default-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/reqmgr-sw-update
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/vaildateCMSSWMergeVersion
--rwxr-xr-x   0 runner    (1001) docker     (123)    19065 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-couchapp-init
--rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-delete-couchdb-workflow
--rwxr-xr-x   0 runner    (1001) docker     (123)    16382 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-mod-config
--rwxr-xr-x   0 runner    (1001) docker     (123)    15441 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-resource-control
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-unregister-wmstats
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-upload-config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7198 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-workqueue
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmc-dist-patch
--rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmc-dist-unpatch
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmc-httpd
--rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-db-init
--rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-new-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-new-flow
--rwxr-xr-x   0 runner    (1001) docker     (123)    10729 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/bin/wmcoreD
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 16:18:15.000000 reqmgr2ms-pileup-2.2.0rc9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 16:18:15.000000 reqmgr2ms-pileup-2.2.0rc9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/setup_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/setup_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.265742 reqmgr2ms-pileup-2.2.0rc9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.269743 reqmgr2ms-pileup-2.2.0rc9/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.277742 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9690 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/CPMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/CertTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/EmailAlert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/ExtendedUnitTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/FileTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/IteratorTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/MathUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/MemoryCache.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/PortForward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/ProcessStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/PythonVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TemporaryEnvironment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Throttled.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TokenManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TwPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.277742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.277742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/MathAlgos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/MiscAlgos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/ParseXMLFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/SubprocessAlgos.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/GenericDataCache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/WMConfigCache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19963 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DAOFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Fileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/JobGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/JobPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/LumiList.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Pickleable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/WMObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/WorkUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/
--rw-r--r--   0 runner    (1001) docker     (123)    53857 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/CMSCouch.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ConfigDBMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/CouchUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBExceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/Dialects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ExecuteDAO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/MongoDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/MySQLCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ResultSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/Transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ipy_profile_couch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/CouchObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Lexicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.269743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/CherryPyThreads/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/CherryPyThreads/HeartbeatMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/CherryPyThreads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.281742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/DataStructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/DataStructs/DefaultStructs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/DataStructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSAuth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSCore.py
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupObj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupReport.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupError.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupTaskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/RestApiHub.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/
--rw-r--r--   0 runner    (1001) docker     (123)    24922 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/Common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/PycurlRucio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/WebGui/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/WebGui/FrontPage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/WebGui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/CherryPyPeriodicTask.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Error.py
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/HeartbeatMonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)   118317 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/DataStructs/
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/DataStructs/RequestStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/DataStructs/RequestType.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/DataStructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.285742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/AlertManager/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/AlertManager/AlertManagerAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/AlertManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/CRIC/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/CRIC/CRIC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/CRIC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/
--rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBS3Reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSErrors.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSWriterObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/ProdException.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/FWJRDB/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/FWJRDB/FWJRDBAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/FWJRDB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/HTTPS/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/HTTPS/HTTPSAuthHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/HTTPS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDBBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDBExceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDBReport.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/McM/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/McM/McM.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/McM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/MonIT/
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/MonIT/Grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/MonIT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/PyCondorAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/PyCondorUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgr/
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgr/ReqMgr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgrAux/
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgrAux/ReqMgrAux.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgrAux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/RequestDBReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/RequestDBWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/
--rw-r--r--   0 runner    (1001) docker     (123)    60261 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/Rucio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/RucioUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RucioConMon/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RucioConMon/RucioConMon.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RucioConMon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/StompAMQ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/StompAMQ/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/TagCollector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/XMLUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/UUIDLib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/UserFileCache/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/UserFileCache/UserFileCache.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/UserFileCache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.289742 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMAgent/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMAgent/WMAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMAgent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/DataMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/WMArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMBS/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMBS/WMBS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMBS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/DataStruct/
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/DataStruct/RequestInfoCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/DataStruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/WMStatsReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/WMStatsWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStatsServer/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStatsServer/WMStatsServer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStatsServer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WorkQueue/
--rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WorkQueue/WorkQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WorkQueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/pycurl_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMConnectionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMException.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMExceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMInit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMLogging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/JsonWrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/JsonWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 16:18:12.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:18:16.293743 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 16:18:16.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-12 16:18:16.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:18:16.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 16:18:16.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 16:18:16.000000 reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.340247 reqmgr2ms-pileup-2.2.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 21:48:32.340247 reqmgr2ms-pileup-2.2.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.296247 reqmgr2ms-pileup-2.2.1rc1/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.296247 reqmgr2ms-pileup-2.2.1rc1/bin/HWMon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23048 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/HWMon/wmcore-SysStat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/acdcserver-tools
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.300247 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/ParseSpecCmsswdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/checkDsetFileCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/checkStuckLQE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/createPileupObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/drainAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/getWQStatusByWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/mongoInit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/parseUnifiedCampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/setrequeststatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/summaryWMStatsFailures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/updateTotalStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/workflowCompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/attempt-to-patch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3324 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/buildrelease.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/check-ACDC-parentage
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/check-phedex-dbs-status
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7262 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/check-request-wq-status
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/clean-oracle
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/combineMinifyWMStats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/couch-thrash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/couch_archiver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/create-iam-token.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/createStoreResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/dbsbuffer-file-fix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5982 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/deploy-rpm-to-jenkins.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4803 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/fix-dbs-parentage
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/inject-to-config-cache
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2939 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/kill-workflow-in-agent
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/kill-workflow-in-global
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/make-local-clones.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3615 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/outputmodules-from-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/patchComponent.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6550 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/paused-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/purgeDeletedCouchDoc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/reqmgr-put-default-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/reqmgr-sw-update
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/vaildateCMSSWMergeVersion
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19065 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-couchapp-init
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-delete-couchdb-workflow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16408 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-mod-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15441 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-resource-control
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-unregister-wmstats
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-upload-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7198 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-workqueue
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmc-dist-patch
+-rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmc-dist-unpatch
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmc-httpd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-db-init
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-new-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-new-flow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10729 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/bin/wmcoreD
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 21:48:30.000000 reqmgr2ms-pileup-2.2.1rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 21:48:32.340247 reqmgr2ms-pileup-2.2.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 21:48:30.000000 reqmgr2ms-pileup-2.2.1rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/setup_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-25 21:48:20.000000 reqmgr2ms-pileup-2.2.1rc1/setup_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.284247 reqmgr2ms-pileup-2.2.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.288246 reqmgr2ms-pileup-2.2.1rc1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.304247 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9690 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/CPMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/CertTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/EmailAlert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/ExtendedUnitTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/FileTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/IteratorTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/MathUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/MemoryCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/PortForward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/ProcessStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/PythonVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TemporaryEnvironment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Throttled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TokenManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TwPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.308247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.308247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/MathAlgos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/MiscAlgos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/ParseXMLFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/SubprocessAlgos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.308247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/GenericDataCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/WMConfigCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DAOFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.312247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Fileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/JobGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/JobPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/LumiList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Pickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/WMObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/WorkUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.312247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/
+-rw-r--r--   0 runner    (1001) docker     (123)    53857 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/CMSCouch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ConfigDBMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/CouchUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBExceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/Dialects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ExecuteDAO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/MySQLCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ResultSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/Transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ipy_profile_couch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.316247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/CouchObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Lexicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.284247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.316247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/CherryPyThreads/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/CherryPyThreads/HeartbeatMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/CherryPyThreads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.316247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/DataStructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/DataStructs/DefaultStructs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/DataStructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.316247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.320247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.320247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupError.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupTaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23082 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.320247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/RestApiHub.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.320247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    24922 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/Common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/PycurlRucio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.320247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/WebGui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/WebGui/FrontPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/WebGui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.324247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/CherryPyPeriodicTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/HeartbeatMonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118317 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.324247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.324247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/DataStructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/DataStructs/RequestStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/DataStructs/RequestType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/DataStructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.324247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.324247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/AlertManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/AlertManager/AlertManagerAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/AlertManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.328247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/CRIC/
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/CRIC/CRIC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/CRIC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.328247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/
+-rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBS3Reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSErrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSWriterObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/ProdException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.328247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/FWJRDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/FWJRDB/FWJRDBAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/FWJRDB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.328247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/HTTPS/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/HTTPS/HTTPSAuthHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/HTTPS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.328247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDBBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDBExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDBReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/McM/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/McM/McM.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/McM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/MonIT/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/MonIT/Grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/MonIT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/PyCondorAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/PyCondorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgr/
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgr/ReqMgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgrAux/
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgrAux/ReqMgrAux.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgrAux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/RequestDBReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/RequestDBWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/
+-rw-r--r--   0 runner    (1001) docker     (123)    60261 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/Rucio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/RucioUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RucioConMon/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RucioConMon/RucioConMon.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RucioConMon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.332247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/StompAMQ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/StompAMQ/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/TagCollector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/XMLUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/UUIDLib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/UserFileCache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/UserFileCache/UserFileCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/UserFileCache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMAgent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMAgent/WMAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMAgent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/DataMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/WMArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMBS/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMBS/WMBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMBS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/DataStruct/
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/DataStruct/RequestInfoCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/DataStruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/WMStatsReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/WMStatsWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStatsServer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStatsServer/WMStatsServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStatsServer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WorkQueue/
+-rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WorkQueue/WorkQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WorkQueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/pycurl_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMConnectionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMException.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMInit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMLogging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.336247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.340247 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 21:48:21.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:32.340247 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 21:48:31.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-25 21:48:32.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:48:31.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 21:48:31.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 21:48:31.000000 reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/top_level.txt
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/LICENSE` & `reqmgr2ms-pileup-2.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/NOTICE` & `reqmgr2ms-pileup-2.2.1rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/README.md` & `reqmgr2ms-pileup-2.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/HWMon/wmcore-SysStat` & `reqmgr2ms-pileup-2.2.1rc1/bin/HWMon/wmcore-SysStat`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/acdcserver-tools` & `reqmgr2ms-pileup-2.2.1rc1/bin/acdcserver-tools`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/ParseSpecCmsswdist.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/ParseSpecCmsswdist.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/checkDsetFileCount.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/checkDsetFileCount.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/checkStuckLQE.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/checkStuckLQE.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/createPileupObjects.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/createPileupObjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
     Get a minimalistic pileup data schema, or return an
     existent pileup object.
 
     :param pileupName: string with the pileup name
     :param pileupDocs: list of pileup documents
     :return: a dictionary with the pileup configuration
     """
-    for doc in pileupDocs:
+    for idx, doc in enumerate(pileupDocs):
         if pileupName == doc["pileupName"]:
             logger.warning("Reusing pileup configuration for pileup: %s", pileupName)
-            return doc
+            return pileupDocs.pop(idx)
     pileupDoc = {
         'pileupName': "",
         'pileupType': "",
         'expectedRSEs': [],
         'campaigns': [],
         'active': False}
     return pileupDoc
@@ -92,15 +92,18 @@
      * expectedRSEs: is a union of all RSEs across different campaigns.
     """
     pileupDocs = []
     for camp in campDocs:
         # for each secondary dataset, create one pileup document
         for puName, puRSEs in camp.get("Secondaries", {}).items():
             puDoc = getPUSchema(puName, pileupDocs, logger)
-            puType = "premix" if puName.split("/")[-1] == "PREMIX" else "classic"
+            if puName.startswith("/Neutrino") or puName.split("/")[-1] == "PREMIX":
+                puType = "premix"
+            else:
+                puType = "classic"
             puDoc["pileupName"] = puName
             puDoc["pileupType"] = puType
             puDoc["expectedRSEs"].extend(puRSEs)
             if camp.get("CampaignName", ""):
                 puDoc["campaigns"].append(camp["CampaignName"])
             # make some of these values unique
             puDoc["expectedRSEs"] = list(set(puDoc["expectedRSEs"]))
@@ -164,15 +167,15 @@
         reqAux = ReqMgrAux(opts.url + "/reqmgr2", hdict, logger=logger)
         campDocs = reqAux.getCampaignConfig("ALL_DOCS")
         logger.info("Retrieved %d campaigns from ReqMgr.", len(campDocs))
         puDocs = parseCampaigns(campDocs, logger)
     if opts.fout:
         logger.info("Saving all %d pileup documents into file: %s", len(puDocs), opts.fout)
         with open(opts.fout, "w") as jo:
-            json.dump(puDocs, jo, indent=2)
+            json.dump(puDocs, jo, indent=2, sort_keys=True)
 
     if opts.inject:
         logger.info("Going to inject %d pileup documents into: %s", len(puDocs), opts.url)
         writePileupDocs(opts.url, puDocs, hdict, logger)
     else:
         logger.info("DRY-RUN: not injecting any pileup documents in MSPileup.")
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/drainAgent.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/drainAgent.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/getWQStatusByWorkflow.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/getWQStatusByWorkflow.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/mongoInit.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/mongoInit.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/parseUnifiedCampaigns.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/parseUnifiedCampaigns.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/setrequeststatus.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/setrequeststatus.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/summaryWMStatsFailures.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/summaryWMStatsFailures.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/updateTotalStats.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/updateTotalStats.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/adhoc-scripts/workflowCompletion.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/adhoc-scripts/workflowCompletion.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/attempt-to-patch.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/attempt-to-patch.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/buildrelease.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/buildrelease.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/check-ACDC-parentage` & `reqmgr2ms-pileup-2.2.1rc1/bin/check-ACDC-parentage`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/check-request-wq-status` & `reqmgr2ms-pileup-2.2.1rc1/bin/check-request-wq-status`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/clean-oracle` & `reqmgr2ms-pileup-2.2.1rc1/bin/clean-oracle`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/combineMinifyWMStats.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/combineMinifyWMStats.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/couch-thrash.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/couch-thrash.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/couch_archiver.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/couch_archiver.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/create-iam-token.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/create-iam-token.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/createStoreResults.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/createStoreResults.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/dbsbuffer-file-fix.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/dbsbuffer-file-fix.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/deploy-rpm-to-jenkins.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/deploy-rpm-to-jenkins.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/fix-dbs-parentage` & `reqmgr2ms-pileup-2.2.1rc1/bin/fix-dbs-parentage`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/inject-to-config-cache` & `reqmgr2ms-pileup-2.2.1rc1/bin/inject-to-config-cache`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 _inject-to-config-cache_
 
 Add a config and it's meta data to the config cache.
 """
 
 import os
 import sys
-import imp
-import subprocess
+import importlib
 
 from PSetTweaks.WMTweak import makeTweak
 from WMCore.Cache.WMConfigCache import ConfigCache
 
 def loadConfig(configPath):
     """
     _loadConfig_
 
     Import a config.
     """
     print("Importing the config, this may take a while...", end=' ')
     sys.stdout.flush()
     cfgBaseName = os.path.basename(configPath).replace(".py", "")
     cfgDirName = os.path.dirname(configPath)
-    modPath = imp.find_module(cfgBaseName, [cfgDirName])
-
-    loadedConfig = imp.load_module(cfgBaseName, modPath[0],
-                                   modPath[1], modPath[2])
+    modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName, [cfgDirName])
+    module = modSpecs.loader.load_module()
 
     print("done.")
-    return loadedConfig
+    return module
 
-if __name__ == "__main__":
+def main():
+    """
+    Main function of the module
+    """
     if len(sys.argv) != 8:
         print("Usage: %s couchUrl database_name user_name group_name input_file label description" % sys.argv[0])
         sys.exit(1)
 
     if not os.path.exists(sys.argv[5]):
         print("Error: Can't locate config file.")
         sys.exit(1)
@@ -50,7 +50,10 @@
     configCache.setDescription(sys.argv[7])
     configCache.save()
 
     print("Added file to the config cache:")
     print("  DocID:    %s" % configCache.document["_id"])
     print("  Revision: %s" % configCache.document["_rev"])
     sys.exit(0)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/kill-workflow-in-agent` & `reqmgr2ms-pileup-2.2.1rc1/bin/kill-workflow-in-agent`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/kill-workflow-in-global` & `reqmgr2ms-pileup-2.2.1rc1/bin/kill-workflow-in-global`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/make-local-clones.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/make-local-clones.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/outputmodules-from-config` & `reqmgr2ms-pileup-2.2.1rc1/bin/outputmodules-from-config`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 """
 _outputmodules-from-config_
 
 Pull output module metadata from a CMSSW config.
 """
 import urllib.request
 
-import imp
+import importlib
 import os
 import sys
 import tempfile
 from json import JSONEncoder, JSONDecoder
 
 
 def loadConfig(configPath):
     """
     _loadConfig_
 
     Import a config.
     """
     cfgBaseName = os.path.basename(configPath).replace(".py", "")
     cfgDirName = os.path.dirname(configPath)
-    modPath = imp.find_module(cfgBaseName, [cfgDirName])
-    
-    loadedConfig = imp.load_module(cfgBaseName, modPath[0],
-                                   modPath[1], modPath[2])
-    
-    return loadedConfig
+    modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName, [cfgDirName])
+    module = modSpecs.loader.load_module()
+    return module
 
 def outputModulesFromConfig(configHandle):
     """
     _outputModulesFromConfig_
 
     Go through all the output modules in a config and extract the meta data.
     """
@@ -51,15 +48,18 @@
                 filterName = filterNameAttr.value()
                 
             outputModules[outputModuleName] = {"dataTier": dataTier,
                                                "filterName": filterName}
             
     return outputModules
 
-if __name__ == "__main__":
+def main():
+    """
+    Main function of the module
+    """
     try:
         jsonDecoder = JSONDecoder()
         jsonEncoder = JSONEncoder()
 
         encodedConfig = sys.stdin.readline()
         config = jsonDecoder.decode(encodedConfig)
 
@@ -98,7 +98,10 @@
         outputHandle.write("%s\n" % outputModulesJSON)
         outputHandle.close()
         
         sys.exit(0)
     except Exception as ex:
         print(ex)
         sys.exit(1)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/patchComponent.sh` & `reqmgr2ms-pileup-2.2.1rc1/bin/patchComponent.sh`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/paused-jobs` & `reqmgr2ms-pileup-2.2.1rc1/bin/paused-jobs`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/purgeDeletedCouchDoc.py` & `reqmgr2ms-pileup-2.2.1rc1/bin/purgeDeletedCouchDoc.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/reqmgr-put-default-config` & `reqmgr2ms-pileup-2.2.1rc1/bin/reqmgr-put-default-config`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/reqmgr-sw-update` & `reqmgr2ms-pileup-2.2.1rc1/bin/reqmgr-sw-update`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/vaildateCMSSWMergeVersion` & `reqmgr2ms-pileup-2.2.1rc1/bin/vaildateCMSSWMergeVersion`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-couchapp-init` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-couchapp-init`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-delete-couchdb-workflow` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-delete-couchdb-workflow`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-mod-config` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-mod-config`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Copyright (c) 2011 Fermilab. All rights reserved.
 
 Note: this script is also used by ASO deployment, see:
 https://github.com/dmwm/deployment/blob/master/asyncstageout/manage#L246
 """
 
 import getopt
-import imp
+import importlib
 import os
 import socket
 import sys
 import traceback
 from urllib.parse import urlparse
 
 from WMCore.Configuration import saveConfigurationFile
@@ -39,15 +39,16 @@
 def importConfigTemplate(filename):
     """
     _importConfigTemplate_
 
     Given filename, load it and grab the configuration object from it
 
     """
-    mod = imp.load_module("wmcore_config_input", open(filename, 'r'), filename, (".py", "r", imp.PY_SOURCE))
+    modSpecs = importlib.machinery.PathFinder().find_spec(filename)
+    mod = modSpecs.loader.load_module("wmcore_config_input")
     config = getattr(mod, 'config', None)
     if config is None:
         msg = "No config attribute found in %s" % filename
         raise RuntimeError(msg)
     return config
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-resource-control` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-resource-control`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-unregister-wmstats` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-unregister-wmstats`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-upload-config` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-upload-config`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmagent-workqueue` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmagent-workqueue`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmc-dist-patch` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmc-dist-patch`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-db-init` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-db-init`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-new-config` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-new-config`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmcore-new-flow` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmcore-new-flow`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/bin/wmcoreD` & `reqmgr2ms-pileup-2.2.1rc1/bin/wmcoreD`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/setup.py` & `reqmgr2ms-pileup-2.2.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/setup_build.py` & `reqmgr2ms-pileup-2.2.1rc1/setup_build.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/setup_dependencies.py` & `reqmgr2ms-pileup-2.2.1rc1/setup_dependencies.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/CPMetrics.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/CPMetrics.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/CertTools.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/CertTools.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/EmailAlert.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/EmailAlert.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/ExtendedUnitTestCase.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/ExtendedUnitTestCase.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/FileTools.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/FileTools.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/IteratorTools.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/IteratorTools.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/MathUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/MathUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/MemoryCache.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/MemoryCache.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Pipeline.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Pipeline.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/PortForward.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/PortForward.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/ProcessStats.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/ProcessStats.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/PythonVersion.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/PythonVersion.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Signals.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Signals.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TemporaryEnvironment.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TemporaryEnvironment.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Throttled.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Throttled.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Timers.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Timers.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TokenManager.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TokenManager.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Tracing.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Tracing.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/TwPrint.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/TwPrint.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/Utils/Utilities.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/Utils/Utilities.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Alarm.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Alarm.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/MathAlgos.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/MathAlgos.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/MiscAlgos.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/MiscAlgos.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/ParseXMLFile.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/ParseXMLFile.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Permissions.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Permissions.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/Singleton.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/Singleton.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Algorithms/SubprocessAlgos.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Algorithms/SubprocessAlgos.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/GenericDataCache.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/GenericDataCache.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Cache/WMConfigCache.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Cache/WMConfigCache.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Configuration.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from future.utils import listvalues
 
 import os
 import traceback
 
 from Utils.PythonVersion import PY3
 
-import imp
+import importlib
 
 _SimpleTypes = [
     bool,
     float,
     # basestring,  # For py2/py3 compatibility, don't let futurize remove PY3 Remove when python 3 transition complete
     newbytes,
     newstr,
@@ -592,20 +592,19 @@
     Load a Configuration File
 
     """
 
     cfgBaseName = os.path.basename(filename).replace(".py", "")
     cfgDirName = os.path.dirname(filename)
     if not cfgDirName:
-        modPath = imp.find_module(cfgBaseName)
+        modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName)
     else:
-        modPath = imp.find_module(cfgBaseName, [cfgDirName])
+        modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName, [cfgDirName])
     try:
-        modRef = imp.load_module(cfgBaseName, modPath[0],
-                                          modPath[1], modPath[2])
+        modRef = modSpecs.loader.load_module()
     except Exception as ex:
         msg = "Unable to load Configuration File:\n"
         msg += "%s\n" % filename
         msg += "Due to error:\n"
         msg += str(ex)
         msg += str(traceback.format_exc())
         raise RuntimeError(msg)
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DAOFactory.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DAOFactory.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/File.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/File.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Fileset.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Fileset.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Job.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Job.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/JobGroup.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/JobGroup.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/JobPackage.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/JobPackage.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/LumiList.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/LumiList.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Mask.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Mask.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Run.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Run.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Subscription.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Subscription.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/WMObject.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/WMObject.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/WorkUnit.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/WorkUnit.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/DataStructs/Workflow.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/DataStructs/Workflow.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/CMSCouch.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/CMSCouch.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ConfigDBMap.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ConfigDBMap.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/CouchUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/CouchUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBCore.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBCore.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBCreator.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBCreator.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBExceptionHandler.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBFactory.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBFactory.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/DBFormatter.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/DBFormatter.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ExecuteDAO.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ExecuteDAO.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/MongoDB.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/MongoDB.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/MySQLCore.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/MySQLCore.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ResultSet.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ResultSet.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/Transaction.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/Transaction.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Database/ipy_profile_couch.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Database/ipy_profile_couch.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/CouchObject.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/CouchObject.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Decorators.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Decorators.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Group.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Group.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/Interface.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/Interface.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/GroupUser/User.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/GroupUser/User.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Lexicon.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Lexicon.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/DataStructs/DefaultStructs.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/DataStructs/DefaultStructs.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSAuth.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSAuth.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSCore.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSCore.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/MSManager.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/MSManager.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSCore/TaskManager.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSCore/TaskManager.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupObj.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupObj.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupReport.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/DataStructs/MSPileupReport.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileup.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileup.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupData.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupData.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,29 @@
 
     if docs and isinstance(docs, dict):
         for key in skeys:
             docs.pop(key, None)
     return docs
 
 
+def getNewTimestamp(doc):
+    """
+    Given a pileup doc - or a subset of it - return a dictionary
+    with a couple timestamp attributes that need to be updated.
+    :param doc: a python dictionary representing the pileup information
+    :return: a python dictionary to update the pileup object
+    """
+    subDoc = {'lastUpdateTime': gmtimeSeconds()}
+    if "active" in doc and doc['active'] is True:
+        subDoc['activatedOn'] = gmtimeSeconds()
+    elif "active" in doc and doc['active'] is False:
+        subDoc['deactivatedOn'] = gmtimeSeconds()
+    return subDoc
+
+
 class MSPileupData():
     """
     MSPileupData provides logic behind data used and stored by MSPileup module
     """
 
     def __init__(self, msConfig, **kwargs):
         """
@@ -160,15 +175,16 @@
             except Exception as exp:
                 msg = f"Failed to update MSPileupObj, {exp}"
                 self.logger.exception(msg)
                 err = MSPileupSchemaError(doc, msg)
                 self.logger.error(err)
                 return [err.error()]
 
-        doc['lastUpdateTime'] = gmtimeSeconds()
+        # mandatory timestamp updates
+        doc.update(getNewTimestamp(doc))
         # we do not need to create MSPileupObj and validate it since our doc comes directly from DB
         try:
             self.dbColl.update_one(spec, {"$set": doc})
             self.logger.info("Pileup object %s successfully updated", spec.get("pileupName"))
         except Exception as exp:
             msg = f"Failed to insert: {doc}, error {exp}"
             self.logger.exception(msg)
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupError.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupError.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupMonitoring.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupMonitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,16 @@
 
     def __init__(self, msConfig=None):
         """
         Constructor for MSPileupMonitoring
         """
         self.userAMQ = msConfig.get('user_amq', None)
         self.passAMQ = msConfig.get('pass_amq', None)
-        self.postToAMQ = msConfig.get('post_to_amq', False)
         self.topicAMQ = msConfig.get('topic_amq', None)
-        self.docTypeAMQ = msConfig.get('doc_type_amg', 'cms-ms-pileup')
+        self.docTypeAMQ = msConfig.get('doc_type_amq', 'cms-ms-pileup')
         self.hostPortAMQ = msConfig.get('host_port_amq', None)
         self.producer = msConfig.get('producer', 'cms-ms-pileup')
         self.logger = msConfig.get('logger', getMSLogger(False))
 
     def uploadToAMQ(self, docs, producer=None):
         """
         _uploadToAMQ_
@@ -99,11 +98,11 @@
                                                                ts=ts, data_subfield="payload")
                 notifications.append(singleNotif)
 
             failures = stompSvc.send(notifications)
             msg = "%i out of %i documents successfully sent to AMQ" % (len(notifications) - len(failures),
                                                                        len(notifications))
             self.logger.info(msg)
-            return {"success": len(notifications)-len(failures), "failures": len(failures)}
+            return {"success": len(notifications) - len(failures), "failures": len(failures)}
         except Exception as ex:
             self.logger.exception("Failed to send data to StompAMQ. Error %s", str(ex))
         return {}
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupTaskManager.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupTaskManager.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     - perform task for inactive pileups
 """
 
 # system modules
 from threading import current_thread
 
 # WMCore modules
+from Utils.Timers import CodeTimer
 from WMCore.MicroService.MSCore.MSCore import MSCore
 from WMCore.MicroService.DataStructs.DefaultStructs import PILEUP_REPORT
 from WMCore.MicroService.MSPileup.MSPileupData import MSPileupData
 from WMCore.MicroService.MSPileup.MSPileupTasks import MSPileupTasks
 from WMCore.MicroService.MSPileup.MSPileupMonitoring import MSPileupMonitoring
 
 
@@ -54,13 +55,19 @@
         summary.update({'tasks': report.getDocuments()})
         return summary
 
     def executeCycle(self):
         """
         execute MSPileupTasks polling cycle
         """
-        self.mgr.pileupSizeTask()
-        self.mgr.monitoringTask()
-        self.mgr.activeTask(marginSpace=self.marginSpace)
-        self.mgr.inactiveTask()
-        self.mgr.cleanupTask(self.cleanupDaysThreshold)
-        self.mgr.cmsMonitTask()
+        with CodeTimer("### pileupSizeTask", logger=self.logger):
+            self.mgr.pileupSizeTask()
+        with CodeTimer("### monitoringTask", logger=self.logger):
+            self.mgr.monitoringTask()
+        with CodeTimer("### activeTask", logger=self.logger):
+            self.mgr.activeTask(marginSpace=self.marginSpace)
+        with CodeTimer("### inactiveTask", logger=self.logger):
+            self.mgr.inactiveTask()
+        with CodeTimer("### cleanupTask", logger=self.logger):
+            self.mgr.cleanupTask(self.cleanupDaysThreshold)
+        with CodeTimer("### cmsMonitTask", logger=self.logger):
+            self.mgr.cmsMonitTask()
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/MSPileup/MSPileupTasks.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/MSPileup/MSPileupTasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,22 @@
         self.mgr = dataManager
         self.monitManager = monitManager
         self.logger = logger
         self.rucioAccount = rucioAccount
         self.rucioClient = rucioClient
         self.report = MSPileupReport()
         self.dryRun = dryRun
+        if dryRun:
+            self.logger.info("MSPileupTasks is set to DRY-RUN mode!")
 
     def pileupSizeTask(self):
         """
         Execute pileup size update task
         """
+        self.logger.info("====> Executing pileupSizeTask method...")
         try:
             # get pileup sizes and update them in DB
             spec = {}
             docs = self.mgr.getPileup(spec)
             rucioAuthUrl = self.rucioClient.rucioParams['auth_host']
             rucioHostUrl = self.rucioClient.rucioParams['rucio_host']
             rucioToken, _tokenValidity = getRucioToken(rucioAuthUrl, self.rucioAccount)
@@ -77,72 +80,74 @@
            - empty ruleIds list; and
            - empty currentRSEs; and
            document has been deactivated for a while (deactivatedOn=XXX),
         2. For those documents which are fetched make delete call to backend database
 
         :param timeThreshold: time threshold in days which will determine document clean-up readiness
         """
+        self.logger.info("====> Executing cleanupTask method...")
         spec = {'active': False}
         docs = self.mgr.getPileup(spec)
         deleteDocs = 0
         seconds = cleanupDaysThreshold * 24 * 60 * 60  # convert to second
         for doc in docs:
             if not doc['ruleIds'] and not doc['currentRSEs'] and \
-                    doc['deactivatedOn'] + seconds > time.time():
+                    time.time() > doc['deactivatedOn'] + seconds:
                 spec = {'pileupName': doc['pileupName']}
-                self.logger.info("Cleanup task delete pileup %s", doc['pileupName'])
-                self.mgr.deletePileup(spec)
-                deleteDocs += 1
+                if not self.dryRun:
+                    self.logger.info("Cleanup task deleting pileup %s", doc['pileupName'])
+                    self.mgr.deletePileup(spec)
+                    deleteDocs += 1
+                else:
+                    self.logger.info(f"DRY-RUN: should have deleted pileup document for {doc['pileupName']}")
         self.logger.info("Cleanup task deleted %d pileup objects", deleteDocs)
 
     def cmsMonitTask(self):
         """
         Execute CMS MONIT task according to the following logic:
 
         1. Read all pileup document from MongoDB
         2. Flatten all docs
         3. Submit flatten docs to CMS MONIT
         """
+        self.logger.info("====> Executing cmsMonitTask method...")
         if not self.monitManager.userAMQ or not self.monitManager.passAMQ:
             self.logger.info("MSPileupMonitoring has no AMQ credentials, will skip the upload to MONIT")
             return
-        startTime = time.time()
         spec = {}
         msPileupDocs = self.mgr.getPileup(spec)
         docs = []
         for doc in msPileupDocs:
             for flatDoc in flatDocuments(doc):
                 docs.append(flatDoc)
         results = self.monitManager.uploadToAMQ(docs)
-        endTime = time.time()
-        elapsedTime = endTime - startTime
         if results and isinstance(results, dict):
             success = results['success']
             failures = results['failures']
             msg = f"MSPileup CMS MONIT task fetched {len(msPileupDocs)} docs from MSPileup backend DB"
             msg += f", and sent {len(docs)} flatten docs to MONIT"
             msg += f", number of success docs {success} and failures {failures},"
-            msg += " in %.2f secs" % elapsedTime
             self.logger.info(msg)
         else:
-            self.logger.error("MSPileup CMS MONIT task failed, execution time %.2f secs", elapsedTime)
+            self.logger.error("MSPileup CMS MONIT task failed!")
 
     def monitoringTask(self):
         """
         Execute Monitoring task according to the following logic:
 
         1. Read pileup document from MongoDB with filter active=true
         2. For each rule id in ruleIds:
            - query Rucio for that rule id and fetch its state (e.g.: afd122143kjmdskj)
            - if state=OK, log that the rule has been satisfied and add that RSE to
            the currentRSEs (unique)
            - otherwise, calculate the rule completion based on the 3 locks_* field
         3. now that all the known rules have been inspected, persist the up-to-date
         pileup doc in MongoDB
         """
+        self.logger.info("====> Executing monitoringTask method...")
         spec = {'active': True}
         docs = self.mgr.getPileup(spec)
         taskSpec = self.getTaskSpec()
         self.logger.info("Running the monitoring task on %d pileup objects", len(docs))
         asyncio.run(performTasks('monitoring', docs, taskSpec))
 
     def inactiveTask(self):
@@ -163,14 +168,15 @@
              from currentRSEs (if any)
         3. make a log record if the DID + Rucio account tuple does not have any
         existent rules
            - and set ruleIds and currentRSEs to an empty list
         4. once all the relevant rules have been removed, persist an up-to-date
         version of the pileup data structure in MongoDB
         """
+        self.logger.info("====> Executing inactiveTask method...")
         spec = {'active': False}
         docs = self.mgr.getPileup(spec)
         taskSpec = self.getTaskSpec()
         self.logger.info("Running the inactive task on %d pileup objects", len(docs))
         asyncio.run(performTasks('inactive', docs, taskSpec))
 
     def activeTask(self, marginSpace=1024**4):
@@ -204,14 +210,15 @@
            - in case there is enough space, make a Rucio rule for
            that DID + Rucio account + RSE
              - now append the rule id to the ruleIds list
         6. once all the relevant rules have been created,
         or if there was any changes to the pileup object,
         persist an up-to-date version of the pileup data structure in MongoDB
         """
+        self.logger.info("====> Executing activeTask method...")
         spec = {'active': True}
         docs = self.mgr.getPileup(spec)
         taskSpec = self.getTaskSpec()
         taskSpec['marginSpace'] = marginSpace
         self.logger.info("Running the active task on %d pileup objects", len(docs))
         asyncio.run(performTasks('active', docs, taskSpec))
 
@@ -279,14 +286,22 @@
             for rse in rses:
                 if rse in doc['currentRSEs']:
                     doc['currentRSEs'].remove(rse)
                     modify = True
                     msg = f"delete rse {rse} from currentRSEs"
                     report.addEntry('monitoring', uuid, msg)
 
+        # now keep track of this rule id in the pileup document
+        for rse in rses:
+            if rse in doc['expectedRSEs'] and rid not in doc['ruleIds']:
+                logger.info(f"Tracking rule id {rid} that was not created by MSPileup")
+                doc['ruleIds'].append(rid)
+                modify = True
+                break
+
     # persist an up-to-date version of the pileup data structure in MongoDB
     if modify:
         logger.info(f"monitoring task {uuid}, update {pname}")
         mgr.updatePileup(doc, validate=False)
         msg = f"update pileup {pname}"
         report.addEntry('monitoring', uuid, msg)
     else:
@@ -302,26 +317,31 @@
     """
     mgr = spec['manager']
     uuid = spec['uuid']
     rucioClient = spec['rucioClient']
     rucioAccount = spec['rucioAccount']
     report = spec['report']
     logger = spec['logger']
+    dryRun = spec['dryRun']
     pname = doc['pileupName']
     kwargs = {'scope': 'cms', 'account': rucioAccount}
     rules = rucioClient.listDataRules(pname, **kwargs)
     modify = False
 
     for rdoc in rules:
         # make a Rucio call to delete that rule id
         rid = rdoc['id']
         msg = f"inactive task {uuid}, container: {pname} for Rucio account {rucioAccount}"
         msg += f", delete replication rule {rid}"
         logger.info(msg)
-        rucioClient.deleteRule(rid)
+        if not dryRun:
+            rucioClient.deleteRule(rid)
+        else:
+            logger.info(f"DRY-RUN: rule id '{rid}' should have been deleted.")
+            continue
         rses = rucioClient.evaluateRSEExpression(rdoc['rse_expression'])
 
         # remove the rule id from ruleIds (if any) and remove the RSE name from currentRSEs (if any)
         if rid in doc['ruleIds']:
             doc['ruleIds'].remove(rid)
             modify = True
             msg = f"remove rid {rid}"
@@ -396,14 +416,16 @@
             rses = rdoc['rses']
             for rse in rses:
                 # if rule RSE is not in expectedRSEs, then this rule needs to be deleted
                 if rse not in expectedRSEs:
                     # upon successful rule deletion, also remove the RSE name from currentRSEs
                     if not dryRun:
                         rucioClient.deleteRule(rid)
+                    else:
+                        logger.info(f"DRY-RUN: rule id '{rid}' should have been deleted.")
                     if rse in doc['currentRSEs']:
                         doc['currentRSEs'].remove(rse)
                         modify = True
                     msg = f"rse {rse} rule is deleted and remove from currentRSEs of {pname}"
                     logger.info(msg)
                     # delete rid in ruleIds (if any)
                     if rid in doc['ruleIds']:
@@ -433,17 +455,20 @@
                     enoughSpace = True
                     break
             dids = [inputArgs]
             if enoughSpace:
                 msg = f"active task {uuid}, for dids {dids} there is enough space at RSE {rse}"
                 logger.warning(msg)
                 # create the rule and append the rule id to ruleIds
-                if dryRun:
+                if not dryRun:
+                    rids = rucioClient.createReplicationRule(pname, rse, **kwargs)
+                else:
+                    msg = f"DRY-RUN: rule for pileup {pname} and rse {rse} should have been created"
+                    logger.info(msg)
                     continue
-                rids = rucioClient.createReplicationRule(pname, rse, **kwargs)
                 # add new ruleId to document ruleIds
                 for rid in rids:
                     if rid not in doc['ruleIds']:
                         doc['ruleIds'].append(rid)
                         modify = True
             else:
                 # make a log record saying that there is not enough space
```

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/Data.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/Data.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Service/RestApiHub.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Service/RestApiHub.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/Common.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/Common.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/Tools/PycurlRucio.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/Tools/PycurlRucio.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/MicroService/WebGui/FrontPage.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/MicroService/WebGui/FrontPage.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Auth.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Auth.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/CherryPyPeriodicTask.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/CherryPyPeriodicTask.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Error.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Error.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Format.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Format.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/HeartbeatMonitorBase.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/HeartbeatMonitorBase.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Main.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Main.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Server.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Server.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Services.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Services.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Test.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Test.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Tools.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Tools.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/REST/Validation.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/REST/Validation.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/ReqMgr/DataStructs/RequestStatus.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/ReqMgr/DataStructs/RequestStatus.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/AlertManager/AlertManagerAPI.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/AlertManager/AlertManagerAPI.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/CRIC/CRIC.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/CRIC/CRIC.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBS3Reader.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBS3Reader.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSErrors.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSErrors.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSReader.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSReader.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/DBSWriterObjects.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/DBSWriterObjects.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/DBS/ProdException.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/DBS/ProdException.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/FWJRDB/FWJRDBAPI.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/FWJRDB/FWJRDBAPI.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/HTTPS/HTTPSAuthHandler.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/HTTPS/HTTPSAuthHandler.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDB.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDB.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDBBackend.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDBBackend.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/LogDB/LogDBReport.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/LogDB/LogDBReport.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/McM/McM.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/McM/McM.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/MonIT/Grafana.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/MonIT/Grafana.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/PyCondorAPI.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/PyCondorAPI.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/PyCondor/PyCondorUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/PyCondor/PyCondorUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgr/ReqMgr.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgr/ReqMgr.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/ReqMgrAux/ReqMgrAux.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/ReqMgrAux/ReqMgrAux.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/RequestDBReader.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/RequestDBReader.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RequestDB/RequestDBWriter.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RequestDB/RequestDBWriter.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Requests.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Requests.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/Rucio.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/Rucio.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Rucio/RucioUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Rucio/RucioUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/RucioConMon/RucioConMon.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/RucioConMon/RucioConMon.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/Service.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/Service.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/TagCollector.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/TagCollector.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/TagCollector/XMLUtils.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/TagCollector/XMLUtils.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/UserFileCache/UserFileCache.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/UserFileCache/UserFileCache.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMAgent/WMAgent.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMAgent/WMAgent.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/DataMap.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/DataMap.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMArchive/WMArchive.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMArchive/WMArchive.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMBS/WMBS.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMBS/WMBS.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/DataStruct/RequestInfoCollection.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/DataStruct/RequestInfoCollection.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/WMStatsReader.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/WMStatsReader.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStats/WMStatsWriter.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStats/WMStatsWriter.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WMStatsServer/WMStatsServer.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WMStatsServer/WMStatsServer.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/WorkQueue/WorkQueue.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/WorkQueue/WorkQueue.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Services/pycurl_manager.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Services/pycurl_manager.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMBase.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMBase.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMConnectionBase.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMConnectionBase.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMException.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMException.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMExceptions.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMExceptions.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMFactory.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMFactory.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMInit.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMInit.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/WMLogging.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/WMLogging.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py` & `reqmgr2ms-pileup-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py`

 * *Files identical despite different names*

### Comparing `reqmgr2ms-pileup-2.2.0rc9/src/python/reqmgr2ms_pileup.egg-info/SOURCES.txt` & `reqmgr2ms-pileup-2.2.1rc1/src/python/reqmgr2ms_pileup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

