# Comparing `tmp/base_system-0.1.0.tar.gz` & `tmp/base_system-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.1.0.tar", last modified: Mon Feb 13 11:31:34 2023, max compression
+gzip compressed data, was "base_system-0.1.2.tar", last modified: Thu Apr 27 03:06:20 2023, max compression
```

## Comparing `base_system-0.1.0.tar` & `base_system-0.1.2.tar`

### file list

```diff
@@ -1,124 +1,53 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.293878 base_system-0.1.0/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.0/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.0/.pypirc
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.0/Dockerfile
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.245850 base_system-0.1.0/Infrastructure/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.0/Infrastructure/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      405 2023-01-04 05:32:12.000000 base_system-0.1.0/Infrastructure/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11815 2023-01-07 01:27:46.000000 base_system-0.1.0/Infrastructure/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      909 2023-01-04 06:34:47.000000 base_system-0.1.0/Infrastructure/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      405 2023-01-04 05:32:12.000000 base_system-0.1.0/Infrastructure/wsgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.0/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.0/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1193 2023-02-13 11:31:34.289876 base_system-0.1.0/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      783 2023-02-07 05:38:34.000000 base_system-0.1.0/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.245850 base_system-0.1.0/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.249852 base_system-0.1.0/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      144 2023-01-04 06:08:43.000000 base_system-0.1.0/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      185 2023-01-04 06:08:44.000000 base_system-0.1.0/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3138 2023-01-04 06:32:37.000000 base_system-0.1.0/base_system/__pycache__/appointment_ser.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      430 2023-01-04 06:08:43.000000 base_system-0.1.0/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    17093 2023-02-13 11:25:43.000000 base_system-0.1.0/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14345 2023-02-08 05:49:25.000000 base_system-0.1.0/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      185 2023-01-04 06:08:44.000000 base_system-0.1.0/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2770 2023-02-07 05:42:26.000000 base_system-0.1.0/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    21077 2023-02-13 11:25:44.000000 base_system-0.1.0/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1945 2023-01-04 06:32:34.000000 base_system-0.1.0/base_system/appointment_ser.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.249852 base_system-0.1.0/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    35282 2023-02-13 11:29:52.000000 base_system-0.1.0/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.285873 base_system-0.1.0/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      940 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0002_auto_20220908_1631.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      568 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0003_auto_20220909_1628.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      697 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0004_auto_20220909_1636.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1087 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0005_auto_20220913_1022.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     4015 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0006_auto_20220915_1130.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      656 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0007_alter_user_name.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1770 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0008_auto_20220916_0952.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      806 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0009_positiontitle_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      665 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0010_alter_expensestandard_fees.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      660 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0011_alter_expensestandard_fees.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      573 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0012_remove_expensestandard_fees.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      653 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0013_expensestandard_fees.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1303 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0014_doctorexpensestandard.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1419 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0015_auto_20220919_1028.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      733 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0016_auto_20220919_1057.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      672 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0017_doctor_is_online_consult.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      758 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0018_user_doctor.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1273 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0019_imagesupload.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      822 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0020_auto_20220923_1439.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      801 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0021_auto_20220923_1443.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      828 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0022_auto_20220926_1023.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2010 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0023_auto_20220927_0937.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2214 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0024_auto_20220927_1018.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      752 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0025_auto_20221012_1514.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      532 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0026_delete_imagesupload.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1412 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0027_inspectiondictionaries.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1418 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0028_examinationdictionaries.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      757 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0029_auto_20221031_1559.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      748 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0030_auto_20221109_1700.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2236 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0030_drugcategory_drugdirectory_drugpreparationtype.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      636 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0031_rename_drug_cod_drugdirectory_drug_code.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      533 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0032_merge_20221110_1143.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      807 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0033_drugdirectory_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1745 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0034_pharmacymanagement_pharmacytype.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      829 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0035_pharmacymanagement_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1597 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0036_auto_20221114_1059.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2245 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0037_pharmacydrug.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1112 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0038_drugtype.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      860 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0039_auto_20221115_1055.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      766 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0040_auto_20221213_0914.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      806 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0041_auto_20221213_1706.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      949 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0042_auto_20221214_1431.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      662 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0043_alter_hospital_logo.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      694 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0044_alter_hospital_hos_images.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      767 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/migrations/__pycache__/0045_auto_20221216_1107.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      155 2023-01-04 06:08:44.000000 base_system-0.1.0/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23840 2023-02-13 10:35:49.000000 base_system-0.1.0/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    12145 2023-02-07 06:55:34.000000 base_system-0.1.0/base_system/serializers.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.285873 base_system-0.1.0/base_system/serializers_folder/
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.289876 base_system-0.1.0/base_system/serializers_folder/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     7018 2023-01-04 06:08:45.000000 base_system-0.1.0/base_system/serializers_folder/__pycache__/group_serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3920 2023-01-04 06:08:45.000000 base_system-0.1.0/base_system/serializers_folder/__pycache__/permission_serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     5337 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/serializers_folder/group_serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2416 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/serializers_folder/permission_serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3398 2023-02-07 03:20:23.000000 base_system-0.1.0/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    34275 2023-02-10 08:31:13.000000 base_system-0.1.0/base_system/views.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.289876 base_system-0.1.0/base_system/viewset/
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.289876 base_system-0.1.0/base_system/viewset/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3485 2023-01-04 06:32:37.000000 base_system-0.1.0/base_system/viewset/__pycache__/appointment_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     8020 2023-01-04 06:08:45.000000 base_system-0.1.0/base_system/viewset/__pycache__/group_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3028 2023-01-04 06:08:45.000000 base_system-0.1.0/base_system/viewset/__pycache__/permission_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3701 2023-01-04 06:10:19.000000 base_system-0.1.0/base_system/viewset/appointment_viewset.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11092 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/viewset/group_viewset.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2513 2023-01-04 05:21:26.000000 base_system-0.1.0/base_system/viewset/permission_viewset.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.249852 base_system-0.1.0/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1193 2023-02-13 11:31:34.000000 base_system-0.1.0/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     5541 2023-02-13 11:31:34.000000 base_system-0.1.0/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-02-13 11:31:34.000000 base_system-0.1.0/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-02-07 05:45:48.000000 base_system-0.1.0/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-02-13 11:31:34.000000 base_system-0.1.0/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       28 2023-02-13 11:31:34.000000 base_system-0.1.0/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.0/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      670 2023-01-04 05:32:12.000000 base_system-0.1.0/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.0/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      570 2023-01-04 05:32:12.000000 base_system-0.1.0/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-02-13 11:31:34.293878 base_system-0.1.0/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2630 2023-02-13 11:31:32.000000 base_system-0.1.0/setup.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.289876 base_system-0.1.0/work_scheduling/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-07 01:24:33.000000 base_system-0.1.0/work_scheduling/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2023-01-07 01:24:33.000000 base_system-0.1.0/work_scheduling/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      161 2023-01-07 01:24:33.000000 base_system-0.1.0/work_scheduling/apps.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-02-13 11:31:34.289876 base_system-0.1.0/work_scheduling/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    13013 2023-02-13 11:27:40.000000 base_system-0.1.0/work_scheduling/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-07 01:24:32.000000 base_system-0.1.0/work_scheduling/migrations/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     9137 2023-01-07 01:24:32.000000 base_system-0.1.0/work_scheduling/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    10338 2023-01-07 01:24:32.000000 base_system-0.1.0/work_scheduling/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       61 2023-01-07 01:24:32.000000 base_system-0.1.0/work_scheduling/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1895 2023-01-07 01:24:32.000000 base_system-0.1.0/work_scheduling/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23385 2023-02-11 05:38:12.000000 base_system-0.1.0/work_scheduling/views.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.2/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.2/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.048670 base_system-0.1.2/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.2/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.2/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11870 2023-04-27 02:20:00.000000 base_system-0.1.2/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.2/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.2/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.2/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.2/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.2/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1192 2023-04-27 03:06:20.052672 base_system-0.1.2/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.2/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.2/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.2/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.2/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.2/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19409 2023-04-27 02:20:02.000000 base_system-0.1.2/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.2/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.2/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.2/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    32530 2023-04-27 02:23:46.000000 base_system-0.1.2/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11937 2023-04-27 02:23:47.000000 base_system-0.1.2/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.2/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.2/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.2/base_system/auth.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39410 2023-04-27 03:00:20.000000 base_system-0.1.2/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.2/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.2/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25384 2023-04-26 09:07:35.000000 base_system-0.1.2/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.2/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.2/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.2/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    71863 2023-04-27 02:23:42.000000 base_system-0.1.2/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14977 2023-04-25 05:48:42.000000 base_system-0.1.2/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:06:20.052672 base_system-0.1.2/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1192 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1243 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-04-27 03:06:19.000000 base_system-0.1.2/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.2/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.2/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.2/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.2/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-04-27 03:06:20.052672 base_system-0.1.2/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2629 2023-04-27 03:05:05.000000 base_system-0.1.2/setup.py
```

### Comparing `base_system-0.1.0/.gitignore` & `base_system-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.1.0/Infrastructure/settings.py` & `base_system-0.1.2/BaseFunctionModule/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Django settings for Infrastructure project.
+Django settings for BaseFunctionModule project.
 
 Generated by 'django-admin startproject' using Django 4.1.1.
 
 For more information on this file, see
 https://docs.djangoproject.com/en/4.1/topics/settings/
 
 For the full list of settings and their values, see
@@ -40,15 +40,14 @@
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'corsheaders',  # 解决跨域
     'rest_framework',
     'django_filters',
     'base_system',
-    'work_scheduling',
 ]
 
 MIDDLEWARE = [
     'corsheaders.middleware.CorsMiddleware',  # 跨域问题解决
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
@@ -101,15 +100,15 @@
     'user-agent',
     'x-csrftoken',
     'x-requested-with',
     'Pragma',
 )
 
 
-ROOT_URLCONF = 'Infrastructure.urls'
+ROOT_URLCONF = 'BaseFunctionModule.urls'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': []
         ,
         'APP_DIRS': True,
@@ -120,21 +119,25 @@
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
             ],
         },
     },
 ]
 
-WSGI_APPLICATION = 'Infrastructure.wsgi.application'
+WSGI_APPLICATION = 'BaseFunctionModule.wsgi.application'
+
+
+# 回写院内ip地址
+WRITEBACK_IP = 'http://ycswjw.com:8041'
 
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql_psycopg2',
-        'NAME': 'infrasdb',
+        'NAME': 'medicaldb',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': 'localhost',
         'PORT': '5432'
     }
 }
```

### Comparing `base_system-0.1.0/LICENCE` & `base_system-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.1.0/PKG-INFO` & `base_system-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.1.0
-Summary: Medical system base data
+Version: 0.1.2
+Summary: Basic feature component
 Home-page: https://devcloud.huaweicloud.com/
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `base_system-0.1.0/README.rst` & `base_system-0.1.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 -----------
 
 1. Add "base_system" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...
         'base_system',
-        'work_scheduling',
     ]
 
 2. Include the polls URLconf in your project urls.py like this::
 
     path('base-system/', include('base_system.urls')),
 
 3. Run `python manage.py migrate` to create the polls models.
```

