# Comparing `tmp/netkiller-devops-0.6.8.tar.gz` & `tmp/netkiller-devops-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netkiller-devops-0.6.8.tar", last modified: Wed Feb  8 05:08:41 2023, max compression
+gzip compressed data, was "netkiller-devops-0.6.9.tar", last modified: Wed Mar  8 14:13:26 2023, max compression
```

## Comparing `netkiller-devops-0.6.8.tar` & `netkiller-devops-0.6.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.503721 netkiller-devops-0.6.8/
--rw-r--r--   0 neo        (501) staff       (20)     1081 2021-04-12 02:34:54.000000 netkiller-devops-0.6.8/LICENSE
--rw-r--r--   0 neo        (501) staff       (20)       13 2021-10-09 03:00:15.000000 netkiller-devops-0.6.8/MANIFEST.in
--rw-r--r--   0 neo        (501) staff       (20)     1746 2023-02-08 05:08:41.503399 netkiller-devops-0.6.8/PKG-INFO
--rw-r--r--   0 neo        (501) staff       (20)     1230 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/README.md
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.488916 netkiller-devops-0.6.8/bin/
--rwxr-xr-x   0 neo        (501) staff       (20)     8175 2021-05-06 06:45:40.000000 netkiller-devops-0.6.8/bin/backup
--rw-r--r--   0 neo        (501) staff       (20)      512 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/bin/chpasswd.sh
--rw-r--r--   0 neo        (501) staff       (20)    18040 2021-04-29 03:46:42.000000 netkiller-devops-0.6.8/bin/deployment
--rw-r--r--   0 neo        (501) staff       (20)     2392 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/dingtalk
--rw-r--r--   0 neo        (501) staff       (20)     1939 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/bin/gitsync
--rw-r--r--   0 neo        (501) staff       (20)     4071 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/logviewer
--rw-r--r--   0 neo        (501) staff       (20)     4223 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/logviewer.docker
--rw-r--r--   0 neo        (501) staff       (20)     5389 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/logviewer.kubectl
--rw-r--r--   0 neo        (501) staff       (20)     3095 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/lrsync
--rw-r--r--   0 neo        (501) staff       (20)       65 2022-09-01 10:12:24.000000 netkiller-devops-0.6.8/bin/matrixpasswd
--rwxr-xr-x   0 neo        (501) staff       (20)     7481 2022-01-09 13:02:59.000000 netkiller-devops-0.6.8/bin/mdump
--rwxr-xr-x   0 neo        (501) staff       (20)     8812 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/merge
--rw-r--r--   0 neo        (501) staff       (20)     5117 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/bin/mysqlshell
--rw-r--r--   0 neo        (501) staff       (20)     9467 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/bin/osconf
--rw-r--r--   0 neo        (501) staff       (20)       53 2022-09-01 10:12:24.000000 netkiller-devops-0.6.8/bin/randpasswd
--rw-r--r--   0 neo        (501) staff       (20)       66 2022-09-01 10:12:24.000000 netkiller-devops-0.6.8/bin/randtext
--rwxr-xr-x   0 neo        (501) staff       (20)     7552 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/sqldump
--rwxr-xr-x   0 neo        (501) staff       (20)     3942 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/voice
--rwxr-xr-x   0 neo        (501) staff       (20)     2262 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/bin/wechat
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.489731 netkiller-devops-0.6.8/doc/
--rw-r--r--   0 neo        (501) staff       (20)     1130 2021-09-28 09:40:58.000000 netkiller-devops-0.6.8/doc/voice.md
--rw-r--r--   0 neo        (501) staff       (20)      964 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/doc/wechat.md
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.493821 netkiller-devops-0.6.8/etc/
--rw-r--r--   0 neo        (501) staff       (20)      336 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/etc/deployment.cfg
--rw-r--r--   0 neo        (501) staff       (20)      398 2021-10-21 09:04:52.000000 netkiller-devops-0.6.8/etc/dump.ini
--rw-r--r--   0 neo        (501) staff       (20)      551 2021-10-22 02:44:34.000000 netkiller-devops-0.6.8/etc/dump.ini.sample
--rw-r--r--   0 neo        (501) staff       (20)      200 2022-11-10 02:00:07.000000 netkiller-devops-0.6.8/etc/logviewer.ini
--rw-r--r--   0 neo        (501) staff       (20)      488 2022-01-09 13:02:59.000000 netkiller-devops-0.6.8/etc/mongo.ini.sample
--rw-r--r--   0 neo        (501) staff       (20)       87 2021-09-28 08:36:03.000000 netkiller-devops-0.6.8/etc/notification.ini
--rw-r--r--   0 neo        (501) staff       (20)      218 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/etc/os.ini
--rw-r--r--   0 neo        (501) staff       (20)      125 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/etc/schedule.cfg
--rw-r--r--   0 neo        (501) staff       (20)     1117 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/etc/task.cfg
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.499064 netkiller-devops-0.6.8/netkiller/
--rw-r--r--   0 neo        (501) staff       (20)       71 2021-09-06 10:55:06.000000 netkiller-devops-0.6.8/netkiller/__init__.py
--rw-r--r--   0 neo        (501) staff       (20)    30819 2022-08-14 15:04:31.000000 netkiller-devops-0.6.8/netkiller/docker.py
--rw-r--r--   0 neo        (501) staff       (20)     5116 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/netkiller/git.py
--rw-r--r--   0 neo        (501) staff       (20)     5432 2022-01-09 13:02:59.000000 netkiller-devops-0.6.8/netkiller/gitlab.py
--rw-r--r--   0 neo        (501) staff       (20)    37206 2022-12-30 23:57:27.000000 netkiller-devops-0.6.8/netkiller/kubernetes.py
--rw-r--r--   0 neo        (501) staff       (20)     4628 2022-01-09 13:02:59.000000 netkiller-devops-0.6.8/netkiller/mongo.py
--rw-r--r--   0 neo        (501) staff       (20)     4199 2022-01-09 13:02:59.000000 netkiller-devops-0.6.8/netkiller/mysql.py
--rw-r--r--   0 neo        (501) staff       (20)     2195 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/netkiller/nagios.py
--rw-r--r--   0 neo        (501) staff       (20)     4878 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/netkiller/pipeline.py
--rw-r--r--   0 neo        (501) staff       (20)     5253 2023-01-08 13:37:26.000000 netkiller-devops-0.6.8/netkiller/podman.py
--rw-r--r--   0 neo        (501) staff       (20)     1705 2021-09-22 11:38:29.000000 netkiller-devops-0.6.8/netkiller/rsync.py
--rw-r--r--   0 neo        (501) staff       (20)     1535 2021-10-15 09:59:59.000000 netkiller-devops-0.6.8/netkiller/wework.py
--rw-r--r--   0 neo        (501) staff       (20)     2320 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/netkiller/whiptail.py
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.500915 netkiller-devops-0.6.8/netkiller_devops.egg-info/
--rw-r--r--   0 neo        (501) staff       (20)     1746 2023-02-08 05:08:40.000000 netkiller-devops-0.6.8/netkiller_devops.egg-info/PKG-INFO
--rw-r--r--   0 neo        (501) staff       (20)     1102 2023-02-08 05:08:41.000000 netkiller-devops-0.6.8/netkiller_devops.egg-info/SOURCES.txt
--rw-r--r--   0 neo        (501) staff       (20)        1 2023-02-08 05:08:40.000000 netkiller-devops-0.6.8/netkiller_devops.egg-info/dependency_links.txt
--rw-r--r--   0 neo        (501) staff       (20)       67 2023-02-08 05:08:41.000000 netkiller-devops-0.6.8/netkiller_devops.egg-info/requires.txt
--rw-r--r--   0 neo        (501) staff       (20)       10 2023-02-08 05:08:41.000000 netkiller-devops-0.6.8/netkiller_devops.egg-info/top_level.txt
--rw-r--r--   0 neo        (501) staff       (20)       38 2023-02-08 05:08:41.503820 netkiller-devops-0.6.8/setup.cfg
--rw-r--r--   0 neo        (501) staff       (20)     2089 2023-02-08 05:08:18.000000 netkiller-devops-0.6.8/setup.py
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.480650 netkiller-devops-0.6.8/share/
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.480464 netkiller-devops-0.6.8/share/example/
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.501271 netkiller-devops-0.6.8/share/example/testing/
--rw-r--r--   0 neo        (501) staff       (20)     1121 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/share/example/testing/example.com.ini
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.501769 netkiller-devops-0.6.8/share/profile.d/
--rw-r--r--   0 neo        (501) staff       (20)       34 2021-04-12 02:34:04.000000 netkiller-devops-0.6.8/share/profile.d/devops.sh
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.480978 netkiller-devops-0.6.8/shell/
-drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-02-08 05:08:41.502960 netkiller-devops-0.6.8/shell/backup/
--rw-r--r--   0 neo        (501) staff       (20)     1500 2022-01-09 13:03:00.000000 netkiller-devops-0.6.8/shell/backup/backup.mysql.gpg.sh
--rw-r--r--   0 neo        (501) staff       (20)     1424 2022-01-09 13:03:00.000000 netkiller-devops-0.6.8/shell/backup/backup.mysql.sh
--rw-r--r--   0 neo        (501) staff       (20)     2426 2022-01-09 13:03:00.000000 netkiller-devops-0.6.8/shell/backup/backup.mysql.struct.sh
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.711833 netkiller-devops-0.6.9/
+-rw-r--r--   0 neo        (501) staff       (20)     1081 2021-04-12 02:34:54.000000 netkiller-devops-0.6.9/LICENSE
+-rw-r--r--   0 neo        (501) staff       (20)       13 2021-10-09 03:00:15.000000 netkiller-devops-0.6.9/MANIFEST.in
+-rw-r--r--   0 neo        (501) staff       (20)     1746 2023-03-08 14:13:26.711486 netkiller-devops-0.6.9/PKG-INFO
+-rw-r--r--   0 neo        (501) staff       (20)     1230 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/README.md
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.690120 netkiller-devops-0.6.9/bin/
+-rwxr-xr-x   0 neo        (501) staff       (20)     8175 2021-05-06 06:45:40.000000 netkiller-devops-0.6.9/bin/backup
+-rw-r--r--   0 neo        (501) staff       (20)      512 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/bin/chpasswd.sh
+-rw-r--r--   0 neo        (501) staff       (20)    18040 2021-04-29 03:46:42.000000 netkiller-devops-0.6.9/bin/deployment
+-rw-r--r--   0 neo        (501) staff       (20)     2392 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/dingtalk
+-rw-r--r--   0 neo        (501) staff       (20)     1939 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/bin/gitsync
+-rw-r--r--   0 neo        (501) staff       (20)     4071 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/logviewer
+-rw-r--r--   0 neo        (501) staff       (20)     4223 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/logviewer.docker
+-rw-r--r--   0 neo        (501) staff       (20)     5389 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/logviewer.kubectl
+-rw-r--r--   0 neo        (501) staff       (20)     3095 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/lrsync
+-rw-r--r--   0 neo        (501) staff       (20)       65 2022-09-01 10:12:24.000000 netkiller-devops-0.6.9/bin/matrixpasswd
+-rwxr-xr-x   0 neo        (501) staff       (20)     7481 2022-01-09 13:02:59.000000 netkiller-devops-0.6.9/bin/mdump
+-rwxr-xr-x   0 neo        (501) staff       (20)     9264 2023-03-08 14:13:11.000000 netkiller-devops-0.6.9/bin/merge
+-rw-r--r--   0 neo        (501) staff       (20)     5117 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/bin/mysqlshell
+-rw-r--r--   0 neo        (501) staff       (20)     9467 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/bin/osconf
+-rw-r--r--   0 neo        (501) staff       (20)       53 2022-09-01 10:12:24.000000 netkiller-devops-0.6.9/bin/randpasswd
+-rw-r--r--   0 neo        (501) staff       (20)       66 2022-09-01 10:12:24.000000 netkiller-devops-0.6.9/bin/randtext
+-rwxr-xr-x   0 neo        (501) staff       (20)     7552 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/sqldump
+-rwxr-xr-x   0 neo        (501) staff       (20)     3942 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/voice
+-rwxr-xr-x   0 neo        (501) staff       (20)     2262 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/bin/wechat
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.691336 netkiller-devops-0.6.9/doc/
+-rw-r--r--   0 neo        (501) staff       (20)     1130 2021-09-28 09:40:58.000000 netkiller-devops-0.6.9/doc/voice.md
+-rw-r--r--   0 neo        (501) staff       (20)      964 2023-02-08 05:08:18.000000 netkiller-devops-0.6.9/doc/wechat.md
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.696729 netkiller-devops-0.6.9/etc/
+-rw-r--r--   0 neo        (501) staff       (20)      336 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/etc/deployment.cfg
+-rw-r--r--   0 neo        (501) staff       (20)      398 2021-10-21 09:04:52.000000 netkiller-devops-0.6.9/etc/dump.ini
+-rw-r--r--   0 neo        (501) staff       (20)      551 2021-10-22 02:44:34.000000 netkiller-devops-0.6.9/etc/dump.ini.sample
+-rw-r--r--   0 neo        (501) staff       (20)      200 2022-11-10 02:00:07.000000 netkiller-devops-0.6.9/etc/logviewer.ini
+-rw-r--r--   0 neo        (501) staff       (20)      488 2022-01-09 13:02:59.000000 netkiller-devops-0.6.9/etc/mongo.ini.sample
+-rw-r--r--   0 neo        (501) staff       (20)       87 2021-09-28 08:36:03.000000 netkiller-devops-0.6.9/etc/notification.ini
+-rw-r--r--   0 neo        (501) staff       (20)      218 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/etc/os.ini
+-rw-r--r--   0 neo        (501) staff       (20)      125 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/etc/schedule.cfg
+-rw-r--r--   0 neo        (501) staff       (20)     1117 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/etc/task.cfg
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.705873 netkiller-devops-0.6.9/netkiller/
+-rw-r--r--   0 neo        (501) staff       (20)       71 2021-09-06 10:55:06.000000 netkiller-devops-0.6.9/netkiller/__init__.py
+-rw-r--r--   0 neo        (501) staff       (20)    30888 2023-02-24 10:09:35.000000 netkiller-devops-0.6.9/netkiller/docker.py
+-rw-r--r--   0 neo        (501) staff       (20)     5198 2023-03-08 14:13:11.000000 netkiller-devops-0.6.9/netkiller/git.py
+-rw-r--r--   0 neo        (501) staff       (20)     5432 2022-01-09 13:02:59.000000 netkiller-devops-0.6.9/netkiller/gitlab.py
+-rw-r--r--   0 neo        (501) staff       (20)    37206 2022-12-30 23:57:27.000000 netkiller-devops-0.6.9/netkiller/kubernetes.py
+-rw-r--r--   0 neo        (501) staff       (20)     4628 2022-01-09 13:02:59.000000 netkiller-devops-0.6.9/netkiller/mongo.py
+-rw-r--r--   0 neo        (501) staff       (20)     4199 2022-01-09 13:02:59.000000 netkiller-devops-0.6.9/netkiller/mysql.py
+-rw-r--r--   0 neo        (501) staff       (20)     2195 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/netkiller/nagios.py
+-rw-r--r--   0 neo        (501) staff       (20)     4889 2023-03-08 14:13:11.000000 netkiller-devops-0.6.9/netkiller/pipeline.py
+-rw-r--r--   0 neo        (501) staff       (20)     5253 2023-01-08 13:37:26.000000 netkiller-devops-0.6.9/netkiller/podman.py
+-rw-r--r--   0 neo        (501) staff       (20)     1705 2021-09-22 11:38:29.000000 netkiller-devops-0.6.9/netkiller/rsync.py
+-rw-r--r--   0 neo        (501) staff       (20)     1535 2021-10-15 09:59:59.000000 netkiller-devops-0.6.9/netkiller/wework.py
+-rw-r--r--   0 neo        (501) staff       (20)     2320 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/netkiller/whiptail.py
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.707956 netkiller-devops-0.6.9/netkiller_devops.egg-info/
+-rw-r--r--   0 neo        (501) staff       (20)     1746 2023-03-08 14:13:25.000000 netkiller-devops-0.6.9/netkiller_devops.egg-info/PKG-INFO
+-rw-r--r--   0 neo        (501) staff       (20)     1102 2023-03-08 14:13:26.000000 netkiller-devops-0.6.9/netkiller_devops.egg-info/SOURCES.txt
+-rw-r--r--   0 neo        (501) staff       (20)        1 2023-03-08 14:13:25.000000 netkiller-devops-0.6.9/netkiller_devops.egg-info/dependency_links.txt
+-rw-r--r--   0 neo        (501) staff       (20)       67 2023-03-08 14:13:26.000000 netkiller-devops-0.6.9/netkiller_devops.egg-info/requires.txt
+-rw-r--r--   0 neo        (501) staff       (20)       10 2023-03-08 14:13:26.000000 netkiller-devops-0.6.9/netkiller_devops.egg-info/top_level.txt
+-rw-r--r--   0 neo        (501) staff       (20)       38 2023-03-08 14:13:26.711939 netkiller-devops-0.6.9/setup.cfg
+-rw-r--r--   0 neo        (501) staff       (20)     2089 2023-03-08 14:13:11.000000 netkiller-devops-0.6.9/setup.py
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.674107 netkiller-devops-0.6.9/share/
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.673849 netkiller-devops-0.6.9/share/example/
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.708299 netkiller-devops-0.6.9/share/example/testing/
+-rw-r--r--   0 neo        (501) staff       (20)     1121 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/share/example/testing/example.com.ini
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.708829 netkiller-devops-0.6.9/share/profile.d/
+-rw-r--r--   0 neo        (501) staff       (20)       34 2021-04-12 02:34:04.000000 netkiller-devops-0.6.9/share/profile.d/devops.sh
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.674511 netkiller-devops-0.6.9/shell/
+drwxr-xr-x   0 neo        (501) staff       (20)        0 2023-03-08 14:13:26.710750 netkiller-devops-0.6.9/shell/backup/
+-rw-r--r--   0 neo        (501) staff       (20)     1500 2022-01-09 13:03:00.000000 netkiller-devops-0.6.9/shell/backup/backup.mysql.gpg.sh
+-rw-r--r--   0 neo        (501) staff       (20)     1424 2022-01-09 13:03:00.000000 netkiller-devops-0.6.9/shell/backup/backup.mysql.sh
+-rw-r--r--   0 neo        (501) staff       (20)     2426 2022-01-09 13:03:00.000000 netkiller-devops-0.6.9/shell/backup/backup.mysql.struct.sh
```

### Comparing `netkiller-devops-0.6.8/LICENSE` & `netkiller-devops-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/PKG-INFO` & `netkiller-devops-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netkiller-devops
-Version: 0.6.8
+Version: 0.6.9
 Summary: DevOps of useful deployment and automation
 Home-page: https://github.com/oscm/devops
 Author: Neo Chen
 Author-email: netkiller@msn.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `netkiller-devops-0.6.8/README.md` & `netkiller-devops-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/backup` & `netkiller-devops-0.6.9/bin/backup`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/chpasswd.sh` & `netkiller-devops-0.6.9/bin/chpasswd.sh`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/deployment` & `netkiller-devops-0.6.9/bin/deployment`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/dingtalk` & `netkiller-devops-0.6.9/bin/dingtalk`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/gitsync` & `netkiller-devops-0.6.9/bin/gitsync`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/logviewer` & `netkiller-devops-0.6.9/bin/logviewer`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/logviewer.docker` & `netkiller-devops-0.6.9/bin/logviewer.docker`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/logviewer.kubectl` & `netkiller-devops-0.6.9/bin/logviewer.kubectl`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/lrsync` & `netkiller-devops-0.6.9/bin/lrsync`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/mdump` & `netkiller-devops-0.6.9/bin/mdump`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/merge` & `netkiller-devops-0.6.9/bin/merge`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
         usage = "usage: %prog [options] <parameter>"
         self.parser = OptionParser(usage)
         self.parser.add_option('-w', '--workspace', dest='workspace',
                                help='workspace ~/workspace', default='None', metavar='~/workspace')
         self.parser.add_option('-p', '--project', dest='project',
                                help='project directory', default=None, metavar='')
