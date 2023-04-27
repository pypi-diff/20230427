# Comparing `tmp/ZEVIT_AIH_SDK-0.5.8.tar.gz` & `tmp/ZEVIT_AIH_SDK-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ZEVIT_AIH_SDK-0.5.8.tar", last modified: Sun Oct 30 13:03:34 2022, max compression
+gzip compressed data, was "dist/ZEVIT_AIH_SDK-0.5.9.tar", last modified: Mon Nov  7 13:35:16 2022, max compression
```

## Comparing `ZEVIT_AIH_SDK-0.5.8.tar` & `ZEVIT_AIH_SDK-0.5.9.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-10-30 13:03:33.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-10-30 13:03:33.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-30 13:03:33.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2632 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3114 2022-10-30 13:03:33.000000 ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/
--rw-r--r--   0 vsts      (1001) docker     (121)      177 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Population.py
--rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Category.py
--rw-r--r--   0 vsts      (1001) docker     (121)      327 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Mitigation.py
--rw-r--r--   0 vsts      (1001) docker     (121)      330 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/PopulationItem.py
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/PropertyDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (121)      165 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Risk.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      203 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/RiskAssessmentTechnique.py
--rw-r--r--   0 vsts      (1001) docker     (121)      889 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Classification.py
--rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/RisksObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/RiskAssessmentResult.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/
--rw-r--r--   0 vsts      (1001) docker     (121)     1159 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/WorkItem.py
--rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Category.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3089 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Media.py
--rw-r--r--   0 vsts      (1001) docker     (121)      192 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/MaintenanceObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2355 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Activity.py
--rw-r--r--   0 vsts      (1001) docker     (121)      199 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Deviation.py
--rw-r--r--   0 vsts      (1001) docker     (121)      209 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/MediaReference.py
--rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/PropertyDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (121)      919 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Classification.py
--rw-r--r--   0 vsts      (1001) docker     (121)      609 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/
--rw-r--r--   0 vsts      (1001) docker     (121)      194 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/DataType.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4442 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/File.py
--rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/DataUploadObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2868 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/v2Object.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/
--rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/MainSystem.py
--rw-r--r--   0 vsts      (1001) docker     (121)      189 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/Equipment.py
--rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/AssetsObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      182 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/Plant.py
--rw-r--r--   0 vsts      (1001) docker     (121)      154 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/
--rw-r--r--   0 vsts      (1001) docker     (121)     2044 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/AssignedElement.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4065 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Media.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/WorkorderItem.py
--rw-r--r--   0 vsts      (1001) docker     (121)      984 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/ApplierLanguage.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1142 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Annotation.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1000 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/MediaReference.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2363 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Assessment.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1241 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/PanoramaImage.py
--rw-r--r--   0 vsts      (1001) docker     (121)      978 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/PanoramicTour.py
--rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Failure.py
--rw-r--r--   0 vsts      (1001) docker     (121)      691 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/
--rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/IdentityObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/User.py
--rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/Role.py
--rw-r--r--   0 vsts      (1001) docker     (121)      119 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Identity/Team.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20017 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Object.py
--rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/AIHExceptions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13453 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/AIHClient.py
--rw-r--r--   0 vsts      (1001) docker     (121)      860 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/v1Object.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/
--rw-r--r--   0 vsts      (1001) docker     (121)      179 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Model.py
--rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Category.py
--rw-r--r--   0 vsts      (1001) docker     (121)      788 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Monitor.py
--rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/PropertyDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/MonitorsObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      904 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Classification.py
--rw-r--r--   0 vsts      (1001) docker     (121)      435 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      814 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/ModelDefinition.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/
--rw-r--r--   0 vsts      (1001) docker     (121)     2364 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/JobConfiguration.py
--rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/DataProcessingObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      199 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/Job.py
--rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/JobDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (121)      179 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/
--rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/ChannelType.py
--rw-r--r--   0 vsts      (1001) docker     (121)      203 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/ChannelAvailability.py
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/Signal.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1149 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/Channel.py
--rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/SignalsObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/DataOrigin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      287 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/
--rw-r--r--   0 vsts      (1001) docker     (121)     1170 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Schema.py
--rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/DesignationsObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Design.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1304 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Structure.py
--rw-r--r--   0 vsts      (1001) docker     (121)      245 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)       63 2022-10-30 13:02:50.000000 ZEVIT_AIH_SDK-0.5.8/AIH_SDK/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3114 2022-10-30 13:03:34.000000 ZEVIT_AIH_SDK-0.5.8/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     2663 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     3114 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/
+-rw-r--r--   0 vsts      (1001) docker     (121)      177 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Population.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Category.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      327 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Mitigation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      330 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/PopulationItem.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/PropertyDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      165 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Risk.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      203 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/RiskAssessmentTechnique.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      889 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Classification.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/RisksObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/RiskAssessmentResult.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1159 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/WorkItem.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Category.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3089 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Media.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      192 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/MaintenanceObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2355 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Activity.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      199 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Deviation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      209 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/MediaReference.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/PropertyDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      919 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Classification.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      609 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/
+-rw-r--r--   0 vsts      (1001) docker     (121)      194 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/DataType.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4442 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/File.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/DataUploadObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2868 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/v2Object.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/
+-rw-r--r--   0 vsts      (1001) docker     (121)      196 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/Organization.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/MainSystem.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      189 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/Equipment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/AssetsObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      182 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/Plant.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      213 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2044 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/AssignedElement.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4065 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Media.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/WorkorderItem.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      984 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/ApplierLanguage.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1142 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1000 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/MediaReference.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2363 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Assessment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1241 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/PanoramaImage.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      978 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/PanoramicTour.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Failure.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      691 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/
+-rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/IdentityObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/User.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/Role.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      119 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Identity/Team.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20017 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Object.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/AIHExceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13423 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/AIHClient.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      860 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/v1Object.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/
+-rw-r--r--   0 vsts      (1001) docker     (121)      179 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Model.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Category.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      788 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/PropertyDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/MonitorsObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      904 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Classification.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      435 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      752 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/ModelDefinition.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2364 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/JobConfiguration.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/DataProcessingObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      199 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/Job.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/JobDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      179 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/
+-rw-r--r--   0 vsts      (1001) docker     (121)      186 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/ChannelType.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      203 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/ChannelAvailability.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/Signal.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1149 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/Channel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      188 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/SignalsObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/DataOrigin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      287 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1170 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Schema.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/DesignationsObject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Design.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1304 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Structure.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      245 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       63 2022-11-07 13:34:34.000000 ZEVIT_AIH_SDK-0.5.9/AIH_SDK/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3114 2022-11-07 13:35:16.000000 ZEVIT_AIH_SDK-0.5.9/PKG-INFO
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/SOURCES.txt` & `ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 AIH_SDK/Object.py
 AIH_SDK/__init__.py
 AIH_SDK/v1Object.py
 AIH_SDK/v2Object.py
 AIH_SDK/Assets/AssetsObject.py
 AIH_SDK/Assets/Equipment.py
 AIH_SDK/Assets/MainSystem.py