### Comparing `base_system-0.1.0/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.1.2/base_system/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 13 10:35:49 2023 UTC, .py size: 23840 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,1069 +1,1214 @@
-00000000: 610d 0d0a 0000 0000 8512 ea63 205d 0000  a..........c ]..
+00000000: 610d 0d0a 0000 0000 d7e9 4864 2863 0000  a.........Hd(c..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8001 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
-00000060: 5a08 4700 6406 6407 8400 6407 6507 6a09  Z.G.d.d...d.e.j.
-00000070: 8303 5a0a 4700 6408 6409 8400 6409 650a  ..Z.G.d.d...d.e.
-00000080: 8303 5a0b 4700 640a 640b 8400 640b 650a  ..Z.G.d.d...d.e.
-00000090: 8303 5a0c 4700 640c 640d 8400 640d 650a  ..Z.G.d.d...d.e.
-000000a0: 8303 5a0d 4700 640e 640f 8400 640f 650a  ..Z.G.d.d...d.e.
-000000b0: 8303 5a0e 4700 6410 6411 8400 6411 6502  ..Z.G.d.d...d.e.
-000000c0: 8303 5a0f 4700 6412 6413 8400 6413 6507  ..Z.G.d.d...d.e.
-000000d0: 6a09 8303 5a10 4700 6414 6415 8400 6415  j...Z.G.d.d...d.
-000000e0: 6507 6a09 8303 5a11 4700 6416 6417 8400  e.j...Z.G.d.d...
-000000f0: 6417 6507 6a09 8303 5a12 4700 6418 6419  d.e.j...Z.G.d.d.
-00000100: 8400 6419 650a 8303 5a13 4700 641a 641b  ..d.e...Z.G.d.d.
-00000110: 8400 641b 650a 8303 5a14 4700 641c 641d  ..d.e...Z.G.d.d.
-00000120: 8400 641d 650a 8303 5a15 4700 641e 641f  ..d.e...Z.G.d.d.
-00000130: 8400 641f 650a 8303 5a16 4700 6420 6421  ..d.e...Z.G.d d!
-00000140: 8400 6421 650a 8303 5a17 4700 6422 6423  ..d!e...Z.G.d"d#
-00000150: 8400 6423 650a 8303 5a18 4700 6424 6425  ..d#e...Z.G.d$d%
-00000160: 8400 6425 650a 8303 5a19 4700 6426 6427  ..d%e...Z.G.d&d'
-00000170: 8400 6427 650a 8303 5a1a 4700 6428 6429  ..d'e...Z.G.d(d)
-00000180: 8400 6429 650a 8303 5a1b 4700 642a 642b  ..d)e...Z.G.d*d+
-00000190: 8400 642b 650a 8303 5a1c 4700 642c 642d  ..d+e...Z.G.d,d-
-000001a0: 8400 642d 650a 8303 5a1d 6401 5300 292e  ..d-e...Z.d.S.).
-000001b0: e900 0000 004e 2902 da0c 4162 7374 7261  .....N)...Abstra
-000001c0: 6374 5573 6572 da05 4772 6f75 7029 01da  ctUser..Group)..
-000001d0: 0b43 6f6e 7465 6e74 5479 7065 2901 da06  .ContentType)...
-000001e0: 6d6f 6465 6c73 2902 2902 da01 3175 0300  models).)...1u..
-000001f0: 0000 e794 b729 02da 0130 7503 0000 00e5  .....)...0u.....
-00000200: a5b3 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000210: 0000 0005 0000 0040 0000 0073 4800 0000  .......@...sH...
-00000220: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00000230: 6402 6403 8d03 5a05 6503 6a04 6404 6402  d.d...Z.e.j.d.d.
-00000240: 6402 6405 8d03 5a06 6503 6a07 6406 6402  d.d...Z.e.j.d.d.
-00000250: 6407 8d02 5a08 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
-00000260: 8302 5a09 640a 5300 290b da10 4d65 6469  ..Z.d.S.)...Medi
-00000270: 6361 6c42 6173 654d 6f64 656c f50c 0000  calBaseModel....
-00000280: 00e5 889b e5bb bae6 97b6 e997 b454 a903  .............T..
-00000290: da0c 7665 7262 6f73 655f 6e61 6d65 da0c  ..verbose_name..
-000002a0: 6175 746f 5f6e 6f77 5f61 6464 da04 6e75  auto_now_add..nu
-000002b0: 6c6c f50c 0000 00e6 9bb4 e696 b0e6 97b6  ll..............
-000002c0: e997 b4a9 0372 0b00 0000 da08 6175 746f  .....r......auto
-000002d0: 5f6e 6f77 720d 0000 00f5 0c00 0000 e698  _nowr...........
-000002e0: afe5 90a6 e590 afe7 94a8 a902 720b 0000  ............r...
-000002f0: 00da 0764 6566 6175 6c74 6300 0000 0000  ...defaultc.....
-00000300: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000310: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000320: 6401 5a03 6402 5300 2903 7a15 4d65 6469  d.Z.d.S.).z.Medi
-00000330: 6361 6c42 6173 654d 6f64 656c 2e4d 6574  calBaseModel.Met
-00000340: 6154 4e29 04da 085f 5f6e 616d 655f 5fda  aTN)...__name__.
-00000350: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000360: 7561 6c6e 616d 655f 5fda 0861 6273 7472  ualname__..abstr
-00000370: 6163 74a9 0072 1800 0000 7218 0000 00fa  act..r....r.....
-00000380: 332f 686f 6d65 2f6c 7968 2f77 6f72 6b2f  3/home/lyh/work/
-00000390: 496e 6672 6173 7472 7563 7475 7265 2f62  Infrastructure/b
-000003a0: 6173 655f 7379 7374 656d 2f6d 6f64 656c  ase_system/model
-000003b0: 732e 7079 da04 4d65 7461 1200 0000 7302  s.py..Meta....s.
-000003c0: 0000 0008 0172 1a00 0000 4e29 0a72 1400  .....r....N).r..
-000003d0: 0000 7215 0000 0072 1600 0000 7205 0000  ..r....r....r...
-000003e0: 00da 0d44 6174 6554 696d 6546 6965 6c64  ...DateTimeField
-000003f0: da0c 6372 6561 7465 645f 7469 6d65 da0c  ..created_time..
-00000400: 7570 6461 7465 645f 7469 6d65 da0c 426f  updated_time..Bo
-00000410: 6f6c 6561 6e46 6965 6c64 da09 6973 5f61  oleanField..is_a
-00000420: 6374 6976 6572 1a00 0000 7218 0000 0072  ctiver....r....r
-00000430: 1800 0000 7218 0000 0072 1900 0000 7208  ....r....r....r.
-00000440: 0000 000d 0000 0073 0800 0000 0801 1001  .......s........
-00000450: 1001 0e02 7208 0000 0063 0000 0000 0000  ....r....c......
-00000460: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-00000470: 0000 73d8 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-00000480: 036a 0464 0164 0264 038d 025a 0565 036a  .j.d.d.d...Z.e.j
-00000490: 0464 0464 0564 0664 0664 078d 045a 0665  .d.d.d.d.d...Z.e
-000004a0: 036a 0764 0864 0664 0664 098d 035a 0865  .j.d.d.d.d...Z.e
-000004b0: 036a 0464 0264 0a64 0664 0b8d 035a 0965  .j.d.d.d.d...Z.e
-000004c0: 036a 0764 0c64 0d8d 015a 0a65 036a 0b64  .j.d.d...Z.e.j.d
-000004d0: 0e64 0d8d 015a 0c65 036a 0b64 0f64 0d8d  .d...Z.e.j.d.d..
-000004e0: 015a 0d65 036a 0e64 1064 1165 036a 0f64  .Z.e.j.d.d.e.j.d
-000004f0: 0664 128d 045a 1065 036a 0464 1364 0564  .d...Z.e.j.d.d.d
-00000500: 1464 0664 158d 045a 1165 036a 0464 1664  .d.d...Z.e.j.d.d
-00000510: 0564 1764 188d 035a 1265 036a 0464 1964  .d.d...Z.e.j.d.d
-00000520: 0564 0664 0664 078d 045a 1365 036a 0464  .d.d.d...Z.e.j.d
-00000530: 1a64 0564 0664 0664 078d 045a 1447 0064  .d.d.d.d...Z.G.d
-00000540: 1b64 1c84 0064 1c83 025a 1564 1d53 0029  .d...d...Z.d.S.)
-00000550: 1eda 0848 6f73 7069 7461 6cf5 0600 0000  ...Hospital.....
-00000560: e590 8de7 a7b0 e9ff 0000 00a9 0272 0b00  .............r..
-00000570: 0000 da0a 6d61 785f 6c65 6e67 7468 f50c  ....max_length..
-00000580: 0000 00e8 8194 e7b3 bbe6 96b9 e5bc 8fe9  ................
-00000590: 6400 0000 54a9 0472 0b00 0000 7224 0000  d...T..r....r$..
-000005a0: 0072 0d00 0000 da05 626c 616e 6b75 0c00  .r......blanku..
-000005b0: 0000 e58c bbe9 99a2 e7ae 80e4 bb8b a903  ................
-000005c0: 720b 0000 0072 0d00 0000 7228 0000 00f5  r....r....r(....
-000005d0: 0600 0000 e7bc 96e7 a081 a903 7224 0000  ............r$..
-000005e0: 0072 0b00 0000 da06 756e 6971 7565 750c  .r......uniqueu.
-000005f0: 0000 00e5 8cbb e999 a2e5 9cb0 e59d 8029  ...............)
-00000600: 0172 0b00 0000 7506 0000 00e7 bb8f e5ba  .r....u.........
-00000610: a675 0600 0000 e7bb b4e5 baa6 da04 7365  .u............se
-00000620: 6c66 f50c 0000 00e6 8980 e5b1 9ee5 8cbb  lf..............
-00000630: e999 a2a9 0372 0b00 0000 da09 6f6e 5f64  .....r......on_d
-00000640: 656c 6574 6572 0d00 0000 750c 0000 00e5  eleter....u.....
-00000650: 8cbb e999 a2e5 9bbe e789 875a 0f68 6f73  ...........Z.hos
-00000660: 7069 7461 6c5f 696d 6167 6573 2904 720b  pital_images).r.
-00000670: 0000 0072 2400 0000 7213 0000 0072 2800  ...r$...r....r(.
-00000680: 0000 da04 6c6f 676f 5a0d 686f 7370 6974  ....logoZ.hospit
-00000690: 616c 5f6c 6f67 6fa9 0372 0b00 0000 7224  al_logo..r....r$
-000006a0: 0000 0072 1300 0000 f509 0000 00e5 889b  ...r............
-000006b0: e5bb bae4 baba f509 0000 00e6 9bb4 e696  ................
-000006c0: b0e4 baba 6300 0000 0000 0000 0000 0000  ....c...........
-000006d0: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
-000006e0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000006f0: 5a04 6504 5a05 6403 5300 2904 7a0d 486f  Z.e.Z.d.S.).z.Ho
-00000700: 7370 6974 616c 2e4d 6574 615a 0b62 735f  spital.MetaZ.bs_
-00000710: 686f 7370 6974 616c 7509 0000 00e5 8cbb  hospitalu.......
-00000720: e999 a2e8 a1a8 4ea9 0672 1400 0000 7215  ......N..r....r.
-00000730: 0000 0072 1600 0000 da08 6462 5f74 6162  ...r......db_tab
-00000740: 6c65 720b 0000 00da 1376 6572 626f 7365  ler......verbose
-00000750: 5f6e 616d 655f 706c 7572 616c 7218 0000  _name_pluralr...
-00000760: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000770: 721a 0000 002b 0000 0073 0600 0000 0801  r....+...s......
-00000780: 0401 0401 721a 0000 004e 2916 7214 0000  ....r....N).r...
-00000790: 0072 1500 0000 7216 0000 0072 0500 0000  .r....r....r....
-000007a0: da09 4368 6172 4669 656c 64da 046e 616d  ..CharField..nam
-000007b0: 65da 0570 686f 6e65 da09 5465 7874 4669  e..phone..TextFi
-000007c0: 656c 64da 0969 6e74 726f 6475 6365 da07  eld..introduce..
-000007d0: 636f 6465 6e75 6dda 0761 6464 7265 7373  codenum..address
-000007e0: da0a 466c 6f61 7446 6965 6c64 5a09 6c6f  ..FloatFieldZ.lo
-000007f0: 6e67 6974 7564 655a 086c 6174 6974 7564  ngitudeZ.latitud
-00000800: 65da 0a46 6f72 6569 676e 4b65 79da 0743  e..ForeignKey..C
-00000810: 4153 4341 4445 da06 7061 7265 6e74 5a0a  ASCADE..parentZ.
-00000820: 686f 735f 696d 6167 6573 7231 0000 00da  hos_imagesr1....
-00000830: 0a63 7265 6174 6564 5f62 79da 0a75 7064  .created_by..upd
-00000840: 6174 6564 5f62 7972 1a00 0000 7218 0000  ated_byr....r...
-00000850: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000860: 7220 0000 0016 0000 0073 2400 0000 0801  r .......s$.....
-00000870: 0e01 1201 1001 1001 0c01 0c01 0c01 0401  ................
-00000880: 0201 0201 0401 02fc 0607 1202 1001 1201  ................
-00000890: 1202 7220 0000 0063 0000 0000 0000 0000  ..r ...c........
-000008a0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-000008b0: 73c8 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
-000008c0: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
-000008d0: 0464 0264 0564 0564 068d 045a 0665 036a  .d.d.d.d...Z.e.j
-000008e0: 0464 0764 0264 0564 0564 068d 045a 0765  .d.d.d.d.d...Z.e
-000008f0: 036a 0464 0864 0264 0564 098d 035a 0865  .j.d.d.d.d...Z.e
-00000900: 036a 0464 0a64 0b64 0564 0564 068d 045a  .j.d.d.d.d.d...Z
-00000910: 0965 036a 0a64 0c64 0564 0564 0d8d 035a  .e.j.d.d.d.d...Z
-00000920: 0b65 036a 0c65 0d64 0e65 036a 0e64 0f8d  .e.j.e.d.e.j.d..
-00000930: 035a 0f65 036a 0c64 1064 1165 036a 0e64  .Z.e.j.d.d.e.j.d
-00000940: 0564 128d 045a 1065 036a 0464 1364 0b64  .d...Z.e.j.d.d.d
-00000950: 0564 0564 068d 045a 1165 036a 0464 1464  .d.d...Z.e.j.d.d
-00000960: 0b64 0564 0564 068d 045a 1247 0064 1564  .d.d.d...Z.G.d.d
-00000970: 1684 0064 1683 025a 1364 1753 0029 18da  ...d...Z.d.S.)..
-00000980: 064f 6666 6963 6572 2100 0000 7222 0000  .Officer!...r"..
-00000990: 0072 2300 0000 750c 0000 00e7 a791 e5ae  .r#...u.........
-000009a0: a4e4 bd8d e7bd ae54 7227 0000 0072 2500  .......Tr'...r%.
-000009b0: 0000 f50c 0000 00e7 a791 e5ae a4e7 bc96  ................
-000009c0: e7a0 81a9 0372 0b00 0000 7224 0000 0072  .....r....r$...r
-000009d0: 2c00 0000 7506 0000 00e7 b1bb e59e 8b72  ,...u..........r
-000009e0: 2600 0000 750c 0000 00e7 a791 e5ae a4e7  &...u...........
-000009f0: ae80 e4bb 8b72 2900 0000 722e 0000 00a9  .....r)...r.....
-00000a00: 0272 0b00 0000 7230 0000 0072 2d00 0000  .r....r0...r-...
-00000a10: 750c 0000 00e4 b88a e7ba a7e7 a791 e5ae  u...............
-00000a20: a472 2f00 0000 7233 0000 0072 3400 0000  .r/...r3...r4...
-00000a30: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000a40: 0001 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
-00000a50: 5a01 6400 5a02 6401 5a03 6402 5a04 6504  Z.d.Z.d.Z.d.Z.e.
-00000a60: 5a05 6403 5300 2904 7a0b 4f66 6669 6365  Z.d.S.).z.Office
-00000a70: 2e4d 6574 615a 0962 735f 6f66 6669 6365  .MetaZ.bs_office
-00000a80: 7509 0000 00e7 a791 e5ae a4e8 a1a8 4e72  u.............Nr
-00000a90: 3500 0000 7218 0000 0072 1800 0000 7218  5...r....r....r.
-00000aa0: 0000 0072 1900 0000 721a 0000 0047 0000  ...r....r....G..
-00000ab0: 0073 0600 0000 0801 0401 0401 721a 0000  .s..........r...
-00000ac0: 004e 2914 7214 0000 0072 1500 0000 7216  .N).r....r....r.
-00000ad0: 0000 0072 0500 0000 7238 0000 0072 3900  ...r....r8...r9.
-00000ae0: 0000 723e 0000 0072 3a00 0000 723d 0000  ..r>...r:...r=..
-00000af0: 005a 0b6f 6666 6963 655f 7479 7065 723b  .Z.office_typer;
-00000b00: 0000 0072 3c00 0000 7240 0000 0072 2000  ...r<...r@...r .
-00000b10: 0000 7241 0000 00da 0868 6f73 7069 7461  ..rA.....hospita
-00000b20: 6c72 4200 0000 7243 0000 0072 4400 0000  lrB...rC...rD...
-00000b30: 721a 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000b40: 1800 0000 7219 0000 0072 4500 0000 3400  ....r....rE...4.
-00000b50: 0000 7326 0000 0008 010e 0112 0112 0110  ..s&............
-00000b60: 0112 0110 0104 0102 0102 0104 fd06 0506  ................
-00000b70: 0102 0104 0102 fd06 0412 0112 0272 4500  .............rE.
-00000b80: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000b90: 0000 0006 0000 0040 0000 0073 6e00 0000  .......@...sn...
-00000ba0: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00000bb0: 6403 8d02 5a05 6503 6a04 6404 6402 6405  d...Z.e.j.d.d.d.
-00000bc0: 6406 8d03 5a06 6503 6a07 6508 6407 6503  d...Z.e.j.e.d.e.
-00000bd0: 6a09 6408 8d03 5a0a 6503 6a04 6409 640a  j.d...Z.e.j.d.d.
-00000be0: 6405 6405 640b 8d04 5a0b 6503 6a04 640c  d.d.d...Z.e.j.d.
-00000bf0: 640a 6405 6405 640b 8d04 5a0c 4700 640d  d.d.d.d...Z.G.d.
-00000c00: 640e 8400 640e 8302 5a0d 640f 5300 2910  d...d...Z.d.S.).
-00000c10: da0d 506f 7369 7469 6f6e 5469 746c 6572  ..PositionTitler
-00000c20: 2100 0000 7222 0000 0072 2300 0000 750c  !...r"...r#...u.
-00000c30: 0000 00e8 818c e7a7 b0e7 bc96 e7a0 8154  ...............T
-00000c40: 7247 0000 0072 2e00 0000 7248 0000 0072  rG...r....rH...r
-00000c50: 3300 0000 7226 0000 0072 2700 0000 7234  3...r&...r'...r4
-00000c60: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000c70: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-00000c80: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00000c90: 0465 045a 0564 0353 0029 047a 1250 6f73  .e.Z.d.S.).z.Pos
-00000ca0: 6974 696f 6e54 6974 6c65 2e4d 6574 615a  itionTitle.MetaZ
-00000cb0: 1162 735f 706f 7369 7469 6f6e 5f74 6974  .bs_position_tit
-00000cc0: 6c65 7509 0000 00e8 818c e7a7 b0e8 a1a8  leu.............
-00000cd0: 4e72 3500 0000 7218 0000 0072 1800 0000  Nr5...r....r....
-00000ce0: 7218 0000 0072 1900 0000 721a 0000 0058  r....r....r....X
-00000cf0: 0000 0073 0600 0000 0801 0401 0401 721a  ...s..........r.
-00000d00: 0000 004e 290e 7214 0000 0072 1500 0000  ...N).r....r....
-00000d10: 7216 0000 0072 0500 0000 7238 0000 0072  r....r....r8...r
-00000d20: 3900 0000 723d 0000 0072 4000 0000 7220  9...r=...r@...r 
-00000d30: 0000 0072 4100 0000 7249 0000 0072 4300  ...rA...rI...rC.
-00000d40: 0000 7244 0000 0072 1a00 0000 7218 0000  ..rD...r....r...
-00000d50: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000d60: 724a 0000 004d 0000 0073 1400 0000 0801  rJ...M...s......
-00000d70: 0e01 1001 0401 0201 0201 04fd 0605 1201  ................
-00000d80: 1202 724a 0000 0063 0000 0000 0000 0000  ..rJ...c........
-00000d90: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
-00000da0: 7352 0100 0065 005a 0164 005a 0265 036a  sR...e.Z.d.Z.e.j
-00000db0: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
-00000dc0: 0464 0564 0664 0664 078d 045a 0665 036a  .d.d.d.d...Z.e.j
-00000dd0: 0464 0864 0564 0664 0664 078d 045a 0765  .d.d.d.d.d...Z.e
-00000de0: 036a 0464 0964 0264 0664 0664 078d 045a  .j.d.d.d.d.d...Z
-00000df0: 0865 036a 0464 0a64 0264 0664 0664 078d  .e.j.d.d.d.d.d..
-00000e00: 045a 0965 036a 0464 0b64 0564 0664 0664  .Z.e.j.d.d.d.d.d
-00000e10: 078d 045a 0a65 036a 0b65 0c64 0c65 036a  ...Z.e.j.e.d.e.j
-00000e20: 0d64 0d8d 035a 0e65 036a 0464 0e64 0f65  .d...Z.e.j.d.d.e
-00000e30: 0f64 0664 0664 108d 055a 1065 036a 0464  .d.d.d...Z.e.j.d
-00000e40: 1164 1264 0664 0664 078d 045a 1165 036a  .d.d.d.d...Z.e.j
-00000e50: 0464 1364 0564 0664 0664 078d 045a 1265  .d.d.d.d.d...Z.e
-00000e60: 036a 0b65 1364 1465 036a 0d64 0d8d 035a  .j.e.d.e.j.d...Z
-00000e70: 1465 036a 0b65 1564 1565 036a 0d64 0d8d  .e.j.e.d.e.j.d..
-00000e80: 035a 1665 036a 1764 1664 0664 0664 178d  .Z.e.j.d.d.d.d..
-00000e90: 035a 1865 036a 0464 1864 0564 1964 1a8d  .Z.e.j.d.d.d.d..
-00000ea0: 035a 1965 036a 1a64 1b64 0664 0664 178d  .Z.e.j.d.d.d.d..
-00000eb0: 035a 1b65 036a 0464 1c64 0564 0664 0664  .Z.e.j.d.d.d.d.d
-00000ec0: 078d 045a 1c65 036a 0464 1d64 0564 0664  ...Z.e.j.d.d.d.d
-00000ed0: 0664 078d 045a 1d65 036a 1e64 1e64 0664  .d...Z.e.j.d.d.d
-00000ee0: 1f8d 025a 1f47 0064 2064 2184 0064 2183  ...Z.G.d d!..d!.
-00000ef0: 025a 2064 2253 0029 23da 0644 6f63 746f  .Z d"S.)#..Docto
-00000f00: 7272 2100 0000 7222 0000 0072 2300 0000  rr!...r"...r#...
-00000f10: 7225 0000 0072 2600 0000 5472 2700 0000  r%...r&...Tr'...
-00000f20: 7506 0000 00e9 82ae e7ae b175 0600 0000  u..........u....
-00000f30: e59c b0e5 9d80 7506 0000 00e5 b7a5 e58f  ......u.........
-00000f40: b775 0600 0000 e881 8ce4 bd8d f506 0000  .u..............
-00000f50: 00e8 818c e7a7 b072 4800 0000 f506 0000  .......rH.......
-00000f60: 00e6 80a7 e588 abe9 0200 0000 a905 720b  ..............r.
-00000f70: 0000 0072 2400 0000 da07 6368 6f69 6365  ...r$.....choice
-00000f80: 7372 0d00 0000 7228 0000 0075 0600 0000  sr....r(...u....
-00000f90: e6b0 91e6 978f e920 0000 00f5 0c00 0000  ....... ........
-00000fa0: e8ba abe4 bbbd e8af 81e5 8fb7 f50c 0000  ................
-00000fb0: 00e6 8980 e5b1 9ee7 a791 e5ae a472 2e00  .............r..
-00000fc0: 0000 f50c 0000 00e5 87ba e794 9fe6 97a5  ................
-00000fd0: e69c 9f72 2900 0000 750c 0000 00e5 8cbb  ...r)...u.......
-00000fe0: e794 9fe7 85a7 e789 875a 0c64 6f63 746f  .........Z.docto
-00000ff0: 725f 7068 6f74 6f72 3200 0000 750c 0000  r_photor2...u...
-00001000: 00e5 8cbb e794 9fe6 8f8f e8bf b072 3300  .............r3.
-00001010: 0000 7234 0000 0075 1500 0000 e698 afe5  ..r4...u........
-00001020: 90a6 e4ba 92e8 8194 e7bd 91e6 8ea5 e8af  ................
-00001030: 8a72 1200 0000 6300 0000 0000 0000 0000  .r....c.........
-00001040: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00001050: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00001060: 6402 5a04 6504 5a05 6403 5300 2904 7a0b  d.Z.e.Z.d.S.).z.
-00001070: 446f 6374 6f72 2e4d 6574 615a 0962 735f  Doctor.MetaZ.bs_
-00001080: 646f 6374 6f72 7509 0000 00e5 8cbb e794  doctoru.........
-00001090: 9fe8 a1a8 4e72 3500 0000 7218 0000 0072  ....Nr5...r....r
-000010a0: 1800 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-000010b0: 0000 007d 0000 0073 0600 0000 0801 0401  ...}...s........
-000010c0: 0401 721a 0000 004e 2921 7214 0000 0072  ..r....N)!r....r
-000010d0: 1500 0000 7216 0000 0072 0500 0000 7238  ....r....r....r8
-000010e0: 0000 0072 3900 0000 723a 0000 00da 0565  ...r9...r:.....e
-000010f0: 6d61 696c 723e 0000 005a 0a6a 6f62 5f6e  mailr>...Z.job_n
-00001100: 756d 6265 72da 0870 6f73 6974 696f 6e72  umber..positionr
-00001110: 4000 0000 724a 0000 0072 4100 0000 5a08  @...rJ...rA...Z.
-00001120: 646f 635f 7261 6e6b da0d 4745 4e44 4552  doc_rank..GENDER
-00001130: 5f43 484f 4943 45da 0667 656e 6465 725a  _CHOICE..genderZ
-00001140: 066e 6174 696f 6e5a 0569 646e 756d 7245  .nationZ.idnumrE
-00001150: 0000 00da 066f 6666 6963 6572 2000 0000  .....officer ...
-00001160: 7249 0000 00da 0944 6174 6546 6965 6c64  rI.....DateField
-00001170: da08 6269 7274 6864 6179 5a05 7068 6f74  ..birthdayZ.phot
-00001180: 6f72 3b00 0000 da08 6465 7363 7269 6265  or;.....describe
-00001190: 7243 0000 0072 4400 0000 721e 0000 005a  rC...rD...r....Z
-000011a0: 1169 735f 6f6e 6c69 6e65 5f63 6f6e 7375  .is_online_consu
-000011b0: 6c74 721a 0000 0072 1800 0000 7218 0000  ltr....r....r...
-000011c0: 0072 1800 0000 7219 0000 0072 4b00 0000  .r....r....rK...
-000011d0: 5e00 0000 7338 0000 0008 010e 0112 0112  ^...s8..........
-000011e0: 0112 0112 0112 0106 0102 0104 fe06 0414  ................
-000011f0: 0112 0112 0106 0102 0104 fe06 0406 0102  ................
-00001200: 0104 fe06 0410 0210 0110 0112 0112 020e  ................
-00001210: 0272 4b00 0000 6300 0000 0000 0000 0000  .rK...c.........
-00001220: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
-00001230: b201 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
-00001240: 6401 6402 6403 6403 6404 8d04 5a05 6503  d.d.d.d.d...Z.e.
-00001250: 6a04 6405 6402 6403 6403 6404 8d04 5a06  j.d.d.d.d.d...Z.
-00001260: 6503 6a07 6406 6403 6403 6407 8d03 5a08  e.j.d.d.d.d...Z.
-00001270: 6503 6a09 6408 6409 640a 8d02 5a0a 6503  e.j.d.d.d...Z.e.
-00001280: 6a04 640b 640c 6403 6403 6404 8d04 5a0b  j.d.d.d.d.d...Z.
-00001290: 6503 6a07 640d 6403 6403 6407 8d03 5a0c  e.j.d.d.d.d...Z.
-000012a0: 6503 6a04 640e 640f 650d 6403 6403 6410  e.j.d.d.e.d.d.d.
-000012b0: 8d05 5a0e 6503 6a04 6411 640c 6403 6403  ..Z.e.j.d.d.d.d.
-000012c0: 6404 8d04 5a0f 6503 6a10 6412 6413 6403  d...Z.e.j.d.d.d.
-000012d0: 6403 6414 8d04 5a11 6503 6a12 6513 6415  d.d...Z.e.j.e.d.
-000012e0: 6503 6a14 6403 6416 8d04 5a15 6503 6a12  e.j.d.d...Z.e.j.
-000012f0: 6516 6417 6503 6a14 6403 6416 8d04 5a17  e.d.e.j.d.d...Z.
-00001300: 6503 6a12 6518 6418 6503 6a14 6403 6416  e.j.e.d.e.j.d.d.
-00001310: 8d04 5a19 6503 6a12 651a 6419 6503 6a14  ..Z.e.j.e.d.e.j.
-00001320: 6403 6416 8d04 5a1b 6503 6a04 641a 640c  d.d...Z.e.j.d.d.
-00001330: 641b 641c 8d03 5a1c 6503 6a04 641d 6402  d.d...Z.e.j.d.d.
-00001340: 6403 6403 6404 8d04 5a1d 6503 6a04 641e  d.d.d...Z.e.j.d.
-00001350: 6402 6403 6403 6404 8d04 5a1e 6503 6a1f  d.d.d.d...Z.e.j.
-00001360: 641f 6403 6403 6407 8d03 5a20 6503 6a04  d.d.d.d...Z e.j.
-00001370: 6420 640c 6403 6403 6404 8d04 5a21 6503  d d.d.d.d...Z!e.
-00001380: 6a04 6421 640c 6403 6403 6404 8d04 5a22  j.d!d.d.d.d...Z"
-00001390: 6503 6a23 6422 6403 6403 6423 8d03 5a24  e.j#d"d.d.d#..Z$
-000013a0: 6503 6a23 6424 6403 6403 6425 8d03 5a25  e.j#d$d.d.d%..Z%
-000013b0: 4700 6426 6427 8400 6427 8302 5a26 6527  G.d&d'..d'..Z&e'
-000013c0: 6428 6429 8400 8301 5a28 6527 642a 642b  d(d)....Z(e'd*d+
-000013d0: 8400 8301 5a29 6527 642c 642d 8400 8301  ....Z)e'd,d-....
-000013e0: 5a2a 642e 5300 292f da04 5573 6572 7221  Z*d.S.)/..Userr!
-000013f0: 0000 0072 2200 0000 5472 2700 0000 7506  ...r"...Tr'...u.
-00001400: 0000 00e5 af86 e7a0 8175 1200 0000 e4b8  .........u......
-00001410: 8ae6 aca1 e799 bbe5 bd95 e697 b6e9 97b4  ................
-00001420: 7229 0000 0075 0f00 0000 e698 afe5 90a6  r)...u..........
-00001430: e698 afe8 b685 e7ae a146 7212 0000 0072  .........Fr....r
-00001440: 2500 0000 7226 0000 0072 5400 0000 724d  %...r&...rT...rM
-00001450: 0000 0072 4e00 0000 724f 0000 0072 5200  ...rN...rO...rR.
-00001460: 0000 f506 0000 00e6 8e92 e5ba 8fe9 0100  ................
-00001470: 0000 a904 720b 0000 0072 1300 0000 720d  ....r....r....r.
-00001480: 0000 0072 2800 0000 7253 0000 0072 2f00  ...r(...rS...r/.
-00001490: 0000 722e 0000 0072 4c00 0000 750c 0000  ..r....rL...u...
-000014a0: 00e7 bb91 e5ae 9ae5 8cbb e794 9f75 0c00  .............u..
-000014b0: 0000 e794 a8e6 88b7 e5a4 b4e5 838f 5a0b  ..............Z.
-000014c0: 7573 6572 5f61 7661 7461 7272 3200 0000  user_avatarr2...
-000014d0: 750c 0000 00e9 bb98 e8ae a4e8 a792 e889  u...............
-000014e0: b275 0f00 0000 e58f afe6 938d e4bd 9ce7  .u..............
-000014f0: a791 e5ae a475 0c00 0000 e6b3 a8e9 878a  .....u..........
-00001500: e8af b4e6 988e 7233 0000 0072 3400 0000  ......r3...r4...
-00001510: 7209 0000 0072 0a00 0000 720e 0000 0072  r....r....r....r
-00001520: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00001530: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-00001540: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00001550: 5300 2903 7a09 5573 6572 2e4d 6574 6175  S.).z.User.Metau
-00001560: 0900 0000 e794 a8e6 88b7 e8a1 a84e 2904  .............N).
-00001570: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001580: 0b00 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
-00001590: 0000 0072 1900 0000 721a 0000 00ab 0000  ...r....r.......
-000015a0: 0073 0200 0000 0802 721a 0000 0063 0100  .s......r....c..
-000015b0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000015c0: 0000 4300 0000 7318 0000 007c 006a 007d  ..C...s....|.j.}
-000015d0: 017c 0173 147c 006a 01a0 02a1 007d 017c  .|.s.|.j.....}.|
-000015e0: 0153 0029 0175 8e00 0000 0a20 2020 2020  .S.).u.....     
-000015f0: 2020 20e8 8eb7 e58f 96e5 bd93 e589 8de7     .............
-00001600: 94a8 e688 b7e9 bb98 e8ae a4e7 94a8 e688  ................
-00001610: b7e7 bb84 2c0a 2020 2020 2020 2020 e5a6  ....,.        ..
-00001620: 82e6 9e9c e69c aae8 aebe e7bd aeef bc8c  ................
-00001630: e8bf 94e5 9b9e e7ac ace4 b880 e4b8 aae7  ................
-00001640: 94a8 e688 b7e7 bb84 0a20 2020 2020 2020  .........       
-00001650: 20e5 90a6 e588 99e8 bf94 e59b 9ee8 aebe   ...............
-00001660: e7bd aee7 9a84 e794 a8e6 88b7 e7bb 840a  ................
-00001670: 2020 2020 2020 2020 2903 5a0d 6465 6661          ).Z.defa
-00001680: 756c 745f 6772 6f75 70da 0667 726f 7570  ult_group..group
-00001690: 73da 0566 6972 7374 a902 722d 0000 005a  s..first..r-...Z
-000016a0: 0972 6574 5f67 726f 7570 7218 0000 0072  .ret_groupr....r
-000016b0: 1800 0000 7219 0000 00da 1167 6574 5f64  ....r......get_d
-000016c0: 6566 6175 6c74 5f67 726f 7570 b300 0000  efault_group....
-000016d0: 7308 0000 0000 0706 0104 010a 017a 1655  s............z.U
-000016e0: 7365 722e 6765 745f 6465 6661 756c 745f  ser.get_default_
-000016f0: 6772 6f75 7063 0100 0000 0000 0000 0000  groupc..........
-00001700: 0000 0200 0000 0200 0000 4300 0000 731c  ..........C...s.
-00001710: 0000 007c 006a 00a0 01a1 007d 017c 0173  ...|.j.....}.|.s
-00001720: 187c 006a 00a0 02a1 007d 017c 0153 00a9  .|.j.....}.|.S..
-00001730: 014e 2903 7261 0000 00da 0361 6c6c da04  .N).ra.....all..
-00001740: 6e6f 6e65 7263 0000 0072 1800 0000 7218  nonerc...r....r.
-00001750: 0000 0072 1900 0000 da0d 6765 745f 616c  ...r......get_al
-00001760: 6c67 726f 7570 73bf 0000 0073 0800 0000  lgroups....s....
-00001770: 0002 0a01 0401 0a01 7a12 5573 6572 2e67  ........z.User.g
-00001780: 6574 5f61 6c6c 6772 6f75 7073 6301 0000  et_allgroupsc...
-00001790: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-000017a0: 0043 0000 0073 1800 0000 6401 7d01 7c00  .C...s....d.}.|.
-000017b0: 6a00 7d01 7c01 7314 7c00 6a01 7d01 7c01  j.}.|.s.|.j.}.|.
-000017c0: 5300 2902 7533 0000 000a 2020 2020 2020  S.).u3....      
-000017d0: 2020 e88e b7e5 8f96 e794 a8e6 88b7 e9bb    ..............
-000017e0: 98e8 aea4 e79a 84e7 bb84 e7bb 87e6 9cba  ................
-000017f0: e69e 840a 2020 2020 2020 2020 4e29 0272  ....        N).r
-00001800: 5900 0000 7249 0000 0029 0272 2d00 0000  Y...rI...).r-...
-00001810: 5a07 7265 745f 6f72 6772 1800 0000 7218  Z.ret_orgr....r.
-00001820: 0000 0072 1900 0000 da18 6765 745f 6465  ...r......get_de
-00001830: 6661 756c 745f 6f72 6761 6e69 7a61 7469  fault_organizati
-00001840: 6f6e c600 0000 730a 0000 0000 0504 0106  on....s.........
-00001850: 0104 0106 017a 1d55 7365 722e 6765 745f  .....z.User.get_
-00001860: 6465 6661 756c 745f 6f72 6761 6e69 7a61  default_organiza
-00001870: 7469 6f6e 4e29 2b72 1400 0000 7215 0000  tionN)+r....r...
-00001880: 0072 1600 0000 7205 0000 0072 3800 0000  .r....r....r8...
-00001890: 7239 0000 00da 0870 6173 7377 6f72 6472  r9.....passwordr
-000018a0: 5a00 0000 da0a 6c61 7374 5f6c 6f67 696e  Z.....last_login
-000018b0: 721e 0000 00da 0c69 735f 7375 7065 7275  r......is_superu
-000018c0: 7365 7272 3a00 0000 725b 0000 0072 5700  serr:...r[...rW.
-000018d0: 0000 7258 0000 005a 0969 6463 6172 646e  ..rX...Z.idcardn
-000018e0: 756d da0c 496e 7465 6765 7246 6965 6c64  um..IntegerField
-000018f0: da08 6f72 6465 725f 6279 7240 0000 0072  ..order_byr@...r
-00001900: 4500 0000 7241 0000 0072 5900 0000 7220  E...rA...rY...r 
-00001910: 0000 0072 4900 0000 724a 0000 005a 0975  ...rI...rJ...Z.u
-00001920: 7365 725f 7261 6e6b 724b 0000 005a 0664  ser_rankrK...Z.d
-00001930: 6f63 746f 725a 0a61 7661 7461 725f 7572  octorZ.avatar_ur
-00001940: 6c5a 1064 6566 6175 6c74 5f67 726f 7570  lZ.default_group
-00001950: 5f69 645a 0c61 6c6c 6f77 5f6f 6666 6963  _idZ.allow_offic
-00001960: 6572 3b00 0000 da04 6e6f 7465 7243 0000  er;.....noterC..
-00001970: 0072 4400 0000 721b 0000 0072 1c00 0000  .rD...r....r....
-00001980: 721d 0000 0072 1a00 0000 da08 7072 6f70  r....r......prop
-00001990: 6572 7479 7264 0000 0072 6800 0000 7269  ertyrd...rh...ri
-000019a0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-000019b0: 0000 7219 0000 0072 5d00 0000 8300 0000  ..r....r].......
-000019c0: 7358 0000 0008 0112 0112 0110 010e 0112  sX..............
-000019d0: 0110 0114 0112 0112 0106 0102 0104 0102  ................
-000019e0: fd06 0506 0102 0104 0102 fd06 0506 0102  ................
-000019f0: 0104 0102 fd06 0506 0102 0104 0102 fd06  ................
-00001a00: 0610 0112 0112 0110 0112 0112 0110 0110  ................
-00001a10: 020e 0802 010a 0b02 010a 0602 0172 5d00  .............r].
-00001a20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001a30: 0000 0007 0000 0040 0000 0073 bc00 0000  .......@...s....
-00001a40: 6500 5a01 6400 5a02 6401 5a03 6504 6a05  e.Z.d.Z.d.Z.e.j.
-00001a50: 6506 6504 6a07 6402 6403 6403 6404 8d05  e.e.j.d.d.d.d...
-00001a60: 5a08 6504 6a09 6403 6405 6403 6406 8d03  Z.e.j.d.d.d.d...
-00001a70: 5a0a 6504 6a0b 6407 6408 6403 6403 6409  Z.e.j.d.d.d.d.d.
-00001a80: 8d04 5a0c 6504 6a0d 650e 640a 6504 6a07  ..Z.e.j.e.d.e.j.
-00001a90: 640b 640c 8d04 5a0f 6504 6a10 640d 640e  d.d...Z.e.j.d.d.
-00001aa0: 6403 640f 8d03 5a11 6504 6a0b 6408 6410  d.d...Z.e.j.d.d.
-00001ab0: 6403 6411 8d03 5a12 6504 6a0b 6408 6412  d.d...Z.e.j.d.d.
-00001ac0: 6403 6403 6413 8d04 5a13 6504 6a14 6414  d.d.d...Z.e.j.d.
-00001ad0: 6403 6403 6415 8d03 5a15 6504 6a14 6416  d.d.d...Z.e.j.d.
-00001ae0: 6403 6403 6417 8d03 5a16 4700 6418 6419  d.d.d...Z.G.d.d.
-00001af0: 8400 6419 8302 5a17 641a 5300 291b da0a  ..d...Z.d.S.)...
-00001b00: 4578 7472 6147 726f 7570 7519 0000 000a  ExtraGroupu.....
-00001b10: 2020 2020 e8a7 92e8 89b2 e689 a9e5 8585      ............
-00001b20: e8a1 a80a 2020 2020 da0b 6578 7472 615f  ....    ..extra_
-00001b30: 6772 6f75 7054 2904 7230 0000 00da 0c72  groupT).r0.....r
-00001b40: 656c 6174 6564 5f6e 616d 6572 0d00 0000  elated_namer....
-00001b50: 7228 0000 0072 1100 0000 2903 7213 0000  r(...r....).r...
-00001b60: 0072 0b00 0000 720d 0000 0075 0600 0000  .r....r....u....
-00001b70: e68f 8fe8 bfb0 e932 0000 0029 0372 2400  .......2...).r$.
-00001b80: 0000 720d 0000 0072 2800 0000 722e 0000  ..r....r(...r...
-00001b90: 0072 6100 0000 a903 720b 0000 0072 3000  .ra.....r....r0.
-00001ba0: 0000 7273 0000 0072 5e00 0000 725f 0000  ..rs...r^...r_..
-00001bb0: 00a9 0372 0b00 0000 7213 0000 0072 0d00  ...r....r....r..
-00001bc0: 0000 750c 0000 00e8 a792 e889 b2e4 bba3  ..u.............
-00001bd0: e7a0 8172 2b00 0000 7233 0000 00a9 0472  ...r+...r3.....r
-00001be0: 2400 0000 720b 0000 0072 0d00 0000 7228  $...r....r....r(
-00001bf0: 0000 0072 0900 0000 720a 0000 0075 1200  ...r....r....u..
-00001c00: 0000 e69c 80e5 908e e69b b4e6 96b0 e697  ................
-00001c10: b6e9 97b4 720f 0000 0063 0000 0000 0000  ....r....c......
-00001c20: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00001c30: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00001c40: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
-00001c50: 047a 0f45 7874 7261 4772 6f75 702e 4d65  .z.ExtraGroup.Me
-00001c60: 7461 5a0e 6273 5f65 7874 7261 5f67 726f  taZ.bs_extra_gro
-00001c70: 7570 7506 0000 00e8 a792 e889 b24e 7235  upu..........Nr5
-00001c80: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00001c90: 0000 7219 0000 0072 1a00 0000 e500 0000  ..r....r........
-00001ca0: 7306 0000 0008 0104 0104 0172 1a00 0000  s..........r....
-00001cb0: 4e29 1872 1400 0000 7215 0000 0072 1600  N).r....r....r..
-00001cc0: 0000 da07 5f5f 646f 635f 5f72 0500 0000  ....__doc__r....
-00001cd0: da0d 4f6e 6554 6f4f 6e65 4669 656c 6472  ..OneToOneFieldr
-00001ce0: 0300 0000 7241 0000 00da 0567 726f 7570  ....rA.....group
-00001cf0: 721e 0000 0072 1f00 0000 7238 0000 0072  r....r....r8...r
-00001d00: 6f00 0000 7240 0000 0072 2000 0000 7249  o...r@...r ...rI
-00001d10: 0000 0072 6d00 0000 726e 0000 005a 0972  ...rm...rn...Z.r
-00001d20: 6f6c 655f 636f 6465 5a0c 6372 6561 7465  ole_codeZ.create
-00001d30: 645f 7573 6572 721b 0000 005a 0a63 7265  d_userr....Z.cre
-00001d40: 6174 6564 5f61 745a 0a75 7064 6174 6564  ated_atZ.updated
-00001d50: 5f61 7472 1a00 0000 7218 0000 0072 1800  _atr....r....r..
-00001d60: 0000 7218 0000 0072 1900 0000 7271 0000  ..r....r....rq..
-00001d70: 00d2 0000 0073 2000 0000 0801 0403 1601  .....s .........
-00001d80: 1001 1201 0401 0201 0201 0401 02fc 0606  ................
-00001d90: 1001 1001 1201 1001 1002 7271 0000 0063  ..........rq...c
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0700 0000 4000 0000 7390 0000 0065 005a  ....@...s....e.Z
-00001dc0: 0164 005a 0264 015a 0365 046a 0564 0264  .d.Z.d.Z.e.j.d.d
-00001dd0: 0364 0464 058d 035a 0665 046a 0764 0664  .d.d...Z.e.j.d.d
-00001de0: 0464 0464 078d 035a 0865 046a 0964 0864  .d.d...Z.e.j.d.d
-00001df0: 0964 0464 0a8d 035a 0a65 046a 0964 0b64  .d.d...Z.e.j.d.d
-00001e00: 0964 0464 0464 0c8d 045a 0b65 046a 0564  .d.d.d...Z.e.j.d
-00001e10: 0d64 0e64 0464 0464 0f8d 045a 0c65 046a  .d.d.d.d...Z.e.j
-00001e20: 0d64 1064 1165 046a 0e64 1264 0464 138d  .d.d.e.j.d.d.d..
-00001e30: 055a 0f47 0064 1464 1584 0064 1583 025a  .Z.G.d.d...d...Z
-00001e40: 1064 1664 1784 005a 1164 1853 0029 19da  .d.d...Z.d.S.)..
-00001e50: 1043 6f6e 7465 6e74 5479 7065 4361 7465  .ContentTypeCate
-00001e60: 7375 1600 0000 0a20 2020 20e8 8f9c e58d  su.....    .....
-00001e70: 95e5 908d e7a7 b00a 2020 2020 7221 0000  ........    r!..
-00001e80: 00e9 1400 0000 54a9 0272 2400 0000 720d  ......T..r$...r.
-00001e90: 0000 0072 1100 0000 a902 7213 0000 0072  ...r......r....r
-00001ea0: 0d00 0000 725e 0000 0072 5f00 0000 7276  ....r^...r_...rv
-00001eb0: 0000 0075 0600 0000 e7ba a7e5 88ab 7260  ...u..........r`
-00001ec0: 0000 00f5 0600 0000 e59b bee6 a087 e9f4  ................
-00001ed0: 0100 0072 2700 0000 722d 0000 0075 0c00  ...r'...r-...u..
-00001ee0: 0000 e788 b6e7 baa7 e88f 9ce5 8d95 da08  ................
-00001ef0: 6368 696c 6472 656e 2904 720b 0000 0072  children).r....r
-00001f00: 3000 0000 7273 0000 0072 0d00 0000 6300  0...rs...r....c.
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001f20: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
-00001f30: 6400 5a02 6401 5a03 6402 5a04 6504 5a05  d.Z.d.Z.d.Z.e.Z.
-00001f40: 6403 5a06 6404 5300 2905 7a15 436f 6e74  d.Z.d.S.).z.Cont
-00001f50: 656e 7454 7970 6543 6174 6573 2e4d 6574  entTypeCates.Met
-00001f60: 615a 1462 735f 636f 6e74 656e 745f 7479  aZ.bs_content_ty
-00001f70: 7065 5f63 6174 7375 0c00 0000 e88f 9ce5  pe_catsu........
-00001f80: 8d95 e590 8de7 a7b0 a901 726e 0000 004e  ..........rn...N
-00001f90: a907 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001fa0: 0072 3600 0000 720b 0000 0072 3700 0000  .r6...r....r7...
-00001fb0: da08 6f72 6465 7269 6e67 7218 0000 0072  ..orderingr....r
-00001fc0: 1800 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00001fd0: 0000 00fc 0000 0073 0800 0000 0801 0401  .......s........
-00001fe0: 0401 0401 721a 0000 0063 0100 0000 0000  ....r....c......
-00001ff0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00002000: 0000 7306 0000 007c 006a 0053 0072 6500  ..s....|.j.S.re.
-00002010: 0000 a901 7239 0000 00a9 0172 2d00 0000  ....r9.....r-...
-00002020: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00002030: 075f 5f73 7472 5f5f 0201 0000 7302 0000  .__str__....s...
-00002040: 0000 017a 1843 6f6e 7465 6e74 5479 7065  ...z.ContentType
-00002050: 4361 7465 732e 5f5f 7374 725f 5f4e 2912  Cates.__str__N).
-00002060: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00002070: 7800 0000 7205 0000 0072 3800 0000 7239  x...r....r8...r9
-00002080: 0000 0072 1e00 0000 721f 0000 0072 6d00  ...r....r....rm.
-00002090: 0000 726e 0000 00da 056c 6576 656c da0a  ..rn.....level..
-000020a0: 6963 6f6e 5f63 6c61 7373 7240 0000 0072  icon_classr@...r
-000020b0: 4100 0000 7242 0000 0072 1a00 0000 7287  A...rB...r....r.
-000020c0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-000020d0: 0000 7219 0000 0072 7b00 0000 eb00 0000  ..r....r{.......
-000020e0: 731e 0000 0008 0104 0310 0110 0110 0112  s...............
-000020f0: 0112 0104 0102 0102 0104 0102 0102 fb06  ................
-00002100: 080e 0672 7b00 0000 6300 0000 0000 0000  ...r{...c.......
-00002110: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00002120: 0073 ce00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002130: 5a03 6504 6a05 6402 6403 6404 6405 8d03  Z.e.j.d.d.d.d...
-00002140: 5a06 6504 6a07 6508 6406 6504 6a09 6407  Z.e.j.e.d.e.j.d.
-00002150: 6408 8d04 5a0a 6504 6a07 6409 640a 6504  d...Z.e.j.d.d.e.
-00002160: 6a09 640b 6408 8d04 5a0b 6504 6a05 640c  j.d.d...Z.e.j.d.
-00002170: 640d 6404 6404 640e 8d04 5a0c 6504 6a0d  d.d.d.d...Z.e.j.
-00002180: 640f 6404 6404 6410 8d03 5a0e 6504 6a0d  d.d.d.d...Z.e.j.
-00002190: 6411 6404 6404 6410 8d03 5a0f 6504 6a05  d.d.d.d...Z.e.j.
-000021a0: 6412 6413 6404 6414 8d03 5a10 6504 6a11  d.d.d.d...Z.e.j.
-000021b0: 6415 6404 6416 8d02 5a12 6504 6a13 6417  d.d.d...Z.e.j.d.
-000021c0: 6404 6404 6418 8d03 5a14 6504 6a15 6419  d.d.d...Z.e.j.d.
-000021d0: 641a 6404 641b 8d03 5a16 4700 641c 641d  d.d.d...Z.G.d.d.
-000021e0: 8400 641d 8302 5a17 641e 641f 8400 5a18  ..d...Z.d.d...Z.
-000021f0: 6420 5300 2921 da0d 436f 6e74 656e 7454  d S.)!..ContentT
-00002200: 7970 6545 7875 1600 0000 0a20 2020 20e5  ypeExu.....    .
-00002210: 8a9f e883 bde7 b1bb e588 ab0a 2020 2020  ............    
-00002220: 7221 0000 0072 7c00 0000 5472 7d00 0000  r!...r|...Tr}...
-00002230: 750c 0000 00e7 b3bb e7bb 9fe5 ba94 e794  u...............
-00002240: a8da 0965 7874 656e 7369 6f6e 7275 0000  ...extensionru..
-00002250: 0072 7b00 0000 7506 0000 00e8 8f9c e58d  .r{...u.........
-00002260: 955a 0d63 6f6e 7465 6e74 5f63 6174 6573  .Z.content_cates
-00002270: 727f 0000 0072 8000 0000 7227 0000 00da  r....r....r'....
-00002280: 0375 726c 7229 0000 0075 0600 0000 e7bb  .urlr)...u......
-00002290: 84e6 8890 7506 0000 00e5 8f82 e695 b072  ....u..........r
-000022a0: 7400 0000 a903 720b 0000 0072 2400 0000  t.....r....r$...
-000022b0: 720d 0000 0075 0900 0000 e987 8de5 ae9a  r....u..........
-000022c0: e590 91a9 0272 0b00 0000 720d 0000 0072  .....r....r....r
-000022d0: 1100 0000 727e 0000 0072 5e00 0000 725f  ....r~...r^...r_
-000022e0: 0000 0072 7600 0000 6300 0000 0000 0000  ...rv...c.......
-000022f0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00002300: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002310: 5a03 6402 5a04 6504 5a05 6403 5a06 6404  Z.d.Z.e.Z.d.Z.d.
-00002320: 5300 2905 7a12 436f 6e74 656e 7454 7970  S.).z.ContentTyp
-00002330: 6545 782e 4d65 7461 5a12 6273 5f63 6f6e  eEx.MetaZ.bs_con
-00002340: 7465 6e74 5f74 7970 655f 6578 7512 0000  tent_type_exu...
-00002350: 00e5 8a9f e883 bde7 b1bb e588 abe8 a1a5  ................
-00002360: e585 8572 8200 0000 4e72 8300 0000 7218  ...r....Nr....r.
-00002370: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00002380: 0000 721a 0000 0017 0100 0073 0800 0000  ..r........s....
-00002390: 0801 0401 0401 0401 721a 0000 0063 0100  ........r....c..
-000023a0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000023b0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-000023c0: 0072 6500 0000 7285 0000 0072 8600 0000  .re...r....r....
-000023d0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000023e0: 8700 0000 1d01 0000 7302 0000 0000 017a  ........s......z
-000023f0: 1543 6f6e 7465 6e74 5479 7065 4578 2e5f  .ContentTypeEx._
-00002400: 5f73 7472 5f5f 4e29 1972 1400 0000 7215  _str__N).r....r.
-00002410: 0000 0072 1600 0000 7278 0000 0072 0500  ...r....rx...r..
-00002420: 0000 7238 0000 0072 3900 0000 7240 0000  ..r8...r9...r@..
-00002430: 0072 0400 0000 7241 0000 00da 0c63 6f6e  .r....rA.....con
-00002440: 7465 6e74 5f74 7970 655a 1063 6f6e 7465  tent_typeZ.conte
-00002450: 6e74 5f74 7970 655f 6361 7472 8900 0000  nt_type_catr....
-00002460: 723b 0000 005a 0966 726f 6e74 5f75 726c  r;...Z.front_url
-00002470: 5a0f 6672 6f6e 745f 636f 6d70 6f6e 656e  Z.front_componen
-00002480: 745a 0c66 726f 6e74 5f70 6172 616d 73da  tZ.front_params.
-00002490: 0855 524c 4669 656c 645a 1266 726f 6e74  .URLFieldZ.front
-000024a0: 5f72 6564 6972 6563 745f 7572 6c72 1e00  _redirect_urlr..
-000024b0: 0000 721f 0000 0072 6d00 0000 726e 0000  ..r....rm...rn..
-000024c0: 0072 1a00 0000 7287 0000 0072 1800 0000  .r....r....r....
-000024d0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000024e0: 8a00 0000 0601 0000 7322 0000 0008 0104  ........s"......
-000024f0: 0310 010c 0102 ff06 020c 0102 ff06 0212  ................
-00002500: 0110 0110 0110 010e 0110 0110 020e 0672  ...............r
-00002510: 8a00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002520: 0000 0000 0006 0000 0040 0000 0073 9e00  .........@...s..
-00002530: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
-00002540: 6402 6403 6404 8d03 5a05 6503 6a04 6405  d.d.d...Z.e.j.d.
-00002550: 6402 6406 8d02 5a06 6503 6a04 6407 6408  d.d...Z.e.j.d.d.
-00002560: 6403 6409 8d03 5a07 6503 6a08 640a 6403  d.d...Z.e.j.d.d.
-00002570: 640b 8d02 5a09 6503 6a0a 650b 640c 6503  d...Z.e.j.e.d.e.
-00002580: 6a0c 6403 640d 8d04 5a0d 6503 6a04 640e  j.d.d...Z.e.j.d.
-00002590: 6402 6403 6403 640f 8d04 5a0e 6503 6a04  d.d.d.d...Z.e.j.
-000025a0: 6410 6402 6403 6403 640f 8d04 5a0f 6503  d.d.d.d.d...Z.e.
-000025b0: 6a10 6511 6411 6403 6412 8d03 5a12 4700  j.e.d.d.d...Z.G.
-000025c0: 6413 6414 8400 6414 8302 5a13 6415 5300  d.d...d...Z.d.S.
-000025d0: 2916 da0f 4578 7065 6e73 6553 7461 6e64  )...ExpenseStand
-000025e0: 6172 6475 0c00 0000 e8b4 b9e7 94a8 e7b1  ardu............
-000025f0: bbe5 9e8b 7226 0000 0054 728d 0000 0075  ....r&...Tr....u
-00002600: 0c00 0000 e6a0 87e5 8786 e590 8de7 a7b0  ................
-00002610: 7223 0000 0075 0c00 0000 e6a0 87e5 8786  r#...u..........
-00002620: e7bc 96e7 a081 7222 0000 0072 4700 0000  ......r"...rG...
-00002630: 7506 0000 00e8 b4b9 e794 a872 8e00 0000  u..........r....
-00002640: 722e 0000 0072 2f00 0000 7233 0000 0072  r....r/...r3...r
-00002650: 2700 0000 7234 0000 0075 1200 0000 e58c  '...r4...u......
-00002660: bbe7 949f e8b4 b9e7 94a8 e6a0 87e5 8786  ................
-00002670: 2902 720b 0000 0072 2800 0000 6300 0000  ).r....r(...c...
-00002680: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002690: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-000026a0: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-000026b0: 5300 2904 7a14 4578 7065 6e73 6553 7461  S.).z.ExpenseSta
-000026c0: 6e64 6172 642e 4d65 7461 5a13 6273 5f65  ndard.MetaZ.bs_e
-000026d0: 7870 656e 7365 5f73 7461 6e64 6172 6475  xpense_standardu
-000026e0: 0f00 0000 e8b4 b9e7 94a8 e6a0 87e5 8786  ................
-000026f0: e8a1 a84e 7235 0000 0072 1800 0000 7218  ...Nr5...r....r.
-00002700: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00002710: 0000 3101 0000 7306 0000 0008 0104 0104  ..1...s.........
-00002720: 0172 1a00 0000 4e29 1472 1400 0000 7215  .r....N).r....r.
-00002730: 0000 0072 1600 0000 7205 0000 0072 3800  ...r....r....r8.
-00002740: 0000 5a0c 6578 7065 6e73 655f 7479 7065  ..Z.expense_type
-00002750: 5a0d 7374 616e 6461 7264 5f6e 616d 655a  Z.standard_nameZ
-00002760: 0d73 7461 6e64 6172 645f 636f 6465 723f  .standard_coder?
-00002770: 0000 005a 0466 6565 7372 4000 0000 7220  ...Z.feesr@...r 
-00002780: 0000 0072 4100 0000 7249 0000 0072 4300  ...rA...rI...rC.
-00002790: 0000 7244 0000 00da 0f4d 616e 7954 6f4d  ..rD.....ManyToM
-000027a0: 616e 7946 6965 6c64 724b 0000 005a 0764  anyFieldrK...Z.d
-000027b0: 6f63 746f 7273 721a 0000 0072 1800 0000  octorsr....r....
-000027c0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000027d0: 9100 0000 2101 0000 731c 0000 0008 0210  ....!...s.......
-000027e0: 010e 0110 010e 0104 0102 0102 0104 0102  ................
-000027f0: fc06 0612 0112 0110 0272 9100 0000 6300  .........r....c.
-00002800: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00002810: 0000 0040 0000 0073 a600 0000 6500 5a01  ...@...s....e.Z.
-00002820: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-00002830: 8d03 5a05 6503 6a04 6405 6406 6407 8d02  ..Z.e.j.d.d.d...
-00002840: 5a06 6503 6a04 6408 6409 6407 8d02 5a07  Z.e.j.d.d.d...Z.
-00002850: 6503 6a04 6408 640a 6407 8d02 5a08 6503  e.j.d.d.d...Z.e.
-00002860: 6a09 640b 6403 640c 8d02 5a0a 6503 6a04  j.d.d.d...Z.e.j.
-00002870: 6408 640d 6403 6403 640e 8d04 5a0b 6503  d.d.d.d.d...Z.e.
-00002880: 6a04 6408 640f 6403 6403 640e 8d04 5a0c  j.d.d.d.d.d...Z.
-00002890: 6503 6a04 6410 6411 6403 6412 8d03 5a0d  e.j.d.d.d.d...Z.
-000028a0: 6503 6a04 6413 6411 6403 6412 8d03 5a0e  e.j.d.d.d.d...Z.
-000028b0: 4700 6414 6415 8400 6415 8302 5a0f 6416  G.d.d...d...Z.d.
-000028c0: 5300 2917 da16 496e 7370 6563 7469 6f6e  S.)...Inspection
-000028d0: 4469 6374 696f 6e61 7269 6573 7222 0000  Dictionariesr"..
-000028e0: 00f5 0c00 0000 e9a1 b9e7 9bae e7bc 96e7  ................
-000028f0: a081 5472 2b00 0000 e940 0000 00f5 0c00  ..Tr+....@......
-00002900: 0000 e9a1 b9e7 9bae e590 8de7 a7b0 a902  ................
-00002910: 7224 0000 0072 0b00 0000 e980 0000 00f5  r$...r..........
-00002920: 0c00 0000 e58c bbe9 99a2 e7bc 96e7 a081  ................
-00002930: 7246 0000 00f5 0c00 0000 e9a1 b9e7 9bae  rF..............
-00002940: e8b4 b9e7 94a8 728e 0000 00f5 0600 0000  ......r.........
-00002950: e5a4 87e6 b3a8 7277 0000 00f5 0c00 0000  ......rw........
-00002960: e58c bae5 8886 e5ad 97e6 aeb5 f512 0000  ................
-00002970: 00e6 a380 e9aa 8ce7 b1bb e59e 8be7 bc96  ................
-00002980: e7a0 8172 7400 0000 728d 0000 00f5 1200  ...rt...r.......
-00002990: 0000 e6a3 80e9 aa8c e7b1 bbe5 9e8b e590  ................
-000029a0: 8de7 a7b0 6300 0000 0000 0000 0000 0000  ....c...........
-000029b0: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
-000029c0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000029d0: 5a04 6504 5a05 6403 5300 2904 7a1b 496e  Z.e.Z.d.S.).z.In
-000029e0: 7370 6563 7469 6f6e 4469 6374 696f 6e61  spectionDictiona
-000029f0: 7269 6573 2e4d 6574 615a 1a62 735f 696e  ries.MetaZ.bs_in
-00002a00: 7370 6563 7469 6f6e 5f64 6963 7469 6f6e  spection_diction
-00002a10: 6172 6965 7375 0c00 0000 e6a3 80e6 9fa5  ariesu..........
-00002a20: e5ad 97e5 85b8 4e72 3500 0000 7218 0000  ......Nr5...r...
-00002a30: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00002a40: 721a 0000 0042 0100 0073 0600 0000 0801  r....B...s......
-00002a50: 0401 0401 721a 0000 004e a910 7214 0000  ....r....N..r...
-00002a60: 0072 1500 0000 7216 0000 0072 0500 0000  .r....r....r....
-00002a70: 7238 0000 005a 0c70 726f 6a65 6374 5f63  r8...Z.project_c
-00002a80: 6f64 655a 0c70 726f 6a65 6374 5f6e 616d  odeZ.project_nam
-00002a90: 655a 0d68 6f73 7069 7461 6c5f 636f 6465  eZ.hospital_code
-00002aa0: 5a0b 6f66 6669 6365 5f63 6f64 6572 3f00  Z.office_coder?.
-00002ab0: 0000 5a0c 7072 6f6a 6563 745f 6665 6573  ..Z.project_fees
-00002ac0: 5a07 7265 6d61 726b 735a 0b64 6973 7469  Z.remarksZ.disti
-00002ad0: 6e67 7569 7368 5a0a 636f 6465 5f73 7276  nguishZ.code_srv
-00002ae0: 7470 5a0a 6e61 6d65 5f73 7276 7470 721a  tpZ.name_srvtpr.
-00002af0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00002b00: 0000 7219 0000 0072 9300 0000 3701 0000  ..r....r....7...
-00002b10: 7314 0000 0008 0110 010e 010e 010e 010e  s...............
-00002b20: 0112 0112 0110 0110 0272 9300 0000 6300  .........r....c.
-00002b30: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00002b40: 0000 0040 0000 0073 a600 0000 6500 5a01  ...@...s....e.Z.
-00002b50: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-00002b60: 8d03 5a05 6503 6a04 6405 6406 6407 8d02  ..Z.e.j.d.d.d...
-00002b70: 5a06 6503 6a04 6408 6409 6407 8d02 5a07  Z.e.j.d.d.d...Z.
-00002b80: 6503 6a04 6408 640a 6407 8d02 5a08 6503  e.j.d.d.d...Z.e.
-00002b90: 6a09 640b 6403 640c 8d02 5a0a 6503 6a04  j.d.d.d...Z.e.j.
-00002ba0: 6408 640d 6403 6403 640e 8d04 5a0b 6503  d.d.d.d.d...Z.e.
-00002bb0: 6a04 6408 640f 6403 6403 640e 8d04 5a0c  j.d.d.d.d.d...Z.
-00002bc0: 6503 6a04 6410 6411 6403 6412 8d03 5a0d  e.j.d.d.d.d...Z.
-00002bd0: 6503 6a04 6413 6411 6403 6412 8d03 5a0e  e.j.d.d.d.d...Z.
-00002be0: 4700 6414 6415 8400 6415 8302 5a0f 6416  G.d.d...d...Z.d.
-00002bf0: 5300 2917 da17 4578 616d 696e 6174 696f  S.)...Examinatio
-00002c00: 6e44 6963 7469 6f6e 6172 6965 7372 2200  nDictionariesr".
-00002c10: 0000 7294 0000 0054 722b 0000 0072 9500  ..r....Tr+...r..
-00002c20: 0000 7296 0000 0072 9700 0000 7298 0000  ..r....r....r...
-00002c30: 0072 9900 0000 7246 0000 0072 9a00 0000  .r....rF...r....
-00002c40: 728e 0000 0072 9b00 0000 7277 0000 0072  r....r....rw...r
-00002c50: 9c00 0000 729d 0000 0072 7400 0000 728d  ....r....rt...r.
-00002c60: 0000 0072 9e00 0000 6300 0000 0000 0000  ...r....c.......
-00002c70: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00002c80: 0073 1800 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002c90: 5a03 6402 5a04 6504 5a05 6403 5300 2904  Z.d.Z.e.Z.d.S.).
-00002ca0: 7a1c 4578 616d 696e 6174 696f 6e44 6963  z.ExaminationDic
-00002cb0: 7469 6f6e 6172 6965 732e 4d65 7461 5a1b  tionaries.MetaZ.
-00002cc0: 6273 5f65 7861 6d69 6e61 7469 6f6e 5f64  bs_examination_d
-00002cd0: 6963 7469 6f6e 6172 6965 7375 0c00 0000  ictionariesu....
-00002ce0: e6a3 80e9 aa8c e5ad 97e5 85b8 4e72 3500  ............Nr5.
-00002cf0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00002d00: 0072 1900 0000 721a 0000 0053 0100 0073  .r....r....S...s
-00002d10: 0600 0000 0801 0401 0401 721a 0000 004e  ..........r....N
-00002d20: 729f 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00002d30: 1800 0000 7219 0000 0072 a000 0000 4801  ....r....r....H.
-00002d40: 0000 7314 0000 0008 0110 010e 010e 010e  ..s.............
-00002d50: 010e 0112 0112 0110 0110 0272 a000 0000  ...........r....
-00002d60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002d70: 0006 0000 0040 0000 0073 3c00 0000 6500  .....@...s<...e.
-00002d80: 5a01 6400 5a02 6503 6a04 6401 6402 6403  Z.d.Z.e.j.d.d.d.
-00002d90: 6404 8d03 5a05 6503 6a04 6405 6406 6403  d...Z.e.j.d.d.d.
-00002da0: 6403 6407 8d04 5a06 4700 6408 6409 8400  d.d...Z.G.d.d...
-00002db0: 6409 8302 5a07 640a 5300 290b da13 4472  d...Z.d.S.)...Dr
-00002dc0: 7567 5072 6570 6172 6174 696f 6e54 7970  ugPreparationTyp
-00002dd0: 6572 2200 0000 722a 0000 0054 722b 0000  er"...r*...Tr+..
-00002de0: 0072 9500 0000 750c 0000 00e7 b1bb e59e  .r....u.........
-00002df0: 8be5 908d e7a7 b072 7700 0000 6300 0000  .......rw...c...
-00002e00: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002e10: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002e20: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-00002e30: 5300 2904 7a18 4472 7567 5072 6570 6172  S.).z.DrugPrepar
-00002e40: 6174 696f 6e54 7970 652e 4d65 7461 5a18  ationType.MetaZ.
-00002e50: 6273 5f64 7275 675f 7072 6570 6172 6174  bs_drug_preparat
-00002e60: 696f 6e5f 7479 7065 7512 0000 00e8 8daf  ion_typeu.......
-00002e70: e593 81e5 88b6 e589 82e7 b1bb e59e 8b4e  ...............N
-00002e80: 7235 0000 0072 1800 0000 7218 0000 0072  r5...r....r....r
-00002e90: 1800 0000 7219 0000 0072 1a00 0000 5d01  ....r....r....].
-00002ea0: 0000 7306 0000 0008 0104 0104 0172 1a00  ..s..........r..
-00002eb0: 0000 4e29 0872 1400 0000 7215 0000 0072  ..N).r....r....r
-00002ec0: 1600 0000 7205 0000 0072 3800 0000 723d  ....r....r8...r=
-00002ed0: 0000 00da 0974 7970 655f 6e61 6d65 721a  .....type_namer.
-00002ee0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00002ef0: 0000 7219 0000 0072 a100 0000 5901 0000  ..r....r....Y...
-00002f00: 7306 0000 0008 0110 0112 0272 a100 0000  s..........r....
-00002f10: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002f20: 0006 0000 0040 0000 0073 3c00 0000 6500  .....@...s<...e.
-00002f30: 5a01 6400 5a02 6503 6a04 6401 6402 6403  Z.d.Z.e.j.d.d.d.
-00002f40: 6404 8d03 5a05 6503 6a04 6405 6406 6403  d...Z.e.j.d.d.d.
-00002f50: 6403 6407 8d04 5a06 4700 6408 6409 8400  d.d...Z.G.d.d...
-00002f60: 6409 8302 5a07 640a 5300 290b da08 4472  d...Z.d.S.)...Dr
-00002f70: 7567 5479 7065 722a 0000 0072 2200 0000  ugTyper*...r"...
-00002f80: 5472 4700 0000 7221 0000 0072 9500 0000  TrG...r!...r....
-00002f90: 7227 0000 0063 0000 0000 0000 0000 0000  r'...c..........
-00002fa0: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-00002fb0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00002fc0: 025a 0465 045a 0564 0353 0029 047a 0d44  .Z.e.Z.d.S.).z.D
-00002fd0: 7275 6754 7970 652e 4d65 7461 5a0c 6273  rugType.MetaZ.bs
-00002fe0: 5f64 7275 675f 7479 7065 f50c 0000 00e8  _drug_type......
-00002ff0: 8daf e593 81e7 b1bb e59e 8b4e 7235 0000  ...........Nr5..
-00003000: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00003010: 7219 0000 0072 1a00 0000 6701 0000 7306  r....r....g...s.
-00003020: 0000 0008 0104 0104 0172 1a00 0000 4ea9  .........r....N.
-00003030: 0872 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00003040: 7205 0000 0072 3800 0000 da04 636f 6465  r....r8.....code
-00003050: 7239 0000 0072 1a00 0000 7218 0000 0072  r9...r....r....r
-00003060: 1800 0000 7218 0000 0072 1900 0000 72a3  ....r....r....r.
-00003070: 0000 0063 0100 0073 0600 0000 0801 1001  ...c...s........
-00003080: 1202 72a3 0000 0063 0000 0000 0000 0000  ..r....c........
-00003090: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-000030a0: 733c 0000 0065 005a 0164 005a 0265 036a  s<...e.Z.d.Z.e.j
-000030b0: 0464 0164 0264 0364 048d 035a 0565 036a  .d.d.d.d...Z.e.j
-000030c0: 0464 0564 0664 0364 0364 078d 045a 0647  .d.d.d.d.d...Z.G
-000030d0: 0064 0864 0984 0064 0983 025a 0764 0a53  .d.d...d...Z.d.S
-000030e0: 0029 0bda 0c44 7275 6743 6174 6567 6f72  .)...DrugCategor
-000030f0: 7972 2200 0000 722a 0000 0054 722b 0000  yr"...r*...Tr+..
-00003100: 0072 9500 0000 750c 0000 00e7 b1bb e588  .r....u.........
-00003110: abe5 908d e7a7 b072 7700 0000 6300 0000  .......rw...c...
-00003120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00003130: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00003140: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-00003150: 5300 2904 7a11 4472 7567 4361 7465 676f  S.).z.DrugCatego
-00003160: 7279 2e4d 6574 615a 1062 735f 6472 7567  ry.MetaZ.bs_drug
-00003170: 5f63 6174 6567 6f72 7975 0c00 0000 e88d  _categoryu......
-00003180: afe5 9381 e7b1 bbe5 88ab 4e72 3500 0000  ..........Nr5...
-00003190: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-000031a0: 1900 0000 721a 0000 0071 0100 0073 0600  ....r....q...s..
-000031b0: 0000 0801 0401 0401 721a 0000 004e 2908  ........r....N).
-000031c0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000031d0: 0500 0000 7238 0000 0072 3d00 0000 5a0d  ....r8...r=...Z.
-000031e0: 6361 7465 676f 7279 5f6e 616d 6572 1a00  category_namer..
-000031f0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00003200: 0072 1900 0000 72a7 0000 006d 0100 0073  .r....r....m...s
-00003210: 0600 0000 0801 1001 1202 72a7 0000 0063  ..........r....c
-00003220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003230: 0600 0000 4000 0000 738e 0100 0065 005a  ....@...s....e.Z
-00003240: 0164 005a 0265 036a 0464 0164 0264 0364  .d.Z.e.j.d.d.d.d
-00003250: 048d 035a 0565 036a 0464 0564 0664 0364  ...Z.e.j.d.d.d.d
-00003260: 0364 078d 045a 0665 036a 0464 0564 0864  .d...Z.e.j.d.d.d
-00003270: 0364 0364 078d 045a 0765 036a 0464 0564  .d.d...Z.e.j.d.d
-00003280: 0964 0364 0364 078d 045a 0865 036a 0464  .d.d.d...Z.e.j.d
-00003290: 0a64 0b64 0364 0364 0c8d 045a 0965 036a  .d.d.d.d...Z.e.j
-000032a0: 0a65 0b64 0d65 036a 0c64 0e8d 035a 0d65  .e.d.e.j.d...Z.e
-000032b0: 036a 0a65 0e64 0f65 036a 0c64 0e8d 035a  .j.e.d.e.j.d...Z
-000032c0: 0f65 036a 0a65 1064 1065 036a 0c64 0e8d  .e.j.e.d.e.j.d..
-000032d0: 035a 1165 036a 0464 1164 0b64 0364 0364  .Z.e.j.d.d.d.d.d
-000032e0: 0c8d 045a 1265 036a 0464 1264 0b64 0364  ...Z.e.j.d.d.d.d
-000032f0: 0364 0c8d 045a 1365 036a 0464 1364 0b64  .d...Z.e.j.d.d.d
-00003300: 0364 0364 0c8d 045a 1465 036a 0464 1464  .d.d...Z.e.j.d.d
-00003310: 0b64 0364 0364 0c8d 045a 1565 036a 0464  .d.d.d...Z.e.j.d
-00003320: 1564 0b64 0364 0364 0c8d 045a 1665 036a  .d.d.d.d...Z.e.j
-00003330: 0464 1664 0b64 0364 0364 0c8d 045a 1765  .d.d.d.d.d...Z.e
-00003340: 036a 0464 1764 0b64 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
-00003350: 1865 036a 1964 1864 0364 198d 025a 1a65  .e.j.d.d.d...Z.e
-00003360: 036a 0464 1a64 0564 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
-00003370: 1b65 036a 0464 1b64 0564 0364 0364 0c8d  .e.j.d.d.d.d.d..
-00003380: 045a 1c65 036a 0464 1c64 0564 0364 0364  .Z.e.j.d.d.d.d.d
-00003390: 0c8d 045a 1d65 036a 0464 0564 1d64 0364  ...Z.e.j.d.d.d.d
-000033a0: 0364 078d 045a 1e65 036a 0464 0564 1e64  .d...Z.e.j.d.d.d
-000033b0: 0364 0364 078d 045a 1f47 0064 1f64 2084  .d.d...Z.G.d.d .
-000033c0: 0064 2083 025a 2064 2153 0029 22da 0d44  .d ..Z d!S.)"..D
-000033d0: 7275 6744 6972 6563 746f 7279 f50c 0000  rugDirectory....
-000033e0: 00e8 8daf e593 81e7 bc96 e7a0 8172 2200  .............r".
-000033f0: 0000 5472 4700 0000 7295 0000 00f5 0c00  ..TrG...r.......
-00003400: 0000 e88d afe5 9381 e590 8de7 a7b0 7277  ..............rw
-00003410: 0000 00f5 0600 0000 e8a7 84e6 a0bc f506  ................
-00003420: 0000 00e5 8d95 e4bd 8d75 1200 0000 e680  .........u......
-00003430: bbe9 878f e58d 95e4 bd8d e7bc 96e7 a081  ................
-00003440: 727c 0000 0072 2700 0000 f50c 0000 00e5  r|...r'.........
-00003450: 88b6 e589 82e7 b1bb e59e 8b72 4800 0000  ...........rH...
-00003460: f506 0000 00e7 b1bb e588 ab72 a400 0000  ...........r....
-00003470: 750c 0000 00e5 8d95 e4bd 8de5 8982 e987  u...............
-00003480: 8ff5 0c00 0000 e8ae a1e9 878f e58d 95e4  ................
-00003490: bd8d 7512 0000 00e8 aea1 e987 8fe5 8d95  ..u.............
-000034a0: e4bd 8de7 bc96 e7a0 81f5 0c00 0000 e5ba  ................
-000034b0: 93e5 ad98 e695 b0e9 878f 750c 0000 00e5  ..........u.....
-000034c0: ba93 e5ad 98e5 8d95 e4bd 8d75 0c00 0000  ...........u....
-000034d0: e58c bbe4 bf9d e7b1 bbe5 88ab 750c 0000  ............u...
-000034e0: 00e5 869c e590 88e7 b1bb e588 ab75 0f00  .............u..
-000034f0: 0000 e698 afe5 90a6 e698 afe5 9fba e88d  ................
-00003500: af72 1200 0000 750c 0000 00e9 ab98 e58d  .r....u.........
-00003510: b1e7 ad89 e7ba a775 1200 0000 e59b bde5  .......u........
-00003520: aeb6 e8b4 afe6 a087 e7bc 96e7 a081 7512  ..............u.
-00003530: 0000 00e5 9bbd e5ae b6e8 b4af e6a0 87e5  ................
-00003540: 908d e7a7 b0f5 0600 0000 e4ba a7e5 9cb0  ................
-00003550: f50c 0000 00e7 949f e4ba a7e5 8e82 e5ae  ................
-00003560: b663 0000 0000 0000 0000 0000 0000 0000  .c..............
-00003570: 0000 0100 0000 4000 0000 7318 0000 0065  ......@...s....e
-00003580: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
-00003590: 045a 0564 0353 0029 047a 1244 7275 6744  .Z.d.S.).z.DrugD
-000035a0: 6972 6563 746f 7279 2e4d 6574 615a 1162  irectory.MetaZ.b
-000035b0: 735f 6472 7567 5f64 6972 6563 746f 7279  s_drug_directory
-000035c0: 750c 0000 00e8 8daf e593 81e7 9bae e5bd  u...............
-000035d0: 954e 7235 0000 0072 1800 0000 7218 0000  .Nr5...r....r...
-000035e0: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-000035f0: 9a01 0000 7306 0000 0008 0104 0104 0172  ....s..........r
-00003600: 1a00 0000 4e29 2172 1400 0000 7215 0000  ....N)!r....r...
-00003610: 0072 1600 0000 7205 0000 0072 3800 0000  .r....r....r8...
-00003620: da09 6472 7567 5f63 6f64 65da 0964 7275  ..drug_code..dru
-00003630: 675f 6e61 6d65 da09 7374 616e 6461 7264  g_name..standard
-00003640: 73da 0575 6e69 7473 5a0f 746f 7461 6c5f  s..unitsZ.total_
-00003650: 756e 6974 5f63 6f64 6572 4000 0000 72a1  unit_coder@...r.
-00003660: 0000 00da 0a44 4f5f 4e4f 5448 494e 47da  .....DO_NOTHING.
-00003670: 1070 7265 7061 7261 7469 6f6e 5f74 7970  .preparation_typ
-00003680: 6572 a700 0000 da08 6361 7465 676f 7279  er......category
-00003690: 72a3 0000 00da 0964 7275 675f 7479 7065  r......drug_type
-000036a0: 5a09 756e 6974 5f64 6f73 655a 0c6d 6561  Z.unit_doseZ.mea
-000036b0: 7375 7265 5f75 6e69 745a 116d 6561 7375  sure_unitZ.measu
-000036c0: 7265 5f75 6e69 745f 636f 6465 5a0a 7374  re_unit_codeZ.st
-000036d0: 6f63 6b5f 6c65 6674 5a0a 7374 6f63 6b5f  ock_leftZ.stock_
-000036e0: 756e 6974 5a03 6d69 635a 0c72 6363 5f63  unitZ.micZ.rcc_c
-000036f0: 6174 6567 6f72 7972 1e00 0000 5a0c 6973  ategoryr....Z.is
-00003700: 5f65 7373 656e 7469 616c 5a08 6872 5f6c  _essentialZ.hr_l
-00003710: 6576 656c 5a07 6762 5f63 6f64 655a 0767  evelZ.gb_codeZ.g
-00003720: 625f 6e61 6d65 da0c 6f72 6967 696e 5f70  b_name..origin_p
-00003730: 6c61 6365 da0c 6d61 6e75 6661 6374 7572  lace..manufactur
-00003740: 6572 721a 0000 0072 1800 0000 7218 0000  err....r....r...
-00003750: 0072 1800 0000 7219 0000 0072 a800 0000  .r....r....r....
-00003760: 7701 0000 7344 0000 0008 0110 0112 0112  w...sD..........
-00003770: 0112 0112 0104 0102 0102 0104 fd06 0504  ................
-00003780: 0102 0102 0104 fd06 0504 0102 0102 0104  ................
-00003790: fd06 0512 0112 0112 0112 0112 0112 0112  ................
-000037a0: 010e 0112 0112 0112 0112 0112 0272 a800  .............r..
-000037b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000037c0: 0000 0006 0000 0040 0000 0073 3c00 0000  .......@...s<...
-000037d0: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-000037e0: 6403 6404 8d03 5a05 6503 6a04 6405 6406  d.d...Z.e.j.d.d.
-000037f0: 6403 6403 6407 8d04 5a06 4700 6408 6409  d.d.d...Z.G.d.d.
-00003800: 8400 6409 8302 5a07 640a 5300 290b da0c  ..d...Z.d.S.)...
-00003810: 5068 6172 6d61 6379 5479 7065 722a 0000  PharmacyTyper*..
-00003820: 0072 2200 0000 5472 4700 0000 7221 0000  .r"...TrG...r!..
-00003830: 0072 9500 0000 7227 0000 0063 0000 0000  .r....r'...c....
-00003840: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00003850: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00003860: 0264 015a 0364 025a 0465 045a 0564 0353  .d.Z.d.Z.e.Z.d.S
-00003870: 0029 047a 1150 6861 726d 6163 7954 7970  .).z.PharmacyTyp
-00003880: 652e 4d65 7461 5a10 6273 5f70 6861 726d  e.MetaZ.bs_pharm
-00003890: 6163 795f 7479 7065 f50c 0000 00e8 8daf  acy_type........
-000038a0: e688 bfe7 b1bb e59e 8b4e 7235 0000 0072  .........Nr5...r
-000038b0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-000038c0: 0000 0072 1a00 0000 a401 0000 7306 0000  ...r........s...
-000038d0: 0008 0104 0104 0172 1a00 0000 4e72 a500  .......r....Nr..
-000038e0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-000038f0: 0072 1900 0000 72bd 0000 00a0 0100 0073  .r....r........s
-00003900: 0600 0000 0801 1001 1202 72bd 0000 0063  ..........r....c
-00003910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003920: 0600 0000 4000 0000 733c 0000 0065 005a  ....@...s<...e.Z
-00003930: 0164 005a 0265 036a 0464 0164 0264 0364  .d.Z.e.j.d.d.d.d
-00003940: 048d 035a 0565 036a 0464 0564 0664 0364  ...Z.e.j.d.d.d.d
-00003950: 0364 078d 045a 0647 0064 0864 0984 0064  .d...Z.G.d.d...d
-00003960: 0983 025a 0764 0a53 0029 0bda 1250 6861  ...Z.d.S.)...Pha
-00003970: 726d 6163 7945 6e74 6572 7072 6973 6572  rmacyEnterpriser
-00003980: 2a00 0000 7222 0000 0054 7247 0000 0072  *...r"...TrG...r
-00003990: 2100 0000 7295 0000 0072 2700 0000 6300  !...r....r'...c.
-000039a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000039b0: 0000 0040 0000 0073 1800 0000 6500 5a01  ...@...s....e.Z.
-000039c0: 6400 5a02 6401 5a03 6402 5a04 6504 5a05  d.Z.d.Z.d.Z.e.Z.
-000039d0: 6403 5300 2904 7a17 5068 6172 6d61 6379  d.S.).z.Pharmacy
-000039e0: 456e 7465 7270 7269 7365 2e4d 6574 615a  Enterprise.MetaZ
-000039f0: 1662 735f 7068 6172 6d61 6379 5f65 6e74  .bs_pharmacy_ent
-00003a00: 6572 7072 6973 6575 0c00 0000 e88d afe4  erpriseu........
-00003a10: bc81 e7ae a1e7 9086 4e72 3500 0000 7218  ........Nr5...r.
-00003a20: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00003a30: 0000 721a 0000 00ae 0100 0073 0600 0000  ..r........s....
-00003a40: 0801 0401 0401 721a 0000 004e 72a5 0000  ......r....Nr...
-00003a50: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00003a60: 7219 0000 0072 bf00 0000 aa01 0000 7306  r....r........s.
-00003a70: 0000 0008 0110 0112 0272 bf00 0000 6300  .........r....c.
-00003a80: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00003a90: 0000 0040 0000 0073 8600 0000 6500 5a01  ...@...s....e.Z.
-00003aa0: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-00003ab0: 8d03 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
-00003ac0: 6407 8d04 5a06 6503 6a07 6508 6408 6503  d...Z.e.j.e.d.e.
-00003ad0: 6a09 6409 8d03 5a0a 6503 6a0b 640a 6403  j.d...Z.e.j.d.d.
-00003ae0: 6403 640b 8d03 5a0c 6503 6a07 650d 640c  d.d...Z.e.j.e.d.
-00003af0: 6503 6a0e 6403 640d 8d04 5a0f 6503 6a07  e.j.d.d...Z.e.j.
-00003b00: 6510 640e 6503 6a0e 6403 640d 8d04 5a11  e.d.e.j.d.d...Z.
-00003b10: 4700 640f 6410 8400 6410 8302 5a12 6411  G.d.d...d...Z.d.
-00003b20: 5300 2912 da12 5068 6172 6d61 6379 4d61  S.)...PharmacyMa
-00003b30: 6e61 6765 6d65 6e74 750c 0000 00e8 8daf  nagementu.......
-00003b40: e688 bfe7 bc96 e7a0 8172 2200 0000 5472  .........r"...Tr
-00003b50: 4700 0000 750c 0000 00e8 8daf e688 bfe5  G...u...........
-00003b60: 908d e7a7 b072 9500 0000 7227 0000 0072  .....r....r'...r
-00003b70: be00 0000 7248 0000 0075 0c00 0000 e88d  ....rH...u......
-00003b80: afe6 88bf e59c b0e5 9d80 7229 0000 0072  ..........r)...r
-00003b90: 2e00 0000 722f 0000 0075 0c00 0000 e689  ....r/...u......
-00003ba0: 80e5 b19e e88d afe4 bc81 6300 0000 0000  ..........c.....
-00003bb0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00003bc0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00003bd0: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
-00003be0: 2904 7a17 5068 6172 6d61 6379 4d61 6e61  ).z.PharmacyMana
-00003bf0: 6765 6d65 6e74 2e4d 6574 615a 1662 735f  gement.MetaZ.bs_
-00003c00: 7068 6172 6d61 6379 5f6d 616e 6167 656d  pharmacy_managem
-00003c10: 656e 7475 0c00 0000 e88d afe6 88bf e7ae  entu............
-00003c20: a1e7 9086 4e72 3500 0000 7218 0000 0072  ....Nr5...r....r
-00003c30: 1800 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00003c40: 0000 00ca 0100 0073 0600 0000 0801 0401  .......s........
-00003c50: 0401 721a 0000 004e 2913 7214 0000 0072  ..r....N).r....r
-00003c60: 1500 0000 7216 0000 0072 0500 0000 7238  ....r....r....r8
-00003c70: 0000 005a 0d70 6861 726d 6163 795f 636f  ...Z.pharmacy_co
-00003c80: 6465 5a0d 7068 6172 6d61 6379 5f6e 616d  deZ.pharmacy_nam
-00003c90: 6572 4000 0000 72bd 0000 0072 b700 0000  er@...r....r....
-00003ca0: 5a0d 7068 6172 6d61 6379 5f74 7970 6572  Z.pharmacy_typer
-00003cb0: 3b00 0000 723e 0000 0072 2000 0000 7241  ;...r>...r ...rA
-00003cc0: 0000 0072 4900 0000 72bf 0000 005a 0a65  ...rI...r....Z.e
-00003cd0: 6e74 6572 7072 6973 6572 1a00 0000 7218  nterpriser....r.
-00003ce0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00003cf0: 0000 72c0 0000 00b4 0100 0073 2600 0000  ..r........s&...
-00003d00: 0801 1001 1201 0401 0201 0201 04fd 0607  ................
-00003d10: 1001 0601 0201 0401 02fd 0605 0601 0201  ................
-00003d20: 0401 02fd 0606 72c0 0000 0063 0000 0000  ......r....c....
-00003d30: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003d40: 4000 0000 734e 0100 0065 005a 0164 005a  @...sN...e.Z.d.Z
-00003d50: 0265 036a 0465 0564 0165 036a 0664 0264  .e.j.e.d.e.j.d.d
-00003d60: 038d 045a 0765 036a 0864 0464 0564 0264  ...Z.e.j.d.d.d.d
-00003d70: 0264 068d 045a 0965 036a 0864 0764 0864  .d...Z.e.j.d.d.d
-00003d80: 0264 0264 098d 045a 0a65 036a 0864 0764  .d.d...Z.e.j.d.d
-00003d90: 0a64 0264 0264 098d 045a 0b65 036a 0864  .d.d.d...Z.e.j.d
-00003da0: 0764 0b64 0264 0264 098d 045a 0c65 036a  .d.d.d.d...Z.e.j
-00003db0: 0465 0d64 0c65 036a 0e64 0d8d 035a 0f65  .e.d.e.j.d...Z.e
-00003dc0: 036a 0465 1064 0e65 036a 0e64 0d8d 035a  .j.e.d.e.j.d...Z
-00003dd0: 1165 036a 0465 1264 0f65 036a 0e64 0d8d  .e.j.e.d.e.j.d..
-00003de0: 035a 1365 036a 0864 0764 1064 0264 0264  .Z.e.j.d.d.d.d.d
-00003df0: 098d 045a 1465 036a 0864 0764 1164 0264  ...Z.e.j.d.d.d.d
-00003e00: 0264 098d 045a 1565 036a 0465 1664 1265  .d...Z.e.j.e.d.e
-00003e10: 036a 0664 0264 038d 045a 1765 036a 1864  .j.d.d...Z.e.j.d
-00003e20: 1364 0264 0264 148d 035a 1965 036a 1a64  .d.d.d...Z.e.j.d
-00003e30: 1564 1664 0264 178d 035a 1b65 036a 0864  .d.d.d...Z.e.j.d
-00003e40: 0764 1864 0264 0264 098d 045a 1c65 036a  .d.d.d.d...Z.e.j
-00003e50: 1d64 1964 0264 1a8d 025a 1e65 036a 1d64  .d.d.d...Z.e.j.d
-00003e60: 1b64 0264 1a8d 025a 1f65 036a 1d64 1c64  .d.d...Z.e.j.d.d
-00003e70: 0264 1a8d 025a 2065 036a 1d64 1d64 0264  .d...Z e.j.d.d.d
-00003e80: 1a8d 025a 2147 0064 1e64 1f84 0064 1f83  ...Z!G.d.d...d..
-00003e90: 025a 2264 2053 0029 21da 0c50 6861 726d  .Z"d S.)!..Pharm
-00003ea0: 6163 7944 7275 6775 0c00 0000 e689 80e5  acyDrugu........
-00003eb0: b19e e88d afe6 88bf 5472 2f00 0000 72a9  ........Tr/...r.
-00003ec0: 0000 0072 2200 0000 7227 0000 0072 9500  ...r"...r'...r..
-00003ed0: 0000 72aa 0000 0072 7700 0000 72ab 0000  ..r....rw...r...
-00003ee0: 0072 ac00 0000 72ad 0000 0072 4800 0000  .r....r....rH...
-00003ef0: 72a4 0000 0072 ae00 0000 72b1 0000 0072  r....r....r....r
-00003f00: b200 0000 722e 0000 0075 0c00 0000 e69c  ....r....u......
-00003f10: 89e6 9588 e697 a5e6 9c9f 720f 0000 0072  ..........r....r
-00003f20: b000 0000 7201 0000 0072 7600 0000 72af  ....r....rv...r.
-00003f30: 0000 0075 0c00 0000 e688 90e6 9cac e58d  ...u............
-00003f40: 95e4 bbb7 728e 0000 0075 0c00 0000 e688  ....r....u......
-00003f50: 90e6 9cac e987 91e9 a29d 750c 0000 00e9  ..........u.....
-00003f60: 9bb6 e594 aee5 8d95 e4bb b775 0c00 0000  ...........u....
-00003f70: e99b b6e5 94ae e987 91e9 a29d 6300 0000  ............c...
-00003f80: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00003f90: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00003fa0: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-00003fb0: 5300 2904 7a11 5068 6172 6d61 6379 4472  S.).z.PharmacyDr
-00003fc0: 7567 2e4d 6574 615a 1062 735f 7068 6172  ug.MetaZ.bs_phar
-00003fd0: 6d61 6379 5f64 7275 6775 0d00 0000 e88d  macy_drugu......
-00003fe0: afe6 88bf 2de8 8daf e593 814e 7235 0000  ....-......Nr5..
-00003ff0: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00004000: 7219 0000 0072 1a00 0000 f801 0000 7306  r....r........s.
-00004010: 0000 0008 0104 0104 0172 1a00 0000 4e29  .........r....N)
-00004020: 2372 1400 0000 7215 0000 0072 1600 0000  #r....r....r....
-00004030: 7205 0000 0072 4000 0000 72c0 0000 0072  r....r@...r....r
-00004040: 4100 0000 5a08 7068 6172 6d61 6379 7238  A...Z.pharmacyr8
-00004050: 0000 0072 b300 0000 72b4 0000 0072 b500  ...r....r....r..
-00004060: 0000 72b6 0000 0072 a100 0000 72b7 0000  ..r....r....r...
-00004070: 0072 b800 0000 72a3 0000 0072 ba00 0000  .r....r....r....
-00004080: 72a7 0000 0072 b900 0000 72bb 0000 0072  r....r....r....r
-00004090: bc00 0000 7220 0000 0072 4900 0000 721b  ....r ...rI...r.
-000040a0: 0000 005a 0a76 616c 6964 5f64 6174 6572  ...Z.valid_dater
-000040b0: 6d00 0000 5a12 696e 7665 6e74 6f72 795f  m...Z.inventory_
-000040c0: 7175 616e 7469 7479 5a10 6d65 6173 7572  quantityZ.measur
-000040d0: 656d 656e 745f 756e 6974 723f 0000 005a  ement_unitr?...Z
-000040e0: 0f63 6f73 745f 756e 6974 5f70 7269 6365  .cost_unit_price
-000040f0: 5a0b 636f 7374 5f61 6d6f 756e 745a 1172  Z.cost_amountZ.r
-00004100: 6574 6169 6c5f 756e 6974 5f70 7269 6365  etail_unit_price
-00004110: 5a0d 7265 7461 696c 5f61 6d6f 756e 7472  Z.retail_amountr
-00004120: 1a00 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
-00004130: 0000 0072 1900 0000 72c1 0000 00d0 0100  ...r....r.......
-00004140: 0073 4e00 0000 0801 0601 0201 0401 02fd  .sN.............
-00004150: 0605 1201 1201 1201 1201 0401 0201 0201  ................
-00004160: 04fd 0605 0401 0201 0201 04fd 0605 0401  ................
-00004170: 0201 0201 04fd 0605 1201 1201 0601 0201  ................
-00004180: 0401 02fd 0605 1001 1001 1201 0e01 0e01  ................
-00004190: 0e01 0e02 72c1 0000 0029 1eda 026f 73da  ....r....)...os.
-000041a0: 1a64 6a61 6e67 6f2e 636f 6e74 7269 622e  .django.contrib.
-000041b0: 6175 7468 2e6d 6f64 656c 7372 0200 0000  auth.modelsr....
-000041c0: 7203 0000 00da 2264 6a61 6e67 6f2e 636f  r....."django.co
-000041d0: 6e74 7269 622e 636f 6e74 656e 7474 7970  ntrib.contenttyp
-000041e0: 6573 2e6d 6f64 656c 7372 0400 0000 da09  es.modelsr......
-000041f0: 646a 616e 676f 2e64 6272 0500 0000 7257  django.dbr....rW
-00004200: 0000 00da 054d 6f64 656c 7208 0000 0072  .....Modelr....r
-00004210: 2000 0000 7245 0000 0072 4a00 0000 724b   ...rE...rJ...rK
-00004220: 0000 0072 5d00 0000 7271 0000 0072 7b00  ...r]...rq...r{.
-00004230: 0000 728a 0000 0072 9100 0000 7293 0000  ..r....r....r...
-00004240: 0072 a000 0000 72a1 0000 0072 a300 0000  .r....r....r....
-00004250: 72a7 0000 0072 a800 0000 72bd 0000 0072  r....r....r....r
-00004260: bf00 0000 72c0 0000 0072 c100 0000 7218  ....r....r....r.
-00004270: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00004280: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00004290: 7330 0000 0008 0210 010c 010c 0204 0612  s0..............
-000042a0: 0910 1e10 1910 1110 2510 4f12 1912 1b12  ........%.O.....
-000042b0: 1b10 1610 1110 1110 0a10 0a10 0a10 2910  ..............).
-000042c0: 0a10 0a10 1c                             .....
+00000020: 0004 0000 0040 0000 0073 d801 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6405 6c0a 6d0b 5a0c 0100 650d 650c 6406  d.l.m.Z...e.e.d.
+00000080: 8302 5a0e 6407 5a0f 4700 6408 6409 8400  ..Z.d.Z.G.d.d...
+00000090: 6409 6509 6a10 8303 5a11 4700 640a 640b  d.e.j...Z.G.d.d.
+000000a0: 8400 640b 6511 8303 5a12 4700 640c 640d  ..d.e...Z.G.d.d.
+000000b0: 8400 640d 6511 8303 5a13 4700 640e 640f  ..d.e...Z.G.d.d.
+000000c0: 8400 640f 6511 8303 5a14 4700 6410 6411  ..d.e...Z.G.d.d.
+000000d0: 8400 6411 6511 8303 5a15 4700 6412 6413  ..d.e...Z.G.d.d.
+000000e0: 8400 6413 6504 8303 5a16 4700 6414 6415  ..d.e...Z.G.d.d.
+000000f0: 8400 6415 6509 6a10 8303 5a17 4700 6416  ..d.e.j...Z.G.d.
+00000100: 6417 8400 6417 6509 6a10 8303 5a18 4700  d...d.e.j...Z.G.
+00000110: 6418 6419 8400 6419 6509 6a10 8303 5a19  d.d...d.e.j...Z.
+00000120: 4700 641a 641b 8400 641b 6511 8303 5a1a  G.d.d...d.e...Z.
+00000130: 4700 641c 641d 8400 641d 6511 8303 5a1b  G.d.d...d.e...Z.
+00000140: 4700 641e 641f 8400 641f 6511 8303 5a1c  G.d.d...d.e...Z.
+00000150: 4700 6420 6421 8400 6421 6511 8303 5a1d  G.d d!..d!e...Z.
+00000160: 4700 6422 6423 8400 6423 6511 8303 5a1e  G.d"d#..d#e...Z.
+00000170: 4700 6424 6425 8400 6425 6511 8303 5a1f  G.d$d%..d%e...Z.
+00000180: 4700 6426 6427 8400 6427 6511 8303 5a20  G.d&d'..d'e...Z 
+00000190: 4700 6428 6429 8400 6429 6511 8303 5a21  G.d(d)..d)e...Z!
+000001a0: 4700 642a 642b 8400 642b 6511 8303 5a22  G.d*d+..d+e...Z"
+000001b0: 4700 642c 642d 8400 642d 6511 8303 5a23  G.d,d-..d-e...Z#
+000001c0: 4700 642e 642f 8400 642f 6511 8303 5a24  G.d.d/..d/e...Z$
+000001d0: 4700 6430 6431 8400 6431 6511 8303 5a25  G.d0d1..d1e...Z%
+000001e0: 4700 6432 6433 8400 6433 6511 8303 5a26  G.d2d3..d3e...Z&
+000001f0: 4700 6434 6435 8400 6435 6509 6a10 8303  G.d4d5..d5e.j...
+00000200: 5a27 6401 5300 2936 e900 0000 004e 2902  Z'd.S.)6.....N).
+00000210: da0c 4162 7374 7261 6374 5573 6572 da05  ..AbstractUser..
+00000220: 4772 6f75 7029 01da 0b43 6f6e 7465 6e74  Group)...Content
+00000230: 5479 7065 2901 da06 6d6f 6465 6c73 2901  Type)...models).
+00000240: da08 7365 7474 696e 6773 da0c 5752 4954  ..settings..WRIT
+00000250: 4542 4143 4b5f 4950 2902 2902 da01 3175  EBACK_IP).)...1u
+00000260: 0300 0000 e794 b729 02da 0130 7503 0000  .......)...0u...
+00000270: 00e5 a5b3 6300 0000 0000 0000 0000 0000  ....c...........
+00000280: 0000 0000 0005 0000 0040 0000 0073 4800  .........@...sH.
+00000290: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
+000002a0: 6402 6402 6403 8d03 5a05 6503 6a04 6404  d.d.d...Z.e.j.d.
+000002b0: 6402 6402 6405 8d03 5a06 6503 6a07 6406  d.d.d...Z.e.j.d.
+000002c0: 6402 6407 8d02 5a08 4700 6408 6409 8400  d.d...Z.G.d.d...
+000002d0: 6409 8302 5a09 640a 5300 290b da10 4d65  d...Z.d.S.)...Me
+000002e0: 6469 6361 6c42 6173 654d 6f64 656c f50c  dicalBaseModel..
+000002f0: 0000 00e5 889b e5bb bae6 97b6 e997 b454  ...............T
+00000300: a903 da0c 7665 7262 6f73 655f 6e61 6d65  ....verbose_name
+00000310: da0c 6175 746f 5f6e 6f77 5f61 6464 da04  ..auto_now_add..
+00000320: 6e75 6c6c f50c 0000 00e6 9bb4 e696 b0e6  null............
+00000330: 97b6 e997 b4a9 0372 0d00 0000 da08 6175  .......r......au
+00000340: 746f 5f6e 6f77 720f 0000 00f5 0c00 0000  to_nowr.........
+00000350: e698 afe5 90a6 e590 afe7 94a8 a902 720d  ..............r.
+00000360: 0000 00da 0764 6566 6175 6c74 6300 0000  .....defaultc...
+00000370: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000380: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000390: 5a02 6401 5a03 6402 5300 2903 7a15 4d65  Z.d.Z.d.S.).z.Me
+000003a0: 6469 6361 6c42 6173 654d 6f64 656c 2e4d  dicalBaseModel.M
+000003b0: 6574 6154 4e29 04da 085f 5f6e 616d 655f  etaTN)...__name_
+000003c0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000003d0: 5f71 7561 6c6e 616d 655f 5fda 0861 6273  _qualname__..abs
+000003e0: 7472 6163 74a9 0072 1a00 0000 721a 0000  tract..r....r...
+000003f0: 00fa 372f 686f 6d65 2f6c 7968 2f77 6f72  ..7/home/lyh/wor
+00000400: 6b2f 4261 7365 4675 6e63 7469 6f6e 4d6f  k/BaseFunctionMo
+00000410: 6475 6c65 2f62 6173 655f 7379 7374 656d  dule/base_system
+00000420: 2f6d 6f64 656c 732e 7079 da04 4d65 7461  /models.py..Meta
+00000430: 1700 0000 7302 0000 0008 0172 1c00 0000  ....s......r....
+00000440: 4e29 0a72 1600 0000 7217 0000 0072 1800  N).r....r....r..
+00000450: 0000 7205 0000 00da 0d44 6174 6554 696d  ..r......DateTim
+00000460: 6546 6965 6c64 da0c 6372 6561 7465 645f  eField..created_
+00000470: 7469 6d65 da0c 7570 6461 7465 645f 7469  time..updated_ti
+00000480: 6d65 da0c 426f 6f6c 6561 6e46 6965 6c64  me..BooleanField
+00000490: da09 6973 5f61 6374 6976 6572 1c00 0000  ..is_activer....
+000004a0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+000004b0: 1b00 0000 720a 0000 0012 0000 0073 0800  ....r........s..
+000004c0: 0000 0801 1001 1001 0e02 720a 0000 0063  ..........r....c
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0600 0000 4000 0000 73d8 0000 0065 005a  ....@...s....e.Z
+000004f0: 0164 005a 0265 036a 0464 0164 0264 038d  .d.Z.e.j.d.d.d..
+00000500: 025a 0565 036a 0464 0464 0564 0664 0664  .Z.e.j.d.d.d.d.d
+00000510: 078d 045a 0665 036a 0764 0864 0664 0664  ...Z.e.j.d.d.d.d
+00000520: 098d 035a 0865 036a 0464 0264 0a64 0664  ...Z.e.j.d.d.d.d
+00000530: 0b8d 035a 0965 036a 0764 0c64 0d8d 015a  ...Z.e.j.d.d...Z
+00000540: 0a65 036a 0b64 0e64 0d8d 015a 0c65 036a  .e.j.d.d...Z.e.j
+00000550: 0b64 0f64 0d8d 015a 0d65 036a 0e64 1064  .d.d...Z.e.j.d.d
+00000560: 1165 036a 0f64 0664 128d 045a 1065 036a  .e.j.d.d...Z.e.j
+00000570: 0464 1364 0564 1464 0664 158d 045a 1165  .d.d.d.d.d...Z.e
+00000580: 036a 0464 1664 0564 1764 188d 035a 1265  .j.d.d.d.d...Z.e
+00000590: 036a 0464 1964 0564 0664 0664 078d 045a  .j.d.d.d.d.d...Z
+000005a0: 1365 036a 0464 1a64 0564 0664 0664 078d  .e.j.d.d.d.d.d..
+000005b0: 045a 1447 0064 1b64 1c84 0064 1c83 025a  .Z.G.d.d...d...Z
+000005c0: 1564 1d53 0029 1eda 0848 6f73 7069 7461  .d.S.)...Hospita
+000005d0: 6cf5 0600 0000 e590 8de7 a7b0 e9ff 0000  l...............
+000005e0: 00a9 0272 0d00 0000 da0a 6d61 785f 6c65  ...r......max_le
+000005f0: 6e67 7468 f50c 0000 00e8 8194 e7b3 bbe6  ngth............
+00000600: 96b9 e5bc 8fe9 6400 0000 54a9 0472 0d00  ......d...T..r..
+00000610: 0000 7226 0000 0072 0f00 0000 da05 626c  ..r&...r......bl
+00000620: 616e 6b75 0c00 0000 e58c bbe9 99a2 e7ae  anku............
+00000630: 80e4 bb8b a903 720d 0000 0072 0f00 0000  ......r....r....
+00000640: 722a 0000 00f5 0600 0000 e7bc 96e7 a081  r*..............
+00000650: a903 7226 0000 0072 0d00 0000 da06 756e  ..r&...r......un
+00000660: 6971 7565 750c 0000 00e5 8cbb e999 a2e5  iqueu...........
+00000670: 9cb0 e59d 8029 0172 0d00 0000 7506 0000  .....).r....u...
+00000680: 00e7 bb8f e5ba a675 0600 0000 e7bb b4e5  .......u........
+00000690: baa6 da04 7365 6c66 f50c 0000 00e6 8980  ....self........
+000006a0: e5b1 9ee5 8cbb e999 a2a9 0372 0d00 0000  ...........r....
+000006b0: da09 6f6e 5f64 656c 6574 6572 0f00 0000  ..on_deleter....
+000006c0: 750c 0000 00e5 8cbb e999 a2e5 9bbe e789  u...............
+000006d0: 875a 0f68 6f73 7069 7461 6c5f 696d 6167  .Z.hospital_imag
+000006e0: 6573 2904 720d 0000 0072 2600 0000 7215  es).r....r&...r.
+000006f0: 0000 0072 2a00 0000 da04 6c6f 676f 5a0d  ...r*.....logoZ.
+00000700: 686f 7370 6974 616c 5f6c 6f67 6fa9 0372  hospital_logo..r
+00000710: 0d00 0000 7226 0000 0072 1500 0000 f509  ....r&...r......
+00000720: 0000 00e5 889b e5bb bae4 baba f509 0000  ................
+00000730: 00e6 9bb4 e696 b0e4 baba 6300 0000 0000  ..........c.....
+00000740: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00000750: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000760: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
+00000770: 2904 7a0d 486f 7370 6974 616c 2e4d 6574  ).z.Hospital.Met
+00000780: 615a 0b62 735f 686f 7370 6974 616c 7506  aZ.bs_hospitalu.
+00000790: 0000 00e5 8cbb e999 a24e a906 7216 0000  .........N..r...
+000007a0: 0072 1700 0000 7218 0000 00da 0864 625f  .r....r......db_
+000007b0: 7461 626c 6572 0d00 0000 da13 7665 7262  tabler......verb
+000007c0: 6f73 655f 6e61 6d65 5f70 6c75 7261 6c72  ose_name_pluralr
+000007d0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+000007e0: 0000 0072 1c00 0000 3000 0000 7306 0000  ...r....0...s...
+000007f0: 0008 0104 0104 0172 1c00 0000 4e29 1672  .......r....N).r
+00000800: 1600 0000 7217 0000 0072 1800 0000 7205  ....r....r....r.
+00000810: 0000 00da 0943 6861 7246 6965 6c64 da04  .....CharField..
+00000820: 6e61 6d65 da05 7068 6f6e 65da 0954 6578  name..phone..Tex
+00000830: 7446 6965 6c64 da09 696e 7472 6f64 7563  tField..introduc
+00000840: 65da 0763 6f64 656e 756d da07 6164 6472  e..codenum..addr
+00000850: 6573 73da 0a46 6c6f 6174 4669 656c 645a  ess..FloatFieldZ
+00000860: 096c 6f6e 6769 7475 6465 5a08 6c61 7469  .longitudeZ.lati
+00000870: 7475 6465 da0a 466f 7265 6967 6e4b 6579  tude..ForeignKey
+00000880: da07 4341 5343 4144 45da 0670 6172 656e  ..CASCADE..paren
+00000890: 745a 0a68 6f73 5f69 6d61 6765 7372 3300  tZ.hos_imagesr3.
+000008a0: 0000 da0a 6372 6561 7465 645f 6279 da0a  ....created_by..
+000008b0: 7570 6461 7465 645f 6279 721c 0000 0072  updated_byr....r
+000008c0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+000008d0: 0000 0072 2200 0000 1b00 0000 7324 0000  ...r".......s$..
+000008e0: 0008 010e 0112 0110 0110 010c 010c 010c  ................
+000008f0: 0104 0102 0102 0104 0102 fc06 0712 0210  ................
+00000900: 0112 0112 0272 2200 0000 6300 0000 0000  .....r"...c.....
+00000910: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+00000920: 0000 0073 a200 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000930: 6503 6a04 6401 6402 6403 8d02 5a05 6503  e.j.d.d.d...Z.e.
+00000940: 6a04 6404 6402 6405 6405 6406 8d04 5a06  j.d.d.d.d.d...Z.
+00000950: 6503 6a04 6407 6402 6405 6405 6406 8d04  e.j.d.d.d.d.d...
+00000960: 5a07 6503 6a04 6408 6402 6403 8d02 5a08  Z.e.j.d.d.d...Z.
+00000970: 6503 6a04 6409 640a 6405 6405 6406 8d04  e.j.d.d.d.d.d...
+00000980: 5a09 6503 6a0a 640b 6405 6405 640c 8d03  Z.e.j.d.d.d.d...
+00000990: 5a0b 6503 6a0c 650d 640d 6503 6a0e 640e  Z.e.j.e.d.e.j.d.
+000009a0: 8d03 5a0f 6503 6a0c 640f 6410 6503 6a0e  ..Z.e.j.d.d.e.j.
+000009b0: 6405 6411 8d04 5a10 4700 6412 6413 8400  d.d...Z.G.d.d...
+000009c0: 6413 8302 5a11 6414 5300 2915 da06 4f66  d...Z.d.S.)...Of
+000009d0: 6669 6365 7223 0000 0072 2400 0000 7225  ficer#...r$...r%
+000009e0: 0000 0075 0c00 0000 e7a7 91e5 aea4 e4bd  ...u............
+000009f0: 8de7 bdae 5472 2900 0000 7227 0000 00f5  ....Tr)...r'....
+00000a00: 0c00 0000 e7a7 91e5 aea4 e7bc 96e7 a081  ................
+00000a10: 7506 0000 00e7 b1bb e59e 8b72 2800 0000  u..........r(...
+00000a20: 750c 0000 00e7 a791 e5ae a4e7 ae80 e4bb  u...............
+00000a30: 8b72 2b00 0000 7230 0000 00a9 0272 0d00  .r+...r0.....r..
+00000a40: 0000 7232 0000 0072 2f00 0000 750c 0000  ..r2...r/...u...
+00000a50: 00e4 b88a e7ba a7e7 a791 e5ae a472 3100  .............r1.
+00000a60: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000a70: 0000 0001 0000 0040 0000 0073 1c00 0000  .......@...s....
+00000a80: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00000a90: 6504 5a05 6403 5a06 6404 5300 2905 7a0b  e.Z.d.Z.d.S.).z.
+00000aa0: 4f66 6669 6365 2e4d 6574 615a 0962 735f  Office.MetaZ.bs_
+00000ab0: 6f66 6669 6365 7506 0000 00e7 a791 e5ae  officeu.........
+00000ac0: a4a9 0129 0272 3f00 0000 da08 686f 7370  ...).r?.....hosp
+00000ad0: 6974 616c 4ea9 0772 1600 0000 7217 0000  italN..r....r...
+00000ae0: 0072 1800 0000 7238 0000 0072 0d00 0000  .r....r8...r....
+00000af0: 7239 0000 00da 0f75 6e69 7175 655f 746f  r9.....unique_to
+00000b00: 6765 7468 6572 721a 0000 0072 1a00 0000  getherr....r....
+00000b10: 721a 0000 0072 1b00 0000 721c 0000 004c  r....r....r....L
+00000b20: 0000 0073 0800 0000 0801 0401 0401 0401  ...s............
+00000b30: 721c 0000 004e 2912 7216 0000 0072 1700  r....N).r....r..
+00000b40: 0000 7218 0000 0072 0500 0000 723a 0000  ..r....r....r:..
+00000b50: 0072 3b00 0000 7240 0000 0072 3c00 0000  .r;...r@...r<...
+00000b60: 723f 0000 005a 0b6f 6666 6963 655f 7479  r?...Z.office_ty
+00000b70: 7065 723d 0000 0072 3e00 0000 7242 0000  per=...r>...rB..
+00000b80: 0072 2200 0000 7243 0000 0072 4b00 0000  .r"...rC...rK...
+00000b90: 7244 0000 0072 1c00 0000 721a 0000 0072  rD...r....r....r
+00000ba0: 1a00 0000 721a 0000 0072 1b00 0000 7247  ....r....r....rG
+00000bb0: 0000 0039 0000 0073 2400 0000 0801 0e01  ...9...s$.......
+00000bc0: 1201 1201 0e01 1201 1001 0401 0201 0201  ................
+00000bd0: 04fd 0605 0401 0201 0201 0401 02fc 0607  ................
+00000be0: 7247 0000 0063 0000 0000 0000 0000 0000  rG...c..........
+00000bf0: 0000 0000 0000 0600 0000 4000 0000 736c  ..........@...sl
+00000c00: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00000c10: 0164 0264 038d 025a 0565 036a 0464 0464  .d.d...Z.e.j.d.d
+00000c20: 0264 038d 025a 0665 036a 0765 0864 0565  .d...Z.e.j.e.d.e
+00000c30: 036a 0964 068d 035a 0a65 036a 0464 0764  .j.d...Z.e.j.d.d
+00000c40: 0864 0964 0964 0a8d 045a 0b65 036a 0464  .d.d.d...Z.e.j.d
+00000c50: 0b64 0864 0964 0964 0a8d 045a 0c47 0064  .d.d.d.d...Z.G.d
+00000c60: 0c64 0d84 0064 0d83 025a 0d64 0e53 0029  .d...d...Z.d.S.)
+00000c70: 0fda 0d50 6f73 6974 696f 6e54 6974 6c65  ...PositionTitle
+00000c80: 7223 0000 0072 2400 0000 7225 0000 0075  r#...r$...r%...u
+00000c90: 0c00 0000 e881 8ce7 a7b0 e7bc 96e7 a081  ................
+00000ca0: 7230 0000 0072 4900 0000 7235 0000 0072  r0...rI...r5...r
+00000cb0: 2800 0000 5472 2900 0000 7236 0000 0063  (...Tr)...r6...c
+00000cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000cd0: 0100 0000 4000 0000 731c 0000 0065 005a  ....@...s....e.Z
+00000ce0: 0164 005a 0264 015a 0364 025a 0465 045a  .d.Z.d.Z.d.Z.e.Z
+00000cf0: 0564 035a 0664 0453 0029 057a 1250 6f73  .d.Z.d.S.).z.Pos
+00000d00: 6974 696f 6e54 6974 6c65 2e4d 6574 615a  itionTitle.MetaZ
+00000d10: 1162 735f 706f 7369 7469 6f6e 5f74 6974  .bs_position_tit
+00000d20: 6c65 f506 0000 00e8 818c e7a7 b072 4a00  le...........rJ.
+00000d30: 0000 4e72 4c00 0000 721a 0000 0072 1a00  ..NrL...r....r..
+00000d40: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000d50: 0060 0000 0073 0800 0000 0801 0401 0401  .`...s..........
+00000d60: 0401 721c 0000 004e 290e 7216 0000 0072  ..r....N).r....r
+00000d70: 1700 0000 7218 0000 0072 0500 0000 723a  ....r....r....r:
+00000d80: 0000 0072 3b00 0000 723f 0000 0072 4200  ...r;...r?...rB.
+00000d90: 0000 7222 0000 0072 4300 0000 724b 0000  ..r"...rC...rK..
+00000da0: 0072 4500 0000 7246 0000 0072 1c00 0000  .rE...rF...r....
+00000db0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00000dc0: 1b00 0000 724e 0000 0055 0000 0073 1400  ....rN...U...s..
+00000dd0: 0000 0801 0e01 0e01 0401 0201 0201 04fd  ................
+00000de0: 0605 1201 1202 724e 0000 0063 0000 0000  ......rN...c....
+00000df0: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+00000e00: 4000 0000 734e 0100 0065 005a 0164 005a  @...sN...e.Z.d.Z
+00000e10: 0265 036a 0464 0164 0264 038d 025a 0565  .e.j.d.d.d...Z.e
+00000e20: 036a 0464 0464 0264 0564 0564 068d 045a  .j.d.d.d.d.d...Z
+00000e30: 0665 036a 0464 0764 0864 0564 0564 068d  .e.j.d.d.d.d.d..
+00000e40: 045a 0765 036a 0464 0964 0a64 0564 0564  .Z.e.j.d.d.d.d.d
+00000e50: 068d 045a 0865 036a 0464 0b64 0c64 038d  ...Z.e.j.d.d.d..
+00000e60: 025a 0965 036a 0464 0d64 0264 0564 0564  .Z.e.j.d.d.d.d.d
+00000e70: 068d 045a 0a65 036a 0b65 0c64 0e65 036a  ...Z.e.j.e.d.e.j
+00000e80: 0d64 0f8d 035a 0e65 036a 0464 1064 1165  .d...Z.e.j.d.d.e
+00000e90: 0f64 0564 0564 128d 055a 1065 036a 0464  .d.d.d...Z.e.j.d
+00000ea0: 1364 1464 0564 0564 068d 045a 1165 036a  .d.d.d.d...Z.e.j
+00000eb0: 0464 1564 0864 0564 0564 068d 045a 1265  .d.d.d.d.d...Z.e
+00000ec0: 036a 0b65 1364 1665 036a 0d64 0f8d 035a  .j.e.d.e.j.d...Z
+00000ed0: 1465 036a 0b65 1564 1765 036a 0d64 0f8d  .e.j.e.d.e.j.d..
+00000ee0: 035a 1665 036a 1764 1864 0564 0564 198d  .Z.e.j.d.d.d.d..
+00000ef0: 035a 1865 036a 0464 1a64 1464 1b64 1c8d  .Z.e.j.d.d.d.d..
+00000f00: 035a 1965 036a 1a64 1d64 0564 0564 198d  .Z.e.j.d.d.d.d..
+00000f10: 035a 1b65 036a 0464 1e64 0264 0564 0564  .Z.e.j.d.d.d.d.d
+00000f20: 068d 045a 1c65 036a 0464 1f64 0264 0564  ...Z.e.j.d.d.d.d
+00000f30: 0564 068d 045a 1d65 036a 1e64 2064 0564  .d...Z.e.j.d d.d
+00000f40: 218d 025a 1f47 0064 2264 2384 0064 2383  !..Z.G.d"d#..d#.
+00000f50: 025a 2064 2453 0029 25da 0644 6f63 746f  .Z d$S.)%..Docto
+00000f60: 7272 2300 0000 e914 0000 0072 2500 0000  rr#........r%...
+00000f70: 7227 0000 0054 7229 0000 0075 0600 0000  r'...Tr)...u....
+00000f80: e982 aee7 aeb1 7228 0000 0075 0600 0000  ......r(...u....
+00000f90: e59c b0e5 9d80 7224 0000 0075 0600 0000  ......r$...u....
+00000fa0: e5b7 a5e5 8fb7 e940 0000 0075 0600 0000  .......@...u....
+00000fb0: e881 8ce4 bd8d 724f 0000 0072 4900 0000  ......rO...rI...
+00000fc0: f506 0000 00e6 80a7 e588 abe9 0200 0000  ................
+00000fd0: a905 720d 0000 0072 2600 0000 da07 6368  ..r....r&.....ch
+00000fe0: 6f69 6365 7372 0f00 0000 722a 0000 0075  oicesr....r*...u
+00000ff0: 0600 0000 e6b0 91e6 978f e90a 0000 00f5  ................
+00001000: 0c00 0000 e8ba abe4 bbbd e8af 81e5 8fb7  ................
+00001010: f50c 0000 00e6 8980 e5b1 9ee7 a791 e5ae  ................
+00001020: a472 3000 0000 f50c 0000 00e5 87ba e794  .r0.............
+00001030: 9fe6 97a5 e69c 9f72 2b00 0000 750c 0000  .......r+...u...
+00001040: 00e5 8cbb e794 9fe7 85a7 e789 875a 0c64  .............Z.d
+00001050: 6f63 746f 725f 7068 6f74 6f72 3400 0000  octor_photor4...
+00001060: 750c 0000 00e5 8cbb e794 9fe6 8f8f e8bf  u...............
+00001070: b072 3500 0000 7236 0000 0075 1500 0000  .r5...r6...u....
+00001080: e698 afe5 90a6 e4ba 92e8 8194 e7bd 91e6  ................
+00001090: 8ea5 e8af 8a72 1400 0000 6300 0000 0000  .....r....c.....
+000010a0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000010b0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000010c0: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
+000010d0: 2904 7a0b 446f 6374 6f72 2e4d 6574 615a  ).z.Doctor.MetaZ
+000010e0: 0962 735f 646f 6374 6f72 7509 0000 00e5  .bs_doctoru.....
+000010f0: 8cbb e794 9fe8 a1a8 4e72 3700 0000 721a  ........Nr7...r.
+00001100: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00001110: 0000 721c 0000 008b 0000 0073 0600 0000  ..r........s....
+00001120: 0801 0401 0401 721c 0000 004e 2921 7216  ......r....N)!r.
+00001130: 0000 0072 1700 0000 7218 0000 0072 0500  ...r....r....r..
+00001140: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+00001150: 00da 0565 6d61 696c 7240 0000 0072 3f00  ...emailr@...r?.
+00001160: 0000 da08 706f 7369 7469 6f6e 7242 0000  ....positionrB..
+00001170: 0072 4e00 0000 7243 0000 005a 0e70 6f73  .rN...rC...Z.pos
+00001180: 6974 696f 6e5f 7469 746c 65da 0d47 454e  ition_title..GEN
+00001190: 4445 525f 4348 4f49 4345 da06 6765 6e64  DER_CHOICE..gend
+000011a0: 6572 5a06 6e61 7469 6f6e 5a05 6964 6e75  erZ.nationZ.idnu
+000011b0: 6d72 4700 0000 da06 6f66 6669 6365 7222  mrG.....officer"
+000011c0: 0000 0072 4b00 0000 da09 4461 7465 4669  ...rK.....DateFi
+000011d0: 656c 64da 0862 6972 7468 6461 795a 0570  eld..birthdayZ.p
+000011e0: 686f 746f 723d 0000 00da 0864 6573 6372  hotor=.....descr
+000011f0: 6962 6572 4500 0000 7246 0000 0072 2000  iberE...rF...r .
+00001200: 0000 5a11 6973 5f6f 6e6c 696e 655f 636f  ..Z.is_online_co
+00001210: 6e73 756c 7472 1c00 0000 721a 0000 0072  nsultr....r....r
+00001220: 1a00 0000 721a 0000 0072 1b00 0000 7250  ....r....r....rP
+00001230: 0000 0069 0000 0073 3e00 0000 0801 0e01  ...i...s>.......
+00001240: 1201 1201 1201 0e01 1201 0401 0201 0201  ................
+00001250: 04fd 0605 1401 1201 1201 0401 0201 0201  ................
+00001260: 04fd 0605 0401 0201 0201 04fd 0605 1002  ................
+00001270: 1001 1001 1201 1202 0e02 7250 0000 0063  ..........rP...c
+00001280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001290: 0700 0000 4000 0000 736e 0100 0065 005a  ....@...sn...e.Z
+000012a0: 0164 005a 0265 036a 0464 0164 0264 0364  .d.Z.e.j.d.d.d.d
+000012b0: 0364 048d 045a 0565 036a 0464 0564 0664  .d...Z.e.j.d.d.d
+000012c0: 0364 0364 048d 045a 0665 036a 0764 0764  .d.d...Z.e.j.d.d
+000012d0: 0364 0364 088d 035a 0865 036a 0464 0964  .d.d...Z.e.j.d.d
+000012e0: 0a65 0964 0364 0364 0b8d 055a 0a65 036a  .e.d.d.d...Z.e.j
+000012f0: 0464 0c64 0664 0364 0364 048d 045a 0b65  .d.d.d.d.d...Z.e
+00001300: 036a 0c64 0d64 0e64 0364 0364 0f8d 045a  .j.d.d.d.d.d...Z
+00001310: 0d65 036a 0e65 0f64 1065 036a 1064 0364  .e.j.e.d.e.j.d.d
+00001320: 118d 045a 1165 036a 0e65 1264 1265 036a  ...Z.e.j.e.d.e.j
+00001330: 1064 0364 118d 045a 1365 036a 0e65 1464  .d.d...Z.e.j.e.d
+00001340: 1365 036a 1064 0364 118d 045a 1565 036a  .e.j.d.d...Z.e.j
+00001350: 0464 1464 0664 1564 168d 035a 1665 036a  .d.d.d.d...Z.e.j
+00001360: 0464 1764 0264 0364 0364 048d 045a 1765  .d.d.d.d.d...Z.e
+00001370: 036a 0464 1864 0264 0364 0364 048d 045a  .j.d.d.d.d.d...Z
+00001380: 1865 036a 1964 1964 0364 0364 088d 035a  .e.j.d.d.d.d...Z
+00001390: 1a65 036a 0464 1a64 0664 0364 0364 048d  .e.j.d.d.d.d.d..
+000013a0: 045a 1b65 036a 0464 1b64 0664 0364 0364  .Z.e.j.d.d.d.d.d
+000013b0: 048d 045a 1c65 036a 1d64 1c64 0364 0364  ...Z.e.j.d.d.d.d
+000013c0: 1d8d 035a 1e65 036a 1d64 1e64 0364 0364  ...Z.e.j.d.d.d.d
+000013d0: 1f8d 035a 1f47 0064 2064 2184 0064 2183  ...Z.G.d d!..d!.
+000013e0: 025a 2065 2164 2264 2384 0083 015a 2265  .Z e!d"d#....Z"e
+000013f0: 2164 2464 2584 0083 015a 2365 2164 2664  !d$d%....Z#e!d&d
+00001400: 2784 0083 015a 2464 2853 0029 29da 0455  '....Z$d(S.))..U
+00001410: 7365 7272 2300 0000 7224 0000 0054 7229  serr#...r$...Tr)
+00001420: 0000 0072 2700 0000 7228 0000 0072 5a00  ...r'...r(...rZ.
+00001430: 0000 722b 0000 0072 5300 0000 7254 0000  ..r+...rS...rT..
+00001440: 0072 5500 0000 7258 0000 00f5 0600 0000  .rU...rX........
+00001450: e68e 92e5 ba8f e901 0000 00a9 0472 0d00  .............r..
+00001460: 0000 7215 0000 0072 0f00 0000 722a 0000  ..r....r....r*..
+00001470: 0072 5900 0000 7231 0000 0072 3000 0000  .rY...r1...r0...
+00001480: 750c 0000 00e7 bb91 e5ae 9ae5 8cbb e794  u...............
+00001490: 9f75 0c00 0000 e794 a8e6 88b7 e5a4 b4e5  .u..............
+000014a0: 838f 5a0b 7573 6572 5f61 7661 7461 7272  ..Z.user_avatarr
+000014b0: 3400 0000 750c 0000 00e9 bb98 e8ae a4e8  4...u...........
+000014c0: a792 e889 b275 0f00 0000 e58f afe6 938d  .....u..........
+000014d0: e4bd 9ce7 a791 e5ae a475 0c00 0000 e6b3  .........u......
+000014e0: a8e9 878a e8af b4e6 988e 7235 0000 0072  ..........r5...r
+000014f0: 3600 0000 720b 0000 0072 0c00 0000 7210  6...r....r....r.
+00001500: 0000 0072 1100 0000 6300 0000 0000 0000  ...r....c.......
+00001510: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00001520: 0073 1000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001530: 5a03 6402 5300 2903 7a09 5573 6572 2e4d  Z.d.S.).z.User.M
+00001540: 6574 6175 0c00 0000 e794 a8e6 88b7 e4bf  etau............
+00001550: a1e6 81af 4e29 0472 1600 0000 7217 0000  ....N).r....r...
+00001560: 0072 1800 0000 720d 0000 0072 1a00 0000  .r....r....r....
+00001570: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00001580: 1c00 0000 b400 0000 7302 0000 0008 0272  ........s......r
+00001590: 1c00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000015a0: 0002 0000 0002 0000 0043 0000 0073 1800  .........C...s..
+000015b0: 0000 7c00 6a00 7d01 7c01 7314 7c00 6a01  ..|.j.}.|.s.|.j.
+000015c0: a002 a100 7d01 7c01 5300 2901 758e 0000  ....}.|.S.).u...
+000015d0: 000a 2020 2020 2020 2020 e88e b7e5 8f96  ..        ......
+000015e0: e5bd 93e5 898d e794 a8e6 88b7 e9bb 98e8  ................
+000015f0: aea4 e794 a8e6 88b7 e7bb 842c 0a20 2020  ...........,.   
+00001600: 2020 2020 20e5 a682 e69e 9ce6 9caa e8ae       ...........
+00001610: bee7 bdae efbc 8ce8 bf94 e59b 9ee7 acac  ................
+00001620: e4b8 80e4 b8aa e794 a8e6 88b7 e7bb 840a  ................
+00001630: 2020 2020 2020 2020 e590 a6e5 8899 e8bf          ........
+00001640: 94e5 9b9e e8ae bee7 bdae e79a 84e7 94a8  ................
+00001650: e688 b7e7 bb84 0a20 2020 2020 2020 2029  .......        )
+00001660: 035a 0d64 6566 6175 6c74 5f67 726f 7570  .Z.default_group
+00001670: da06 6772 6f75 7073 da05 6669 7273 74a9  ..groups..first.
+00001680: 0272 2f00 0000 5a09 7265 745f 6772 6f75  .r/...Z.ret_grou
+00001690: 7072 1a00 0000 721a 0000 0072 1b00 0000  pr....r....r....
+000016a0: da11 6765 745f 6465 6661 756c 745f 6772  ..get_default_gr
+000016b0: 6f75 70bc 0000 0073 0800 0000 0007 0601  oup....s........
+000016c0: 0401 0a01 7a16 5573 6572 2e67 6574 5f64  ....z.User.get_d
+000016d0: 6566 6175 6c74 5f67 726f 7570 6301 0000  efault_groupc...
+000016e0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000016f0: 0043 0000 0073 1c00 0000 7c00 6a00 a001  .C...s....|.j...
+00001700: a100 7d01 7c01 7318 7c00 6a00 a002 a100  ..}.|.s.|.j.....
+00001710: 7d01 7c01 5300 a901 4e29 0372 6700 0000  }.|.S...N).rg...
+00001720: da03 616c 6cda 046e 6f6e 6572 6900 0000  ..all..noneri...
+00001730: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00001740: 0d67 6574 5f61 6c6c 6772 6f75 7073 c800  .get_allgroups..
+00001750: 0000 7308 0000 0000 020a 0104 010a 017a  ..s............z
+00001760: 1255 7365 722e 6765 745f 616c 6c67 726f  .User.get_allgro
+00001770: 7570 7363 0100 0000 0000 0000 0000 0000  upsc............
+00001780: 0200 0000 0100 0000 4300 0000 7318 0000  ........C...s...
+00001790: 0064 017d 017c 006a 007d 017c 0173 147c  .d.}.|.j.}.|.s.|
+000017a0: 006a 017d 017c 0153 0029 0275 3300 0000  .j.}.|.S.).u3...
+000017b0: 0a20 2020 2020 2020 20e8 8eb7 e58f 96e7  .        .......
+000017c0: 94a8 e688 b7e9 bb98 e8ae a4e7 9a84 e7bb  ................
+000017d0: 84e7 bb87 e69c bae6 9e84 0a20 2020 2020  ...........     
+000017e0: 2020 204e 2902 725f 0000 0072 4b00 0000     N).r_...rK...
+000017f0: 2902 722f 0000 005a 0772 6574 5f6f 7267  ).r/...Z.ret_org
+00001800: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00001810: 1867 6574 5f64 6566 6175 6c74 5f6f 7267  .get_default_org
+00001820: 616e 697a 6174 696f 6ecf 0000 0073 0a00  anization....s..
+00001830: 0000 0005 0401 0601 0401 0601 7a1d 5573  ............z.Us
+00001840: 6572 2e67 6574 5f64 6566 6175 6c74 5f6f  er.get_default_o
+00001850: 7267 616e 697a 6174 696f 6e4e 2925 7216  rganizationN)%r.
+00001860: 0000 0072 1700 0000 7218 0000 0072 0500  ...r....r....r..
+00001870: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+00001880: 0072 6000 0000 7261 0000 0072 5d00 0000  .r`...ra...r]...
+00001890: 725e 0000 005a 0969 6463 6172 646e 756d  r^...Z.idcardnum
+000018a0: da0c 496e 7465 6765 7246 6965 6c64 da08  ..IntegerField..
+000018b0: 6f72 6465 725f 6279 7242 0000 0072 4700  order_byrB...rG.
+000018c0: 0000 7243 0000 0072 5f00 0000 7222 0000  ..rC...r_...r"..
+000018d0: 0072 4b00 0000 7250 0000 005a 0664 6f63  .rK...rP...Z.doc
+000018e0: 746f 725a 0a61 7661 7461 725f 7572 6c5a  torZ.avatar_urlZ
+000018f0: 1064 6566 6175 6c74 5f67 726f 7570 5f69  .default_group_i
+00001900: 645a 0c61 6c6c 6f77 5f6f 6666 6963 6572  dZ.allow_officer
+00001910: 3d00 0000 da04 6e6f 7465 7245 0000 0072  =.....noterE...r
+00001920: 4600 0000 721d 0000 0072 1e00 0000 721f  F...r....r....r.
+00001930: 0000 0072 1c00 0000 da08 7072 6f70 6572  ...r......proper
+00001940: 7479 726a 0000 0072 6e00 0000 726f 0000  tyrj...rn...ro..
+00001950: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00001960: 721b 0000 0072 6300 0000 9100 0000 734e  r....rc.......sN
+00001970: 0000 0008 0112 0112 0110 0114 0112 0112  ................
+00001980: 0104 0102 0102 0104 0102 fc06 0604 0102  ................
+00001990: 0102 0104 0102 fc06 0604 0102 0102 0104  ................
+000019a0: 0102 fc06 0710 0112 0112 0110 0112 0112  ................
+000019b0: 0110 0110 020e 0802 010a 0b02 010a 0602  ................
+000019c0: 0172 6300 0000 6300 0000 0000 0000 0000  .rc...c.........
+000019d0: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
+000019e0: ca00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+000019f0: 6504 6a05 6506 6504 6a07 6402 6403 6403  e.j.e.e.j.d.d.d.
+00001a00: 6404 8d05 5a08 6504 6a09 6405 6406 6403  d...Z.e.j.d.d.d.
+00001a10: 6407 8d03 5a0a 6504 6a09 6405 6408 6409  d...Z.e.j.d.d.d.
+00001a20: 8d02 5a0b 6504 6a0c 6403 640a 6403 640b  ..Z.e.j.d.d.d.d.
+00001a30: 8d03 5a0d 6504 6a09 640c 6405 6403 6403  ..Z.e.j.d.d.d.d.
+00001a40: 640d 8d04 5a0e 6504 6a0f 6510 640e 6504  d...Z.e.j.e.d.e.
+00001a50: 6a07 640f 6410 8d04 5a11 6504 6a12 6411  j.d.d...Z.e.j.d.
+00001a60: 6412 6403 6413 8d03 5a13 6504 6a09 6405  d.d.d...Z.e.j.d.
+00001a70: 6414 6403 6403 6415 8d04 5a14 6504 6a15  d.d.d.d...Z.e.j.
+00001a80: 6416 6403 6403 6417 8d03 5a16 6504 6a15  d.d.d.d...Z.e.j.
+00001a90: 6418 6403 6403 6419 8d03 5a17 4700 641a  d.d.d.d...Z.G.d.
+00001aa0: 641b 8400 641b 8302 5a18 641c 5300 291d  d...d...Z.d.S.).
+00001ab0: da0a 4578 7472 6147 726f 7570 7519 0000  ..ExtraGroupu...
+00001ac0: 000a 2020 2020 e8a7 92e8 89b2 e689 a9e5  ..    ..........
+00001ad0: 8585 e8a1 a80a 2020 2020 da0b 6578 7472  ......    ..extr
+00001ae0: 615f 6772 6f75 7054 2904 7232 0000 00da  a_groupT).r2....
+00001af0: 0c72 656c 6174 6564 5f6e 616d 6572 0f00  .related_namer..
+00001b00: 0000 722a 0000 00e9 3200 0000 750c 0000  ..r*....2...u...
+00001b10: 00e8 a792 e889 b2e4 bba3 e7a0 8172 2d00  .............r-.
+00001b20: 0000 750c 0000 00e8 a792 e889 b2e5 908d  ..u.............
+00001b30: e7a7 b0a9 0272 2600 0000 720d 0000 0072  .....r&...r....r
+00001b40: 1300 0000 2903 7215 0000 0072 0d00 0000  ....).r....r....
+00001b50: 720f 0000 0075 0600 0000 e68f 8fe8 bfb0  r....u..........
+00001b60: 2903 7226 0000 0072 0f00 0000 722a 0000  ).r&...r....r*..
+00001b70: 0072 3000 0000 7267 0000 00a9 0372 0d00  .r0...rg.....r..
+00001b80: 0000 7232 0000 0072 7600 0000 7264 0000  ..r2...rv...rd..
+00001b90: 0072 6500 0000 a903 720d 0000 0072 1500  .re.....r....r..
+00001ba0: 0000 720f 0000 0072 3500 0000 a904 7226  ..r....r5.....r&
+00001bb0: 0000 0072 0d00 0000 720f 0000 0072 2a00  ...r....r....r*.
+00001bc0: 0000 720b 0000 0072 0c00 0000 7512 0000  ..r....r....u...
+00001bd0: 00e6 9c80 e590 8ee6 9bb4 e696 b0e6 97b6  ................
+00001be0: e997 b472 1100 0000 6300 0000 0000 0000  ...r....c.......
+00001bf0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00001c00: 0073 1800 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001c10: 5a03 6402 5a04 6504 5a05 6403 5300 2904  Z.d.Z.e.Z.d.S.).
+00001c20: 7a0f 4578 7472 6147 726f 7570 2e4d 6574  z.ExtraGroup.Met
+00001c30: 615a 0e62 735f 6578 7472 615f 6772 6f75  aZ.bs_extra_grou
+00001c40: 7075 0600 0000 e8a7 92e8 89b2 4e72 3700  pu..........Nr7.
+00001c50: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00001c60: 0072 1b00 0000 721c 0000 00ef 0000 0073  .r....r........s
+00001c70: 0600 0000 0801 0401 0401 721c 0000 004e  ..........r....N
+00001c80: 2919 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
+00001c90: 00da 075f 5f64 6f63 5f5f 7205 0000 00da  ...__doc__r.....
+00001ca0: 0d4f 6e65 546f 4f6e 6546 6965 6c64 7203  .OneToOneFieldr.
+00001cb0: 0000 0072 4300 0000 da05 6772 6f75 7072  ...rC.....groupr
+00001cc0: 3a00 0000 5a09 726f 6c65 5f63 6f64 655a  :...Z.role_codeZ
+00001cd0: 0972 6f6c 655f 6e61 6d65 7220 0000 0072  .role_namer ...r
+00001ce0: 2100 0000 7272 0000 0072 4200 0000 7222  !...rr...rB...r"
+00001cf0: 0000 0072 4b00 0000 7270 0000 0072 7100  ...rK...rp...rq.
+00001d00: 0000 5a0c 6372 6561 7465 645f 7573 6572  ..Z.created_user
+00001d10: 721d 0000 005a 0a63 7265 6174 6564 5f61  r....Z.created_a
+00001d20: 745a 0a75 7064 6174 6564 5f61 7472 1c00  tZ.updated_atr..
+00001d30: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00001d40: 0072 1b00 0000 7274 0000 00db 0000 0073  .r....rt.......s
+00001d50: 2200 0000 0801 0403 1601 1001 0e01 1001  "...............
+00001d60: 1201 0401 0201 0201 0401 02fc 0606 1001  ................
+00001d70: 1201 1001 1002 7274 0000 0063 0000 0000  ......rt...c....
+00001d80: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+00001d90: 4000 0000 738c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00001da0: 0264 015a 0365 046a 0564 0264 0364 048d  .d.Z.e.j.d.d.d..
+00001db0: 025a 0665 046a 0764 0564 0664 078d 025a  .Z.e.j.d.d.d...Z
+00001dc0: 0865 046a 0964 0864 0964 0664 0a8d 035a  .e.j.d.d.d.d...Z
+00001dd0: 0a65 046a 0964 0b64 0964 0664 0664 0c8d  .e.j.d.d.d.d.d..
+00001de0: 045a 0b65 046a 0564 0d64 0e64 0664 0664  .Z.e.j.d.d.d.d.d
+00001df0: 0f8d 045a 0c65 046a 0d64 1064 1165 046a  ...Z.e.j.d.d.e.j
+00001e00: 0e64 1264 0664 138d 055a 0f47 0064 1464  .d.d.d...Z.G.d.d
+00001e10: 1584 0064 1583 025a 1064 1664 1784 005a  ...d...Z.d.d...Z
+00001e20: 1164 1853 0029 19da 1043 6f6e 7465 6e74  .d.S.)...Content
+00001e30: 5479 7065 4361 7465 7375 1600 0000 0a20  TypeCatesu..... 
+00001e40: 2020 20e8 8f9c e58d 95e5 908d e7a7 b00a     .............
+00001e50: 2020 2020 7223 0000 0072 5100 0000 2901      r#...rQ...).
+00001e60: 7226 0000 0072 1300 0000 5429 0172 1500  r&...r....T).r..
+00001e70: 0000 7264 0000 0072 6500 0000 727a 0000  ..rd...re...rz..
+00001e80: 0075 0600 0000 e7ba a7e5 88ab 7266 0000  .u..........rf..
+00001e90: 00f5 0600 0000 e59b bee6 a087 e9f4 0100  ................
+00001ea0: 0072 2900 0000 722f 0000 0075 0c00 0000  .r)...r/...u....
+00001eb0: e788 b6e7 baa7 e88f 9ce5 8d95 da08 6368  ..............ch
+00001ec0: 696c 6472 656e a904 720d 0000 0072 3200  ildren..r....r2.
+00001ed0: 0000 7276 0000 0072 0f00 0000 6300 0000  ..rv...r....c...
+00001ee0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00001ef0: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001f00: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
+00001f10: 5a06 6404 5300 2905 7a15 436f 6e74 656e  Z.d.S.).z.Conten
+00001f20: 7454 7970 6543 6174 6573 2e4d 6574 615a  tTypeCates.MetaZ
+00001f30: 1462 735f 636f 6e74 656e 745f 7479 7065  .bs_content_type
+00001f40: 5f63 6174 7375 0c00 0000 e88f 9ce5 8d95  _catsu..........
+00001f50: e590 8de7 a7b0 a901 7271 0000 004e a907  ........rq...N..
+00001f60: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001f70: 3800 0000 720d 0000 0072 3900 0000 da08  8...r....r9.....
+00001f80: 6f72 6465 7269 6e67 721a 0000 0072 1a00  orderingr....r..
+00001f90: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00001fa0: 0006 0100 0073 0800 0000 0801 0401 0401  .....s..........
+00001fb0: 0401 721c 0000 0063 0100 0000 0000 0000  ..r....c........
+00001fc0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00001fd0: 7306 0000 007c 006a 0053 0072 6b00 0000  s....|.j.S.rk...
+00001fe0: a901 723b 0000 00a9 0172 2f00 0000 721a  ..r;.....r/...r.
+00001ff0: 0000 0072 1a00 0000 721b 0000 00da 075f  ...r....r......_
+00002000: 5f73 7472 5f5f 0c01 0000 7302 0000 0000  _str__....s.....
+00002010: 017a 1843 6f6e 7465 6e74 5479 7065 4361  .z.ContentTypeCa
+00002020: 7465 732e 5f5f 7374 725f 5f4e 2912 7216  tes.__str__N).r.
+00002030: 0000 0072 1700 0000 7218 0000 0072 7c00  ...r....r....r|.
+00002040: 0000 7205 0000 0072 3a00 0000 723b 0000  ..r....r:...r;..
+00002050: 0072 2000 0000 7221 0000 0072 7000 0000  .r ...r!...rp...
+00002060: 7271 0000 00da 056c 6576 656c da0a 6963  rq.....level..ic
+00002070: 6f6e 5f63 6c61 7373 7242 0000 0072 4300  on_classrB...rC.
+00002080: 0000 7244 0000 0072 1c00 0000 7289 0000  ..rD...r....r...
+00002090: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+000020a0: 721b 0000 0072 7f00 0000 f500 0000 731e  r....r........s.
+000020b0: 0000 0008 0104 030e 010e 0110 0112 0112  ................
+000020c0: 0104 0102 0102 0104 0102 0102 fb06 080e  ................
+000020d0: 0672 7f00 0000 6300 0000 0000 0000 0000  .r....c.........
+000020e0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+000020f0: ce00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00002100: 6504 6a05 6402 6403 6404 6405 8d03 5a06  e.j.d.d.d.d...Z.
+00002110: 6504 6a07 6508 6406 6504 6a09 6407 6408  e.j.e.d.e.j.d.d.
+00002120: 8d04 5a0a 6504 6a07 6409 640a 6504 6a09  ..Z.e.j.d.d.e.j.
+00002130: 640b 6408 8d04 5a0b 6504 6a05 640c 640d  d.d...Z.e.j.d.d.
+00002140: 6404 6404 640e 8d04 5a0c 6504 6a0d 640f  d.d.d...Z.e.j.d.
+00002150: 6404 6404 6410 8d03 5a0e 6504 6a0d 6411  d.d.d...Z.e.j.d.
+00002160: 6404 6404 6410 8d03 5a0f 6504 6a05 6412  d.d.d...Z.e.j.d.
+00002170: 6413 6404 6414 8d03 5a10 6504 6a11 6415  d.d.d...Z.e.j.d.
+00002180: 6404 6416 8d02 5a12 6504 6a13 6417 6404  d.d...Z.e.j.d.d.
+00002190: 6404 6418 8d03 5a14 6504 6a15 6419 641a  d.d...Z.e.j.d.d.
+000021a0: 6404 641b 8d03 5a16 4700 641c 641d 8400  d.d...Z.G.d.d...
+000021b0: 641d 8302 5a17 641e 641f 8400 5a18 6420  d...Z.d.d...Z.d 
+000021c0: 5300 2921 da0d 436f 6e74 656e 7454 7970  S.)!..ContentTyp
+000021d0: 6545 7875 1600 0000 0a20 2020 20e5 8a9f  eExu.....    ...
+000021e0: e883 bde7 b1bb e588 ab0a 2020 2020 7223  ..........    r#
+000021f0: 0000 0072 5100 0000 5429 0272 2600 0000  ...rQ...T).r&...
+00002200: 720f 0000 0075 0c00 0000 e7b3 bbe7 bb9f  r....u..........
+00002210: e5ba 94e7 94a8 da09 6578 7465 6e73 696f  ........extensio
+00002220: 6e72 7900 0000 727f 0000 0075 0600 0000  nry...r....u....
+00002230: e88f 9ce5 8d95 5a0d 636f 6e74 656e 745f  ......Z.content_
+00002240: 6361 7465 7372 8000 0000 7281 0000 0072  catesr....r....r
+00002250: 2900 0000 da03 7572 6c72 2b00 0000 7506  ).....urlr+...u.
+00002260: 0000 00e7 bb84 e688 9075 0600 0000 e58f  .........u......
+00002270: 82e6 95b0 7277 0000 00a9 0372 0d00 0000  ....rw.....r....
+00002280: 7226 0000 0072 0f00 0000 7509 0000 00e9  r&...r....u.....
+00002290: 878d e5ae 9ae5 9091 a902 720d 0000 0072  ..........r....r
+000022a0: 0f00 0000 7213 0000 0029 0272 1500 0000  ....r....).r....
+000022b0: 720f 0000 0072 6400 0000 7265 0000 0072  r....rd...re...r
+000022c0: 7a00 0000 6300 0000 0000 0000 0000 0000  z...c...........
+000022d0: 0000 0000 0001 0000 0040 0000 0073 1c00  .........@...s..
+000022e0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000022f0: 5a04 6504 5a05 6403 5a06 6404 5300 2905  Z.e.Z.d.Z.d.S.).
+00002300: 7a12 436f 6e74 656e 7454 7970 6545 782e  z.ContentTypeEx.
+00002310: 4d65 7461 5a12 6273 5f63 6f6e 7465 6e74  MetaZ.bs_content
+00002320: 5f74 7970 655f 6578 7512 0000 00e5 8a9f  _type_exu.......
+00002330: e883 bde7 b1bb e588 abe8 a1a5 e585 8572  ...............r
+00002340: 8400 0000 4e72 8500 0000 721a 0000 0072  ....Nr....r....r
+00002350: 1a00 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00002360: 0000 0029 0100 0073 0800 0000 0801 0401  ...)...s........
+00002370: 0401 0401 721c 0000 0063 0100 0000 0000  ....r....c......
+00002380: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00002390: 0000 7306 0000 007c 006a 0053 0072 6b00  ..s....|.j.S.rk.
+000023a0: 0000 7287 0000 0072 8800 0000 721a 0000  ..r....r....r...
+000023b0: 0072 1a00 0000 721b 0000 0072 8900 0000  .r....r....r....
+000023c0: 2f01 0000 7302 0000 0000 017a 1543 6f6e  /...s......z.Con
+000023d0: 7465 6e74 5479 7065 4578 2e5f 5f73 7472  tentTypeEx.__str
+000023e0: 5f5f 4e29 1972 1600 0000 7217 0000 0072  __N).r....r....r
+000023f0: 1800 0000 727c 0000 0072 0500 0000 723a  ....r|...r....r:
+00002400: 0000 0072 3b00 0000 7242 0000 0072 0400  ...r;...rB...r..
+00002410: 0000 7243 0000 00da 0c63 6f6e 7465 6e74  ..rC.....content
+00002420: 5f74 7970 655a 1063 6f6e 7465 6e74 5f74  _typeZ.content_t
+00002430: 7970 655f 6361 7472 8b00 0000 723d 0000  ype_catr....r=..
+00002440: 00da 0966 726f 6e74 5f75 726c 5a0f 6672  ...front_urlZ.fr
+00002450: 6f6e 745f 636f 6d70 6f6e 656e 745a 0c66  ont_componentZ.f
+00002460: 726f 6e74 5f70 6172 616d 73da 0855 524c  ront_params..URL
+00002470: 4669 656c 645a 1266 726f 6e74 5f72 6564  FieldZ.front_red
+00002480: 6972 6563 745f 7572 6c72 2000 0000 7221  irect_urlr ...r!
+00002490: 0000 0072 7000 0000 7271 0000 0072 1c00  ...rp...rq...r..
+000024a0: 0000 7289 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000024b0: 0072 1a00 0000 721b 0000 0072 8c00 0000  .r....r....r....
+000024c0: 1001 0000 732e 0000 0008 0104 0310 0104  ....s...........
+000024d0: 0102 0102 0104 0102 fc06 0604 0102 0102  ................
+000024e0: 0104 0102 fc06 0612 0110 0110 0110 010e  ................
+000024f0: 0110 0110 020e 0672 8c00 0000 6300 0000  .......r....c...
+00002500: 0000 0000 0000 0000 0000 0000 0006 0000  ................
+00002510: 0040 0000 0073 9c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00002520: 5a02 6503 6a04 6401 6402 6403 6404 8d03  Z.e.j.d.d.d.d...
+00002530: 5a05 6503 6a04 6405 6402 6406 8d02 5a06  Z.e.j.d.d.d...Z.
+00002540: 6503 6a04 6407 6408 6406 8d02 5a07 6503  e.j.d.d.d...Z.e.
+00002550: 6a08 6409 6403 640a 8d02 5a09 6503 6a0a  j.d.d.d...Z.e.j.
+00002560: 650b 640b 6503 6a0c 6403 640c 8d04 5a0d  e.d.e.j.d.d...Z.
+00002570: 6503 6a04 640d 6402 6403 6403 640e 8d04  e.j.d.d.d.d.d...
+00002580: 5a0e 6503 6a04 640f 6402 6403 6403 640e  Z.e.j.d.d.d.d.d.
+00002590: 8d04 5a0f 6503 6a10 6511 6410 6403 6411  ..Z.e.j.e.d.d.d.
+000025a0: 8d03 5a12 4700 6412 6413 8400 6413 8302  ..Z.G.d.d...d...
+000025b0: 5a13 6414 5300 2915 da0f 4578 7065 6e73  Z.d.S.)...Expens
+000025c0: 6553 7461 6e64 6172 6475 0c00 0000 e8b4  eStandardu......
+000025d0: b9e7 94a8 e7b1 bbe5 9e8b 7228 0000 0054  ..........r(...T
+000025e0: 728f 0000 0075 0c00 0000 e6a0 87e5 8786  r....u..........
+000025f0: e590 8de7 a7b0 7225 0000 0075 0c00 0000  ......r%...u....
+00002600: e6a0 87e5 8786 e7bc 96e7 a081 7224 0000  ............r$..
+00002610: 0075 0600 0000 e8b4 b9e7 94a8 7290 0000  .u..........r...
+00002620: 0072 3000 0000 7231 0000 0072 3500 0000  .r0...r1...r5...
+00002630: 7229 0000 0072 3600 0000 7512 0000 00e5  r)...r6...u.....
+00002640: 8cbb e794 9fe8 b4b9 e794 a8e6 a087 e587  ................
+00002650: 8629 0272 0d00 0000 722a 0000 0063 0000  .).r....r*...c..
+00002660: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00002670: 0000 4000 0000 731c 0000 0065 005a 0164  ..@...s....e.Z.d
+00002680: 005a 0264 015a 0364 025a 0465 045a 0564  .Z.d.Z.d.Z.e.Z.d
+00002690: 035a 0664 0453 0029 057a 1445 7870 656e  .Z.d.S.).z.Expen
+000026a0: 7365 5374 616e 6461 7264 2e4d 6574 615a  seStandard.MetaZ
+000026b0: 1362 735f 6578 7065 6e73 655f 7374 616e  .bs_expense_stan
+000026c0: 6461 7264 750f 0000 00e8 b4b9 e794 a8e6  dardu...........
+000026d0: a087 e587 86e8 a1a8 2901 2902 da0d 7374  ........).)...st
+000026e0: 616e 6461 7264 5f63 6f64 6572 4b00 0000  andard_coderK...
+000026f0: 4e72 4c00 0000 721a 0000 0072 1a00 0000  NrL...r....r....
+00002700: 721a 0000 0072 1b00 0000 721c 0000 0043  r....r....r....C
+00002710: 0100 0073 0800 0000 0801 0401 0401 0401  ...s............
+00002720: 721c 0000 004e 2914 7216 0000 0072 1700  r....N).r....r..
+00002730: 0000 7218 0000 0072 0500 0000 723a 0000  ..r....r....r:..
+00002740: 005a 0c65 7870 656e 7365 5f74 7970 655a  .Z.expense_typeZ
+00002750: 0d73 7461 6e64 6172 645f 6e61 6d65 7295  .standard_namer.
+00002760: 0000 0072 4100 0000 5a04 6665 6573 7242  ...rA...Z.feesrB
+00002770: 0000 0072 2200 0000 7243 0000 0072 4b00  ...r"...rC...rK.
+00002780: 0000 7245 0000 0072 4600 0000 da0f 4d61  ..rE...rF.....Ma
+00002790: 6e79 546f 4d61 6e79 4669 656c 6472 5000  nyToManyFieldrP.
+000027a0: 0000 5a07 646f 6374 6f72 7372 1c00 0000  ..Z.doctorsr....
+000027b0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+000027c0: 1b00 0000 7294 0000 0033 0100 0073 1c00  ....r....3...s..
+000027d0: 0000 0802 1001 0e01 0e01 0e01 0401 0201  ................
+000027e0: 0201 0401 02fc 0606 1201 1201 1002 7294  ..............r.
+000027f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002800: 0000 0000 0700 0000 4000 0000 734c 0000  ........@...sL..
+00002810: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00002820: 0264 038d 025a 0565 036a 0464 0464 0264  .d...Z.e.j.d.d.d
+00002830: 038d 025a 0665 036a 0764 0564 0665 036a  ...Z.e.j.d.d.e.j
+00002840: 0864 0764 0864 098d 055a 0947 0064 0a64  .d.d.d...Z.G.d.d
+00002850: 0b84 0064 0b83 025a 0a64 0c53 0029 0dda  ...d...Z.d.S.)..
+00002860: 0e49 6e73 7065 6374 696f 6e54 7970 65f5  .InspectionType.
+00002870: 1200 0000 e6a3 80e6 9fa5 e7b1 bbe5 9e8b  ................
+00002880: e7bc 96e7 a081 7277 0000 0072 2500 0000  ......rw...r%...
+00002890: f512 0000 00e6 a380 e69f a5e7 b1bb e59e  ................
+000028a0: 8be5 908d e7a7 b072 2f00 0000 f506 0000  .......r/.......
+000028b0: 00e7 88b6 e7ba a772 8200 0000 5472 8300  .......r....Tr..
+000028c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000028d0: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+000028e0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+000028f0: 6504 5a05 6403 5300 2904 7a13 496e 7370  e.Z.d.S.).z.Insp
+00002900: 6563 7469 6f6e 5479 7065 2e4d 6574 615a  ectionType.MetaZ
+00002910: 1262 735f 696e 7370 6563 7469 6f6e 5f74  .bs_inspection_t
+00002920: 7970 6575 1200 0000 e6a3 80e6 9fa5 e5ad  ypeu............
+00002930: 97e5 85b8 e7b1 bbe5 9e8b 4e72 3700 0000  ..........Nr7...
+00002940: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002950: 1b00 0000 721c 0000 0057 0100 0073 0600  ....r....W...s..
+00002960: 0000 0801 0401 0401 721c 0000 004e a90b  ........r....N..
+00002970: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00002980: 0500 0000 723a 0000 00da 0a63 6f64 655f  ....r:.....code_
+00002990: 7372 7674 70da 0a6e 616d 655f 7372 7674  srvtp..name_srvt
+000029a0: 7072 4200 0000 7243 0000 0072 4400 0000  prB...rC...rD...
+000029b0: 721c 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+000029c0: 1a00 0000 721b 0000 0072 9700 0000 4c01  ....r....r....L.
+000029d0: 0000 7314 0000 0008 010e 010e 0104 0102  ..s.............
+000029e0: 0102 0104 0102 0102 fb06 0872 9700 0000  ...........r....
+000029f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002a00: 0006 0000 0040 0000 0073 a600 0000 6500  .....@...s....e.
+00002a10: 5a01 6400 5a02 6503 6a04 6401 6402 6403  Z.d.Z.e.j.d.d.d.
+00002a20: 6404 8d03 5a05 6503 6a04 6405 6406 6407  d...Z.e.j.d.d.d.
+00002a30: 8d02 5a06 6503 6a04 6408 6409 6407 8d02  ..Z.e.j.d.d.d...
+00002a40: 5a07 6503 6a04 6408 640a 6407 8d02 5a08  Z.e.j.d.d.d...Z.
+00002a50: 6503 6a09 640b 6403 640c 8d02 5a0a 6503  e.j.d.d.d...Z.e.
+00002a60: 6a04 6408 640d 6403 6403 640e 8d04 5a0b  j.d.d.d.d.d...Z.
+00002a70: 6503 6a04 6408 640f 6403 6403 640e 8d04  e.j.d.d.d.d.d...
+00002a80: 5a0c 6503 6a04 6410 6411 6403 6412 8d03  Z.e.j.d.d.d.d...
+00002a90: 5a0d 6503 6a04 6413 6411 6403 6412 8d03  Z.e.j.d.d.d.d...
+00002aa0: 5a0e 4700 6414 6415 8400 6415 8302 5a0f  Z.G.d.d...d...Z.
+00002ab0: 6416 5300 2917 da16 496e 7370 6563 7469  d.S.)...Inspecti
+00002ac0: 6f6e 4469 6374 696f 6e61 7269 6573 7224  onDictionariesr$
+00002ad0: 0000 00f5 0c00 0000 e9a1 b9e7 9bae e7bc  ................
+00002ae0: 96e7 a081 5472 2d00 0000 7252 0000 00f5  ....Tr-...rR....
+00002af0: 0c00 0000 e9a1 b9e7 9bae e590 8de7 a7b0  ................
+00002b00: 7278 0000 00e9 8000 0000 f50c 0000 00e5  rx..............
+00002b10: 8cbb e999 a2e7 bc96 e7a0 8172 4800 0000  ...........rH...
+00002b20: f50c 0000 00e9 a1b9 e79b aee8 b4b9 e794  ................
+00002b30: a872 9000 0000 f506 0000 00e5 a487 e6b3  .r..............
+00002b40: a872 7b00 0000 f50c 0000 00e5 8cba e588  .r{.............
+00002b50: 86e5 ad97 e6ae b572 9800 0000 7277 0000  .......r....rw..
+00002b60: 0072 8f00 0000 7299 0000 0063 0000 0000  .r....r....c....
+00002b70: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00002b80: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00002b90: 0264 015a 0364 025a 0465 045a 0564 0353  .d.Z.d.Z.e.Z.d.S
+00002ba0: 0029 047a 1b49 6e73 7065 6374 696f 6e44  .).z.InspectionD
+00002bb0: 6963 7469 6f6e 6172 6965 732e 4d65 7461  ictionaries.Meta
+00002bc0: 5a1a 6273 5f69 6e73 7065 6374 696f 6e5f  Z.bs_inspection_
+00002bd0: 6469 6374 696f 6e61 7269 6573 750c 0000  dictionariesu...
+00002be0: 00e6 a380 e69f a5e5 ad97 e585 b84e 7237  .............Nr7
+00002bf0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00002c00: 0000 721b 0000 0072 1c00 0000 6801 0000  ..r....r....h...
+00002c10: 7306 0000 0008 0104 0104 0172 1c00 0000  s..........r....
+00002c20: 4ea9 1072 1600 0000 7217 0000 0072 1800  N..r....r....r..
+00002c30: 0000 7205 0000 0072 3a00 0000 5a0c 7072  ..r....r:...Z.pr
+00002c40: 6f6a 6563 745f 636f 6465 5a0c 7072 6f6a  oject_codeZ.proj
+00002c50: 6563 745f 6e61 6d65 da0d 686f 7370 6974  ect_name..hospit
+00002c60: 616c 5f63 6f64 655a 0b6f 6666 6963 655f  al_codeZ.office_
+00002c70: 636f 6465 7241 0000 005a 0c70 726f 6a65  coderA...Z.proje
+00002c80: 6374 5f66 6565 735a 0772 656d 6172 6b73  ct_feesZ.remarks
+00002c90: 5a0b 6469 7374 696e 6775 6973 6872 9c00  Z.distinguishr..
+00002ca0: 0000 729d 0000 0072 1c00 0000 721a 0000  ..r....r....r...
+00002cb0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00002cc0: 729e 0000 005d 0100 0073 1400 0000 0801  r....]...s......
+00002cd0: 1001 0e01 0e01 0e01 0e01 1201 1201 1001  ................
+00002ce0: 1002 729e 0000 0063 0000 0000 0000 0000  ..r....c........
+00002cf0: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
+00002d00: 734c 0000 0065 005a 0164 005a 0265 036a  sL...e.Z.d.Z.e.j
+00002d10: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
+00002d20: 0464 0264 038d 025a 0665 036a 0764 0564  .d.d...Z.e.j.d.d
+00002d30: 0665 036a 0864 0764 0864 098d 055a 0947  .e.j.d.d.d...Z.G
+00002d40: 0064 0a64 0b84 0064 0b83 025a 0a64 0c53  .d.d...d...Z.d.S
+00002d50: 0029 0dda 0f45 7861 6d69 6e61 7469 6f6e  .)...Examination
+00002d60: 5479 7065 7298 0000 0072 7700 0000 7225  Typer....rw...r%
+00002d70: 0000 0072 9900 0000 722f 0000 0072 9a00  ...r....r/...r..
+00002d80: 0000 7282 0000 0054 7283 0000 0063 0000  ..r....Tr....c..
+00002d90: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00002da0: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00002db0: 005a 0264 015a 0364 025a 0465 045a 0564  .Z.d.Z.d.Z.e.Z.d
+00002dc0: 0353 0029 047a 1445 7861 6d69 6e61 7469  .S.).z.Examinati
+00002dd0: 6f6e 5479 7065 2e4d 6574 615a 1362 735f  onType.MetaZ.bs_
+00002de0: 6578 616d 696e 6174 696f 6e5f 7479 7065  examination_type
+00002df0: 7512 0000 00e6 a380 e9aa 8ce5 ad97 e585  u...............
+00002e00: b8e7 b1bb e59e 8b4e 7237 0000 0072 1a00  .......Nr7...r..
+00002e10: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00002e20: 0072 1c00 0000 7901 0000 7306 0000 0008  .r....y...s.....
+00002e30: 0104 0104 0172 1c00 0000 4e72 9b00 0000  .....r....Nr....
+00002e40: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002e50: 1b00 0000 72a8 0000 006e 0100 0073 1400  ....r....n...s..
+00002e60: 0000 0801 0e01 0e01 0401 0201 0201 0401  ................
+00002e70: 0201 02fb 0608 72a8 0000 0063 0000 0000  ......r....c....
+00002e80: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00002e90: 4000 0000 73a6 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00002ea0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+00002eb0: 0565 036a 0464 0564 0664 078d 025a 0665  .e.j.d.d.d...Z.e
+00002ec0: 036a 0464 0864 0964 078d 025a 0765 036a  .j.d.d.d...Z.e.j
+00002ed0: 0464 0864 0a64 078d 025a 0865 036a 0964  .d.d.d...Z.e.j.d
+00002ee0: 0b64 0364 0c8d 025a 0a65 036a 0464 0864  .d.d...Z.e.j.d.d
+00002ef0: 0d64 0364 0364 0e8d 045a 0b65 036a 0464  .d.d.d...Z.e.j.d
+00002f00: 0864 0f64 0364 0364 0e8d 045a 0c65 036a  .d.d.d.d...Z.e.j
+00002f10: 0464 1064 1164 0364 128d 035a 0d65 036a  .d.d.d.d...Z.e.j
+00002f20: 0464 1364 1164 0364 128d 035a 0e47 0064  .d.d.d.d...Z.G.d
+00002f30: 1464 1584 0064 1583 025a 0f64 1653 0029  .d...d...Z.d.S.)
+00002f40: 17da 1745 7861 6d69 6e61 7469 6f6e 4469  ...ExaminationDi
+00002f50: 6374 696f 6e61 7269 6573 7224 0000 0072  ctionariesr$...r
+00002f60: 9f00 0000 5472 2d00 0000 7252 0000 0072  ....Tr-...rR...r
+00002f70: a000 0000 7278 0000 0072 a100 0000 72a2  ....rx...r....r.
+00002f80: 0000 0072 4800 0000 72a3 0000 0072 9000  ...rH...r....r..
+00002f90: 0000 72a4 0000 0072 7b00 0000 72a5 0000  ..r....r{...r...
+00002fa0: 0075 1200 0000 e6a3 80e9 aa8c e7b1 bbe5  .u..............
+00002fb0: 9e8b e7bc 96e7 a081 7277 0000 0072 8f00  ........rw...r..
+00002fc0: 0000 7512 0000 00e6 a380 e9aa 8ce7 b1bb  ..u.............
+00002fd0: e59e 8be5 908d e7a7 b063 0000 0000 0000  .........c......
+00002fe0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00002ff0: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00003000: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
+00003010: 047a 1c45 7861 6d69 6e61 7469 6f6e 4469  .z.ExaminationDi
+00003020: 6374 696f 6e61 7269 6573 2e4d 6574 615a  ctionaries.MetaZ
+00003030: 1b62 735f 6578 616d 696e 6174 696f 6e5f  .bs_examination_
+00003040: 6469 6374 696f 6e61 7269 6573 750c 0000  dictionariesu...
+00003050: 00e6 a380 e9aa 8ce5 ad97 e585 b84e 7237  .............Nr7
+00003060: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00003070: 0000 721b 0000 0072 1c00 0000 8a01 0000  ..r....r........
+00003080: 7306 0000 0008 0104 0104 0172 1c00 0000  s..........r....
+00003090: 4e72 a600 0000 721a 0000 0072 1a00 0000  Nr....r....r....
+000030a0: 721a 0000 0072 1b00 0000 72a9 0000 007f  r....r....r.....
+000030b0: 0100 0073 1400 0000 0801 1001 0e01 0e01  ...s............
+000030c0: 0e01 0e01 1201 1201 1001 1002 72a9 0000  ............r...
+000030d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000030e0: 0000 0600 0000 4000 0000 733c 0000 0065  ......@...s<...e
+000030f0: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+00003100: 0364 048d 035a 0565 036a 0464 0564 0664  .d...Z.e.j.d.d.d
+00003110: 0364 0364 078d 045a 0647 0064 0864 0984  .d.d...Z.G.d.d..
+00003120: 0064 0983 025a 0764 0a53 0029 0bda 1344  .d...Z.d.S.)...D
+00003130: 7275 6750 7265 7061 7261 7469 6f6e 5479  rugPreparationTy
+00003140: 7065 7224 0000 0072 2c00 0000 5472 2d00  per$...r,...Tr-.
+00003150: 0000 7252 0000 0075 0c00 0000 e7b1 bbe5  ..rR...u........
+00003160: 9e8b e590 8de7 a7b0 727b 0000 0063 0000  ........r{...c..
+00003170: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00003180: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00003190: 005a 0264 015a 0364 025a 0465 045a 0564  .Z.d.Z.d.Z.e.Z.d
+000031a0: 0353 0029 047a 1844 7275 6750 7265 7061  .S.).z.DrugPrepa
+000031b0: 7261 7469 6f6e 5479 7065 2e4d 6574 615a  rationType.MetaZ
+000031c0: 1862 735f 6472 7567 5f70 7265 7061 7261  .bs_drug_prepara
+000031d0: 7469 6f6e 5f74 7970 6575 1200 0000 e88d  tion_typeu......
+000031e0: afe5 9381 e588 b6e5 8982 e7b1 bbe5 9e8b  ................
+000031f0: 4e72 3700 0000 721a 0000 0072 1a00 0000  Nr7...r....r....
+00003200: 721a 0000 0072 1b00 0000 721c 0000 0094  r....r....r.....
+00003210: 0100 0073 0600 0000 0801 0401 0401 721c  ...s..........r.
+00003220: 0000 004e 2908 7216 0000 0072 1700 0000  ...N).r....r....
+00003230: 7218 0000 0072 0500 0000 723a 0000 0072  r....r....r:...r
+00003240: 3f00 0000 da09 7479 7065 5f6e 616d 6572  ?.....type_namer
+00003250: 1c00 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
+00003260: 0000 0072 1b00 0000 72aa 0000 0090 0100  ...r....r.......
+00003270: 0073 0600 0000 0801 1001 1202 72aa 0000  .s..........r...
+00003280: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003290: 0000 0600 0000 4000 0000 733c 0000 0065  ......@...s<...e
+000032a0: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+000032b0: 0364 048d 035a 0565 036a 0464 0564 0664  .d...Z.e.j.d.d.d
+000032c0: 0364 0364 078d 045a 0647 0064 0864 0984  .d.d...Z.G.d.d..
+000032d0: 0064 0983 025a 0764 0a53 0029 0bda 0844  .d...Z.d.S.)...D
+000032e0: 7275 6754 7970 6572 2c00 0000 7224 0000  rugTyper,...r$..
+000032f0: 0054 a903 720d 0000 0072 2600 0000 722e  .T..r....r&...r.
+00003300: 0000 0072 2300 0000 7252 0000 0072 2900  ...r#...rR...r).
+00003310: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003320: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+00003330: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00003340: 6504 5a05 6403 5300 2904 7a0d 4472 7567  e.Z.d.S.).z.Drug
+00003350: 5479 7065 2e4d 6574 615a 0c62 735f 6472  Type.MetaZ.bs_dr
+00003360: 7567 5f74 7970 65f5 0c00 0000 e88d afe5  ug_type.........
+00003370: 9381 e7b1 bbe5 9e8b 4e72 3700 0000 721a  ........Nr7...r.
+00003380: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00003390: 0000 721c 0000 009e 0100 0073 0600 0000  ..r........s....
+000033a0: 0801 0401 0401 721c 0000 004e a908 7216  ......r....N..r.
+000033b0: 0000 0072 1700 0000 7218 0000 0072 0500  ...r....r....r..
+000033c0: 0000 723a 0000 00da 0463 6f64 6572 3b00  ..r:.....coder;.
+000033d0: 0000 721c 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000033e0: 0072 1a00 0000 721b 0000 0072 ac00 0000  .r....r....r....
+000033f0: 9a01 0000 7306 0000 0008 0110 0112 0272  ....s..........r
+00003400: ac00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003410: 0000 0000 0006 0000 0040 0000 0073 3c00  .........@...s<.
+00003420: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
+00003430: 6402 6403 6404 8d03 5a05 6503 6a04 6405  d.d.d...Z.e.j.d.
+00003440: 6406 6403 6403 6407 8d04 5a06 4700 6408  d.d.d.d...Z.G.d.
+00003450: 6409 8400 6409 8302 5a07 640a 5300 290b  d...d...Z.d.S.).
+00003460: da0c 4472 7567 4361 7465 676f 7279 7224  ..DrugCategoryr$
+00003470: 0000 0072 2c00 0000 5472 2d00 0000 7252  ...r,...Tr-...rR
+00003480: 0000 0075 0c00 0000 e7b1 bbe5 88ab e590  ...u............
+00003490: 8de7 a7b0 727b 0000 0063 0000 0000 0000  ....r{...c......
+000034a0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+000034b0: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000034c0: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
+000034d0: 047a 1144 7275 6743 6174 6567 6f72 792e  .z.DrugCategory.
+000034e0: 4d65 7461 5a10 6273 5f64 7275 675f 6361  MetaZ.bs_drug_ca
+000034f0: 7465 676f 7279 750c 0000 00e8 8daf e593  tegoryu.........
+00003500: 81e7 b1bb e588 ab4e 7237 0000 0072 1a00  .......Nr7...r..
+00003510: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00003520: 0072 1c00 0000 a801 0000 7306 0000 0008  .r........s.....
+00003530: 0104 0104 0172 1c00 0000 4e29 0872 1600  .....r....N).r..
+00003540: 0000 7217 0000 0072 1800 0000 7205 0000  ..r....r....r...
+00003550: 0072 3a00 0000 723f 0000 005a 0d63 6174  .r:...r?...Z.cat
+00003560: 6567 6f72 795f 6e61 6d65 721c 0000 0072  egory_namer....r
+00003570: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+00003580: 0000 0072 b100 0000 a401 0000 7306 0000  ...r........s...
+00003590: 0008 0110 0112 0272 b100 0000 6300 0000  .......r....c...
+000035a0: 0000 0000 0000 0000 0000 0000 0006 0000  ................
+000035b0: 0040 0000 0073 8e01 0000 6500 5a01 6400  .@...s....e.Z.d.
+000035c0: 5a02 6503 6a04 6401 6402 6403 6404 8d03  Z.e.j.d.d.d.d...
+000035d0: 5a05 6503 6a04 6405 6406 6403 6403 6407  Z.e.j.d.d.d.d.d.
+000035e0: 8d04 5a06 6503 6a04 6405 6408 6403 6403  ..Z.e.j.d.d.d.d.
+000035f0: 6407 8d04 5a07 6503 6a04 6405 6409 6403  d...Z.e.j.d.d.d.
+00003600: 6403 6407 8d04 5a08 6503 6a04 640a 640b  d.d...Z.e.j.d.d.
+00003610: 6403 6403 640c 8d04 5a09 6503 6a0a 650b  d.d.d...Z.e.j.e.
+00003620: 640d 6503 6a0c 640e 8d03 5a0d 6503 6a0a  d.e.j.d...Z.e.j.
+00003630: 650e 640f 6503 6a0c 640e 8d03 5a0f 6503  e.d.e.j.d...Z.e.
+00003640: 6a0a 6510 6410 6503 6a0c 640e 8d03 5a11  j.e.d.e.j.d...Z.
+00003650: 6503 6a04 6411 640b 6403 6403 640c 8d04  e.j.d.d.d.d.d...
+00003660: 5a12 6503 6a04 6412 640b 6403 6403 640c  Z.e.j.d.d.d.d.d.
+00003670: 8d04 5a13 6503 6a04 6413 640b 6403 6403  ..Z.e.j.d.d.d.d.
+00003680: 640c 8d04 5a14 6503 6a04 6414 640b 6403  d...Z.e.j.d.d.d.
+00003690: 6403 640c 8d04 5a15 6503 6a04 6415 640b  d.d...Z.e.j.d.d.
+000036a0: 6403 6403 640c 8d04 5a16 6503 6a04 6416  d.d.d...Z.e.j.d.
+000036b0: 640b 6403 6403 640c 8d04 5a17 6503 6a04  d.d.d.d...Z.e.j.
+000036c0: 6417 640b 6403 6403 640c 8d04 5a18 6503  d.d.d.d.d...Z.e.
+000036d0: 6a19 6418 6403 6419 8d02 5a1a 6503 6a04  j.d.d.d...Z.e.j.
+000036e0: 641a 6405 6403 6403 640c 8d04 5a1b 6503  d.d.d.d.d...Z.e.
+000036f0: 6a04 641b 6405 6403 6403 640c 8d04 5a1c  j.d.d.d.d.d...Z.
+00003700: 6503 6a04 641c 6405 6403 6403 640c 8d04  e.j.d.d.d.d.d...
+00003710: 5a1d 6503 6a04 6405 641d 6403 6403 6407  Z.e.j.d.d.d.d.d.
+00003720: 8d04 5a1e 6503 6a04 6405 641e 6403 6403  ..Z.e.j.d.d.d.d.
+00003730: 6407 8d04 5a1f 4700 641f 6420 8400 6420  d...Z.G.d.d ..d 
+00003740: 8302 5a20 6421 5300 2922 da0d 4472 7567  ..Z d!S.)"..Drug
+00003750: 4469 7265 6374 6f72 79f5 0c00 0000 e88d  Directory.......
+00003760: afe5 9381 e7bc 96e7 a081 7224 0000 0054  ..........r$...T
+00003770: 72ad 0000 0072 5200 0000 f50c 0000 00e8  r....rR.........
+00003780: 8daf e593 81e5 908d e7a7 b072 7b00 0000  ...........r{...
+00003790: f506 0000 00e8 a784 e6a0 bc75 0c00 0000  ...........u....
+000037a0: e59f bae6 9cac e58d 95e4 bd8d 7512 0000  ............u...
+000037b0: 00e6 80bb e987 8fe5 8d95 e4bd 8de7 bc96  ................
+000037c0: e7a0 8172 5100 0000 7229 0000 00f5 0c00  ...rQ...r)......
+000037d0: 0000 e588 b6e5 8982 e7b1 bbe5 9e8b 7249  ..............rI
+000037e0: 0000 00f5 0600 0000 e7b1 bbe5 88ab 72ae  ..............r.
+000037f0: 0000 0075 0c00 0000 e58d 95e4 bd8d e589  ...u............
+00003800: 82e9 878f 7513 0000 00e8 aea1 e987 8f2f  ....u........../
+00003810: e99b b6e5 94ae e58d 95e4 bd8d 7512 0000  ............u...
+00003820: 00e8 aea1 e987 8fe5 8d95 e4bd 8de7 bc96  ................
+00003830: e7a0 81f5 0c00 0000 e5ba 93e5 ad98 e695  ................
+00003840: b0e9 878f 750c 0000 00e5 ba93 e5ad 98e5  ....u...........
+00003850: 8d95 e4bd 8d75 0c00 0000 e58c bbe4 bf9d  .....u..........
+00003860: e7b1 bbe5 88ab 750c 0000 00e5 869c e590  ......u.........
+00003870: 88e7 b1bb e588 ab75 0f00 0000 e698 afe5  .......u........
+00003880: 90a6 e698 afe5 9fba e88d af72 1400 0000  ...........r....
+00003890: 750c 0000 00e9 ab98 e58d b1e7 ad89 e7ba  u...............
+000038a0: a775 1200 0000 e59b bde5 aeb6 e8b4 afe6  .u..............
+000038b0: a087 e7bc 96e7 a081 7512 0000 00e5 9bbd  ........u.......
+000038c0: e5ae b6e8 b4af e6a0 87e5 908d e7a7 b0f5  ................
+000038d0: 0600 0000 e4ba a7e5 9cb0 f50c 0000 00e7  ................
+000038e0: 949f e4ba a7e5 8e82 e5ae b663 0000 0000  ...........c....
+000038f0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00003900: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00003910: 0264 015a 0364 025a 0465 045a 0564 0353  .d.Z.d.Z.e.Z.d.S
+00003920: 0029 047a 1244 7275 6744 6972 6563 746f  .).z.DrugDirecto
+00003930: 7279 2e4d 6574 615a 1162 735f 6472 7567  ry.MetaZ.bs_drug
+00003940: 5f64 6972 6563 746f 7279 750c 0000 00e8  _directoryu.....
+00003950: 8daf e593 81e7 9bae e5bd 954e 7237 0000  ...........Nr7..
+00003960: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00003970: 721b 0000 0072 1c00 0000 d101 0000 7306  r....r........s.
+00003980: 0000 0008 0104 0104 0172 1c00 0000 4e29  .........r....N)
+00003990: 2172 1600 0000 7217 0000 0072 1800 0000  !r....r....r....
+000039a0: 7205 0000 0072 3a00 0000 da09 6472 7567  r....r:.....drug
+000039b0: 5f63 6f64 65da 0964 7275 675f 6e61 6d65  _code..drug_name
+000039c0: da09 7374 616e 6461 7264 735a 0a74 6f74  ..standardsZ.tot
+000039d0: 616c 5f75 6e69 745a 0f74 6f74 616c 5f75  al_unitZ.total_u
+000039e0: 6e69 745f 636f 6465 7242 0000 0072 aa00  nit_coderB...r..
+000039f0: 0000 da0a 444f 5f4e 4f54 4849 4e47 da10  ....DO_NOTHING..
+00003a00: 7072 6570 6172 6174 696f 6e5f 7479 7065  preparation_type
+00003a10: 72b1 0000 00da 0863 6174 6567 6f72 7972  r......categoryr
+00003a20: ac00 0000 da09 6472 7567 5f74 7970 655a  ......drug_typeZ
+00003a30: 0975 6e69 745f 646f 7365 5a0c 6d65 6173  .unit_doseZ.meas
+00003a40: 7572 655f 756e 6974 5a11 6d65 6173 7572  ure_unitZ.measur
+00003a50: 655f 756e 6974 5f63 6f64 655a 0a73 746f  e_unit_codeZ.sto
+00003a60: 636b 5f6c 6566 745a 0a73 746f 636b 5f75  ck_leftZ.stock_u
+00003a70: 6e69 745a 036d 6963 5a0c 7263 635f 6361  nitZ.micZ.rcc_ca
+00003a80: 7465 676f 7279 7220 0000 005a 0c69 735f  tegoryr ...Z.is_
+00003a90: 6573 7365 6e74 6961 6c5a 0868 725f 6c65  essentialZ.hr_le
+00003aa0: 7665 6c5a 0767 625f 636f 6465 5a07 6762  velZ.gb_codeZ.gb
+00003ab0: 5f6e 616d 65da 0c6f 7269 6769 6e5f 706c  _name..origin_pl
+00003ac0: 6163 65da 0c6d 616e 7566 6163 7475 7265  ace..manufacture
+00003ad0: 7272 1c00 0000 721a 0000 0072 1a00 0000  rr....r....r....
+00003ae0: 721a 0000 0072 1b00 0000 72b2 0000 00ae  r....r....r.....
+00003af0: 0100 0073 4400 0000 0801 1001 1201 1201  ...sD...........
+00003b00: 1201 1201 0401 0201 0201 04fd 0605 0401  ................
+00003b10: 0201 0201 04fd 0605 0401 0201 0201 04fd  ................
+00003b20: 0605 1201 1201 1201 1201 1201 1201 1201  ................
+00003b30: 0e01 1201 1201 1201 1201 1202 72b2 0000  ............r...
+00003b40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003b50: 0000 0600 0000 4000 0000 733c 0000 0065  ......@...s<...e
+00003b60: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+00003b70: 0364 048d 035a 0565 036a 0464 0564 0664  .d...Z.e.j.d.d.d
+00003b80: 0364 0364 078d 045a 0647 0064 0864 0984  .d.d...Z.G.d.d..
+00003b90: 0064 0983 025a 0764 0a53 0029 0bda 0c50  .d...Z.d.S.)...P
+00003ba0: 6861 726d 6163 7954 7970 6572 2c00 0000  harmacyTyper,...
+00003bb0: 7224 0000 0054 72ad 0000 0072 2300 0000  r$...Tr....r#...
+00003bc0: 7252 0000 0072 2900 0000 6300 0000 0000  rR...r)...c.....
+00003bd0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00003be0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00003bf0: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
+00003c00: 2904 7a11 5068 6172 6d61 6379 5479 7065  ).z.PharmacyType
+00003c10: 2e4d 6574 615a 1062 735f 7068 6172 6d61  .MetaZ.bs_pharma
+00003c20: 6379 5f74 7970 65f5 0c00 0000 e88d afe6  cy_type.........
+00003c30: 88bf e7b1 bbe5 9e8b 4e72 3700 0000 721a  ........Nr7...r.
+00003c40: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00003c50: 0000 721c 0000 00db 0100 0073 0600 0000  ..r........s....
+00003c60: 0801 0401 0401 721c 0000 004e 72af 0000  ......r....Nr...
+00003c70: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00003c80: 721b 0000 0072 c400 0000 d701 0000 7306  r....r........s.
+00003c90: 0000 0008 0110 0112 0272 c400 0000 6300  .........r....c.
+00003ca0: 0000 0000 0000 0000 0000 0000 0000 0006  ................
+00003cb0: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
+00003cc0: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
+00003cd0: 8d03 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
+00003ce0: 6407 8d04 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
+00003cf0: 8302 5a07 640a 5300 290b da12 5068 6172  ..Z.d.S.)...Phar
+00003d00: 6d61 6379 456e 7465 7270 7269 7365 722c  macyEnterpriser,
+00003d10: 0000 0072 2400 0000 5472 ad00 0000 7223  ...r$...Tr....r#
+00003d20: 0000 0072 5200 0000 7229 0000 0063 0000  ...rR...r)...c..
+00003d30: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00003d40: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00003d50: 005a 0264 015a 0364 025a 0465 045a 0564  .Z.d.Z.d.Z.e.Z.d
+00003d60: 0353 0029 047a 1750 6861 726d 6163 7945  .S.).z.PharmacyE
+00003d70: 6e74 6572 7072 6973 652e 4d65 7461 5a16  nterprise.MetaZ.
+00003d80: 6273 5f70 6861 726d 6163 795f 656e 7465  bs_pharmacy_ente
+00003d90: 7270 7269 7365 750c 0000 00e8 8daf e4bc  rpriseu.........
+00003da0: 81e7 aea1 e790 864e 7237 0000 0072 1a00  .......Nr7...r..
+00003db0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00003dc0: 0072 1c00 0000 e501 0000 7306 0000 0008  .r........s.....
+00003dd0: 0104 0104 0172 1c00 0000 4e72 af00 0000  .....r....Nr....
+00003de0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00003df0: 1b00 0000 72c6 0000 00e1 0100 0073 0600  ....r........s..
+00003e00: 0000 0801 1001 1202 72c6 0000 0063 0000  ........r....c..
+00003e10: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00003e20: 0000 4000 0000 7386 0000 0065 005a 0164  ..@...s....e.Z.d
+00003e30: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
+00003e40: 035a 0565 036a 0464 0564 0664 0364 0364  .Z.e.j.d.d.d.d.d
+00003e50: 078d 045a 0665 036a 0765 0864 0865 036a  ...Z.e.j.e.d.e.j
+00003e60: 0964 098d 035a 0a65 036a 0b64 0a64 0364  .d...Z.e.j.d.d.d
+00003e70: 0364 0b8d 035a 0c65 036a 0765 0d64 0c65  .d...Z.e.j.e.d.e
+00003e80: 036a 0e64 0364 0d8d 045a 0f65 036a 0765  .j.d.d...Z.e.j.e
+00003e90: 1064 0e65 036a 0e64 0364 0d8d 045a 1147  .d.e.j.d.d...Z.G
+00003ea0: 0064 0f64 1084 0064 1083 025a 1264 1153  .d.d...d...Z.d.S
+00003eb0: 0029 12da 1250 6861 726d 6163 794d 616e  .)...PharmacyMan
+00003ec0: 6167 656d 656e 7475 0c00 0000 e88d afe6  agementu........
+00003ed0: 88bf e7bc 96e7 a081 7224 0000 0054 72ad  ........r$...Tr.
+00003ee0: 0000 0075 0c00 0000 e88d afe6 88bf e590  ...u............
+00003ef0: 8de7 a7b0 7252 0000 0072 2900 0000 72c5  ....rR...r)...r.
+00003f00: 0000 0072 4900 0000 750c 0000 00e8 8daf  ...rI...u.......
+00003f10: e688 bfe5 9cb0 e59d 8072 2b00 0000 7230  .........r+...r0
+00003f20: 0000 0072 3100 0000 750c 0000 00e6 8980  ...r1...u.......
+00003f30: e5b1 9ee8 8daf e4bc 8163 0000 0000 0000  .........c......
+00003f40: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00003f50: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00003f60: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
+00003f70: 047a 1750 6861 726d 6163 794d 616e 6167  .z.PharmacyManag
+00003f80: 656d 656e 742e 4d65 7461 5a16 6273 5f70  ement.MetaZ.bs_p
+00003f90: 6861 726d 6163 795f 6d61 6e61 6765 6d65  harmacy_manageme
+00003fa0: 6e74 750c 0000 00e8 8daf e688 bfe7 aea1  ntu.............
+00003fb0: e790 864e 7237 0000 0072 1a00 0000 721a  ...Nr7...r....r.
+00003fc0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00003fd0: 0000 f701 0000 7306 0000 0008 0104 0104  ......s.........
+00003fe0: 0172 1c00 0000 4e29 1372 1600 0000 7217  .r....N).r....r.
+00003ff0: 0000 0072 1800 0000 7205 0000 0072 3a00  ...r....r....r:.
+00004000: 0000 5a0d 7068 6172 6d61 6379 5f63 6f64  ..Z.pharmacy_cod
+00004010: 655a 0d70 6861 726d 6163 795f 6e61 6d65  eZ.pharmacy_name
+00004020: 7242 0000 0072 c400 0000 72be 0000 005a  rB...r....r....Z
+00004030: 0d70 6861 726d 6163 795f 7479 7065 723d  .pharmacy_typer=
+00004040: 0000 0072 4000 0000 7222 0000 0072 4300  ...r@...r"...rC.
+00004050: 0000 724b 0000 0072 c600 0000 5a0a 656e  ..rK...r....Z.en
+00004060: 7465 7270 7269 7365 721c 0000 0072 1a00  terpriser....r..
+00004070: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00004080: 0072 c700 0000 eb01 0000 7316 0000 0008  .r........s.....
+00004090: 0110 0112 0104 0102 0102 0104 fd06 0510  ................
+000040a0: 0114 0114 0272 c700 0000 6300 0000 0000  .....r....c.....
+000040b0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+000040c0: 0000 0073 4e01 0000 6500 5a01 6400 5a02  ...sN...e.Z.d.Z.
+000040d0: 6503 6a04 6505 6401 6503 6a06 6402 6403  e.j.e.d.e.j.d.d.
+000040e0: 8d04 5a07 6503 6a08 6404 6405 6402 6402  ..Z.e.j.d.d.d.d.
+000040f0: 6406 8d04 5a09 6503 6a08 6407 6408 6402  d...Z.e.j.d.d.d.
+00004100: 6402 6409 8d04 5a0a 6503 6a08 6407 640a  d.d...Z.e.j.d.d.
+00004110: 6402 6402 6409 8d04 5a0b 6503 6a08 6407  d.d.d...Z.e.j.d.
+00004120: 640b 6402 6402 6409 8d04 5a0c 6503 6a04  d.d.d.d...Z.e.j.
+00004130: 650d 640c 6503 6a0e 640d 8d03 5a0f 6503  e.d.e.j.d...Z.e.
+00004140: 6a04 6510 640e 6503 6a0e 640d 8d03 5a11  j.e.d.e.j.d...Z.
+00004150: 6503 6a04 6512 640f 6503 6a0e 640d 8d03  e.j.e.d.e.j.d...
+00004160: 5a13 6503 6a08 6410 6411 6402 6402 6409  Z.e.j.d.d.d.d.d.
+00004170: 8d04 5a14 6503 6a08 6412 6413 6402 6402  ..Z.e.j.d.d.d.d.
+00004180: 6409 8d04 5a15 6503 6a04 6516 6414 6503  d...Z.e.j.e.d.e.
+00004190: 6a06 6402 6403 8d04 5a17 6503 6a18 6415  j.d.d...Z.e.j.d.
+000041a0: 6402 6402 6416 8d03 5a19 6503 6a1a 6417  d.d.d...Z.e.j.d.
+000041b0: 6418 6402 6419 8d03 5a1b 6503 6a08 6407  d.d.d...Z.e.j.d.
+000041c0: 641a 6402 6402 6409 8d04 5a1c 6503 6a1d  d.d.d.d...Z.e.j.
+000041d0: 641b 6402 641c 8d02 5a1e 6503 6a1d 641d  d.d.d...Z.e.j.d.
+000041e0: 6402 641c 8d02 5a1f 6503 6a1d 641e 6402  d.d...Z.e.j.d.d.
+000041f0: 641c 8d02 5a20 6503 6a1d 641f 6402 641c  d...Z e.j.d.d.d.
+00004200: 8d02 5a21 4700 6420 6421 8400 6421 8302  ..Z!G.d d!..d!..
+00004210: 5a22 6422 5300 2923 da0c 5068 6172 6d61  Z"d"S.)#..Pharma
+00004220: 6379 4472 7567 750c 0000 00e6 8980 e5b1  cyDrugu.........
+00004230: 9ee8 8daf e688 bf54 7231 0000 0072 b300  .......Tr1...r..
+00004240: 0000 7224 0000 0072 2900 0000 7252 0000  ..r$...r)...rR..
+00004250: 0072 b400 0000 727b 0000 0072 b500 0000  .r....r{...r....
+00004260: 7506 0000 00e5 8d95 e4bd 8d72 b600 0000  u..........r....
+00004270: 7249 0000 0072 ae00 0000 72b7 0000 0072  rI...r....r....r
+00004280: 8100 0000 72b9 0000 00e9 c800 0000 72ba  ....r.........r.
+00004290: 0000 0072 3000 0000 750c 0000 00e6 9c89  ...r0...u.......
+000042a0: e695 88e6 97a5 e69c 9f72 1100 0000 72b8  .........r....r.
+000042b0: 0000 0072 0100 0000 727a 0000 0075 0c00  ...r....rz...u..
+000042c0: 0000 e8ae a1e9 878f e58d 95e4 bd8d 750c  ..............u.
+000042d0: 0000 00e6 8890 e69c ace5 8d95 e4bb b772  ...............r
+000042e0: 9000 0000 750c 0000 00e6 8890 e69c ace9  ....u...........
+000042f0: 8791 e9a2 9d75 0c00 0000 e99b b6e5 94ae  .....u..........
+00004300: e58d 95e4 bbb7 750c 0000 00e9 9bb6 e594  ......u.........
+00004310: aee9 8791 e9a2 9d63 0000 0000 0000 0000  .......c........
+00004320: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00004330: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00004340: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
+00004350: 1150 6861 726d 6163 7944 7275 672e 4d65  .PharmacyDrug.Me
+00004360: 7461 5a10 6273 5f70 6861 726d 6163 795f  taZ.bs_pharmacy_
+00004370: 6472 7567 750d 0000 00e8 8daf e688 bf2d  drugu..........-
+00004380: e88d afe5 9381 4e72 3700 0000 721a 0000  ......Nr7...r...
+00004390: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000043a0: 721c 0000 001d 0200 0073 0600 0000 0801  r........s......
+000043b0: 0401 0401 721c 0000 004e 2923 7216 0000  ....r....N)#r...
+000043c0: 0072 1700 0000 7218 0000 0072 0500 0000  .r....r....r....
+000043d0: 7242 0000 0072 c700 0000 7243 0000 005a  rB...r....rC...Z
+000043e0: 0870 6861 726d 6163 7972 3a00 0000 72bb  .pharmacyr:...r.
+000043f0: 0000 0072 bc00 0000 72bd 0000 00da 0575  ...r....r......u
+00004400: 6e69 7473 72aa 0000 0072 be00 0000 72bf  nitsr....r....r.
+00004410: 0000 0072 ac00 0000 72c1 0000 0072 b100  ...r....r....r..
+00004420: 0000 72c0 0000 0072 c200 0000 72c3 0000  ..r....r....r...
+00004430: 0072 2200 0000 724b 0000 0072 6000 0000  .r"...rK...r`...
+00004440: 5a0a 7661 6c69 645f 6461 7465 7270 0000  Z.valid_daterp..
+00004450: 005a 1269 6e76 656e 746f 7279 5f71 7561  .Z.inventory_qua
+00004460: 6e74 6974 795a 106d 6561 7375 7265 6d65  ntityZ.measureme
+00004470: 6e74 5f75 6e69 7472 4100 0000 5a0f 636f  nt_unitrA...Z.co
+00004480: 7374 5f75 6e69 745f 7072 6963 655a 0b63  st_unit_priceZ.c
+00004490: 6f73 745f 616d 6f75 6e74 5a11 7265 7461  ost_amountZ.reta
+000044a0: 696c 5f75 6e69 745f 7072 6963 655a 0d72  il_unit_priceZ.r
+000044b0: 6574 6169 6c5f 616d 6f75 6e74 721c 0000  etail_amountr...
+000044c0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+000044d0: 721b 0000 0072 c800 0000 fd01 0000 733e  r....r........s>
+000044e0: 0000 0008 0114 0112 0112 0112 0112 0104  ................
+000044f0: 0102 0102 0104 fd06 0504 0102 0102 0104  ................
+00004500: fd06 0504 0102 0102 0104 fd06 0512 0112  ................
+00004510: 0114 0110 0110 0112 010e 010e 010e 010e  ................
+00004520: 0272 c800 0000 6300 0000 0000 0000 0000  .r....c.........
+00004530: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+00004540: a800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00004550: 6401 6402 6403 8d02 5a05 6503 6a04 6401  d.d.d...Z.e.j.d.
+00004560: 6404 6403 8d02 5a06 6503 6a04 6401 6405  d.d...Z.e.j.d.d.
+00004570: 6406 6406 6407 8d04 5a07 6503 6a04 6401  d.d.d...Z.e.j.d.
+00004580: 6408 6403 8d02 5a08 6503 6a04 6401 6409  d.d...Z.e.j.d.d.
+00004590: 6403 8d02 5a09 6503 6a04 640a 640b 6403  d...Z.e.j.d.d.d.
+000045a0: 8d02 5a0a 6503 6a0b 640c 6406 6406 640d  ..Z.e.j.d.d.d.d.
+000045b0: 8d03 5a0c 6503 6a0b 640e 6406 6406 640f  ..Z.e.j.d.d.d.d.
+000045c0: 8d03 5a0d 6503 6a0e 6410 6406 6411 8d02  ..Z.e.j.d.d.d...
+000045d0: 5a0f 4700 6412 6413 8400 6413 8302 5a10  Z.G.d.d...d...Z.
+000045e0: 6414 6415 8400 5a11 6416 5300 2917 da07  d.d...Z.d.S.)...
+000045f0: 4170 6949 6e66 6f72 7700 0000 72a2 0000  ApiInforw...r...
+00004600: 0072 7800 0000 750c 0000 00e8 afb7 e6b1  .rx...u.........
+00004610: 82e7 bc96 e7a0 8175 0c00 0000 e8af b7e6  .......u........
+00004620: b182 e590 8de7 a7b0 5472 7b00 0000 750c  ........Tr{...u.
+00004630: 0000 00e8 afb7 e6b1 82e6 96b9 e5bc 8f75  ...............u
+00004640: 1200 0000 e8af b7e6 b182 e695 b0e6 8dae  ................
+00004650: e7b1 bbe5 9e8b 72c9 0000 0075 0c00 0000  ......r....u....
+00004660: e8af b7e6 b182 e8b7 afe7 94b1 720b 0000  ............r...
+00004670: 0072 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00004680: 7213 0000 0072 1400 0000 6300 0000 0000  r....r....c.....
+00004690: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000046a0: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000046b0: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
+000046c0: 6404 5300 2905 7a0c 4170 6949 6e66 6f2e  d.S.).z.ApiInfo.
+000046d0: 4d65 7461 5a0b 6273 5f61 7069 5f69 6e66  MetaZ.bs_api_inf
+000046e0: 6f75 0c00 0000 e68e a5e5 8fa3 e4bf a1e6  ou..............
+000046f0: 81af 2901 a902 da08 6f72 675f 636f 6465  ..).....org_code
+00004700: da08 7265 715f 636f 6465 4e72 4c00 0000  ..req_codeNrL...
+00004710: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00004720: 1b00 0000 721c 0000 002e 0200 0073 0800  ....r........s..
+00004730: 0000 0801 0401 0401 0401 721c 0000 0063  ..........r....c
+00004740: 0300 0000 0000 0000 0000 0000 0700 0000  ................
+00004750: 0500 0000 4300 0000 73b8 0000 0074 006a  ....C...s....t.j
+00004760: 016a 027c 0164 0119 007c 0264 028d 02a0  .j.|.d...|.d....
+00004770: 03a1 007d 037c 0372 a674 047c 036a 0517  ...}.|.r.t.|.j..
+00004780: 007d 047c 036a 0664 036b 0272 4074 076a  .}.|.j.d.k.r@t.j
+00004790: 087c 047c 0164 048d 027d 056e 587c 036a  .|.|.d...}.nX|.j
+000047a0: 0664 056b 0272 5a74 076a 097c 047c 0164  .d.k.rZt.j.|.|.d
+000047b0: 068d 027d 056e 3e7c 036a 0664 076b 0272  ...}.n>|.j.d.k.r
+000047c0: 7474 076a 0a7c 047c 0164 088d 027d 056e  tt.j.|.|.d...}.n
+000047d0: 247c 036a 0664 096b 0272 8c74 076a 0b7c  $|.j.d.k.r.t.j.|
+000047e0: 0464 0a8d 017d 056e 0c74 076a 0c7c 0464  .d...}.n.t.j.|.d
+000047f0: 0a8d 017d 0574 0da0 0e7c 056a 0fa1 017d  ...}.t...|.j...}
+00004800: 066e 0e64 0b64 0c64 0d69 0064 0e9c 047d  .n.d.d.d.i.d...}
+00004810: 067c 0653 0029 0f4e 72a7 0000 0072 cc00  .|.S.).Nr....r..
+00004820: 0000 da04 504f 5354 2902 728e 0000 00da  ....POST).r.....
+00004830: 046a 736f 6eda 0347 4554 2902 728e 0000  .json..GET).r...
+00004840: 00da 0670 6172 616d 73da 0350 5554 2902  ...params..PUT).
+00004850: 728e 0000 00da 0464 6174 61da 0644 454c  r......data..DEL
+00004860: 4554 4529 0172 8e00 0000 4669 d107 0000  ETE).r....Fi....
+00004870: 751e 0000 00e4 b88d e5ad 98e5 9ca8 e5af  u...............
+00004880: b9e6 8ea5 e58c bbe9 99a2 e4bf a1e6 81af  ................
+00004890: efbc 8129 04da 0773 7563 6365 7373 72b0  ...)...successr.
+000048a0: 0000 00da 076d 6573 7361 6765 72d4 0000  .....messager...
+000048b0: 0029 1072 cb00 0000 da07 6f62 6a65 6374  .).r......object
+000048c0: 73da 0666 696c 7465 7272 6800 0000 7207  s..filterrh...r.
+000048d0: 0000 0072 9200 0000 da0a 7265 715f 6d65  ...r......req_me
+000048e0: 7468 6f64 da08 7265 7175 6573 7473 da04  thod..requests..
+000048f0: 706f 7374 da03 6765 74da 0370 7574 da06  post..get..put..
+00004900: 6465 6c65 7465 da05 7061 7463 6872 d000  delete..patchr..
+00004910: 0000 da05 6c6f 6164 73da 0474 6578 7429  ....loads..text)
+00004920: 0772 2f00 0000 5a07 696e 5f64 6174 6172  .r/...Z.in_datar
+00004930: ce00 0000 5a0c 6170 695f 696e 666f 5f6f  ....Z.api_info_o
+00004940: 626a 5a07 636d 735f 7572 6cda 0372 6573  bjZ.cms_url..res
+00004950: 5a08 7265 735f 6a73 6f6e 721a 0000 0072  Z.res_jsonr....r
+00004960: 1a00 0000 721b 0000 00da 0977 7269 7465  ....r......write
+00004970: 6261 636b 3602 0000 731e 0000 0000 0118  back6...s.......
+00004980: 0104 010a 010a 0110 010a 0110 010a 0110  ................
+00004990: 010a 010e 020c 010e 020e 017a 1141 7069  ...........z.Api
+000049a0: 496e 666f 2e77 7269 7465 6261 636b 4e29  Info.writebackN)
+000049b0: 1272 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+000049c0: 7205 0000 0072 3a00 0000 72cd 0000 0072  r....r:...r....r
+000049d0: ce00 0000 5a08 7265 715f 6e61 6d65 72da  ....Z.req_namer.
+000049e0: 0000 0072 9100 0000 7292 0000 0072 1d00  ...r....r....r..
+000049f0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00004a00: 0072 2100 0000 721c 0000 0072 e400 0000  .r!...r....r....
+00004a10: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00004a20: 1b00 0000 72cb 0000 0023 0200 0073 1600  ....r....#...s..
+00004a30: 0000 0801 0e01 0e01 1201 0e01 0e01 0e01  ................
+00004a40: 1001 1001 0e02 0e08 72cb 0000 0029 2872  ........r....)(r
+00004a50: d000 0000 da02 6f73 72db 0000 00da 1a64  ......osr......d
+00004a60: 6a61 6e67 6f2e 636f 6e74 7269 622e 6175  jango.contrib.au
+00004a70: 7468 2e6d 6f64 656c 7372 0200 0000 7203  th.modelsr....r.
+00004a80: 0000 00da 2264 6a61 6e67 6f2e 636f 6e74  ...."django.cont
+00004a90: 7269 622e 636f 6e74 656e 7474 7970 6573  rib.contenttypes
+00004aa0: 2e6d 6f64 656c 7372 0400 0000 da09 646a  .modelsr......dj
+00004ab0: 616e 676f 2e64 6272 0500 0000 da0b 646a  ango.dbr......dj
+00004ac0: 616e 676f 2e63 6f6e 6672 0600 0000 da0f  ango.confr......
+00004ad0: 646a 616e 676f 5f73 6574 7469 6e67 73da  django_settings.
+00004ae0: 0767 6574 6174 7472 7207 0000 0072 5d00  .getattrr....r].
+00004af0: 0000 da05 4d6f 6465 6c72 0a00 0000 7222  ....Modelr....r"
+00004b00: 0000 0072 4700 0000 724e 0000 0072 5000  ...rG...rN...rP.
+00004b10: 0000 7263 0000 0072 7400 0000 727f 0000  ..rc...rt...r...
+00004b20: 0072 8c00 0000 7294 0000 0072 9700 0000  .r....r....r....
+00004b30: 729e 0000 0072 a800 0000 72a9 0000 0072  r....r....r....r
+00004b40: aa00 0000 72ac 0000 0072 b100 0000 72b2  ....r....r....r.
+00004b50: 0000 0072 c400 0000 72c6 0000 0072 c700  ...r....r....r..
+00004b60: 0000 72c8 0000 0072 cb00 0000 721a 0000  ..r....r....r...
+00004b70: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00004b80: da08 3c6d 6f64 756c 653e 0100 0000 733e  ..<module>....s>
+00004b90: 0000 0008 0108 0208 0110 010c 010c 010c  ................
+00004ba0: 020a 0204 0612 0910 1e10 1c10 1410 2810  ..............(.
+00004bb0: 4a12 1a12 1b12 2310 1910 1110 1110 1110  J.....#.........
+00004bc0: 1110 0a10 0a10 0a10 2910 0a10 0a10 1210  ........).......
+00004bd0: 26                                       &
```

### Comparing `base_system-0.1.0/base_system/auth.py` & `base_system-0.1.2/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.0/base_system/migrations/0001_initial.py` & `base_system-0.1.2/base_system/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 3.2 on 2023-02-13 19:27
+# Generated by Django 3.2 on 2023-04-27 10:27
 
 import django.contrib.auth.models
 import django.contrib.auth.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 