+        self.parser.add_option('-C', '--changelist', dest='changelist', help='Change list',
+                               default=None, metavar='2023-03-01')
         self.parser.add_option('-l', '--logfile', dest='logfile', help='log file',
                                default='/tmp/merge.log', metavar='/tmp/merge.log')
         self.parser.add_option('-d', '--debug', dest='debug',
                                action='store_true', help="debug")
 
         group = OptionGroup(self.parser, "Repository")
         group.add_option('-c', '--clone', dest='clone', help='clone branch', default=None,
@@ -153,27 +155,35 @@
     def reset(self, ver=None):
         git = GitReset(self.project, self.logger)
         git.hard(ver).execute()
 
     def push(self):
         git = Git(self.project, self.logger)
         git.push(True).execute()
+    def changelist(self, since):
+        git = Git(self.project, self.logger)
+        git.log('--since="'+since+'" --no-merges --pretty=format:"%h %an %ai %s"')
+        git.execute()
 
     def main(self):
         if self.options.workspace:
             self.workspace = self.options.workspace
 
         if self.options.project:
             if self.workspace:
                 self.project = self.workspace + '/' + self.project
             else:
                 self.project = self.options.project
         else:
             self.project = os.getcwd()
 
+        if self.options.changelist :
+            self.changelist(self.options.changelist)
+            exit()
+
         if self.options.clone:
             self.clone(self.options.clone)
             exit()
 
         if self.options.checkout:
             self.checkout(self.options.checkout)
             exit()
```

### Comparing `netkiller-devops-0.6.8/bin/mysqlshell` & `netkiller-devops-0.6.9/bin/mysqlshell`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/osconf` & `netkiller-devops-0.6.9/bin/osconf`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/sqldump` & `netkiller-devops-0.6.9/bin/sqldump`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/voice` & `netkiller-devops-0.6.9/bin/voice`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/bin/wechat` & `netkiller-devops-0.6.9/bin/wechat`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/doc/voice.md` & `netkiller-devops-0.6.9/doc/voice.md`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/doc/wechat.md` & `netkiller-devops-0.6.9/doc/wechat.md`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/etc/dump.ini.sample` & `netkiller-devops-0.6.9/etc/dump.ini.sample`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/etc/task.cfg` & `netkiller-devops-0.6.9/etc/task.cfg`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/docker.py` & `netkiller-devops-0.6.9/netkiller/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,15 +853,15 @@
                 obj.exec(service, cmd)
         return (self)
 
     def usage(self):
         print("Python controls the docker manager.")
         self.parser.print_help()
         print(
-            "\nHomepage: http://www.netkiller.cn\tAuthor: Neo <netkiller@msn.com>"
+            "\nHomepage: http://www.netkiller.cn\tAuthor: Neo <netkiller@msn.com>\nHelp: https://github.com/netkiller/devops/blob/master/doc/docker.md"
         )
         exit()
 
     def main(self):
 
         if self.options.export:
             self.save_all()
```

### Comparing `netkiller-devops-0.6.8/netkiller/git.py` & `netkiller-devops-0.6.9/netkiller/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #-*- coding: utf-8 -*-
 import os, sys,logging
 class Git():
 	def __init__(self, workspace = None, logger = None):
 		self.cmd = []
+		self.opt = None
 		if logger :
 			self.logger = logger
 		else:
 			self.logger = logging.getLogger()
 		self.workspace = os.path.expanduser(workspace)
 		if os.path.exists(self.workspace) :
 			os.chdir(self.workspace)
@@ -40,16 +41,19 @@
 		return(self)
 	def checkout(self, branch):
 		self.cmd.append('checkout {0}'.format(branch))
 		return(self)
 	def status(self):
 		self.cmd.append('status')
 		return(self)
-	def log(self):
-		self.cmd.append('log')
+	def log(self, opt = None):
+		if opt :
+			self.cmd.append('log '+ opt)
+		else:
+			self.cmd.append('log')
 		return(self)
 	def pull(self):
 		# if self.workspace :
 			# os.chdir(self.workspace)
 		self.cmd.append('pull --progress')
 		return(self)
 	def fetch(self):
```

### Comparing `netkiller-devops-0.6.8/netkiller/gitlab.py` & `netkiller-devops-0.6.9/netkiller/gitlab.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/kubernetes.py` & `netkiller-devops-0.6.9/netkiller/kubernetes.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/mongo.py` & `netkiller-devops-0.6.9/netkiller/mongo.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/mysql.py` & `netkiller-devops-0.6.9/netkiller/mysql.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/nagios.py` & `netkiller-devops-0.6.9/netkiller/nagios.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/pipeline.py` & `netkiller-devops-0.6.9/netkiller/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         if script:
             self.pipelines['end'] = script
         try:
             for stage in ['begin','init', 'checkout', 'build', 'dockerfile', 'deploy', 'stop', 'startup', 'end']:
                 if stage in self.pipelines.keys():
                     for command in self.pipelines[stage]:
                         rev = subprocess.call(command, shell=True)
-                        if rev == 0 :
+                        if rev.returncode == 0 :
                             status = 'done'
                         else:
                             status = 'error'
                         self.logging.info("command: %s, %s, status: %s" % (rev, command,status))
                         # if rev != 0 :
                         # raise Exception("{} 执行失败".format(command))
         except KeyboardInterrupt as e:
```

### Comparing `netkiller-devops-0.6.8/netkiller/podman.py` & `netkiller-devops-0.6.9/netkiller/podman.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/rsync.py` & `netkiller-devops-0.6.9/netkiller/rsync.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/wework.py` & `netkiller-devops-0.6.9/netkiller/wework.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller/whiptail.py` & `netkiller-devops-0.6.9/netkiller/whiptail.py`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/netkiller_devops.egg-info/PKG-INFO` & `netkiller-devops-0.6.9/netkiller_devops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netkiller-devops
-Version: 0.6.8
+Version: 0.6.9
 Summary: DevOps of useful deployment and automation
 Home-page: https://github.com/oscm/devops
 Author: Neo Chen
 Author-email: netkiller@msn.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `netkiller-devops-0.6.8/netkiller_devops.egg-info/SOURCES.txt` & `netkiller-devops-0.6.9/netkiller_devops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/setup.py` & `netkiller-devops-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from netkiller import __version__, __author__
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
 	name="netkiller-devops",
-	version="0.6.8",
+	version="0.6.9",
 	author="Neo Chen",
 	author_email="netkiller@msn.com",
 	description="DevOps of useful deployment and automation",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/oscm/devops",
 	license='BSD',
```

### Comparing `netkiller-devops-0.6.8/share/example/testing/example.com.ini` & `netkiller-devops-0.6.9/share/example/testing/example.com.ini`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/shell/backup/backup.mysql.gpg.sh` & `netkiller-devops-0.6.9/shell/backup/backup.mysql.gpg.sh`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/shell/backup/backup.mysql.sh` & `netkiller-devops-0.6.9/shell/backup/backup.mysql.sh`

 * *Files identical despite different names*

### Comparing `netkiller-devops-0.6.8/shell/backup/backup.mysql.struct.sh` & `netkiller-devops-0.6.9/shell/backup/backup.mysql.struct.sh`

 * *Files identical despite different names*

