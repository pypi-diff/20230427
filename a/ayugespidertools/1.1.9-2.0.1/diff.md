# Comparing `tmp/ayugespidertools-1.1.9.tar.gz` & `tmp/ayugespidertools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-1.1.9.tar", max compression
+gzip compressed data, was "ayugespidertools-2.0.1.tar", max compression
```

## Comparing `ayugespidertools-1.1.9.tar` & `ayugespidertools-2.0.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/LICENSE
--rw-r--r--   0        0        0    13490 2023-04-18 02:43:49.000000 ayugespidertools-1.1.9/README.md
--rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyuRequest.py
--rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyugeCrawlSpider.py
--rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/AyugeSpider.py
--rw-r--r--   0        0        0     8203 2023-04-19 06:53:29.000000 ayugespidertools-1.1.9/ayugespidertools/DownloaderMiddlewares.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.9/ayugespidertools/FormatData.py
--rw-r--r--   0        0        0     7681 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/ImgOperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.9/ayugespidertools/Items.py
--rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/Middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/MongoClient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/MysqlClient.py
--rw-r--r--   0        0        0     5475 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/Oss.py
--rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/Pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/ProcessManager.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/RPA.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/RunJs.py
--rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/VerificationCode.py
--rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.9/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-1.1.9/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      158 2023-04-18 06:47:49.372425 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      536 2023-04-17 09:29:59.544907 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2914 2023-04-18 06:47:49.395425 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-04-19 07:06:38.147286 ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.9/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4170 2023-04-18 02:26:28.000000 ayugespidertools-1.1.9/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-1.1.9/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0     3704 2023-04-14 07:32:45.000000 ayugespidertools-1.1.9/ayugespidertools/common/Encryption.py
--rw-r--r--   0        0        0     6622 2023-04-14 08:08:19.000000 ayugespidertools-1.1.9/ayugespidertools/common/Expend.py
--rw-r--r--   0        0        0     3847 2023-04-20 03:24:39.000000 ayugespidertools-1.1.9/ayugespidertools/common/MongoDBPipe.py
--rw-r--r--   0        0        0    11850 2023-04-18 08:38:38.000000 ayugespidertools-1.1.9/ayugespidertools/common/MultiPlexing.py
--rw-r--r--   0        0        0    13474 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/common/MysqlErrorHandle.py
--rw-r--r--   0        0        0    32577 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/common/Params.py
--rw-r--r--   0        0        0     4264 2023-04-18 13:16:46.000000 ayugespidertools-1.1.9/ayugespidertools/common/SpiderDBConf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-1.1.9/ayugespidertools/common/SqlFormat.py
--rw-r--r--   0        0        0     1514 2023-04-18 06:42:57.000000 ayugespidertools-1.1.9/ayugespidertools/common/TypeVars.py
--rw-r--r--   0        0        0    10924 2023-04-18 09:04:47.000000 ayugespidertools-1.1.9/ayugespidertools/common/Utils.py
--rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/common/YiDunGap.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-1.1.9/ayugespidertools/config.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0      813 2023-04-18 08:27:37.369445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-04-18 08:27:37.370445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
--rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0     2178 2023-04-18 08:27:37.372445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
--rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0      175 2023-04-18 08:27:37.372445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3927 2023-04-18 08:27:37.374445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
--rw-r--r--   0        0        0     3051 2023-04-18 08:27:37.376445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
--rw-r--r--   0        0        0     7802 2023-04-18 08:27:37.381445 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
--rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11208 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      885 2023-04-14 09:46:54.212591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0      173 2023-04-14 09:46:54.212591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3093 2023-04-14 09:46:54.213591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1820 2023-04-14 09:46:54.217591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-12 02:07:09.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13398 2023-04-18 06:55:07.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0    11211 2023-04-18 07:50:48.385727 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3005 2023-04-18 06:47:10.331390 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-04-14 09:46:54.228591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1998 2023-04-14 09:46:54.228591 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
--rw-r--r--   0        0        0     3621 2023-04-18 06:47:10.350390 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     2824 2023-04-18 06:45:18.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3897 2023-04-18 06:44:38.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-18 13:17:20.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-18 13:18:47.788335 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-13 07:18:02.706131 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      627 2023-04-20 06:55:52.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
--rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4161 2023-04-19 03:35:24.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.9/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.9/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.9/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0      155 2023-04-17 09:29:59.415907 ayugespidertools-1.1.9/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5360 2023-04-18 06:47:53.532429 ayugespidertools-1.1.9/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
--rw-r--r--   0        0        0     5953 2023-04-18 02:22:33.000000 ayugespidertools-1.1.9/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     3136 2023-04-19 07:13:26.000000 ayugespidertools-1.1.9/pyproject.toml
--rw-r--r--   0        0        0    15160 1970-01-01 00:00:00.000000 ayugespidertools-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/LICENSE
+-rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.1/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.1/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.1/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2871 2023-04-27 08:04:48.083361 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.1/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4050 2023-04-27 07:39:48.000000 ayugespidertools-2.0.1/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.1/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.1/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.1/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     3858 2023-04-25 02:55:36.000000 ayugespidertools-2.0.1/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.1/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.1/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.1/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.1/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.1/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.1/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.1/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.1/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.1/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.1/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.1/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.1/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.1/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.1/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-2.0.1/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.1/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.1/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
+-rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
+-rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
+-rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3093 2023-04-25 08:58:19.203438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     3022 2023-04-25 03:00:27.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3005 2023-04-25 08:58:19.211438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1998 2023-04-25 08:58:19.220438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     2824 2023-04-25 03:01:16.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2840 2023-04-25 03:01:31.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.1/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5327 2023-04-27 08:04:47.882360 ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
+-rw-r--r--   0        0        0     5920 2023-04-27 07:40:39.000000 ayugespidertools-2.0.1/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.1/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3004 2023-04-26 09:50:14.000000 ayugespidertools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    15467 1970-01-01 00:00:00.000000 ayugespidertools-2.0.1/PKG-INFO
```

### Comparing `ayugespidertools-1.1.9/LICENSE` & `ayugespidertools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/README.md` & `ayugespidertools-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 > `python 3.8+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
-注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
+注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.4` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
 ## 2. 使用方法
 
 > 项目主要包含两部分：
 >
 
 - 开发场景中的工具库
@@ -47,27 +47,27 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：ayugespidertools cli 的名称也可用 ayuge 来代替，输入体验更友好。
+# 注：更推荐使用 ayuge 的 cli 名称，输入体验更友好，（ayugespidertools 的 cli 则会在下一大版本中会剔除）。
 
 # 查看库版本
-ayugespidertools version
+ayuge version
 
 # 创建项目
-ayugespidertools startproject <project_name>
+ayuge startproject <project_name>
 
 # 进入项目根目录
 cd <project_name>
 
 # 生成爬虫脚本
-ayugespidertools genspider <spider_name> <example.com>
+ayuge genspider <spider_name> <example.com>
 
 # 替换(覆盖)为真实的配置 .conf 文件；
 # 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 运行脚本
 scrapy crawl <spider_name>
@@ -144,14 +144,15 @@
 
 ### 3.2. 你可能在意的事
 
 > 此项目会慢慢丰富 `python` 开发中的遇到的通用方法，详情请见 [TodoList](#TodoList)。
 
 1. 若你觉得某些场景下的功能实现不太符合你的预期，想要修改或添加自定义功能，或移除对你无用模块、修改库名等，你可以自行修改后 `build`。
 2. 本库主推 `scrapy` 扩展（即增强版的自定义模板）的功能，在使用本库时，理论上并不会影响你 `scrapy` 项目及其它组件，且你也可以根据上条须知来增强此库功能。因为模板功能天生就有及其明确的优缺点，我无法覆盖所有应用场景，**但是它的高效率的确会解放双手**。
+3. **当然，你也可以选择给此项目做出贡献，比如增加或优化某些功能等，但在此之前请提相关的 `ISSUES` 经确认后再开发和提交 `PULL REQUESTS`，以免不太符合本库场景或已废弃等原因造成你的贡献浪费，那就太可惜了！**
 
 ### 3.3. Build-Your-Own-Library
 
 > 具体内容请以 [poetry 官方文档](https://python-poetry.org/docs/) 为准。
 
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/FormatData.py` & `ayugespidertools-2.0.1/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/ImgOperation.py` & `ayugespidertools-2.0.1/ayugespidertools/imgoperation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union
 
 import cv2
 from PIL import Image
 
-from ayugespidertools.common.Encryption import EncryptOperation
-from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.encryption import EncryptOperation
+from ayugespidertools.common.multiplexing import ReuseOperation
 
 __all__ = [
     "Picture",
 ]
 
 
 class Picture(object):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/Items.py` & `ayugespidertools-2.0.1/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/Middlewares.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+# Define here the models for your spider middleware
+#
+# See documentation in:
+# https://docs.scrapy.org/en/latest/topics/spider-middleware.html
 from ayugespidertools.scraper.middlewares.headers.ua import RandomRequestUaMiddleware
+from ayugespidertools.scraper.middlewares.netlib.aiohttplib import (
+    AiohttpAsyncDownloaderMiddleware,
+    AiohttpDownloaderMiddleware,
+)
 from ayugespidertools.scraper.middlewares.netlib.requestslib import (
-    RequestByRequestsMiddleware,
+    RequestsDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.dynamic import (
     AbuDynamicProxyDownloaderMiddleware,
     DynamicProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.exclusive import (
     ExclusiveProxyDownloaderMiddleware,
 )
+from ayugespidertools.scraper.middlewares.proxy.private import (
+    PrivateProxyDownloaderMiddleware,
+)
 
 __all__ = [
     "RandomRequestUaMiddleware",
+    "RequestsDownloaderMiddleware",
+    "AiohttpAsyncDownloaderMiddleware",
+    "AiohttpDownloaderMiddleware",
     "DynamicProxyDownloaderMiddleware",
-    "ExclusiveProxyDownloaderMiddleware",
     "AbuDynamicProxyDownloaderMiddleware",
-    "RequestByRequestsMiddleware",
+    "ExclusiveProxyDownloaderMiddleware",
+    "PrivateProxyDownloaderMiddleware",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/MongoClient.py` & `ayugespidertools-2.0.1/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/MysqlClient.py` & `ayugespidertools-2.0.1/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/Oss.py` & `ayugespidertools-2.0.1/ayugespidertools/oss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import warnings
 from typing import Union
 
 import oss2
 import requests
 from retrying import retry
 
-from ayugespidertools.common.Encryption import EncryptOperation
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.encryption import EncryptOperation
+from ayugespidertools.common.params import Param
 
 warnings.filterwarnings("ignore")
 
 __all__ = [
     "AliOssBase",
 ]
 
@@ -22,50 +22,51 @@
         https://github.com/aliyun/aliyun-oss-python-sdk?spm=5176.8465980.tools.dpython-github.572b1450ON6Z9R
     阿里云官方 oss sdk 文档地址：
         https://www.alibabacloud.com/help/zh/object-storage-service/latest/python-quick-start
     """
 
     def __init__(
         self,
-        OssAccessKeyId: str,
-        OssAccessKeySecret: str,
-        Endpoint: str,
-        examplebucket: str,
-        operateDoc: str,
+        access_key_id: str,
+        access_key_secret: str,
+        endpoint: str,
+        bucket: str,
+        doc: str,
     ) -> None:
         """
         初始化 auth，bucket 等信息
         注：阿里云账号 AccessKey 拥有所有 API 的访问权限，风险很高；
             强烈建议您创建并使用 RAM 用户进行 API 访问或日常运维，请登录 RAM 控制台创建 RAM 用户
         Args:
-            OssAccessKeyId: 阿里云账号 AccessKey
-            OssAccessKeySecret: 阿里云账号 AccessKey 对应的秘钥
-            Endpoint: 填写 Bucket 所在地域对应的 Endpoint；
+            access_key_id: 阿里云账号 AccessKey
+            access_key_secret: 阿里云账号 AccessKey 对应的秘钥
+            endpoint: 填写 Bucket 所在地域对应的 Endpoint；
                 以华东1（杭州）为例，Endpoint 填写为 https://oss-cn-hangzhou.aliyuncs.com（注意二级域名等问题）
-            examplebucket: 填写 Bucket 名称，此 oss 项目所在文件夹目录
+            bucket: 填写 Bucket 名称，此 oss 项目所属 bucket
+            doc: 需要操作的 oss 文件夹目录
         """
-        self.Endpoint = Endpoint
-        self.operateDoc = operateDoc
-        self.examplebucket = examplebucket
-        self.auth = oss2.Auth(OssAccessKeyId, OssAccessKeySecret)
-        self.bucket = oss2.Bucket(self.auth, f"{self.Endpoint}/", self.examplebucket)
+        self.endpoint = endpoint
+        self.doc = doc
+        self.bucket = bucket
+        self.auth = oss2.Auth(access_key_id, access_key_secret)
+        self.bucket = oss2.Bucket(self.auth, f"{self.endpoint}/", self.bucket)
         self.headers = {"Connection": "close"}
 
     def delete_oss(self, del_logo_url: str):
         """
-        删除单个文件: 以下代码用于删除 examplebucket 中的 del_logo_url 所对应的文件
+        删除单个文件: 以下代码用于删除 bucket 中的 del_logo_url 所对应的文件
         Args:
             del_logo_url: 需要参数的阿里云链接全路径 url
 
         Returns:
             None
         """
         try:
             self.bucket.delete_object(
-                f"{self.operateDoc}/{del_logo_url.replace(f'{self.Endpoint}/{self.operateDoc}/', '')}"
+                f"{self.doc}/{del_logo_url.replace(f'{self.endpoint}/{self.doc}/', '')}"
             )
         except oss2.exceptions.NoSuchKey as e:
             raise ValueError(
                 f"delete_oss error: status={e.status}, request_id={e.request_id}"
             ) from e
 
     @retry(
@@ -98,15 +99,15 @@
         if isinstance(put_bytes_or_url, str):
             put_bytes_or_url = requests.get(
                 url=put_bytes_or_url, headers=self.headers, verify=False
             ).content
 
         try:
             self.bucket.put_object(
-                f"{self.operateDoc}/{input_file_name}.{file_format}",
+                f"{self.doc}/{input_file_name}.{file_format}",
                 put_bytes_or_url,
             )
         except Exception:
             return False, ""
         return True, input_file_name
 
     def enumer_file_by_pre(
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/Pipelines.py` & `ayugespidertools-2.0.1/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/RPA.py` & `ayugespidertools-2.0.1/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/RunJs.py` & `ayugespidertools-2.0.1/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/VerificationCode.py` & `ayugespidertools-2.0.1/ayugespidertools/verificationcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import random
 
 import cv2
 import numpy as np
 
-from ayugespidertools.common.YiDunGap import YiDunGetGap
+from ayugespidertools.common.yidungap import YiDunGetGap
 
 __all__ = [
     "match_img_get_distance",
     "get_selenium_tracks",
     "get_yidun_tracks",
     "get_yidun_gap",
     "get_normal_track",
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 02:26:28 2023 UTC, .py size: 4170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 d4ff 3d64 4a10 0000  U.........=dJ...
+00000000: 550d 0d0a 0000 0000 c426 4a64 d20f 0000  U........&Jd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6401 6c0d  m.Z.m.Z...d.d.l.
@@ -12,172 +12,169 @@
 000000b0: 5300 290e e900 0000 004e 2901 da04 5061  S.)......N)...Pa
 000000c0: 7468 2902 da0f 6967 6e6f 7265 5f70 6174  th)...ignore_pat
 000000d0: 7465 726e 73da 046d 6f76 6529 01da 0743  terns..move)...C
 000000e0: 6f6d 6d61 6e64 2901 da0a 5573 6167 6545  ommand)...UsageE
 000000f0: 7272 6f72 2902 da13 7265 6e64 6572 5f74  rror)...render_t
 00000100: 656d 706c 6174 6566 696c 65da 1073 7472  emplatefile..str
 00000110: 696e 675f 6361 6d65 6c63 6173 6529 01da  ing_camelcase)..
-00000120: 0550 6172 616d 290c a901 7a0a 2e67 6974  .Param)...z..git
+00000120: 0550 6172 616d 290b a901 7a0a 2e67 6974  .Param)...z..git
 00000130: 6967 6e6f 7265 2901 7a0e 7079 7072 6f6a  ignore).z.pyproj
 00000140: 6563 742e 746f 6d6c 2901 7a09 5245 4144  ect.toml).z.READ
 00000150: 4d45 2e6d 6429 017a 1072 6571 7569 7265  ME.md).z.require
 00000160: 6d65 6e74 732e 7478 7472 0a00 0000 2901  ments.txtr....).
 00000170: fa0a 7363 7261 7079 2e63 6667 2902 fa0f  ..scrapy.cfg)...
 00000180: 247b 7072 6f6a 6563 745f 6e61 6d65 7d7a  ${project_name}z
 00000190: 1073 6574 7469 6e67 732e 7079 2e74 6d70  .settings.py.tmp
 000001a0: 6c29 0272 0c00 0000 7a0d 6974 656d 732e  l).r....z.items.
 000001b0: 7079 2e74 6d70 6c29 0272 0c00 0000 7a11  py.tmpl).r....z.
 000001c0: 7069 7065 6c69 6e65 732e 7079 2e74 6d70  pipelines.py.tmp
 000001d0: 6c29 0272 0c00 0000 7a13 6d69 6464 6c65  l).r....z.middle
 000001e0: 7761 7265 732e 7079 2e74 6d70 6c29 0272  wares.py.tmpl).r
 000001f0: 0c00 0000 7a0b 7275 6e2e 7079 2e74 6d70  ....z.run.py.tmp
-00000200: 6c29 0272 0c00 0000 7a17 636f 6d6d 6f6e  l).r....z.common
-00000210: 2f44 6174 6145 6e75 6d2e 7079 2e74 6d70  /DataEnum.py.tmp
-00000220: 6c7a 052a 2e70 7963 da0b 5f5f 7079 6361  lz.*.pyc..__pyca
-00000230: 6368 655f 5f7a 042e 7376 6e63 0000 0000  che__z..svnc....
-00000240: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000250: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
-00000260: 0264 0164 0284 005a 0365 0465 0564 039c  .d.d...Z.e.e.d..
-00000270: 0164 0464 0584 0483 015a 0664 0653 0029  .d.d.....Z.d.S.)
-00000280: 07da 0a41 7975 436f 6d6d 616e 6463 0300  ...AyuCommandc..
-00000290: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
-000002a0: 0000 0300 0000 73c2 0100 0074 007c 0183  ......s....t.|..
-000002b0: 0164 016b 0772 1274 0183 0082 017c 0164  .d.k.r.t.....|.d
-000002c0: 0219 0089 0074 007c 0183 0164 036b 0272  .....t.|...d.k.r
-000002d0: 3864 047d 0374 027c 0164 0519 0083 017d  8d.}.t.|.d.....}
-000002e0: 046e 1064 067d 0374 027c 0164 0219 0083  .n.d.}.t.|.d....
-000002f0: 017d 047c 0464 071b 00a0 03a1 0072 7064  .}.|.d.......rpd
-00000300: 057c 005f 0474 0564 087c 04a0 06a1 009b  .|._.t.d.|......
-00000310: 009d 0283 0101 0064 0053 007c 00a0 0788  .......d.S.|....
-00000320: 00a1 0173 8464 057c 005f 0464 0053 007c  ...s.d.|._.d.S.|
-00000330: 00a0 0874 027c 006a 0983 017c 04a0 06a1  ...t.|.j...|....
-00000340: 00a1 0201 0074 0a7c 0464 091b 007c 0488  .....t.|.d...|..
-00000350: 001b 0083 0201 0074 0b44 005d 347d 0574  .......t.D.]4}.t
-00000360: 027c 0466 0187 0066 0164 0a64 0b84 087c  .|.f...f.d.d...|
-00000370: 0544 0083 019e 028e 007d 0674 0c7c 0688  .D.......}.t.|..
-00000380: 0064 0c74 0d88 0083 0164 0d8d 0401 0071  .d.t.....d.....q
-00000390: b07c 0372 fc7c 049b 0064 0e88 009b 0064  .|.r.|...d.....d
-000003a0: 0f9d 047d 076e 107c 049b 0064 0e7c 049b  ...}.n.|...d.|..
-000003b0: 0064 0f9d 047d 0774 027c 0483 01a0 06a1  .d...}.t.|......
-000003c0: 007d 0874 0e6a 0f90 0172 4674 0564 1083  .}.t.j...rFt.d..
-000003d0: 0101 0074 027c 0783 017d 0974 02a0 037c  ...t.|...}.t...|
-000003e0: 09a1 0190 0172 647c 09a0 10a1 0001 006e  .....rd|.......n
-000003f0: 1e74 0c7c 077c 0874 0d74 117c 0883 0183  .t.|.|.t.t.|....
-00000400: 0188 0074 0d88 0083 0164 118d 0501 0074  ...t.....d.....t
-00000410: 0564 1288 009b 0064 137c 006a 099b 0064  .d.....d.|.j...d
-00000420: 149d 0583 0101 0074 0564 157c 04a0 06a1  .......t.d.|....
-00000430: 009b 0064 169d 0383 0101 0074 0564 1783  ...d.......t.d..
-00000440: 0101 0074 0564 187c 049b 009d 0283 0101  ...t.d.|........
-00000450: 0074 0564 1983 0101 0074 0564 1a83 0101  .t.d.....t.d....
-00000460: 0074 0564 1b83 0101 0064 0053 0029 1c4e  .t.d.....d.S.).N
-00000470: 2902 e901 0000 00e9 0200 0000 7201 0000  )...........r...
-00000480: 0072 1000 0000 5472 0f00 0000 4672 0b00  .r....Tr....Fr..
-00000490: 0000 7a24 4572 726f 723a 2073 6372 6170  ..z$Error: scrap
-000004a0: 792e 6366 6720 616c 7265 6164 7920 6578  y.cfg already ex
-000004b0: 6973 7473 2069 6e20 da06 6d6f 6475 6c65  ists in ..module
-000004c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000004d0: 0004 0000 0033 0000 0073 2000 0000 7c00  .....3...s ...|.
-000004e0: 5d18 7d01 7400 a001 7c01 a101 6a02 8800  ].}.t...|...j...
-000004f0: 6400 8d01 5600 0100 7102 6401 5300 2902  d...V...q.d.S.).
-00000500: a901 da0c 7072 6f6a 6563 745f 6e61 6d65  ....project_name
-00000510: 4e29 03da 0673 7472 696e 67da 0854 656d  N)...string..Tem
-00000520: 706c 6174 65da 0a73 7562 7374 6974 7574  plate..substitut
-00000530: 6529 02da 022e 30da 0173 7212 0000 00a9  e)....0..sr.....
-00000540: 00fa 472f 726f 6f74 2f6d 7970 726f 6a2f  ..G/root/myproj/
-00000550: 4179 7567 6553 7069 6465 7254 6f6f 6c73  AyugeSpiderTools
-00000560: 2f61 7975 6765 7370 6964 6572 746f 6f6c  /ayugespidertool
-00000570: 732f 636f 6d6d 616e 6473 2f73 7461 7274  s/commands/start
-00000580: 7072 6f6a 6563 742e 7079 da09 3c67 656e  project.py..<gen
-00000590: 6578 7072 3e3d 0000 0073 0400 0000 0402  expr>=...s......
-000005a0: 02ff 7a21 4179 7543 6f6d 6d61 6e64 2e72  ..z!AyuCommand.r
-000005b0: 756e 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  un.<locals>.<gen
-000005c0: 6578 7072 3e7a 0324 7079 2903 7213 0000  expr>z.$py).r...
-000005d0: 00da 0270 79da 0b50 726f 6a65 6374 4e61  ...py..ProjectNa
-000005e0: 6d65 fa01 2f7a 0c2f 7275 6e2e 7368 2e74  me../z./run.sh.t
-000005f0: 6d70 6c7a 3a49 6e66 6f3a 2054 6865 2072  mplz:Info: The r
-00000600: 756e 2e73 6820 6669 6c65 2069 7320 6e6f  un.sh file is no
-00000610: 206c 6f6e 6765 7220 6765 6e65 7261 7465   longer generate
-00000620: 6420 756e 6465 7220 7769 6e64 6f77 7329  d under windows)
-00000630: 045a 1370 726f 6a65 6374 5f73 7461 7274  .Z.project_start
-00000640: 7570 5f64 6972 5a11 5072 6f6a 6563 7453  up_dirZ.ProjectS
-00000650: 7461 7274 7570 4469 7272 1300 0000 721d  tartupDirr....r.
-00000660: 0000 007a 144e 6577 2053 6372 6170 7920  ...z.New Scrapy 
-00000670: 7072 6f6a 6563 7420 277a 1d27 2c20 7573  project 'z.', us
-00000680: 696e 6720 7465 6d70 6c61 7465 2064 6972  ing template dir
-00000690: 6563 746f 7279 2027 7a0e 272c 2063 7265  ectory 'z.', cre
-000006a0: 6174 6564 2069 6e3a 7a04 2020 2020 da01  ated in:z.    ..
-000006b0: 0a7a 2559 6f75 2063 616e 2073 7461 7274  .z%You can start
-000006c0: 2079 6f75 7220 6669 7273 7420 7370 6964   your first spid
-000006d0: 6572 2077 6974 683a 7a07 2020 2020 6364  er with:z.    cd
-000006e0: 207a 2820 2020 2073 6372 6170 7920 6765   z(    scrapy ge
-000006f0: 6e73 7069 6465 7220 6578 616d 706c 6520  nspider example 
-00000700: 6578 616d 706c 652e 636f 6d7a 394f 7220  example.comz9Or 
-00000710: 796f 7520 6361 6e20 7374 6172 7420 796f  you can start yo
-00000720: 7572 2066 6972 7374 2073 7069 6465 7220  ur first spider 
-00000730: 7769 7468 2061 7975 6765 7370 6964 6572  with ayugespider
-00000740: 746f 6f6c 733a 7a32 2020 2020 6179 7567  tools:z2    ayug
-00000750: 6573 7069 6465 7274 6f6f 6c73 2067 656e  espidertools gen
-00000760: 7370 6964 6572 2065 7861 6d70 6c65 2065  spider example e
-00000770: 7861 6d70 6c65 2e63 6f6d 2912 da03 6c65  xample.com)...le
-00000780: 6e72 0600 0000 7202 0000 00da 0665 7869  nr....r......exi
-00000790: 7374 73da 0865 7869 7463 6f64 65da 0570  sts..exitcode..p
-000007a0: 7269 6e74 da07 7265 736f 6c76 655a 0e5f  rint..resolveZ._
-000007b0: 6973 5f76 616c 6964 5f6e 616d 65da 095f  is_valid_name.._
-000007c0: 636f 7079 7472 6565 da0d 7465 6d70 6c61  copytree..templa
-000007d0: 7465 735f 6469 7272 0400 0000 da13 5445  tes_dirr......TE
-000007e0: 4d50 4c41 5445 535f 544f 5f52 454e 4445  MPLATES_TO_RENDE
-000007f0: 5272 0700 0000 7208 0000 0072 0900 0000  Rr....r....r....
-00000800: da0a 4953 5f57 494e 444f 5753 da06 756e  ..IS_WINDOWS..un
-00000810: 6c69 6e6b da03 7374 7229 0ada 0473 656c  link..str)...sel
-00000820: 66da 0461 7267 73da 046f 7074 735a 155f  f..args..optsZ._
-00000830: 6861 735f 7072 6f6a 6563 745f 6469 725f  has_project_dir_
-00000840: 6172 6773 da0b 7072 6f6a 6563 745f 6469  args..project_di
-00000850: 72da 0570 6174 6873 5a07 7470 6c66 696c  r..pathsZ.tplfil
-00000860: 655a 0e72 756e 5f73 6865 6c6c 5f70 6174  eZ.run_shell_pat
-00000870: 685a 1172 756e 5f73 6865 6c6c 5f61 6273  hZ.run_shell_abs
-00000880: 7061 7468 5a08 6465 6c5f 6669 6c65 7219  pathZ.del_filer.
-00000890: 0000 0072 1200 0000 721a 0000 00da 0372  ...r....r......r
-000008a0: 756e 2200 0000 7370 0000 0000 010c 0106  un"...sp........
-000008b0: 0208 020c 0104 010e 0204 010c 020c 0106  ................
-000008c0: 0112 0104 020a 0106 0104 0216 0112 0108  ................
-000008d0: 0102 0102 ff02 020a 0202 fe04 fe06 0702  ................
-000008e0: 0102 0102 0202 0106 fb08 0904 0112 0210  ................
-000008f0: 010c 0208 0108 0108 010c 010a 0302 0102  ................
-00000900: 0102 010a 0102 0106 fb06 0802 0112 ff04  ................
-00000910: 0414 0108 010e 0108 0208 017a 0e41 7975  ...........z.Ayu
-00000920: 436f 6d6d 616e 642e 7275 6e29 01da 0672  Command.run)...r
-00000930: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-00000940: 0000 0100 0000 0500 0000 4300 0000 731a  ..........C...s.
-00000950: 0000 0074 0074 0174 0174 026a 0364 0119  ...t.t.t.t.j.d..
-00000960: 0064 0283 0264 0383 0283 0153 0029 044e  .d...d.....S.).N
-00000970: 7201 0000 00da 0974 656d 706c 6174 6573  r......templates
-00000980: da07 7072 6f6a 6563 7429 0472 2a00 0000  ..project).r*...
-00000990: 7202 0000 00da 1061 7975 6765 7370 6964  r......ayugespid
-000009a0: 6572 746f 6f6c 73da 085f 5f70 6174 685f  ertools..__path_
-000009b0: 5f29 0172 2b00 0000 7219 0000 0072 1900  _).r+...r....r..
-000009c0: 0000 721a 0000 0072 2600 0000 6c00 0000  ..r....r&...l...
-000009d0: 730c 0000 0000 0302 0102 010e 0102 fe02  s...............
-000009e0: ff7a 1841 7975 436f 6d6d 616e 642e 7465  .z.AyuCommand.te
-000009f0: 6d70 6c61 7465 735f 6469 724e 2907 da08  mplates_dirN)...
-00000a00: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000a10: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000a20: 5f5f 7230 0000 00da 0870 726f 7065 7274  __r0.....propert
-00000a30: 7972 2a00 0000 7226 0000 0072 1900 0000  yr*...r&...r....
-00000a40: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000a50: 0e00 0000 2100 0000 7306 0000 0008 0108  ....!...s.......
-00000a60: 4a02 0172 0e00 0000 2913 7214 0000 00da  J..r....).r.....
-00000a70: 0770 6174 686c 6962 7202 0000 00da 0673  .pathlibr......s
-00000a80: 6875 7469 6c72 0300 0000 7204 0000 005a  hutilr....r....Z
-00000a90: 1c73 6372 6170 792e 636f 6d6d 616e 6473  .scrapy.commands
-00000aa0: 2e73 7461 7274 7072 6f6a 6563 7472 0500  .startprojectr..
-00000ab0: 0000 da11 7363 7261 7079 2e65 7863 6570  ....scrapy.excep
-00000ac0: 7469 6f6e 7372 0600 0000 da15 7363 7261  tionsr......scra
-00000ad0: 7079 2e75 7469 6c73 2e74 656d 706c 6174  py.utils.templat
-00000ae0: 6572 0700 0000 7208 0000 0072 3400 0000  er....r....r4...
-00000af0: da1e 6179 7567 6573 7069 6465 7274 6f6f  ..ayugespidertoo
-00000b00: 6c73 2e63 6f6d 6d6f 6e2e 5061 7261 6d73  ls.common.Params
-00000b10: 7209 0000 0072 2700 0000 5a06 4947 4e4f  r....r'...Z.IGNO
-00000b20: 5245 720e 0000 0072 1900 0000 7219 0000  REr....r....r...
-00000b30: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
-00000b40: 6475 6c65 3e01 0000 0073 1400 0000 0801  dule>....s......
-00000b50: 0c01 1002 0c01 0c01 1002 0801 0c03 0411  ................
-00000b60: 0c03                                     ..
+00000200: 6c7a 052a 2e70 7963 da0b 5f5f 7079 6361  lz.*.pyc..__pyca
+00000210: 6368 655f 5f7a 042e 7376 6e63 0000 0000  che__z..svnc....
+00000220: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000230: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
+00000240: 0264 0164 0284 005a 0365 0465 0564 039c  .d.d...Z.e.e.d..
+00000250: 0164 0464 0584 0483 015a 0664 0653 0029  .d.d.....Z.d.S.)
+00000260: 07da 0a41 7975 436f 6d6d 616e 6463 0300  ...AyuCommandc..
+00000270: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
+00000280: 0000 0300 0000 73c2 0100 0074 007c 0183  ......s....t.|..
+00000290: 0164 016b 0772 1274 0183 0082 017c 0164  .d.k.r.t.....|.d
+000002a0: 0219 0089 0074 007c 0183 0164 036b 0272  .....t.|...d.k.r
+000002b0: 3864 047d 0374 027c 0164 0519 0083 017d  8d.}.t.|.d.....}
+000002c0: 046e 1064 067d 0374 027c 0164 0219 0083  .n.d.}.t.|.d....
+000002d0: 017d 047c 0464 071b 00a0 03a1 0072 7064  .}.|.d.......rpd
+000002e0: 057c 005f 0474 0564 087c 04a0 06a1 009b  .|._.t.d.|......
+000002f0: 009d 0283 0101 0064 0053 007c 00a0 0788  .......d.S.|....
+00000300: 00a1 0173 8464 057c 005f 0464 0053 007c  ...s.d.|._.d.S.|
+00000310: 00a0 0874 027c 006a 0983 017c 04a0 06a1  ...t.|.j...|....
+00000320: 00a1 0201 0074 0a7c 0464 091b 007c 0488  .....t.|.d...|..
+00000330: 001b 0083 0201 0074 0b44 005d 347d 0574  .......t.D.]4}.t
+00000340: 027c 0466 0187 0066 0164 0a64 0b84 087c  .|.f...f.d.d...|
+00000350: 0544 0083 019e 028e 007d 0674 0c7c 0688  .D.......}.t.|..
+00000360: 0064 0c74 0d88 0083 0164 0d8d 0401 0071  .d.t.....d.....q
+00000370: b07c 0372 fc7c 049b 0064 0e88 009b 0064  .|.r.|...d.....d
+00000380: 0f9d 047d 076e 107c 049b 0064 0e7c 049b  ...}.n.|...d.|..
+00000390: 0064 0f9d 047d 0774 027c 0483 01a0 06a1  .d...}.t.|......
+000003a0: 007d 0874 0e6a 0f90 0172 4674 0564 1083  .}.t.j...rFt.d..
+000003b0: 0101 0074 027c 0783 017d 0974 02a0 037c  ...t.|...}.t...|
+000003c0: 09a1 0190 0172 647c 09a0 10a1 0001 006e  .....rd|.......n
+000003d0: 1e74 0c7c 077c 0874 0d74 117c 0883 0183  .t.|.|.t.t.|....
+000003e0: 0188 0074 0d88 0083 0164 118d 0501 0074  ...t.....d.....t
+000003f0: 0564 1288 009b 0064 137c 006a 099b 0064  .d.....d.|.j...d
+00000400: 149d 0583 0101 0074 0564 157c 04a0 06a1  .......t.d.|....
+00000410: 009b 0064 169d 0383 0101 0074 0564 1783  ...d.......t.d..
+00000420: 0101 0074 0564 187c 049b 009d 0283 0101  ...t.d.|........
+00000430: 0074 0564 1983 0101 0074 0564 1a83 0101  .t.d.....t.d....
+00000440: 0074 0564 1b83 0101 0064 0053 0029 1c4e  .t.d.....d.S.).N
+00000450: 2902 e901 0000 00e9 0200 0000 7201 0000  )...........r...
+00000460: 0072 1000 0000 5472 0f00 0000 4672 0b00  .r....Tr....Fr..
+00000470: 0000 7a24 4572 726f 723a 2073 6372 6170  ..z$Error: scrap
+00000480: 792e 6366 6720 616c 7265 6164 7920 6578  y.cfg already ex
+00000490: 6973 7473 2069 6e20 da06 6d6f 6475 6c65  ists in ..module
+000004a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000004b0: 0004 0000 0033 0000 0073 2000 0000 7c00  .....3...s ...|.
+000004c0: 5d18 7d01 7400 a001 7c01 a101 6a02 8800  ].}.t...|...j...
+000004d0: 6400 8d01 5600 0100 7102 6401 5300 2902  d...V...q.d.S.).
+000004e0: a901 da0c 7072 6f6a 6563 745f 6e61 6d65  ....project_name
+000004f0: 4e29 03da 0673 7472 696e 67da 0854 656d  N)...string..Tem
+00000500: 706c 6174 65da 0a73 7562 7374 6974 7574  plate..substitut
+00000510: 6529 02da 022e 30da 0173 7212 0000 00a9  e)....0..sr.....
+00000520: 00fa 472f 726f 6f74 2f6d 7970 726f 6a2f  ..G/root/myproj/
+00000530: 4179 7567 6553 7069 6465 7254 6f6f 6c73  AyugeSpiderTools
+00000540: 2f61 7975 6765 7370 6964 6572 746f 6f6c  /ayugespidertool
+00000550: 732f 636f 6d6d 616e 6473 2f73 7461 7274  s/commands/start
+00000560: 7072 6f6a 6563 742e 7079 da09 3c67 656e  project.py..<gen
+00000570: 6578 7072 3e3b 0000 0073 0400 0000 0402  expr>;...s......
+00000580: 02ff 7a21 4179 7543 6f6d 6d61 6e64 2e72  ..z!AyuCommand.r
+00000590: 756e 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  un.<locals>.<gen
+000005a0: 6578 7072 3e7a 0324 7079 2903 7213 0000  expr>z.$py).r...
+000005b0: 00da 0270 79da 0b50 726f 6a65 6374 4e61  ...py..ProjectNa
+000005c0: 6d65 fa01 2f7a 0c2f 7275 6e2e 7368 2e74  me../z./run.sh.t
+000005d0: 6d70 6c7a 3a49 6e66 6f3a 2054 6865 2072  mplz:Info: The r
+000005e0: 756e 2e73 6820 6669 6c65 2069 7320 6e6f  un.sh file is no
+000005f0: 206c 6f6e 6765 7220 6765 6e65 7261 7465   longer generate
+00000600: 6420 756e 6465 7220 7769 6e64 6f77 7329  d under windows)
+00000610: 045a 1370 726f 6a65 6374 5f73 7461 7274  .Z.project_start
+00000620: 7570 5f64 6972 5a11 5072 6f6a 6563 7453  up_dirZ.ProjectS
+00000630: 7461 7274 7570 4469 7272 1300 0000 721d  tartupDirr....r.
+00000640: 0000 007a 144e 6577 2053 6372 6170 7920  ...z.New Scrapy 
+00000650: 7072 6f6a 6563 7420 277a 1d27 2c20 7573  project 'z.', us
+00000660: 696e 6720 7465 6d70 6c61 7465 2064 6972  ing template dir
+00000670: 6563 746f 7279 2027 7a0e 272c 2063 7265  ectory 'z.', cre
+00000680: 6174 6564 2069 6e3a 7a04 2020 2020 da01  ated in:z.    ..
+00000690: 0a7a 2559 6f75 2063 616e 2073 7461 7274  .z%You can start
+000006a0: 2079 6f75 7220 6669 7273 7420 7370 6964   your first spid
+000006b0: 6572 2077 6974 683a 7a07 2020 2020 6364  er with:z.    cd
+000006c0: 207a 2820 2020 2073 6372 6170 7920 6765   z(    scrapy ge
+000006d0: 6e73 7069 6465 7220 6578 616d 706c 6520  nspider example 
+000006e0: 6578 616d 706c 652e 636f 6d7a 394f 7220  example.comz9Or 
+000006f0: 796f 7520 6361 6e20 7374 6172 7420 796f  you can start yo
+00000700: 7572 2066 6972 7374 2073 7069 6465 7220  ur first spider 
+00000710: 7769 7468 2061 7975 6765 7370 6964 6572  with ayugespider
+00000720: 746f 6f6c 733a 7a27 2020 2020 6179 7567  tools:z'    ayug
+00000730: 6520 6765 6e73 7069 6465 7220 6578 616d  e genspider exam
+00000740: 706c 6520 6578 616d 706c 652e 636f 6d29  ple example.com)
+00000750: 12da 036c 656e 7206 0000 0072 0200 0000  ...lenr....r....
+00000760: da06 6578 6973 7473 da08 6578 6974 636f  ..exists..exitco
+00000770: 6465 da05 7072 696e 74da 0772 6573 6f6c  de..print..resol
+00000780: 7665 5a0e 5f69 735f 7661 6c69 645f 6e61  veZ._is_valid_na
+00000790: 6d65 da09 5f63 6f70 7974 7265 65da 0d74  me.._copytree..t
+000007a0: 656d 706c 6174 6573 5f64 6972 7204 0000  emplates_dirr...
+000007b0: 00da 1354 454d 504c 4154 4553 5f54 4f5f  ...TEMPLATES_TO_
+000007c0: 5245 4e44 4552 7207 0000 0072 0800 0000  RENDERr....r....
+000007d0: 7209 0000 00da 0a49 535f 5749 4e44 4f57  r......IS_WINDOW
+000007e0: 53da 0675 6e6c 696e 6bda 0373 7472 290a  S..unlink..str).
+000007f0: da04 7365 6c66 da04 6172 6773 da04 6f70  ..self..args..op
+00000800: 7473 5a15 5f68 6173 5f70 726f 6a65 6374  tsZ._has_project
+00000810: 5f64 6972 5f61 7267 735a 0b70 726f 6a65  _dir_argsZ.proje
+00000820: 6374 5f64 6972 da05 7061 7468 735a 0774  ct_dir..pathsZ.t
+00000830: 706c 6669 6c65 5a0e 7275 6e5f 7368 656c  plfileZ.run_shel
+00000840: 6c5f 7061 7468 5a11 7275 6e5f 7368 656c  l_pathZ.run_shel
+00000850: 6c5f 6162 7370 6174 685a 0864 656c 5f66  l_abspathZ.del_f
+00000860: 696c 6572 1900 0000 7212 0000 0072 1a00  iler....r....r..
+00000870: 0000 da03 7275 6e20 0000 0073 7000 0000  ....run ...sp...
+00000880: 0001 0c01 0602 0802 0c01 0401 0e02 0401  ................
+00000890: 0c02 0c01 0601 1201 0402 0a01 0601 0402  ................
+000008a0: 1601 1201 0801 0201 02ff 0202 0a02 02fe  ................
+000008b0: 04fe 0607 0201 0201 0202 0201 06fb 0809  ................
+000008c0: 0401 1202 1001 0c02 0801 0801 0801 0c01  ................
+000008d0: 0a03 0201 0201 0201 0a01 0201 06fb 0608  ................
+000008e0: 0201 12ff 0404 1401 0801 0e01 0802 0801  ................
+000008f0: 7a0e 4179 7543 6f6d 6d61 6e64 2e72 756e  z.AyuCommand.run
+00000900: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
+00000910: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00000920: 0000 0073 1a00 0000 7400 7401 7401 7402  ...s....t.t.t.t.
+00000930: 6a03 6401 1900 6402 8302 6403 8302 8301  j.d...d...d.....
+00000940: 5300 2904 4e72 0100 0000 da09 7465 6d70  S.).Nr......temp
+00000950: 6c61 7465 73da 0770 726f 6a65 6374 2904  lates..project).
+00000960: 722a 0000 0072 0200 0000 da10 6179 7567  r*...r......ayug
+00000970: 6573 7069 6465 7274 6f6f 6c73 da08 5f5f  espidertools..__
+00000980: 7061 7468 5f5f 2901 722b 0000 0072 1900  path__).r+...r..
+00000990: 0000 7219 0000 0072 1a00 0000 7226 0000  ..r....r....r&..
+000009a0: 006a 0000 0073 0c00 0000 0003 0201 0201  .j...s..........
+000009b0: 0e01 02fe 02ff 7a18 4179 7543 6f6d 6d61  ......z.AyuComma
+000009c0: 6e64 2e74 656d 706c 6174 6573 5f64 6972  nd.templates_dir
+000009d0: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000009e0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000009f0: 6c6e 616d 655f 5f72 2f00 0000 da08 7072  lname__r/.....pr
+00000a00: 6f70 6572 7479 722a 0000 0072 2600 0000  opertyr*...r&...
+00000a10: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000a20: 1a00 0000 720e 0000 001f 0000 0073 0600  ....r........s..
+00000a30: 0000 0801 084a 0201 720e 0000 0029 1372  .....J..r....).r
+00000a40: 1400 0000 da07 7061 7468 6c69 6272 0200  ......pathlibr..
+00000a50: 0000 da06 7368 7574 696c 7203 0000 0072  ....shutilr....r
+00000a60: 0400 0000 5a1c 7363 7261 7079 2e63 6f6d  ....Z.scrapy.com
+00000a70: 6d61 6e64 732e 7374 6172 7470 726f 6a65  mands.startproje
+00000a80: 6374 7205 0000 00da 1173 6372 6170 792e  ctr......scrapy.
+00000a90: 6578 6365 7074 696f 6e73 7206 0000 00da  exceptionsr.....
+00000aa0: 1573 6372 6170 792e 7574 696c 732e 7465  .scrapy.utils.te
+00000ab0: 6d70 6c61 7465 7207 0000 0072 0800 0000  mplater....r....
+00000ac0: 7233 0000 00da 1e61 7975 6765 7370 6964  r3.....ayugespid
+00000ad0: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e70  ertools.common.p
+00000ae0: 6172 616d 7372 0900 0000 7227 0000 005a  aramsr....r'...Z
+00000af0: 0649 474e 4f52 4572 0e00 0000 7219 0000  .IGNOREr....r...
+00000b00: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000b10: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
+00000b20: 0000 0008 010c 0110 020c 010c 0110 0208  ................
+00000b30: 010c 0304 0f0c 03                        .......
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/startproject.py` & `ayugespidertools-2.0.1/ayugespidertools/commands/startproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from shutil import ignore_patterns, move
 
 from scrapy.commands.startproject import Command
 from scrapy.exceptions import UsageError
 from scrapy.utils.template import render_templatefile, string_camelcase
 
 import ayugespidertools
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.params import Param
 
 # 添加需要的自定义配置文件
 TEMPLATES_TO_RENDER = (
     (".gitignore",),
     ("pyproject.toml",),
     ("README.md",),
     ("requirements.txt",),
@@ -19,16 +19,14 @@
     ("scrapy.cfg",),
     ("${project_name}", "settings.py.tmpl"),
     ("${project_name}", "items.py.tmpl"),
     ("${project_name}", "pipelines.py.tmpl"),
     ("${project_name}", "middlewares.py.tmpl"),
     # 添加 run.py 总运行文件
     ("${project_name}", "run.py.tmpl"),
-    # 渲染 common 文件夹下的 DataEnum.py 模板
-    ("${project_name}", "common/DataEnum.py.tmpl"),
 )
 
 IGNORE = ignore_patterns("*.pyc", "__pycache__", ".svn")
 
 
 class AyuCommand(Command):
     def run(self, args, opts):
@@ -99,15 +97,15 @@
         )
         print(f"    {project_dir.resolve()}\n")
         print("You can start your first spider with:")
         print(f"    cd {project_dir}")
         print("    scrapy genspider example example.com")
         # 添加本库的文字提示内容
         print("Or you can start your first spider with ayugespidertools:")
-        print("    ayugespidertools genspider example example.com")
+        print("    ayuge genspider example example.com")
 
     @property
     def templates_dir(self) -> str:
         # 修改 startproject 模板文件路径为 ayugespidertools 的自定义路径
         return str(
             Path(
                 Path(ayugespidertools.__path__[0], "templates"),
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/commands/version.py` & `ayugespidertools-2.0.1/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/Encryption.py` & `ayugespidertools-2.0.1/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/Expend.py` & `ayugespidertools-2.0.1/ayugespidertools/common/expend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 
 import pymysql
 from retrying import retry
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import MysqlConfig
 from ayugespidertools.config import logger
 
 __all__ = [
     "MysqlPipeEnhanceMixin",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/MongoDBPipe.py` & `ayugespidertools-2.0.1/ayugespidertools/common/mongodbpipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from abc import ABC, abstractmethod
 
 from itemadapter import ItemAdapter
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
 
 __all__ = [
     "Synchronize",
     "TwistedAsynchronous",
     "mongodb_pipe",
 ]
 
 
 class AbstractClass(ABC):
     """
-    用于处理 mysql 异常的模板方法类
+    用于处理 mongodb pipeline 存储的模板方法类
     """
 
     def _get_collection_name(self, table: str, collection_prefix: str = "") -> str:
         """
         获取集合名称
         Args:
             table: item 中的 table 字段
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/MultiPlexing.py` & `ayugespidertools-2.0.1/ayugespidertools/common/multiplexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import cv2
 import numpy as np
 import pymysql
 from scrapy.settings import Settings
 from twisted.internet.defer import Deferred
 
-from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.common.typevars import MysqlConfig
 from ayugespidertools.config import logger
 
 __all__ = [
     "ReuseOperation",
 ]
 
 
@@ -275,17 +275,16 @@
         Args:
             settings: scrapy 的 settings 信息
 
         Returns:
             consul_conf_dict_min: 满足要求的最少要求的 consul 配置
         """
         consul_conf_dict = settings.get("CONSUL_CONFIG", {})
-        consul_conf_dict_lowered = cls.dict_keys_to_lower(consul_conf_dict)
         return cls.get_items_by_keys(
-            dict_conf=consul_conf_dict_lowered, key_list=["token", "url", "format"]
+            dict_conf=consul_conf_dict, key_list=["token", "url", "format"]
         )
 
     @classmethod
     def judge_str_is_json(cls, judge_str: str) -> bool:
         """
         判断字符串是否为 json 格式
         Args:
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/MysqlErrorHandle.py` & `ayugespidertools-2.0.1/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Optional, Type, Union
 
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import TableEnumTypeVar
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import TableEnumTypeVar
 from ayugespidertools.config import logger
 
 __all__ = [
     "Synchronize",
     "TwistedAsynchronous",
     "deal_mysql_err",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/Params.py` & `ayugespidertools-2.0.1/ayugespidertools/common/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import platform
 import random
 from typing import List, TypeVar
 
+# 用于 type hint，不要删除
 import pymongo
 import pymysql
+from itemadapter import ItemAdapter
 
-from ayugespidertools.Items import MongoDataItem, MysqlDataItem, ScrapyClassicItem
+from ayugespidertools.items import MongoDataItem, MysqlDataItem, ScrapyClassicItem
 
 __all__ = [
     "Param",
 ]
 
 
 class Param:
@@ -23,14 +25,15 @@
     B_Str = TypeVar("B_Str", bytes, str)
     I_Str_N = TypeVar("I_Str_N", int, str, NoneType)
     Str_Lstr = TypeVar("Str_Lstr", str, List[str])
     PymongoDataBase = TypeVar("PymongoDataBase", bound="pymongo.database.Database")
     PymysqlConnect = TypeVar("PymysqlConnect", bound="pymysql.connections.Connection")
     PymysqlCursor = TypeVar("PymysqlCursor", bound="pymysql.cursors.Cursor")
     PymysqlDictCursor = TypeVar("PymysqlDictCursor", bound="pymysql.cursors.DictCursor")
+    ItemAdapterType = TypeVar("ItemAdapterType", bound="ItemAdapter")
     # 此框架中 Item 的类型种类
     ScrapyItems = TypeVar(
         "ScrapyItems", MysqlDataItem, MongoDataItem, ScrapyClassicItem
     )
 
     # 基本的请求头
     base_headers = {
@@ -54,34 +57,34 @@
     requests_time_sleep_random = random.choice(requests_time_sleep_list)
 
     # aiohttp 连接超时，响应时间超时，随机休眠间隔等设置
     aiohttp_req_timeout = 1
     aiohttp_res_timeout = 1
     aiohttp_time_sleep_list = [x / 10 for x in range(5, 19)]
     aiohttp_time_sleep_random = random.choice(aiohttp_time_sleep_list)
-    aiohttp_timeout_default = 5
+    aiohttp_timeout_default = 25
     aiohttp_sleep_default = 1
     aiohttp_retry_times_default = 3
 
     # 部署运行的平台为 win 或 linux
     IS_WINDOWS = platform.system().lower() == "windows"
     IS_LINUX = platform.system().lower() == "linux"
 
     # 动态隧道代理配置示例
     dynamic_proxy_conf_example = {
-        "PROXY_URL": "动态隧道代理地址：***.***.com:*****",
-        "USERNAME": "隧道代理用户名",
-        "PASSWORD": "对应用户的密码",
+        "proxy": "动态隧道代理地址：***.***.com:*****",
+        "username": "隧道代理用户名",
+        "password": "对应用户的密码",
     }
     # 独享代理配置示例
     exclusive_proxy_conf_example = {
-        "PROXY_URL": "独享代理地址：'http://***.com/api/***&num=100&format=json'",
-        "USERNAME": "独享代理用户名",
-        "PASSWORD": "对应用户的密码",
-        "PROXY_INDEX": "需要返回的独享代理的索引",
+        "proxy": "独享代理地址：'http://***.com/api/***&num=100&format=json'",
+        "username": "独享代理用户名",
+        "password": "对应用户的密码",
+        "index": "需要返回的独享代理的索引",
     }
 
     # aiohttp 配置示例
     aiohttp_conf_example = {
         "timeout": 5,
         "proxy": "127.0.0.1:80",
         "sleep": 1,
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/SpiderDBConf.py` & `ayugespidertools-2.0.1/ayugespidertools/common/spiderdbconf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Union
 
 from scrapy.settings import Settings
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.TypeVars import MongoDBConfig, MysqlConfig
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.typevars import MongoDBConfig, MysqlConfig
+from ayugespidertools.common.utils import ToolsForAyu
 
 __all__ = [
     "get_spider_db_conf",
     "MysqlConfCreator",
     "MongoDBConfCreator",
 ]
 
@@ -35,71 +35,71 @@
         self._consul_conf = consul_conf
 
     def get_db_conn_conf(self) -> Union[MysqlConfig, None]:
         # 自定义 mysql 链接配置
         local_mysql_conf = self._settings.get("LOCAL_MYSQL_CONFIG", {})
         # 是否开启应用配置管理
         app_conf_manage = self._settings.get("APP_CONF_MANAGE", False)
-        if all([not local_mysql_conf.get("DATABASE"), not app_conf_manage]):
+        if all([not local_mysql_conf.get("database"), not app_conf_manage]):
             return None
 
         # 1). 如果开启应用管理，从 consul 中获取应用配置
         if app_conf_manage:
             _consul_conf_dict = ToolsForAyu.get_conf_by_consul(
-                conf_name="MYSQL", **self._consul_conf
+                conf_name="mysql", **self._consul_conf
             )
             return MysqlConfig(**_consul_conf_dict)
 
         # 2). 从本地 local_mysql_config 的参数中取值
         if ReuseOperation.is_dict_meet_min_limit(
             dict_conf=local_mysql_conf,
-            key_list=["HOST", "PORT", "USER", "PASSWORD", "CHARSET", "DATABASE"],
+            key_list=["host", "port", "user", "password", "charset", "database"],
         ):
             return MysqlConfig(
-                host=local_mysql_conf.get("HOST"),
-                port=local_mysql_conf.get("PORT"),
-                user=local_mysql_conf.get("USER"),
-                password=local_mysql_conf.get("PASSWORD"),
-                database=local_mysql_conf.get("DATABASE"),
-                charset=local_mysql_conf.get("CHARSET") or "utf8mb4",
+                host=local_mysql_conf.get("host"),
+                port=local_mysql_conf.get("port"),
+                user=local_mysql_conf.get("user"),
+                password=local_mysql_conf.get("password"),
+                database=local_mysql_conf.get("database"),
+                charset=local_mysql_conf.get("charset") or "utf8mb4",
             )
 
 
 class MongoDBConfProduct(Product):
     def __init__(self, settings, consul_conf):
         self._settings = settings
         self._consul_conf = consul_conf
 
     def get_db_conn_conf(self) -> Union[MongoDBConfig, None]:
         # 自定义 mysql 链接配置
         local_mongodb_conf = self._settings.get("LOCAL_MONGODB_CONFIG", {})
         # 是否开启应用配置管理
         app_conf_manage = self._settings.get("APP_CONF_MANAGE", False)
-        if all([not local_mongodb_conf.get("DATABASE"), not app_conf_manage]):
+        if all([not local_mongodb_conf.get("database"), not app_conf_manage]):
             return None
 
         # 1). 如果开启应用管理，从 consul 中获取应用配置
         if app_conf_manage:
             _consul_conf_dict = ToolsForAyu.get_conf_by_consul(
-                conf_name="MONGODB", **self._consul_conf
+                conf_name="mongodb", **self._consul_conf
             )
             return MongoDBConfig(**_consul_conf_dict)
 
         # 2). 从本地 local_mongo_conf 的参数中取值
         if ReuseOperation.is_dict_meet_min_limit(
             dict_conf=local_mongodb_conf,
-            key_list=["HOST", "PORT", "USER", "PASSWORD", "DATABASE"],
+            key_list=["host", "port", "user", "password", "database"],
         ):
             return MongoDBConfig(
-                host=local_mongodb_conf.get("HOST"),
-                port=local_mongodb_conf.get("PORT"),
-                user=local_mongodb_conf.get("USER"),
-                password=local_mongodb_conf.get("PASSWORD"),
-                database=local_mongodb_conf.get("DATABASE"),
-                authsource=local_mongodb_conf.get("AUTHSOURCE"),
+                host=local_mongodb_conf.get("host"),
+                port=local_mongodb_conf.get("port"),
+                user=local_mongodb_conf.get("user"),
+                password=local_mongodb_conf.get("password"),
+                database=local_mongodb_conf.get("database"),
+                authsource=local_mongodb_conf.get("authsource"),
             )
 
 
 class MysqlConfCreator(Creator):
     def create_product(self, settings: Settings, consul_conf: dict) -> Product:
         return MysqlConfProduct(settings, consul_conf)
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/SqlFormat.py` & `ayugespidertools-2.0.1/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/Utils.py` & `ayugespidertools-2.0.1/ayugespidertools/common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import copy
 import json
 import xml.etree.ElementTree as ET
-from typing import List, Literal, Optional, Union
+from typing import Any, List, Literal, Optional, Union
 from urllib.parse import urlparse
 
 import hcl2
 import pandas
 import requests
 import yaml
 from itemadapter import ItemAdapter
 
-from ayugespidertools.common.Encryption import EncryptOperation
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.common.encryption import EncryptOperation
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import MysqlConfig
 from ayugespidertools.config import logger
-from ayugespidertools.FormatData import DataHandle
+from ayugespidertools.formatdata import DataHandle
 
 __all__ = [
     "ToolsForAyu",
 ]
 
 ConsulFormatStr = Literal["json", "hcl", "yaml", "xml"]
-ConsulConfNameStr = Literal["MONGODB", "MYSQL"]
+ConsulConfNameStr = Literal["mongodb", "mysql"]
 
 
 class ToolsForAyu(object):
     """
     这里用于存放框架所依赖的方法
     """
 
@@ -102,18 +102,19 @@
             for child in root:
                 conf_data[child.tag] = {}
                 for sub_child in child:
                     conf_data[child.tag][sub_child.tag] = sub_child.text
         else:
             raise ValueError("consul 暂不支持该格式的配置")
 
+        conf_data = ReuseOperation.dict_keys_to_lower(conf_data)
         _conf = conf_data.get(conf_name, {})
         if not _conf:
             logger.info(f"consul 中未设置 {conf_name} 的配置信息")
-        return ReuseOperation.dict_keys_to_lower(_conf)
+        return _conf
 
     @classmethod
     @DataHandle.simple_deal_for_extract
     def extract_with_css(
         cls, response, query: str, get_all: bool = False, return_selector: bool = False
     ):
         """
@@ -250,14 +251,27 @@
 
         Returns:
             1). 转换的 ItemAdapter 结果，可以通过  obj["params"] 或 obj.get("params") 来取值
         """
         return ItemAdapter(item)
 
     @staticmethod
+    def first_not_none(data_lst: List[Any]) -> Any:
+        """
+        获取列表中第一个不为 None 的值
+        Args:
+            data_lst: 数据列表
+
+        Returns:
+            1). 第一个不为 None 的值
+        """
+        _res = [x for x in data_lst if x is not None]
+        return _res[0] if _res else None
+
+    @staticmethod
     def get_dict_form_scrapy_req_headers(scrapy_headers) -> dict:
         """
         根据 scrapy request 中的 headers 信息转化为正常的 dict 格式
         Args:
             scrapy_headers: scrapy 的 request headers 内容
 
         Returns:
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/common/YiDunGap.py` & `ayugespidertools-2.0.1/ayugespidertools/common/yidungap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 
 import cv2
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.multiplexing import ReuseOperation
 
 __all__ = [
     "YiDunGetGap",
 ]
 
 
 class YiDunGetGap(object):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-import copy
-from typing import Callable, List, Optional, Union
-
-from scrapy import Request
-
-from ayugespidertools.common.Params import Param
-
-__all__ = [
-    "AiohttpRequest",
-]
-
-
-class AiohttpRequest(Request):
-    """
-    为 scrapy 的 Request 对象添加额外的参数
-    """
-
-    def __init__(
-        self,
-        url: str,
-        callback: Optional[Callable] = None,
-        method: str = "GET",
-        headers: Optional[dict] = None,
-        body: Optional[Union[bytes, str]] = None,
-        cookies: Optional[Union[dict, List[dict]]] = None,
-        meta: Optional[dict] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        # 用 meta 缓存 scrapy meta 的参数
-        meta = copy.deepcopy(meta) or {}
-        aiohttp_meta = meta.get("aiohttp_args") or {}
-
-        # TODO: 可添加和修改默认参数的值，后续可以在此完善功能
-        self.proxy = aiohttp_meta.get("proxy", {"http:": "http://10.10.10.10:10000"})
-        self.timeout = aiohttp_meta.get("timeout", Param.aiohttp_req_timeout)
-        self.sleep = aiohttp_meta.get("sleep", None)
-
-        aiohttp_meta = meta.setdefault("aiohttp_args", {})
-        aiohttp_meta["proxy"] = self.proxy
-        aiohttp_meta["timeout"] = self.timeout
-        super(AiohttpRequest, self).__init__(
-            url,
-            callback,
-            method=method,
-            headers=headers,
-            body=body,
-            cookies=cookies,
-            meta=meta,
-            *args,
-            **kwargs,
-        )
+import copy
+from dataclasses import asdict
+from typing import Callable, List, Optional, Union
+
+from scrapy import Request
+
+from ayugespidertools.common.typevars import AiohttpRequestArgs
+
+__all__ = [
+    "AiohttpRequest",
+]
+
+
+class AiohttpRequest(Request):
+    """
+    为 scrapy 的 Request 对象添加额外的参数
+    """
+
+    def __init__(
+        self,
+        url: str,
+        callback: Optional[Callable] = None,
+        method: str = "GET",
+        headers: Optional[dict] = None,
+        body: Optional[Union[bytes, str]] = None,
+        cookies: Optional[Union[dict, List[dict]]] = None,
+        meta: Optional[dict] = None,
+        args: Union[AiohttpRequestArgs, dict] = None,
+        **kwargs,
+    ) -> None:
+        # 用 meta 缓存 scrapy meta 的参数
+        meta = copy.deepcopy(meta) or {}
+        aiohttp_meta = meta.setdefault("aiohttp", {})
+
+        _args = {"url": url}
+        if isinstance(args, AiohttpRequestArgs):
+            args = asdict(args)
+        _args.update(args or {})
+        _args.update(aiohttp_meta.get("args", {}))
+        aiohttp_meta["args"] = _args
+
+        super(AiohttpRequest, self).__init__(
+            url,
+            callback,
+            method=method,
+            headers=headers,
+            body=body,
+            cookies=cookies,
+            meta=meta,
+            **kwargs,
+        )
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-2.0.1/ayugespidertools/middlewares.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Define here the models for your spider middleware
-#
-# See documentation in:
-# https://docs.scrapy.org/en/latest/topics/spider-middleware.html
 from ayugespidertools.scraper.middlewares.headers.ua import RandomRequestUaMiddleware
+from ayugespidertools.scraper.middlewares.netlib.aiohttplib import (
+    AiohttpAsyncDownloaderMiddleware,
+    AiohttpDownloaderMiddleware,
+)
 from ayugespidertools.scraper.middlewares.netlib.requestslib import (
-    RequestByRequestsMiddleware,
+    RequestsDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.dynamic import (
     AbuDynamicProxyDownloaderMiddleware,
     DynamicProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.exclusive import (
     ExclusiveProxyDownloaderMiddleware,
 )
-from ayugespidertools.scraper.middlewares.proxy.private import (
-    PrivateProxyDownloaderMiddleware,
-)
 
 __all__ = [
     "RandomRequestUaMiddleware",
-    "RequestByRequestsMiddleware",
-    "DynamicProxyDownloaderMiddleware",
+    "AiohttpAsyncDownloaderMiddleware",
+    "AiohttpDownloaderMiddleware",
+    "RequestsDownloaderMiddleware",
     "AbuDynamicProxyDownloaderMiddleware",
+    "DynamicProxyDownloaderMiddleware",
     "ExclusiveProxyDownloaderMiddleware",
-    "PrivateProxyDownloaderMiddleware",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Feb 28 02:20:41 2023 UTC, .py size: 970 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-00000000: 550d 0d0a 0000 0000 f964 fd63 ca03 0000  U........d.c....
+00000000: 550d 0d0a 0000 0000 93e8 4564 ab04 0000  U.........Ed....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000020: 0008 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
-00000070: 6407 6408 6409 640a 640b 6706 5a0b 640c  d.d.d.d.d.g.Z.d.
-00000080: 5300 290d e900 0000 0029 01da 1952 616e  S.)......)...Ran
-00000090: 646f 6d52 6571 7565 7374 5561 4d69 6464  domRequestUaMidd
-000000a0: 6c65 7761 7265 2901 da1b 5265 7175 6573  leware)...Reques
-000000b0: 7442 7952 6571 7565 7374 734d 6964 646c  tByRequestsMiddl
-000000c0: 6577 6172 6529 02da 2341 6275 4479 6e61  eware)..#AbuDyna
-000000d0: 6d69 6350 726f 7879 446f 776e 6c6f 6164  micProxyDownload
-000000e0: 6572 4d69 6464 6c65 7761 7265 da20 4479  erMiddleware. Dy
-000000f0: 6e61 6d69 6350 726f 7879 446f 776e 6c6f  namicProxyDownlo
-00000100: 6164 6572 4d69 6464 6c65 7761 7265 2901  aderMiddleware).
-00000110: da22 4578 636c 7573 6976 6550 726f 7879  ."ExclusiveProxy
-00000120: 446f 776e 6c6f 6164 6572 4d69 6464 6c65  DownloaderMiddle
-00000130: 7761 7265 2901 da20 5072 6976 6174 6550  ware).. PrivateP
-00000140: 726f 7879 446f 776e 6c6f 6164 6572 4d69  roxyDownloaderMi
-00000150: 6464 6c65 7761 7265 7202 0000 0072 0300  ddlewarer....r..
-00000160: 0000 7205 0000 0072 0400 0000 7206 0000  ..r....r....r...
-00000170: 0072 0700 0000 4e29 0cda 2f61 7975 6765  .r....N)../ayuge
-00000180: 7370 6964 6572 746f 6f6c 732e 7363 7261  spidertools.scra
-00000190: 7065 722e 6d69 6464 6c65 7761 7265 732e  per.middlewares.
-000001a0: 6865 6164 6572 732e 7561 7202 0000 00da  headers.uar.....
-000001b0: 3761 7975 6765 7370 6964 6572 746f 6f6c  7ayugespidertool
-000001c0: 732e 7363 7261 7065 722e 6d69 6464 6c65  s.scraper.middle
-000001d0: 7761 7265 732e 6e65 746c 6962 2e72 6571  wares.netlib.req
-000001e0: 7565 7374 736c 6962 7203 0000 00da 3261  uestslibr.....2a
-000001f0: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
-00000200: 7363 7261 7065 722e 6d69 6464 6c65 7761  scraper.middlewa
-00000210: 7265 732e 7072 6f78 792e 6479 6e61 6d69  res.proxy.dynami
-00000220: 6372 0400 0000 7205 0000 00da 3461 7975  cr....r.....4ayu
-00000230: 6765 7370 6964 6572 746f 6f6c 732e 7363  gespidertools.sc
-00000240: 7261 7065 722e 6d69 6464 6c65 7761 7265  raper.middleware
-00000250: 732e 7072 6f78 792e 6578 636c 7573 6976  s.proxy.exclusiv
-00000260: 6572 0600 0000 5a32 6179 7567 6573 7069  er....Z2ayugespi
-00000270: 6465 7274 6f6f 6c73 2e73 6372 6170 6572  dertools.scraper
-00000280: 2e6d 6964 646c 6577 6172 6573 2e70 726f  .middlewares.pro
-00000290: 7879 2e70 7269 7661 7465 7207 0000 00da  xy.privater.....
-000002a0: 075f 5f61 6c6c 5f5f a900 720d 0000 0072  .__all__..r....r
-000002b0: 0d00 0000 fa4e 2f72 6f6f 742f 6d79 7072  .....N/root/mypr
-000002c0: 6f6a 2f41 7975 6765 5370 6964 6572 546f  oj/AyugeSpiderTo
-000002d0: 6f6c 732f 6179 7567 6573 7069 6465 7274  ols/ayugespidert
-000002e0: 6f6f 6c73 2f73 6372 6170 6572 2f6d 6964  ools/scraper/mid
-000002f0: 646c 6577 6172 6573 2f5f 5f69 6e69 745f  dlewares/__init_
-00000300: 5f2e 7079 da08 3c6d 6f64 756c 653e 0500  _.py..<module>..
-00000310: 0000 7316 0000 000c 010c 0310 040c 030c  ..s.............
-00000320: 0502 0102 0102 0102 0102 0102 fa         .............
+00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
+00000080: 6408 6409 640a 640b 640c 640d 640e 6708  d.d.d.d.d.d.d.g.
+00000090: 5a0e 640f 5300 2910 e900 0000 0029 01da  Z.d.S.)......)..
+000000a0: 1952 616e 646f 6d52 6571 7565 7374 5561  .RandomRequestUa
+000000b0: 4d69 6464 6c65 7761 7265 2902 da20 4169  Middleware).. Ai
+000000c0: 6f68 7474 7041 7379 6e63 446f 776e 6c6f  ohttpAsyncDownlo
+000000d0: 6164 6572 4d69 6464 6c65 7761 7265 da1b  aderMiddleware..
+000000e0: 4169 6f68 7474 7044 6f77 6e6c 6f61 6465  AiohttpDownloade
+000000f0: 724d 6964 646c 6577 6172 6529 01da 1c52  rMiddleware)...R
+00000100: 6571 7565 7374 7344 6f77 6e6c 6f61 6465  equestsDownloade
+00000110: 724d 6964 646c 6577 6172 6529 02da 2341  rMiddleware)..#A
+00000120: 6275 4479 6e61 6d69 6350 726f 7879 446f  buDynamicProxyDo
+00000130: 776e 6c6f 6164 6572 4d69 6464 6c65 7761  wnloaderMiddlewa
+00000140: 7265 da20 4479 6e61 6d69 6350 726f 7879  re. DynamicProxy
+00000150: 446f 776e 6c6f 6164 6572 4d69 6464 6c65  DownloaderMiddle
+00000160: 7761 7265 2901 da22 4578 636c 7573 6976  ware).."Exclusiv
+00000170: 6550 726f 7879 446f 776e 6c6f 6164 6572  eProxyDownloader
+00000180: 4d69 6464 6c65 7761 7265 2901 da20 5072  Middleware).. Pr
+00000190: 6976 6174 6550 726f 7879 446f 776e 6c6f  ivateProxyDownlo
+000001a0: 6164 6572 4d69 6464 6c65 7761 7265 7202  aderMiddlewarer.
+000001b0: 0000 0072 0500 0000 7203 0000 0072 0400  ...r....r....r..
+000001c0: 0000 7207 0000 0072 0600 0000 7208 0000  ..r....r....r...
+000001d0: 0072 0900 0000 4e29 0fda 2f61 7975 6765  .r....N)../ayuge
+000001e0: 7370 6964 6572 746f 6f6c 732e 7363 7261  spidertools.scra
+000001f0: 7065 722e 6d69 6464 6c65 7761 7265 732e  per.middlewares.
+00000200: 6865 6164 6572 732e 7561 7202 0000 00da  headers.uar.....
+00000210: 3661 7975 6765 7370 6964 6572 746f 6f6c  6ayugespidertool
+00000220: 732e 7363 7261 7065 722e 6d69 6464 6c65  s.scraper.middle
+00000230: 7761 7265 732e 6e65 746c 6962 2e61 696f  wares.netlib.aio
+00000240: 6874 7470 6c69 6272 0300 0000 7204 0000  httplibr....r...
+00000250: 00da 3761 7975 6765 7370 6964 6572 746f  ..7ayugespiderto
+00000260: 6f6c 732e 7363 7261 7065 722e 6d69 6464  ols.scraper.midd
+00000270: 6c65 7761 7265 732e 6e65 746c 6962 2e72  lewares.netlib.r
+00000280: 6571 7565 7374 736c 6962 7205 0000 00da  equestslibr.....
+00000290: 3261 7975 6765 7370 6964 6572 746f 6f6c  2ayugespidertool
+000002a0: 732e 7363 7261 7065 722e 6d69 6464 6c65  s.scraper.middle
+000002b0: 7761 7265 732e 7072 6f78 792e 6479 6e61  wares.proxy.dyna
+000002c0: 6d69 6372 0600 0000 7207 0000 00da 3461  micr....r.....4a
+000002d0: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
+000002e0: 7363 7261 7065 722e 6d69 6464 6c65 7761  scraper.middlewa
+000002f0: 7265 732e 7072 6f78 792e 6578 636c 7573  res.proxy.exclus
+00000300: 6976 6572 0800 0000 5a32 6179 7567 6573  iver....Z2ayuges
+00000310: 7069 6465 7274 6f6f 6c73 2e73 6372 6170  pidertools.scrap
+00000320: 6572 2e6d 6964 646c 6577 6172 6573 2e70  er.middlewares.p
+00000330: 726f 7879 2e70 7269 7661 7465 7209 0000  roxy.privater...
+00000340: 00da 075f 5f61 6c6c 5f5f a900 7210 0000  ...__all__..r...
+00000350: 0072 1000 0000 fa4e 2f72 6f6f 742f 6d79  .r.....N/root/my
+00000360: 7072 6f6a 2f41 7975 6765 5370 6964 6572  proj/AyugeSpider
+00000370: 546f 6f6c 732f 6179 7567 6573 7069 6465  Tools/ayugespide
+00000380: 7274 6f6f 6c73 2f73 6372 6170 6572 2f6d  rtools/scraper/m
+00000390: 6964 646c 6577 6172 6573 2f5f 5f69 6e69  iddlewares/__ini
+000003a0: 745f 5f2e 7079 da08 3c6d 6f64 756c 653e  t__.py..<module>
+000003b0: 0500 0000 731c 0000 000c 0110 040c 0310  ....s...........
+000003c0: 040c 030c 0502 0102 0102 0102 0102 0102  ................
+000003d0: 0102 0102 f8                             .....
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 11 07:50:13 2023 UTC, .py size: 1742 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 3511 3564 ce06 0000  U.......5.5d....
+00000000: 550d 0d0a 0000 0000 c841 4764 ce06 0000  U........AGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6701 5a05 4700 6405 6404 8400 6404 6506  g.Z.G.d.d...d.e.
 00000060: 8303 5a07 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da07 7369 676e 616c 7329 01da 0550  )...signals)...P
@@ -129,13 +129,13 @@
 00000800: 6173 736d 6574 686f 6472 1800 0000 7214  assmethodr....r.
 00000810: 0000 0072 2f00 0000 7208 0000 0072 0800  ...r/...r....r..
 00000820: 0000 7208 0000 0072 0900 0000 7204 0000  ..r....r....r...
 00000830: 000c 0000 0073 0e00 0000 0801 0404 0804  .....s..........
 00000840: 0e07 0201 0a05 080d 2908 720d 0000 00da  ........).r.....
 00000850: 0673 6372 6170 7972 0200 0000 da1e 6179  .scrapyr......ay
 00000860: 7567 6573 7069 6465 7274 6f6f 6c73 2e63  ugespidertools.c
-00000870: 6f6d 6d6f 6e2e 5061 7261 6d73 7203 0000  ommon.Paramsr...
+00000870: 6f6d 6d6f 6e2e 7061 7261 6d73 7203 0000  ommon.paramsr...
 00000880: 00da 075f 5f61 6c6c 5f5f da06 6f62 6a65  ...__all__..obje
 00000890: 6374 7204 0000 0072 0800 0000 7208 0000  ctr....r....r...
 000008a0: 0072 0800 0000 7209 0000 00da 083c 6d6f  .r....r......<mo
 000008b0: 6475 6c65 3e01 0000 0073 0a00 0000 0802  dule>....s......
 000008c0: 0c02 0c03 02ff 0405                      ........
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 
 from scrapy import signals
 
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.params import Param
 
 __all__ = [
     "RandomRequestUaMiddleware",
 ]
 
 
 class RandomRequestUaMiddleware(object):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 11 07:41:24 2023 UTC, .py size: 4275 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,138 @@
-00000000: 550d 0d0a 0000 0000 240f 3564 b310 0000  U.......$.5d....
+00000000: 550d 0d0a 0000 0000 f341 4764 eb10 0000  U........AGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
+00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
-00000070: 6509 8303 5a0a 6401 5300 2908 e900 0000  e...Z.d.S.).....
-00000080: 004e 2901 da0c 4874 6d6c 5265 7370 6f6e  .N)...HtmlRespon
-00000090: 7365 2901 da0e 5265 7573 654f 7065 7261  se)...ReuseOpera
-000000a0: 7469 6f6e 2901 da05 5061 7261 6d29 01da  tion)...Param)..
-000000b0: 0b54 6f6f 6c73 466f 7241 7975 6300 0000  .ToolsForAyuc...
-000000c0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000000d0: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-000000e0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-000000f0: 5300 2905 da1b 5265 7175 6573 7442 7952  S.)...RequestByR
-00000100: 6571 7565 7374 734d 6964 646c 6577 6172  equestsMiddlewar
-00000110: 6575 3900 0000 0a20 2020 20e5 b086 2073  eu9....    ... s
-00000120: 6372 6170 7920 e79a 8420 5265 7175 6573  crapy ... Reques
-00000130: 7420 e8af b7e6 b182 e69b bfe6 8da2 e4b8  t ..............
-00000140: ba20 7265 7175 6573 7473 0a20 2020 2063  . requests.    c
-00000150: 0300 0000 0000 0000 0000 0000 0900 0000  ................
-00000160: 0a00 0000 4300 0000 7362 0100 0090 017a  ....C...sb.....z
-00000170: 1874 006a 017c 016a 0264 018d 017d 0374  .t.j.|.j.d...}.t
-00000180: 037c 016a 0464 0264 038d 027d 0474 037c  .|.j.d.d...}.t.|
-00000190: 016a 0583 01a0 06a1 007d 057c 0564 046b  .j.......}.|.d.k
-000001a0: 0272 867c 016a 0473 6074 076a 087c 057c  .r.|.j.s`t.j.|.|
-000001b0: 016a 097c 037c 016a 0a64 0574 0b6a 0c74  .j.|.|.j.d.t.j.t
-000001c0: 0b6a 0d66 0264 068d 067d 066e 2474 076a  .j.f.d...}.n$t.j
-000001d0: 087c 057c 016a 097c 037c 016a 0a7c 0464  .|.|.j.|.|.j.|.d
-000001e0: 0574 0b6a 0c74 0b6a 0d66 0264 078d 077d  .t.j.t.j.f.d...}
-000001f0: 066e 7c7c 0564 086b 0272 fa74 0e6a 0f7c  .n||.d.k.r.t.j.|
-00000200: 0464 098d 0172 c074 076a 087c 057c 016a  .d...r.t.j.|.|.j
-00000210: 097c 037c 047c 016a 0a64 0574 0b6a 0c74  .|.|.|.j.d.t.j.t
-00000220: 0b6a 0d66 0264 0a8d 077d 066e 3864 0b64  .j.f.d...}.n8d.d
-00000230: 0c84 007c 04a0 1064 0da1 0144 0083 017d  ...|...d...D...}
-00000240: 0774 076a 087c 057c 016a 097c 037c 077c  .t.j.|.|.j.|.|.|
-00000250: 016a 0a64 0574 0b6a 0c74 0b6a 0d66 0264  .j.d.t.j.t.j.f.d
-00000260: 0a8d 077d 066e 0874 1164 0e83 0182 0174  ...}.n.t.d.....t
-00000270: 127c 016a 097c 066a 137c 066a 147c 0164  .|.j.|.j.|.j.|.d
-00000280: 0264 0f8d 0557 0053 0004 0074 156b 0a90  .d...W.S...t.k..
-00000290: 0172 5c01 007d 0801 007a 2274 127c 016a  .r\..}...z"t.|.j
-000002a0: 0964 1064 117c 089b 009d 027c 0164 0264  .d.d.|.....|.d.d
-000002b0: 0f8d 0506 0057 0059 00a2 0253 0064 007d  .....W.Y...S.d.}
-000002c0: 087e 0858 0059 006e 0258 0064 0053 0029  .~.X.Y.n.X.d.S.)
-000002d0: 124e 2901 da0e 7363 7261 7079 5f68 6561  .N)...scrapy_hea
-000002e0: 6465 7273 7a05 7574 662d 3829 01da 0865  dersz.utf-8)...e
-000002f0: 6e63 6f64 696e 67da 0347 4554 4629 06da  ncoding..GETF)..
-00000300: 066d 6574 686f 64da 0375 726c da07 6865  .method..url..he
-00000310: 6164 6572 73da 0763 6f6f 6b69 6573 da06  aders..cookies..
-00000320: 7665 7269 6679 da07 7469 6d65 6f75 7429  verify..timeout)
-00000330: 0772 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000340: 720d 0000 00da 0464 6174 6172 0e00 0000  r......datar....
-00000350: 720f 0000 00da 0450 4f53 5429 01da 096a  r......POST)...j
-00000360: 7564 6765 5f73 7472 2907 720a 0000 0072  udge_str).r....r
-00000370: 0b00 0000 720c 0000 0072 1000 0000 720d  ....r....r....r.
-00000380: 0000 0072 0e00 0000 720f 0000 0063 0100  ...r....r....c..
-00000390: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000003a0: 0000 5300 0000 7326 0000 0069 007c 005d  ..S...s&...i.|.]
-000003b0: 1e7d 017c 01a0 0064 00a1 0164 0119 007c  .}.|...d...d...|
-000003c0: 01a0 0064 00a1 0164 0219 0093 0271 0453  ...d...d.....q.S
-000003d0: 0029 03fa 013d 7201 0000 00e9 0100 0000  .)...=r.........
-000003e0: 2901 da05 7370 6c69 7429 02da 022e 30da  )...split)....0.
-000003f0: 0178 a900 7218 0000 00fa 582f 726f 6f74  .x..r.....X/root
-00000400: 2f6d 7970 726f 6a2f 4179 7567 6553 7069  /myproj/AyugeSpi
-00000410: 6465 7254 6f6f 6c73 2f61 7975 6765 7370  derTools/ayugesp
-00000420: 6964 6572 746f 6f6c 732f 7363 7261 7065  idertools/scrape
-00000430: 722f 6d69 6464 6c65 7761 7265 732f 6e65  r/middlewares/ne
-00000440: 746c 6962 2f72 6571 7565 7374 736c 6962  tlib/requestslib
-00000450: 2e70 79da 0a3c 6469 6374 636f 6d70 3e46  .py..<dictcomp>F
-00000460: 0000 0073 0600 0000 0602 02ff 0c00 7a3f  ...s..........z?
-00000470: 5265 7175 6573 7442 7952 6571 7565 7374  RequestByRequest
-00000480: 734d 6964 646c 6577 6172 652e 7072 6f63  sMiddleware.proc
-00000490: 6573 735f 7265 7175 6573 742e 3c6c 6f63  ess_request.<loc
-000004a0: 616c 733e 2e3c 6469 6374 636f 6d70 3efa  als>.<dictcomp>.
-000004b0: 0126 752d 0000 00e5 87ba e78e b0e6 9caa  .&u-............
-000004c0: e79f a5e8 afb7 e6b1 82e6 96b9 e5bc 8fef  ................
-000004d0: bc8c e8af b7e5 8f8a e697 b6e6 9fa5 e79c  ................
-000004e0: 8bef bc81 2905 720b 0000 00da 0673 7461  ....).r......sta
-000004f0: 7475 73da 0462 6f64 79da 0772 6571 7565  tus..body..reque
-00000500: 7374 7208 0000 00e9 ca00 0000 751e 0000  str.........u...
-00000510: 0072 6571 7565 7374 7320 e8af b7e6 b182  .requests ......
-00000520: e587 bae7 8eb0 e994 99e8 afaf efbc 9a29  ...............)
-00000530: 1672 0500 0000 da20 6765 745f 6469 6374  .r..... get_dict
-00000540: 5f66 6f72 6d5f 7363 7261 7079 5f72 6571  _form_scrapy_req
-00000550: 5f68 6561 6465 7273 720c 0000 00da 0373  _headersr......s
-00000560: 7472 721d 0000 0072 0a00 0000 da05 7570  trr....r......up
-00000570: 7065 72da 0872 6571 7565 7374 7372 1e00  per..requestsr..
-00000580: 0000 720b 0000 0072 0d00 0000 7204 0000  ..r....r....r...
-00000590: 00da 1472 6571 7565 7374 735f 7265 715f  ...requests_req_
-000005a0: 7469 6d65 6f75 74da 1472 6571 7565 7374  timeout..request
-000005b0: 735f 7265 735f 7469 6d65 6f75 7472 0300  s_res_timeoutr..
-000005c0: 0000 da11 6a75 6467 655f 7374 725f 6973  ....judge_str_is
-000005d0: 5f6a 736f 6e72 1500 0000 da0a 5661 6c75  _jsonr......Valu
-000005e0: 6545 7272 6f72 7202 0000 00da 0b73 7461  eErrorr......sta
-000005f0: 7475 735f 636f 6465 da04 7465 7874 da09  tus_code..text..
-00000600: 4578 6365 7074 696f 6e29 09da 0473 656c  Exception)...sel
-00000610: 6672 1e00 0000 da06 7370 6964 6572 5a09  fr......spiderZ.
-00000620: 725f 6865 6164 6572 735a 1072 6571 7565  r_headersZ.reque
-00000630: 7374 5f62 6f64 795f 7374 725a 1573 6372  st_body_strZ.scr
-00000640: 6170 795f 7265 7175 6573 745f 6d65 7468  apy_request_meth
-00000650: 6f64 5a0a 725f 7265 7370 6f6e 7365 5a0e  odZ.r_responseZ.
-00000660: 706f 7374 5f64 6174 615f 6469 6374 da01  post_data_dict..
-00000670: 6572 1800 0000 7218 0000 0072 1900 0000  er....r....r....
-00000680: da0f 7072 6f63 6573 735f 7265 7175 6573  ..process_reques
-00000690: 740e 0000 0073 9000 0000 0001 0402 0401  t....s..........
-000006a0: 04ff 0604 0e01 0e01 0802 0601 0401 0201  ................
-000006b0: 0401 0201 0401 0202 0401 04fe 02fa 080e  ................
-000006c0: 0401 0201 0401 0201 0401 0201 0202 0401  ................
-000006d0: 04fe 02f9 080d 0802 0c01 0401 0201 0401  ................
-000006e0: 0201 0201 0401 0202 0401 04fe 02f9 080e  ................
-000006f0: 0602 08fe 0604 0401 0201 0401 0201 0201  ................
-00000700: 0401 0202 0401 04fe 02f9 080d 0801 0201  ................
-00000710: 0401 0401 0401 0201 02fb 0808 1202 0201  ................
-00000720: 0401 0201 0801 0201 02fb 7a2b 5265 7175  ..........z+Requ
-00000730: 6573 7442 7952 6571 7565 7374 734d 6964  estByRequestsMid
-00000740: 646c 6577 6172 652e 7072 6f63 6573 735f  dleware.process_
-00000750: 7265 7175 6573 744e 2905 da08 5f5f 6e61  requestN)...__na
-00000760: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000770: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000780: 5f5f 646f 635f 5f72 2e00 0000 7218 0000  __doc__r....r...
-00000790: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-000007a0: 7206 0000 0009 0000 0073 0400 0000 0801  r........s......
-000007b0: 0404 7206 0000 0029 0b72 2300 0000 da0b  ..r....).r#.....
-000007c0: 7363 7261 7079 2e68 7474 7072 0200 0000  scrapy.httpr....
-000007d0: da24 6179 7567 6573 7069 6465 7274 6f6f  .$ayugespidertoo
-000007e0: 6c73 2e63 6f6d 6d6f 6e2e 4d75 6c74 6950  ls.common.MultiP
-000007f0: 6c65 7869 6e67 7203 0000 00da 1e61 7975  lexingr......ayu
-00000800: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00000810: 6d6d 6f6e 2e50 6172 616d 7372 0400 0000  mmon.Paramsr....
-00000820: da1d 6179 7567 6573 7069 6465 7274 6f6f  ..ayugespidertoo
-00000830: 6c73 2e63 6f6d 6d6f 6e2e 5574 696c 7372  ls.common.Utilsr
-00000840: 0500 0000 da06 6f62 6a65 6374 7206 0000  ......objectr...
-00000850: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000860: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000870: 0000 0073 0a00 0000 0801 0c02 0c01 0c01  ...s............
-00000880: 0c03                                     ..
+00000060: 6d08 5a08 0100 6406 6701 5a09 4700 6407  m.Z...d.g.Z.G.d.
+00000070: 6406 8400 6406 650a 8303 5a0b 6401 5300  d...d.e...Z.d.S.
+00000080: 2908 e900 0000 004e 2901 da0c 4874 6d6c  )......N)...Html
+00000090: 5265 7370 6f6e 7365 2901 da0e 5265 7573  Response)...Reus
+000000a0: 654f 7065 7261 7469 6f6e 2901 da05 5061  eOperation)...Pa
+000000b0: 7261 6d29 01da 0b54 6f6f 6c73 466f 7241  ram)...ToolsForA
+000000c0: 7975 da1c 5265 7175 6573 7473 446f 776e  yu..RequestsDown
+000000d0: 6c6f 6164 6572 4d69 6464 6c65 7761 7265  loaderMiddleware
+000000e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000000f0: 0002 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
+00000100: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+00000110: 5a04 6404 5300 2905 7206 0000 0075 3900  Z.d.S.).r....u9.
+00000120: 0000 0a20 2020 20e5 b086 2073 6372 6170  ...    ... scrap
+00000130: 7920 e79a 8420 5265 7175 6573 7420 e8af  y ... Request ..
+00000140: b7e6 b182 e69b bfe6 8da2 e4b8 ba20 7265  ............. re
+00000150: 7175 6573 7473 0a20 2020 2063 0300 0000  quests.    c....
+00000160: 0000 0000 0000 0000 0900 0000 0a00 0000  ................
+00000170: 4300 0000 7362 0100 0090 017a 1874 006a  C...sb.....z.t.j
+00000180: 017c 016a 0264 018d 017d 0374 037c 016a  .|.j.d...}.t.|.j
+00000190: 0464 0264 038d 027d 0474 037c 016a 0583  .d.d...}.t.|.j..
+000001a0: 01a0 06a1 007d 057c 0564 046b 0272 867c  .....}.|.d.k.r.|
+000001b0: 016a 0473 6074 076a 087c 057c 016a 097c  .j.s`t.j.|.|.j.|
+000001c0: 037c 016a 0a64 0574 0b6a 0c74 0b6a 0d66  .|.j.d.t.j.t.j.f
+000001d0: 0264 068d 067d 066e 2474 076a 087c 057c  .d...}.n$t.j.|.|
+000001e0: 016a 097c 037c 016a 0a7c 0464 0574 0b6a  .j.|.|.j.|.d.t.j
+000001f0: 0c74 0b6a 0d66 0264 078d 077d 066e 7c7c  .t.j.f.d...}.n||
+00000200: 0564 086b 0272 fa74 0e6a 0f7c 0464 098d  .d.k.r.t.j.|.d..
+00000210: 0172 c074 076a 087c 057c 016a 097c 037c  .r.t.j.|.|.j.|.|
+00000220: 047c 016a 0a64 0574 0b6a 0c74 0b6a 0d66  .|.j.d.t.j.t.j.f
+00000230: 0264 0a8d 077d 066e 3864 0b64 0c84 007c  .d...}.n8d.d...|
+00000240: 04a0 1064 0da1 0144 0083 017d 0774 076a  ...d...D...}.t.j
+00000250: 087c 057c 016a 097c 037c 077c 016a 0a64  .|.|.j.|.|.|.j.d
+00000260: 0574 0b6a 0c74 0b6a 0d66 0264 0a8d 077d  .t.j.t.j.f.d...}
+00000270: 066e 0874 1164 0e83 0182 0174 127c 016a  .n.t.d.....t.|.j
+00000280: 097c 066a 137c 066a 147c 0164 0264 0f8d  .|.j.|.j.|.d.d..
+00000290: 0557 0053 0004 0074 156b 0a90 0172 5c01  .W.S...t.k...r\.
+000002a0: 007d 0801 007a 2274 127c 016a 0964 1064  .}...z"t.|.j.d.d
+000002b0: 117c 089b 009d 027c 0164 0264 0f8d 0506  .|.....|.d.d....
+000002c0: 0057 0059 00a2 0253 0064 007d 087e 0858  .W.Y...S.d.}.~.X
+000002d0: 0059 006e 0258 0064 0053 0029 124e 2901  .Y.n.X.d.S.).N).
+000002e0: da0e 7363 7261 7079 5f68 6561 6465 7273  ..scrapy_headers
+000002f0: 7a05 7574 662d 3829 01da 0865 6e63 6f64  z.utf-8)...encod
+00000300: 696e 67da 0347 4554 4629 06da 066d 6574  ing..GETF)...met
+00000310: 686f 64da 0375 726c da07 6865 6164 6572  hod..url..header
+00000320: 73da 0763 6f6f 6b69 6573 da06 7665 7269  s..cookies..veri
+00000330: 6679 da07 7469 6d65 6f75 7429 0772 0a00  fy..timeout).r..
+00000340: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000350: 00da 0464 6174 6172 0e00 0000 720f 0000  ...datar....r...
+00000360: 00da 0450 4f53 5429 01da 096a 7564 6765  ...POST)...judge
+00000370: 5f73 7472 2907 720a 0000 0072 0b00 0000  _str).r....r....
+00000380: 720c 0000 0072 1000 0000 720d 0000 0072  r....r....r....r
+00000390: 0e00 0000 720f 0000 0063 0100 0000 0000  ....r....c......
+000003a0: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
+000003b0: 0000 7326 0000 0069 007c 005d 1e7d 017c  ..s&...i.|.].}.|
+000003c0: 01a0 0064 00a1 0164 0119 007c 01a0 0064  ...d...d...|...d
+000003d0: 00a1 0164 0219 0093 0271 0453 0029 03fa  ...d.....q.S.)..
+000003e0: 013d 7201 0000 00e9 0100 0000 2901 da05  .=r.........)...
+000003f0: 7370 6c69 7429 02da 022e 30da 0178 a900  split)....0..x..
+00000400: 7218 0000 00fa 582f 726f 6f74 2f6d 7970  r.....X/root/myp
+00000410: 726f 6a2f 4179 7567 6553 7069 6465 7254  roj/AyugeSpiderT
+00000420: 6f6f 6c73 2f61 7975 6765 7370 6964 6572  ools/ayugespider
+00000430: 746f 6f6c 732f 7363 7261 7065 722f 6d69  tools/scraper/mi
+00000440: 6464 6c65 7761 7265 732f 6e65 746c 6962  ddlewares/netlib
+00000450: 2f72 6571 7565 7374 736c 6962 2e70 79da  /requestslib.py.
+00000460: 0a3c 6469 6374 636f 6d70 3e4a 0000 0073  .<dictcomp>J...s
+00000470: 0600 0000 0602 02ff 0c00 7a40 5265 7175  ..........z@Requ
+00000480: 6573 7473 446f 776e 6c6f 6164 6572 4d69  estsDownloaderMi
+00000490: 6464 6c65 7761 7265 2e70 726f 6365 7373  ddleware.process
+000004a0: 5f72 6571 7565 7374 2e3c 6c6f 6361 6c73  _request.<locals
+000004b0: 3e2e 3c64 6963 7463 6f6d 703e fa01 2675  >.<dictcomp>..&u
+000004c0: 2d00 0000 e587 bae7 8eb0 e69c aae7 9fa5  -...............
+000004d0: e8af b7e6 b182 e696 b9e5 bc8f efbc 8ce8  ................
+000004e0: afb7 e58f 8ae6 97b6 e69f a5e7 9c8b efbc  ................
+000004f0: 8129 0572 0b00 0000 da06 7374 6174 7573  .).r......status
+00000500: da04 626f 6479 da07 7265 7175 6573 7472  ..body..requestr
+00000510: 0800 0000 e9ca 0000 0075 1e00 0000 7265  .........u....re
+00000520: 7175 6573 7473 20e8 afb7 e6b1 82e5 87ba  quests .........
+00000530: e78e b0e9 9499 e8af afef bc9a 2916 7205  ............).r.
+00000540: 0000 00da 2067 6574 5f64 6963 745f 666f  .... get_dict_fo
+00000550: 726d 5f73 6372 6170 795f 7265 715f 6865  rm_scrapy_req_he
+00000560: 6164 6572 7372 0c00 0000 da03 7374 7272  adersr......strr
+00000570: 1d00 0000 720a 0000 00da 0575 7070 6572  ....r......upper
+00000580: da08 7265 7175 6573 7473 721e 0000 0072  ..requestsr....r
+00000590: 0b00 0000 720d 0000 0072 0400 0000 da14  ....r....r......
+000005a0: 7265 7175 6573 7473 5f72 6571 5f74 696d  requests_req_tim
+000005b0: 656f 7574 da14 7265 7175 6573 7473 5f72  eout..requests_r
+000005c0: 6573 5f74 696d 656f 7574 7203 0000 00da  es_timeoutr.....
+000005d0: 116a 7564 6765 5f73 7472 5f69 735f 6a73  .judge_str_is_js
+000005e0: 6f6e 7215 0000 00da 0a56 616c 7565 4572  onr......ValueEr
+000005f0: 726f 7272 0200 0000 da0b 7374 6174 7573  rorr......status
+00000600: 5f63 6f64 65da 0474 6578 74da 0945 7863  _code..text..Exc
+00000610: 6570 7469 6f6e 2909 da04 7365 6c66 721e  eption)...selfr.
+00000620: 0000 00da 0673 7069 6465 725a 0972 5f68  .....spiderZ.r_h
+00000630: 6561 6465 7273 da10 7265 7175 6573 745f  eaders..request_
+00000640: 626f 6479 5f73 7472 da15 7363 7261 7079  body_str..scrapy
+00000650: 5f72 6571 7565 7374 5f6d 6574 686f 645a  _request_methodZ
+00000660: 0a72 5f72 6573 706f 6e73 655a 0e70 6f73  .r_responseZ.pos
+00000670: 745f 6461 7461 5f64 6963 74da 0165 7218  t_data_dict..er.
+00000680: 0000 0072 1800 0000 7219 0000 00da 0f70  ...r....r......p
+00000690: 726f 6365 7373 5f72 6571 7565 7374 1200  rocess_request..
+000006a0: 0000 7390 0000 0000 0104 0204 0104 ff06  ..s.............
+000006b0: 040e 010e 0108 0206 0104 0102 0104 0102  ................
+000006c0: 0104 0102 0204 0104 fe02 fa08 0e04 0102  ................
+000006d0: 0104 0102 0104 0102 0102 0204 0104 fe02  ................
+000006e0: f908 0d08 020c 0104 0102 0104 0102 0102  ................
+000006f0: 0104 0102 0204 0104 fe02 f908 0e06 0208  ................
+00000700: fe06 0404 0102 0104 0102 0102 0104 0102  ................
+00000710: 0204 0104 fe02 f908 0d08 0102 0104 0104  ................
+00000720: 0104 0102 0102 fb08 0812 0202 0104 0102  ................
+00000730: 0108 0102 0102 fb7a 2c52 6571 7565 7374  .......z,Request
+00000740: 7344 6f77 6e6c 6f61 6465 724d 6964 646c  sDownloaderMiddl
+00000750: 6577 6172 652e 7072 6f63 6573 735f 7265  eware.process_re
+00000760: 7175 6573 744e 2905 da08 5f5f 6e61 6d65  questN)...__name
+00000770: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000780: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000790: 646f 635f 5f72 3000 0000 7218 0000 0072  doc__r0...r....r
+000007a0: 1800 0000 7218 0000 0072 1900 0000 7206  ....r....r....r.
+000007b0: 0000 000d 0000 0073 0400 0000 0801 0404  .......s........
+000007c0: 290c 7223 0000 00da 0b73 6372 6170 792e  ).r#.....scrapy.
+000007d0: 6874 7470 7202 0000 00da 2461 7975 6765  httpr.....$ayuge
+000007e0: 7370 6964 6572 746f 6f6c 732e 636f 6d6d  spidertools.comm
+000007f0: 6f6e 2e6d 756c 7469 706c 6578 696e 6772  on.multiplexingr
+00000800: 0300 0000 da1e 6179 7567 6573 7069 6465  ......ayugespide
+00000810: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7061  rtools.common.pa
+00000820: 7261 6d73 7204 0000 00da 1d61 7975 6765  ramsr......ayuge
+00000830: 7370 6964 6572 746f 6f6c 732e 636f 6d6d  spidertools.comm
+00000840: 6f6e 2e75 7469 6c73 7205 0000 00da 075f  on.utilsr......_
+00000850: 5f61 6c6c 5f5f da06 6f62 6a65 6374 7206  _all__..objectr.
+00000860: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
+00000870: 0000 7219 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000880: 3e01 0000 0073 0e00 0000 0801 0c02 0c01  >....s..........
+00000890: 0c01 0c03 02ff 0405                      ........
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import requests
 from scrapy.http import HtmlResponse
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.utils import ToolsForAyu
 
+__all__ = [
+    "RequestsDownloaderMiddleware",
+]
 
-class RequestByRequestsMiddleware(object):
+
+class RequestsDownloaderMiddleware(object):
     """
     将 scrapy 的 Request 请求替换为 requests
     """
 
     def process_request(self, request, spider):
         try:
             # 将 scrapy 的 request headers 的值，原封不动地转移到 requests 中
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 11 07:45:40 2023 UTC, .py size: 4244 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2410 3564 9410 0000  U.......$.5d....
+00000000: 550d 0d0a 0000 0000 0642 4764 8410 0000  U........BGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6507 8303 5a08 4700 6407 6408  ..d.e...Z.G.d.d.
 00000070: 8400 6408 6507 8303 5a09 6401 5300 2909  ..d.e...Z.d.S.).
@@ -28,219 +28,218 @@
 000001b0: 5f07 7c02 6405 1900 7c00 5f08 6402 5300  _.|.d...|._.d.S.
 000001c0: 2908 7547 0000 000a 2020 2020 2020 2020  ).uG....        
 000001d0: e4bb 8e20 7363 7261 7079 20e9 858d e7bd  ... scrapy .....
 000001e0: aee4 b8ad e58f 96e5 87ba e58a a8e6 8081  ................
 000001f0: e99a a7e9 8193 e4bb a3e7 9086 e79a 84e4  ................
 00000200: bfa1 e681 af0a 2020 2020 2020 2020 da14  ......        ..
 00000210: 4459 4e41 4d49 435f 5052 4f58 595f 434f  DYNAMIC_PROXY_CO
-00000220: 4e46 4947 4eda 0950 524f 5859 5f55 524c  NFIGN..PROXY_URL
-00000230: da08 5553 4552 4e41 4d45 da08 5041 5353  ..USERNAME..PASS
-00000240: 574f 5244 a902 da09 6469 6374 5f63 6f6e  WORD....dict_con
-00000250: 66da 086b 6579 5f6c 6973 74f5 3300 0000  f..key_list.3...
-00000260: e6b2 a1e6 9c89 e985 8de7 bdae e58a a8e6  ................
-00000270: 8081 e99a a7e9 8193 e4bb a3e7 9086 efbc  ................
-00000280: 8ce9 858d e7bd aee7 a4ba e4be 8be4 b8ba  ................
-00000290: efbc 9aa9 09da 0367 6574 7203 0000 00da  .......getr.....
-000002a0: 1669 735f 6469 6374 5f6d 6565 745f 6d69  .is_dict_meet_mi
-000002b0: 6e5f 6c69 6d69 74da 0e41 7373 6572 7469  n_limit..Asserti
-000002c0: 6f6e 4572 726f 7272 0400 0000 da1a 6479  onErrorr......dy
-000002d0: 6e61 6d69 635f 7072 6f78 795f 636f 6e66  namic_proxy_conf
-000002e0: 5f65 7861 6d70 6c65 da09 7072 6f78 795f  _example..proxy_
-000002f0: 7572 6cda 0875 7365 726e 616d 65da 0870  url..username..p
-00000300: 6173 7377 6f72 64a9 04da 0473 656c 66da  assword....self.
-00000310: 0873 6574 7469 6e67 735a 1264 796e 616d  .settingsZ.dynam
-00000320: 6963 5f70 726f 7879 5f63 6f6e 665a 0869  ic_proxy_confZ.i
-00000330: 735f 6d61 7463 68a9 0072 1900 0000 fa53  s_match..r.....S
-00000340: 2f72 6f6f 742f 6d79 7072 6f6a 2f41 7975  /root/myproj/Ayu
-00000350: 6765 5370 6964 6572 546f 6f6c 732f 6179  geSpiderTools/ay
-00000360: 7567 6573 7069 6465 7274 6f6f 6c73 2f73  ugespidertools/s
-00000370: 6372 6170 6572 2f6d 6964 646c 6577 6172  craper/middlewar
-00000380: 6573 2f70 726f 7879 2f64 796e 616d 6963  es/proxy/dynamic
-00000390: 2e70 79da 085f 5f69 6e69 745f 5f0e 0000  .py..__init__...
-000003a0: 0073 1200 0000 0004 0c02 0401 0201 08fe  .s..............
-000003b0: 0604 1402 0a01 0a01 7a29 4479 6e61 6d69  ........z)Dynami
-000003c0: 6350 726f 7879 446f 776e 6c6f 6164 6572  cProxyDownloader
-000003d0: 4d69 6464 6c65 7761 7265 2e5f 5f69 6e69  Middleware.__ini
-000003e0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-000003f0: 0300 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-00000400: 007c 007c 016a 0083 017d 027c 016a 016a  .|.|.j...}.|.j.j
-00000410: 027c 026a 0374 016a 0364 018d 0201 007c  .|.j.t.j.d.....|
-00000420: 0253 00a9 024e 2901 da06 7369 676e 616c  .S...N)...signal
-00000430: a904 7218 0000 0072 0200 0000 da07 636f  ..r....r......co
-00000440: 6e6e 6563 74da 0d73 7069 6465 725f 6f70  nnect..spider_op
-00000450: 656e 6564 a903 da03 636c 73da 0763 7261  ened....cls..cra
-00000460: 776c 6572 da01 7372 1900 0000 7219 0000  wler..sr....r...
-00000470: 0072 1a00 0000 da0c 6672 6f6d 5f63 7261  .r......from_cra
-00000480: 776c 6572 1e00 0000 7306 0000 0000 020a  wler....s.......
-00000490: 0114 017a 2d44 796e 616d 6963 5072 6f78  ...z-DynamicProx
-000004a0: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
-000004b0: 6577 6172 652e 6672 6f6d 5f63 7261 776c  eware.from_crawl
-000004c0: 6572 6303 0000 0000 0000 0000 0000 0003  erc.............
-000004d0: 0000 0007 0000 0043 0000 0073 9200 0000  .......C...s....
-000004e0: 7c01 6a00 a001 6401 a101 7232 6401 7c00  |.j...d...r2d.|.
-000004f0: 6a02 9b00 6402 7c00 6a03 9b00 6403 7c00  j...d.|.j...d.|.
-00000500: 6a04 9b00 6404 9d07 7c01 6a05 6405 3c00  j...d...|.j.d.<.
-00000510: 6e48 7c01 6a00 a001 6406 a101 7264 6406  nH|.j...d...rdd.
-00000520: 7c00 6a02 9b00 6402 7c00 6a03 9b00 6403  |.j...d.|.j...d.
-00000530: 7c00 6a04 9b00 6404 9d07 7c01 6a05 6405  |.j...d...|.j.d.
-00000540: 3c00 6e16 7c02 6a06 a007 6407 7c01 6a00  <.n.|.j...d.|.j.
-00000550: 9b00 6408 9d03 a101 0100 6409 7c01 6a08  ..d.......d.|.j.
-00000560: 640a 3c00 640b 7c01 6a08 640c 3c00 6400  d.<.d.|.j.d.<.d.
-00000570: 5300 290d 4efa 0868 7474 7073 3a2f 2ffa  S.).N..https://.
-00000580: 013a fa01 40fa 012f da05 7072 6f78 79fa  .:..@../..proxy.
-00000590: 0768 7474 703a 2f2f 7a0d 7265 7175 6573  .http://z.reques
-000005a0: 7420 7572 6c3a 207a 2220 6572 726f 7220  t url: z" error 
-000005b0: 7768 656e 2075 7365 2070 726f 7879 206d  when use proxy m
-000005c0: 6964 646c 6577 6172 6573 21da 0563 6c6f  iddlewares!..clo
-000005d0: 7365 da0a 436f 6e6e 6563 7469 6f6e da04  se..Connection..
-000005e0: 677a 6970 7a0f 4163 6365 7074 2d45 6e63  gzipz.Accept-Enc
-000005f0: 6f64 696e 6729 09da 0375 726c da0a 7374  oding)...url..st
-00000600: 6172 7473 7769 7468 7214 0000 0072 1500  artswithr....r..
-00000610: 0000 7213 0000 00da 046d 6574 61da 0473  ..r......meta..s
-00000620: 6c6f 67da 0469 6e66 6fda 0768 6561 6465  log..info..heade
-00000630: 7273 2903 7217 0000 00da 0772 6571 7565  rs).r......reque
-00000640: 7374 da06 7370 6964 6572 7219 0000 0072  st..spiderr....r
-00000650: 1900 0000 721a 0000 00da 0f70 726f 6365  ....r......proce
-00000660: 7373 5f72 6571 7565 7374 2400 0000 731e  ss_request$...s.
-00000670: 0000 0000 030c 031c fe04 0102 ff04 030c  ................
-00000680: 031c fe04 0102 ff04 0406 010c ff04 050a  ................
-00000690: 027a 3044 796e 616d 6963 5072 6f78 7944  .z0DynamicProxyD
-000006a0: 6f77 6e6c 6f61 6465 724d 6964 646c 6577  ownloaderMiddlew
-000006b0: 6172 652e 7072 6f63 6573 735f 7265 7175  are.process_requ
-000006c0: 6573 7463 0200 0000 0000 0000 0000 0000  estc............
-000006d0: 0200 0000 0400 0000 4300 0000 7318 0000  ........C...s...
-000006e0: 007c 016a 00a0 0164 017c 016a 029b 009d  .|.j...d.|.j....
-000006f0: 02a1 0101 0064 0053 0029 024e 755b 0000  .....d.S.).Nu[..
-00000700: 00e5 8aa8 e680 81e9 9aa7 e981 93e4 bba3  ................
-00000710: e790 86e4 b8ad e997 b4e4 bbb6 3a20 4479  ............: Dy
-00000720: 6e61 6d69 6350 726f 7879 446f 776e 6c6f  namicProxyDownlo
-00000730: 6164 6572 4d69 6464 6c65 7761 7265 20e5  aderMiddleware .
-00000740: b7b2 e5bc 80e5 90af efbc 8ce7 949f e695  ................
-00000750: 88e8 849a e69c ace4 b8ba 3a20 a903 7232  ..........: ..r2
-00000760: 0000 0072 3300 0000 da04 6e61 6d65 a902  ...r3.....name..
-00000770: 7217 0000 0072 3600 0000 7219 0000 0072  r....r6...r....r
-00000780: 1900 0000 721a 0000 0072 2000 0000 3900  ....r....r ...9.
-00000790: 0000 7306 0000 0000 0106 010a ff7a 2e44  ..s..........z.D
-000007a0: 796e 616d 6963 5072 6f78 7944 6f77 6e6c  ynamicProxyDownl
-000007b0: 6f61 6465 724d 6964 646c 6577 6172 652e  oaderMiddleware.
-000007c0: 7370 6964 6572 5f6f 7065 6e65 644e 2909  spider_openedN).
-000007d0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000007e0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000007f0: 6d65 5f5f da07 5f5f 646f 635f 5f72 1b00  me__..__doc__r..
-00000800: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-00000810: 2500 0000 7237 0000 0072 2000 0000 7219  %...r7...r ...r.
-00000820: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000830: 0000 7205 0000 0009 0000 0073 0c00 0000  ..r........s....
-00000840: 0801 0404 0810 0201 0a05 0815 7205 0000  ............r...
-00000850: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000860: 0000 0300 0000 4000 0000 7334 0000 0065  ......@...s4...e
-00000870: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-00000880: 005a 0465 0564 0464 0584 0083 015a 0664  .Z.e.d.d.....Z.d
-00000890: 0664 0784 005a 0764 0864 0984 005a 0864  .d...Z.d.d...Z.d
-000008a0: 0a53 0029 0bda 2341 6275 4479 6e61 6d69  .S.)..#AbuDynami
-000008b0: 6350 726f 7879 446f 776e 6c6f 6164 6572  cProxyDownloader
-000008c0: 4d69 6464 6c65 7761 7265 755b 0000 000a  Middlewareu[....
-000008d0: 2020 2020 e998 bfe5 b883 e4ba 91e5 8aa8      ............
-000008e0: e680 81e4 bba3 e790 8620 2d20 e99a a7e9  ......... - ....
-000008f0: 8193 e9aa 8ce8 af81 e696 b9e5 bc8f efbc  ................
-00000900: 88e5 85b6 e5ae 9ee5 928c e5bf abe4 bba3  ................
-00000910: e790 86e7 9a84 e586 99e6 b395 e4b8 80e8  ................
-00000920: 87b4 efbc 890a 2020 2020 6302 0000 0000  ......    c.....
-00000930: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-00000940: 0000 0073 5600 0000 7c01 a000 6401 6402  ...sV...|...d.d.
-00000950: a102 7d02 7401 6a02 7c02 6403 6404 6405  ..}.t.j.|.d.d.d.
-00000960: 6703 6406 8d02 7d03 7c03 7334 7403 6407  g.d...}.|.s4t.d.
-00000970: 7404 6a05 9b00 9d02 8301 8201 7c02 6403  t.j.........|.d.
-00000980: 1900 7c00 5f06 7c02 6404 1900 7c00 5f07  ..|._.|.d...|._.
-00000990: 7c02 6405 1900 7c00 5f08 6402 5300 2908  |.d...|._.d.S.).
-000009a0: 757f 0000 000a 2020 2020 2020 2020 e4bb  u.....        ..
-000009b0: 8e20 7363 7261 7079 20e9 858d e7bd aee4  . scrapy .......
-000009c0: b8ad e58f 96e5 87ba e58a a8e6 8081 e99a  ................
-000009d0: a7e9 8193 e4bb a3e7 9086 e79a 84e4 bfa1  ................
-000009e0: e681 af0a 2020 2020 2020 2020 4172 6773  ....        Args
-000009f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00000a00: 7474 696e 6773 3a20 7363 7261 7079 20e9  ttings: scrapy .
-00000a10: 858d e7bd aee4 bfa1 e681 af0a 2020 2020  ............    
-00000a20: 2020 2020 7206 0000 004e 7207 0000 0072      r....Nr....r
-00000a30: 0800 0000 7209 0000 0072 0a00 0000 720d  ....r....r....r.
-00000a40: 0000 0072 0e00 0000 7216 0000 0072 1900  ...r....r....r..
-00000a50: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000a60: 0044 0000 0073 1200 0000 0006 0c02 0401  .D...s..........
-00000a70: 0201 08fe 0604 1402 0a01 0a01 7a2c 4162  ............z,Ab
-00000a80: 7544 796e 616d 6963 5072 6f78 7944 6f77  uDynamicProxyDow
-00000a90: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
-00000aa0: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
-00000ab0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00000ac0: 0000 0073 2200 0000 7c00 7c01 6a00 8301  ...s"...|.|.j...
-00000ad0: 7d02 7c01 6a01 6a02 7c02 6a03 7401 6a03  }.|.j.j.|.j.t.j.
-00000ae0: 6401 8d02 0100 7c02 5300 721c 0000 0072  d.....|.S.r....r
-00000af0: 1e00 0000 7221 0000 0072 1900 0000 7219  ....r!...r....r.
-00000b00: 0000 0072 1a00 0000 7225 0000 0056 0000  ...r....r%...V..
-00000b10: 0073 0600 0000 0002 0a01 1401 7a30 4162  .s..........z0Ab
-00000b20: 7544 796e 616d 6963 5072 6f78 7944 6f77  uDynamicProxyDow
-00000b30: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
-00000b40: 652e 6672 6f6d 5f63 7261 776c 6572 6302  e.from_crawlerc.
-00000b50: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000b60: 0000 0043 0000 0073 1800 0000 7c01 6a00  ...C...s....|.j.
-00000b70: a001 6401 7c01 6a02 9b00 9d02 a101 0100  ..d.|.j.........
-00000b80: 6400 5300 2902 4e75 6700 0000 e998 bfe5  d.S.).Nug.......
-00000b90: b883 e4ba 91e5 8aa8 e680 81e9 9aa7 e981  ................
-00000ba0: 93e4 bba3 e790 86e4 b8ad e997 b4e4 bbb6  ................
-00000bb0: 3a20 4162 7544 796e 616d 6963 5072 6f78  : AbuDynamicProx
-00000bc0: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
-00000bd0: 6577 6172 6520 e5b7 b2e5 bc80 e590 afef  eware ..........
-00000be0: bc8c e794 9fe6 9588 e884 9ae6 9cac e4b8  ................
-00000bf0: ba3a 2072 3800 0000 723a 0000 0072 1900  .: r8...r:...r..
-00000c00: 0000 7219 0000 0072 1a00 0000 7220 0000  ..r....r....r ..
-00000c10: 005c 0000 0073 0600 0000 0001 0601 0aff  .\...s..........
-00000c20: 7a31 4162 7544 796e 616d 6963 5072 6f78  z1AbuDynamicProx
-00000c30: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
-00000c40: 6577 6172 652e 7370 6964 6572 5f6f 7065  eware.spider_ope
-00000c50: 6e65 6463 0300 0000 0000 0000 0000 0000  nedc............
-00000c60: 0500 0000 0600 0000 4300 0000 738e 0000  ........C...s...
-00000c70: 007c 016a 00a0 0164 01a1 0172 2064 017c  .|.j...d...r d.|
-00000c80: 006a 029b 009d 027c 016a 0364 023c 006e  .j.....|.j.d.<.n
-00000c90: 347c 016a 00a0 0164 03a1 0172 4064 037c  4|.j...d...r@d.|
-00000ca0: 006a 029b 009d 027c 016a 0364 023c 006e  .j.....|.j.d.<.n
-00000cb0: 147c 026a 04a0 0564 047c 016a 009b 009d  .|.j...d.|.j....
-00000cc0: 02a1 0101 007c 006a 069b 0064 057c 006a  .....|.j...d.|.j
-00000cd0: 079b 009d 037d 0364 0674 08a0 0974 0a7c  .....}.d.t...t.|
-00000ce0: 0364 0783 02a1 01a0 0b64 08a1 0117 007d  .d.......d.....}
-00000cf0: 047c 047c 016a 0c64 093c 0064 0053 0029  .|.|.j.d.<.d.S.)
-00000d00: 0a4e 7226 0000 0072 2a00 0000 722b 0000  .Nr&...r*...r+..
-00000d10: 007a 1372 6571 7565 7374 2075 726c 2065  .z.request url e
-00000d20: 7272 6f72 3a20 7227 0000 007a 0642 6173  rror: r'...z.Bas
-00000d30: 6963 20da 0561 7363 6969 da04 7574 6638  ic ..ascii..utf8
-00000d40: 7a13 5072 6f78 792d 4175 7468 6f72 697a  z.Proxy-Authoriz
-00000d50: 6174 696f 6e29 0d72 2f00 0000 7230 0000  ation).r/...r0..
-00000d60: 0072 1300 0000 7231 0000 0072 3200 0000  .r....r1...r2...
-00000d70: 7233 0000 0072 1400 0000 7215 0000 00da  r3...r....r.....
-00000d80: 0662 6173 6536 34da 1175 726c 7361 6665  .base64..urlsafe
-00000d90: 5f62 3634 656e 636f 6465 da05 6279 7465  _b64encode..byte
-00000da0: 73da 0664 6563 6f64 6572 3400 0000 2905  s..decoder4...).
-00000db0: 7217 0000 0072 3500 0000 7236 0000 005a  r....r5...r6...Z
-00000dc0: 0f70 726f 7879 5f75 7365 725f 7061 7373  .proxy_user_pass
-00000dd0: 5a11 656e 636f 6465 645f 7573 6572 5f70  Z.encoded_user_p
-00000de0: 6173 7372 1900 0000 7219 0000 0072 1a00  assr....r....r..
-00000df0: 0000 7237 0000 0061 0000 0073 1800 0000  ..r7...a...s....
-00000e00: 0001 0c01 1401 0c01 1402 1402 1201 0601  ................
-00000e10: 08ff 0402 02fe 0603 7a33 4162 7544 796e  ........z3AbuDyn
-00000e20: 616d 6963 5072 6f78 7944 6f77 6e6c 6f61  amicProxyDownloa
-00000e30: 6465 724d 6964 646c 6577 6172 652e 7072  derMiddleware.pr
-00000e40: 6f63 6573 735f 7265 7175 6573 744e 2909  ocess_requestN).
-00000e50: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
-00000e60: 3e00 0000 721b 0000 0072 3f00 0000 7225  >...r....r?...r%
-00000e70: 0000 0072 2000 0000 7237 0000 0072 1900  ...r ...r7...r..
-00000e80: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000e90: 0072 4000 0000 3f00 0000 730c 0000 0008  .r@...?...s.....
-00000ea0: 0104 0408 1202 010a 0508 0572 4000 0000  ...........r@...
-00000eb0: 290a 7243 0000 00da 0673 6372 6170 7972  ).rC.....scrapyr
-00000ec0: 0200 0000 da24 6179 7567 6573 7069 6465  .....$ayugespide
-00000ed0: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 4d75  rtools.common.Mu
-00000ee0: 6c74 6950 6c65 7869 6e67 7203 0000 00da  ltiPlexingr.....
-00000ef0: 1e61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
-00000f00: 732e 636f 6d6d 6f6e 2e50 6172 616d 7372  s.common.Paramsr
-00000f10: 0400 0000 da06 6f62 6a65 6374 7205 0000  ......objectr...
-00000f20: 0072 4000 0000 7219 0000 0072 1900 0000  .r@...r....r....
-00000f30: 7219 0000 0072 1a00 0000 da08 3c6d 6f64  r....r......<mod
-00000f40: 756c 653e 0100 0000 730a 0000 0008 020c  ule>....s.......
-00000f50: 020c 010c 0310 36                        ......6
+00000220: 4e46 4947 4eda 0570 726f 7879 da08 7573  NFIGN..proxy..us
+00000230: 6572 6e61 6d65 da08 7061 7373 776f 7264  ername..password
+00000240: a902 da09 6469 6374 5f63 6f6e 66da 086b  ....dict_conf..k
+00000250: 6579 5f6c 6973 74f5 3300 0000 e6b2 a1e6  ey_list.3.......
+00000260: 9c89 e985 8de7 bdae e58a a8e6 8081 e99a  ................
+00000270: a7e9 8193 e4bb a3e7 9086 efbc 8ce9 858d  ................
+00000280: e7bd aee7 a4ba e4be 8be4 b8ba efbc 9aa9  ................
+00000290: 09da 0367 6574 7203 0000 00da 1669 735f  ...getr......is_
+000002a0: 6469 6374 5f6d 6565 745f 6d69 6e5f 6c69  dict_meet_min_li
+000002b0: 6d69 74da 0e41 7373 6572 7469 6f6e 4572  mit..AssertionEr
+000002c0: 726f 7272 0400 0000 da1a 6479 6e61 6d69  rorr......dynami
+000002d0: 635f 7072 6f78 795f 636f 6e66 5f65 7861  c_proxy_conf_exa
+000002e0: 6d70 6c65 da09 7072 6f78 795f 7572 6c72  mple..proxy_urlr
+000002f0: 0800 0000 7209 0000 00a9 04da 0473 656c  ....r........sel
+00000300: 66da 0873 6574 7469 6e67 735a 1264 796e  f..settingsZ.dyn
+00000310: 616d 6963 5f70 726f 7879 5f63 6f6e 665a  amic_proxy_confZ
+00000320: 0869 735f 6d61 7463 68a9 0072 1700 0000  .is_match..r....
+00000330: fa53 2f72 6f6f 742f 6d79 7072 6f6a 2f41  .S/root/myproj/A
+00000340: 7975 6765 5370 6964 6572 546f 6f6c 732f  yugeSpiderTools/
+00000350: 6179 7567 6573 7069 6465 7274 6f6f 6c73  ayugespidertools
+00000360: 2f73 6372 6170 6572 2f6d 6964 646c 6577  /scraper/middlew
+00000370: 6172 6573 2f70 726f 7879 2f64 796e 616d  ares/proxy/dynam
+00000380: 6963 2e70 79da 085f 5f69 6e69 745f 5f0e  ic.py..__init__.
+00000390: 0000 0073 1200 0000 0004 0c02 0401 0201  ...s............
+000003a0: 08fe 0604 1402 0a01 0a01 7a29 4479 6e61  ..........z)Dyna
+000003b0: 6d69 6350 726f 7879 446f 776e 6c6f 6164  micProxyDownload
+000003c0: 6572 4d69 6464 6c65 7761 7265 2e5f 5f69  erMiddleware.__i
+000003d0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+000003e0: 0000 0300 0000 0400 0000 4300 0000 7322  ..........C...s"
+000003f0: 0000 007c 007c 016a 0083 017d 027c 016a  ...|.|.j...}.|.j
+00000400: 016a 027c 026a 0374 016a 0364 018d 0201  .j.|.j.t.j.d....
+00000410: 007c 0253 00a9 024e 2901 da06 7369 676e  .|.S...N)...sign
+00000420: 616c a904 7216 0000 0072 0200 0000 da07  al..r....r......
+00000430: 636f 6e6e 6563 74da 0d73 7069 6465 725f  connect..spider_
+00000440: 6f70 656e 6564 a903 da03 636c 73da 0763  opened....cls..c
+00000450: 7261 776c 6572 da01 7372 1700 0000 7217  rawler..sr....r.
+00000460: 0000 0072 1800 0000 da0c 6672 6f6d 5f63  ...r......from_c
+00000470: 7261 776c 6572 1e00 0000 7306 0000 0000  rawler....s.....
+00000480: 020a 0114 017a 2d44 796e 616d 6963 5072  .....z-DynamicPr
+00000490: 6f78 7944 6f77 6e6c 6f61 6465 724d 6964  oxyDownloaderMid
+000004a0: 646c 6577 6172 652e 6672 6f6d 5f63 7261  dleware.from_cra
+000004b0: 776c 6572 6303 0000 0000 0000 0000 0000  wlerc...........
+000004c0: 0003 0000 0007 0000 0043 0000 0073 9200  .........C...s..
+000004d0: 0000 7c01 6a00 a001 6401 a101 7232 6401  ..|.j...d...r2d.
+000004e0: 7c00 6a02 9b00 6402 7c00 6a03 9b00 6403  |.j...d.|.j...d.
+000004f0: 7c00 6a04 9b00 6404 9d07 7c01 6a05 6405  |.j...d...|.j.d.
+00000500: 3c00 6e48 7c01 6a00 a001 6406 a101 7264  <.nH|.j...d...rd
+00000510: 6406 7c00 6a02 9b00 6402 7c00 6a03 9b00  d.|.j...d.|.j...
+00000520: 6403 7c00 6a04 9b00 6404 9d07 7c01 6a05  d.|.j...d...|.j.
+00000530: 6405 3c00 6e16 7c02 6a06 a007 6407 7c01  d.<.n.|.j...d.|.
+00000540: 6a00 9b00 6408 9d03 a101 0100 6409 7c01  j...d.......d.|.
+00000550: 6a08 640a 3c00 640b 7c01 6a08 640c 3c00  j.d.<.d.|.j.d.<.
+00000560: 6400 5300 290d 4efa 0868 7474 7073 3a2f  d.S.).N..https:/
+00000570: 2ffa 013a fa01 40fa 012f 7207 0000 00fa  /..:..@../r.....
+00000580: 0768 7474 703a 2f2f 7a0d 7265 7175 6573  .http://z.reques
+00000590: 7420 7572 6c3a 207a 2220 6572 726f 7220  t url: z" error 
+000005a0: 7768 656e 2075 7365 2070 726f 7879 206d  when use proxy m
+000005b0: 6964 646c 6577 6172 6573 21da 0563 6c6f  iddlewares!..clo
+000005c0: 7365 da0a 436f 6e6e 6563 7469 6f6e da04  se..Connection..
+000005d0: 677a 6970 7a0f 4163 6365 7074 2d45 6e63  gzipz.Accept-Enc
+000005e0: 6f64 696e 6729 09da 0375 726c da0a 7374  oding)...url..st
+000005f0: 6172 7473 7769 7468 7208 0000 0072 0900  artswithr....r..
+00000600: 0000 7213 0000 00da 046d 6574 61da 0473  ..r......meta..s
+00000610: 6c6f 67da 0469 6e66 6fda 0768 6561 6465  log..info..heade
+00000620: 7273 2903 7215 0000 00da 0772 6571 7565  rs).r......reque
+00000630: 7374 da06 7370 6964 6572 7217 0000 0072  st..spiderr....r
+00000640: 1700 0000 7218 0000 00da 0f70 726f 6365  ....r......proce
+00000650: 7373 5f72 6571 7565 7374 2400 0000 731e  ss_request$...s.
+00000660: 0000 0000 030c 031c fe04 0102 ff04 030c  ................
+00000670: 031c fe04 0102 ff04 0406 010c ff04 050a  ................
+00000680: 027a 3044 796e 616d 6963 5072 6f78 7944  .z0DynamicProxyD
+00000690: 6f77 6e6c 6f61 6465 724d 6964 646c 6577  ownloaderMiddlew
+000006a0: 6172 652e 7072 6f63 6573 735f 7265 7175  are.process_requ
+000006b0: 6573 7463 0200 0000 0000 0000 0000 0000  estc............
+000006c0: 0200 0000 0400 0000 4300 0000 7318 0000  ........C...s...
+000006d0: 007c 016a 00a0 0164 017c 016a 029b 009d  .|.j...d.|.j....
+000006e0: 02a1 0101 0064 0053 0029 024e 755b 0000  .....d.S.).Nu[..
+000006f0: 00e5 8aa8 e680 81e9 9aa7 e981 93e4 bba3  ................
+00000700: e790 86e4 b8ad e997 b4e4 bbb6 3a20 4479  ............: Dy
+00000710: 6e61 6d69 6350 726f 7879 446f 776e 6c6f  namicProxyDownlo
+00000720: 6164 6572 4d69 6464 6c65 7761 7265 20e5  aderMiddleware .
+00000730: b7b2 e5bc 80e5 90af efbc 8ce7 949f e695  ................
+00000740: 88e8 849a e69c ace4 b8ba 3a20 a903 722f  ..........: ..r/
+00000750: 0000 0072 3000 0000 da04 6e61 6d65 a902  ...r0.....name..
+00000760: 7215 0000 0072 3300 0000 7217 0000 0072  r....r3...r....r
+00000770: 1700 0000 7218 0000 0072 1e00 0000 3900  ....r....r....9.
+00000780: 0000 7306 0000 0000 0106 010a ff7a 2e44  ..s..........z.D
+00000790: 796e 616d 6963 5072 6f78 7944 6f77 6e6c  ynamicProxyDownl
+000007a0: 6f61 6465 724d 6964 646c 6577 6172 652e  oaderMiddleware.
+000007b0: 7370 6964 6572 5f6f 7065 6e65 644e 2909  spider_openedN).
+000007c0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000007d0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000007e0: 6d65 5f5f da07 5f5f 646f 635f 5f72 1900  me__..__doc__r..
+000007f0: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
+00000800: 2300 0000 7234 0000 0072 1e00 0000 7217  #...r4...r....r.
+00000810: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000820: 0000 7205 0000 0009 0000 0073 0c00 0000  ..r........s....
+00000830: 0801 0404 0810 0201 0a05 0815 7205 0000  ............r...
+00000840: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000850: 0000 0300 0000 4000 0000 7334 0000 0065  ......@...s4...e
+00000860: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
+00000870: 005a 0465 0564 0464 0584 0083 015a 0664  .Z.e.d.d.....Z.d
+00000880: 0664 0784 005a 0764 0864 0984 005a 0864  .d...Z.d.d...Z.d
+00000890: 0a53 0029 0bda 2341 6275 4479 6e61 6d69  .S.)..#AbuDynami
+000008a0: 6350 726f 7879 446f 776e 6c6f 6164 6572  cProxyDownloader
+000008b0: 4d69 6464 6c65 7761 7265 755b 0000 000a  Middlewareu[....
+000008c0: 2020 2020 e998 bfe5 b883 e4ba 91e5 8aa8      ............
+000008d0: e680 81e4 bba3 e790 8620 2d20 e99a a7e9  ......... - ....
+000008e0: 8193 e9aa 8ce8 af81 e696 b9e5 bc8f efbc  ................
+000008f0: 88e5 85b6 e5ae 9ee5 928c e5bf abe4 bba3  ................
+00000900: e790 86e7 9a84 e586 99e6 b395 e4b8 80e8  ................
+00000910: 87b4 efbc 890a 2020 2020 6302 0000 0000  ......    c.....
+00000920: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00000930: 0000 0073 5600 0000 7c01 a000 6401 6402  ...sV...|...d.d.
+00000940: a102 7d02 7401 6a02 7c02 6403 6404 6405  ..}.t.j.|.d.d.d.
+00000950: 6703 6406 8d02 7d03 7c03 7334 7403 6407  g.d...}.|.s4t.d.
+00000960: 7404 6a05 9b00 9d02 8301 8201 7c02 6403  t.j.........|.d.
+00000970: 1900 7c00 5f06 7c02 6404 1900 7c00 5f07  ..|._.|.d...|._.
+00000980: 7c02 6405 1900 7c00 5f08 6402 5300 2908  |.d...|._.d.S.).
+00000990: 757f 0000 000a 2020 2020 2020 2020 e4bb  u.....        ..
+000009a0: 8e20 7363 7261 7079 20e9 858d e7bd aee4  . scrapy .......
+000009b0: b8ad e58f 96e5 87ba e58a a8e6 8081 e99a  ................
+000009c0: a7e9 8193 e4bb a3e7 9086 e79a 84e4 bfa1  ................
+000009d0: e681 af0a 2020 2020 2020 2020 4172 6773  ....        Args
+000009e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000009f0: 7474 696e 6773 3a20 7363 7261 7079 20e9  ttings: scrapy .
+00000a00: 858d e7bd aee4 bfa1 e681 af0a 2020 2020  ............    
+00000a10: 2020 2020 7206 0000 004e 7207 0000 0072      r....Nr....r
+00000a20: 0800 0000 7209 0000 0072 0a00 0000 720d  ....r....r....r.
+00000a30: 0000 0072 0e00 0000 7214 0000 0072 1700  ...r....r....r..
+00000a40: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000a50: 0044 0000 0073 1200 0000 0006 0c02 0401  .D...s..........
+00000a60: 0201 08fe 0604 1402 0a01 0a01 7a2c 4162  ............z,Ab
+00000a70: 7544 796e 616d 6963 5072 6f78 7944 6f77  uDynamicProxyDow
+00000a80: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
+00000a90: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
+00000aa0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000ab0: 0000 0073 2200 0000 7c00 7c01 6a00 8301  ...s"...|.|.j...
+00000ac0: 7d02 7c01 6a01 6a02 7c02 6a03 7401 6a03  }.|.j.j.|.j.t.j.
+00000ad0: 6401 8d02 0100 7c02 5300 721a 0000 0072  d.....|.S.r....r
+00000ae0: 1c00 0000 721f 0000 0072 1700 0000 7217  ....r....r....r.
+00000af0: 0000 0072 1800 0000 7223 0000 0056 0000  ...r....r#...V..
+00000b00: 0073 0600 0000 0002 0a01 1401 7a30 4162  .s..........z0Ab
+00000b10: 7544 796e 616d 6963 5072 6f78 7944 6f77  uDynamicProxyDow
+00000b20: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
+00000b30: 652e 6672 6f6d 5f63 7261 776c 6572 6302  e.from_crawlerc.
+00000b40: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000b50: 0000 0043 0000 0073 1800 0000 7c01 6a00  ...C...s....|.j.
+00000b60: a001 6401 7c01 6a02 9b00 9d02 a101 0100  ..d.|.j.........
+00000b70: 6400 5300 2902 4e75 6700 0000 e998 bfe5  d.S.).Nug.......
+00000b80: b883 e4ba 91e5 8aa8 e680 81e9 9aa7 e981  ................
+00000b90: 93e4 bba3 e790 86e4 b8ad e997 b4e4 bbb6  ................
+00000ba0: 3a20 4162 7544 796e 616d 6963 5072 6f78  : AbuDynamicProx
+00000bb0: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
+00000bc0: 6577 6172 6520 e5b7 b2e5 bc80 e590 afef  eware ..........
+00000bd0: bc8c e794 9fe6 9588 e884 9ae6 9cac e4b8  ................
+00000be0: ba3a 2072 3500 0000 7237 0000 0072 1700  .: r5...r7...r..
+00000bf0: 0000 7217 0000 0072 1800 0000 721e 0000  ..r....r....r...
+00000c00: 005c 0000 0073 0600 0000 0001 0601 0aff  .\...s..........
+00000c10: 7a31 4162 7544 796e 616d 6963 5072 6f78  z1AbuDynamicProx
+00000c20: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
+00000c30: 6577 6172 652e 7370 6964 6572 5f6f 7065  eware.spider_ope
+00000c40: 6e65 6463 0300 0000 0000 0000 0000 0000  nedc............
+00000c50: 0500 0000 0600 0000 4300 0000 738e 0000  ........C...s...
+00000c60: 007c 016a 00a0 0164 01a1 0172 2064 017c  .|.j...d...r d.|
+00000c70: 006a 029b 009d 027c 016a 0364 023c 006e  .j.....|.j.d.<.n
+00000c80: 347c 016a 00a0 0164 03a1 0172 4064 037c  4|.j...d...r@d.|
+00000c90: 006a 029b 009d 027c 016a 0364 023c 006e  .j.....|.j.d.<.n
+00000ca0: 147c 026a 04a0 0564 047c 016a 009b 009d  .|.j...d.|.j....
+00000cb0: 02a1 0101 007c 006a 069b 0064 057c 006a  .....|.j...d.|.j
+00000cc0: 079b 009d 037d 0364 0674 08a0 0974 0a7c  .....}.d.t...t.|
+00000cd0: 0364 0783 02a1 01a0 0b64 08a1 0117 007d  .d.......d.....}
+00000ce0: 047c 047c 016a 0c64 093c 0064 0053 0029  .|.|.j.d.<.d.S.)
+00000cf0: 0a4e 7224 0000 0072 0700 0000 7228 0000  .Nr$...r....r(..
+00000d00: 007a 1372 6571 7565 7374 2075 726c 2065  .z.request url e
+00000d10: 7272 6f72 3a20 7225 0000 007a 0642 6173  rror: r%...z.Bas
+00000d20: 6963 20da 0561 7363 6969 da04 7574 6638  ic ..ascii..utf8
+00000d30: 7a13 5072 6f78 792d 4175 7468 6f72 697a  z.Proxy-Authoriz
+00000d40: 6174 696f 6e29 0d72 2c00 0000 722d 0000  ation).r,...r-..
+00000d50: 0072 1300 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00000d60: 7230 0000 0072 0800 0000 7209 0000 00da  r0...r....r.....
+00000d70: 0662 6173 6536 34da 1175 726c 7361 6665  .base64..urlsafe
+00000d80: 5f62 3634 656e 636f 6465 da05 6279 7465  _b64encode..byte
+00000d90: 73da 0664 6563 6f64 6572 3100 0000 2905  s..decoder1...).
+00000da0: 7215 0000 0072 3200 0000 7233 0000 005a  r....r2...r3...Z
+00000db0: 0f70 726f 7879 5f75 7365 725f 7061 7373  .proxy_user_pass
+00000dc0: 5a11 656e 636f 6465 645f 7573 6572 5f70  Z.encoded_user_p
+00000dd0: 6173 7372 1700 0000 7217 0000 0072 1800  assr....r....r..
+00000de0: 0000 7234 0000 0061 0000 0073 1800 0000  ..r4...a...s....
+00000df0: 0001 0c01 1401 0c01 1402 1402 1201 0601  ................
+00000e00: 08ff 0402 02fe 0603 7a33 4162 7544 796e  ........z3AbuDyn
+00000e10: 616d 6963 5072 6f78 7944 6f77 6e6c 6f61  amicProxyDownloa
+00000e20: 6465 724d 6964 646c 6577 6172 652e 7072  derMiddleware.pr
+00000e30: 6f63 6573 735f 7265 7175 6573 744e 2909  ocess_requestN).
+00000e40: 7238 0000 0072 3900 0000 723a 0000 0072  r8...r9...r:...r
+00000e50: 3b00 0000 7219 0000 0072 3c00 0000 7223  ;...r....r<...r#
+00000e60: 0000 0072 1e00 0000 7234 0000 0072 1700  ...r....r4...r..
+00000e70: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000e80: 0072 3d00 0000 3f00 0000 730c 0000 0008  .r=...?...s.....
+00000e90: 0104 0408 1202 010a 0508 0572 3d00 0000  ...........r=...
+00000ea0: 290a 7240 0000 00da 0673 6372 6170 7972  ).r@.....scrapyr
+00000eb0: 0200 0000 da24 6179 7567 6573 7069 6465  .....$ayugespide
+00000ec0: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 6d75  rtools.common.mu
+00000ed0: 6c74 6970 6c65 7869 6e67 7203 0000 00da  ltiplexingr.....
+00000ee0: 1e61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
+00000ef0: 732e 636f 6d6d 6f6e 2e70 6172 616d 7372  s.common.paramsr
+00000f00: 0400 0000 da06 6f62 6a65 6374 7205 0000  ......objectr...
+00000f10: 0072 3d00 0000 7217 0000 0072 1700 0000  .r=...r....r....
+00000f20: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
+00000f30: 756c 653e 0100 0000 730a 0000 0008 020c  ule>....s.......
+00000f40: 020c 010c 0310 36                        ......6
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 11 07:45:43 2023 UTC, .py size: 2869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2710 3564 350b 0000  U.......'.5d5...
+00000000: 550d 0d0a 0000 0000 d58f 4864 3c0b 0000  U.........Hd<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6508 8303  ..G.d.d...d.e...
 00000070: 5a09 6401 5300 2907 e900 0000 004e 2901  Z.d.S.)......N).
@@ -30,162 +30,162 @@
 000001d0: 2020 e588 9de5 a78b e58c 96e7 8bac e4ba    ..............
 000001e0: abe4 bba3 e790 86e8 aebe e7bd ae0a 2020  ..............  
 000001f0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
 00000200: 2020 2020 2020 2020 6578 636c 7573 6976          exclusiv
 00000210: 655f 7072 6f78 795f 636f 6e66 3a20 e4bd  e_proxy_conf: ..
 00000220: bfe7 94a8 e79a 84e7 8bac e4ba abe4 bba3  ................
 00000230: e790 86e7 9a84 e985 8de7 bdae e4bf a1e6  ................
-00000240: 81af 0a20 2020 2020 2020 204e da09 5052  ...        N..PR
-00000250: 4f58 595f 5552 4cda 0855 5345 524e 414d  OXY_URL..USERNAM
-00000260: 45da 0850 4153 5357 4f52 44da 0b50 524f  E..PASSWORD..PRO
-00000270: 5859 5f49 4e44 4558 2902 da09 6469 6374  XY_INDEX)...dict
-00000280: 5f63 6f6e 66da 086b 6579 5f6c 6973 7475  _conf..key_listu
-00000290: 2d00 0000 e6b2 a1e6 9c89 e985 8de7 bdae  -...............
-000002a0: e78b ace4 baab e4bb a3e7 9086 efbc 8ce9  ................
-000002b0: 858d e7bd aee7 a4ba e4be 8be4 b8ba efbc  ................
-000002c0: 9a29 0ada 0570 726f 7879 7203 0000 00da  .)...proxyr.....
-000002d0: 1669 735f 6469 6374 5f6d 6565 745f 6d69  .is_dict_meet_mi
-000002e0: 6e5f 6c69 6d69 74da 0e41 7373 6572 7469  n_limit..Asserti
-000002f0: 6f6e 4572 726f 7272 0400 0000 da1c 6578  onErrorr......ex
-00000300: 636c 7573 6976 655f 7072 6f78 795f 636f  clusive_proxy_co
-00000310: 6e66 5f65 7861 6d70 6c65 da09 7072 6f78  nf_example..prox
-00000320: 795f 7572 6cda 0875 7365 726e 616d 65da  y_url..username.
-00000330: 0870 6173 7377 6f72 64da 0b70 726f 7879  .password..proxy
-00000340: 5f69 6e64 6578 2903 da04 7365 6c66 da14  _index)...self..
-00000350: 6578 636c 7573 6976 655f 7072 6f78 795f  exclusive_proxy_
-00000360: 636f 6e66 da08 6973 5f6d 6174 6368 a900  conf..is_match..
-00000370: 7217 0000 00fa 552f 726f 6f74 2f6d 7970  r.....U/root/myp
-00000380: 726f 6a2f 4179 7567 6553 7069 6465 7254  roj/AyugeSpiderT
-00000390: 6f6f 6c73 2f61 7975 6765 7370 6964 6572  ools/ayugespider
-000003a0: 746f 6f6c 732f 7363 7261 7065 722f 6d69  tools/scraper/mi
-000003b0: 6464 6c65 7761 7265 732f 7072 6f78 792f  ddlewares/proxy/
-000003c0: 6578 636c 7573 6976 652e 7079 da08 5f5f  exclusive.py..__
-000003d0: 696e 6974 5f5f 0f00 0000 7314 0000 0000  init__....s.....
-000003e0: 0606 0204 0102 010a fe06 0414 020a 010a  ................
-000003f0: 010a 017a 2b45 7863 6c75 7369 7665 5072  ...z+ExclusivePr
-00000400: 6f78 7944 6f77 6e6c 6f61 6465 724d 6964  oxyDownloaderMid
-00000410: 646c 6577 6172 652e 5f5f 696e 6974 5f5f  dleware.__init__
-00000420: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000430: 0005 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
-00000440: 7c01 6a00 a001 6401 6400 a102 6402 8d01  |.j...d.d...d...
-00000450: 7d02 7c01 6a02 6a03 7c02 6a04 7402 6a04  }.|.j.j.|.j.t.j.
-00000460: 6403 8d02 0100 7c02 5300 2904 4e5a 1645  d.....|.S.).NZ.E
-00000470: 5843 4c55 5349 5645 5f50 524f 5859 5f43  XCLUSIVE_PROXY_C
-00000480: 4f4e 4649 4729 0172 1500 0000 2901 da06  ONFIG).r....)...
-00000490: 7369 676e 616c 2905 da08 7365 7474 696e  signal)...settin
-000004a0: 6773 da03 6765 7472 0200 0000 da07 636f  gs..getr......co
-000004b0: 6e6e 6563 74da 0d73 7069 6465 725f 6f70  nnect..spider_op
-000004c0: 656e 6564 2903 da03 636c 73da 0763 7261  ened)...cls..cra
-000004d0: 776c 6572 da01 7372 1700 0000 7217 0000  wler..sr....r...
-000004e0: 0072 1800 0000 da0c 6672 6f6d 5f63 7261  .r......from_cra
-000004f0: 776c 6572 2200 0000 730a 0000 0000 0202  wler"...s.......
-00000500: 010c ff06 0314 017a 2f45 7863 6c75 7369  .......z/Exclusi
-00000510: 7665 5072 6f78 7944 6f77 6e6c 6f61 6465  veProxyDownloade
-00000520: 724d 6964 646c 6577 6172 652e 6672 6f6d  rMiddleware.from
-00000530: 5f63 7261 776c 6572 6301 0000 0000 0000  _crawlerc.......
-00000540: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00000550: 0073 7200 0000 7a50 7400 a001 7c00 6a02  .sr...zPt...|.j.
-00000560: a101 7d01 7c01 a003 a100 a001 6401 a101  ..}.|.......d...
-00000570: a001 6402 a101 7d02 7c02 a004 a100 0100  ..d...}.|.......
-00000580: 7c00 6a05 7406 7c02 8301 6b00 7246 7c02  |.j.t.|...k.rF|.
-00000590: 7c00 6a05 1900 7c00 5f07 6e08 7408 6403  |.j...|._.n.t.d.
-000005a0: 8301 8201 5700 6e1c 0400 7408 6b0a 726c  ....W.n...t.k.rl
-000005b0: 0100 0100 0100 7408 6404 8301 8201 5900  ......t.d.....Y.
-000005c0: 6e02 5800 6405 5300 2906 7540 0000 00e8  n.X.d.S.).u@....
-000005d0: 8eb7 e58f 96e7 8bac e4ba abe4 bba3 e790  ................
-000005e0: 86e6 8ea5 e58f a3e7 9a84 e7b4 a2e5 bc95  ................
-000005f0: e4b8 ba20 7072 6f78 795f 696e 6465 7820  ... proxy_index 
-00000600: e79a 84e4 bba3 e790 86e4 bfa1 e681 afda  ................
-00000610: 0464 6174 61da 0a70 726f 7879 5f6c 6973  .data..proxy_lis
-00000620: 7475 4500 0000 e78b ace4 baab e4bb a3e7  tuE.............
-00000630: 9086 e7b4 a2e5 bc95 e8b6 85e5 87ba e88c  ................
-00000640: 83e5 9bb4 efbc 8ce8 afb7 e7a1 aee8 aea4  ................
-00000650: e78b ace4 baab e4bb a3e7 9086 e69c 8de5  ................
-00000660: 8aa1 e683 85e5 86b5 e380 8275 3000 0000  ...........u0...
-00000670: e88e b7e5 8f96 e78b ace4 baab e4bb a3e7  ................
-00000680: 9086 e698 afe5 a4b1 e8b4 a5ef bc8c e8af  ................
-00000690: b7e5 8f8a e697 b6e6 9fa5 e79c 8be3 8082  ................
-000006a0: 4e29 09da 0872 6571 7565 7374 7372 1c00  N)...requestsr..
-000006b0: 0000 7210 0000 00da 046a 736f 6eda 0473  ..r......json..s
-000006c0: 6f72 7472 1300 0000 da03 6c65 6e72 0c00  ortr......lenr..
-000006d0: 0000 da09 4578 6365 7074 696f 6e29 0372  ....Exception).r
-000006e0: 1400 0000 da01 7272 2400 0000 7217 0000  ......rr$...r...
-000006f0: 0072 1700 0000 7218 0000 00da 0c67 6574  .r....r......get
-00000700: 5f70 726f 7879 5f69 702a 0000 0073 1200  _proxy_ip*...s..
-00000710: 0000 0002 0201 0c01 1401 0801 0e01 0e02  ................
-00000720: 0c02 0e01 7a2f 4578 636c 7573 6976 6550  ....z/ExclusiveP
-00000730: 726f 7879 446f 776e 6c6f 6164 6572 4d69  roxyDownloaderMi
-00000740: 6464 6c65 7761 7265 2e67 6574 5f70 726f  ddleware.get_pro
-00000750: 7879 5f69 7063 0300 0000 0000 0000 0000  xy_ipc..........
-00000760: 0000 0500 0000 0600 0000 4300 0000 738e  ..........C...s.
-00000770: 0000 007c 016a 00a0 0164 01a1 0172 2064  ...|.j...d...r d
-00000780: 017c 006a 029b 009d 027c 016a 0364 023c  .|.j.....|.j.d.<
-00000790: 006e 347c 016a 00a0 0164 03a1 0172 4064  .n4|.j...d...r@d
-000007a0: 037c 006a 029b 009d 027c 016a 0364 023c  .|.j.....|.j.d.<
-000007b0: 006e 147c 026a 04a0 0564 047c 016a 009b  .n.|.j...d.|.j..
-000007c0: 009d 02a1 0101 007c 006a 069b 0064 057c  .......|.j...d.|
-000007d0: 006a 079b 009d 037d 0364 0674 08a0 0974  .j.....}.d.t...t
-000007e0: 0a7c 0364 0783 02a1 01a0 0b64 08a1 0117  .|.d.......d....
-000007f0: 007d 047c 047c 016a 0c64 093c 0064 0053  .}.|.|.j.d.<.d.S
-00000800: 0029 0a4e 7a08 6874 7470 733a 2f2f 720c  .).Nz.https://r.
-00000810: 0000 007a 0768 7474 703a 2f2f 7a13 7265  ...z.http://z.re
-00000820: 7175 6573 7420 7572 6c20 6572 726f 723a  quest url error:
-00000830: 20fa 013a 7a06 4261 7369 6320 da05 6173   ..:z.Basic ..as
-00000840: 6369 69da 0475 7466 387a 1350 726f 7879  cii..utf8z.Proxy
-00000850: 2d41 7574 686f 7269 7a61 7469 6f6e 290d  -Authorization).
-00000860: da03 7572 6cda 0a73 7461 7274 7377 6974  ..url..startswit
-00000870: 6872 0c00 0000 da04 6d65 7461 da04 736c  hr......meta..sl
-00000880: 6f67 da04 696e 666f 7211 0000 0072 1200  og..infor....r..
-00000890: 0000 da06 6261 7365 3634 da11 7572 6c73  ....base64..urls
-000008a0: 6166 655f 6236 3465 6e63 6f64 65da 0562  afe_b64encode..b
-000008b0: 7974 6573 da06 6465 636f 6465 da07 6865  ytes..decode..he
-000008c0: 6164 6572 7329 0572 1400 0000 da07 7265  aders).r......re
-000008d0: 7175 6573 74da 0673 7069 6465 72da 0f70  quest..spider..p
-000008e0: 726f 7879 5f75 7365 725f 7061 7373 da11  roxy_user_pass..
-000008f0: 656e 636f 6465 645f 7573 6572 5f70 6173  encoded_user_pas
-00000900: 7372 1700 0000 7217 0000 0072 1800 0000  sr....r....r....
-00000910: da0f 7072 6f63 6573 735f 7265 7175 6573  ..process_reques
-00000920: 7438 0000 0073 1800 0000 0001 0c01 1401  t8...s..........
-00000930: 0c01 1402 1402 1201 0601 08ff 0402 02fe  ................
-00000940: 0603 7a32 4578 636c 7573 6976 6550 726f  ..z2ExclusivePro
-00000950: 7879 446f 776e 6c6f 6164 6572 4d69 6464  xyDownloaderMidd
-00000960: 6c65 7761 7265 2e70 726f 6365 7373 5f72  leware.process_r
-00000970: 6571 7565 7374 6302 0000 0000 0000 0000  equestc.........
-00000980: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00000990: 2800 0000 7c00 a000 a100 0100 7c01 6a01  (...|.......|.j.
-000009a0: a002 6401 7c01 6a03 9b00 6402 7c00 6a04  ..d.|.j...d.|.j.
-000009b0: 9b00 9d04 a101 0100 6400 5300 2903 4e75  ........d.S.).Nu
-000009c0: 5700 0000 e78b ace4 baab e4bb a3e7 9086  W...............
-000009d0: e4b8 ade9 97b4 e4bb b63a 2045 7863 6c75  .........: Exclu
-000009e0: 7369 7665 5072 6f78 7944 6f77 6e6c 6f61  siveProxyDownloa
-000009f0: 6465 724d 6964 646c 6577 6172 6520 e5b7  derMiddleware ..
-00000a00: b2e5 bc80 e590 afef bc8c e794 9fe6 9588  ................
-00000a10: e884 9ae6 9cac e4b8 ba3a 2075 1a00 0000  .........: u....
-00000a20: efbc 8ce5 bd93 e589 8de7 8bac e4ba abe4  ................
-00000a30: bba3 e790 86e4 b8ba 3a20 2905 722b 0000  ........: ).r+..
-00000a40: 0072 3200 0000 7233 0000 00da 046e 616d  .r2...r3.....nam
-00000a50: 6572 0c00 0000 2902 7214 0000 0072 3a00  er....).r....r:.
-00000a60: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000a70: 0072 1e00 0000 4600 0000 7308 0000 0000  .r....F...s.....
-00000a80: 0108 0106 0112 ff7a 3045 7863 6c75 7369  .......z0Exclusi
-00000a90: 7665 5072 6f78 7944 6f77 6e6c 6f61 6465  veProxyDownloade
-00000aa0: 724d 6964 646c 6577 6172 652e 7370 6964  rMiddleware.spid
-00000ab0: 6572 5f6f 7065 6e65 644e 290a da08 5f5f  er_openedN)...__
-00000ac0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000ad0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000ae0: da07 5f5f 646f 635f 5f72 1900 0000 da0b  ..__doc__r......
-00000af0: 636c 6173 736d 6574 686f 6472 2200 0000  classmethodr"...
-00000b00: 722b 0000 0072 3d00 0000 721e 0000 0072  r+...r=...r....r
-00000b10: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000b20: 0000 0072 0500 0000 0a00 0000 730e 0000  ...r........s...
-00000b30: 0008 0104 0408 1302 010a 0708 0e08 0e72  ...............r
-00000b40: 0500 0000 290a 7234 0000 0072 2500 0000  ....).r4...r%...
-00000b50: da06 7363 7261 7079 7202 0000 00da 2461  ..scrapyr.....$a
-00000b60: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
-00000b70: 636f 6d6d 6f6e 2e4d 756c 7469 506c 6578  common.MultiPlex
-00000b80: 696e 6772 0300 0000 da1e 6179 7567 6573  ingr......ayuges
-00000b90: 7069 6465 7274 6f6f 6c73 2e63 6f6d 6d6f  pidertools.commo
-00000ba0: 6e2e 5061 7261 6d73 7204 0000 00da 066f  n.Paramsr......o
-00000bb0: 626a 6563 7472 0500 0000 7217 0000 0072  bjectr....r....r
-00000bc0: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-00000bd0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000be0: 0008 0208 010c 020c 010c 03              ...........
+00000240: 81af 0a20 2020 2020 2020 204e da05 7072  ...        N..pr
+00000250: 6f78 79da 0875 7365 726e 616d 65da 0870  oxy..username..p
+00000260: 6173 7377 6f72 64da 0569 6e64 6578 2902  assword..index).
+00000270: da09 6469 6374 5f63 6f6e 66da 086b 6579  ..dict_conf..key
+00000280: 5f6c 6973 7475 2d00 0000 e6b2 a1e6 9c89  _listu-.........
+00000290: e985 8de7 bdae e78b ace4 baab e4bb a3e7  ................
+000002a0: 9086 efbc 8ce9 858d e7bd aee7 a4ba e4be  ................
+000002b0: 8be4 b8ba efbc 9a29 0a72 0600 0000 7203  .......).r....r.
+000002c0: 0000 00da 1669 735f 6469 6374 5f6d 6565  .....is_dict_mee
+000002d0: 745f 6d69 6e5f 6c69 6d69 74da 0e41 7373  t_min_limit..Ass
+000002e0: 6572 7469 6f6e 4572 726f 7272 0400 0000  ertionErrorr....
+000002f0: da1c 6578 636c 7573 6976 655f 7072 6f78  ..exclusive_prox
+00000300: 795f 636f 6e66 5f65 7861 6d70 6c65 da09  y_conf_example..
+00000310: 7072 6f78 795f 7572 6c72 0700 0000 7208  proxy_urlr....r.
+00000320: 0000 00da 0b70 726f 7879 5f69 6e64 6578  .....proxy_index
+00000330: 2903 da04 7365 6c66 da14 6578 636c 7573  )...self..exclus
+00000340: 6976 655f 7072 6f78 795f 636f 6e66 da08  ive_proxy_conf..
+00000350: 6973 5f6d 6174 6368 a900 7214 0000 00fa  is_match..r.....
+00000360: 552f 726f 6f74 2f6d 7970 726f 6a2f 4179  U/root/myproj/Ay
+00000370: 7567 6553 7069 6465 7254 6f6f 6c73 2f61  ugeSpiderTools/a
+00000380: 7975 6765 7370 6964 6572 746f 6f6c 732f  yugespidertools/
+00000390: 7363 7261 7065 722f 6d69 6464 6c65 7761  scraper/middlewa
+000003a0: 7265 732f 7072 6f78 792f 6578 636c 7573  res/proxy/exclus
+000003b0: 6976 652e 7079 da08 5f5f 696e 6974 5f5f  ive.py..__init__
+000003c0: 0f00 0000 7314 0000 0000 0606 0204 0102  ....s...........
+000003d0: 010a fe06 0414 020a 010a 010a 017a 2b45  .............z+E
+000003e0: 7863 6c75 7369 7665 5072 6f78 7944 6f77  xclusiveProxyDow
+000003f0: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
+00000400: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
+00000410: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00000420: 0000 0073 2c00 0000 7c00 7c01 6a00 a001  ...s,...|.|.j...
+00000430: 6401 6400 a102 6402 8d01 7d02 7c01 6a02  d.d...d...}.|.j.
+00000440: 6a03 7c02 6a04 7402 6a04 6403 8d02 0100  j.|.j.t.j.d.....
+00000450: 7c02 5300 2904 4e5a 1645 5843 4c55 5349  |.S.).NZ.EXCLUSI
+00000460: 5645 5f50 524f 5859 5f43 4f4e 4649 4729  VE_PROXY_CONFIG)
+00000470: 0172 1200 0000 2901 da06 7369 676e 616c  .r....)...signal
+00000480: 2905 da08 7365 7474 696e 6773 da03 6765  )...settings..ge
+00000490: 7472 0200 0000 da07 636f 6e6e 6563 74da  tr......connect.
+000004a0: 0d73 7069 6465 725f 6f70 656e 6564 2903  .spider_opened).
+000004b0: da03 636c 73da 0763 7261 776c 6572 da01  ..cls..crawler..
+000004c0: 7372 1400 0000 7214 0000 0072 1500 0000  sr....r....r....
+000004d0: da0c 6672 6f6d 5f63 7261 776c 6572 2200  ..from_crawler".
+000004e0: 0000 730a 0000 0000 0202 010c ff06 0314  ..s.............
+000004f0: 017a 2f45 7863 6c75 7369 7665 5072 6f78  .z/ExclusiveProx
+00000500: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
+00000510: 6577 6172 652e 6672 6f6d 5f63 7261 776c  eware.from_crawl
+00000520: 6572 6301 0000 0000 0000 0000 0000 0003  erc.............
+00000530: 0000 0008 0000 0043 0000 0073 7200 0000  .......C...sr...
+00000540: 7a50 7400 a001 7c00 6a02 a101 7d01 7c01  zPt...|.j...}.|.
+00000550: a003 a100 a001 6401 a101 a001 6402 a101  ......d.....d...
+00000560: 7d02 7c02 a004 a100 0100 7c00 6a05 7406  }.|.......|.j.t.
+00000570: 7c02 8301 6b00 7246 7c02 7c00 6a05 1900  |...k.rF|.|.j...
+00000580: 7c00 5f07 6e08 7408 6403 8301 8201 5700  |._.n.t.d.....W.
+00000590: 6e1c 0400 7408 6b0a 726c 0100 0100 0100  n...t.k.rl......
+000005a0: 7408 6404 8301 8201 5900 6e02 5800 6405  t.d.....Y.n.X.d.
+000005b0: 5300 2906 7540 0000 00e8 8eb7 e58f 96e7  S.).u@..........
+000005c0: 8bac e4ba abe4 bba3 e790 86e6 8ea5 e58f  ................
+000005d0: a3e7 9a84 e7b4 a2e5 bc95 e4b8 ba20 7072  ............. pr
+000005e0: 6f78 795f 696e 6465 7820 e79a 84e4 bba3  oxy_index ......
+000005f0: e790 86e4 bfa1 e681 afda 0464 6174 61da  ...........data.
+00000600: 0a70 726f 7879 5f6c 6973 7475 4500 0000  .proxy_listuE...
+00000610: e78b ace4 baab e4bb a3e7 9086 e7b4 a2e5  ................
+00000620: bc95 e8b6 85e5 87ba e88c 83e5 9bb4 efbc  ................
+00000630: 8ce8 afb7 e7a1 aee8 aea4 e78b ace4 baab  ................
+00000640: e4bb a3e7 9086 e69c 8de5 8aa1 e683 85e5  ................
+00000650: 86b5 e380 8275 4b00 0000 e88e b7e5 8f96  .....uK.........
+00000660: e78b ace4 baab e4bb a3e7 9086 e697 b6e5  ................
+00000670: a4b1 e8b4 a5ef bc8c e8af b7e6 9fa5 e79c  ................
+00000680: 8be7 8bac e4ba abe9 858d e7bd aee5 8f8a  ................
+00000690: e7bd 91e7 bb9c e698 afe5 90a6 e6ad a3e5  ................
+000006a0: b8b8 e380 824e 2909 da08 7265 7175 6573  .....N)...reques
+000006b0: 7473 7219 0000 0072 0f00 0000 da04 6a73  tsr....r......js
+000006c0: 6f6e da04 736f 7274 7210 0000 00da 036c  on..sortr......l
+000006d0: 656e 7206 0000 00da 0945 7863 6570 7469  enr......Excepti
+000006e0: 6f6e 2903 7211 0000 00da 0172 7221 0000  on).r......rr!..
+000006f0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000700: da0c 6765 745f 7072 6f78 795f 6970 2a00  ..get_proxy_ip*.
+00000710: 0000 7312 0000 0000 0202 010c 0114 0108  ..s.............
+00000720: 010e 010e 020c 020e 017a 2f45 7863 6c75  .........z/Exclu
+00000730: 7369 7665 5072 6f78 7944 6f77 6e6c 6f61  siveProxyDownloa
+00000740: 6465 724d 6964 646c 6577 6172 652e 6765  derMiddleware.ge
+00000750: 745f 7072 6f78 795f 6970 6303 0000 0000  t_proxy_ipc.....
+00000760: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
+00000770: 0000 0073 8e00 0000 7c01 6a00 a001 6401  ...s....|.j...d.
+00000780: a101 7220 6401 7c00 6a02 9b00 9d02 7c01  ..r d.|.j.....|.
+00000790: 6a03 6402 3c00 6e34 7c01 6a00 a001 6403  j.d.<.n4|.j...d.
+000007a0: a101 7240 6403 7c00 6a02 9b00 9d02 7c01  ..r@d.|.j.....|.
+000007b0: 6a03 6402 3c00 6e14 7c02 6a04 a005 6404  j.d.<.n.|.j...d.
+000007c0: 7c01 6a00 9b00 9d02 a101 0100 7c00 6a06  |.j.........|.j.
+000007d0: 9b00 6405 7c00 6a07 9b00 9d03 7d03 6406  ..d.|.j.....}.d.
+000007e0: 7408 a009 740a 7c03 6407 8302 a101 a00b  t...t.|.d.......
+000007f0: 6408 a101 1700 7d04 7c04 7c01 6a0c 6409  d.....}.|.|.j.d.
+00000800: 3c00 6400 5300 290a 4e7a 0868 7474 7073  <.d.S.).Nz.https
+00000810: 3a2f 2f72 0600 0000 7a07 6874 7470 3a2f  ://r....z.http:/
+00000820: 2f7a 1372 6571 7565 7374 2075 726c 2065  /z.request url e
+00000830: 7272 6f72 3a20 fa01 3a7a 0642 6173 6963  rror: ..:z.Basic
+00000840: 20da 0561 7363 6969 da04 7574 6638 7a13   ..ascii..utf8z.
+00000850: 5072 6f78 792d 4175 7468 6f72 697a 6174  Proxy-Authorizat
+00000860: 696f 6e29 0dda 0375 726c da0a 7374 6172  ion)...url..star
+00000870: 7473 7769 7468 7206 0000 00da 046d 6574  tswithr......met
+00000880: 61da 0473 6c6f 67da 0469 6e66 6f72 0700  a..slog..infor..
+00000890: 0000 7208 0000 00da 0662 6173 6536 34da  ..r......base64.
+000008a0: 1175 726c 7361 6665 5f62 3634 656e 636f  .urlsafe_b64enco
+000008b0: 6465 da05 6279 7465 73da 0664 6563 6f64  de..bytes..decod
+000008c0: 65da 0768 6561 6465 7273 2905 7211 0000  e..headers).r...
+000008d0: 00da 0772 6571 7565 7374 da06 7370 6964  ...request..spid
+000008e0: 6572 da0f 7072 6f78 795f 7573 6572 5f70  er..proxy_user_p
+000008f0: 6173 73da 1165 6e63 6f64 6564 5f75 7365  ass..encoded_use
+00000900: 725f 7061 7373 7214 0000 0072 1400 0000  r_passr....r....
+00000910: 7215 0000 00da 0f70 726f 6365 7373 5f72  r......process_r
+00000920: 6571 7565 7374 3800 0000 7318 0000 0000  equest8...s.....
+00000930: 010c 0114 010c 0114 0214 0212 0106 0108  ................
+00000940: ff04 0202 fe06 037a 3245 7863 6c75 7369  .......z2Exclusi
+00000950: 7665 5072 6f78 7944 6f77 6e6c 6f61 6465  veProxyDownloade
+00000960: 724d 6964 646c 6577 6172 652e 7072 6f63  rMiddleware.proc
+00000970: 6573 735f 7265 7175 6573 7463 0200 0000  ess_requestc....
+00000980: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000990: 4300 0000 7328 0000 007c 00a0 00a1 0001  C...s(...|......
+000009a0: 007c 016a 01a0 0264 017c 016a 039b 0064  .|.j...d.|.j...d
+000009b0: 027c 006a 049b 009d 04a1 0101 0064 0053  .|.j.........d.S
+000009c0: 0029 034e 7557 0000 00e7 8bac e4ba abe4  .).NuW..........
+000009d0: bba3 e790 86e4 b8ad e997 b4e4 bbb6 3a20  ..............: 
+000009e0: 4578 636c 7573 6976 6550 726f 7879 446f  ExclusiveProxyDo
+000009f0: 776e 6c6f 6164 6572 4d69 6464 6c65 7761  wnloaderMiddlewa
+00000a00: 7265 20e5 b7b2 e5bc 80e5 90af efbc 8ce7  re .............
+00000a10: 949f e695 88e8 849a e69c ace4 b8ba 3a20  ..............: 
+00000a20: 751a 0000 00ef bc8c e5bd 93e5 898d e78b  u...............
+00000a30: ace4 baab e4bb a3e7 9086 e4b8 ba3a 2029  .............: )
+00000a40: 0572 2800 0000 722f 0000 0072 3000 0000  .r(...r/...r0...
+00000a50: da04 6e61 6d65 7206 0000 0029 0272 1100  ..namer....).r..
+00000a60: 0000 7237 0000 0072 1400 0000 7214 0000  ..r7...r....r...
+00000a70: 0072 1500 0000 721b 0000 0046 0000 0073  .r....r....F...s
+00000a80: 0800 0000 0001 0801 0601 12ff 7a30 4578  ............z0Ex
+00000a90: 636c 7573 6976 6550 726f 7879 446f 776e  clusiveProxyDown
+00000aa0: 6c6f 6164 6572 4d69 6464 6c65 7761 7265  loaderMiddleware
+00000ab0: 2e73 7069 6465 725f 6f70 656e 6564 4e29  .spider_openedN)
+00000ac0: 0ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000ad0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000ae0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7216  ame__..__doc__r.
+00000af0: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
+00000b00: 721f 0000 0072 2800 0000 723a 0000 0072  r....r(...r:...r
+00000b10: 1b00 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+00000b20: 0000 0072 1500 0000 7205 0000 000a 0000  ...r....r.......
+00000b30: 0073 0e00 0000 0801 0404 0813 0201 0a07  .s..............
+00000b40: 080e 080e 7205 0000 0029 0a72 3100 0000  ....r....).r1...
+00000b50: 7222 0000 00da 0673 6372 6170 7972 0200  r".....scrapyr..
+00000b60: 0000 da24 6179 7567 6573 7069 6465 7274  ...$ayugespidert
+00000b70: 6f6f 6c73 2e63 6f6d 6d6f 6e2e 6d75 6c74  ools.common.mult
+00000b80: 6970 6c65 7869 6e67 7203 0000 00da 1e61  iplexingr......a
+00000b90: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
+00000ba0: 636f 6d6d 6f6e 2e70 6172 616d 7372 0400  common.paramsr..
+00000bb0: 0000 da06 6f62 6a65 6374 7205 0000 0072  ....objectr....r
+00000bc0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+00000bd0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000be0: 0073 0a00 0000 0802 0801 0c02 0c01 0c03  .s..............
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 12 09:55:11 2023 UTC, .py size: 11208 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ff7f 3664 c82b 0000  U.........6d.+..
+00000000: 550d 0d0a 0000 0000 1742 4764 c12b 0000  U........BGd.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6401 6c08 5a09 6400  m.Z...d.d.l.Z.d.
 00000070: 6401 6c0a 5a0a 6400 6404 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
@@ -65,424 +65,424 @@
 00000400: 6c6f 6164 6572 4d69 6464 6c65 7761 7265  loaderMiddleware
 00000410: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
 00000420: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
 00000430: 0000 7340 0000 007c 007c 016a 00a0 0164  ..s@...|.|.j...d
 00000440: 0164 00a1 0264 028d 017d 027c 016a 026a  .d...d...}.|.j.j
 00000450: 037c 026a 0474 026a 0464 038d 0201 007c  .|.j.t.j.d.....|
 00000460: 016a 026a 037c 026a 0574 026a 0564 038d  .j.j.|.j.t.j.d..
-00000470: 0201 007c 0253 0029 044e 5a0c 5757 5852  ...|.S.).NZ.WWXR
-00000480: 6f62 6f74 5f6b 6579 720d 0000 0029 01da  obot_keyr....)..
-00000490: 0673 6967 6e61 6c29 0672 1000 0000 da03  .signal).r......
-000004a0: 6765 7472 0500 0000 da07 636f 6e6e 6563  getr......connec
-000004b0: 74da 0d73 7069 6465 725f 6f70 656e 6564  t..spider_opened
-000004c0: da0d 7370 6964 6572 5f63 6c6f 7365 6429  ..spider_closed)
-000004d0: 03da 0363 6c73 da07 6372 6177 6c65 72da  ...cls..crawler.
-000004e0: 0173 7218 0000 0072 1800 0000 7219 0000  .sr....r....r...
-000004f0: 00da 0c66 726f 6d5f 6372 6177 6c65 7220  ...from_crawler 
-00000500: 0000 0073 0800 0000 0002 1401 1401 1401  ...s............
-00000510: 7a2d 5072 6976 6174 6550 726f 7879 446f  z-PrivateProxyDo
-00000520: 776e 6c6f 6164 6572 4d69 6464 6c65 7761  wnloaderMiddlewa
-00000530: 7265 2e66 726f 6d5f 6372 6177 6c65 7229  re.from_crawler)
-00000540: 01da 1773 746f 705f 6d61 785f 6174 7465  ...stop_max_atte
-00000550: 6d70 745f 6e75 6d62 6572 4e29 01da 0669  mpt_numberN)...i
-00000560: 7364 6963 7463 0300 0000 0000 0000 0000  sdictc..........
-00000570: 0000 0900 0000 0a00 0000 4300 0000 7392  ..........C...s.
-00000580: 0100 0064 017c 006a 0064 0219 009b 0064  ...d.|.j.d.....d
-00000590: 037c 019b 0064 047c 006a 0064 0519 009b  .|...d.|.j.d....
-000005a0: 0064 069d 077d 037c 006a 0172 3274 0264  .d...}.|.j.r2t.d
-000005b0: 0783 0182 017a 1274 03a0 047c 03a1 01a0  .....z.t...|....
-000005c0: 05a1 007d 0457 006e 2c04 0074 066b 0a72  ...}.W.n,..t.k.r
-000005d0: 7001 007d 0501 007a 0e74 0264 0883 017c  p..}...z.t.d...|
-000005e0: 0582 0257 0035 0064 007d 057e 0558 0059  ...W.5.d.}.~.X.Y
-000005f0: 006e 0258 007c 0464 0919 0064 0a6b 0290  .n.X.|.d...d.k..
-00000600: 0172 4e7a 9e7c 04a0 0464 0ba1 01a0 0464  .rNz.|...d.....d
-00000610: 0ca1 017d 067c 04a0 0464 0ba1 01a0 0464  ...}.|...d.....d
-00000620: 0da1 017d 077c 0690 0172 147c 0790 0172  ...}.|...r.|...r
-00000630: 147c 0764 0e6b 0072 cc7c 0764 0f6b 0572  .|.d.k.r.|.d.k.r
-00000640: cc7c 006a 07a0 0864 10a1 0101 006e 327c  .|.j...d.....n2|
-00000650: 0764 0f6b 0072 ea7c 0764 116b 0572 ea7c  .d.k.r.|.d.k.r.|
-00000660: 006a 07a0 0864 12a1 0101 006e 147c 0764  .j...d.....n.|.d
-00000670: 116b 0072 fe7c 006a 07a0 0864 13a1 0101  .k.r.|.j...d....
-00000680: 007c 0290 0172 0c7c 067c 005f 096e 067c  .|...r.|.|._.n.|
-00000690: 0657 0053 006e 0874 0264 0783 0182 0157  .W.S.n.t.d.....W
-000006a0: 006e 2c04 0074 066b 0a90 0172 4a01 0001  .n,..t.k...rJ...
-000006b0: 0001 0064 147c 005f 0174 0aa0 0ba1 0001  ...d.|._.t......
-000006c0: 0074 0264 1583 0182 0159 006e 0258 006e  .t.d.....Y.n.X.n
-000006d0: 407c 04a0 0464 16a1 0104 007d 0890 0172  @|...d.....}...r
-000006e0: 807c 006a 07a0 0864 177c 089b 009d 02a1  .|.j...d.|......
-000006f0: 0101 0074 0264 187c 089b 009d 0283 0182  ...t.d.|........
-00000700: 016e 0e64 147c 005f 0174 0264 0783 0182  .n.d.|._.t.d....
-00000710: 0164 0053 0029 194e 7a29 6874 7470 3a2f  .d.S.).Nz)http:/
-00000720: 2f64 7073 2e6b 646c 6170 692e 636f 6d2f  /dps.kdlapi.com/
-00000730: 6170 692f 6765 7464 7073 3f6f 7264 6572  api/getdps?order
-00000740: 6964 3dda 076f 7264 6572 6964 7a05 266e  id=..orderidz.&n
-00000750: 756d 3d7a 0b26 7369 676e 6174 7572 653d  um=z.&signature=
-00000760: da09 7369 676e 6174 7572 657a 0c26 666f  ..signaturez.&fo
-00000770: 726d 6174 3d6a 736f 6e75 4c00 0000 6970  rmat=jsonuL...ip
-00000780: 20e8 8eb7 e58f 96e6 96b9 e5bc 8fe6 9c89   ...............
-00000790: e8af afef bc8c e8af b7e9 878d e69e 84e7  ................
-000007a0: a781 e5af 86e4 bba3 e790 86e4 b8ad e997  ................
-000007b0: b4e4 bbb6 e88e b7e5 8f96 2069 7020 e79a  .......... ip ..
-000007c0: 84e6 a8a1 e59d 97ef bc81 757a 0000 00e5  ..........uz....
-000007d0: bfab e4bb a3e7 9086 e8af b7e6 b182 e88e  ................
-000007e0: b7e5 8f96 2069 7020 e697 a0e5 938d e5ba  .... ip ........
-000007f0: 94ef bc8c e8af b7e6 a380 e69f a5e6 98af  ................
-00000800: e590 a6e8 83bd e5a4 9fe6 ada3 e5b8 b8e8  ................
-00000810: aebf e997 aee5 bfab e4bb a3e7 9086 e688  ................
-00000820: 96e8 8085 206e 6163 6f73 20e7 9a84 e985  .... nacos .....
-00000830: 8de7 bdae e698 afe5 90a6 e4bb a5e5 8f8a  ................
-00000840: e5a4 b1e6 9588 efbc 81da 0463 6f64 6572  ...........coder
-00000850: 0100 0000 da04 6461 7461 da0a 7072 6f78  ......data..prox
-00000860: 795f 6c69 7374 5a10 746f 6461 795f 6c65  y_listZ.today_le
-00000870: 6674 5f63 6f75 6e74 e964 0000 00e9 3200  ft_count.d....2.
-00000880: 0000 7565 0000 00e7 a781 e5af 86e4 bba3  ..ue............
-00000890: e790 86e4 b889 e7ba a7e8 ada6 e68a a5ef  ................
-000008a0: bc9a e79b b8e5 85b3 e983 a8e9 97a8 e8af  ................
-000008b0: b7e6 b3a8 e684 8fef bc8c 6970 20e6 95b0  ..........ip ...
-000008c0: e987 8fe5 b7b2 e7bb 8fe5 b091 e4ba 8e20  ............... 
-000008d0: 3130 3020 e4b8 aaef bc81 e8af b7e5 8f8a  100 ............
-000008e0: e697 b6e5 8585 e580 bcef bc81 e90a 0000  ................
-000008f0: 0075 7800 0000 e7a7 81e5 af86 e4bb a3e7  .ux.............
-00000900: 9086 e4ba 8ce7 baa7 e8ad a6e6 8aa5 efbc  ................
-00000910: 9ae7 9bb8 e585 b3e9 83a8 e997 a8e8 afb7  ................
-00000920: e6b3 a8e6 848f efbc 8ce7 9bb8 e585 b3e9  ................
-00000930: 83a8 e997 a8e8 afb7 e6b3 a8e6 848f 2c20  .............., 
-00000940: 6970 20e6 95b0 e987 8fe5 b7b2 e7bb 8fe5  ip .............
-00000950: b091 2035 3020 e4b8 aaef bc81 e8af b7e5  .. 50 ..........
-00000960: 8f8a e697 b6e5 8585 e580 bcef bc81 7596  ..............u.
-00000970: 0000 00e7 a781 e5af 86e4 bba3 e790 86e4  ................
-00000980: b880 e7ba a7e8 ada6 e68a a5ef bc9a e79b  ................
-00000990: b8e5 85b3 e983 a8e9 97a8 e8af b7e6 b3a8  ................
-000009a0: e684 8fef bc8c efbc 8ce7 9bb8 e585 b3e9  ................
-000009b0: 83a8 e997 a8e8 afb7 e6b3 a8e6 848f efbc  ................
-000009c0: 8ce7 9bb8 e585 b3e9 83a8 e997 a8e8 afb7  ................
-000009d0: e6b3 a8e6 848f 2c20 6970 20e6 95b0 e987  ......, ip .....
-000009e0: 8fe5 b7b2 e7bb 8fe5 b091 e4ba 8e20 3130  ............. 10
-000009f0: 20e4 b8aa efbc 81e8 afb7 e58f 8ae6 97b6   ...............
-00000a00: e585 85e5 80bc efbc 8154 754a 0000 0069  .........TuJ...i
-00000a10: 7020 e88e b7e5 8f96 e696 b9e5 bc8f e69c  p ..............
-00000a20: 89e8 afaf efbc 8ce8 afb7 e987 8de6 9e84  ................
-00000a30: e7a7 81e5 af86 e4bb a3e7 9086 e4b8 ade9  ................
-00000a40: 97b4 e4bb b6e8 8eb7 e58f 9669 70e7 9a84  ...........ip...
-00000a50: e6a8 a1e5 9d97 efbc 81da 036d 7367 7547  ...........msguG
-00000a60: 0000 00e7 a781 e5af 86e4 bba3 e790 86e7  ................
-00000a70: 89b9 e7ba a7e8 ada6 e68a a5ef bc9a e7a7  ................
-00000a80: 81e5 af86 e4bb a3e7 9086 e587 bae7 8eb0  ................
-00000a90: e994 99e8 afaf efbc 8ce9 9499 e8af afe5  ................
-00000aa0: 8e9f e59b a0e6 98af 3a20 7523 0000 00e8  ........: u#....
-00000ab0: 8eb7 e58f 96e7 a781 e5af 8669 70e5 a4b1  ...........ip...
-00000ac0: e8b4 a5ef bc8c e58e 9fe5 9ba0 e698 afef  ................
-00000ad0: bc9a 290c da0e 7369 6d69 6461 696c 695f  ..)...simidaili_
-00000ae0: 636f 6e66 7213 0000 00da 0a56 616c 7565  confr......Value
-00000af0: 4572 726f 72da 0872 6571 7565 7374 7372  Error..requestsr
-00000b00: 1b00 0000 da04 6a73 6f6e da09 4578 6365  ......json..Exce
-00000b10: 7074 696f 6e72 1400 0000 5a09 7365 6e64  ptionr....Z.send
-00000b20: 5f74 6578 7472 2900 0000 da09 7472 6163  _textr).....trac
-00000b30: 6562 6163 6bda 0970 7269 6e74 5f65 7863  eback..print_exc
-00000b40: 2909 7215 0000 00da 0473 697a 6572 2400  ).r......sizer$.
-00000b50: 0000 da09 7072 6f78 795f 7572 6cda 0172  ....proxy_url..r
-00000b60: da01 655a 0669 706c 6973 745a 096e 6f77  ..eZ.iplistZ.now
-00000b70: 5f69 706e 756d 722d 0000 0072 1800 0000  _ipnumr-...r....
-00000b80: 7218 0000 0072 1900 0000 da0c 6765 745f  r....r......get_
-00000b90: 7072 6f78 795f 6970 2700 0000 7348 0000  proxy_ip'...sH..
-00000ba0: 0000 0322 ff02 0506 0108 0202 0112 0110  ..."............
-00000bb0: 011c 020e 0102 0110 0110 010c 0110 010e  ................
-00000bc0: 0110 0106 0102 ff06 0308 0106 0102 ff04  ................
-00000bd0: 0406 0108 0208 020c 0110 0106 0108 0110  ................
-00000be0: 0210 0112 0110 0206 017a 2d50 7269 7661  .........z-Priva
-00000bf0: 7465 5072 6f78 7944 6f77 6e6c 6f61 6465  teProxyDownloade
-00000c00: 724d 6964 646c 6577 6172 652e 6765 745f  rMiddleware.get_
-00000c10: 7072 6f78 795f 6970 6303 0000 0000 0000  proxy_ipc.......
-00000c20: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
-00000c30: 0073 c400 0000 7400 a001 7c00 6a02 a101  .s....t...|.j...
-00000c40: 7d03 7c00 6a03 7c03 1900 7d04 7c00 6a04  }.|.j.|...}.|.j.
-00000c50: 7c03 0500 1900 6401 3700 0300 3c00 7c00  |.....d.7...<.|.
-00000c60: a005 a100 0100 7c01 6a06 a007 6402 a101  ......|.j...d...
-00000c70: 724e 6402 7c04 9b00 9d02 7c01 6a08 6403  rNd.|.....|.j.d.
-00000c80: 3c00 6e32 7c01 6a06 a007 6404 a101 726c  <.n2|.j...d...rl
-00000c90: 6404 7c04 9b00 9d02 7c01 6a08 6403 3c00  d.|.....|.j.d.<.
-00000ca0: 6e14 7c02 6a09 a00a 6405 7c01 6a06 9b00  n.|.j...d.|.j...
-00000cb0: 9d02 a101 0100 6406 7c01 6a08 6407 3c00  ......d.|.j.d.<.
-00000cc0: 7c00 6a0b 9b00 6408 7c00 6a0c 9b00 9d03  |.j...d.|.j.....
-00000cd0: 7d05 6409 740d a00e 740f 7c05 640a 8302  }.d.t...t.|.d...
-00000ce0: a101 a010 640b a101 1700 7d06 7c06 7c01  ....d.....}.|.|.
-00000cf0: 6a11 640c 3c00 6400 5300 290d 4e67 0000  j.d.<.d.S.).Ng..
-00000d00: 0000 0000 f03f fa08 6874 7470 733a 2f2f  .....?..https://
-00000d10: da05 7072 6f78 79fa 0768 7474 703a 2f2f  ..proxy..http://
-00000d20: fa13 7265 7175 6573 7420 7572 6c20 6572  ..request url er
-00000d30: 726f 723a 2054 5a0a 646f 6e74 5f72 6574  ror: TZ.dont_ret
-00000d40: 7279 fa01 3a7a 0642 6173 6963 20da 0561  ry..:z.Basic ..a
-00000d50: 7363 6969 da04 7574 6638 7a13 5072 6f78  scii..utf8z.Prox
-00000d60: 792d 4175 7468 6f72 697a 6174 696f 6e29  y-Authorization)
-00000d70: 12da 026e 70da 0661 7267 6d69 6eda 0776  ...np..argmin..v
-00000d80: 5f63 6f75 6e74 7229 0000 00da 0c72 6571  _countr).....req
-00000d90: 6e75 6d5f 636f 756e 74da 0576 5f73 756d  num_count..v_sum
-00000da0: da03 7572 6cda 0a73 7461 7274 7377 6974  ..url..startswit
-00000db0: 68da 046d 6574 61da 0473 6c6f 67da 0469  h..meta..slog..i
-00000dc0: 6e66 6fda 0875 7365 726e 616d 65da 0870  nfo..username..p
-00000dd0: 6173 7377 6f72 64da 0662 6173 6536 34da  assword..base64.
-00000de0: 1175 726c 7361 6665 5f62 3634 656e 636f  .urlsafe_b64enco
-00000df0: 6465 da05 6279 7465 73da 0664 6563 6f64  de..bytes..decod
-00000e00: 65da 0768 6561 6465 7273 2907 7215 0000  e..headers).r...
-00000e10: 00da 0772 6571 7565 7374 da06 7370 6964  ...request..spid
-00000e20: 6572 da10 6375 7272 656e 745f 6970 5f69  er..current_ip_i
-00000e30: 6e64 6578 da0a 6375 7272 656e 745f 6970  ndex..current_ip
-00000e40: da0f 7072 6f78 795f 7573 6572 5f70 6173  ..proxy_user_pas
-00000e50: 73da 1165 6e63 6f64 6564 5f75 7365 725f  s..encoded_user_
-00000e60: 7061 7373 7218 0000 0072 1800 0000 7219  passr....r....r.
-00000e70: 0000 00da 0f70 726f 6365 7373 5f72 6571  .....process_req
-00000e80: 7565 7374 5800 0000 7322 0000 0000 020c  uestX...s"......
-00000e90: 010a 0312 0108 030c 0112 010c 0112 0214  ................
-00000ea0: 030a 0212 0106 0108 ff04 0202 fe06 037a  ...............z
-00000eb0: 3050 7269 7661 7465 5072 6f78 7944 6f77  0PrivateProxyDow
-00000ec0: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
-00000ed0: 652e 7072 6f63 6573 735f 7265 7175 6573  e.process_reques
-00000ee0: 7463 0400 0000 0000 0000 0000 0000 0700  tc..............
-00000ef0: 0000 0500 0000 4300 0000 73ac 0000 007c  ......C...s....|
-00000f00: 026a 007c 006a 016b 0772 107c 0253 0074  .j.|.j.k.r.|.S.t
-00000f10: 02a0 037c 006a 04a1 017d 047c 006a 057c  ...|.j...}.|.j.|
-00000f20: 0419 007d 057c 006a 067c 0405 0019 0064  ...}.|.j.|.....d
-00000f30: 0137 0003 003c 007c 00a0 07a1 0001 007c  .7...<.|.......|
-00000f40: 016a 08a0 0964 02a1 0172 5e64 027c 059b  .j...d...r^d.|..
-00000f50: 009d 027c 016a 0a64 033c 006e 327c 016a  ...|.j.d.<.n2|.j
-00000f60: 08a0 0964 04a1 0172 7c64 047c 059b 009d  ...d...r|d.|....
-00000f70: 027c 016a 0a64 033c 006e 147c 036a 0ba0  .|.j.d.<.n.|.j..
-00000f80: 0c64 057c 016a 089b 009d 02a1 0101 0074  .d.|.j.........t
-00000f90: 0d7c 026a 0083 017d 067c 00a0 0e7c 017c  .|.j...}.|...|.|
-00000fa0: 067c 03a1 0370 aa7c 0253 0029 064e e901  .|...p.|.S.).N..
-00000fb0: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
-00000fc0: 0000 723d 0000 0029 0fda 0673 7461 7475  ..r=...)...statu
-00000fd0: 735a 1072 6574 7279 5f68 7474 705f 636f  sZ.retry_http_co
-00000fe0: 6465 7372 4100 0000 7242 0000 0072 4300  desrA...rB...rC.
-00000ff0: 0000 7229 0000 0072 4400 0000 7245 0000  ..r)...rD...rE..
-00001000: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
-00001010: 7249 0000 00da 0565 7272 6f72 7209 0000  rI.....errorr...
-00001020: 00da 065f 7265 7472 7929 0772 1500 0000  ..._retry).r....
-00001030: 7252 0000 00da 0872 6573 706f 6e73 6572  rR.....responser
-00001040: 5300 0000 7254 0000 0072 5500 0000 da06  S...rT...rU.....
-00001050: 7265 6173 6f6e 7218 0000 0072 1800 0000  reasonr....r....
-00001060: 7219 0000 00da 1070 726f 6365 7373 5f72  r......process_r
-00001070: 6573 706f 6e73 6572 0000 0073 1a00 0000  esponser...s....
-00001080: 0001 0c01 0402 0c01 0a03 1201 0802 0c01  ................
-00001090: 1201 0c01 1202 1402 0a01 7a31 5072 6976  ..........z1Priv
-000010a0: 6174 6550 726f 7879 446f 776e 6c6f 6164  ateProxyDownload
-000010b0: 6572 4d69 6464 6c65 7761 7265 2e70 726f  erMiddleware.pro
-000010c0: 6365 7373 5f72 6573 706f 6e73 6563 0400  cess_responsec..
-000010d0: 0000 0000 0000 0000 0000 0900 0000 0500  ................
-000010e0: 0000 4300 0000 736e 0200 0074 007c 027c  ..C...sn...t.|.|
-000010f0: 006a 0183 0290 0272 6a7c 016a 0264 0119  .j.....rj|.j.d..
-00001100: 00a0 0364 0264 021a 00a1 0164 0319 007d  ...d.d.....d...}
-00001110: 0464 04a0 047c 006a 0564 0519 007c 006a  .d...|.j.d...|.j
-00001120: 0564 0619 007c 04a1 037d 0574 06a0 077c  .d...|...}.t...|
-00001130: 05a1 01a0 08a1 007d 067c 0664 0719 007c  .......}.|.d...|
-00001140: 0419 0090 0273 087c 047c 006a 096b 0690  .....s.|.|.j.k..
-00001150: 0172 d87c 036a 0aa0 0b64 08a1 0101 007c  .r.|.j...d.....|
-00001160: 006a 09a0 0c7c 04a1 017d 077c 006a 09a0  .j...|...}.|.j..
-00001170: 0d7c 07a1 0101 0074 0e6a 0f7c 006a 107c  .|.....t.j.|.j.|
-00001180: 0764 0964 0a8d 037c 005f 1074 0e6a 0f7c  .d.d...|._.t.j.|
-00001190: 006a 117c 0764 0964 0a8d 037c 005f 1174  .j.|.d.d...|._.t
-000011a0: 0ea0 127c 006a 13a1 0164 0b6b 0590 0172  ...|.j...d.k...r
-000011b0: 2a74 147c 006a 0983 0164 0c6b 0090 0172  *t.|.j...d.k...r
-000011c0: 2a7c 00a0 1564 0da1 0144 005d 467d 087c  *|...d...D.]F}.|
-000011d0: 006a 09a0 167c 08a1 0101 0074 0ea0 167c  .j...|.....t...|
-000011e0: 006a 1064 0ea1 027c 005f 1074 0ea0 167c  .j.d...|._.t...|
-000011f0: 006a 1164 09a1 027c 005f 117c 087d 047c  .j.d...|._.|.}.|
-00001200: 006a 1164 0305 0019 0064 0f37 0003 003c  .j.d.....d.7...<
-00001210: 0071 e06e 8c74 147c 006a 0983 017c 006a  .q.n.t.|.j...|.j
-00001220: 176b 0090 0172 8e7c 00a0 1564 0fa1 0164  .k...r.|...d...d
-00001230: 0919 007d 087c 006a 09a0 167c 08a1 0101  ...}.|.j...|....
-00001240: 0074 0ea0 167c 006a 1064 0ea1 027c 005f  .t...|.j.d...|._
-00001250: 1074 0ea0 167c 006a 1164 09a1 027c 005f  .t...|.j.d...|._
-00001260: 117c 087d 047c 006a 1164 0305 0019 0064  .|.}.|.j.d.....d
-00001270: 0f37 0003 003c 006e 2874 0ea0 187c 006a  .7...<.n(t...|.j
-00001280: 13a1 017d 077c 006a 097c 0719 007d 047c  ...}.|.j.|...}.|
-00001290: 006a 117c 0705 0019 0064 0f37 0003 003c  .j.|.....d.7...<
-000012a0: 007c 036a 0aa0 0b64 1074 147c 006a 0983  .|.j...d.t.|.j..
-000012b0: 019b 009d 02a1 0101 007c 00a0 19a1 0001  .........|......
-000012c0: 006e 3074 0ea0 187c 006a 13a1 017d 077c  .n0t...|.j...}.|
-000012d0: 006a 097c 0719 007d 047c 006a 117c 0705  .j.|...}.|.j.|..
-000012e0: 0019 0064 0f37 0003 003c 007c 00a0 19a1  ...d.7...<.|....
-000012f0: 0001 007c 016a 1aa0 1b64 11a1 0190 0272  ...|.j...d.....r
-00001300: 2864 12a0 047c 04a1 017c 016a 0264 013c  (d...|...|.j.d.<
-00001310: 006e 347c 016a 1aa0 1b64 13a1 0190 0272  .n4|.j...d.....r
-00001320: 4864 14a0 047c 04a1 017c 016a 0264 013c  Hd...|...|.j.d.<
-00001330: 006e 147c 036a 0aa0 0b64 157c 016a 1a9b  .n.|.j...d.|.j..
-00001340: 009d 02a1 0101 007c 00a0 1c7c 017c 027c  .......|...|.|.|
-00001350: 03a1 0353 0064 0053 0029 164e 723b 0000  ...S.d.S.).Nr;..
-00001360: 00da 00e9 ffff ffff 7a49 6874 7470 733a  ........zIhttps:
-00001370: 2f2f 6470 732e 6b64 6c61 7069 2e63 6f6d  //dps.kdlapi.com
-00001380: 2f61 7069 2f63 6865 636b 6470 7376 616c  /api/checkdpsval
-00001390: 6964 3f6f 7264 6572 6964 3d7b 7d26 7369  id?orderid={}&si
-000013a0: 676e 6174 7572 653d 7b7d 2670 726f 7879  gnature={}&proxy
-000013b0: 3d7b 7d72 2500 0000 7226 0000 0072 2800  ={}r%...r&...r(.
-000013c0: 0000 7508 0000 00e6 9bb4 e696 b069 7072  ..u..........ipr
-000013d0: 0100 0000 2901 da04 6178 6973 6700 0000  ....)...axisg...
-000013e0: 0000 0012 40e9 0700 0000 e902 0000 00e7  ....@...........
-000013f0: 0000 0000 0000 e03f 7259 0000 0075 2300  .......?rY...u#.
-00001400: 0000 e79b aee5 898d 2069 7020 e6b1 a0e5  ........ ip ....
-00001410: ad98 e987 8f20 6970 20e6 95b0 e987 8fe4  ..... ip .......
-00001420: b8ba efbc 9a72 3a00 0000 7a0a 6874 7470  .....r:...z.http
-00001430: 733a 2f2f 7b7d 723c 0000 007a 0968 7474  s://{}r<...z.htt
-00001440: 703a 2f2f 7b7d 723d 0000 0029 1dda 0a69  p://{}r=...)...i
-00001450: 7369 6e73 7461 6e63 655a 1345 5843 4550  sinstanceZ.EXCEP
-00001460: 5449 4f4e 535f 544f 5f52 4554 5259 7248  TIONS_TO_RETRYrH
-00001470: 0000 00da 0573 706c 6974 da06 666f 726d  .....split..form
-00001480: 6174 722e 0000 0072 3000 0000 721b 0000  atr....r0...r...
-00001490: 0072 3100 0000 7229 0000 0072 4900 0000  .r1...r)...rI...
-000014a0: 724a 0000 00da 0569 6e64 6578 da03 706f  rJ.....index..po
-000014b0: 7072 4100 0000 da06 6465 6c65 7465 da0a  prA.....delete..
-000014c0: 7469 6d65 5f63 6f75 6e74 7244 0000 00da  time_countrD....
-000014d0: 0761 7665 7261 6765 7243 0000 00da 036c  .averagerC.....l
-000014e0: 656e 7239 0000 00da 0661 7070 656e 64da  enr9.....append.
-000014f0: 0e70 726f 7879 706f 6f6c 5f73 697a 6572  .proxypool_sizer
-00001500: 4200 0000 7245 0000 0072 4600 0000 7247  B...rE...rF...rG
-00001510: 0000 0072 5c00 0000 2909 7215 0000 0072  ...r\...).r....r
-00001520: 5200 0000 da09 6578 6365 7074 696f 6e72  R.....exceptionr
-00001530: 5300 0000 7255 0000 0072 4600 0000 da09  S...rU...rF.....
-00001540: 6973 5f65 7869 7374 7372 5400 0000 5a06  is_existsrT...Z.
-00001550: 6e65 775f 6970 7218 0000 0072 1800 0000  new_ipr....r....
-00001560: 7219 0000 00da 1170 726f 6365 7373 5f65  r......process_e
-00001570: 7863 6570 7469 6f6e 8700 0000 7368 0000  xception....sh..
-00001580: 0000 010e 0118 0104 0108 0108 0102 fd04  ................
-00001590: 050e 010e 010c 010c 020c 010c 0104 0104  ................
-000015a0: 0002 0002 ff08 0304 0104 0002 0002 ff08  ................
-000015b0: 0522 010e 010c 0110 0110 0104 0116 0112  ."..............
-000015c0: 010e 010c 0110 0110 0104 0114 020c 010a  ................
-000015d0: 0112 0218 010a 020c 010a 0112 0108 020e  ................
-000015e0: 0112 010e 0112 0214 027a 3250 7269 7661  .........z2Priva
-000015f0: 7465 5072 6f78 7944 6f77 6e6c 6f61 6465  teProxyDownloade
-00001600: 724d 6964 646c 6577 6172 652e 7072 6f63  rMiddleware.proc
-00001610: 6573 735f 6578 6365 7074 696f 6e63 0100  ess_exceptionc..
-00001620: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001630: 0000 4300 0000 7312 0000 007c 006a 007c  ..C...s....|.j.|
-00001640: 006a 011b 007c 005f 0264 0053 0029 014e  .j...|._.d.S.).N
-00001650: 2903 7244 0000 0072 6c00 0000 7243 0000  ).rD...rl...rC..
-00001660: 0029 0172 1500 0000 7218 0000 0072 1800  .).r....r....r..
-00001670: 0000 7219 0000 0072 4500 0000 c200 0000  ..r....rE.......
-00001680: 7302 0000 0000 017a 2650 7269 7661 7465  s......z&Private
-00001690: 5072 6f78 7944 6f77 6e6c 6f61 6465 724d  ProxyDownloaderM
-000016a0: 6964 646c 6577 6172 652e 765f 7375 6d63  iddleware.v_sumc
-000016b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000016c0: 0400 0000 4300 0000 7326 0000 007c 006a  ....C...s&...|.j
-000016d0: 0073 2274 01a0 0264 01a1 0101 0074 03a0  .s"t...d.....t..
-000016e0: 047c 006a 0564 01a1 027c 005f 0571 0064  .|.j.d...|._.q.d
-000016f0: 0053 0029 024e 679a 9999 9999 99c9 3f29  .S.).Ng.......?)
-00001700: 06da 0865 6e64 5f74 696d 65da 0474 696d  ...end_time..tim
-00001710: 65da 0573 6c65 6570 7241 0000 00da 0361  e..sleeprA.....a
-00001720: 6464 726c 0000 00a9 0272 1500 0000 7253  ddrl.....r....rS
-00001730: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00001740: 0000 da05 636c 6f63 6bc5 0000 0073 0600  ....clock....s..
-00001750: 0000 0001 0601 0a01 7a26 5072 6976 6174  ........z&Privat
-00001760: 6550 726f 7879 446f 776e 6c6f 6164 6572  eProxyDownloader
-00001770: 4d69 6464 6c65 7761 7265 2e63 6c6f 636b  Middleware.clock
-00001780: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00001790: 0005 0000 0043 0000 0073 1401 0000 7400  .....C...s....t.
-000017a0: 8300 7d02 7401 a002 6401 6401 6402 9c02  ..}.t...d.d.d...
-000017b0: a101 7d03 7401 a003 7c03 a101 7c00 5f04  ..}.t...|...|._.
-000017c0: 7c00 6a04 6403 1900 7c00 5f05 7c00 6a04  |.j.d...|._.|.j.
-000017d0: 6404 1900 7c00 5f06 7c02 a007 6405 a101  d...|._.|...d...
-000017e0: 7280 7c02 a007 6405 a101 6406 6b00 725c  r.|...d...d.k.r\
-000017f0: 7408 6407 8301 8201 6e16 7c02 a007 6405  t.d.....n.|...d.
-00001800: a101 6408 6b04 7272 7408 6409 8301 8201  ..d.k.rrt.d.....
-00001810: 7c02 a007 6405 a101 7c00 5f09 6e06 6406  |...d...|._.n.d.
-00001820: 7c00 5f09 640a 7c00 5f0a 740b a00c 7c00  |._.d.|._.t...|.
-00001830: 6a09 6601 a101 640b 1700 7c00 5f0d 740b  j.f...d...|._.t.
-00001840: a00c 7c00 6a09 6601 a101 7c00 5f0e 7c00  ..|.j.f...|._.|.
-00001850: a00f a100 0100 7410 7c00 6a11 7c01 6601  ......t.|.j.|.f.
-00001860: 640c 640d 8d03 7c00 5f12 7c00 6a12 a013  d.d...|._.|.j...
-00001870: a100 0100 7c00 a014 7c00 6a09 640c a102  ....|...|.j.d...
-00001880: 0100 7c01 6a15 a016 640e 7417 7c00 6a18  ..|.j...d.t.|.j.
-00001890: 8301 9b00 9d02 a101 0100 7c01 6a15 a016  ..........|.j...
-000018a0: 640f 7c01 6a19 9b00 9d02 a101 0100 6400  d.|.j.........d.
-000018b0: 5300 2910 4e7a 032a 2a2a 2902 724b 0000  S.).Nz.***).rK..
-000018c0: 0072 4c00 0000 724b 0000 0072 4c00 0000  .rL...rK...rL...
-000018d0: 5a08 534d 5050 5349 5a45 7259 0000 0075  Z.SMPPSIZErY...u
-000018e0: 6d00 0000 e682 a8e8 be93 e585 a5e7 9a84  m...............
-000018f0: 2069 7020 e6b1 a0e5 ad90 e5a4 a7e5 b08f   ip ............
-00001900: e4b8 8de8 83bd e5b0 8fe4 ba8e 2031 efbc  ............ 1..
-00001910: 81e8 afb7 e987 8de6 96b0 e4bf aee6 94b9  ................
-00001920: 2073 6574 7469 6e67 7320 e4b8 ade7 9a84   settings ......
-00001930: 2053 4d50 5053 495a 4520 e79a 84e5 80bc   SMPPSIZE ......
-00001940: e4b8 bae5 a4a7 e4ba 8ee7 ad89 e4ba 8e20  ............... 
-00001950: 3172 6300 0000 754b 0000 00e4 bda0 e7a4  1rc...uK........
-00001960: bce8 b28c e590 97ef bc8c 6970 20e6 b1a0  ..........ip ...
-00001970: e69c 80e5 a4a7 e695 b0e9 878f e4b8 8de5  ................
-00001980: 8faf e4bb a5e8 b685 e8bf 8720 3720 e4b8  ........... 7 ..
-00001990: aaef bc81 e8af b7e9 878d e696 b0e8 aebe  ................
-000019a0: e7bd aeef bc81 4672 6500 0000 5429 03da  ......Fre...T)..
-000019b0: 0674 6172 6765 74da 0461 7267 73da 0664  .target..args..d
-000019c0: 6165 6d6f 6e75 2500 0000 e588 9de5 a78b  aemonu%.........
-000019d0: e58c 9620 6970 20e5 ad97 e585 b8ef bc8c  ... ip .........
-000019e0: 6970 20e6 95b0 e987 8fe4 b8ba efbc 9a7a  ip ............z
-000019f0: 2950 7269 7661 7465 5072 6f78 7944 6f77  )PrivateProxyDow
-00001a00: 6e6c 6f61 6465 724d 6964 646c 6577 6172  nloaderMiddlewar
-00001a10: 6520 6f70 656e 6564 3a20 291a 7208 0000  e opened: ).r...
-00001a20: 0072 3100 0000 da05 6475 6d70 73da 056c  .r1.....dumps..l
-00001a30: 6f61 6473 722e 0000 0072 4b00 0000 724c  oadsr....rK...rL
-00001a40: 0000 0072 1b00 0000 722f 0000 0072 7000  ...r....r/...rp.
-00001a50: 0000 7274 0000 0072 4100 0000 da05 7a65  ..rt...rA.....ze
-00001a60: 726f 7372 6c00 0000 7244 0000 0072 4500  rosrl...rD...rE.
-00001a70: 0000 7202 0000 0072 7900 0000 da01 74da  ..r....ry.....t.
-00001a80: 0573 7461 7274 7239 0000 0072 4900 0000  .startr9...rI...
-00001a90: 724a 0000 0072 6e00 0000 7229 0000 00da  rJ...rn...r)....
-00001aa0: 046e 616d 6529 0472 1500 0000 7253 0000  .name).r....rS..
-00001ab0: 0072 1000 0000 da04 7265 7378 7218 0000  .r......resxr...
-00001ac0: 0072 1800 0000 7219 0000 0072 1d00 0000  .r....r....r....
-00001ad0: ca00 0000 732e 0000 0000 0106 0210 010c  ....s...........
-00001ae0: 010c 010c 020a 010e 0102 0102 ff06 030e  ................
-00001af0: 0108 020e 0206 0106 0114 0110 0108 0114  ................
-00001b00: 010a 010e 0118 017a 2e50 7269 7661 7465  .......z.Private
-00001b10: 5072 6f78 7944 6f77 6e6c 6f61 6465 724d  ProxyDownloaderM
-00001b20: 6964 646c 6577 6172 652e 7370 6964 6572  iddleware.spider
-00001b30: 5f6f 7065 6e65 6463 0200 0000 0000 0000  _openedc........
-00001b40: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001b50: 7328 0000 0064 017c 005f 007c 006a 01a0  s(...d.|._.|.j..
-00001b60: 02a1 0001 007c 016a 03a0 0464 027c 016a  .....|.j...d.|.j
-00001b70: 059b 009d 02a1 0101 0064 0053 0029 034e  .........d.S.).N
-00001b80: 547a 2950 7269 7661 7465 5072 6f78 7944  Tz)PrivateProxyD
-00001b90: 6f77 6e6c 6f61 6465 724d 6964 646c 6577  ownloaderMiddlew
-00001ba0: 6172 6520 636c 6f73 6564 3a20 2906 7274  are closed: ).rt
-00001bb0: 0000 0072 8000 0000 da04 6a6f 696e 7249  ...r......joinrI
-00001bc0: 0000 0072 4a00 0000 7282 0000 0072 7800  ...rJ...r....rx.
-00001bd0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001be0: 0072 1e00 0000 e700 0000 7306 0000 0000  .r........s.....
-00001bf0: 0106 010a 017a 2e50 7269 7661 7465 5072  .....z.PrivatePr
-00001c00: 6f78 7944 6f77 6e6c 6f61 6465 724d 6964  oxyDownloaderMid
-00001c10: 646c 6577 6172 652e 7370 6964 6572 5f63  dleware.spider_c
-00001c20: 6c6f 7365 6429 014e 2916 da08 5f5f 6e61  losed).N)...__na
-00001c30: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001c40: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00001c50: 5f5f 646f 635f 5fda 0373 7472 7212 0000  __doc__..strr...
-00001c60: 00da 0b63 6c61 7373 6d65 7468 6f64 7222  ...classmethodr"
-00001c70: 0000 0072 0400 0000 720b 0000 00da 0972  ...r....r......r
-00001c80: 6574 7279 5f6e 756d 7203 0000 00da 0462  etry_numr......b
-00001c90: 6f6f 6c72 3900 0000 7258 0000 0072 5f00  oolr9...rX...r_.
-00001ca0: 0000 7273 0000 0072 4500 0000 7279 0000  ..rs...rE...ry..
-00001cb0: 0072 1d00 0000 721e 0000 00da 0d5f 5f63  .r....r......__c
-00001cc0: 6c61 7373 6365 6c6c 5f5f 7218 0000 0072  lasscell__r....r
-00001cd0: 1800 0000 7216 0000 0072 1900 0000 720c  ....r....r....r.
-00001ce0: 0000 0015 0000 0073 1a00 0000 0801 0404  .......s........
-00001cf0: 1206 0201 0a06 0a01 1630 081a 0815 083b  .........0.....;
-00001d00: 0803 0805 081d 720c 0000 0029 1c72 4d00  ......r....).rM.
-00001d10: 0000 7231 0000 0072 7500 0000 7233 0000  ..r1...ru...r3..
-00001d20: 00da 0974 6872 6561 6469 6e67 7202 0000  ...threadingr...
-00001d30: 00da 0674 7970 696e 6772 0300 0000 da05  ...typingr......
-00001d40: 6e75 6d70 7972 4100 0000 7230 0000 00da  numpyrA...r0....
-00001d50: 0872 6574 7279 696e 6772 0400 0000 da06  .retryingr......
-00001d60: 7363 7261 7079 7205 0000 005a 2273 6372  scrapyr....Z"scr
-00001d70: 6170 792e 646f 776e 6c6f 6164 6572 6d69  apy.downloadermi
-00001d80: 6464 6c65 7761 7265 732e 7265 7472 7972  ddlewares.retryr
-00001d90: 0600 0000 da0f 7363 7261 7079 2e73 6574  ......scrapy.set
-00001da0: 7469 6e67 7372 0700 0000 5a14 7363 7261  tingsr....Z.scra
-00001db0: 7079 2e75 7469 6c73 2e70 726f 6a65 6374  py.utils.project
-00001dc0: 7208 0000 00da 1573 6372 6170 792e 7574  r......scrapy.ut
-00001dd0: 696c 732e 7265 7370 6f6e 7365 7209 0000  ils.responser...
-00001de0: 005a 2157 6f72 6b57 6569 7869 6e52 6f62  .Z!WorkWeixinRob
-00001df0: 6f74 2e77 6f72 6b5f 7765 6978 696e 5f72  ot.work_weixin_r
-00001e00: 6f62 6f74 720a 0000 00da 1e61 7975 6765  obotr......ayuge
-00001e10: 7370 6964 6572 746f 6f6c 732e 636f 6d6d  spidertools.comm
-00001e20: 6f6e 2e50 6172 616d 7372 0b00 0000 720c  on.Paramsr....r.
-00001e30: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00001e40: 0000 7219 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001e50: 3e01 0000 0073 2000 0000 0801 0801 0801  >....s .........
-00001e60: 0801 0c01 0c02 0801 0801 0c01 0c01 0c01  ................
-00001e70: 0c01 0c01 0c01 0c02 0c03                 ..........
+00000470: 0201 007c 0253 0029 044e 5a05 7778 626f  ...|.S.).NZ.wxbo
+00000480: 7472 0d00 0000 2901 da06 7369 676e 616c  tr....)...signal
+00000490: 2906 7210 0000 00da 0367 6574 7205 0000  ).r......getr...
+000004a0: 00da 0763 6f6e 6e65 6374 da0d 7370 6964  ...connect..spid
+000004b0: 6572 5f6f 7065 6e65 64da 0d73 7069 6465  er_opened..spide
+000004c0: 725f 636c 6f73 6564 2903 da03 636c 73da  r_closed)...cls.
+000004d0: 0763 7261 776c 6572 da01 7372 1800 0000  .crawler..sr....
+000004e0: 7218 0000 0072 1900 0000 da0c 6672 6f6d  r....r......from
+000004f0: 5f63 7261 776c 6572 2000 0000 7308 0000  _crawler ...s...
+00000500: 0000 0214 0114 0114 017a 2d50 7269 7661  .........z-Priva
+00000510: 7465 5072 6f78 7944 6f77 6e6c 6f61 6465  teProxyDownloade
+00000520: 724d 6964 646c 6577 6172 652e 6672 6f6d  rMiddleware.from
+00000530: 5f63 7261 776c 6572 2901 5a17 7374 6f70  _crawler).Z.stop
+00000540: 5f6d 6178 5f61 7474 656d 7074 5f6e 756d  _max_attempt_num
+00000550: 6265 724e 2901 da06 6973 6469 6374 6303  berN)...isdictc.
+00000560: 0000 0000 0000 0000 0000 0009 0000 000a  ................
+00000570: 0000 0043 0000 0073 9201 0000 6401 7c00  ...C...s....d.|.
+00000580: 6a00 6402 1900 9b00 6403 7c01 9b00 6404  j.d.....d.|...d.
+00000590: 7c00 6a00 6405 1900 9b00 6406 9d07 7d03  |.j.d.....d...}.
+000005a0: 7c00 6a01 7232 7402 6407 8301 8201 7a12  |.j.r2t.d.....z.
+000005b0: 7403 a004 7c03 a101 a005 a100 7d04 5700  t...|.......}.W.
+000005c0: 6e2c 0400 7406 6b0a 7270 0100 7d05 0100  n,..t.k.rp..}...
+000005d0: 7a0e 7402 6408 8301 7c05 8202 5700 3500  z.t.d...|...W.5.
+000005e0: 6400 7d05 7e05 5800 5900 6e02 5800 7c04  d.}.~.X.Y.n.X.|.
+000005f0: 6409 1900 640a 6b02 9001 724e 7a9e 7c04  d...d.k...rNz.|.
+00000600: a004 640b a101 a004 640c a101 7d06 7c04  ..d.....d...}.|.
+00000610: a004 640b a101 a004 640d a101 7d07 7c06  ..d.....d...}.|.
+00000620: 9001 7214 7c07 9001 7214 7c07 640e 6b00  ..r.|...r.|.d.k.
+00000630: 72cc 7c07 640f 6b05 72cc 7c00 6a07 a008  r.|.d.k.r.|.j...
+00000640: 6410 a101 0100 6e32 7c07 640f 6b00 72ea  d.....n2|.d.k.r.
+00000650: 7c07 6411 6b05 72ea 7c00 6a07 a008 6412  |.d.k.r.|.j...d.
+00000660: a101 0100 6e14 7c07 6411 6b00 72fe 7c00  ....n.|.d.k.r.|.
+00000670: 6a07 a008 6413 a101 0100 7c02 9001 720c  j...d.....|...r.
+00000680: 7c06 7c00 5f09 6e06 7c06 5700 5300 6e08  |.|._.n.|.W.S.n.
+00000690: 7402 6407 8301 8201 5700 6e2c 0400 7406  t.d.....W.n,..t.
+000006a0: 6b0a 9001 724a 0100 0100 0100 6414 7c00  k...rJ......d.|.
+000006b0: 5f01 740a a00b a100 0100 7402 6415 8301  _.t.......t.d...
+000006c0: 8201 5900 6e02 5800 6e40 7c04 a004 6416  ..Y.n.X.n@|...d.
+000006d0: a101 0400 7d08 9001 7280 7c00 6a07 a008  ....}...r.|.j...
+000006e0: 6417 7c08 9b00 9d02 a101 0100 7402 6418  d.|.........t.d.
+000006f0: 7c08 9b00 9d02 8301 8201 6e0e 6414 7c00  |.........n.d.|.
+00000700: 5f01 7402 6407 8301 8201 6400 5300 2919  _.t.d.....d.S.).
+00000710: 4e7a 2968 7474 703a 2f2f 6470 732e 6b64  Nz)http://dps.kd
+00000720: 6c61 7069 2e63 6f6d 2f61 7069 2f67 6574  lapi.com/api/get
+00000730: 6470 733f 6f72 6465 7269 643d da07 6f72  dps?orderid=..or
+00000740: 6465 7269 647a 0526 6e75 6d3d 7a0b 2673  deridz.&num=z.&s
+00000750: 6967 6e61 7475 7265 3dda 0973 6967 6e61  ignature=..signa
+00000760: 7475 7265 7a0c 2666 6f72 6d61 743d 6a73  turez.&format=js
+00000770: 6f6e 754c 0000 0069 7020 e88e b7e5 8f96  onuL...ip ......
+00000780: e696 b9e5 bc8f e69c 89e8 afaf efbc 8ce8  ................
+00000790: afb7 e987 8de6 9e84 e7a7 81e5 af86 e4bb  ................
+000007a0: a3e7 9086 e4b8 ade9 97b4 e4bb b6e8 8eb7  ................
+000007b0: e58f 9620 6970 20e7 9a84 e6a8 a1e5 9d97  ... ip .........
+000007c0: efbc 8175 7a00 0000 e5bf abe4 bba3 e790  ...uz...........
+000007d0: 86e8 afb7 e6b1 82e8 8eb7 e58f 9620 6970  ............. ip
+000007e0: 20e6 97a0 e593 8de5 ba94 efbc 8ce8 afb7   ...............
+000007f0: e6a3 80e6 9fa5 e698 afe5 90a6 e883 bde5  ................
+00000800: a49f e6ad a3e5 b8b8 e8ae bfe9 97ae e5bf  ................
+00000810: abe4 bba3 e790 86e6 8896 e880 8520 6e61  ............. na
+00000820: 636f 7320 e79a 84e9 858d e7bd aee6 98af  cos ............
+00000830: e590 a6e4 bba5 e58f 8ae5 a4b1 e695 88ef  ................
+00000840: bc81 da04 636f 6465 7201 0000 00da 0464  ....coder......d
+00000850: 6174 61da 0a70 726f 7879 5f6c 6973 745a  ata..proxy_listZ
+00000860: 1074 6f64 6179 5f6c 6566 745f 636f 756e  .today_left_coun
+00000870: 74e9 6400 0000 e932 0000 0075 6500 0000  t.d....2...ue...
+00000880: e7a7 81e5 af86 e4bb a3e7 9086 e4b8 89e7  ................
+00000890: baa7 e8ad a6e6 8aa5 efbc 9ae7 9bb8 e585  ................
+000008a0: b3e9 83a8 e997 a8e8 afb7 e6b3 a8e6 848f  ................
+000008b0: efbc 8c69 7020 e695 b0e9 878f e5b7 b2e7  ...ip ..........
+000008c0: bb8f e5b0 91e4 ba8e 2031 3030 20e4 b8aa  ........ 100 ...
+000008d0: efbc 81e8 afb7 e58f 8ae6 97b6 e585 85e5  ................
+000008e0: 80bc efbc 81e9 0a00 0000 7578 0000 00e7  ..........ux....
+000008f0: a781 e5af 86e4 bba3 e790 86e4 ba8c e7ba  ................
+00000900: a7e8 ada6 e68a a5ef bc9a e79b b8e5 85b3  ................
+00000910: e983 a8e9 97a8 e8af b7e6 b3a8 e684 8fef  ................
+00000920: bc8c e79b b8e5 85b3 e983 a8e9 97a8 e8af  ................
+00000930: b7e6 b3a8 e684 8f2c 2069 7020 e695 b0e9  ......., ip ....
+00000940: 878f e5b7 b2e7 bb8f e5b0 9120 3530 20e4  ........... 50 .
+00000950: b8aa efbc 81e8 afb7 e58f 8ae6 97b6 e585  ................
+00000960: 85e5 80bc efbc 8175 9600 0000 e7a7 81e5  .......u........
+00000970: af86 e4bb a3e7 9086 e4b8 80e7 baa7 e8ad  ................
+00000980: a6e6 8aa5 efbc 9ae7 9bb8 e585 b3e9 83a8  ................
+00000990: e997 a8e8 afb7 e6b3 a8e6 848f efbc 8cef  ................
+000009a0: bc8c e79b b8e5 85b3 e983 a8e9 97a8 e8af  ................
+000009b0: b7e6 b3a8 e684 8fef bc8c e79b b8e5 85b3  ................
+000009c0: e983 a8e9 97a8 e8af b7e6 b3a8 e684 8f2c  ...............,
+000009d0: 2069 7020 e695 b0e9 878f e5b7 b2e7 bb8f   ip ............
+000009e0: e5b0 91e4 ba8e 2031 3020 e4b8 aaef bc81  ...... 10 ......
+000009f0: e8af b7e5 8f8a e697 b6e5 8585 e580 bcef  ................
+00000a00: bc81 5475 4a00 0000 6970 20e8 8eb7 e58f  ..TuJ...ip .....
+00000a10: 96e6 96b9 e5bc 8fe6 9c89 e8af afef bc8c  ................
+00000a20: e8af b7e9 878d e69e 84e7 a781 e5af 86e4  ................
+00000a30: bba3 e790 86e4 b8ad e997 b4e4 bbb6 e88e  ................
+00000a40: b7e5 8f96 6970 e79a 84e6 a8a1 e59d 97ef  ....ip..........
+00000a50: bc81 da03 6d73 6775 4700 0000 e7a7 81e5  ....msguG.......
+00000a60: af86 e4bb a3e7 9086 e789 b9e7 baa7 e8ad  ................
+00000a70: a6e6 8aa5 efbc 9ae7 a781 e5af 86e4 bba3  ................
+00000a80: e790 86e5 87ba e78e b0e9 9499 e8af afef  ................
+00000a90: bc8c e994 99e8 afaf e58e 9fe5 9ba0 e698  ................
+00000aa0: af3a 2075 2300 0000 e88e b7e5 8f96 e7a7  .: u#...........
+00000ab0: 81e5 af86 6970 e5a4 b1e8 b4a5 efbc 8ce5  ....ip..........
+00000ac0: 8e9f e59b a0e6 98af efbc 9a29 0cda 0e73  ...........)...s
+00000ad0: 696d 6964 6169 6c69 5f63 6f6e 6672 1300  imidaili_confr..
+00000ae0: 0000 da0a 5661 6c75 6545 7272 6f72 da08  ....ValueError..
+00000af0: 7265 7175 6573 7473 721b 0000 00da 046a  requestsr......j
+00000b00: 736f 6eda 0945 7863 6570 7469 6f6e 7214  son..Exceptionr.
+00000b10: 0000 005a 0973 656e 645f 7465 7874 7228  ...Z.send_textr(
+00000b20: 0000 00da 0974 7261 6365 6261 636b da09  .....traceback..
+00000b30: 7072 696e 745f 6578 6329 0972 1500 0000  print_exc).r....
+00000b40: da04 7369 7a65 7223 0000 00da 0970 726f  ..sizer#.....pro
+00000b50: 7879 5f75 726c da01 72da 0165 5a06 6970  xy_url..r..eZ.ip
+00000b60: 6c69 7374 5a09 6e6f 775f 6970 6e75 6d72  listZ.now_ipnumr
+00000b70: 2c00 0000 7218 0000 0072 1800 0000 7219  ,...r....r....r.
+00000b80: 0000 00da 0c67 6574 5f70 726f 7879 5f69  .....get_proxy_i
+00000b90: 7027 0000 0073 4800 0000 0003 22ff 0205  p'...sH....."...
+00000ba0: 0601 0802 0201 1201 1001 1c02 0e01 0201  ................
+00000bb0: 1001 1001 0c01 1001 0e01 1001 0601 02ff  ................
+00000bc0: 0603 0801 0601 02ff 0404 0601 0802 0802  ................
+00000bd0: 0c01 1001 0601 0801 1002 1001 1201 1002  ................
+00000be0: 0601 7a2d 5072 6976 6174 6550 726f 7879  ..z-PrivateProxy
+00000bf0: 446f 776e 6c6f 6164 6572 4d69 6464 6c65  DownloaderMiddle
+00000c00: 7761 7265 2e67 6574 5f70 726f 7879 5f69  ware.get_proxy_i
+00000c10: 7063 0300 0000 0000 0000 0000 0000 0700  pc..............
+00000c20: 0000 0600 0000 4300 0000 73c4 0000 0074  ......C...s....t
+00000c30: 00a0 017c 006a 02a1 017d 037c 006a 037c  ...|.j...}.|.j.|
+00000c40: 0319 007d 047c 006a 047c 0305 0019 0064  ...}.|.j.|.....d
+00000c50: 0137 0003 003c 007c 00a0 05a1 0001 007c  .7...<.|.......|
+00000c60: 016a 06a0 0764 02a1 0172 4e64 027c 049b  .j...d...rNd.|..
+00000c70: 009d 027c 016a 0864 033c 006e 327c 016a  ...|.j.d.<.n2|.j
+00000c80: 06a0 0764 04a1 0172 6c64 047c 049b 009d  ...d...rld.|....
+00000c90: 027c 016a 0864 033c 006e 147c 026a 09a0  .|.j.d.<.n.|.j..
+00000ca0: 0a64 057c 016a 069b 009d 02a1 0101 0064  .d.|.j.........d
+00000cb0: 067c 016a 0864 073c 007c 006a 0b9b 0064  .|.j.d.<.|.j...d
+00000cc0: 087c 006a 0c9b 009d 037d 0564 0974 0da0  .|.j.....}.d.t..
+00000cd0: 0e74 0f7c 0564 0a83 02a1 01a0 1064 0ba1  .t.|.d.......d..
+00000ce0: 0117 007d 067c 067c 016a 1164 0c3c 0064  ...}.|.|.j.d.<.d
+00000cf0: 0053 0029 0d4e 6700 0000 0000 00f0 3ffa  .S.).Ng.......?.
+00000d00: 0868 7474 7073 3a2f 2fda 0570 726f 7879  .https://..proxy
+00000d10: fa07 6874 7470 3a2f 2ffa 1372 6571 7565  ..http://..reque
+00000d20: 7374 2075 726c 2065 7272 6f72 3a20 545a  st url error: TZ
+00000d30: 0a64 6f6e 745f 7265 7472 79fa 013a 7a06  .dont_retry..:z.
+00000d40: 4261 7369 6320 da05 6173 6369 69da 0475  Basic ..ascii..u
+00000d50: 7466 387a 1350 726f 7879 2d41 7574 686f  tf8z.Proxy-Autho
+00000d60: 7269 7a61 7469 6f6e 2912 da02 6e70 da06  rization)...np..
+00000d70: 6172 676d 696e da07 765f 636f 756e 7472  argmin..v_countr
+00000d80: 2800 0000 da0c 7265 716e 756d 5f63 6f75  (.....reqnum_cou
+00000d90: 6e74 da05 765f 7375 6dda 0375 726c da0a  nt..v_sum..url..
+00000da0: 7374 6172 7473 7769 7468 da04 6d65 7461  startswith..meta
+00000db0: da04 736c 6f67 da04 696e 666f da08 7573  ..slog..info..us
+00000dc0: 6572 6e61 6d65 da08 7061 7373 776f 7264  ername..password
+00000dd0: da06 6261 7365 3634 da11 7572 6c73 6166  ..base64..urlsaf
+00000de0: 655f 6236 3465 6e63 6f64 65da 0562 7974  e_b64encode..byt
+00000df0: 6573 da06 6465 636f 6465 da07 6865 6164  es..decode..head
+00000e00: 6572 7329 0772 1500 0000 da07 7265 7175  ers).r......requ
+00000e10: 6573 74da 0673 7069 6465 72da 1063 7572  est..spider..cur
+00000e20: 7265 6e74 5f69 705f 696e 6465 78da 0a63  rent_ip_index..c
+00000e30: 7572 7265 6e74 5f69 70da 0f70 726f 7879  urrent_ip..proxy
+00000e40: 5f75 7365 725f 7061 7373 da11 656e 636f  _user_pass..enco
+00000e50: 6465 645f 7573 6572 5f70 6173 7372 1800  ded_user_passr..
+00000e60: 0000 7218 0000 0072 1900 0000 da0f 7072  ..r....r......pr
+00000e70: 6f63 6573 735f 7265 7175 6573 7458 0000  ocess_requestX..
+00000e80: 0073 2200 0000 0002 0c01 0a03 1201 0803  .s".............
+00000e90: 0c01 1201 0c01 1202 1403 0a02 1201 0601  ................
+00000ea0: 08ff 0402 02fe 0603 7a30 5072 6976 6174  ........z0Privat
+00000eb0: 6550 726f 7879 446f 776e 6c6f 6164 6572  eProxyDownloader
+00000ec0: 4d69 6464 6c65 7761 7265 2e70 726f 6365  Middleware.proce
+00000ed0: 7373 5f72 6571 7565 7374 6304 0000 0000  ss_requestc.....
+00000ee0: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
+00000ef0: 0000 0073 ac00 0000 7c02 6a00 7c00 6a01  ...s....|.j.|.j.
+00000f00: 6b07 7210 7c02 5300 7402 a003 7c00 6a04  k.r.|.S.t...|.j.
+00000f10: a101 7d04 7c00 6a05 7c04 1900 7d05 7c00  ..}.|.j.|...}.|.
+00000f20: 6a06 7c04 0500 1900 6401 3700 0300 3c00  j.|.....d.7...<.
+00000f30: 7c00 a007 a100 0100 7c01 6a08 a009 6402  |.......|.j...d.
+00000f40: a101 725e 6402 7c05 9b00 9d02 7c01 6a0a  ..r^d.|.....|.j.
+00000f50: 6403 3c00 6e32 7c01 6a08 a009 6404 a101  d.<.n2|.j...d...
+00000f60: 727c 6404 7c05 9b00 9d02 7c01 6a0a 6403  r|d.|.....|.j.d.
+00000f70: 3c00 6e14 7c03 6a0b a00c 6405 7c01 6a08  <.n.|.j...d.|.j.
+00000f80: 9b00 9d02 a101 0100 740d 7c02 6a00 8301  ........t.|.j...
+00000f90: 7d06 7c00 a00e 7c01 7c06 7c03 a103 70aa  }.|...|.|.|...p.
+00000fa0: 7c02 5300 2906 4ee9 0100 0000 7239 0000  |.S.).N.....r9..
+00000fb0: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
+00000fc0: 290f da06 7374 6174 7573 5a10 7265 7472  )...statusZ.retr
+00000fd0: 795f 6874 7470 5f63 6f64 6573 7240 0000  y_http_codesr@..
+00000fe0: 0072 4100 0000 7242 0000 0072 2800 0000  .rA...rB...r(...
+00000ff0: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
+00001000: 4600 0000 7247 0000 0072 4800 0000 da05  F...rG...rH.....
+00001010: 6572 726f 7272 0900 0000 da06 5f72 6574  errorr......_ret
+00001020: 7279 2907 7215 0000 0072 5100 0000 da08  ry).r....rQ.....
+00001030: 7265 7370 6f6e 7365 7252 0000 0072 5300  responserR...rS.
+00001040: 0000 7254 0000 00da 0672 6561 736f 6e72  ..rT.....reasonr
+00001050: 1800 0000 7218 0000 0072 1900 0000 da10  ....r....r......
+00001060: 7072 6f63 6573 735f 7265 7370 6f6e 7365  process_response
+00001070: 7200 0000 731a 0000 0000 010c 0104 020c  r...s...........
+00001080: 010a 0312 0108 020c 0112 010c 0112 0214  ................
+00001090: 020a 017a 3150 7269 7661 7465 5072 6f78  ...z1PrivateProx
+000010a0: 7944 6f77 6e6c 6f61 6465 724d 6964 646c  yDownloaderMiddl
+000010b0: 6577 6172 652e 7072 6f63 6573 735f 7265  eware.process_re
+000010c0: 7370 6f6e 7365 6304 0000 0000 0000 0000  sponsec.........
+000010d0: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+000010e0: 6e02 0000 7400 7c02 7c00 6a01 8302 9002  n...t.|.|.j.....
+000010f0: 726a 7c01 6a02 6401 1900 a003 6402 6402  rj|.j.d.....d.d.
+00001100: 1a00 a101 6403 1900 7d04 6404 a004 7c00  ....d...}.d...|.
+00001110: 6a05 6405 1900 7c00 6a05 6406 1900 7c04  j.d...|.j.d...|.
+00001120: a103 7d05 7406 a007 7c05 a101 a008 a100  ..}.t...|.......
+00001130: 7d06 7c06 6407 1900 7c04 1900 9002 7308  }.|.d...|.....s.
+00001140: 7c04 7c00 6a09 6b06 9001 72d8 7c03 6a0a  |.|.j.k...r.|.j.
+00001150: a00b 6408 a101 0100 7c00 6a09 a00c 7c04  ..d.....|.j...|.
+00001160: a101 7d07 7c00 6a09 a00d 7c07 a101 0100  ..}.|.j...|.....
+00001170: 740e 6a0f 7c00 6a10 7c07 6409 640a 8d03  t.j.|.j.|.d.d...
+00001180: 7c00 5f10 740e 6a0f 7c00 6a11 7c07 6409  |._.t.j.|.j.|.d.
+00001190: 640a 8d03 7c00 5f11 740e a012 7c00 6a13  d...|._.t...|.j.
+000011a0: a101 640b 6b05 9001 722a 7414 7c00 6a09  ..d.k...r*t.|.j.
+000011b0: 8301 640c 6b00 9001 722a 7c00 a015 640d  ..d.k...r*|...d.
+000011c0: a101 4400 5d46 7d08 7c00 6a09 a016 7c08  ..D.]F}.|.j...|.
+000011d0: a101 0100 740e a016 7c00 6a10 640e a102  ....t...|.j.d...
+000011e0: 7c00 5f10 740e a016 7c00 6a11 6409 a102  |._.t...|.j.d...
+000011f0: 7c00 5f11 7c08 7d04 7c00 6a11 6403 0500  |._.|.}.|.j.d...
+00001200: 1900 640f 3700 0300 3c00 71e0 6e8c 7414  ..d.7...<.q.n.t.
+00001210: 7c00 6a09 8301 7c00 6a17 6b00 9001 728e  |.j...|.j.k...r.
+00001220: 7c00 a015 640f a101 6409 1900 7d08 7c00  |...d...d...}.|.
+00001230: 6a09 a016 7c08 a101 0100 740e a016 7c00  j...|.....t...|.
+00001240: 6a10 640e a102 7c00 5f10 740e a016 7c00  j.d...|._.t...|.
+00001250: 6a11 6409 a102 7c00 5f11 7c08 7d04 7c00  j.d...|._.|.}.|.
+00001260: 6a11 6403 0500 1900 640f 3700 0300 3c00  j.d.....d.7...<.
+00001270: 6e28 740e a018 7c00 6a13 a101 7d07 7c00  n(t...|.j...}.|.
+00001280: 6a09 7c07 1900 7d04 7c00 6a11 7c07 0500  j.|...}.|.j.|...
+00001290: 1900 640f 3700 0300 3c00 7c03 6a0a a00b  ..d.7...<.|.j...
+000012a0: 6410 7414 7c00 6a09 8301 9b00 9d02 a101  d.t.|.j.........
+000012b0: 0100 7c00 a019 a100 0100 6e30 740e a018  ..|.......n0t...
+000012c0: 7c00 6a13 a101 7d07 7c00 6a09 7c07 1900  |.j...}.|.j.|...
+000012d0: 7d04 7c00 6a11 7c07 0500 1900 640f 3700  }.|.j.|.....d.7.
+000012e0: 0300 3c00 7c00 a019 a100 0100 7c01 6a1a  ..<.|.......|.j.
+000012f0: a01b 6411 a101 9002 7228 6412 a004 7c04  ..d.....r(d...|.
+00001300: a101 7c01 6a02 6401 3c00 6e34 7c01 6a1a  ..|.j.d.<.n4|.j.
+00001310: a01b 6413 a101 9002 7248 6414 a004 7c04  ..d.....rHd...|.
+00001320: a101 7c01 6a02 6401 3c00 6e14 7c03 6a0a  ..|.j.d.<.n.|.j.
+00001330: a00b 6415 7c01 6a1a 9b00 9d02 a101 0100  ..d.|.j.........
+00001340: 7c00 a01c 7c01 7c02 7c03 a103 5300 6400  |...|.|.|...S.d.
+00001350: 5300 2916 4e72 3a00 0000 da00 e9ff ffff  S.).Nr:.........
+00001360: ff7a 4968 7474 7073 3a2f 2f64 7073 2e6b  .zIhttps://dps.k
+00001370: 646c 6170 692e 636f 6d2f 6170 692f 6368  dlapi.com/api/ch
+00001380: 6563 6b64 7073 7661 6c69 643f 6f72 6465  eckdpsvalid?orde
+00001390: 7269 643d 7b7d 2673 6967 6e61 7475 7265  rid={}&signature
+000013a0: 3d7b 7d26 7072 6f78 793d 7b7d 7224 0000  ={}&proxy={}r$..
+000013b0: 0072 2500 0000 7227 0000 0075 0800 0000  .r%...r'...u....
+000013c0: e69b b4e6 96b0 6970 7201 0000 0029 01da  ......ipr....)..
+000013d0: 0461 7869 7367 0000 0000 0000 1240 e907  .axisg.......@..
+000013e0: 0000 00e9 0200 0000 e700 0000 0000 00e0  ................
+000013f0: 3f72 5800 0000 7523 0000 00e7 9bae e589  ?rX...u#........
+00001400: 8d20 6970 20e6 b1a0 e5ad 98e9 878f 2069  . ip ......... i
+00001410: 7020 e695 b0e9 878f e4b8 baef bc9a 7239  p ............r9
+00001420: 0000 007a 0a68 7474 7073 3a2f 2f7b 7d72  ...z.https://{}r
+00001430: 3b00 0000 7a09 6874 7470 3a2f 2f7b 7d72  ;...z.http://{}r
+00001440: 3c00 0000 291d da0a 6973 696e 7374 616e  <...)...isinstan
+00001450: 6365 5a13 4558 4345 5054 494f 4e53 5f54  ceZ.EXCEPTIONS_T
+00001460: 4f5f 5245 5452 5972 4700 0000 da05 7370  O_RETRYrG.....sp
+00001470: 6c69 74da 0666 6f72 6d61 7472 2d00 0000  lit..formatr-...
+00001480: 722f 0000 0072 1b00 0000 7230 0000 0072  r/...r....r0...r
+00001490: 2800 0000 7248 0000 0072 4900 0000 da05  (...rH...rI.....
+000014a0: 696e 6465 78da 0370 6f70 7240 0000 00da  index..popr@....
+000014b0: 0664 656c 6574 65da 0a74 696d 655f 636f  .delete..time_co
+000014c0: 756e 7472 4300 0000 da07 6176 6572 6167  untrC.....averag
+000014d0: 6572 4200 0000 da03 6c65 6e72 3800 0000  erB.....lenr8...
+000014e0: da06 6170 7065 6e64 da0e 7072 6f78 7970  ..append..proxyp
+000014f0: 6f6f 6c5f 7369 7a65 7241 0000 0072 4400  ool_sizerA...rD.
+00001500: 0000 7245 0000 0072 4600 0000 725b 0000  ..rE...rF...r[..
+00001510: 0029 0972 1500 0000 7251 0000 00da 0965  .).r....rQ.....e
+00001520: 7863 6570 7469 6f6e 7252 0000 0072 5400  xceptionrR...rT.
+00001530: 0000 7245 0000 00da 0969 735f 6578 6973  ..rE.....is_exis
+00001540: 7473 7253 0000 005a 066e 6577 5f69 7072  tsrS...Z.new_ipr
+00001550: 1800 0000 7218 0000 0072 1900 0000 da11  ....r....r......
+00001560: 7072 6f63 6573 735f 6578 6365 7074 696f  process_exceptio
+00001570: 6e87 0000 0073 6800 0000 0001 0e01 1801  n....sh.........
+00001580: 0401 0801 0801 02fd 0405 0e01 0e01 0c01  ................
+00001590: 0c02 0c01 0c01 0401 0400 0200 02ff 0803  ................
+000015a0: 0401 0400 0200 02ff 0805 2201 0e01 0c01  ..........".....
+000015b0: 1001 1001 0401 1601 1201 0e01 0c01 1001  ................
+000015c0: 1001 0401 1402 0c01 0a01 1202 1801 0a02  ................
+000015d0: 0c01 0a01 1201 0802 0e01 1201 0e01 1202  ................
+000015e0: 1402 7a32 5072 6976 6174 6550 726f 7879  ..z2PrivateProxy
+000015f0: 446f 776e 6c6f 6164 6572 4d69 6464 6c65  DownloaderMiddle
+00001600: 7761 7265 2e70 726f 6365 7373 5f65 7863  ware.process_exc
+00001610: 6570 7469 6f6e 6301 0000 0000 0000 0000  eptionc.........
+00001620: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00001630: 1200 0000 7c00 6a00 7c00 6a01 1b00 7c00  ....|.j.|.j...|.
+00001640: 5f02 6400 5300 2901 4e29 0372 4300 0000  _.d.S.).N).rC...
+00001650: 726b 0000 0072 4200 0000 2901 7215 0000  rk...rB...).r...
+00001660: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001670: 7244 0000 00c2 0000 0073 0200 0000 0001  rD.......s......
+00001680: 7a26 5072 6976 6174 6550 726f 7879 446f  z&PrivateProxyDo
+00001690: 776e 6c6f 6164 6572 4d69 6464 6c65 7761  wnloaderMiddlewa
+000016a0: 7265 2e76 5f73 756d 6302 0000 0000 0000  re.v_sumc.......
+000016b0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000016c0: 0073 2600 0000 7c00 6a00 7322 7401 a002  .s&...|.j.s"t...
+000016d0: 6401 a101 0100 7403 a004 7c00 6a05 6401  d.....t...|.j.d.
+000016e0: a102 7c00 5f05 7100 6400 5300 2902 4e67  ..|._.q.d.S.).Ng
+000016f0: 9a99 9999 9999 c93f 2906 da08 656e 645f  .......?)...end_
+00001700: 7469 6d65 da04 7469 6d65 da05 736c 6565  time..time..slee
+00001710: 7072 4000 0000 da03 6164 6472 6b00 0000  pr@.....addrk...
+00001720: a902 7215 0000 0072 5200 0000 7218 0000  ..r....rR...r...
+00001730: 0072 1800 0000 7219 0000 00da 0563 6c6f  .r....r......clo
+00001740: 636b c500 0000 7306 0000 0000 0106 010a  ck....s.........
+00001750: 017a 2650 7269 7661 7465 5072 6f78 7944  .z&PrivateProxyD
+00001760: 6f77 6e6c 6f61 6465 724d 6964 646c 6577  ownloaderMiddlew
+00001770: 6172 652e 636c 6f63 6b63 0200 0000 0000  are.clockc......
+00001780: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00001790: 0000 7314 0100 0074 0083 007d 0274 01a0  ..s....t...}.t..
+000017a0: 0264 0164 0164 029c 02a1 017d 0374 01a0  .d.d.d.....}.t..
+000017b0: 037c 03a1 017c 005f 047c 006a 0464 0319  .|...|._.|.j.d..
+000017c0: 007c 005f 057c 006a 0464 0419 007c 005f  .|._.|.j.d...|._
+000017d0: 067c 02a0 0764 05a1 0172 807c 02a0 0764  .|...d...r.|...d
+000017e0: 05a1 0164 066b 0072 5c74 0864 0783 0182  ...d.k.r\t.d....
+000017f0: 016e 167c 02a0 0764 05a1 0164 086b 0472  .n.|...d...d.k.r
+00001800: 7274 0864 0983 0182 017c 02a0 0764 05a1  rt.d.....|...d..
+00001810: 017c 005f 096e 0664 067c 005f 0964 0a7c  .|._.n.d.|._.d.|
+00001820: 005f 0a74 0ba0 0c7c 006a 0966 01a1 0164  ._.t...|.j.f...d
+00001830: 0b17 007c 005f 0d74 0ba0 0c7c 006a 0966  ...|._.t...|.j.f
+00001840: 01a1 017c 005f 0e7c 00a0 0fa1 0001 0074  ...|._.|.......t
+00001850: 107c 006a 117c 0166 0164 0c64 0d8d 037c  .|.j.|.f.d.d...|
+00001860: 005f 127c 006a 12a0 13a1 0001 007c 00a0  ._.|.j.......|..
+00001870: 147c 006a 0964 0ca1 0201 007c 016a 15a0  .|.j.d.....|.j..
+00001880: 1664 0e74 177c 006a 1883 019b 009d 02a1  .d.t.|.j........
+00001890: 0101 007c 016a 15a0 1664 0f7c 016a 199b  ...|.j...d.|.j..
+000018a0: 009d 02a1 0101 0064 0053 0029 104e 7a03  .......d.S.).Nz.
+000018b0: 2a2a 2a29 0272 4a00 0000 724b 0000 0072  ***).rJ...rK...r
+000018c0: 4a00 0000 724b 0000 005a 0853 4d50 5053  J...rK...Z.SMPPS
+000018d0: 495a 4572 5800 0000 756d 0000 00e6 82a8  IZErX...um......
+000018e0: e8be 93e5 85a5 e79a 8420 6970 20e6 b1a0  ......... ip ...
+000018f0: e5ad 90e5 a4a7 e5b0 8fe4 b88d e883 bde5  ................
+00001900: b08f e4ba 8e20 31ef bc81 e8af b7e9 878d  ..... 1.........
+00001910: e696 b0e4 bfae e694 b920 7365 7474 696e  ......... settin
+00001920: 6773 20e4 b8ad e79a 8420 534d 5050 5349  gs ...... SMPPSI
+00001930: 5a45 20e7 9a84 e580 bce4 b8ba e5a4 a7e4  ZE .............
+00001940: ba8e e7ad 89e4 ba8e 2031 7262 0000 0075  ........ 1rb...u
+00001950: 4b00 0000 e4bd a0e7 a4bc e8b2 8ce5 9097  K...............
+00001960: efbc 8c69 7020 e6b1 a0e6 9c80 e5a4 a7e6  ...ip ..........
+00001970: 95b0 e987 8fe4 b88d e58f afe4 bba5 e8b6  ................
+00001980: 85e8 bf87 2037 20e4 b8aa efbc 81e8 afb7  .... 7 .........
+00001990: e987 8de6 96b0 e8ae bee7 bdae efbc 8146  ...............F
+000019a0: 7264 0000 0054 2903 da06 7461 7267 6574  rd...T)...target
+000019b0: da04 6172 6773 da06 6461 656d 6f6e 7525  ..args..daemonu%
+000019c0: 0000 00e5 889d e5a7 8be5 8c96 2069 7020  ............ ip 
+000019d0: e5ad 97e5 85b8 efbc 8c69 7020 e695 b0e9  .........ip ....
+000019e0: 878f e4b8 baef bc9a 7a29 5072 6976 6174  ........z)Privat
+000019f0: 6550 726f 7879 446f 776e 6c6f 6164 6572  eProxyDownloader
+00001a00: 4d69 6464 6c65 7761 7265 206f 7065 6e65  Middleware opene
+00001a10: 643a 2029 1a72 0800 0000 7230 0000 00da  d: ).r....r0....
+00001a20: 0564 756d 7073 da05 6c6f 6164 7372 2d00  .dumps..loadsr-.
+00001a30: 0000 724a 0000 0072 4b00 0000 721b 0000  ..rJ...rK...r...
+00001a40: 0072 2e00 0000 726f 0000 0072 7300 0000  .r....ro...rs...
+00001a50: 7240 0000 00da 057a 6572 6f73 726b 0000  r@.....zerosrk..
+00001a60: 0072 4300 0000 7244 0000 0072 0200 0000  .rC...rD...r....
+00001a70: 7278 0000 00da 0174 da05 7374 6172 7472  rx.....t..startr
+00001a80: 3800 0000 7248 0000 0072 4900 0000 726d  8...rH...rI...rm
+00001a90: 0000 0072 2800 0000 da04 6e61 6d65 2904  ...r(.....name).
+00001aa0: 7215 0000 0072 5200 0000 7210 0000 00da  r....rR...r.....
+00001ab0: 0472 6573 7872 1800 0000 7218 0000 0072  .resxr....r....r
+00001ac0: 1900 0000 721d 0000 00ca 0000 0073 2e00  ....r........s..
+00001ad0: 0000 0001 0602 1001 0c01 0c01 0c02 0a01  ................
+00001ae0: 0e01 0201 02ff 0603 0e01 0802 0e02 0601  ................
+00001af0: 0601 1401 1001 0801 1401 0a01 0e01 1801  ................
+00001b00: 7a2e 5072 6976 6174 6550 726f 7879 446f  z.PrivateProxyDo
+00001b10: 776e 6c6f 6164 6572 4d69 6464 6c65 7761  wnloaderMiddlewa
+00001b20: 7265 2e73 7069 6465 725f 6f70 656e 6564  re.spider_opened
+00001b30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001b40: 0004 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
+00001b50: 7c00 5f00 7c00 6a01 a002 a100 0100 7c01  |._.|.j.......|.
+00001b60: 6a03 a004 6402 7c01 6a05 9b00 9d02 a101  j...d.|.j.......
+00001b70: 0100 6400 5300 2903 4e54 7a29 5072 6976  ..d.S.).NTz)Priv
+00001b80: 6174 6550 726f 7879 446f 776e 6c6f 6164  ateProxyDownload
+00001b90: 6572 4d69 6464 6c65 7761 7265 2063 6c6f  erMiddleware clo
+00001ba0: 7365 643a 2029 0672 7300 0000 727f 0000  sed: ).rs...r...
+00001bb0: 00da 046a 6f69 6e72 4800 0000 7249 0000  ...joinrH...rI..
+00001bc0: 0072 8100 0000 7277 0000 0072 1800 0000  .r....rw...r....
+00001bd0: 7218 0000 0072 1900 0000 721e 0000 00e7  r....r....r.....
+00001be0: 0000 0073 0600 0000 0001 0601 0a01 7a2e  ...s..........z.
+00001bf0: 5072 6976 6174 6550 726f 7879 446f 776e  PrivateProxyDown
+00001c00: 6c6f 6164 6572 4d69 6464 6c65 7761 7265  loaderMiddleware
+00001c10: 2e73 7069 6465 725f 636c 6f73 6564 2901  .spider_closed).
+00001c20: 4e29 16da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00001c30: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001c40: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00001c50: da03 7374 7272 1200 0000 da0b 636c 6173  ..strr......clas
+00001c60: 736d 6574 686f 6472 2200 0000 7204 0000  smethodr"...r...
+00001c70: 0072 0b00 0000 da09 7265 7472 795f 6e75  .r......retry_nu
+00001c80: 6d72 0300 0000 da04 626f 6f6c 7238 0000  mr......boolr8..
+00001c90: 0072 5700 0000 725e 0000 0072 7200 0000  .rW...r^...rr...
+00001ca0: 7244 0000 0072 7800 0000 721d 0000 0072  rD...rx...r....r
+00001cb0: 1e00 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00001cc0: 6c5f 5f72 1800 0000 7218 0000 0072 1600  l__r....r....r..
+00001cd0: 0000 7219 0000 0072 0c00 0000 1500 0000  ..r....r........
+00001ce0: 731a 0000 0008 0104 0412 0602 010a 060a  s...............
+00001cf0: 0116 3008 1a08 1508 3b08 0308 0508 1d72  ..0.....;......r
+00001d00: 0c00 0000 291c 724c 0000 0072 3000 0000  ....).rL...r0...
+00001d10: 7274 0000 0072 3200 0000 da09 7468 7265  rt...r2.....thre
+00001d20: 6164 696e 6772 0200 0000 da06 7479 7069  adingr......typi
+00001d30: 6e67 7203 0000 00da 056e 756d 7079 7240  ngr......numpyr@
+00001d40: 0000 0072 2f00 0000 da08 7265 7472 7969  ...r/.....retryi
+00001d50: 6e67 7204 0000 00da 0673 6372 6170 7972  ngr......scrapyr
+00001d60: 0500 0000 5a22 7363 7261 7079 2e64 6f77  ....Z"scrapy.dow
+00001d70: 6e6c 6f61 6465 726d 6964 646c 6577 6172  nloadermiddlewar
+00001d80: 6573 2e72 6574 7279 7206 0000 00da 0f73  es.retryr......s
+00001d90: 6372 6170 792e 7365 7474 696e 6773 7207  crapy.settingsr.
+00001da0: 0000 005a 1473 6372 6170 792e 7574 696c  ...Z.scrapy.util
+00001db0: 732e 7072 6f6a 6563 7472 0800 0000 da15  s.projectr......
+00001dc0: 7363 7261 7079 2e75 7469 6c73 2e72 6573  scrapy.utils.res
+00001dd0: 706f 6e73 6572 0900 0000 5a21 576f 726b  ponser....Z!Work
+00001de0: 5765 6978 696e 526f 626f 742e 776f 726b  WeixinRobot.work
+00001df0: 5f77 6569 7869 6e5f 726f 626f 7472 0a00  _weixin_robotr..
+00001e00: 0000 da1e 6179 7567 6573 7069 6465 7274  ....ayugespidert
+00001e10: 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7061 7261  ools.common.para
+00001e20: 6d73 720b 0000 0072 0c00 0000 7218 0000  msr....r....r...
+00001e30: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001e40: da08 3c6d 6f64 756c 653e 0100 0000 7320  ..<module>....s 
+00001e50: 0000 0008 0108 0108 0108 010c 010c 0208  ................
+00001e60: 0108 010c 010c 010c 010c 010c 010c 010c  ................
+00001e70: 020c 03                                  ...
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 
 from scrapy import signals
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
 
 
 class DynamicProxyDownloaderMiddleware(object):
     """
     动态隧道代理中间件
     """
 
@@ -15,21 +15,21 @@
         """
         从 scrapy 配置中取出动态隧道代理的信息
         """
         dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
         # 查看动态隧道代理配置是否符合要求
         is_match = ReuseOperation.is_dict_meet_min_limit(
             dict_conf=dynamic_proxy_conf,
-            key_list=["PROXY_URL", "USERNAME", "PASSWORD"],
+            key_list=["proxy", "username", "password"],
         )
         assert is_match, f"没有配置动态隧道代理，配置示例为：{Param.dynamic_proxy_conf_example}"
 
-        self.proxy_url = dynamic_proxy_conf["PROXY_URL"]
-        self.username = dynamic_proxy_conf["USERNAME"]
-        self.password = dynamic_proxy_conf["PASSWORD"]
+        self.proxy_url = dynamic_proxy_conf["proxy"]
+        self.username = dynamic_proxy_conf["username"]
+        self.password = dynamic_proxy_conf["password"]
 
     @classmethod
     def from_crawler(cls, crawler):
         s = cls(crawler.settings)
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
@@ -71,21 +71,21 @@
         Args:
             settings: scrapy 配置信息
         """
         dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
         # 查看动态隧道代理配置是否符合要求
         is_match = ReuseOperation.is_dict_meet_min_limit(
             dict_conf=dynamic_proxy_conf,
-            key_list=["PROXY_URL", "USERNAME", "PASSWORD"],
+            key_list=["proxy", "username", "password"],
         )
         assert is_match, f"没有配置动态隧道代理，配置示例为：{Param.dynamic_proxy_conf_example}"
 
-        self.proxy_url = dynamic_proxy_conf["PROXY_URL"]
-        self.username = dynamic_proxy_conf["USERNAME"]
-        self.password = dynamic_proxy_conf["PASSWORD"]
+        self.proxy_url = dynamic_proxy_conf["proxy"]
+        self.username = dynamic_proxy_conf["username"]
+        self.password = dynamic_proxy_conf["password"]
 
     @classmethod
     def from_crawler(cls, crawler):
         s = cls(crawler.settings)
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 
 import requests
 from scrapy import signals
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
 
 
 class ExclusiveProxyDownloaderMiddleware(object):
     """
     独享代理中间件
     """
 
@@ -18,22 +18,22 @@
         Args:
             exclusive_proxy_conf: 使用的独享代理的配置信息
         """
         self.proxy = None
         # 查看独享代理配置是否符合要求
         is_match = ReuseOperation.is_dict_meet_min_limit(
             dict_conf=exclusive_proxy_conf,
-            key_list=["PROXY_URL", "USERNAME", "PASSWORD", "PROXY_INDEX"],
+            key_list=["proxy", "username", "password", "index"],
         )
         assert is_match, f"没有配置独享代理，配置示例为：{Param.exclusive_proxy_conf_example}"
 
-        self.proxy_url = exclusive_proxy_conf["PROXY_URL"]
-        self.username = exclusive_proxy_conf["USERNAME"]
-        self.password = exclusive_proxy_conf["PASSWORD"]
-        self.proxy_index = exclusive_proxy_conf["PROXY_INDEX"]
+        self.proxy_url = exclusive_proxy_conf["proxy"]
+        self.username = exclusive_proxy_conf["username"]
+        self.password = exclusive_proxy_conf["password"]
+        self.proxy_index = exclusive_proxy_conf["index"]
 
     @classmethod
     def from_crawler(cls, crawler):
         s = cls(
             exclusive_proxy_conf=crawler.settings.get("EXCLUSIVE_PROXY_CONFIG", None)
         )
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
@@ -47,15 +47,15 @@
             proxy_list.sort()
             if self.proxy_index < len(proxy_list):
                 self.proxy = proxy_list[self.proxy_index]
             else:
                 raise Exception("独享代理索引超出范围，请确认独享代理服务情况。")
 
         except Exception:
-            raise Exception("获取独享代理是失败，请及时查看。")
+            raise Exception("获取独享代理时失败，请查看独享配置及网络是否正常。")
 
     def process_request(self, request, spider):
         if request.url.startswith("https://"):
             request.meta["proxy"] = f"https://{self.proxy}"
         elif request.url.startswith("http://"):
             request.meta["proxy"] = f"http://{self.proxy}"
         else:
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from scrapy import signals
 from scrapy.downloadermiddlewares.retry import RetryMiddleware
 from scrapy.settings import Settings
 from scrapy.utils.project import get_project_settings
 from scrapy.utils.response import response_status_message
 from WorkWeixinRobot.work_weixin_robot import WWXRobot
 
-from ayugespidertools.common.Params import Param
+from ayugespidertools.common.params import Param
 
 
 class PrivateProxyDownloaderMiddleware(RetryMiddleware):
     """
     基于独享代理的自定义动态代理中间件，此中间件暂不使用，后期优化
     """
 
@@ -27,15 +27,15 @@
         self.settings = Settings()
         super(PrivateProxyDownloaderMiddleware, self).__init__(self.settings)
         self.important_error = False
         self.WWX = WWXRobot(key=wwx_robot_key)
 
     @classmethod
     def from_crawler(cls, crawler):
-        s = cls(wwx_robot_key=crawler.settings.get("WWXRobot_key", None))
+        s = cls(wwx_robot_key=crawler.settings.get("wxbot", None))
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         crawler.signals.connect(s.spider_closed, signal=signals.spider_closed)
         return s
 
     @retry(stop_max_attempt_number=Param.retry_num)
     def get_proxy_ip(self, size, isdict: Optional[bool] = None):
         proxy_url = (
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Apr 10 09:37:05 2023 UTC, .py size: 3022 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c1d8 3364 ce0b 0000  U.........3d....
+00000000: 550d 0d0a 0000 0000 4b42 4764 ce0b 0000  U.......KBGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6701 5a0b 4700 6407 6406 8400 6406 650a  g.Z.G.d.d...d.e.
@@ -174,21 +174,21 @@
 00000ad0: 2a00 0000 722c 0000 0072 3200 0000 da0d  *...r,...r2.....
 00000ae0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1300  __classcell__r..
 00000af0: 0000 7213 0000 0072 2800 0000 7214 0000  ..r....r(...r...
 00000b00: 0072 0800 0000 0d00 0000 7316 0000 0008  .r........s.....
 00000b10: 0104 0600 fe02 0202 0102 fd0c 1202 010a  ................
 00000b20: 050c 1308 044e 290d da06 7479 7069 6e67  .....N)...typing
 00000b30: 7202 0000 005a 2361 7975 6765 7370 6964  r....Z#ayugespid
-00000b40: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e4d  ertools.common.M
-00000b50: 6f6e 676f 4442 5069 7065 7203 0000 0072  ongoDBPiper....r
+00000b40: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e6d  ertools.common.m
+00000b50: 6f6e 676f 6462 7069 7065 7203 0000 0072  ongodbpiper....r
 00000b60: 0400 0000 da20 6179 7567 6573 7069 6465  ..... ayugespide
-00000b70: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 5479  rtools.common.Ty
-00000b80: 7065 5661 7273 7205 0000 00da 1d61 7975  peVarsr......ayu
+00000b70: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7479  rtools.common.ty
+00000b80: 7065 7661 7273 7205 0000 00da 1d61 7975  pevarsr......ayu
 00000b90: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00000ba0: 6d6d 6f6e 2e55 7469 6c73 7206 0000 005a  mmon.Utilsr....Z
+00000ba0: 6d6d 6f6e 2e75 7469 6c73 7206 0000 005a  mmon.utilsr....Z
 00000bb0: 1c61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
-00000bc0: 732e 4d6f 6e67 6f43 6c69 656e 7472 0700  s.MongoClientr..
+00000bc0: 732e 6d6f 6e67 6f63 6c69 656e 7472 0700  s.mongoclientr..
 00000bd0: 0000 da07 5f5f 616c 6c5f 5f72 0800 0000  ....__all__r....
 00000be0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
 00000bf0: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000c00: 0000 730e 0000 000c 0210 010c 010c 010c  ..s.............
 00000c10: 0302 ff04 05                             .....
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 12 02:07:09 2023 UTC, .py size: 1356 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 4d12 3664 4c05 0000  U.......M.6dL...
+00000000: 550d 0d0a 0000 0000 5a42 4764 4c05 0000  U.......ZBGdL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6405 6701 5a0a 4700 6406  m.Z...d.g.Z.G.d.
 00000070: 6405 8400 6405 6509 8303 5a0b 6407 5300  d...d.e...Z.d.S.
@@ -96,18 +96,18 @@
 000005f0: 7219 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
 00000600: 6c6c 5f5f 7211 0000 0072 1100 0000 720f  ll__r....r....r.
 00000610: 0000 0072 1200 0000 7208 0000 000c 0000  ...r....r.......
 00000620: 0073 0c00 0000 0801 0404 0c03 0804 0401  .s..............
 00000630: 0a06 4e29 0cda 1074 7769 7374 6564 2e69  ..N)...twisted.i
 00000640: 6e74 6572 6e65 7472 0200 0000 7203 0000  nternetr....r...
 00000650: 00da 2361 7975 6765 7370 6964 6572 746f  ..#ayugespiderto
-00000660: 6f6c 732e 636f 6d6d 6f6e 2e4d 6f6e 676f  ols.common.Mongo
-00000670: 4442 5069 7065 7204 0000 0072 0500 0000  DBPiper....r....
+00000660: 6f6c 732e 636f 6d6d 6f6e 2e6d 6f6e 676f  ols.common.mongo
+00000670: 6462 7069 7065 7204 0000 0072 0500 0000  dbpiper....r....
 00000680: da1d 6179 7567 6573 7069 6465 7274 6f6f  ..ayugespidertoo
-00000690: 6c73 2e63 6f6d 6d6f 6e2e 5574 696c 7372  ls.common.Utilsr
+00000690: 6c73 2e63 6f6d 6d6f 6e2e 7574 696c 7372  ls.common.utilsr
 000006a0: 0600 0000 da30 6179 7567 6573 7069 6465  .....0ayugespide
 000006b0: 7274 6f6f 6c73 2e73 6372 6170 6572 2e70  rtools.scraper.p
 000006c0: 6970 656c 696e 6573 2e6d 6f6e 676f 2e66  ipelines.mongo.f
 000006d0: 616e 7461 7379 7207 0000 00da 075f 5f61  antasyr......__a
 000006e0: 6c6c 5f5f 7208 0000 0072 1100 0000 7211  ll__r....r....r.
 000006f0: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
 00000700: 6d6f 6475 6c65 3e01 0000 0073 0c00 0000  module>....s....
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
-from ayugespidertools.common.MongoDBPipe import Synchronize, mongodb_pipe
-from ayugespidertools.common.TypeVars import MongoDBConfig
-from ayugespidertools.common.Utils import ToolsForAyu
-from ayugespidertools.MongoClient import MongoDbBase
+from ayugespidertools.common.mongodbpipe import Synchronize, mongodb_pipe
+from ayugespidertools.common.typevars import MongoDBConfig
+from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.mongoclient import MongoDbBase
 
 __all__ = [
     "AyuFtyMongoPipeline",
 ]
 
 
 class AyuFtyMongoPipeline(MongoDbBase):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from twisted.internet import defer, reactor
 
-from ayugespidertools.common.MongoDBPipe import TwistedAsynchronous, mongodb_pipe
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.mongodbpipe import TwistedAsynchronous, mongodb_pipe
+from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 
 __all__ = [
     "AyuTwistedMongoPipeline",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 import warnings
 from typing import Optional, Tuple, Type
 
 import pymysql
 from retrying import retry
 
-from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.MysqlErrorHandle import Synchronize, deal_mysql_err
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import AlterItem, MysqlConfig, TableEnumTypeVar
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.mysqlerrhandle import Synchronize, deal_mysql_err
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import AlterItem, MysqlConfig, TableEnumTypeVar
+from ayugespidertools.common.utils import ToolsForAyu
 
 # 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
 warnings.filterwarnings(
     "error", category=pymysql.Warning, message=".*Data truncated for column.*"
 )
 
 __all__ = [
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 06:55:07 2023 UTC, .py size: 13398 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cb3e 3e64 5634 0000  U........>>dV4..
+00000000: 550d 0d0a 0000 0000 7142 4764 5434 0000  U.......qBGdT4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6400 6403 6c07  ..d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -98,15 +98,15 @@
 00000610: 0206 0106 0106 0106 0106 017a 1941 7975  ...........z.Ayu
 00000620: 4d79 7371 6c50 6970 656c 696e 652e 5f5f  MysqlPipeline.__
 00000630: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
 00000640: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
 00000650: 3400 0000 7c00 7c01 6a00 a001 6401 6402  4...|.|.j...d.d.
 00000660: a102 7c01 6a00 a001 6403 a101 7c01 6a00  ..|.j...d...|.j.
 00000670: a001 6404 a101 7c01 6a00 a001 6405 6406  ..d...|.j...d.d.
-00000680: a102 6407 8d04 5300 2908 4eda 124d 5953  ..d...S.).N..MYS
+00000680: a102 6407 8d04 5300 2908 4e5a 124d 5953  ..d...S.).NZ.MYS
 00000690: 514c 5f54 4142 4c45 5f50 5245 4649 58da  QL_TABLE_PREFIX.
 000006a0: 00da 0944 4154 415f 454e 554d da03 454e  ...DATA_ENUM..EN
 000006b0: 56da 1352 4543 4f52 445f 4c4f 475f 544f  V..RECORD_LOG_TO
 000006c0: 5f4d 5953 514c 4629 0472 1300 0000 7214  _MYSQLF).r....r.
 000006d0: 0000 0072 1500 0000 7216 0000 0029 02da  ...r....r....)..
 000006e0: 0873 6574 7469 6e67 73da 0367 6574 2902  .settings..get).
 000006f0: da03 636c 73da 0763 7261 776c 6572 7222  ..cls..crawlerr"
@@ -160,16 +160,16 @@
 000009f0: 8f82 e695 b0fa 0120 755d 0000 00e6 95b0  ....... u]......
 00000a00: e68d aee8 a1a8 e590 8de4 b88d e883 bde5  ................
 00000a10: 90ab e7a9 bae6 a0bc efbc 8ce8 afb7 e6a3  ................
 00000a20: 80e6 9fa5 204d 5953 514c 5f54 4142 4c45  .... MYSQL_TABLE
 00000a30: 5f50 5245 4649 5820 e58f 82e6 95b0 e592  _PREFIX ........
 00000a40: 8c20 6974 656d 20e4 b8ad e79a 8420 7461  . item ...... ta
 00000a50: 626c 6520 e58f 82e6 95b0 2904 da0a 6973  ble ......)...is
-00000a60: 696e 7374 616e 6365 da03 7374 7272 3000  instance..strr0.
-00000a70: 0000 7213 0000 0029 0372 2100 0000 7235  ..r....).r!...r5
+00000a60: 696e 7374 616e 6365 da03 7374 7272 2f00  instance..strr/.
+00000a70: 0000 7213 0000 0029 0372 2100 0000 7234  ..r....).r!...r4
 00000a80: 0000 005a 0f66 756c 6c5f 7461 626c 655f  ...Z.full_table_
 00000a90: 6e61 6d65 7222 0000 0072 2200 0000 7223  namer"...r"...r#
 00000aa0: 0000 00da 0e67 6574 5f74 6162 6c65 5f6e  .....get_table_n
 00000ab0: 616d 654f 0000 0073 0e00 0000 0009 1201  ameO...s........
 00000ac0: 0e04 06ff 0402 02fe 0403 7a1f 4179 754d  ..........z.AyuM
 00000ad0: 7973 716c 5069 7065 6c69 6e65 2e67 6574  ysqlPipeline.get
 00000ae0: 5f74 6162 6c65 5f6e 616d 6529 0172 1700  _table_name).r..
@@ -197,28 +197,28 @@
 00000c40: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
 00000c50: 6974 656d 3a20 7363 7261 7079 2069 7465  item: scrapy ite
 00000c60: 6d0a 0a20 2020 2020 2020 2052 6574 7572  m..        Retur
 00000c70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
 00000c80: 3129 2e20 e695 b4e5 9088 e590 8ee7 9a84  1). ............
 00000c90: 2069 7465 6d0a 2020 2020 2020 2020 da07   item.        ..
 00000ca0: 616c 6c64 6174 61da 096b 6579 5f76 616c  alldata..key_val
-00000cb0: 7565 7226 0000 00da 056e 6f74 6573 7235  uer&.....notesr5
+00000cb0: 7565 7225 0000 00da 056e 6f74 6573 7234  uer%.....notesr4
 00000cc0: 0000 00da 0969 7465 6d5f 6d6f 6465 2902  .....item_mode).
 00000cd0: da09 6469 6374 5f63 6f6e 66da 086b 6579  ..dict_conf..key
 00000ce0: 5f6c 6973 7429 02da 086e 6577 5f69 7465  _list)...new_ite
-00000cf0: 6dda 096e 6f74 6573 5f64 6963 290e 722b  m..notes_dic).r+
-00000d00: 0000 00da 0361 6c6c 7237 0000 00da 0464  .....allr7.....d
+00000cf0: 6dda 096e 6f74 6573 5f64 6963 290e 722a  m..notes_dic).r*
+00000d00: 0000 00da 0361 6c6c 7236 0000 00da 0464  .....allr6.....d
 00000d10: 6963 74da 046e 6578 74da 0469 7465 72da  ict..next..iter.
 00000d20: 0676 616c 7565 7372 0700 0000 da16 6973  .valuesr......is
 00000d30: 5f6e 616d 6564 7475 706c 655f 696e 7374  _namedtuple_inst
-00000d40: 616e 6365 da05 6974 656d 7372 3b00 0000  ance..itemsr;...
-00000d50: 723c 0000 00da 1567 6574 5f69 7465 6d73  r<.....get_items
+00000d40: 616e 6365 da05 6974 656d 7372 3a00 0000  ance..itemsr:...
+00000d50: 723b 0000 00da 1567 6574 5f69 7465 6d73  r;.....get_items
 00000d60: 5f65 7863 6570 745f 6b65 7973 720b 0000  _except_keysr...
-00000d70: 0029 0972 2100 0000 da04 6974 656d 7240  .).r!.....itemr@
-00000d80: 0000 0072 4100 0000 da0b 696e 7365 7274  ...rA.....insert
+00000d70: 0029 0972 2100 0000 da04 6974 656d 723f  .).r!.....itemr?
+00000d80: 0000 0072 4000 0000 da0b 696e 7365 7274  ...r@.....insert
 00000d90: 5f64 6174 61da 0a6a 7564 6765 5f69 7465  _data..judge_ite
 00000da0: 6dda 036b 6579 da05 7661 6c75 655a 0e73  m..key..valueZ.s
 00000db0: 6176 655f 6461 7461 5f69 7465 6d72 2200  ave_data_itemr".
 00000dc0: 0000 7222 0000 0072 2300 0000 da0c 6765  ..r"...r#.....ge
 00000dd0: 745f 6e65 775f 6974 656d 6100 0000 7330  t_new_itema...s0
 00000de0: 0000 0000 0904 0104 040a 0112 0110 020a  ................
 00000df0: 0110 010a 010e 020a 0110 0110 0110 0310  ................
@@ -226,28 +226,28 @@
 00000e10: 010a 027a 1d41 7975 4d79 7371 6c50 6970  ...z.AyuMysqlPip
 00000e20: 656c 696e 652e 6765 745f 6e65 775f 6974  eline.get_new_it
 00000e30: 656d 6303 0000 0000 0000 0000 0000 0004  emc.............
 00000e40: 0000 0006 0000 0043 0000 0073 3800 0000  .......C...s8...
 00000e50: 7400 a001 7c01 a101 7d03 7c03 6401 1900  t...|...}.|.d...
 00000e60: 6402 6b02 7234 7c00 6a02 7c00 a003 7c03  d.k.r4|.j.|...|.
 00000e70: a101 7c00 a004 7c03 6403 1900 a101 6404  ..|...|.d.....d.
-00000e80: 8d02 0100 7c01 5300 2905 4e72 3d00 0000  ....|.S.).Nr=...
-00000e90: da05 4d79 7371 6c72 3500 0000 a902 da0a  ..Mysqlr5.......
-00000ea0: 616c 7465 725f 6974 656d 7235 0000 0029  alter_itemr5...)
+00000e80: 8d02 0100 7c01 5300 2905 4e72 3c00 0000  ....|.S.).Nr<...
+00000e90: da05 4d79 7371 6c72 3400 0000 a902 da0a  ..Mysqlr4.......
+00000ea0: 616c 7465 725f 6974 656d 7234 0000 0029  alter_itemr4...)
 00000eb0: 0572 0e00 0000 da15 636f 6e76 6572 745f  .r......convert_
 00000ec0: 6974 656d 735f 746f 5f64 6963 74da 0b69  items_to_dict..i
-00000ed0: 6e73 6572 745f 6974 656d 724f 0000 0072  nsert_itemrO...r
-00000ee0: 3900 0000 2904 7221 0000 0072 4a00 0000  9...).r!...rJ...
-00000ef0: 7233 0000 00da 0969 7465 6d5f 6469 6374  r3.....item_dict
+00000ed0: 6e73 6572 745f 6974 656d 724e 0000 0072  nsert_itemrN...r
+00000ee0: 3800 0000 2904 7221 0000 0072 4900 0000  8...).r!...rI...
+00000ef0: 7232 0000 00da 0969 7465 6d5f 6469 6374  r2.....item_dict
 00000f00: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
 00000f10: 0c70 726f 6365 7373 5f69 7465 6d8e 0000  .process_item...
 00000f20: 0073 0e00 0000 0001 0a02 0c01 0401 0801  .s..............
 00000f30: 0cfe 0604 7a1d 4179 754d 7973 716c 5069  ....z.AyuMysqlPi
 00000f40: 7065 6c69 6e65 2e70 726f 6365 7373 5f69  peline.process_i
-00000f50: 7465 6d72 5100 0000 6303 0000 0000 0000  temrQ...c.......
+00000f50: 7465 6d72 5000 0000 6303 0000 0000 0000  temrP...c.......
 00000f60: 0000 0000 0007 0000 0010 0000 0043 0000  .............C..
 00000f70: 0073 ec00 0000 7c01 6a00 0400 7d03 730e  .s....|.j...}.s.
 00000f80: 6401 5300 7c01 6a01 7d04 7c00 6a02 7c02  d.S.|.j.}.|.j.|.
 00000f90: 7c03 6402 8d02 7d05 7a28 7c00 6a03 a004  |.d...}.z(|.j...
 00000fa0: 7c05 7405 7c03 a006 a100 8301 6403 1400  |.t.|.......d...
 00000fb0: a102 7248 7c00 6a07 a008 a100 0100 5700  ..rH|.j.......W.
 00000fc0: 6e9c 0400 7409 6b0a 72e6 0100 7d06 0100  n...t.k.r...}...
@@ -273,64 +273,64 @@
 00001100: 2020 616c 7465 725f 6974 656d 3a20 e7bb    alter_item: ..
 00001110: 8fe8 bf87 e8bd ace5 8f98 e590 8ee7 9a84  ................
 00001120: 2069 7465 6d0a 2020 2020 2020 2020 2020   item.          
 00001130: 2020 7461 626c 653a 20e6 95b0 e68d aee5    table: .......
 00001140: ba93 e8a1 a8e5 908d 0a0a 2020 2020 2020  ..........      
 00001150: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
 00001160: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
-00001170: 2020 2020 4ea9 0272 3500 0000 724a 0000      N..r5...rJ..
+00001170: 2020 2020 4ea9 0272 3400 0000 7249 0000      N..r4...rI..
 00001180: 00e9 0200 0000 fa01 3a7a 0549 7465 6d3a  ........:z.Item:
 00001190: 7a09 2020 5461 626c 653a 2029 0ada 0765  z.  Table: )...e
 000011a0: 7272 5f6d 7367 721a 0000 0072 1c00 0000  rr_msgr....r....
 000011b0: da07 6368 6172 7365 7472 1800 0000 da08  ..charsetr......
-000011c0: 6461 7461 6261 7365 7235 0000 0072 1300  databaser5...r..
+000011c0: 6461 7461 6261 7365 7234 0000 0072 1300  databaser4...r..
 000011d0: 0000 7214 0000 00da 086e 6f74 655f 6469  ..r......note_di
-000011e0: 6329 1772 4000 0000 7241 0000 00da 105f  c).r@...rA....._
+000011e0: 6329 1772 3f00 0000 7240 0000 00da 105f  c).r?...r@....._
 000011f0: 6765 745f 7371 6c5f 6279 5f69 7465 6d72  get_sql_by_itemr
 00001200: 1c00 0000 da07 6578 6563 7574 65da 0574  ......execute..t
-00001210: 7570 6c65 7246 0000 0072 1a00 0000 da06  uplerF...r......
+00001210: 7570 6c65 7245 0000 0072 1a00 0000 da06  uplerE...r......
 00001220: 636f 6d6d 6974 da09 4578 6365 7074 696f  commit..Exceptio
 00001230: 6e72 1b00 0000 da07 7761 726e 696e 67da  nr......warning.
 00001240: 0872 6f6c 6c62 6163 6b72 0900 0000 7208  .rollbackr....r.
-00001250: 0000 0072 3800 0000 7219 0000 0072 5b00  ...r8...r....r[.
-00001260: 0000 7218 0000 0072 5c00 0000 7213 0000  ..r....r\...r...
-00001270: 0072 1400 0000 7254 0000 0029 0772 2100  .r....rT...).r!.
-00001280: 0000 7252 0000 0072 3500 0000 7240 0000  ..rR...r5...r@..
-00001290: 0072 5d00 0000 da03 7371 6cda 0165 7222  .r].....sql..er"
-000012a0: 0000 0072 2200 0000 7223 0000 0072 5400  ...r"...r#...rT.
+00001250: 0000 0072 3700 0000 7219 0000 0072 5a00  ...r7...r....rZ.
+00001260: 0000 7218 0000 0072 5b00 0000 7213 0000  ..r....r[...r...
+00001270: 0072 1400 0000 7253 0000 0029 0772 2100  .r....rS...).r!.
+00001280: 0000 7251 0000 0072 3400 0000 723f 0000  ..rQ...r4...r?..
+00001290: 0072 5c00 0000 da03 7371 6cda 0165 7222  .r\.....sql..er"
+000012a0: 0000 0072 2200 0000 7223 0000 0072 5300  ...r"...r#...rS.
 000012b0: 0000 9800 0000 7332 0000 0000 0a0a 0104  ......s2........
 000012c0: 0206 010e 0202 011a 010e 0210 0112 0118  ................
 000012d0: 010a 0102 0104 0106 0104 0104 0106 0104  ................
 000012e0: 0106 0102 0104 0104 0102 f506 0d7a 1c41  .............z.A
 000012f0: 7975 4d79 7371 6c50 6970 656c 696e 652e  yuMysqlPipeline.
 00001300: 696e 7365 7274 5f69 7465 6d63 0200 0000  insert_itemc....
 00001310: 0000 0000 0000 0000 0300 0000 0500 0000  ................
 00001320: 4300 0000 734c 0000 007c 006a 0072 387c  C...sL...|.j.r8|
 00001330: 006a 017c 017c 006a 0264 018d 027d 027c  .j.|.|.j.d...}.|
 00001340: 00a0 037c 02a1 0101 007c 006a 047c 016a  ...|.....|.j.|.j
 00001350: 057c 016a 066a 077c 006a 0264 028d 0301  .|.j.j.|.j.d....
 00001360: 007c 006a 0872 487c 006a 08a0 09a1 0001  .|.j.rH|.j......
-00001370: 0064 0053 0029 034e 2902 7233 0000 0072  .d.S.).N).r3...r
+00001370: 0064 0053 0029 034e 2902 7232 0000 0072  .d.S.).N).r2...r
 00001380: 2000 0000 a903 da0b 7370 6964 6572 5f6e   .......spider_n
-00001390: 616d 6572 5c00 0000 7220 0000 0029 0a72  amer\...r ...).r
-000013a0: 1600 0000 da12 5f67 6574 5f6c 6f67 5f62  ......_get_log_b
+00001390: 616d 6572 5b00 0000 7220 0000 0029 0a72  amer[...r ...).r
+000013a0: 1600 0000 5a12 5f67 6574 5f6c 6f67 5f62  ....Z._get_log_b
 000013b0: 795f 7370 6964 6572 7220 0000 00da 1869  y_spiderr .....i
 000013c0: 6e73 6572 745f 7363 7269 7074 5f73 7461  nsert_script_sta
 000013d0: 7469 7374 6963 73da 1b74 6162 6c65 5f63  tistics..table_c
 000013e0: 6f6c 6c65 6374 696f 6e5f 7374 6174 6973  ollection_statis
 000013f0: 7469 6373 da04 6e61 6d65 7219 0000 0072  tics..namer....r
-00001400: 5c00 0000 721a 0000 00da 0563 6c6f 7365  \...r......close
-00001410: 2903 7221 0000 0072 3300 0000 da08 6c6f  ).r!...r3.....lo
+00001400: 5b00 0000 721a 0000 00da 0563 6c6f 7365  [...r......close
+00001410: 2903 7221 0000 0072 3200 0000 5a08 6c6f  ).r!...r2...Z.lo
 00001420: 675f 696e 666f 7222 0000 0072 2200 0000  g_infor"...r"...
 00001430: 7223 0000 00da 0c63 6c6f 7365 5f73 7069  r#.....close_spi
 00001440: 6465 72bf 0000 0073 1a00 0000 0002 0601  der....s........
 00001450: 0401 0200 04ff 0605 0a01 0401 0401 0601  ................
 00001460: 04fd 0606 0601 7a1d 4179 754d 7973 716c  ......z.AyuMysql
 00001470: 5069 7065 6c69 6e65 2e63 6c6f 7365 5f73  Pipeline.close_s
-00001480: 7069 6465 7272 6700 0000 6304 0000 0000  piderrg...c.....
+00001480: 7069 6465 7272 6600 0000 6304 0000 0000  piderrf...c.....
 00001490: 0000 0000 0000 000a 0000 0008 0000 0043  ...............C
 000014a0: 0000 0073 9600 0000 6401 7c03 9b00 6402  ...s....d.|...d.
 000014b0: 7c02 9b00 6403 9d05 7d04 7c00 6a00 a001  |...d...}.|.j...
 000014c0: 7c04 a101 0100 7c00 6a00 a002 a100 7d05  |.....|.j.....}.
 000014d0: 6404 6405 8400 7c05 4400 8301 0400 7d06  d.d...|.D.....}.
 000014e0: 7292 6406 a003 7c06 a101 7d07 7c00 6a00  r.d...|...}.|.j.
 000014f0: a001 7c07 a101 0100 7c00 6a00 a002 a100  ..|.....|.j.....
@@ -391,34 +391,34 @@
 00001860: 3c6c 6973 7463 6f6d 703e e700 0000 7304  <listcomp>....s.
 00001870: 0000 0006 0002 007a 4041 7975 4d79 7371  .......z@AyuMysq
 00001880: 6c50 6970 656c 696e 652e 7461 626c 655f  lPipeline.table_
 00001890: 636f 6c6c 6563 7469 6f6e 5f73 7461 7469  collection_stati
 000018a0: 7374 6963 732e 3c6c 6f63 616c 733e 2e3c  stics.<locals>.<
 000018b0: 6c69 7374 636f 6d70 3e7a 0b20 756e 696f  listcomp>z. unio
 000018c0: 6e20 616c 6c20 7201 0000 00e9 0100 0000  n all r.........
-000018d0: 7258 0000 0029 0572 6800 0000 725c 0000  rX...).rh...r\..
+000018d0: 7257 0000 0029 0572 6700 0000 725b 0000  rW...).rg...r[..
 000018e0: 00da 0a74 6162 6c65 5f6e 616d 65da 066e  ...table_name..n
 000018f0: 756d 6265 7272 2000 0000 4e29 0672 1c00  umberr ...N).r..
-00001900: 0000 725f 0000 00da 0866 6574 6368 616c  ..r_.....fetchal
-00001910: 6cda 046a 6f69 6e72 3800 0000 da17 696e  l..joinr8.....in
+00001900: 0000 725e 0000 00da 0866 6574 6368 616c  ..r^.....fetchal
+00001910: 6cda 046a 6f69 6e72 3700 0000 da17 696e  l..joinr7.....in
 00001920: 7365 7274 5f74 6162 6c65 5f73 7461 7469  sert_table_stati
-00001930: 7374 6963 7329 0a72 2100 0000 7268 0000  stics).r!...rh..
-00001940: 0072 5c00 0000 7220 0000 0072 6500 0000  .r\...r ...re...
+00001930: 7374 6963 7329 0a72 2100 0000 7267 0000  stics).r!...rg..
+00001940: 0072 5b00 0000 7220 0000 0072 6400 0000  .r[...r ...rd...
 00001950: da07 7265 7375 6c74 735a 0873 716c 5f6c  ..resultsZ.sql_l
-00001960: 6973 745a 0773 716c 5f61 6c6c 7271 0000  istZ.sql_allrq..
+00001960: 6973 745a 0773 716c 5f61 6c6c 726e 0000  istZ.sql_allrn..
 00001970: 005a 1074 6162 6c65 5f73 7461 7469 7374  .Z.table_statist
 00001980: 6963 7372 2200 0000 7222 0000 0072 2300  icsr"...r"...r#.
-00001990: 0000 726b 0000 00d1 0000 0073 2600 0000  ..rk.......s&...
+00001990: 0000 7269 0000 00d1 0000 0073 2600 0000  ..ri.......s&...
 000019a0: 000d 0203 02fd 0404 02fc 0807 0c01 0a01  ................
 000019b0: 1201 0a01 0c01 0a02 0802 0201 0201 0601  ................
 000019c0: 0601 0efb 0607 7a2c 4179 754d 7973 716c  ......z,AyuMysql
 000019d0: 5069 7065 6c69 6e65 2e74 6162 6c65 5f63  Pipeline.table_c
 000019e0: 6f6c 6c65 6374 696f 6e5f 7374 6174 6973  ollection_statis
-000019f0: 7469 6373 726b 0000 0029 02da 0464 6174  ticsrk...)...dat
-00001a00: 6172 3500 0000 6303 0000 0000 0000 0000  ar5...c.........
+000019f0: 7469 6373 7269 0000 0029 02da 0464 6174  ticsri...)...dat
+00001a00: 6172 3400 0000 6303 0000 0000 0000 0000  ar4...c.........
 00001a10: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
 00001a20: 4400 0000 6401 7c02 9b00 6402 9d03 7d03  D...d.|...d...}.
 00001a30: 7c00 6a00 a001 7c03 a101 0100 7c00 6a02  |.j...|.....|.j.
 00001a40: 7c02 7c01 6403 8d02 7d04 7c00 6a03 7c04  |.|.d...}.|.j.|.
 00001a50: 7404 7c01 a005 a100 8301 6404 1400 6405  t.|.......d...d.
 00001a60: 8d02 0100 6406 5300 2907 75b2 0000 000a  ....d.S.).u.....
 00001a70: 2020 2020 2020 2020 e68f 92e5 85a5 e7bb          ........
@@ -477,23 +477,23 @@
 00001dc0: 2020 2020 2020 2020 2920 454e 4749 4e45          ) ENGINE
 00001dd0: 3d49 6e6e 6f44 4220 4445 4641 554c 5420  =InnoDB DEFAULT 
 00001de0: 4348 4152 5345 543d 7574 6638 6d62 3420  CHARSET=utf8mb4 
 00001df0: 524f 575f 464f 524d 4154 3d44 594e 414d  ROW_FORMAT=DYNAM
 00001e00: 4943 2043 4f4d 4d45 4e54 3d27 e9a1 b9e7  IC COMMENT='....
 00001e10: 9bae e5af b9e5 ba94 e5ba 93e4 b8ad e590  ................
 00001e20: 84e8 a1a8 e987 87e9 9b86 e7bb 9fe8 aea1  ................
-00001e30: e8a1 a827 3b0a 2020 2020 2020 2020 7257  ...';.        rW
-00001e40: 0000 0072 5800 0000 a902 7265 0000 0072  ...rX.....re...r
-00001e50: 7a00 0000 4ea9 0672 1c00 0000 725f 0000  z...N..r....r_..
-00001e60: 0072 5e00 0000 da0b 5f6c 6f67 5f72 6563  .r^....._log_rec
-00001e70: 6f72 6472 6000 0000 7246 0000 0029 0572  ordr`...rF...).r
-00001e80: 2100 0000 727a 0000 0072 3500 0000 5a10  !...rz...r5...Z.
+00001e30: e8a1 a827 3b0a 2020 2020 2020 2020 7256  ...';.        rV
+00001e40: 0000 0072 5700 0000 a902 7264 0000 0072  ...rW.....rd...r
+00001e50: 7700 0000 4ea9 0672 1c00 0000 725e 0000  w...N..r....r^..
+00001e60: 0072 5d00 0000 da0b 5f6c 6f67 5f72 6563  .r]....._log_rec
+00001e70: 6f72 6472 5f00 0000 7245 0000 0029 0572  ordr_...rE...).r
+00001e80: 2100 0000 7277 0000 0072 3400 0000 5a10  !...rw...r4...Z.
 00001e90: 6372 6561 7465 5f74 6162 6c65 5f73 716c  create_table_sql
-00001ea0: 7265 0000 0072 2200 0000 7222 0000 0072  re...r"...r"...r
-00001eb0: 2300 0000 7278 0000 00f6 0000 0073 0c00  #...rx.......s..
+00001ea0: 7264 0000 0072 2200 0000 7222 0000 0072  rd...r"...r"...r
+00001eb0: 2300 0000 7275 0000 00f6 0000 0073 0c00  #...ru.......s..
 00001ec0: 0000 000c 0201 02ff 080b 0c02 0e01 7a28  ..............z(
 00001ed0: 4179 754d 7973 716c 5069 7065 6c69 6e65  AyuMysqlPipeline
 00001ee0: 2e69 6e73 6572 745f 7461 626c 655f 7374  .insert_table_st
 00001ef0: 6174 6973 7469 6373 2903 da17 7374 6f70  atistics)...stop
 00001f00: 5f6d 6178 5f61 7474 656d 7074 5f6e 756d  _max_attempt_num
 00001f10: 6265 72da 0f77 6169 745f 7261 6e64 6f6d  ber..wait_random
 00001f20: 5f6d 696e da0f 7761 6974 5f72 616e 646f  _min..wait_rando
@@ -609,23 +609,23 @@
 00002600: 454e 4749 4e45 3d49 6e6e 6f44 4220 4445  ENGINE=InnoDB DE
 00002610: 4641 554c 5420 4348 4152 5345 543d 7574  FAULT CHARSET=ut
 00002620: 6638 6d62 3420 524f 575f 464f 524d 4154  f8mb4 ROW_FORMAT
 00002630: 3d44 594e 414d 4943 2043 4f4d 4d45 4e54  =DYNAMIC COMMENT
 00002640: 3d27 e9a1 b9e7 9bae e8bf 90e8 a18c e884  ='..............
 00002650: 9ae6 9cac e7bb 9fe8 aea1 e4bf a1e6 81af  ................
 00002660: e8a1 a827 3b0a 2020 2020 2020 2020 2020  ...';.          
-00002670: 2020 7257 0000 0072 5800 0000 727b 0000    rW...rX...r{..
-00002680: 004e 727c 0000 0029 0472 2100 0000 727a  .Nr|...).r!...rz
-00002690: 0000 0072 3500 0000 7265 0000 0072 2200  ...r5...re...r".
-000026a0: 0000 7222 0000 0072 2300 0000 726a 0000  ..r"...r#...rj..
+00002670: 2020 7256 0000 0072 5700 0000 7278 0000    rV...rW...rx..
+00002680: 004e 7279 0000 0029 0472 2100 0000 7277  .Nry...).r!...rw
+00002690: 0000 0072 3400 0000 7264 0000 0072 2200  ...r4...rd...r".
+000026a0: 0000 7222 0000 0072 2300 0000 7268 0000  ..r"...r#...rh..
 000026b0: 0012 0100 0073 0e00 0000 0011 0601 0201  .....s..........
 000026c0: 02ff 06ff 0417 0e01 7a29 4179 754d 7973  ........z)AyuMys
 000026d0: 716c 5069 7065 6c69 6e65 2e69 6e73 6572  qlPipeline.inser
 000026e0: 745f 7363 7269 7074 5f73 7461 7469 7374  t_script_statist
-000026f0: 6963 7329 0372 6500 0000 727a 0000 0072  ics).re...rz...r
+000026f0: 6963 7329 0372 6400 0000 7277 0000 0072  ics).rd...rw...r
 00002700: 1700 0000 6303 0000 0000 0000 0000 0000  ....c...........
 00002710: 0004 0000 000a 0000 0043 0000 0073 6000  .........C...s`.
 00002720: 0000 7a1c 7c00 6a00 a001 7c01 7c02 a102  ..z.|.j...|.|...
 00002730: 721a 7c00 6a02 a003 a100 0100 5700 6e3e  r.|.j.......W.n>
 00002740: 0400 7404 6b0a 725a 0100 7d03 0100 7a20  ..t.k.rZ..}...z 
 00002750: 7c00 6a02 a005 a100 0100 7c00 6a06 a007  |.j.......|.j...
 00002760: 6401 7c03 9b00 9d02 a101 0100 5700 3500  d.|.........W.5.
@@ -637,65 +637,65 @@
 000027c0: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
 000027d0: 3a20 7371 6c20 e8af ade5 8fa5 0a20 2020  : sql .......   
 000027e0: 2020 2020 2020 2020 2064 6174 613a 2073           data: s
 000027f0: 716c 20e8 afad e58f a5e4 b8ad e79a 84e5  ql .............
 00002800: 8f82 e695 b00a 0a20 2020 2020 2020 2052  .......        R
 00002810: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
 00002820: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00002830: 2072 5900 0000 4e29 0872 1c00 0000 725f   rY...N).r....r_
-00002840: 0000 0072 1a00 0000 7261 0000 0072 6200  ...r....ra...rb.
-00002850: 0000 7264 0000 0072 1b00 0000 7263 0000  ..rd...r....rc..
-00002860: 0029 0472 2100 0000 7265 0000 0072 7a00  .).r!...re...rz.
-00002870: 0000 7266 0000 0072 2200 0000 7222 0000  ..rf...r"...r"..
-00002880: 0072 2300 0000 727d 0000 003d 0100 0073  .r#...r}...=...s
+00002830: 2072 5800 0000 4e29 0872 1c00 0000 725e   rX...N).r....r^
+00002840: 0000 0072 1a00 0000 7260 0000 0072 6100  ...r....r`...ra.
+00002850: 0000 7263 0000 0072 1b00 0000 7262 0000  ..rc...r....rb..
+00002860: 0029 0472 2100 0000 7264 0000 0072 7700  .).r!...rd...rw.
+00002870: 0000 7265 0000 0072 2200 0000 7222 0000  ..re...r"...r"..
+00002880: 0072 2300 0000 727a 0000 003d 0100 0073  .r#...rz...=...s
 00002890: 0c00 0000 000a 0201 0e01 0e01 1001 0a01  ................
 000028a0: 7a1c 4179 754d 7973 716c 5069 7065 6c69  z.AyuMysqlPipeli
 000028b0: 6e65 2e5f 6c6f 675f 7265 636f 7264 2901  ne._log_record).
-000028c0: 4629 0172 6b00 0000 2901 7281 0000 0029  F).rk...).r....)
+000028c0: 4629 0172 6900 0000 2901 727e 0000 0029  F).ri...).r~...)
 000028d0: 20da 085f 5f6e 616d 655f 5fda 0a5f 5f6d   ..__name__..__m
 000028e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000028f0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7238  ame__..__doc__r8
+000028f0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7237  ame__..__doc__r7
 00002900: 0000 0072 0400 0000 720d 0000 0072 0200  ...r....r....r..
 00002910: 0000 da04 626f 6f6c 7224 0000 00da 0b63  ....boolr$.....c
-00002920: 6c61 7373 6d65 7468 6f64 722e 0000 0072  lassmethodr....r
-00002930: 3400 0000 7239 0000 0072 0b00 0000 724f  4...r9...r....rO
-00002940: 0000 0072 5600 0000 7254 0000 0072 6f00  ...rV...rT...ro.
-00002950: 0000 721d 0000 0072 1e00 0000 726b 0000  ..r....r....rk..
-00002960: 0072 4300 0000 7278 0000 0072 0500 0000  .rC...rx...r....
+00002920: 6c61 7373 6d65 7468 6f64 722d 0000 0072  lassmethodr-...r
+00002930: 3300 0000 7238 0000 0072 0b00 0000 724e  3...r8...r....rN
+00002940: 0000 0072 5500 0000 7253 0000 0072 6c00  ...rU...rS...rl.
+00002950: 0000 721d 0000 0072 1e00 0000 7269 0000  ..r....r....ri..
+00002960: 0072 4200 0000 7275 0000 0072 0500 0000  .rB...ru...r....
 00002970: 720a 0000 00da 0972 6574 7279 5f6e 756d  r......retry_num
 00002980: da0e 7265 7472 795f 7469 6d65 5f6d 696e  ..retry_time_min
 00002990: da0e 7265 7472 795f 7469 6d65 5f6d 6178  ..retry_time_max
-000029a0: 726a 0000 0072 0300 0000 727d 0000 0072  rj...r....r}...r
+000029a0: 7268 0000 0072 0300 0000 727a 0000 0072  rh...r....rz...r
 000029b0: 2200 0000 7222 0000 0072 2200 0000 7223  "...r"...r"...r#
 000029c0: 0000 0072 1200 0000 1900 0000 734a 0000  ...r........sJ..
 000029d0: 0008 0104 0900 fb02 0202 0106 0102 0106  ................
 000029e0: 0102 fa0c 1b02 010a 0c08 0910 120e 2d08  ..............-.
 000029f0: 0a10 2708 1302 0002 0004 ff0c 2600 ff02  ..'.........&...
 00002a00: 0102 0002 ff0c 1c02 0104 0104 0104 fd04  ................
 00002a10: 0600 ff02 0102 0002 ff0e 2629 1c72 1d00  ..........&).r..
 00002a20: 0000 da08 7761 726e 696e 6773 da06 7479  ....warnings..ty
 00002a30: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
 00002a40: 0000 00da 0770 796d 7973 716c da08 7265  .....pymysql..re
-00002a50: 7472 7969 6e67 7205 0000 00da 1e61 7975  tryingr......ayu
+00002a50: 7472 7969 6e67 7205 0000 005a 1e61 7975  tryingr....Z.ayu
 00002a60: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00002a70: 6d6d 6f6e 2e45 7870 656e 6472 0600 0000  mmon.Expendr....
+00002a70: 6d6d 6f6e 2e65 7870 656e 6472 0600 0000  mmon.expendr....
 00002a80: da24 6179 7567 6573 7069 6465 7274 6f6f  .$ayugespidertoo
-00002a90: 6c73 2e63 6f6d 6d6f 6e2e 4d75 6c74 6950  ls.common.MultiP
-00002aa0: 6c65 7869 6e67 7207 0000 005a 2861 7975  lexingr....Z(ayu
+00002a90: 6c73 2e63 6f6d 6d6f 6e2e 6d75 6c74 6970  ls.common.multip
+00002aa0: 6c65 7869 6e67 7207 0000 005a 2661 7975  lexingr....Z&ayu
 00002ab0: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00002ac0: 6d6d 6f6e 2e4d 7973 716c 4572 726f 7248  mmon.MysqlErrorH
-00002ad0: 616e 646c 6572 0800 0000 7209 0000 00da  andler....r.....
-00002ae0: 1e61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
-00002af0: 732e 636f 6d6d 6f6e 2e50 6172 616d 7372  s.common.Paramsr
-00002b00: 0a00 0000 da20 6179 7567 6573 7069 6465  ..... ayugespide
-00002b10: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 5479  rtools.common.Ty
-00002b20: 7065 5661 7273 720b 0000 0072 0c00 0000  peVarsr....r....
-00002b30: 720d 0000 00da 1d61 7975 6765 7370 6964  r......ayugespid
-00002b40: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e55  ertools.common.U
-00002b50: 7469 6c73 720e 0000 00da 0e66 696c 7465  tilsr......filte
-00002b60: 7277 6172 6e69 6e67 73da 0757 6172 6e69  rwarnings..Warni
-00002b70: 6e67 da07 5f5f 616c 6c5f 5f72 1200 0000  ng..__all__r....
-00002b80: 7222 0000 0072 2200 0000 7222 0000 0072  r"...r"...r"...r
-00002b90: 2300 0000 da08 3c6d 6f64 756c 653e 0100  #.....<module>..
-00002ba0: 0000 7324 0000 0008 0108 0114 0208 010c  ..s$............
-00002bb0: 020c 010c 0110 010c 0114 010c 0304 0102  ................
-00002bc0: 0004 0002 ff06 0502 ff04 05              ...........
+00002ac0: 6d6d 6f6e 2e6d 7973 716c 6572 7268 616e  mmon.mysqlerrhan
+00002ad0: 646c 6572 0800 0000 7209 0000 00da 1e61  dler....r......a
+00002ae0: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
+00002af0: 636f 6d6d 6f6e 2e70 6172 616d 7372 0a00  common.paramsr..
+00002b00: 0000 da20 6179 7567 6573 7069 6465 7274  ... ayugespidert
+00002b10: 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7479 7065  ools.common.type
+00002b20: 7661 7273 720b 0000 0072 0c00 0000 720d  varsr....r....r.
+00002b30: 0000 00da 1d61 7975 6765 7370 6964 6572  .....ayugespider
+00002b40: 746f 6f6c 732e 636f 6d6d 6f6e 2e75 7469  tools.common.uti
+00002b50: 6c73 720e 0000 00da 0e66 696c 7465 7277  lsr......filterw
+00002b60: 6172 6e69 6e67 73da 0757 6172 6e69 6e67  arnings..Warning
+00002b70: da07 5f5f 616c 6c5f 5f72 1200 0000 7222  ..__all__r....r"
+00002b80: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00002b90: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002ba0: 7324 0000 0008 0108 0114 0208 010c 020c  s$..............
+00002bb0: 010c 0110 010c 0114 010c 0304 0102 0004  ................
+00002bc0: 0002 ff06 0502 ff04 05                   .........
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 06:45:18 2023 UTC, .py size: 2824 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7e3c 3e64 080b 0000  U.......~<>d....
+00000000: 550d 0d0a 0000 0000 7c42 4764 080b 0000  U.......|BGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6405 6701 5a09  d.l.m.Z...d.g.Z.
 00000070: 4700 6406 6405 8400 6405 6508 8303 5a0a  G.d.d...d.e...Z.
@@ -171,18 +171,18 @@
 00000aa0: 2100 0000 7242 0000 0072 4a00 0000 da0d  !...rB...rJ.....
 00000ab0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1100  __classcell__r..
 00000ac0: 0000 7211 0000 0072 3f00 0000 7212 0000  ..r....r?...r...
 00000ad0: 0072 0500 0000 0d00 0000 730c 0000 0008  .r........s.....
 00000ae0: 0108 0808 0d08 070c 1108 0329 0b72 1f00  ...........).r..
 00000af0: 0000 7245 0000 0072 1a00 0000 da24 6179  ..rE...r.....$ay
 00000b00: 7567 6573 7069 6465 7274 6f6f 6c73 2e63  ugespidertools.c
-00000b10: 6f6d 6d6f 6e2e 4d75 6c74 6950 6c65 7869  ommon.MultiPlexi
+00000b10: 6f6d 6d6f 6e2e 6d75 6c74 6970 6c65 7869  ommon.multiplexi
 00000b20: 6e67 7202 0000 00da 1d61 7975 6765 7370  ngr......ayugesp
 00000b30: 6964 6572 746f 6f6c 732e 636f 6d6d 6f6e  idertools.common
-00000b40: 2e55 7469 6c73 7203 0000 00da 2861 7975  .Utilsr.....(ayu
+00000b40: 2e75 7469 6c73 7203 0000 00da 2861 7975  .utilsr.....(ayu
 00000b50: 6765 7370 6964 6572 746f 6f6c 732e 7363  gespidertools.sc
 00000b60: 7261 7065 722e 7069 7065 6c69 6e65 732e  raper.pipelines.
 00000b70: 6d79 7371 6c72 0400 0000 da07 5f5f 616c  mysqlr......__al
 00000b80: 6c5f 5f72 0500 0000 7211 0000 0072 1100  l__r....r....r..
 00000b90: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
 00000ba0: 6f64 756c 653e 0100 0000 730e 0000 0008  odule>....s.....
 00000bb0: 0108 0208 020c 010c 010c 0206 03         .............
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr  6 08:21:44 2023 UTC, .py size: 2840 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1881 2e64 180b 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 8b42 4764 180b 0000  U........BGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6701 5a07  d.l.m.Z...d.g.Z.
 00000060: 4700 6406 6405 8400 6405 6506 8303 5a08  G.d.d...d.e...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
@@ -111,15 +111,15 @@
 000006e0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
 000006f0: 0e00 0000 720e 0000 0072 0c00 0000 720f  ....r....r....r.
 00000700: 0000 0072 0500 0000 0c00 0000 730a 0000  ...r........s...
 00000710: 0008 0104 040c 0402 010a 0f29 0972 2e00  ...........).r..
 00000720: 0000 5a11 6462 7574 696c 732e 706f 6f6c  ..Z.dbutils.pool
 00000730: 6564 5f64 6272 0200 0000 da1d 6179 7567  ed_dbr......ayug
 00000740: 6573 7069 6465 7274 6f6f 6c73 2e63 6f6d  espidertools.com
-00000750: 6d6f 6e2e 5574 696c 7372 0300 0000 da28  mon.Utilsr.....(
+00000750: 6d6f 6e2e 7574 696c 7372 0300 0000 da28  mon.utilsr.....(
 00000760: 6179 7567 6573 7069 6465 7274 6f6f 6c73  ayugespidertools
 00000770: 2e73 6372 6170 6572 2e70 6970 656c 696e  .scraper.pipelin
 00000780: 6573 2e6d 7973 716c 7204 0000 00da 075f  es.mysqlr......_
 00000790: 5f61 6c6c 5f5f 7205 0000 0072 0e00 0000  _all__r....r....
 000007a0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
 000007b0: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
 000007c0: 0000 0801 0c02 0c01 0c03 02ff 0405       ..............
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 06:44:38 2023 UTC, .py size: 3897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 563c 3e64 390f 0000  U.......V<>d9...
+00000000: 550d 0d0a 0000 0000 bc42 4764 d20e 0000  U........BGd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6701 5a0b 4700 6407 6406 8400 6406 650a  g.Z.G.d.d...d.e.
@@ -207,21 +207,21 @@
 00000ce0: 0000 0072 3500 0000 7236 0000 0072 4f00  ...r5...r6...rO.
 00000cf0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
 00000d00: 5f72 1200 0000 7212 0000 0072 1000 0000  _r....r....r....
 00000d10: 7213 0000 0072 0800 0000 0d00 0000 7312  r....r........s.
 00000d20: 0000 0008 0104 060c 0408 1a08 0308 0308  ................
 00000d30: 080c 2008 034e 290d 721c 0000 0072 0200  .. ..N).r....r..
 00000d40: 0000 5a12 7477 6973 7465 642e 656e 7465  ..Z.twisted.ente
-00000d50: 7270 7269 7365 7203 0000 00da 2861 7975  rpriser.....(ayu
+00000d50: 7270 7269 7365 7203 0000 00da 2661 7975  rpriser.....&ayu
 00000d60: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00000d70: 6d6d 6f6e 2e4d 7973 716c 4572 726f 7248  mmon.MysqlErrorH
-00000d80: 616e 646c 6572 0400 0000 7205 0000 00da  andler....r.....
-00000d90: 1d61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
-00000da0: 732e 636f 6d6d 6f6e 2e55 7469 6c73 7206  s.common.Utilsr.
-00000db0: 0000 00da 2861 7975 6765 7370 6964 6572  ....(ayugespider
-00000dc0: 746f 6f6c 732e 7363 7261 7065 722e 7069  tools.scraper.pi
-00000dd0: 7065 6c69 6e65 732e 6d79 7371 6c72 0700  pelines.mysqlr..
-00000de0: 0000 da07 5f5f 616c 6c5f 5f72 0800 0000  ....__all__r....
-00000df0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000e00: 1300 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000e10: 0000 730e 0000 000c 010c 0210 010c 010c  ..s.............
-00000e20: 0302 ff04 05                             .....
+00000d70: 6d6d 6f6e 2e6d 7973 716c 6572 7268 616e  mmon.mysqlerrhan
+00000d80: 646c 6572 0400 0000 7205 0000 00da 1d61  dler....r......a
+00000d90: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
+00000da0: 636f 6d6d 6f6e 2e75 7469 6c73 7206 0000  common.utilsr...
+00000db0: 00da 2861 7975 6765 7370 6964 6572 746f  ..(ayugespiderto
+00000dc0: 6f6c 732e 7363 7261 7065 722e 7069 7065  ols.scraper.pipe
+00000dd0: 6c69 6e65 732e 6d79 7371 6c72 0700 0000  lines.mysqlr....
+00000de0: da07 5f5f 616c 6c5f 5f72 0800 0000 7212  ..__all__r....r.
+00000df0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000e00: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000e10: 730e 0000 000c 010c 0210 010c 010c 0302  s...............
+00000e20: ff04 05                                  ...
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import contextlib
 
 import aiomysql
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
 __all__ = ["AsyncMysqlPipeline"]
 
 
 class AsyncMysqlPipeline(AyuMysqlPipeline):
     def open_spider(self, spider):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 import datetime
 
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines import AyuMysqlPipeline
 
 __all__ = [
     "AyuStatisticsMysqlPipeline",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pymysql
 from dbutils.pooled_db import PooledDB
 
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
 __all__ = [
     "AyuTurboMysqlPipeline",
 ]
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from pymysql import cursors
-from twisted.enterprise import adbapi
-
-from ayugespidertools.common.MysqlErrorHandle import TwistedAsynchronous, deal_mysql_err
-from ayugespidertools.common.Utils import ToolsForAyu
-from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
-
-__all__ = [
-    "AyuTwistedMysqlPipeline",
-]
-
-
-class AyuTwistedMysqlPipeline(AyuMysqlPipeline):
-    """
-    使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
-    注意：
-        1. 推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
-    """
-
-    def __init__(self, *args, **kwargs):
-        super(AyuTwistedMysqlPipeline, self).__init__(*args, **kwargs)
-        self.dbpool = None
-
-    def open_spider(self, spider):
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
-
-        # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。
-        # 记录日志时需要此连接对象，否则直接关闭
-        if self.record_log_to_mysql:
-            self.conn = self._connect(self.mysql_conf)
-            self.cursor = self.conn.cursor()
-        else:
-            self._connect(self.mysql_conf).close()
-
-        _mysql_conf = {
-            "user": spider.mysql_conf.user,
-            "password": spider.mysql_conf.password,
-            "host": spider.mysql_conf.host,
-            "port": spider.mysql_conf.port,
-            "db": spider.mysql_conf.database,
-            "charset": spider.mysql_conf.charset,
-            "cursorclass": cursors.DictCursor,
-        }
-        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
-        query = self.dbpool.runInteraction(self.db_create)
-        query.addErrback(self.db_create_err)
-
-    def db_create(self, cursor):
-        pass
-
-    def db_create_err(self, failure):
-        self.slog.error(f"创建数据表失败: {failure}")
-
-    def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "Mysql":
-            query = self.dbpool.runInteraction(self.db_insert, item_dict)
-            query.addErrback(self.handle_error, item)
-        return item
-
-    def db_insert(self, cursor, item):
-        alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
-        table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["table"])
-
-        if not (new_item := alter_item.new_item):
-            return
-
-        note_dic = alter_item.notes_dic
-        sql = self._get_sql_by_item(table=table, item=new_item)
-
-        try:
-            cursor.execute(sql, tuple(new_item.values()) * 2)
-
-        except Exception as e:
-            self.slog.warning(f":{e}")
-            self.slog.warning(f"Item:{new_item}  Table: {table}")
-            deal_mysql_err(
-                TwistedAsynchronous(),
-                err_msg=str(e),
-                cursor=cursor,
-                charset=self.mysql_conf.charset,
-                collate=self.collate,
-                database=self.mysql_conf.database,
-                table=table,
-                table_prefix=self.table_prefix,
-                table_enum=self.table_enum,
-                note_dic=note_dic,
-            )
-            return self.db_insert(cursor, item)
-
-        return item
-
-    def handle_error(self, failure, item):
-        self.slog.error(f"插入数据失败:{failure}, item: {item}")
-
-    def close_spider(self, spider):
-        # 这里新建数据库链接，是为了正常继承父类的脚本运行统计的方法（需要 self 的 mysql 连接对象存在）
-        super(AyuTwistedMysqlPipeline, self).close_spider(spider)
+from pymysql import cursors
+from twisted.enterprise import adbapi
+
+from ayugespidertools.common.mysqlerrhandle import TwistedAsynchronous, deal_mysql_err
+from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
+
+__all__ = [
+    "AyuTwistedMysqlPipeline",
+]
+
+
+class AyuTwistedMysqlPipeline(AyuMysqlPipeline):
+    """
+    使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
+    注意：
+        1. 推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
+    """
+
+    def __init__(self, *args, **kwargs):
+        super(AyuTwistedMysqlPipeline, self).__init__(*args, **kwargs)
+        self.dbpool = None
+
+    def open_spider(self, spider):
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
+
+        # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。
+        # 记录日志时需要此连接对象，否则直接关闭
+        if self.record_log_to_mysql:
+            self.conn = self._connect(self.mysql_conf)
+            self.cursor = self.conn.cursor()
+        else:
+            self._connect(self.mysql_conf).close()
+
+        _mysql_conf = {
+            "user": spider.mysql_conf.user,
+            "password": spider.mysql_conf.password,
+            "host": spider.mysql_conf.host,
+            "port": spider.mysql_conf.port,
+            "db": spider.mysql_conf.database,
+            "charset": spider.mysql_conf.charset,
+            "cursorclass": cursors.DictCursor,
+        }
+        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
+        query = self.dbpool.runInteraction(self.db_create)
+        query.addErrback(self.db_create_err)
+
+    def db_create(self, cursor):
+        pass
+
+    def db_create_err(self, failure):
+        self.slog.error(f"创建数据表失败: {failure}")
+
+    def process_item(self, item, spider):
+        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        # 先查看存储场景是否匹配
+        if item_dict["item_mode"] == "Mysql":
+            query = self.dbpool.runInteraction(self.db_insert, item_dict)
+            query.addErrback(self.handle_error, item)
+        return item
+
+    def db_insert(self, cursor, item):
+        alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
+        table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["table"])
+
+        if not (new_item := alter_item.new_item):
+            return
+
+        note_dic = alter_item.notes_dic
+        sql = self._get_sql_by_item(table=table, item=new_item)
+
+        try:
+            cursor.execute(sql, tuple(new_item.values()) * 2)
+
+        except Exception as e:
+            self.slog.warning(f":{e}")
+            self.slog.warning(f"Item:{new_item}  Table: {table}")
+            deal_mysql_err(
+                TwistedAsynchronous(),
+                err_msg=str(e),
+                cursor=cursor,
+                charset=self.mysql_conf.charset,
+                collate=self.collate,
+                database=self.mysql_conf.database,
+                table=table,
+                table_prefix=self.table_prefix,
+                table_enum=self.table_enum,
+                note_dic=note_dic,
+            )
+            return self.db_insert(cursor, item)
+
+        return item
+
+    def handle_error(self, failure, item):
+        self.slog.error(f"插入数据失败:{failure}, item: {item}")
+
+    def close_spider(self, spider):
+        # 这里新建数据库链接，是为了正常继承父类的脚本运行统计的方法（需要 self 的 mysql 连接对象存在）
+        super(AyuTwistedMysqlPipeline, self).close_spider(spider)
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 import time
 
 from scrapy.spiders import Spider
 from sqlalchemy import create_engine
 
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.SpiderDBConf import (
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.spiderdbconf import (
     MongoDBConfCreator,
     MysqlConfCreator,
     get_spider_db_conf,
 )
 from ayugespidertools.config import logger
 
 __all__ = [
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 13:17:20 2023 UTC, .py size: 6737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6098 3e64 511a 0000  U.......`.>dQ...
+00000000: 550d 0d0a 0000 0000 ce42 4764 511a 0000  U........BGdQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -87,44 +87,44 @@
 00000560: 890a 2020 2020 46e9 0300 0000 e9ff ffff  ..    F.........
 00000570: ffda 0364 6576 2905 da0e 524f 424f 5453  ...dev)...ROBOTS
 00000580: 5458 545f 4f42 4559 5a15 5445 4c4e 4554  TXT_OBEYZ.TELNET
 00000590: 434f 4e53 4f4c 455f 454e 4142 4c45 44da  CONSOLE_ENABLED.
 000005a0: 0b52 4554 5259 5f54 494d 4553 da0e 4445  .RETRY_TIMES..DE
 000005b0: 5054 485f 5052 494f 5249 5459 da03 454e  PTH_PRIORITY..EN
 000005c0: 56da 0544 4542 5547 e914 0000 00da 0474  V..DEBUG.......t
-000005d0: 6573 744e 2909 da09 4c4f 475f 4c45 5645  estN)...LOG_LEVE
+000005d0: 6573 744e 2909 5a09 4c4f 475f 4c45 5645  estN).Z.LOG_LEVE
 000005e0: 4c72 2200 0000 5a10 444f 574e 4c4f 4144  Lr"...Z.DOWNLOAD
 000005f0: 5f54 494d 454f 5554 7223 0000 005a 1052  _TIMEOUTr#...Z.R
 00000600: 4544 4952 4543 545f 454e 4142 4c45 4472  EDIRECT_ENABLEDr
 00000610: 2400 0000 7225 0000 00da 0944 4154 415f  $...r%.....DATA_
-00000620: 454e 554d da13 5245 434f 5244 5f4c 4f47  ENUM..RECORD_LOG
+00000620: 454e 554d 5a13 5245 434f 5244 5f4c 4f47  ENUMZ.RECORD_LOG
 00000630: 5f54 4f5f 4d59 5351 4cda 0545 5252 4f52  _TO_MYSQL..ERROR
 00000640: da04 7072 6f64 7a08 2559 2d25 6d2d 2564  ..prodz.%Y-%m-%d
 00000650: da06 636f 6d6d 6f6e da00 6302 0000 0000  ..common..c.....
 00000660: 0000 0000 0000 0003 0000 0003 0000 000b  ................
 00000670: 0000 0073 1800 0000 7400 7401 7c00 8302  ...s....t.t.|...
 00000680: 6a02 7c01 6601 7c02 8e01 0100 6401 5300  j.|.f.|.....d.S.
 00000690: 2902 753d 0000 000a 2020 2020 2020 2020  ).u=....        
 000006a0: e5ae 9ee7 8eb0 e689 80e7 bba7 e689 bfe7  ................
 000006b0: b1bb e79a 8420 6162 7374 7261 6374 20e6  ..... abstract .
 000006c0: 96b9 e6b3 9520 7061 7273 650a 2020 2020  ..... parse.    
 000006d0: 2020 2020 4e29 03da 0573 7570 6572 7209      N)...superr.
 000006e0: 0000 00da 0570 6172 7365 2903 720c 0000  .....parse).r...
 000006f0: 00da 0872 6573 706f 6e73 6572 1800 0000  ...responser....
 00000700: a901 da09 5f5f 636c 6173 735f 5f72 0e00  ....__class__r..
-00000710: 0000 720f 0000 0072 3100 0000 6400 0000  ..r....r1...d...
+00000710: 0000 720f 0000 0072 2f00 0000 6400 0000  ..r....r/...d...
 00000720: 7302 0000 0000 047a 0f41 7975 5370 6964  s......z.AyuSpid
 00000730: 6572 2e70 6172 7365 6301 0000 0000 0000  er.parsec.......
 00000740: 0000 0000 0003 0000 0003 0000 000f 0000  ................
 00000750: 0073 1c00 0000 7400 7401 7c00 8302 6a02  .s....t.t.|...j.
 00000760: 7c01 7c02 8e01 0100 6400 7c00 5f03 6400  |.|.....d.|._.d.
-00000770: 5300 2901 4e29 0472 3000 0000 7209 0000  S.).N).r0...r...
+00000770: 5300 2901 4e29 0472 2e00 0000 7209 0000  S.).N).r....r...
 00000780: 0072 1000 0000 da0c 6d79 7371 6c5f 656e  .r......mysql_en
 00000790: 6769 6e65 2903 720c 0000 0072 1700 0000  gine).r....r....
-000007a0: 7218 0000 0072 3300 0000 720e 0000 0072  r....r3...r....r
+000007a0: 7218 0000 0072 3100 0000 720e 0000 0072  r....r1...r....r
 000007b0: 0f00 0000 7210 0000 006a 0000 0073 0400  ....r....j...s..
 000007c0: 0000 0001 1201 7a12 4179 7553 7069 6465  ......z.AyuSpide
 000007d0: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
 000007e0: 0000 0000 0000 0003 0000 0004 0000 0003  ................
 000007f0: 0000 0073 4c00 0000 7c00 6a00 6a01 a002  ...sL...|.j.j...
 00000800: 6401 a101 7d01 7c00 6a00 6a01 a002 6402  d...}.|.j.j...d.
 00000810: 6403 a102 7d02 7403 7c02 7404 8302 7330  d...}.t.|.t...s0
@@ -159,39 +159,39 @@
 000009e0: 5552 555f 454e 4142 4c45 4454 7529 0000  URU_ENABLEDTu)..
 000009f0: 006c 6f67 7572 755f 656e 6162 6c65 6420  .loguru_enabled 
 00000a00: e58f 82e6 95b0 e6a0 bce5 bc8f e99c 80e8  ................
 00000a10: a681 e4b8 ba20 626f 6f6c 4e29 09da 0763  ..... boolN)...c
 00000a20: 7261 776c 6572 da08 7365 7474 696e 6773  rawler..settings
 00000a30: da03 6765 74da 0a69 7369 6e73 7461 6e63  ..get..isinstanc
 00000a40: 65da 0462 6f6f 6cda 0e41 7373 6572 7469  e..bool..Asserti
-00000a50: 6f6e 4572 726f 7272 0800 0000 7230 0000  onErrorr....r0..
+00000a50: 6f6e 4572 726f 7272 0800 0000 722e 0000  onErrorr....r...
 00000a60: 0072 0900 0000 2903 720c 0000 005a 0f6c  .r....).r....Z.l
 00000a70: 6f67 7572 755f 636f 6e66 5f74 6d70 5a0e  oguru_conf_tmpZ.
-00000a80: 6c6f 6775 7275 5f65 6e61 626c 6564 7233  loguru_enabledr3
+00000a80: 6c6f 6775 7275 5f65 6e61 626c 6564 7231  loguru_enabledr1
 00000a90: 0000 0072 0e00 0000 720f 0000 00da 0473  ...r....r......s
 00000aa0: 6c6f 676e 0000 0073 0c00 0000 000a 0e02  logn...s........
 00000ab0: 1001 1203 0402 0804 7a0e 4179 7553 7069  ........z.AyuSpi
 00000ac0: 6465 722e 736c 6f67 6302 0000 0000 0000  der.slogc.......
 00000ad0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
 00000ae0: 0073 5e00 0000 7400 7c00 6401 6400 8303  .s^...t.|.d.d...
 00000af0: 7d02 7400 7c00 6402 6403 8303 7d03 7400  }.t.|.d.d...}.t.
 00000b00: 7c00 6404 7c03 9b00 6405 9d03 6900 8303  |.d.|...d...i...
 00000b10: 7d04 7c02 7238 7c02 7c04 6406 3c00 7c01  }.|.r8|.|.d.<.|.
 00000b20: 6a01 7c04 6407 6408 8d02 0100 7c01 6a01  j.|.d.d.....|.j.
 00000b30: 7c00 6a02 7052 6900 6409 6408 8d02 0100  |.j.pRi.d.d.....
 00000b40: 6400 5300 290a 4eda 1163 7573 746f 6d5f  d.S.).N..custom_
 00000b50: 7461 626c 655f 656e 756d da0d 7365 7474  table_enum..sett
-00000b60: 696e 6773 5f74 7970 6572 2e00 0000 5a07  ings_typer....Z.
+00000b60: 696e 6773 5f74 7970 6572 2c00 0000 5a07  ings_typer,...Z.
 00000b70: 6375 7374 6f6d 5fda 095f 7365 7474 696e  custom_.._settin
-00000b80: 6773 722a 0000 00da 0770 726f 6a65 6374  gsr*.....project
+00000b80: 6773 7229 0000 005a 0770 726f 6a65 6374  gsr)...Z.project
 00000b90: 2901 da08 7072 696f 7269 7479 da06 7370  )...priority..sp
 00000ba0: 6964 6572 2903 da07 6765 7461 7474 72da  ider)...getattr.
 00000bb0: 0773 6574 6469 6374 da0f 6375 7374 6f6d  .setdict..custom
 00000bc0: 5f73 6574 7469 6e67 7329 0572 1600 0000  _settings).r....
-00000bd0: 7237 0000 0072 3d00 0000 723e 0000 005a  r7...r=...r>...Z
+00000bd0: 7235 0000 0072 3b00 0000 723c 0000 005a  r5...r;...r<...Z
 00000be0: 0e69 6e6e 6572 5f73 6574 7469 6e67 7372  .inner_settingsr
 00000bf0: 0e00 0000 720e 0000 0072 0f00 0000 da0f  ....r....r......
 00000c00: 7570 6461 7465 5f73 6574 7469 6e67 7386  update_settings.
 00000c10: 0000 0073 0e00 0000 0002 0c02 0c02 1402  ...s............
 00000c20: 0401 0804 0e01 7a19 4179 7553 7069 6465  ......z.AyuSpide
 00000c30: 722e 7570 6461 7465 5f73 6574 7469 6e67  r.update_setting
 00000c40: 7363 0200 0000 0000 0000 0000 0000 0900  sc..............
@@ -208,78 +208,78 @@
 00000cf0: 139b 0064 087c 066a 149b 0064 097c 066a  ...d.|.j...d.|.j
 00000d00: 159b 009d 0c7d 0774 167c 0764 0a8d 016a  .....}.t.|.d...j
 00000d10: 177c 045f 1874 0a74 1983 006a 0c7c 016a  .|._.t.t...j.|.j
 00000d20: 097c 0564 038d 0283 0104 007d 0872 e27c  .|.d.......}.r.|
 00000d30: 046a 04a0 0d64 0ba1 0101 007c 087c 045f  .j...d.....|.|._
 00000d40: 1a7c 0453 0029 0c4e 7516 0000 0073 6574  .|.S.).Nu....set
 00000d50: 7469 6e67 735f 7479 7065 20e9 858d e7bd  tings_type .....
-00000d60: ae3a 2029 0172 3700 0000 2902 7237 0000  .: ).r7...).r7..
+00000d60: ae3a 2029 0172 3500 0000 2902 7235 0000  .: ).r5...).r5..
 00000d70: 005a 0b63 6f6e 7375 6c5f 636f 6e66 7524  .Z.consul_confu$
 00000d80: 0000 00e9 a1b9 e79b aee4 b8ad e985 8de7  ................
 00000d90: bdae e4ba 8620 6d79 7371 6c5f 636f 6e66  ..... mysql_conf
 00000da0: 20e4 bfa1 e681 af7a 106d 7973 716c 2b70   ......z.mysql+p
 00000db0: 796d 7973 716c 3a2f 2ffa 013a fa01 40fa  ymysql://..:..@.
 00000dc0: 012f 7a09 3f63 6861 7273 6574 3d29 0172  ./z.?charset=).r
 00000dd0: 0d00 0000 7526 0000 00e9 a1b9 e79b aee4  ....u&..........
 00000de0: b8ad e985 8de7 bdae e4ba 8620 6d6f 6e67  ........... mong
 00000df0: 6f64 625f 636f 6e66 20e4 bfa1 e681 af29  odb_conf ......)
-00000e00: 1b72 3000 0000 7209 0000 00da 0c66 726f  .r0...r......fro
+00000e00: 1b72 2e00 0000 7209 0000 00da 0c66 726f  .r....r......fro
 00000e10: 6d5f 6372 6177 6c65 72da 0573 7461 7473  m_crawler..stats
-00000e20: 723c 0000 00da 0564 6562 7567 723e 0000  r<.....debugr>..
+00000e20: 723a 0000 00da 0564 6562 7567 723c 0000  r:.....debugr<..
 00000e30: 0072 0400 0000 5a0f 6765 745f 636f 6e73  .r....Z.get_cons
-00000e40: 756c 5f63 6f6e 6672 3700 0000 7207 0000  ul_confr7...r...
+00000e40: 756c 5f63 6f6e 6672 3500 0000 7207 0000  ul_confr5...r...
 00000e50: 0072 0600 0000 5a0e 6372 6561 7465 5f70  .r....Z.create_p
 00000e60: 726f 6475 6374 da04 696e 666f da0a 6d79  roduct..info..my
 00000e70: 7371 6c5f 636f 6e66 da14 6d79 7371 6c5f  sql_conf..mysql_
 00000e80: 656e 6769 6e65 5f65 6e61 626c 6564 da04  engine_enabled..
 00000e90: 7573 6572 da08 7061 7373 776f 7264 da04  user..password..
 00000ea0: 686f 7374 da04 706f 7274 da08 6461 7461  host..port..data
 00000eb0: 6261 7365 da07 6368 6172 7365 7472 0a00  base..charsetr..
-00000ec0: 0000 720b 0000 0072 3500 0000 7205 0000  ..r....r5...r...
+00000ec0: 0000 720b 0000 0072 3300 0000 7205 0000  ..r....r3...r...
 00000ed0: 00da 0c6d 6f6e 676f 6462 5f63 6f6e 6629  ...mongodb_conf)
-00000ee0: 0972 1600 0000 7236 0000 0072 1700 0000  .r....r6...r....
-00000ef0: 7218 0000 0072 4200 0000 5a0c 5f63 6f6e  r....rB...Z._con
-00000f00: 7375 6c5f 636f 6e66 724e 0000 005a 096d  sul_confrN...Z.m
-00000f10: 7973 716c 5f75 726c 7256 0000 0072 3300  ysql_urlrV...r3.
-00000f20: 0000 720e 0000 0072 0f00 0000 724a 0000  ..r....r....rJ..
+00000ee0: 0972 1600 0000 7234 0000 0072 1700 0000  .r....r4...r....
+00000ef0: 7218 0000 0072 3f00 0000 5a0c 5f63 6f6e  r....r?...Z._con
+00000f00: 7375 6c5f 636f 6e66 724b 0000 005a 096d  sul_confrK...Z.m
+00000f10: 7973 716c 5f75 726c 7253 0000 0072 3100  ysql_urlrS...r1.
+00000f20: 0000 720e 0000 0072 0f00 0000 7247 0000  ..r....r....rG..
 00000f30: 0096 0000 0073 3200 0000 0002 1801 0803  .....s2.........
 00000f40: 1402 0e02 0201 0601 0400 02ff 04ff 0805  ................
 00000f50: 0c01 0601 0602 32ff 0206 0e03 0201 0601  ......2.........
 00000f60: 0400 02ff 04ff 0805 0c01 0601 7a16 4179  ............z.Ay
 00000f70: 7553 7069 6465 722e 6672 6f6d 5f63 7261  uSpider.from_cra
 00000f80: 776c 6572 2917 7219 0000 0072 1a00 0000  wler).r....r....
 00000f90: 721b 0000 0072 1c00 0000 5a16 6375 7374  r....r....Z.cust
 00000fa0: 6f6d 5f63 6f6d 6d6f 6e5f 7365 7474 696e  om_common_settin
 00000fb0: 6773 5a15 6375 7374 6f6d 5f64 6562 7567  gsZ.custom_debug
 00000fc0: 5f73 6574 7469 6e67 735a 1763 7573 746f  _settingsZ.custo
 00000fd0: 6d5f 7072 6f64 7563 745f 7365 7474 696e  m_product_settin
 00000fe0: 6773 da04 7469 6d65 da08 7374 7266 7469  gs..time..strfti
 00000ff0: 6d65 da09 6c6f 6361 6c74 696d 655a 0b53  me..localtimeZ.S
-00001000: 5049 4445 525f 5449 4d45 723e 0000 005a  PIDER_TIMEr>...Z
+00001000: 5049 4445 525f 5449 4d45 723c 0000 005a  PIDER_TIMEr<...Z
 00001010: 0f70 726f 6a65 6374 5f63 6f6e 7465 6e74  .project_content
-00001020: 723d 0000 0072 4f00 0000 7231 0000 0072  r=...rO...r1...r
-00001030: 1000 0000 da08 7072 6f70 6572 7479 723c  ......propertyr<
+00001020: 723b 0000 0072 4c00 0000 722f 0000 0072  r;...rL...r/...r
+00001030: 1000 0000 da08 7072 6f70 6572 7479 723a  ......propertyr:
 00001040: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
-00001050: 7246 0000 0072 4a00 0000 da0d 5f5f 636c  rF...rJ.....__cl
+00001050: 7243 0000 0072 4700 0000 da0d 5f5f 636c  rC...rG.....__cl
 00001060: 6173 7363 656c 6c5f 5f72 0e00 0000 720e  asscell__r....r.
-00001070: 0000 0072 3300 0000 720f 0000 0072 0900  ...r3...r....r..
+00001070: 0000 0072 3100 0000 720f 0000 0072 0900  ...r1...r....r..
 00001080: 0000 2900 0000 7350 0000 0008 0104 0602  ..)...sP........
 00001090: 0102 0102 0102 0102 fb06 0b02 0102 0202  ................
 000010a0: 0202 0202 0202 0202 0202 0202 ef06 1602  ................
 000010b0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 000010c0: f706 0d10 0204 0204 0204 0204 020c 060c  ................
 000010d0: 0402 010e 1702 010a 0f02 0129 1172 1d00  ...........).r..
-000010e0: 0000 7257 0000 00da 0e73 6372 6170 792e  ..rW.....scrapy.
+000010e0: 0000 7254 0000 00da 0e73 6372 6170 792e  ..rT.....scrapy.
 000010f0: 7370 6964 6572 7372 0200 0000 5a0a 7371  spidersr....Z.sq
 00001100: 6c61 6c63 6865 6d79 7203 0000 005a 2461  lalchemyr....Z$a
 00001110: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
-00001120: 636f 6d6d 6f6e 2e4d 756c 7469 506c 6578  common.MultiPlex
+00001120: 636f 6d6d 6f6e 2e6d 756c 7469 706c 6578  common.multiplex
 00001130: 696e 6772 0400 0000 5a24 6179 7567 6573  ingr....Z$ayuges
 00001140: 7069 6465 7274 6f6f 6c73 2e63 6f6d 6d6f  pidertools.commo
-00001150: 6e2e 5370 6964 6572 4442 436f 6e66 7205  n.SpiderDBConfr.
+00001150: 6e2e 7370 6964 6572 6462 636f 6e66 7205  n.spiderdbconfr.
 00001160: 0000 0072 0600 0000 7207 0000 005a 1761  ...r....r....Z.a
 00001170: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
 00001180: 636f 6e66 6967 7208 0000 00da 075f 5f61  configr......__a
 00001190: 6c6c 5f5f 720a 0000 0072 0900 0000 720e  ll__r....r....r.
 000011a0: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
 000011b0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
 000011c0: 7314 0000 0008 0108 020c 010c 020c 0114  s...............
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-2.0.1/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files 18% similar despite different names*

```diff
@@ -40,67 +40,67 @@
 
 # 加载秘钥等配置信息
 config_parser = configparser.ConfigParser()
 config_parser.read(f"{VIT_DIR}/.conf", encoding="utf-8")
 
 # Mysql 数据库配置
 LOCAL_MYSQL_CONFIG = {
-    "HOST": config_parser.get("MYSQL", "HOST", fallback=None),
-    "PORT": config_parser.getint("MYSQL", "PORT", fallback=3306),
-    "USER": config_parser.get("MYSQL", "USER", fallback="root"),
-    "PASSWORD": config_parser.get("MYSQL", "PASSWORD", fallback=None),
-    "CHARSET": config_parser.get("MYSQL", "CHARSET", fallback="utf8mb4"),
-    "DATABASE": config_parser.get("MYSQL", "DATABASE", fallback=None),
+    "host": config_parser.get("mysql", "host", fallback=None),
+    "port": config_parser.getint("mysql", "port", fallback=3306),
+    "user": config_parser.get("mysql", "user", fallback="root"),
+    "password": config_parser.get("mysql", "password", fallback=None),
+    "charset": config_parser.get("mysql", "charset", fallback="utf8mb4"),
+    "database": config_parser.get("mysql", "database", fallback=None),
     # 数据库 engin 采用的驱动，可不填此参数
-    "DRIVER": "mysqlconnector",
+    "driver": "mysqlconnector",
 }
 
 # MongoDB 数据库配置
 LOCAL_MONGODB_CONFIG = {
-    "HOST": config_parser.get("MONGODB", "HOST", fallback=None),
-    "PORT": config_parser.getint("MONGODB", "PORT", fallback=27017),
-    "AUTHSOURCE": config_parser.get("MONGODB", "AUTHSOURCE", fallback="admin"),
-    "USER": config_parser.get("MONGODB", "USER", fallback="admin"),
-    "PASSWORD": config_parser.get("MONGODB", "PASSWORD", fallback=None),
-    "DATABASE": config_parser.get("MONGODB", "DATABASE", fallback=None),
+    "host": config_parser.get("mongodb", "host", fallback=None),
+    "port": config_parser.getint("mongodb", "port", fallback=27017),
+    "authsource": config_parser.get("mongodb", "authsource", fallback="admin"),
+    "user": config_parser.get("mongodb", "user", fallback="admin"),
+    "password": config_parser.get("mongodb", "password", fallback=None),
+    "database": config_parser.get("mongodb", "database", fallback=None),
 }
 
 # consul 应用管理的连接配置
 CONSUL_CONFIG = {
-    "TOKEN": config_parser.get("CONSUL", "TOKEN", fallback=None),
-    "URL": config_parser.get("CONSUL", "URL", fallback=None),
-    "FORMAT": config_parser.get("CONSUL", "FORMAT", fallback="json"),
+    "token": config_parser.get("consul", "token", fallback=None),
+    "url": config_parser.get("consul", "url", fallback=None),
+    "format": config_parser.get("consul", "format", fallback="json"),
 }
 
 # 动态隧道代理（快代理版本）
 DYNAMIC_PROXY_CONFIG = {
-    "PROXY_URL": config_parser.get("KDL_DYNAMIC_PROXY", "PROXY_URL", fallback=None),
-    "USERNAME": config_parser.get("KDL_DYNAMIC_PROXY", "USERNAME", fallback=None),
-    "PASSWORD": config_parser.get("KDL_DYNAMIC_PROXY", "PASSWORD", fallback=None),
+    "proxy": config_parser.get("kdl_dynamic_proxy", "proxy", fallback=None),
+    "username": config_parser.get("kdl_dynamic_proxy", "username", fallback=None),
+    "password": config_parser.get("kdl_dynamic_proxy", "password", fallback=None),
 }
 
 # 独享代理（快代理版本）
 EXCLUSIVE_PROXY_CONFIG = {
-    "PROXY_URL": config_parser.get("KDL_EXCLUSIVE_PROXY", "PROXY_URL", fallback=None),
-    "USERNAME": config_parser.get("KDL_EXCLUSIVE_PROXY", "USERNAME", fallback=None),
-    "PASSWORD": config_parser.get("KDL_EXCLUSIVE_PROXY", "PASSWORD", fallback=None),
-    "PROXY_INDEX": config_parser.getint(
-        "KDL_EXCLUSIVE_PROXY", "PROXY_INDEX", fallback=1
+    "proxy": config_parser.get("kdl_exclusive_proxy", "proxy", fallback=None),
+    "username": config_parser.get("kdl_exclusive_proxy", "username", fallback=None),
+    "password": config_parser.get("kdl_exclusive_proxy", "password", fallback=None),
+    "index": config_parser.getint(
+        "kdl_exclusive_proxy", "index", fallback=1
     ),
 }
 
 # ali oss 对象存储
 OSS_CONFIG = {
-    "OssAccessKeyId": config_parser.get("ALI_OSS", "OssAccessKeyId", fallback=None),
-    "OssAccessKeySecret": config_parser.get(
-        "ALI_OSS", "OssAccessKeySecret", fallback=None
+    "accesskeyid": config_parser.get("ali_oss", "accesskeyid", fallback=None),
+    "accesskeysecret": config_parser.get(
+        "ali_oss", "accesskeysecret", fallback=None
     ),
-    "Endpoint": config_parser.get("ALI_OSS", "Endpoint", fallback=None),
-    "examplebucket": config_parser.get("ALI_OSS", "Examplebucket", fallback=None),
-    "operateDoc": config_parser.get("ALI_OSS", "OperateDoc", fallback=None),
+    "endpoint": config_parser.get("ali_oss", "endpoint", fallback=None),
+    "bucket": config_parser.get("ali_oss", "bucket", fallback=None),
+    "doc": config_parser.get("ali_oss", "doc", fallback=None),
 }
 
 # 日志管理
 LOG_LEVEL = env.str("LOG_LEVEL", "ERROR")
 LOG_FILE = f"{LOG_DIR}/$project_name.log"
 logger.add(
     env.str("LOG_ERROR_FILE", f"{LOG_DIR}/error.log"),
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/async.tmpl`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp
 from scrapy.http import Request
 from $project_name.settings import logger
 from scrapy.http.response.text import TextResponse
-from ayugespidertools.AyugeSpider import AyuSpider
+from ayugespidertools.spiders import AyuSpider
 
 """
 ########################################################################################################################
 # collection_website: $domain - 采集的目标站点介绍
 # collection_content: 采集内容介绍
 # create_time: xxxx-xx-xx
 # explain: async 协程在 spider 中的写法示例
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas
 from scrapy.http import Request
 from $project_name.settings import logger
 from scrapy.http.response.text import TextResponse
-from $project_name.common.DataEnum import TableEnum
-from ayugespidertools.AyugeSpider import AyuSpider
-from ayugespidertools.common.Utils import ToolsForAyu
-from ayugespidertools.Items import DataItem, MysqlDataItem, MongoDataItem
+from $project_name.items import TableEnum
+from ayugespidertools.spiders import AyuSpider
+from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.items import DataItem, MysqlDataItem, MongoDataItem
 
 """
 ####################################################################################################
 # collection_website: $domain - 采集的目标站点介绍
 # collection_content: 采集内容介绍
 # create_time: xxxx-xx-xx
 # explain:
@@ -36,21 +36,21 @@
         "LOGURU_CONFIG": logger,
         # Mysql 数据表的前缀名称，用于标记属于哪个项目，可不配置
         "MYSQL_TABLE_PREFIX": "demo_basic_",
         # MongoDB 集合的前缀名称，用于标记属于哪个项目，可不配置
         "MONGODB_COLLECTION_PREFIX": "demo_basic_",
         "ITEM_PIPELINES": {
             # 激活此项则数据会存储至 Mysql
-            "ayugespidertools.Pipelines.AyuFtyMysqlPipeline": 300,
+            "ayugespidertools.pipelines.AyuFtyMysqlPipeline": 300,
             # 激活此项则数据会存储至 MongoDB
-            "ayugespidertools.Pipelines.AyuFtyMongoPipeline": 301,
+            "ayugespidertools.pipelines.AyuFtyMongoPipeline": 301,
         },
         "DOWNLOADER_MIDDLEWARES": {
             # 随机请求头
-            "ayugespidertools.Middlewares.RandomRequestUaMiddleware": 400,
+            "ayugespidertools.middlewares.RandomRequestUaMiddleware": 400,
         },
     }
 
     # 打开 mysql 引擎开关，用于数据入库前更新逻辑判断
     mysql_engine_enabled = True
 
     def start_requests(self):
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import scrapy
 from scrapy.spiders import Rule
 from $project_name.settings import logger
 from scrapy.linkextractors import LinkExtractor
-from ayugespidertools.Items import MysqlDataItem
+from ayugespidertools.items import MysqlDataItem
 from $project_name.common.DataEnum import TableEnum
-from ayugespidertools.AyugeCrawlSpider import AyuCrawlSpider
+from ayugespidertools.spiders import AyuCrawlSpider
 
 
 class $classname(AyuCrawlSpider):
     name = "$name"
     allowed_domains = ["$domain"]
     start_urls = ["http://$domain/"]
 
@@ -19,19 +19,19 @@
     custom_settings = {
         # scrapy 日志等级配置
         "LOG_LEVEL": "DEBUG",
         # Mysql数据表的前缀名称，用于标记属于哪个项目，也可以不用配置
         "MYSQL_TABLE_PREFIX": "demo_crawl_",
         "ITEM_PIPELINES": {
             # 激活此项则数据会存储至 Mysql
-            "ayugespidertools.Pipelines.AyuFtyMysqlPipeline": 300,
+            "ayugespidertools.pipelines.AyuFtyMysqlPipeline": 300,
         },
         "DOWNLOADER_MIDDLEWARES": {
             # 随机请求头
-            "ayugespidertools.Middlewares.RandomRequestUaMiddleware": 400,
+            "ayugespidertools.middlewares.RandomRequestUaMiddleware": 400,
         },
     }
 
     rules = (
         # Rule(LinkExtractor(allow=r"Items/"), callback="parse_item", follow=True),
         Rule(LinkExtractor(restrict_xpaths='//div[@class="rank_d_b_name"]/a'), callback="parse_item"),
     )
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.9/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc` & `ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 18 02:22:33 2023 UTC, .py size: 5953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e9fe 3d64 4117 0000  U.........=dA...
+00000000: 550d 0d0a 0000 0000 f726 4a64 2017 0000  U........&Jd ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 2401 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
@@ -160,176 +160,174 @@
 000009f0: 8301 0100 7401 6402 8301 0100 7401 6403  ....t.d.....t.d.
 00000a00: 8301 0100 7402 7c00 7c01 8302 7d02 7403  ....t.|.|...}.t.
 00000a10: 7c02 a004 a100 8301 4400 5d22 5c02 7d03  |.......D.]"\.}.
 00000a20: 7d04 7401 6404 7c03 6405 9b04 6406 7c04  }.t.d.|.d...d.|.
 00000a30: a005 a100 9b00 9d04 8301 0100 7138 7c01  ............q8|.
 00000a40: 736e 7401 8300 0100 7401 6407 8301 0100  snt.....t.d.....
 00000a50: 7401 8300 0100 7401 6408 8301 0100 6400  t.....t.d.....d.
-00000a60: 5300 2909 4e7a 0655 7361 6765 3a7a 2e20  S.).Nz.Usage:z. 
-00000a70: 2061 7975 6765 7370 6964 6572 746f 6f6c   ayugespidertool
-00000a80: 7320 3c63 6f6d 6d61 6e64 3e20 5b6f 7074  s <command> [opt
-00000a90: 696f 6e73 5d20 5b61 7267 735d 0a7a 1341  ions] [args].z.A
-00000aa0: 7661 696c 6162 6c65 2063 6f6d 6d61 6e64  vailable command
-00000ab0: 733a 7a02 2020 7a03 3c31 33fa 0120 7a47  s:z.  z.<13.. zG
-00000ac0: 2020 5b20 6d6f 7265 205d 2020 2020 2020    [ more ]      
-00000ad0: 4d6f 7265 2063 6f6d 6d61 6e64 7320 6176  More commands av
-00000ae0: 6169 6c61 626c 6520 7768 656e 2072 756e  ailable when run
-00000af0: 2066 726f 6d20 7072 6f6a 6563 7420 6469   from project di
-00000b00: 7265 6374 6f72 797a 4455 7365 2022 6179  rectoryzDUse "ay
-00000b10: 7567 6573 7069 6465 7274 6f6f 6c73 203c  ugespidertools <
-00000b20: 636f 6d6d 616e 643e 202d 6822 2074 6f20  command> -h" to 
-00000b30: 7365 6520 6d6f 7265 2069 6e66 6f20 6162  see more info ab
-00000b40: 6f75 7420 6120 636f 6d6d 616e 6429 0672  out a command).r
-00000b50: 4600 0000 7244 0000 0072 3700 0000 da06  F...rD...r7.....
-00000b60: 736f 7274 6564 da05 6974 656d 735a 0a73  sorted..itemsZ.s
-00000b70: 686f 7274 5f64 6573 6329 0572 3600 0000  hort_desc).r6...
-00000b80: 7226 0000 0072 3100 0000 7229 0000 005a  r&...r1...r)...Z
-00000b90: 0863 6d64 636c 6173 7372 1300 0000 7213  .cmdclassr....r.
-00000ba0: 0000 0072 1400 0000 da0f 5f70 7269 6e74  ...r......_print
-00000bb0: 5f63 6f6d 6d61 6e64 7357 0000 0073 1800  _commandsW...s..
-00000bc0: 0000 0001 0a01 0801 0801 0801 0a01 1401  ................
-00000bd0: 1c01 0401 0601 0801 0601 724a 0000 0063  ..........rJ...c
-00000be0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000bf0: 0400 0000 4300 0000 7326 0000 0074 007c  ....C...s&...t.|
-00000c00: 007c 0283 0201 0074 0164 017c 019b 0064  .|.....t.d.|...d
-00000c10: 029d 0383 0101 0074 0164 0383 0101 0064  .......t.d.....d
-00000c20: 0053 0029 044e 7a11 556e 6b6e 6f77 6e20  .S.).Nz.Unknown 
-00000c30: 636f 6d6d 616e 643a 2072 4200 0000 7a30  command: rB...z0
-00000c40: 5573 6520 2261 7975 6765 7370 6964 6572  Use "ayugespider
-00000c50: 746f 6f6c 7322 2074 6f20 7365 6520 6176  tools" to see av
-00000c60: 6169 6c61 626c 6520 636f 6d6d 616e 6473  ailable commands
-00000c70: 2902 7246 0000 0072 4400 0000 2903 7236  ).rF...rD...).r6
-00000c80: 0000 0072 2900 0000 7226 0000 0072 1300  ...r)...r&...r..
-00000c90: 0000 7213 0000 0072 1400 0000 da16 5f70  ..r....r......_p
-00000ca0: 7269 6e74 5f75 6e6b 6e6f 776e 5f63 6f6d  rint_unknown_com
-00000cb0: 6d61 6e64 6600 0000 7306 0000 0000 010a  mandf...s.......
-00000cc0: 0110 0172 4b00 0000 6302 0000 0000 0000  ...rK...c.......
-00000cd0: 0000 0000 0005 0000 000a 0000 004f 0000  .............O..
-00000ce0: 0073 6400 0000 7a0e 7c01 7c02 7c03 8e01  .sd...z.|.|.|...
-00000cf0: 0100 5700 6e50 0400 7400 6b0a 725e 0100  ..W.nP..t.k.r^..
-00000d00: 7d04 0100 7a32 7401 7c04 8301 7236 7c00  }...z2t.|...r6|.
-00000d10: a002 7401 7c04 8301 a101 0100 7c04 6a03  ..t.|.......|.j.
-00000d20: 7244 7c00 a003 a100 0100 7404 a005 6401  rD|.......t...d.
-00000d30: a101 0100 5700 3500 6400 7d04 7e04 5800  ....W.5.d.}.~.X.
-00000d40: 5900 6e02 5800 6400 5300 2902 4e72 0c00  Y.n.X.d.S.).Nr..
-00000d50: 0000 2906 7205 0000 00da 0373 7472 da05  ..).r......str..
-00000d60: 6572 726f 72da 0a70 7269 6e74 5f68 656c  error..print_hel
-00000d70: 70da 0373 7973 da04 6578 6974 2905 da06  p..sys..exit)...
-00000d80: 7061 7273 6572 da04 6675 6e63 da01 61da  parser..func..a.
-00000d90: 026b 77da 0165 7213 0000 0072 1300 0000  .kw..er....r....
-00000da0: 7214 0000 00da 0f5f 7275 6e5f 7072 696e  r......_run_prin
-00000db0: 745f 6865 6c70 6c00 0000 7310 0000 0000  t_helpl...s.....
-00000dc0: 0102 010e 0110 0108 010e 0106 0108 0172  ...............r
-00000dd0: 5600 0000 6302 0000 0000 0000 0000 0000  V...c...........
-00000de0: 000a 0000 0008 0000 0043 0000 0073 3601  .........C...s6.
-00000df0: 0000 7c00 6400 6b08 720e 7400 6a01 7d00  ..|.d.k.r.t.j.}.
-00000e00: 7c01 6400 6b08 7248 7402 8300 7d01 7a0e  |.d.k.rHt...}.z.
-00000e10: 7403 6a04 6401 1900 7d02 5700 6e14 0400  t.j.d...}.W.n...
-00000e20: 7405 6b0a 723e 0100 0100 0100 5900 6e0a  t.k.r>......Y.n.
-00000e30: 5800 7c02 7c01 6401 3c00 7406 8300 7d03  X.|.|.d.<.t...}.
-00000e40: 7407 7c01 7c03 8302 7d04 7408 7c00 8301  t.|.|...}.t.|...
-00000e50: 7d05 7c05 737a 7409 7c01 7c03 8302 0100  }.|.szt.|.|.....
-00000e60: 7400 a00a 6402 a101 0100 6e1e 7c05 7c04  t...d.....n.|.|.
-00000e70: 6b07 7298 740b 7c01 7c05 7c03 8303 0100  k.r.t.|.|.|.....
-00000e80: 7400 a00a 6403 a101 0100 7c04 7c05 1900  t...d.....|.|...
-00000e90: 7d06 740c 740d 6404 7c05 9b00 6405 7c06  }.t.t.d.|...d.|.
-00000ea0: a00e a100 9b00 9d04 6406 7c06 a00f a100  ........d.|.....
-00000eb0: 6407 8d04 7d07 7c01 6a10 7c06 6a11 6408  d...}.|.j.|.j.d.
-00000ec0: 6409 8d02 0100 7c01 7c06 5f12 7c06 a013  d.....|.|._.|...
-00000ed0: 7c07 a101 0100 7c07 6a14 7c00 640a 6400  |.....|.j.|.d.d.
-00000ee0: 8502 1900 640b 8d01 5c02 7d08 7d09 7415  ....d...\.}.}.t.
-00000ef0: 7c07 7c06 6a16 7c09 7c08 8304 0100 7417  |.|.j.|.|.....t.
-00000f00: 7c01 8301 7c06 5f18 7415 7c07 7419 7c06  |...|._.t.|.t.|.
-00000f10: 7c09 7c08 8305 0100 7400 a00a 7c06 6a1a  |.|.....t...|.j.
-00000f20: a101 0100 6400 5300 290c 4eda 0645 4449  ....d.S.).N..EDI
-00000f30: 544f 5272 0100 0000 720c 0000 007a 1161  TORr....r....z.a
-00000f40: 7975 6765 7370 6964 6572 746f 6f6c 7320  yugespidertools 
-00000f50: 7247 0000 00da 0772 6573 6f6c 7665 2904  rG.....resolve).
-00000f60: da0f 666f 726d 6174 7465 725f 636c 6173  ..formatter_clas
-00000f70: 73da 0575 7361 6765 da10 636f 6e66 6c69  s..usage..confli
-00000f80: 6374 5f68 616e 646c 6572 da0b 6465 7363  ct_handler..desc
-00000f90: 7269 7074 696f 6eda 0763 6f6d 6d61 6e64  ription..command
-00000fa0: 2901 da08 7072 696f 7269 7479 7238 0000  )...priorityr8..
-00000fb0: 0029 0172 3f00 0000 291b 724f 0000 0072  .).r?...).rO...r
-00000fc0: 3b00 0000 7207 0000 00da 026f 73da 0765  ;...r......os..e
-00000fd0: 6e76 6972 6f6e da08 4b65 7945 7272 6f72  nviron..KeyError
-00000fe0: 7208 0000 0072 3700 0000 723e 0000 0072  r....r7...r>...r
-00000ff0: 4a00 0000 7250 0000 0072 4b00 0000 720b  J...rP...rK...r.
-00001000: 0000 0072 0300 0000 5a06 7379 6e74 6178  ...r....Z.syntax
-00001010: 5a09 6c6f 6e67 5f64 6573 63da 0773 6574  Z.long_desc..set
-00001020: 6469 6374 da10 6465 6661 756c 745f 7365  dict..default_se
-00001030: 7474 696e 6773 7236 0000 005a 0b61 6464  ttingsr6...Z.add
-00001040: 5f6f 7074 696f 6e73 da10 7061 7273 655f  _options..parse_
-00001050: 6b6e 6f77 6e5f 6172 6773 7256 0000 005a  known_argsrV...Z
-00001060: 0f70 726f 6365 7373 5f6f 7074 696f 6e73  .process_options
-00001070: 7204 0000 005a 0f63 7261 776c 6572 5f70  r....Z.crawler_p
-00001080: 726f 6365 7373 da0c 5f72 756e 5f63 6f6d  rocess.._run_com
-00001090: 6d61 6e64 da08 6578 6974 636f 6465 290a  mand..exitcode).
-000010a0: 723b 0000 0072 3600 0000 5a06 6564 6974  r;...r6...Z.edit
-000010b0: 6f72 7226 0000 0072 3100 0000 7229 0000  orr&...r1...r)..
-000010c0: 0072 2800 0000 7251 0000 0072 4000 0000  .r(...rQ...r@...
-000010d0: 723f 0000 0072 1300 0000 7213 0000 0072  r?...r....r....r
-000010e0: 1400 0000 da07 6578 6563 7574 6577 0000  ......executew..
-000010f0: 0073 4200 0000 0001 0801 0602 0801 0602  .sB.............
-00001100: 0201 0e01 0e01 0602 0802 0601 0a01 0801  ................
-00001110: 0401 0a01 0c01 0801 0c01 0a02 0801 0201  ................
-00001120: 0201 1201 0201 06fc 0606 1001 0601 0a01  ................
-00001130: 1801 1002 0a01 1001 7267 0000 0063 0300  ........rg...c..
-00001140: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001150: 0000 4300 0000 7324 0000 007c 026a 0072  ..C...s$...|.j.r
-00001160: 1474 017c 007c 017c 0283 0301 006e 0c7c  .t.|.|.|.....n.|
-00001170: 00a0 027c 017c 02a1 0201 0064 0053 0072  ...|.|.....d.S.r
-00001180: 1900 0000 2903 da07 7072 6f66 696c 65da  ....)...profile.
-00001190: 155f 7275 6e5f 636f 6d6d 616e 645f 7072  ._run_command_pr
-000011a0: 6f66 696c 6564 7243 0000 0029 0372 2800  ofiledrC...).r(.
-000011b0: 0000 723f 0000 0072 4000 0000 7213 0000  ..r?...r@...r...
-000011c0: 0072 1300 0000 7214 0000 0072 6500 0000  .r....r....re...
-000011d0: a100 0000 7306 0000 0000 0106 010e 0272  ....s..........r
-000011e0: 6500 0000 6303 0000 0000 0000 0000 0000  e...c...........
-000011f0: 0005 0000 0005 0000 0043 0000 0073 5000  .........C...sP.
-00001200: 0000 7c02 6a00 721c 7401 6a02 a003 6401  ..|.j.r.t.j...d.
-00001210: 7c02 6a00 9b02 6402 9d03 a101 0100 7404  |.j...d.......t.
-00001220: 8300 7d03 7405 a006 a100 7d04 7c04 a007  ..}.t.....}.|...
-00001230: 6403 7408 8300 7c03 a103 0100 7c02 6a00  d.t...|.....|.j.
-00001240: 724c 7c04 a009 7c02 6a00 a101 0100 6400  rL|...|.j.....d.
-00001250: 5300 2904 4e7a 2c61 7975 6765 7370 6964  S.).Nz,ayugespid
-00001260: 6572 746f 6f6c 733a 2077 7269 7469 6e67  ertools: writing
-00001270: 2063 5072 6f66 696c 6520 7374 6174 7320   cProfile stats 
-00001280: 746f 2072 4200 0000 7a13 636d 642e 7275  to rB...z.cmd.ru
-00001290: 6e28 6172 6773 2c20 6f70 7473 2929 0a72  n(args, opts)).r
-000012a0: 6800 0000 724f 0000 00da 0673 7464 6572  h...rO.....stder
-000012b0: 72da 0577 7269 7465 da06 6c6f 6361 6c73  r..write..locals
-000012c0: da08 6350 726f 6669 6c65 5a07 5072 6f66  ..cProfileZ.Prof
-000012d0: 696c 655a 0672 756e 6374 78da 0767 6c6f  ileZ.runctx..glo
-000012e0: 6261 6c73 5a0a 6475 6d70 5f73 7461 7473  balsZ.dump_stats
-000012f0: 2905 7228 0000 0072 3f00 0000 7240 0000  ).r(...r?...r@..
-00001300: 00da 036c 6f63 da01 7072 1300 0000 7213  ...loc..pr....r.
-00001310: 0000 0072 1400 0000 7269 0000 00a8 0000  ...r....ri......
-00001320: 0073 1200 0000 0001 0601 0601 0cff 0403  .s..............
-00001330: 0601 0801 1001 0601 7269 0000 00da 085f  ........ri....._
-00001340: 5f6d 6169 6e5f 5f29 0172 2b00 0000 2902  _main__).r+...).
-00001350: 4e4e 2925 da08 6172 6770 6172 7365 726d  NN)%..argparserm
-00001360: 0000 0072 1c00 0000 725f 0000 0072 4f00  ...r....r_...rO.
-00001370: 0000 722c 0000 005a 0f73 6372 6170 792e  ..r,...Z.scrapy.
-00001380: 636f 6d6d 616e 6473 7202 0000 0072 0300  commandsr....r..
-00001390: 0000 5a0e 7363 7261 7079 2e63 7261 776c  ..Z.scrapy.crawl
-000013a0: 6572 7204 0000 00da 1173 6372 6170 792e  err......scrapy.
-000013b0: 6578 6365 7074 696f 6e73 7205 0000 00da  exceptionsr.....
-000013c0: 1173 6372 6170 792e 7574 696c 732e 6d69  .scrapy.utils.mi
-000013d0: 7363 7206 0000 005a 1473 6372 6170 792e  scr....Z.scrapy.
-000013e0: 7574 696c 732e 7072 6f6a 6563 7472 0700  utils.projectr..
-000013f0: 0000 7208 0000 00da 1373 6372 6170 792e  ..r......scrapy.
-00001400: 7574 696c 732e 7079 7468 6f6e 7209 0000  utils.pythonr...
-00001410: 005a 2161 7975 6765 7370 6964 6572 746f  .Z!ayugespiderto
-00001420: 6f6c 732e 636f 6d6d 616e 6473 2e76 6572  ols.commands.ver
-00001430: 7369 6f6e 720a 0000 00da 0e41 7267 756d  sionr......Argum
-00001440: 656e 7450 6172 7365 7272 0b00 0000 7222  entParserr....r"
-00001450: 0000 0072 2a00 0000 7233 0000 0072 3700  ...r*...r3...r7.
-00001460: 0000 723e 0000 0072 4600 0000 724a 0000  ..r>...rF...rJ..
-00001470: 0072 4b00 0000 7256 0000 0072 6700 0000  .rK...rV...rg...
-00001480: 7265 0000 0072 6900 0000 7215 0000 0072  re...ri...r....r
-00001490: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-000014a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000014b0: 0073 3a00 0000 0801 0801 0801 0801 0802  .s:.............
-000014c0: 0801 1001 0c01 0c01 0c01 1001 0c02 0c03  ................
-000014d0: 1209 080e 0809 0a0b 0809 0809 0808 080f  ................
-000014e0: 0806 080b 0a2a 0807 080c 0a01 0201 0a05  .....*..........
+00000a60: 5300 2909 4e7a 0655 7361 6765 3a7a 2320  S.).Nz.Usage:z# 
+00000a70: 2061 7975 6765 203c 636f 6d6d 616e 643e   ayuge <command>
+00000a80: 205b 6f70 7469 6f6e 735d 205b 6172 6773   [options] [args
+00000a90: 5d0a 7a13 4176 6169 6c61 626c 6520 636f  ].z.Available co
+00000aa0: 6d6d 616e 6473 3a7a 0220 207a 033c 3133  mmands:z.  z.<13
+00000ab0: fa01 207a 4720 205b 206d 6f72 6520 5d20  .. zG  [ more ] 
+00000ac0: 2020 2020 204d 6f72 6520 636f 6d6d 616e       More comman
+00000ad0: 6473 2061 7661 696c 6162 6c65 2077 6865  ds available whe
+00000ae0: 6e20 7275 6e20 6672 6f6d 2070 726f 6a65  n run from proje
+00000af0: 6374 2064 6972 6563 746f 7279 7a39 5573  ct directoryz9Us
+00000b00: 6520 2261 7975 6765 203c 636f 6d6d 616e  e "ayuge <comman
+00000b10: 643e 202d 6822 2074 6f20 7365 6520 6d6f  d> -h" to see mo
+00000b20: 7265 2069 6e66 6f20 6162 6f75 7420 6120  re info about a 
+00000b30: 636f 6d6d 616e 6429 0672 4600 0000 7244  command).rF...rD
+00000b40: 0000 0072 3700 0000 da06 736f 7274 6564  ...r7.....sorted
+00000b50: da05 6974 656d 735a 0a73 686f 7274 5f64  ..itemsZ.short_d
+00000b60: 6573 6329 0572 3600 0000 7226 0000 0072  esc).r6...r&...r
+00000b70: 3100 0000 7229 0000 005a 0863 6d64 636c  1...r)...Z.cmdcl
+00000b80: 6173 7372 1300 0000 7213 0000 0072 1400  assr....r....r..
+00000b90: 0000 da0f 5f70 7269 6e74 5f63 6f6d 6d61  ...._print_comma
+00000ba0: 6e64 7357 0000 0073 1800 0000 0001 0a01  ndsW...s........
+00000bb0: 0801 0801 0801 0a01 1401 1c01 0401 0601  ................
+00000bc0: 0801 0601 724a 0000 0063 0300 0000 0000  ....rJ...c......
+00000bd0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000be0: 0000 7326 0000 0074 007c 007c 0283 0201  ..s&...t.|.|....
+00000bf0: 0074 0164 017c 019b 0064 029d 0383 0101  .t.d.|...d......
+00000c00: 0074 0164 0383 0101 0064 0053 0029 044e  .t.d.....d.S.).N
+00000c10: 7a11 556e 6b6e 6f77 6e20 636f 6d6d 616e  z.Unknown comman
+00000c20: 643a 2072 4200 0000 7a25 5573 6520 2261  d: rB...z%Use "a
+00000c30: 7975 6765 2220 746f 2073 6565 2061 7661  yuge" to see ava
+00000c40: 696c 6162 6c65 2063 6f6d 6d61 6e64 7329  ilable commands)
+00000c50: 0272 4600 0000 7244 0000 0029 0372 3600  .rF...rD...).r6.
+00000c60: 0000 7229 0000 0072 2600 0000 7213 0000  ..r)...r&...r...
+00000c70: 0072 1300 0000 7214 0000 00da 165f 7072  .r....r......_pr
+00000c80: 696e 745f 756e 6b6e 6f77 6e5f 636f 6d6d  int_unknown_comm
+00000c90: 616e 6466 0000 0073 0600 0000 0001 0a01  andf...s........
+00000ca0: 1001 724b 0000 0063 0200 0000 0000 0000  ..rK...c........
+00000cb0: 0000 0000 0500 0000 0a00 0000 4f00 0000  ............O...
+00000cc0: 7364 0000 007a 0e7c 017c 027c 038e 0101  sd...z.|.|.|....
+00000cd0: 0057 006e 5004 0074 006b 0a72 5e01 007d  .W.nP..t.k.r^..}
+00000ce0: 0401 007a 3274 017c 0483 0172 367c 00a0  ...z2t.|...r6|..
+00000cf0: 0274 017c 0483 01a1 0101 007c 046a 0372  .t.|.......|.j.r
+00000d00: 447c 00a0 03a1 0001 0074 04a0 0564 01a1  D|.......t...d..
+00000d10: 0101 0057 0035 0064 007d 047e 0458 0059  ...W.5.d.}.~.X.Y
+00000d20: 006e 0258 0064 0053 0029 024e 720c 0000  .n.X.d.S.).Nr...
+00000d30: 0029 0672 0500 0000 da03 7374 72da 0565  .).r......str..e
+00000d40: 7272 6f72 da0a 7072 696e 745f 6865 6c70  rror..print_help
+00000d50: da03 7379 73da 0465 7869 7429 05da 0670  ..sys..exit)...p
+00000d60: 6172 7365 72da 0466 756e 63da 0161 da02  arser..func..a..
+00000d70: 6b77 da01 6572 1300 0000 7213 0000 0072  kw..er....r....r
+00000d80: 1400 0000 da0f 5f72 756e 5f70 7269 6e74  ......_run_print
+00000d90: 5f68 656c 706c 0000 0073 1000 0000 0001  _helpl...s......
+00000da0: 0201 0e01 1001 0801 0e01 0601 0801 7256  ..............rV
+00000db0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000dc0: 0a00 0000 0800 0000 4300 0000 7336 0100  ........C...s6..
+00000dd0: 007c 0064 006b 0872 0e74 006a 017d 007c  .|.d.k.r.t.j.}.|
+00000de0: 0164 006b 0872 4874 0283 007d 017a 0e74  .d.k.rHt...}.z.t
+00000df0: 036a 0464 0119 007d 0257 006e 1404 0074  .j.d...}.W.n...t
+00000e00: 056b 0a72 3e01 0001 0001 0059 006e 0a58  .k.r>......Y.n.X
+00000e10: 007c 027c 0164 013c 0074 0683 007d 0374  .|.|.d.<.t...}.t
+00000e20: 077c 017c 0383 027d 0474 087c 0083 017d  .|.|...}.t.|...}
+00000e30: 057c 0573 7a74 097c 017c 0383 0201 0074  .|.szt.|.|.....t
+00000e40: 00a0 0a64 02a1 0101 006e 1e7c 057c 046b  ...d.....n.|.|.k
+00000e50: 0772 9874 0b7c 017c 057c 0383 0301 0074  .r.t.|.|.|.....t
+00000e60: 00a0 0a64 03a1 0101 007c 047c 0519 007d  ...d.....|.|...}
+00000e70: 0674 0c74 0d64 047c 059b 0064 057c 06a0  .t.t.d.|...d.|..
+00000e80: 0ea1 009b 009d 0464 067c 06a0 0fa1 0064  .......d.|.....d
+00000e90: 078d 047d 077c 016a 107c 066a 1164 0864  ...}.|.j.|.j.d.d
+00000ea0: 098d 0201 007c 017c 065f 127c 06a0 137c  .....|.|._.|...|
+00000eb0: 07a1 0101 007c 076a 147c 0064 0a64 0085  .....|.j.|.d.d..
+00000ec0: 0219 0064 0b8d 015c 027d 087d 0974 157c  ...d...\.}.}.t.|
+00000ed0: 077c 066a 167c 097c 0883 0401 0074 177c  .|.j.|.|.....t.|
+00000ee0: 0183 017c 065f 1874 157c 0774 197c 067c  ...|._.t.|.t.|.|
+00000ef0: 097c 0883 0501 0074 00a0 0a7c 066a 1aa1  .|.....t...|.j..
+00000f00: 0101 0064 0053 0029 0c4e da06 4544 4954  ...d.S.).N..EDIT
+00000f10: 4f52 7201 0000 0072 0c00 0000 7a11 6179  ORr....r....z.ay
+00000f20: 7567 6573 7069 6465 7274 6f6f 6c73 2072  ugespidertools r
+00000f30: 4700 0000 da07 7265 736f 6c76 6529 04da  G.....resolve)..
+00000f40: 0f66 6f72 6d61 7474 6572 5f63 6c61 7373  .formatter_class
+00000f50: da05 7573 6167 65da 1063 6f6e 666c 6963  ..usage..conflic
+00000f60: 745f 6861 6e64 6c65 72da 0b64 6573 6372  t_handler..descr
+00000f70: 6970 7469 6f6e da07 636f 6d6d 616e 6429  iption..command)
+00000f80: 01da 0870 7269 6f72 6974 7972 3800 0000  ...priorityr8...
+00000f90: 2901 723f 0000 0029 1b72 4f00 0000 723b  ).r?...).rO...r;
+00000fa0: 0000 0072 0700 0000 da02 6f73 da07 656e  ...r......os..en
+00000fb0: 7669 726f 6eda 084b 6579 4572 726f 7272  viron..KeyErrorr
+00000fc0: 0800 0000 7237 0000 0072 3e00 0000 724a  ....r7...r>...rJ
+00000fd0: 0000 0072 5000 0000 724b 0000 0072 0b00  ...rP...rK...r..
+00000fe0: 0000 7203 0000 005a 0673 796e 7461 785a  ..r....Z.syntaxZ
+00000ff0: 096c 6f6e 675f 6465 7363 da07 7365 7464  .long_desc..setd
+00001000: 6963 74da 1064 6566 6175 6c74 5f73 6574  ict..default_set
+00001010: 7469 6e67 7372 3600 0000 5a0b 6164 645f  tingsr6...Z.add_
+00001020: 6f70 7469 6f6e 73da 1070 6172 7365 5f6b  options..parse_k
+00001030: 6e6f 776e 5f61 7267 7372 5600 0000 5a0f  nown_argsrV...Z.
+00001040: 7072 6f63 6573 735f 6f70 7469 6f6e 7372  process_optionsr
+00001050: 0400 0000 5a0f 6372 6177 6c65 725f 7072  ....Z.crawler_pr
+00001060: 6f63 6573 73da 0c5f 7275 6e5f 636f 6d6d  ocess.._run_comm
+00001070: 616e 64da 0865 7869 7463 6f64 6529 0a72  and..exitcode).r
+00001080: 3b00 0000 7236 0000 005a 0665 6469 746f  ;...r6...Z.edito
+00001090: 7272 2600 0000 7231 0000 0072 2900 0000  rr&...r1...r)...
+000010a0: 7228 0000 0072 5100 0000 7240 0000 0072  r(...rQ...r@...r
+000010b0: 3f00 0000 7213 0000 0072 1300 0000 7214  ?...r....r....r.
+000010c0: 0000 00da 0765 7865 6375 7465 7700 0000  .....executew...
+000010d0: 7342 0000 0000 0108 0106 0208 0106 0202  sB..............
+000010e0: 010e 010e 0106 0208 0206 010a 0108 0104  ................
+000010f0: 010a 010c 0108 010c 010a 0208 0102 0102  ................
+00001100: 0112 0102 0106 fc06 0610 0106 010a 0118  ................
+00001110: 0110 020a 0110 0172 6700 0000 6303 0000  .......rg...c...
+00001120: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00001130: 0043 0000 0073 2400 0000 7c02 6a00 7214  .C...s$...|.j.r.
+00001140: 7401 7c00 7c01 7c02 8303 0100 6e0c 7c00  t.|.|.|.....n.|.
+00001150: a002 7c01 7c02 a102 0100 6400 5300 7219  ..|.|.....d.S.r.
+00001160: 0000 0029 03da 0770 726f 6669 6c65 da15  ...)...profile..
+00001170: 5f72 756e 5f63 6f6d 6d61 6e64 5f70 726f  _run_command_pro
+00001180: 6669 6c65 6472 4300 0000 2903 7228 0000  filedrC...).r(..
+00001190: 0072 3f00 0000 7240 0000 0072 1300 0000  .r?...r@...r....
+000011a0: 7213 0000 0072 1400 0000 7265 0000 00a1  r....r....re....
+000011b0: 0000 0073 0600 0000 0001 0601 0e02 7265  ...s..........re
+000011c0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+000011d0: 0500 0000 0500 0000 4300 0000 7350 0000  ........C...sP..
+000011e0: 007c 026a 0072 1c74 016a 02a0 0364 017c  .|.j.r.t.j...d.|
+000011f0: 026a 009b 0264 029d 03a1 0101 0074 0483  .j...d.......t..
+00001200: 007d 0374 05a0 06a1 007d 047c 04a0 0764  .}.t.....}.|...d
+00001210: 0374 0883 007c 03a1 0301 007c 026a 0072  .t...|.....|.j.r
+00001220: 4c7c 04a0 097c 026a 00a1 0101 0064 0053  L|...|.j.....d.S
+00001230: 0029 044e 7a2c 6179 7567 6573 7069 6465  .).Nz,ayugespide
+00001240: 7274 6f6f 6c73 3a20 7772 6974 696e 6720  rtools: writing 
+00001250: 6350 726f 6669 6c65 2073 7461 7473 2074  cProfile stats t
+00001260: 6f20 7242 0000 007a 1363 6d64 2e72 756e  o rB...z.cmd.run
+00001270: 2861 7267 732c 206f 7074 7329 290a 7268  (args, opts)).rh
+00001280: 0000 0072 4f00 0000 da06 7374 6465 7272  ...rO.....stderr
+00001290: da05 7772 6974 65da 066c 6f63 616c 73da  ..write..locals.
+000012a0: 0863 5072 6f66 696c 655a 0750 726f 6669  .cProfileZ.Profi
+000012b0: 6c65 5a06 7275 6e63 7478 da07 676c 6f62  leZ.runctx..glob
+000012c0: 616c 735a 0a64 756d 705f 7374 6174 7329  alsZ.dump_stats)
+000012d0: 0572 2800 0000 723f 0000 0072 4000 0000  .r(...r?...r@...
+000012e0: da03 6c6f 63da 0170 7213 0000 0072 1300  ..loc..pr....r..
+000012f0: 0000 7214 0000 0072 6900 0000 a800 0000  ..r....ri.......
+00001300: 7312 0000 0000 0106 0106 010c ff04 0306  s...............
+00001310: 0108 0110 0106 0172 6900 0000 da08 5f5f  .......ri.....__
+00001320: 6d61 696e 5f5f 2901 722b 0000 0029 024e  main__).r+...).N
+00001330: 4e29 25da 0861 7267 7061 7273 6572 6d00  N)%..argparserm.
+00001340: 0000 721c 0000 0072 5f00 0000 724f 0000  ..r....r_...rO..
+00001350: 0072 2c00 0000 5a0f 7363 7261 7079 2e63  .r,...Z.scrapy.c
+00001360: 6f6d 6d61 6e64 7372 0200 0000 7203 0000  ommandsr....r...
+00001370: 005a 0e73 6372 6170 792e 6372 6177 6c65  .Z.scrapy.crawle
+00001380: 7272 0400 0000 da11 7363 7261 7079 2e65  rr......scrapy.e
+00001390: 7863 6570 7469 6f6e 7372 0500 0000 da11  xceptionsr......
+000013a0: 7363 7261 7079 2e75 7469 6c73 2e6d 6973  scrapy.utils.mis
+000013b0: 6372 0600 0000 5a14 7363 7261 7079 2e75  cr....Z.scrapy.u
+000013c0: 7469 6c73 2e70 726f 6a65 6374 7207 0000  tils.projectr...
+000013d0: 0072 0800 0000 da13 7363 7261 7079 2e75  .r......scrapy.u
+000013e0: 7469 6c73 2e70 7974 686f 6e72 0900 0000  tils.pythonr....
+000013f0: 5a21 6179 7567 6573 7069 6465 7274 6f6f  Z!ayugespidertoo
+00001400: 6c73 2e63 6f6d 6d61 6e64 732e 7665 7273  ls.commands.vers
+00001410: 696f 6e72 0a00 0000 da0e 4172 6775 6d65  ionr......Argume
+00001420: 6e74 5061 7273 6572 720b 0000 0072 2200  ntParserr....r".
+00001430: 0000 722a 0000 0072 3300 0000 7237 0000  ..r*...r3...r7..
+00001440: 0072 3e00 0000 7246 0000 0072 4a00 0000  .r>...rF...rJ...
+00001450: 724b 0000 0072 5600 0000 7267 0000 0072  rK...rV...rg...r
+00001460: 6500 0000 7269 0000 0072 1500 0000 7213  e...ri...r....r.
+00001470: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00001480: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001490: 733a 0000 0008 0108 0108 0108 0108 0208  s:..............
+000014a0: 0110 010c 010c 010c 0110 010c 020c 0312  ................
+000014b0: 0908 0e08 090a 0b08 0908 0908 0808 0f08  ................
+000014c0: 0608 0b0a 2a08 0708 0c0a 0102 010a 05    ....*..........
```

### Comparing `ayugespidertools-1.1.9/ayugespidertools/utils/cmdline.py` & `ayugespidertools-2.0.1/ayugespidertools/utils/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,30 +83,30 @@
     else:
         print(f"AyugeSpiderTools {version} - no active project\n")
 
 
 def _print_commands(settings, inproject):
     _print_header(settings, inproject)
     print("Usage:")
-    print("  ayugespidertools <command> [options] [args]\n")
+    print("  ayuge <command> [options] [args]\n")
     print("Available commands:")
     cmds = _get_commands_dict(settings, inproject)
     for cmdname, cmdclass in sorted(cmds.items()):
         print(f"  {cmdname:<13} {cmdclass.short_desc()}")
     if not inproject:
         print()
         print("  [ more ]      More commands available when run from project directory")
     print()
-    print('Use "ayugespidertools <command> -h" to see more info about a command')
+    print('Use "ayuge <command> -h" to see more info about a command')
 
 
 def _print_unknown_command(settings, cmdname, inproject):
     _print_header(settings, inproject)
     print(f"Unknown command: {cmdname}\n")
-    print('Use "ayugespidertools" to see available commands')
+    print('Use "ayuge" to see available commands')
 
 
 def _run_print_help(parser, func, *a, **kw):
     try:
         func(*a, **kw)
     except UsageError as e:
         if str(e):
```

### Comparing `ayugespidertools-1.1.9/pyproject.toml` & `ayugespidertools-2.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "1.1.9"
+version = "2.0.1"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -83,17 +83,14 @@
 omit = [
     "tests/docs/*",
     "tests/VIT/*",
     "tests/conftest.py",
     "tests/**/__init__.py",
     "ayugespidertools/**/__init__.py",
     "ayugespidertools/utils/cmdline.py",
-    "ayugespidertools/scraper/pipelines/*",
-    "ayugespidertools/scraper/http/*",
-    "ayugespidertools/scraper/middlewares/*",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "if __name__ == '__main__':",
     "pragma: no cover",
     "raise AssertionError",
```

### Comparing `ayugespidertools-1.1.9/PKG-INFO` & `ayugespidertools-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 1.1.9
+Version: 2.0.1
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -68,15 +68,15 @@
 
 > `python 3.8+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
-注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.6` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
+注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.4` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
 ## 2. 使用方法
 
 > 项目主要包含两部分：
 >
 
 - 开发场景中的工具库
@@ -91,27 +91,27 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：ayugespidertools cli 的名称也可用 ayuge 来代替，输入体验更友好。
+# 注：更推荐使用 ayuge 的 cli 名称，输入体验更友好，（ayugespidertools 的 cli 则会在下一大版本中会剔除）。
 
 # 查看库版本
-ayugespidertools version
+ayuge version
 
 # 创建项目
-ayugespidertools startproject <project_name>
+ayuge startproject <project_name>
 
 # 进入项目根目录
 cd <project_name>
 
 # 生成爬虫脚本
-ayugespidertools genspider <spider_name> <example.com>
+ayuge genspider <spider_name> <example.com>
 
 # 替换(覆盖)为真实的配置 .conf 文件；
 # 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 运行脚本
 scrapy crawl <spider_name>
@@ -188,14 +188,15 @@
 
 ### 3.2. 你可能在意的事
 
 > 此项目会慢慢丰富 `python` 开发中的遇到的通用方法，详情请见 [TodoList](#TodoList)。
 
 1. 若你觉得某些场景下的功能实现不太符合你的预期，想要修改或添加自定义功能，或移除对你无用模块、修改库名等，你可以自行修改后 `build`。
 2. 本库主推 `scrapy` 扩展（即增强版的自定义模板）的功能，在使用本库时，理论上并不会影响你 `scrapy` 项目及其它组件，且你也可以根据上条须知来增强此库功能。因为模板功能天生就有及其明确的优缺点，我无法覆盖所有应用场景，**但是它的高效率的确会解放双手**。
+3. **当然，你也可以选择给此项目做出贡献，比如增加或优化某些功能等，但在此之前请提相关的 `ISSUES` 经确认后再开发和提交 `PULL REQUESTS`，以免不太符合本库场景或已废弃等原因造成你的贡献浪费，那就太可惜了！**
 
 ### 3.3. Build-Your-Own-Library
 
 > 具体内容请以 [poetry 官方文档](https://python-poetry.org/docs/) 为准。
 
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
```