@@ -17,58 +17,29 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='ContentTypeCates',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=20, null=True, verbose_name='名称')),
-                ('is_active', models.BooleanField(default=True, null=True, verbose_name='是否启用')),
+                ('name', models.CharField(max_length=20, verbose_name='名称')),
+                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('order_by', models.IntegerField(default=1, null=True, verbose_name='排序')),
                 ('level', models.IntegerField(blank=True, default=1, null=True, verbose_name='级别')),
                 ('icon_class', models.CharField(blank=True, max_length=500, null=True, verbose_name='图标')),
                 ('parent', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='children', to='base_system.contenttypecates', verbose_name='父级菜单')),
             ],
             options={
                 'verbose_name': '菜单名称',
                 'verbose_name_plural': '菜单名称',
                 'db_table': 'bs_content_type_cats',
                 'ordering': ('order_by',),
             },
         ),
         migrations.CreateModel(
-            name='Doctor',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
-                ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
-                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
-                ('name', models.CharField(max_length=255, verbose_name='名称')),
-                ('phone', models.CharField(blank=True, max_length=100, null=True, verbose_name='联系方式')),
-                ('email', models.CharField(blank=True, max_length=100, null=True, verbose_name='邮箱')),
-                ('address', models.CharField(blank=True, max_length=255, null=True, verbose_name='地址')),
-                ('job_number', models.CharField(blank=True, max_length=255, null=True, verbose_name='工号')),
-                ('position', models.CharField(blank=True, max_length=100, null=True, verbose_name='职位')),
-                ('gender', models.CharField(blank=True, choices=[('1', '男'), ('0', '女')], max_length=2, null=True, verbose_name='性别')),
-                ('nation', models.CharField(blank=True, max_length=32, null=True, verbose_name='民族')),
-                ('idnum', models.CharField(blank=True, max_length=100, null=True, verbose_name='身份证号')),
-                ('birthday', models.DateField(blank=True, null=True, verbose_name='出生日期')),
-                ('photo', models.CharField(default='doctor_photo', max_length=100, verbose_name='医生照片')),
-                ('describe', models.TextField(blank=True, null=True, verbose_name='医生描述')),
-                ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
-                ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
-                ('is_online_consult', models.BooleanField(default=True, verbose_name='是否互联网接诊')),
-            ],
-            options={
-                'verbose_name': '医生表',
-                'verbose_name_plural': '医生表',
-                'db_table': 'bs_doctor',
-            },
-        ),
-        migrations.CreateModel(
             name='DrugCategory',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('codenum', models.CharField(max_length=255, unique=True, verbose_name='编码')),
@@ -152,16 +123,16 @@
                 ('hos_images', models.CharField(blank=True, default='hospital_images', max_length=100, verbose_name='医院图片')),
                 ('logo', models.CharField(default='hospital_logo', max_length=100, verbose_name='logo')),
                 ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
                 ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
                 ('parent', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
             ],
             options={
-                'verbose_name': '医院表',
-                'verbose_name_plural': '医院表',
+                'verbose_name': '医院',
+                'verbose_name_plural': '医院',
                 'db_table': 'bs_hospital',
             },
         ),
         migrations.CreateModel(
             name='InspectionDictionaries',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
@@ -171,16 +142,16 @@
                 ('project_code', models.CharField(max_length=255, unique=True, verbose_name='项目编码')),
                 ('project_name', models.CharField(max_length=64, verbose_name='项目名称')),
                 ('hospital_code', models.CharField(max_length=128, verbose_name='医院编码')),
                 ('office_code', models.CharField(max_length=128, verbose_name='科室编码')),
                 ('project_fees', models.FloatField(null=True, verbose_name='项目费用')),
                 ('remarks', models.CharField(blank=True, max_length=128, null=True, verbose_name='备注')),
                 ('distinguish', models.CharField(blank=True, max_length=128, null=True, verbose_name='区分字段')),
-                ('code_srvtp', models.CharField(max_length=50, null=True, verbose_name='检验类型编码')),
-                ('name_srvtp', models.CharField(max_length=50, null=True, verbose_name='检验类型名称')),
+                ('code_srvtp', models.CharField(max_length=50, null=True, verbose_name='检查类型编码')),
+                ('name_srvtp', models.CharField(max_length=50, null=True, verbose_name='检查类型名称')),
             ],
             options={
                 'verbose_name': '检查字典',
                 'verbose_name_plural': '检查字典',
                 'db_table': 'bs_inspection_dictionaries',
             },
         ),