+AIH_SDK/Assets/Organization.py
 AIH_SDK/Assets/Plant.py
 AIH_SDK/Assets/__init__.py
 AIH_SDK/DataProcessing/DataProcessingObject.py
 AIH_SDK/DataProcessing/Job.py
 AIH_SDK/DataProcessing/JobConfiguration.py
 AIH_SDK/DataProcessing/JobDefinition.py
 AIH_SDK/DataProcessing/__init__.py
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/ZEVIT_AIH_SDK.egg-info/PKG-INFO` & `ZEVIT_AIH_SDK-0.5.9/ZEVIT_AIH_SDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZEVIT-AIH-SDK
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python SDK to connect with ZEVIT Asset Integrity Hub
 Home-page: UNKNOWN
 Author: Mikkel Schmidt
 Author-email: sebastian.hansen@zevit.net
 License: UNKNOWN
 Description: # Introduction 
         This project makes it possible to easily interact with the objects in ZEVIT's Asset Integrity Hub.
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/setup.cfg` & `ZEVIT_AIH_SDK-0.5.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ZEVIT_AIH_SDK
-version = 0.5.8
+version = 0.5.9
 author = Mikkel Schmidt
 author_email = sebastian.hansen@zevit.net
 description = Python SDK to connect with ZEVIT Asset Integrity Hub
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/README.md` & `ZEVIT_AIH_SDK-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/Classification.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/Classification.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Risks/__init__.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Risks/__init__.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/WorkItem.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/WorkItem.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Media.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Media.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Activity.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Activity.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/Classification.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/Classification.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Maintenance/__init__.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataUpload/File.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataUpload/File.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/v2Object.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/v2Object.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Assets/MainSystem.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Assets/MainSystem.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/AssignedElement.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/AssignedElement.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Media.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Media.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/WorkorderItem.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/WorkorderItem.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/ApplierLanguage.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/ApplierLanguage.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Annotation.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Annotation.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/MediaReference.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/MediaReference.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Assessment.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Assessment.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/PanoramaImage.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/PanoramaImage.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/PanoramicTour.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/PanoramicTour.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/Failure.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/Failure.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Workitems/__init__.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Workitems/__init__.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Object.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Object.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/AIHClient.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/AIHClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         OUT: response (json) - A json object for the response
         """
         
         if(self._is_expired()):
             self._update_token()
         
         if parameters:
-            print(parameters)
             params = '&'.join([f'{k}={v}' for k,v in parameters])
             url = f'https://{self.environment}-{api}-{self.location}-api.azurewebsites.net/{endpoint}?{params}'   
         else:
             url = f'https://{self.environment}-{api}-{self.location}-api.azurewebsites.net/{endpoint}'
         
         response = self.client.get(url)
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/v1Object.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/v1Object.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Monitor.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Monitor.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/Classification.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/Classification.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Monitors/ModelDefinition.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Monitors/ModelDefinition.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,9 +13,8 @@
             return super().get(parameters=parameters)
         elif not version:
             return self._client._get(self._api, f'{self._endpoint}/{name}/versions')
         else:
             return self._client._get(self._api, f'{self._endpoint}/{name}/versions/{version}')
     
     def delete(self, name: str=None, version: str=None, parameters: dict={}):
-        #print(f'{self._endpoint}/{name}/versions/{version}')
         return self._client._delete(self._api, f'{self._endpoint}/{name}/versions/{version}')
```

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/DataProcessing/JobConfiguration.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/DataProcessing/JobConfiguration.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/Signal.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/Signal.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Signals/Channel.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Signals/Channel.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Schema.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Schema.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Design.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Design.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/AIH_SDK/Designations/Structure.py` & `ZEVIT_AIH_SDK-0.5.9/AIH_SDK/Designations/Structure.py`

 * *Files identical despite different names*

### Comparing `ZEVIT_AIH_SDK-0.5.8/PKG-INFO` & `ZEVIT_AIH_SDK-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZEVIT_AIH_SDK
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python SDK to connect with ZEVIT Asset Integrity Hub
 Home-page: UNKNOWN
 Author: Mikkel Schmidt
 Author-email: sebastian.hansen@zevit.net
 License: UNKNOWN
 Description: # Introduction 
         This project makes it possible to easily interact with the objects in ZEVIT's Asset Integrity Hub.
```