@@ -220,23 +191,24 @@
             name='PositionTitle',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('name', models.CharField(max_length=255, verbose_name='名称')),
-                ('codenum', models.CharField(max_length=255, unique=True, verbose_name='职称编码')),
+                ('codenum', models.CharField(max_length=255, verbose_name='职称编码')),
                 ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
                 ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
                 ('hospital', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
             ],
             options={
-                'verbose_name': '职称表',
-                'verbose_name_plural': '职称表',
+                'verbose_name': '职称',
+                'verbose_name_plural': '职称',
                 'db_table': 'bs_position_title',
+                'unique_together': {('codenum', 'hospital')},
             },
         ),
         migrations.CreateModel(
             name='PharmacyManagement',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
@@ -262,17 +234,17 @@
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('drug_code', models.CharField(blank=True, max_length=255, null=True, verbose_name='药品编码')),
                 ('drug_name', models.CharField(blank=True, max_length=64, null=True, verbose_name='药品名称')),
                 ('standards', models.CharField(blank=True, max_length=64, null=True, verbose_name='规格')),
                 ('units', models.CharField(blank=True, max_length=64, null=True, verbose_name='单位')),
-                ('origin_place', models.CharField(blank=True, max_length=64, null=True, verbose_name='产地')),
-                ('manufacturer', models.CharField(blank=True, max_length=64, null=True, verbose_name='生产厂家')),
-                ('valid_date', models.DateTimeField(auto_now=True, null=True, verbose_name='有效日期')),
+                ('origin_place', models.CharField(blank=True, max_length=500, null=True, verbose_name='产地')),
+                ('manufacturer', models.CharField(blank=True, max_length=200, null=True, verbose_name='生产厂家')),
+                ('valid_date', models.DateField(auto_now=True, null=True, verbose_name='有效日期')),
                 ('inventory_quantity', models.IntegerField(default=0, null=True, verbose_name='库存数量')),
                 ('measurement_unit', models.CharField(blank=True, max_length=64, null=True, verbose_name='计量单位')),
                 ('cost_unit_price', models.FloatField(null=True, verbose_name='成本单价')),
                 ('cost_amount', models.FloatField(null=True, verbose_name='成本金额')),
                 ('retail_unit_price', models.FloatField(null=True, verbose_name='零售单价')),
                 ('retail_amount', models.FloatField(null=True, verbose_name='零售金额')),
                 ('category', models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, to='base_system.drugcategory', verbose_name='类别')),
@@ -293,84 +265,96 @@
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('name', models.CharField(max_length=255, verbose_name='名称')),
                 ('address', models.CharField(blank=True, max_length=255, null=True, verbose_name='科室位置')),
                 ('phone', models.CharField(blank=True, max_length=255, null=True, verbose_name='联系方式')),
-                ('codenum', models.CharField(max_length=255, unique=True, verbose_name='科室编码')),
+                ('codenum', models.CharField(max_length=255, verbose_name='科室编码')),
                 ('office_type', models.CharField(blank=True, max_length=100, null=True, verbose_name='类型')),
                 ('introduce', models.TextField(blank=True, null=True, verbose_name='科室简介')),
-                ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
-                ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
                 ('hospital', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
                 ('parent', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.office', verbose_name='上级科室')),
             ],
             options={
-                'verbose_name': '科室表',
-                'verbose_name_plural': '科室表',
+                'verbose_name': '科室',
+                'verbose_name_plural': '科室',
                 'db_table': 'bs_office',
+                'unique_together': {('codenum', 'hospital')},
+            },
+        ),
+        migrations.CreateModel(
+            name='InspectionType',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
+                ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
+                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
+                ('code_srvtp', models.CharField(max_length=50, verbose_name='检查类型编码')),
+                ('name_srvtp', models.CharField(max_length=50, verbose_name='检查类型名称')),
+                ('parent', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='children', to='base_system.inspectiontype', verbose_name='父级')),
+            ],
+            options={
+                'verbose_name': '检查字典类型',
+                'verbose_name_plural': '检查字典类型',
+                'db_table': 'bs_inspection_type',
             },
         ),
         migrations.CreateModel(
             name='ExtraGroup',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('role_code', models.CharField(max_length=50, unique=True, verbose_name='角色代码')),
+                ('role_name', models.CharField(max_length=50, verbose_name='角色名称')),
                 ('is_active', models.BooleanField(default=True, null=True, verbose_name='是否启用')),
                 ('note', models.CharField(blank=True, max_length=50, null=True, verbose_name='描述')),
                 ('order_by', models.IntegerField(default=1, null=True, verbose_name='排序')),
-                ('role_code', models.CharField(max_length=50, unique=True, verbose_name='角色代码')),
                 ('created_user', models.CharField(blank=True, max_length=50, null=True, verbose_name='创建人')),
                 ('created_at', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_at', models.DateTimeField(auto_now=True, null=True, verbose_name='最后更新时间')),
                 ('group', models.OneToOneField(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='extra_group', to='auth.group')),
                 ('hospital', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='groups', to='base_system.hospital', verbose_name='所属医院')),
             ],
             options={
                 'verbose_name': '角色',
                 'verbose_name_plural': '角色',
                 'db_table': 'bs_extra_group',
             },
         ),
         migrations.CreateModel(
-            name='ExpenseStandard',
+            name='ExaminationType',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
-                ('expense_type', models.CharField(max_length=100, null=True, verbose_name='费用类型')),
-                ('standard_name', models.CharField(max_length=100, verbose_name='标准名称')),
-                ('standard_code', models.CharField(max_length=255, unique=True, verbose_name='标准编码')),
-                ('fees', models.FloatField(null=True, verbose_name='费用')),
-                ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
-                ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
-                ('doctors', models.ManyToManyField(blank=True, to='base_system.Doctor', verbose_name='医生费用标准')),
-                ('hospital', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
+                ('code_srvtp', models.CharField(max_length=50, verbose_name='检查类型编码')),
+                ('name_srvtp', models.CharField(max_length=50, verbose_name='检查类型名称')),
+                ('parent', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='children', to='base_system.examinationtype', verbose_name='父级')),
             ],
             options={
-                'verbose_name': '费用标准表',
-                'verbose_name_plural': '费用标准表',
-                'db_table': 'bs_expense_standard',
+                'verbose_name': '检验字典类型',
+                'verbose_name_plural': '检验字典类型',
+                'db_table': 'bs_examination_type',
             },
         ),
         migrations.CreateModel(
             name='DrugDirectory',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
                 ('drug_code', models.CharField(max_length=255, unique=True, verbose_name='药品编码')),
                 ('drug_name', models.CharField(blank=True, max_length=64, null=True, verbose_name='药品名称')),
                 ('standards', models.CharField(blank=True, max_length=64, null=True, verbose_name='规格')),
-                ('units', models.CharField(blank=True, max_length=64, null=True, verbose_name='单位')),
+                ('total_unit', models.CharField(blank=True, max_length=64, null=True, verbose_name='基本单位')),
                 ('total_unit_code', models.CharField(blank=True, max_length=20, null=True, verbose_name='总量单位编码')),
                 ('unit_dose', models.CharField(blank=True, max_length=20, null=True, verbose_name='单位剂量')),
-                ('measure_unit', models.CharField(blank=True, max_length=20, null=True, verbose_name='计量单位')),
+                ('measure_unit', models.CharField(blank=True, max_length=20, null=True, verbose_name='计量/零售单位')),
                 ('measure_unit_code', models.CharField(blank=True, max_length=20, null=True, verbose_name='计量单位编码')),
                 ('stock_left', models.CharField(blank=True, max_length=20, null=True, verbose_name='库存数量')),
                 ('stock_unit', models.CharField(blank=True, max_length=20, null=True, verbose_name='库存单位')),
                 ('mic', models.CharField(blank=True, max_length=20, null=True, verbose_name='医保类别')),
                 ('rcc_category', models.CharField(blank=True, max_length=20, null=True, verbose_name='农合类别')),
                 ('is_essential', models.BooleanField(default=True, verbose_name='是否是基药')),
                 ('hr_level', models.CharField(blank=True, max_length=64, null=True, verbose_name='高危等级')),
@@ -384,28 +368,45 @@
             ],
             options={
                 'verbose_name': '药品目录',
                 'verbose_name_plural': '药品目录',
                 'db_table': 'bs_drug_directory',
             },
         ),
-        migrations.AddField(
-            model_name='doctor',
-            name='doc_rank',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.positiontitle', verbose_name='职称'),
-        ),
-        migrations.AddField(
-            model_name='doctor',
-            name='hospital',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院'),
-        ),
-        migrations.AddField(
-            model_name='doctor',
-            name='office',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.office', verbose_name='所属科室'),
+        migrations.CreateModel(
+            name='Doctor',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
+                ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
+                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
+                ('name', models.CharField(max_length=20, verbose_name='名称')),
+                ('phone', models.CharField(blank=True, max_length=20, null=True, verbose_name='联系方式')),
+                ('email', models.CharField(blank=True, max_length=100, null=True, verbose_name='邮箱')),
+                ('address', models.CharField(blank=True, max_length=255, null=True, verbose_name='地址')),
+                ('codenum', models.CharField(max_length=64, verbose_name='工号')),
+                ('position', models.CharField(blank=True, max_length=20, null=True, verbose_name='职位')),
+                ('gender', models.CharField(blank=True, choices=[('1', '男'), ('0', '女')], max_length=2, null=True, verbose_name='性别')),
+                ('nation', models.CharField(blank=True, max_length=10, null=True, verbose_name='民族')),
+                ('idnum', models.CharField(blank=True, max_length=100, null=True, verbose_name='身份证号')),
+                ('birthday', models.DateField(blank=True, null=True, verbose_name='出生日期')),
+                ('photo', models.CharField(default='doctor_photo', max_length=10, verbose_name='医生照片')),
+                ('describe', models.TextField(blank=True, null=True, verbose_name='医生描述')),
+                ('created_by', models.CharField(blank=True, max_length=20, null=True, verbose_name='创建人')),
+                ('updated_by', models.CharField(blank=True, max_length=20, null=True, verbose_name='更新人')),
+                ('is_online_consult', models.BooleanField(default=True, verbose_name='是否互联网接诊')),
+                ('hospital', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
+                ('office', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.office', verbose_name='所属科室')),
+                ('position_title', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='base_system.positiontitle', verbose_name='职称')),
+            ],
+            options={
+                'verbose_name': '医生表',
+                'verbose_name_plural': '医生表',
+                'db_table': 'bs_doctor',
+            },
         ),
         migrations.CreateModel(
             name='ContentTypeEx',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=20, null=True, verbose_name='名称')),
                 ('icon_class', models.CharField(blank=True, max_length=500, null=True, verbose_name='图标')),
@@ -422,28 +423,49 @@
                 'verbose_name': '功能类别补充',
                 'verbose_name_plural': '功能类别补充',
                 'db_table': 'bs_content_type_ex',
                 'ordering': ('order_by',),
             },
         ),
         migrations.CreateModel(
+            name='ApiInfo',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('org_code', models.CharField(max_length=50, verbose_name='医院编码')),
+                ('req_code', models.CharField(max_length=50, verbose_name='请求编码')),
+                ('req_name', models.CharField(blank=True, max_length=50, null=True, verbose_name='请求名称')),
+                ('req_method', models.CharField(max_length=50, verbose_name='请求方式')),
+                ('content_type', models.CharField(max_length=50, verbose_name='请求数据类型')),
+                ('front_url', models.CharField(max_length=200, verbose_name='请求路由')),
+                ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
+                ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
+                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
+            ],
+            options={
+                'verbose_name': '接口信息',
+                'verbose_name_plural': '接口信息',
+                'db_table': 'bs_api_info',
+                'unique_together': {('org_code', 'req_code')},
+            },
+        ),
+        migrations.CreateModel(
             name='User',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('password', models.CharField(max_length=128, verbose_name='password')),
+                ('last_login', models.DateTimeField(blank=True, null=True, verbose_name='last login')),
+                ('is_superuser', models.BooleanField(default=False, help_text='Designates that this user has all permissions without explicitly assigning them.', verbose_name='superuser status')),
                 ('username', models.CharField(error_messages={'unique': 'A user with that username already exists.'}, help_text='Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.', max_length=150, unique=True, validators=[django.contrib.auth.validators.UnicodeUsernameValidator()], verbose_name='username')),
                 ('first_name', models.CharField(blank=True, max_length=150, verbose_name='first name')),
                 ('last_name', models.CharField(blank=True, max_length=150, verbose_name='last name')),
                 ('email', models.EmailField(blank=True, max_length=254, verbose_name='email address')),
                 ('is_staff', models.BooleanField(default=False, help_text='Designates whether the user can log into this admin site.', verbose_name='staff status')),
                 ('is_active', models.BooleanField(default=True, help_text='Designates whether this user should be treated as active. Unselect this instead of deleting accounts.', verbose_name='active')),
                 ('date_joined', models.DateTimeField(default=django.utils.timezone.now, verbose_name='date joined')),
                 ('name', models.CharField(blank=True, max_length=255, null=True, verbose_name='名称')),
-                ('password', models.CharField(blank=True, max_length=255, null=True, verbose_name='密码')),
-                ('last_login', models.DateField(blank=True, null=True, verbose_name='上次登录时间')),
-                ('is_superuser', models.BooleanField(default=False, verbose_name='是否是超管')),
                 ('phone', models.CharField(blank=True, max_length=100, null=True, verbose_name='联系方式')),
                 ('birthday', models.DateField(blank=True, null=True, verbose_name='出生日期')),
                 ('gender', models.CharField(blank=True, choices=[('1', '男'), ('0', '女')], max_length=2, null=True, verbose_name='性别')),
                 ('idcardnum', models.CharField(blank=True, max_length=100, null=True, verbose_name='身份证号')),
                 ('order_by', models.IntegerField(blank=True, default=1, null=True, verbose_name='排序')),
                 ('avatar_url', models.CharField(default='user_avatar', max_length=100, verbose_name='用户头像')),
                 ('default_group_id', models.CharField(blank=True, max_length=255, null=True, verbose_name='默认角色')),
@@ -454,17 +476,45 @@
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('doctor', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.doctor', verbose_name='绑定医生')),
                 ('groups', models.ManyToManyField(blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.', related_name='user_set', related_query_name='user', to='auth.Group', verbose_name='groups')),
                 ('hospital', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
                 ('office', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.office', verbose_name='所属科室')),
                 ('user_permissions', models.ManyToManyField(blank=True, help_text='Specific permissions for this user.', related_name='user_set', related_query_name='user', to='auth.Permission', verbose_name='user permissions')),
-                ('user_rank', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.positiontitle', verbose_name='职称')),
             ],
             options={
-                'verbose_name': '用户表',
+                'verbose_name': '用户信息',
             },
             managers=[
                 ('objects', django.contrib.auth.models.UserManager()),
             ],
+
+        ),
+        migrations.RunSQL(
+            """
+            INSERT INTO "base_system_user"("id", "username", "first_name", "last_name", "email", "is_staff", "is_active", "date_joined", "name", "password", "last_login", "is_superuser", "phone", "birthday", "gender", "idcardnum", "order_by", "avatar_url", "default_group_id", "allow_office", "note", "created_by", "created_time", "updated_time", "hospital_id", "office_id", "user_rank_id", "updated_by", "doctor_id") VALUES (1, 'admin', '', '', 'admin@admin.com', 't', 't', '2023-02-13 10:22:39+08', '管理员', 'pbkdf2_sha256$260000$eR3ouH02QKSmOTLN0Y2vsL$rx5zmoAR0PgQ2fB6l5gKLCvLPxkw2NtBsTDXQO7iIT8=', '2022-09-08', 't', NULL, NULL, NULL, NULL, 1, 'user_avatar', NULL, NULL, NULL, NULL, '2022-09-08 16:32:24.192312+08', '2023-03-23 09:54:21.211661+08', NULL, NULL, NULL, NULL, NULL);
+            """
+        ),
+        migrations.CreateModel(
+            name='ExpenseStandard',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
+                ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
+                ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
+                ('expense_type', models.CharField(max_length=100, null=True, verbose_name='费用类型')),
+                ('standard_name', models.CharField(max_length=100, verbose_name='标准名称')),
+                ('standard_code', models.CharField(max_length=255, verbose_name='标准编码')),
+                ('fees', models.FloatField(null=True, verbose_name='费用')),
+                ('created_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='创建人')),
+                ('updated_by', models.CharField(blank=True, max_length=100, null=True, verbose_name='更新人')),
+                ('doctors', models.ManyToManyField(blank=True, to='base_system.Doctor', verbose_name='医生费用标准')),
+                ('hospital', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='base_system.hospital', verbose_name='所属医院')),
+            ],
+            options={
+                'verbose_name': '费用标准表',
+                'verbose_name_plural': '费用标准表',
+                'db_table': 'bs_expense_standard',
+                'unique_together': {('standard_code', 'hospital')},
+            },
         ),
     ]
```

### Comparing `base_system-0.1.0/base_system/models.py` & `base_system-0.1.2/base_system/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import json
 import os
 
+import requests
 from django.contrib.auth.models import AbstractUser, Group
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
+from django.conf import settings as django_settings
+
+WRITEBACK_IP = getattr(django_settings, 'WRITEBACK_IP')
 
 GENDER_CHOICE = (
     ('1', '男'),
     ('0', '女'),
 )
 
 
@@ -38,143 +43,147 @@
     # logo = models.ImageField(verbose_name="logo", upload_to="images/logo", null=True, blank=True)
     logo = models.CharField(verbose_name="logo", max_length=100, default='hospital_logo')
     created_by = models.CharField(verbose_name="创建人", max_length=100, null=True, blank=True)
     updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
 
     class Meta:
         db_table = "bs_hospital"
-        verbose_name = "医院表"
+        verbose_name = "医院"
         verbose_name_plural = verbose_name
 
     # def __str__(self):
     #     return self.name
 
 
 class Office(MedicalBaseModel):
     name = models.CharField(verbose_name="名称", max_length=255)
     address = models.CharField(verbose_name="科室位置", max_length=255, null=True, blank=True)
     phone = models.CharField(verbose_name='联系方式', max_length=255, null=True, blank=True)
-    codenum = models.CharField(verbose_name="科室编码", max_length=255, unique=True)
+    codenum = models.CharField(verbose_name="科室编码", max_length=255)
     office_type = models.CharField(verbose_name="类型", max_length=100, null=True, blank=True)
     introduce = models.TextField(verbose_name="科室简介", null=True, blank=True)
     hospital = models.ForeignKey(
         Hospital,
         verbose_name="所属医院",
         on_delete=models.CASCADE,
     )
-    parent = models.ForeignKey('self',
-                               verbose_name="上级科室",
-                               on_delete=models.CASCADE,
-                               null=True)
-    created_by = models.CharField(verbose_name="创建人", max_length=100, null=True, blank=True)
-    updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
+    parent = models.ForeignKey(
+        'self',
+        verbose_name="上级科室",
+        on_delete=models.CASCADE,
+        null=True
+    )
 
     class Meta:
         db_table = "bs_office"
-        verbose_name = "科室表"
+        verbose_name = "科室"
         verbose_name_plural = verbose_name
+        unique_together = (
+            ('codenum', 'hospital',),  # 联合唯一
+        )
 
 
 class PositionTitle(MedicalBaseModel):
     name = models.CharField(verbose_name="名称", max_length=255)
-    codenum = models.CharField(verbose_name="职称编码", max_length=255, unique=True)
+    codenum = models.CharField(verbose_name="职称编码", max_length=255)
     hospital = models.ForeignKey(
         Hospital,
         verbose_name="所属医院",
         on_delete=models.CASCADE,
     )
     created_by = models.CharField(verbose_name="创建人", max_length=100, null=True, blank=True)
     updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
 
     class Meta:
         db_table = "bs_position_title"
-        verbose_name = "职称表"
+        verbose_name = "职称"
         verbose_name_plural = verbose_name
+        unique_together = (
+            ('codenum', 'hospital',),  # 联合唯一
+        )
 
 
 class Doctor(MedicalBaseModel):
-    name = models.CharField(verbose_name="名称", max_length=255)
-    phone = models.CharField(verbose_name='联系方式', max_length=100, null=True, blank=True)
+    name = models.CharField(verbose_name="名称", max_length=20)
+    phone = models.CharField(verbose_name='联系方式', max_length=20, null=True, blank=True)
     email = models.CharField(verbose_name='邮箱', max_length=100, null=True, blank=True)
     address = models.CharField(verbose_name="地址", max_length=255, null=True, blank=True)
-    job_number = models.CharField(verbose_name="工号", max_length=255, null=True, blank=True)
-    position = models.CharField(verbose_name="职位", max_length=100, null=True, blank=True)
-    doc_rank = models.ForeignKey(PositionTitle,
-                                 verbose_name="职称",
-                                 on_delete=models.CASCADE,
-                                 )
+    codenum = models.CharField(verbose_name="工号", max_length=64)
+    position = models.CharField(verbose_name="职位", max_length=20, null=True, blank=True)
+    position_title = models.ForeignKey(
+        PositionTitle,
+        verbose_name="职称",
+        on_delete=models.CASCADE,
+    )
     gender = models.CharField(verbose_name='性别', max_length=2, choices=GENDER_CHOICE, null=True, blank=True)
-    nation = models.CharField(verbose_name="民族", max_length=32, null=True, blank=True)
+    nation = models.CharField(verbose_name="民族", max_length=10, null=True, blank=True)
     idnum = models.CharField(verbose_name="身份证号", max_length=100, null=True, blank=True)
-    office = models.ForeignKey(Office,
-                               verbose_name="所属科室",
-                               on_delete=models.CASCADE,
-                               )
-    hospital = models.ForeignKey(Hospital,
-                                 verbose_name="所属医院",
-                                 on_delete=models.CASCADE,
-                                 )
+    office = models.ForeignKey(
+        Office,
+        verbose_name="所属科室",
+        on_delete=models.CASCADE,
+    )
+    hospital = models.ForeignKey(
+        Hospital,
+        verbose_name="所属医院",
+        on_delete=models.CASCADE,
+    )
     birthday = models.DateField(verbose_name='出生日期', null=True, blank=True)
     # photo = models.ImageField(verbose_name="医生照片", upload_to="images/doctor", null=True, blank=True)
-    photo = models.CharField(verbose_name="医生照片", max_length=100, default='doctor_photo')
+    photo = models.CharField(verbose_name="医生照片", max_length=10, default='doctor_photo')
     describe = models.TextField(verbose_name="医生描述", null=True, blank=True)
-    created_by = models.CharField(verbose_name="创建人", max_length=100, null=True, blank=True)
-    updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
+    created_by = models.CharField(verbose_name="创建人", max_length=20, null=True, blank=True)
+    updated_by = models.CharField(verbose_name="更新人", max_length=20, null=True, blank=True)
 
     is_online_consult = models.BooleanField(verbose_name="是否互联网接诊", default=True)
 
     class Meta:
         db_table = "bs_doctor"
         verbose_name = "医生表"
         verbose_name_plural = verbose_name
 
 
 class User(AbstractUser):
     name = models.CharField(verbose_name="名称", max_length=255, null=True, blank=True)
-    password = models.CharField(verbose_name="密码", max_length=255, null=True, blank=True)
-    last_login = models.DateField(verbose_name='上次登录时间', null=True, blank=True)
-    is_superuser = models.BooleanField(verbose_name="是否是超管", default=False)
     phone = models.CharField(verbose_name='联系方式', max_length=100, null=True, blank=True)
     birthday = models.DateField(verbose_name='出生日期', null=True, blank=True)
     gender = models.CharField(verbose_name='性别', max_length=2, choices=GENDER_CHOICE, null=True, blank=True)
     idcardnum = models.CharField(verbose_name='身份证号', max_length=100, null=True, blank=True)
     order_by = models.IntegerField(verbose_name='排序', default=1, null=True, blank=True)
-    office = models.ForeignKey(Office,
-                               verbose_name="所属科室",
-                               on_delete=models.CASCADE,
-                               null=True
-                               )
-    hospital = models.ForeignKey(Hospital,
-                                 verbose_name="所属医院",
-                                 on_delete=models.CASCADE,
-                                 null=True
-                                 )
-    user_rank = models.ForeignKey(PositionTitle,
-                                  verbose_name="职称",
-                                  on_delete=models.CASCADE,
-                                  null=True
-                                  )
-    doctor = models.ForeignKey(Doctor,
-                               verbose_name="绑定医生",
-                               on_delete=models.CASCADE,
-                               null=True
-                               )
+    office = models.ForeignKey(
+        Office,
+        verbose_name="所属科室",
+        on_delete=models.CASCADE,
+        null=True
+    )
+    hospital = models.ForeignKey(
+        Hospital,
+        verbose_name="所属医院",
+        on_delete=models.CASCADE,
+        null=True
+    )
+    doctor = models.ForeignKey(
+        Doctor,
+        verbose_name="绑定医生",
+        on_delete=models.CASCADE,
+        null=True
+    )
     # avatar_url = models.ImageField(verbose_name="用户头像", upload_to="images/user", null=True, blank=True)
     avatar_url = models.CharField(verbose_name="用户头像", max_length=100, default='user_avatar')
     default_group_id = models.CharField(verbose_name='默认角色', max_length=255, null=True, blank=True)
     allow_office = models.CharField(verbose_name='可操作科室', max_length=255, null=True, blank=True)
     note = models.TextField(verbose_name="注释说明", null=True, blank=True)
     created_by = models.CharField(verbose_name="创建人", max_length=100, null=True, blank=True)
     updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
     created_time = models.DateTimeField(verbose_name='创建时间', auto_now_add=True, null=True)
     updated_time = models.DateTimeField(verbose_name='更新时间', auto_now=True, null=True)
 
     class Meta:
         # db_table = "bs_user"
-        verbose_name = "用户表"
+        verbose_name = "用户信息"
         # verbose_name_plural = verbose_name
 
     # def __str__(self):
     #     return self.name
 
     @property
     def get_default_group(self):
@@ -208,40 +217,41 @@
 
 
 class ExtraGroup(models.Model):
     """
     角色扩充表
     """
     group = models.OneToOneField(Group, on_delete=models.CASCADE, related_name="extra_group", null=True, blank=True)
+    role_code = models.CharField(max_length=50, verbose_name="角色代码", unique=True)
+    role_name = models.CharField(max_length=50, verbose_name="角色名称")
     is_active = models.BooleanField(default=True, verbose_name='是否启用', null=True)
     note = models.CharField('描述', max_length=50, null=True, blank=True)
     hospital = models.ForeignKey(
         Hospital,
         verbose_name='所属医院',
         on_delete=models.CASCADE,
         related_name='groups',
     )
     order_by = models.IntegerField(verbose_name='排序', default=1, null=True)
-    role_code = models.CharField(max_length=50, verbose_name="角色代码", unique=True)
     created_user = models.CharField(max_length=50, verbose_name="创建人", null=True, blank=True)
     created_at = models.DateTimeField(verbose_name="创建时间", auto_now_add=True, null=True)
     updated_at = models.DateTimeField(verbose_name="最后更新时间", auto_now=True, null=True)
 
     class Meta:
         db_table = 'bs_extra_group'
         verbose_name = "角色"
         verbose_name_plural = verbose_name
 
 
 class ContentTypeCates(models.Model):
     """
     菜单名称
     """
-    name = models.CharField('名称', max_length=20, null=True)
-    is_active = models.BooleanField('是否启用', default=True, null=True)
+    name = models.CharField('名称', max_length=20)
+    is_active = models.BooleanField('是否启用', default=True)
     order_by = models.IntegerField(verbose_name='排序', default=1, null=True)
     level = models.IntegerField(verbose_name="级别", default=1, null=True, blank=True)
     icon_class = models.CharField(verbose_name="图标", max_length=500, null=True, blank=True)
     parent = models.ForeignKey(
         'self',
         verbose_name='父级菜单',
         on_delete=models.CASCADE,
@@ -260,18 +270,26 @@
 
 
 class ContentTypeEx(models.Model):
     """
     功能类别
     """
     name = models.CharField('名称', max_length=20, null=True)
-    content_type = models.ForeignKey(ContentType, verbose_name="系统应用", on_delete=models.CASCADE,
-                                     related_name='extension')
-    content_type_cat = models.ForeignKey('ContentTypeCates', verbose_name='菜单', on_delete=models.CASCADE,
-                                         related_name='content_cates')
+    content_type = models.ForeignKey(
+        ContentType,
+        verbose_name="系统应用",
+        on_delete=models.CASCADE,
+        related_name='extension'
+    )
+    content_type_cat = models.ForeignKey(
+        'ContentTypeCates',
+        verbose_name='菜单',
+        on_delete=models.CASCADE,
+        related_name='content_cates'
+    )
     icon_class = models.CharField(verbose_name="图标", max_length=500, null=True, blank=True)
     front_url = models.TextField(verbose_name='url', null=True, blank=True)
     front_component = models.TextField(verbose_name='组成', null=True, blank=True)
     front_params = models.CharField(verbose_name='参数', max_length=50, null=True)
     front_redirect_url = models.URLField(verbose_name='重定向', null=True)
     is_active = models.BooleanField('是否启用', default=True, null=True)
     order_by = models.IntegerField(verbose_name='排序', default=1, null=True)
@@ -286,15 +304,15 @@
         return self.name
 
 
 class ExpenseStandard(MedicalBaseModel):
     # 挂号费用：1、电话问诊：2、在线问诊：3
     expense_type = models.CharField(verbose_name="费用类型", max_length=100, null=True)
     standard_name = models.CharField(verbose_name="标准名称", max_length=100)
-    standard_code = models.CharField(verbose_name="标准编码", max_length=255, unique=True)
+    standard_code = models.CharField(verbose_name="标准编码", max_length=255)
     fees = models.FloatField(verbose_name="费用", null=True)
     hospital = models.ForeignKey(
         Hospital,
         verbose_name='所属医院',
         on_delete=models.CASCADE,
         null=True
     )
@@ -302,33 +320,70 @@
     updated_by = models.CharField(verbose_name="更新人", max_length=100, null=True, blank=True)
     doctors = models.ManyToManyField(Doctor, verbose_name="医生费用标准", blank=True)
 
     class Meta:
         db_table = 'bs_expense_standard'
         verbose_name = '费用标准表'
         verbose_name_plural = verbose_name
+        unique_together = (
+            ('standard_code', 'hospital',),  # 联合唯一
+        )
+
+
+class InspectionType(MedicalBaseModel):
+    code_srvtp = models.CharField(verbose_name="检查类型编码", max_length=50)
+    name_srvtp = models.CharField(verbose_name="检查类型名称", max_length=50)
+    parent = models.ForeignKey(
+        'self',
+        verbose_name='父级',
+        on_delete=models.CASCADE,
+        related_name='children',
+        null=True
+    )
+
+    class Meta:
+        db_table = 'bs_inspection_type'
+        verbose_name = '检查字典类型'
+        verbose_name_plural = verbose_name
 
 
 class InspectionDictionaries(MedicalBaseModel):
     project_code = models.CharField(max_length=255, verbose_name="项目编码", unique=True)
     project_name = models.CharField(max_length=64, verbose_name="项目名称")
     hospital_code = models.CharField(max_length=128, verbose_name="医院编码")
     office_code = models.CharField(max_length=128, verbose_name="科室编码")
     project_fees = models.FloatField(verbose_name="项目费用", null=True)
     remarks = models.CharField(max_length=128, verbose_name="备注", null=True, blank=True)
     distinguish = models.CharField(max_length=128, verbose_name="区分字段", null=True, blank=True)
-    code_srvtp = models.CharField(verbose_name="检验类型编码", max_length=50, null=True)
-    name_srvtp = models.CharField(verbose_name="检验类型名称", max_length=50, null=True)
+    code_srvtp = models.CharField(verbose_name="检查类型编码", max_length=50, null=True)
+    name_srvtp = models.CharField(verbose_name="检查类型名称", max_length=50, null=True)
 
     class Meta:
         db_table = 'bs_inspection_dictionaries'
         verbose_name = '检查字典'
         verbose_name_plural = verbose_name
 
 
+class ExaminationType(MedicalBaseModel):
+    code_srvtp = models.CharField(verbose_name="检查类型编码", max_length=50)
+    name_srvtp = models.CharField(verbose_name="检查类型名称", max_length=50)
+    parent = models.ForeignKey(
+        'self',
+        verbose_name='父级',
+        on_delete=models.CASCADE,
+        related_name='children',
+        null=True
+    )
+
+    class Meta:
+        db_table = 'bs_examination_type'
+        verbose_name = '检验字典类型'
+        verbose_name_plural = verbose_name
+
+
 class ExaminationDictionaries(MedicalBaseModel):
     project_code = models.CharField(max_length=255, verbose_name="项目编码", unique=True)
     project_name = models.CharField(max_length=64, verbose_name="项目名称")
     hospital_code = models.CharField(max_length=128, verbose_name="医院编码")
     office_code = models.CharField(max_length=128, verbose_name="科室编码")
     project_fees = models.FloatField(verbose_name="项目费用", null=True)
     remarks = models.CharField(max_length=128, verbose_name="备注", null=True, blank=True)
@@ -372,15 +427,15 @@
         verbose_name_plural = verbose_name
 
 
 class DrugDirectory(MedicalBaseModel):
     drug_code = models.CharField(verbose_name="药品编码", max_length=255, unique=True)
     drug_name = models.CharField(max_length=64, verbose_name="药品名称", null=True, blank=True)
     standards = models.CharField(max_length=64, verbose_name="规格", null=True, blank=True)
-    units = models.CharField(max_length=64, verbose_name="单位", null=True, blank=True)  # 盒，袋，瓶
+    total_unit = models.CharField(max_length=64, verbose_name="基本单位", null=True, blank=True)  # 盒，袋，瓶
     total_unit_code = models.CharField(verbose_name="总量单位编码", max_length=20, null=True, blank=True)
     preparation_type = models.ForeignKey(
         DrugPreparationType,
         verbose_name='制剂类型',
         on_delete=models.DO_NOTHING,
     )
     category = models.ForeignKey(
@@ -390,15 +445,15 @@
     )
     drug_type = models.ForeignKey(
         DrugType,
         verbose_name='药品类型',
         on_delete=models.DO_NOTHING,
     )
     unit_dose = models.CharField(verbose_name="单位剂量", max_length=20, null=True, blank=True)
-    measure_unit = models.CharField(verbose_name="计量单位", max_length=20, null=True, blank=True)
+    measure_unit = models.CharField(verbose_name="计量/零售单位", max_length=20, null=True, blank=True)
     measure_unit_code = models.CharField(verbose_name="计量单位编码", max_length=20, null=True, blank=True)
     stock_left = models.CharField(verbose_name="库存数量", max_length=20, null=True, blank=True)
     stock_unit = models.CharField(verbose_name="库存单位", max_length=20, null=True, blank=True)
     mic = models.CharField(verbose_name="医保类别", max_length=20, null=True, blank=True)
     rcc_category = models.CharField(verbose_name="农合类别", max_length=20, null=True, blank=True)
     is_essential = models.BooleanField(verbose_name="是否是基药", default=True)
     hr_level = models.CharField(verbose_name="高危等级", max_length=64, null=True, blank=True)
@@ -437,40 +492,26 @@
     pharmacy_code = models.CharField(verbose_name="药房编码", max_length=255, unique=True)
     pharmacy_name = models.CharField(verbose_name="药房名称", max_length=64, null=True, blank=True)
     pharmacy_type = models.ForeignKey(
         PharmacyType,
         verbose_name='药房类型',
         on_delete=models.DO_NOTHING,
     )
-    # belong_unit = models.CharField(verbose_name="所属单位", max_length=64, null=True, blank=True)
-
     address = models.TextField(verbose_name="药房地址", null=True, blank=True)
-    hospital = models.ForeignKey(Hospital,
-                                 verbose_name="所属医院",
-                                 on_delete=models.CASCADE,
-                                 null=True
-                                 )
-    enterprise = models.ForeignKey(PharmacyEnterprise,
-                                   verbose_name="所属药企",
-                                   on_delete=models.CASCADE,
-                                   null=True
-                                   )
+    hospital = models.ForeignKey(Hospital, verbose_name="所属医院", on_delete=models.CASCADE,null=True)
+    enterprise = models.ForeignKey(PharmacyEnterprise, verbose_name="所属药企", on_delete=models.CASCADE, null=True)
 
     class Meta:
         db_table = 'bs_pharmacy_management'
         verbose_name = '药房管理'
         verbose_name_plural = verbose_name
 
 
 class PharmacyDrug(MedicalBaseModel):
-    pharmacy = models.ForeignKey(PharmacyManagement,
-                                 verbose_name="所属药房",
-                                 on_delete=models.CASCADE,
-                                 null=True
-                                 )
+    pharmacy = models.ForeignKey(PharmacyManagement, verbose_name="所属药房", on_delete=models.CASCADE, null=True)
     drug_code = models.CharField(verbose_name="药品编码", max_length=255, null=True, blank=True)
     drug_name = models.CharField(max_length=64, verbose_name="药品名称", null=True, blank=True)
     standards = models.CharField(max_length=64, verbose_name="规格", null=True, blank=True)
     units = models.CharField(max_length=64, verbose_name="单位", null=True, blank=True)
     preparation_type = models.ForeignKey(
         DrugPreparationType,
         verbose_name='制剂类型',
@@ -482,26 +523,61 @@
         on_delete=models.DO_NOTHING,
     )
     category = models.ForeignKey(
         DrugCategory,
         verbose_name='类别',
         on_delete=models.DO_NOTHING,
     )
-    origin_place = models.CharField(max_length=64, verbose_name="产地", null=True, blank=True)
-    manufacturer = models.CharField(max_length=64, verbose_name="生产厂家", null=True, blank=True)
-    hospital = models.ForeignKey(Hospital,
-                                 verbose_name="所属医院",
-                                 on_delete=models.CASCADE,
-                                 null=True
-                                 )
-    valid_date = models.DateTimeField(verbose_name='有效日期', auto_now=True, null=True)
+    origin_place = models.CharField(max_length=500, verbose_name="产地", null=True, blank=True)
+    manufacturer = models.CharField(max_length=200, verbose_name="生产厂家", null=True, blank=True)
+    hospital = models.ForeignKey(Hospital, verbose_name="所属医院", on_delete=models.CASCADE, null=True)
+    valid_date = models.DateField(verbose_name='有效日期', auto_now=True, null=True)
     inventory_quantity = models.IntegerField(verbose_name='库存数量', default=0, null=True)
     measurement_unit = models.CharField(max_length=64, verbose_name="计量单位", null=True, blank=True)
     cost_unit_price = models.FloatField(verbose_name="成本单价", null=True)
     cost_amount = models.FloatField(verbose_name="成本金额", null=True)
     retail_unit_price = models.FloatField(verbose_name="零售单价", null=True)
     retail_amount = models.FloatField(verbose_name="零售金额", null=True)
 
     class Meta:
         db_table = 'bs_pharmacy_drug'
         verbose_name = '药房-药品'
         verbose_name_plural = verbose_name
+
+
+class ApiInfo(models.Model):
+    org_code = models.CharField(max_length=50, verbose_name="医院编码")
+    req_code = models.CharField(max_length=50, verbose_name="请求编码")
+    req_name = models.CharField(max_length=50, verbose_name="请求名称", null=True, blank=True)
+    req_method = models.CharField(max_length=50, verbose_name="请求方式")
+    content_type = models.CharField(max_length=50, verbose_name="请求数据类型")
+    front_url = models.CharField(max_length=200, verbose_name="请求路由")
+    created_time = models.DateTimeField(verbose_name='创建时间', auto_now_add=True, null=True)
+    updated_time = models.DateTimeField(verbose_name='更新时间', auto_now=True, null=True)
+    is_active = models.BooleanField(verbose_name="是否启用", default=True)
+
+    class Meta:
+        db_table = "bs_api_info"
+        verbose_name = "接口信息"
+        verbose_name_plural = verbose_name
+        unique_together = (
+            ('org_code', 'req_code',),  # 联合唯一
+        )
+
+    def writeback(self, in_data, req_code):
+        api_info_obj = ApiInfo.objects.filter(org_code=in_data['hospital_code'], req_code=req_code).first()
+        if api_info_obj:
+            cms_url = WRITEBACK_IP + api_info_obj.front_url
+            if api_info_obj.req_method == "POST":
+                res = requests.post(url=cms_url, json=in_data)
+            elif api_info_obj.req_method == "GET":
+                res = requests.get(url=cms_url, params=in_data)
+            elif api_info_obj.req_method == "PUT":
+                res = requests.put(url=cms_url, data=in_data)
+            elif api_info_obj.req_method == "DELETE":
+                res = requests.delete(url=cms_url)
+            else:
+                res = requests.patch(url=cms_url)
+            res_json = json.loads(res.text)
+        else:
+            res_json = {"success": False, "code": 2001, "message": "不存在对接医院信息！", "data": {}}
+        return res_json
```

### Comparing `base_system-0.1.0/base_system/urls.py` & `base_system-0.1.2/base_system/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Infrastructure URL Configuration
+"""MedicalSystem URL Configuration
 
 The `urlpatterns` list routes URLs to views. For more information please see:
     https://docs.djangoproject.com/en/4.1/topics/http/urls/
 Examples:
 Function views
     1. Add an import:  from my_app import views
     2. Add a URL to urlpatterns:  path('', views.home, name='home')
@@ -15,49 +15,56 @@
 """
 from django.contrib import admin
 from django.urls import path, include
 from rest_framework import routers
 
 from . import views
 from base_system.views import PermissionsView
-from base_system.viewset import group_viewset, permission_viewset, appointment_viewset
+from base_system import viewsets
 from rest_framework_jwt.views import obtain_jwt_token
 from rest_framework_jwt.views import refresh_jwt_token
 from rest_framework_jwt.views import verify_jwt_token
 
 urlpatterns = [
     # path('login/',views.login),
     path('register/', views.register),
     path('login/', obtain_jwt_token),  # 登录
     path('token/refresh/', refresh_jwt_token),
     path('verify/', verify_jwt_token),
     path('permissions/', PermissionsView.as_view(), name='permissions'),
     path('change-password/', views.change_password),
-    path('all-permissions/', group_viewset.all_permissions),  # 获取系统所有权限
-    path('own-menu/', group_viewset.get_own_permissions),  # 获取系统所有权限
+    path('all-permissions/', viewsets.all_permissions),  # 获取系统所有权限
+    path('own-menu/', viewsets.get_own_permissions),  # 获取系统所有权限
     path('import_position_title/', views.import_position_title),  # 职称信息导入接口
     path('import_office/', views.import_office),  # 科室信息导入接口
     path('import_doctor/', views.import_doctor),  # 医生信息导入接口
-    path('menu_permissions/', permission_viewset.menu_permissions),
+    path('import_ins_dic/', views.import_inspection_dictionaries),  # 导入检查字典excel表数据
+    path('import_exa_dic/', views.import_examination_dictionaries),  # 导入检验字典excel表数据
+    path('import_drug_dir/', views.import_drug_directory),  # 导入药品目录excel表数据
+    path('import_pharmacy_drug/', views.import_pharmacy_drug),  # 导入药房药品excel表数据
+    path('menu_permissions/', viewsets.menu_permissions),
+
 ]
 router = routers.DefaultRouter()
 router.register(r'export_hospital', views.HospitalInfoExportViewSet)  # 医院信息导出接口
 router.register(r'export_office', views.OfficeInfoExportViewSet)  # 科室信息导出接口
 router.register(r'export_group', views.GroupExportViewSet)  # 角色信息导出接口
 router.register(r'export_doctor', views.DoctorInfoExportViewSet)  # 医生信息导出接口
 router.register(r'export_user', views.UserInfoExportViewSet)  # 用户信息导出接口
-router.register(r'groups', group_viewset.GroupViewSet)  # 角色
+router.register(r'groups', viewsets.GroupViewSet)  # 角色
 router.register(r'users', views.UserViewSet)  # 用户信息
 router.register(r'ins_dic', views.InspectionDictionariesViewSet)  # 检查字典
 router.register(r'export_ins_dic', views.InspectionDictionariesInfoExportViewSet)  # 导出检查字典
 router.register(r'exa_dic', views.ExaminationDictionariesViewSet)  # 检验字典
 router.register(r'export_exa_dic', views.ExaminationDictionariesInfoExportViewSet)  # 导出检验字典
 router.register(r'export_drug_directory', views.DrugDirectoryExportViewSet)  # 导出药品目录
+router.register(r'export_pharmacy_drug', views.PharmacyDrugExportViewSet)  # 导出药房药品目录
 router.register(r'pharmacy_management', views.PharmacyManagementViewSet)  # 药房管理
 router.register(r'drug_directories', views.DrugDirectoryViewSet)  # 药品目录
+router.register(r'apinfos', views.ApiInfoViewSet)  # 接口信息
 
 # 预约相关
-router.register(r'hospitals', appointment_viewset.HospitalViewSet)
-router.register(r'offices', appointment_viewset.OfficeViewSet)
-router.register(r'doctors', appointment_viewset.DoctorViewSet)
+router.register(r'hospitals', viewsets.HospitalViewSet)
+router.register(r'offices', viewsets.OfficeViewSet)
+router.register(r'doctors', viewsets.DoctorViewSet)
 
 urlpatterns += router.urls
```

### Comparing `base_system-0.1.0/base_system/viewset/group_viewset.py` & `base_system-0.1.2/base_system/viewsets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,257 +1,370 @@
-from django.contrib.auth.models import Group, Permission
-from django.contrib.contenttypes.models import ContentType
-from django.http import JsonResponse
-from rest_framework.exceptions import ValidationError
-from rest_framework.viewsets import ModelViewSet
-from rest_framework.decorators import action
-from rest_framework.response import Response
-from rest_framework import status
-
-from base_system.models import ExtraGroup, ContentTypeCates, ContentTypeEx, User, Hospital
-from base_system.serializers_folder.group_serializers import GroupSerializer, ExtraGroupSerializer, ContentTypeCateSerializer, \
-    ContentTypeExSerializer, MenuSerializer
-
-
-class GroupViewSet(ModelViewSet):
-    queryset = Group.objects.all()
-    serializer_class = GroupSerializer
-    filter_fields = "__all__"
-    # filterset_class = UserfFilter
-
-    def get_parent(self, li, rels):
-        if rels.parent:
-            li.append(rels.parent)
-            self.get_parent(li, rels.parent)
-        return li
-
-    @action(methods=["GET"], detail=True)
-    def get_group_permission(self, request, pk):
-        obj = self.get_object()
-        # 获取当前组所拥有的权限
-        permissions = Permission.objects.filter(group=obj.id).all().order_by('content_type_id')
-        # serializer = PermissionSerializer(permissions, many=True)
-        # return Response(data=serializer.data, status=status.HTTP_200_OK)
-        data = self.serializer_permission(permissions)
-        return Response(data=data, status=status.HTTP_200_OK)
-
-    @action(methods=["GET"], detail=False)
-    def get_all_permission(self, request):
-        # 获取所有的权限
-        permissions = Permission.objects.all().order_by('content_type_id')
-        # serializer = PermissionSerializer(permissions, many=True)
-        # return Response(data=serializer.data, status=status.HTTP_200_OK)
-        data = self.serializer_permission(permissions)
-        return Response(data=data, status=status.HTTP_200_OK)
-
-    @action(methods=["GET"], detail=False)
-    def get_ct_permission(self, request):
-        # 获取当前组所拥有的权限
-        ctrels = ContentTypeEx.objects.all().order_by('content_type_id')
-
-        ret = map(
-            lambda ctrel: {
-                "id": ctrel.id,
-                "name": ctrel.name,
-                "permissions": map(
-                    lambda p: {
-                        "id": p.id,
-                        "name": p.name,
-                        "codename": p.codename
-                    },
-                    ctrel.content_type.permission_set.all()
-                )
-            },
-            ctrels
-        )
-
-        # serializer = PermissionSerializer(permissions, many=True)
-        # return Response(data=serializer.data, status=status.HTTP_200_OK)
-
-        # data = self.serializer_permission(permissions)
-        return Response(data=ret, status=status.HTTP_200_OK)
-
-    def serializer_permission(self, permissions):
-        # 通过权限来得到权限的分类及权限的序列化信息
-        permissions = set(permissions)
-        content_types = map(lambda p: p.content_type, permissions)
-        content_types = list(set(content_types))  # 得到去重的列表
-        return map(
-            lambda ct: {
-                "id": ct.id,
-                "name": ct.model,
-                "permissions": map(
-                    lambda p: {"id": p.id, "name": p.name, "codename": p.codename},
-                    set(ct.permission_set.all()) & permissions
-                )
-            },
-            content_types
-        )
-
-    # def retrieve(self, request, *args, **kwargs):
-    #     # 获取单个角色的基本信息，该角色的权限，以及所有的权限
-    #     obj = self.get_object()
-    #     serializer = self.get_serializer(obj)
-    #     # 基本的角色信息
-    #     data = serializer.data
-    #     # 该角色所拥有的权限
-    #     permissions = Permission.objects.filter(group=obj.id).all().order_by('content_type_id')
-    #     # serializer = PermissionSerializer(permissions, many=True)
-    #     # data["permissions"] = serializer.data
-    #     data["self_permissions"] = self.serializer_permission(permissions)
-    #     # 所有的权限提供给修改使用
-    #     total_permissions = Permission.objects.all().order_by('content_type_id')
-    #     # serializer = PermissionSerializer(total_permissions, many=True)
-    #     # data["total_permissions"] = serializer.data
-    #     data["total_permissions"] = self.serializer_permission(total_permissions)
-    #     return Response(data=data, status=status.HTTP_200_OK)
-
-    def create(self, request, *args, **kwargs):
-        extra, group_data = self.check_data(request.data)
-        # 创建角色及相关及权限
-        new_group = Group.objects.filter(name=group_data["name"])
-        if new_group:
-            return Response(data={"msg": "角色已经存在"}, status=210)
-        group = Group.objects.create(name=group_data["name"])
-        group.permissions.set(group_data["permission_ids"])
-        group.save()
-        # 创建用户附加信息
-        # extra = ExtraGroup.objects.create(group_id=group.pk, **extra)
-        extra['group']=group.pk
-
-        serializer = ExtraGroupSerializer(data=extra)
-        serializer.is_valid(raise_exception=True)
-        serializer.save()
-        return Response(data=GroupSerializer(group).data, status=status.HTTP_201_CREATED)
-
-    def check_data(self, data):
-        # 校验角色额外信息数据
-        extra = dict()
-        # data = dict(data)
-        extra["note"] = data.get("note")
-        extra["is_active"] = data.get("is_active", 1)
-        extra["hospital"] = data.get("hospital_id")
-        extra["order_by"] = data.get("order_by")
-        extra["created_user"] = data.get("created_user")
-        extra["role_code"] = data.get("role_code")
-        serializer = ExtraGroupSerializer(data=extra)
-        serializer.is_valid(raise_exception=True)
-        extra = serializer.data
-
-        # 校验角色数据
-        group_data = dict()
-        permissions = data.get("permission_ids")
-        # group_data["permission_ids"] = eval(permissions) if permissions else None
-        group_data["permission_ids"] = permissions if permissions else []
-        if data.get("name"):
-            group_data["name"] = data.get("name")
-            serializer = GroupSerializer(data=group_data)
-            serializer.is_valid(raise_exception=True)
-            # group_data = serializer.data
-
-        return extra, group_data
-
-    def update(self, request, *args, **kwargs):
-        group = self.get_object()
-        extra_group = group.extra_group
-        if request.data.get("name") == group.name:
-            del request.data["name"]
-        extra, group_data = self.check_data(request.data)
-        extra_group.note = extra["note"]
-        extra_group.is_active = extra["is_active"]
-        extra_group.index = extra["order_by"]
-        extra_group.hospital_id = extra["hospital"]
-        extra_group.created_user = extra["created_user"]
-        extra_group.role_code = extra["role_code"]
-        extra_group.save()
-        group.name = group_data.get('name', group.name)
-        # if group_data.get("permission_ids"):
-        group.permissions.set(group_data["permission_ids"])
-        group.save()
-        return Response(data=GroupSerializer(group).data, status=status.HTTP_205_RESET_CONTENT)
-
-    # def destroy(self, request, *args, **kwargs):
-    #     group = self.get_object()
-    #     group.extra_group.is_active = 0
-    #     group.extra_group.save()
-    #     return Response(data={"message": "删除成功"}, status=status.HTTP_204_NO_CONTENT)
-
-
-class ExtraGroupViewSet(ModelViewSet):
-    queryset = ExtraGroup.objects.all()
-    serializer_class = ExtraGroupSerializer
-    filter_fields = "__all__"
-
-
-class ContentTypeCatesViewSet(ModelViewSet):
-    queryset = ContentTypeCates.objects.all()
-    serializer_class = ContentTypeCateSerializer
-    pagination_class = None
-    filter_fields = "__all__"
-
-
-class ContentTypeExViewSet(ModelViewSet):
-    queryset = ContentTypeEx.objects.all()
-    serializer_class = ContentTypeExSerializer
-    filter_fields = "__all__"
-
-
-def get_parent(li, rels):
-    if rels.parent:
-        if rels.parent not in li:
-            li.append(rels.parent)
-            get_parent(li, rels.parent)
-    return li
-
-
-def get_permissions(serializer,permissions,value):
-    content_type_ids = list(map(lambda perm: perm.content_type_id, permissions))
-    content_types = ContentType.objects.filter(id__in=content_type_ids).distinct().all()
-    content_type_ex = ContentTypeEx.objects.filter(is_active=True,content_type_id__in=content_type_ids)
-    content_type_cat_ids = list(map(lambda cat: cat.content_type_cat_id, content_type_ex))
-    # print(content_type_cat_ids)
-    content_type_cats = ContentTypeCates.objects.filter(id__in=content_type_cat_ids).order_by('order_by')
-    rel_list = []
-    for rel in content_type_cats:
-        get_parent(rel_list, rel)
-    rel_list += content_type_cats
-    rel_list = list(set(rel_list))
-    serializer_rels = serializer(rel_list, many=True)
-    all_menu = serializer_rels.data
-    menu_list = [menu for menu in all_menu if not menu['parent']]
-    # for menu in all_menu:
-    #     if not menu['parent']:
-    #         menu_list.append(menu)
-    for menu_1 in all_menu:
-        children_list = [children for children in all_menu if children['parent'] == menu_1['id']]
-        # for children in all_menu:
-        #     if children['parent'] == menu_1['id']:
-        #         children_list.append(children)
-        children_list = sorted(children_list, key=lambda x: x['order_by'])
-        menu_1['children'] = children_list
-        content_type_ex = ContentTypeEx.objects.filter(content_type_cat_id=menu_1['id']).first()
-        if value:
-            if content_type_ex:
-                menu_1["permissions"] = list(map(lambda p: {"id": p.id, "name": p.name, "codename": p.codename},
-                                                 content_type_ex.content_type.permission_set.all()))
-    menu_list = sorted(menu_list, key=lambda x: x['order_by'])
-    return menu_list
-
-def get_own_permissions(request):
-    user_id=request.GET.get('user_id')
-    user=User.objects.get(id=request.GET.get('user_id'))
-    # defaultgroup = user.get_default_group
-    # print(defaultgroup)
-    # permissions = Permission.objects.filter(group=defaultgroup)
-
-    allgroups = user.get_allgroups
-    permissions = Permission.objects.filter(group__in=allgroups).distinct()
-    serializer = MenuSerializer
-    menu_list = get_permissions(serializer,permissions, 0)
-    return JsonResponse({"data": menu_list})
-
-
-def all_permissions(request):
-    permissions = Permission.objects.all()
-    serializer = MenuSerializer
-    menu_list=get_permissions(serializer,permissions,1)
-    return JsonResponse({"data": menu_list})
+import datetime
+
+from rest_framework.response import Response
+from rest_framework.viewsets import ModelViewSet
+import django_filters as filters
+from base_system.models import Hospital, Office, Doctor
+
+
+from django.contrib.auth.models import Group, Permission
+from django.http import JsonResponse
+from rest_framework.exceptions import ValidationError
+from rest_framework.decorators import action
+from rest_framework import status
+
+from base_system.models import ExtraGroup, ContentTypeCates, ContentTypeEx, User, Hospital
+from base_system.serializers import GroupSerializer, ExtraGroupSerializer, ContentTypeCateSerializer, \
+    ContentTypeExSerializer, MenuSerializer, HospitalSerializer, OfficeSerializer, DoctorSerializer
+from django.db import transaction
+
+
+class GroupViewSet(ModelViewSet):
+    queryset = Group.objects.all()
+    serializer_class = GroupSerializer
+    filter_fields = "__all__"
+    # filterset_class = UserfFilter
+
+    def get_parent(self, li, rels):
+        if rels.parent:
+            li.append(rels.parent)
+            self.get_parent(li, rels.parent)
+        return li
+
+    @action(methods=["GET"], detail=True)
+    def get_group_permission(self, request, pk):
+        obj = self.get_object()
+        # 获取当前组所拥有的权限
+        permissions = Permission.objects.filter(group=obj.id).all().order_by('content_type_id')
+        # serializer = PermissionSerializer(permissions, many=True)
+        # return Response(data=serializer.data, status=status.HTTP_200_OK)
+        data = self.serializer_permission(permissions)
+        return Response(data=data, status=status.HTTP_200_OK)
+
+    @action(methods=["GET"], detail=False)
+    def get_all_permission(self, request):
+        # 获取所有的权限
+        permissions = Permission.objects.all().order_by('content_type_id')
+        # serializer = PermissionSerializer(permissions, many=True)
+        # return Response(data=serializer.data, status=status.HTTP_200_OK)
+        data = self.serializer_permission(permissions)
+        return Response(data=data, status=status.HTTP_200_OK)
+
+    @action(methods=["GET"], detail=False)
+    def get_ct_permission(self, request):
+        # 获取当前组所拥有的权限
+        ctrels = ContentTypeEx.objects.all().order_by('content_type_id')
+
+        ret = map(
+            lambda ctrel: {
+                "id": ctrel.id,
+                "name": ctrel.name,
+                "permissions": map(
+                    lambda p: {
+                        "id": p.id,
+                        "name": p.name,
+                        "codename": p.codename
+                    },
+                    ctrel.content_type.permission_set.all()
+                )
+            },
+            ctrels
+        )
+
+        # serializer = PermissionSerializer(permissions, many=True)
+        # return Response(data=serializer.data, status=status.HTTP_200_OK)
+
+        # data = self.serializer_permission(permissions)
+        return Response(data=ret, status=status.HTTP_200_OK)
+
+    def serializer_permission(self, permissions):
+        # 通过权限来得到权限的分类及权限的序列化信息
+        permissions = set(permissions)
+        content_types = map(lambda p: p.content_type, permissions)
+        content_types = list(set(content_types))  # 得到去重的列表
+        return map(
+            lambda ct: {
+                "id": ct.id,
+                "name": ct.model,
+                "permissions": map(
+                    lambda p: {"id": p.id, "name": p.name, "codename": p.codename},
+                    set(ct.permission_set.all()) & permissions
+                )
+            },
+            content_types
+        )
+
+    # def retrieve(self, request, *args, **kwargs):
+    #     # 获取单个角色的基本信息，该角色的权限，以及所有的权限
+    #     obj = self.get_object()
+    #     serializer = self.get_serializer(obj)
+    #     # 基本的角色信息
+    #     data = serializer.data
+    #     # 该角色所拥有的权限
+    #     permissions = Permission.objects.filter(group=obj.id).all().order_by('content_type_id')
+    #     # serializer = PermissionSerializer(permissions, many=True)
+    #     # data["permissions"] = serializer.data
+    #     data["self_permissions"] = self.serializer_permission(permissions)
+    #     # 所有的权限提供给修改使用
+    #     total_permissions = Permission.objects.all().order_by('content_type_id')
+    #     # serializer = PermissionSerializer(total_permissions, many=True)
+    #     # data["total_permissions"] = serializer.data
+    #     data["total_permissions"] = self.serializer_permission(total_permissions)
+    #     return Response(data=data, status=status.HTTP_200_OK)
+    @transaction.atomic
+    def create(self, request, *args, **kwargs):
+        msec_str = datetime.datetime.now().strftime('%f')
+        extra, group_data = self.check_data(request.data)
+        # 创建角色及相关及权限
+        new_group = Group.objects.filter(name=msec_str+group_data["name"])
+        if new_group:
+            return Response(data={"msg": "角色已经存在"}, status=210)
+        group = Group.objects.create(name=group_data["name"])
+        group.permissions.set(group_data["permission_ids"])
+        group.save()
+        # 创建用户附加信息
+        # extra = ExtraGroup.objects.create(group_id=group.pk, **extra)
+        extra['group']=group.pk
+
+        serializer = ExtraGroupSerializer(data=extra)
+        serializer.is_valid(raise_exception=True)
+        serializer.save()
+        return Response(data=GroupSerializer(group).data, status=status.HTTP_201_CREATED)
+
+    def check_data(self, data):
+        # 校验角色额外信息数据
+        extra = dict()
+        # data = dict(data)
+        extra["note"] = data.get("note")
+        extra["is_active"] = data.get("is_active", 1)
+        extra["hospital"] = data.get("hospital_id")
+        extra["order_by"] = data.get("order_by")
+        extra["created_user"] = data.get("created_user")
+        extra["role_code"] = data.get("role_code")
+        extra["role_name"] = data.get("role_name")
+        serializer = ExtraGroupSerializer(data=extra)
+        serializer.is_valid(raise_exception=True)
+        extra = serializer.data
+
+        # 校验角色数据
+        group_data = dict()
+        permissions = data.get("permission_ids")
+        # group_data["permission_ids"] = eval(permissions) if permissions else None
+        group_data["permission_ids"] = permissions if permissions else []
+        if data.get("name"):
+            group_data["name"] = data.get("name")
+            serializer = GroupSerializer(data=group_data)
+            serializer.is_valid(raise_exception=True)
+            # group_data = serializer.data
+
+        return extra, group_data
+
+    @transaction.atomic
+    def update(self, request, *args, **kwargs):
+        group = self.get_object()
+        extra_group = group.extra_group
+        if request.data.get("name") == group.name:
+            del request.data["name"]
+        extra, group_data = self.check_data(request.data)
+        extra_group.note = extra["note"]
+        extra_group.is_active = extra["is_active"]
+        extra_group.index = extra["order_by"]
+        extra_group.hospital_id = extra["hospital"]
+        extra_group.created_user = extra["created_user"]
+        extra_group.role_code = extra["role_code"]
+        extra_group.role_name = extra["role_name"]
+        extra_group.save()
+        group.name = group_data.get('name', group.name)
+        # if group_data.get("permission_ids"):
+        group.permissions.set(group_data["permission_ids"])
+        group.save()
+        return Response(data=GroupSerializer(group).data, status=status.HTTP_205_RESET_CONTENT)
+
+    # def destroy(self, request, *args, **kwargs):
+    #     group = self.get_object()
+    #     group.extra_group.is_active = 0
+    #     group.extra_group.save()
+    #     return Response(data={"message": "删除成功"}, status=status.HTTP_204_NO_CONTENT)
+
+
+class ExtraGroupViewSet(ModelViewSet):
+    queryset = ExtraGroup.objects.all()
+    serializer_class = ExtraGroupSerializer
+    filter_fields = "__all__"
+
+
+class ContentTypeCatesViewSet(ModelViewSet):
+    queryset = ContentTypeCates.objects.all()
+    serializer_class = ContentTypeCateSerializer
+    pagination_class = None
+    filter_fields = "__all__"
+
+
+class ContentTypeExViewSet(ModelViewSet):
+    queryset = ContentTypeEx.objects.all()
+    serializer_class = ContentTypeExSerializer
+    filter_fields = "__all__"
+
+
+def get_own_permissions(request):
+    user_id=request.GET.get('user_id')
+    user=User.objects.get(id=request.GET.get('user_id'))
+    # defaultgroup = user.get_default_group
+    # print(defaultgroup)
+    # permissions = Permission.objects.filter(group=defaultgroup)
+
+    allgroups = user.get_allgroups
+    permissions = Permission.objects.filter(group__in=allgroups).distinct()
+    serializer = MenuSerializer
+    menu_list = get_permissions(serializer,permissions, 0)
+    return JsonResponse({"data": menu_list})
+
+
+def all_permissions(request):
+    permissions = Permission.objects.all()
+    serializer = MenuSerializer
+    menu_list=get_permissions(serializer,permissions,1)
+    return JsonResponse({"data": menu_list})
+
+
+class MenuViewSet(ModelViewSet):
+    queryset = ContentTypeCates.objects.filter(is_active=True, parent=None)
+    serializer_class = MenuSerializer
+    pagination_class = None
+    filter_fields = "__all__"
+
+
+def get_permissions(serializer,permissions,value):
+    content_type_ids = list(map(lambda perm: perm.content_type_id, permissions))
+    content_type_ex = ContentTypeEx.objects.filter(is_active=True,content_type_id__in=content_type_ids)
+    content_type_cat_ids = list(map(lambda cat: cat.content_type_cat_id, content_type_ex))
+    content_type_cats = ContentTypeCates.objects.filter(id__in=content_type_cat_ids).order_by('order_by')
+    rel_list = []
+    for rel in content_type_cats:
+        get_parent(rel_list, rel)
+    rel_list += content_type_cats
+    rel_list = list(set(rel_list))
+    serializer_rels = serializer(rel_list, many=True)
+    all_menu = serializer_rels.data
+
+    menu_list = [menu for menu in all_menu if not menu['parent']]
+    for menu_1 in all_menu:
+        children_list = [children for children in all_menu if children['parent'] == int(menu_1['id'].replace('n',''))]
+        children_list = sorted(children_list, key=lambda x: x['order_by'])
+        menu_1['children'] = children_list
+        content_type_ex = ContentTypeEx.objects.filter(content_type_cat_id=int(menu_1['id'].replace('n',''))).first()
+        if value:
+            if content_type_ex and children_list ==[]:
+                menu_1["children"] = list(map(lambda p: {"id": p.id, "name": p.name, "codename": p.codename},
+                                                 content_type_ex.content_type.permission_set.all()))
+    menu_list = sorted(menu_list, key=lambda x: x['order_by'])
+    return menu_list
+
+
+def menu_permissions(request):
+    permissions = Permission.objects.all()
+    serializer = MenuSerializer
+    menu_list = get_permissions(serializer, permissions, 1)
+    return JsonResponse({"data": menu_list})
+
+
+def get_parent(li, rels):
+    if rels.parent:
+        if rels.parent not in li:
+            li.append(rels.parent)
+            get_parent(li, rels.parent)
+    return li
+
+
+class HospitalFilter(filters.FilterSet):
+    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
+    codenum = filters.CharFilter(field_name="codenum", lookup_expr='icontains')
+    parent = filters.CharFilter(field_name="parent")
+
+    class Meta:
+        model = Hospital
+        fields = (
+            "name",
+            "codenum",
+            "parent",
+        )
+
+
+class HospitalViewSet(ModelViewSet):
+    queryset = Hospital.objects.filter(is_active=True).order_by('id')
+    serializer_class = HospitalSerializer
+    filterset_class = HospitalFilter
+    # filter_fields = "__all__"
+
+
+class OfficeFilter(filters.FilterSet):
+    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
+    codenum = filters.CharFilter(field_name="codenum", lookup_expr='icontains')
+    office_type = filters.CharFilter(field_name="office_type", lookup_expr='icontains')
+    hospital = filters.CharFilter(field_name="hospital")
+    parent = filters.CharFilter(field_name="parent")
+
+    class Meta:
+        model = Office
+        fields = "__all__"
+        search_fields = ('name', 'codenum', 'office_type')  # 允许模糊查询的字段
+
+
+class OfficeViewSet(ModelViewSet):
+    queryset = Office.objects.filter(is_active=True)
+    serializer_class = OfficeSerializer
+    # filter_fields = "__all__"
+    filterset_class = OfficeFilter
+
+    def list(self, request, *args, **kwargs):
+        queryset = self.filter_queryset(self.get_queryset())
+        # page = None
+        if 'page' in self.request.query_params.keys():
+            page = self.paginate_queryset(queryset)
+            # if page is not None:
+            serializer = self.get_serializer(page, many=True)
+            return self.get_paginated_response(serializer.data)
+
+        serializer = self.get_serializer(queryset, many=True)
+        return Response({'results': serializer.data})
+
+
+class DoctorFilter(filters.FilterSet):
+    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
+    job_number = filters.CharFilter(field_name="job_number", lookup_expr='icontains')
+    phone = filters.CharFilter(field_name="phone", lookup_expr='icontains')
+
+    class Meta:
+        model = Doctor
+        fields = "__all__"
+        search_fields = ('name', 'job_number', 'phone')  # 允许模糊查询的字段
+
+
+class DoctorViewSet(ModelViewSet):
+    queryset = Doctor.objects.filter(is_active=True)
+    serializer_class = DoctorSerializer
+    filterset_class = DoctorFilter
+
+    def list(self, request, *args, **kwargs):
+        queryset = self.filter_queryset(self.get_queryset())
+        page = None
+        if 'page' in self.request.query_params.keys():
+            page = self.paginate_queryset(queryset)
+        if page is not None:
+            serializer = self.get_serializer(page, many=True)
+            return self.get_paginated_response(serializer.data)
+        if 'fee_type' in self.request.query_params.keys():
+            fee_type = self.request.query_params.get('fee_type')
+            serializer = self.get_serializer(queryset, many=True, context={'fee_type': fee_type})
+            return Response({'results': serializer.data})
+
+        serializer = self.get_serializer(queryset, many=True)
+        return Response({'results': serializer.data})
+
+    def retrieve(self, request, *args, **kwargs):
+        instance = self.get_object()
+        if 'fee_type' in self.request.query_params.keys():
+            fee_type = self.request.query_params.get('fee_type')
+            serializer = self.get_serializer(instance, context={'fee_type': fee_type})
+            return Response(serializer.data)
+        serializer = self.get_serializer(instance)
+        return Response(serializer.data)
```

### Comparing `base_system-0.1.0/base_system.egg-info/PKG-INFO` & `base_system-0.1.2/base_system.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.1.0
-Summary: Medical system base data
+Version: 0.1.2
+Summary: Basic feature component
 Home-page: https://devcloud.huaweicloud.com/
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `base_system-0.1.0/init_data.json` & `base_system-0.1.2/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.1.0/manage.py` & `base_system-0.1.2/manage.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'Infrastructure.settings')
+    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'BaseFunctionModule.settings')
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `base_system-0.1.0/requirements.txt` & `base_system-0.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.0/runtests.py` & `base_system-0.1.2/runtests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import django
 from django.conf import settings
 from django.test.utils import get_runner
 
-os.environ['DJANGO_SETTINGS_MODULE'] = 'Infrastructure.settings'
+os.environ['DJANGO_SETTINGS_MODULE'] = 'BaseFunctionModule.settings'
 test_dir = os.path.join(os.path.dirname(__file__), 'base_system')
 sys.path.insert(0, test_dir)
 
 
 
 def runtests():
     TestRunner = get_runner(settings)
```

### Comparing `base_system-0.1.0/setup.py` & `base_system-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.1.0',
-    description="Medical system base data",
+    version='0.1.2',
+    description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://devcloud.huaweicloud.com/",
     include_package_data=True,
```

