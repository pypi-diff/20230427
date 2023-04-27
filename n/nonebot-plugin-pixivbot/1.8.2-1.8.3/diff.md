# Comparing `tmp/nonebot_plugin_pixivbot-1.8.2.tar.gz` & `tmp/nonebot_plugin_pixivbot-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pixivbot-1.8.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_pixivbot-1.8.3.tar", max compression
```

## Comparing `nonebot_plugin_pixivbot-1.8.2.tar` & `nonebot_plugin_pixivbot-1.8.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.2/LICENSE
--rw-r--r--   0        0        0     1825 2023-04-26 10:41:59.754033 nonebot_plugin_pixivbot-1.8.2/pyproject.toml
--rw-r--r--   0        0        0    17350 2023-04-26 10:41:42.613891 nonebot_plugin_pixivbot-1.8.2/README.md
--rw-r--r--   0        0        0     1192 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/__init__.py
--rw-r--r--   0        0        0     7747 2023-04-26 10:41:42.786890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/config.py
--rw-r--r--   0        0        0     4322 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/context.py
--rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/__init__.py
--rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/errors.py
--rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
--rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
--rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/base.py
--rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
--rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
--rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
--rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
--rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
--rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
--rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
--rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
--rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
--rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
--rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
--rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
--rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
--rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
--rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
--rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
--rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
--rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
--rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
--rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
--rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
--rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
--rw-r--r--   0        0        0    19437 2023-04-26 10:41:42.824894 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
--rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
--rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
--rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
--rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
--rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
--rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
--rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
--rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
--rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
--rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
--rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
--rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
--rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
--rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
--rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
--rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
--rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
--rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/base.py
--rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
--rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/sql.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/__init__.py
--rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
--rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
--rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
--rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
--rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/base.py
--rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
--rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
--rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/enums.py
--rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/global_context.py
--rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/__init__.py
--rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/base.py
--rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/__init__.py
--rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/bind.py
--rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/command.py
--rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/help.py
--rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
--rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/schedule.py
--rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
--rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/watch.py
--rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/__init__.py
--rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/base.py
--rw-r--r--   0        0        0     1629 2023-04-26 11:11:55.420381 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/illust.py
--rw-r--r--   0        0        0     1440 2023-04-26 11:20:41.831066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/more.py
--rw-r--r--   0        0        0     2817 2023-04-26 11:20:41.858064 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
--rw-r--r--   0        0        0     1752 2023-04-26 11:20:41.846065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
--rw-r--r--   0        0        0     1599 2023-04-26 11:20:41.862066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
--rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
--rw-r--r--   0        0        0     2089 2023-04-26 11:20:41.819065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
--rw-r--r--   0        0        0     4204 2023-04-26 11:20:41.854065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/ranking.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
--rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
--rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
--rw-r--r--   0        0        0     1380 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
--rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
--rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
--rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
--rw-r--r--   0        0        0      919 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
--rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
--rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
--rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/pkg_context.py
--rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/recorder.py
--rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
--rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/base.py
--rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
--rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
--rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
--rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
--rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
--rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
--rw-r--r--   0        0        0     1011 2023-04-26 11:20:41.843065 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
--rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/utils.py
--rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
--rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/base.py
--rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
--rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
--rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/identifier.py
--rw-r--r--   0        0        0     1786 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/illust.py
--rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/interval_task.py
--rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_message.py
--rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/__init__.py
--rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
--rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/subscription.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
--rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/subscription.py
--rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/tag.py
--rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/user.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/user_preview.py
--rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/watch_task.py
--rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/plugin_service.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
--rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
--rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
--rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/__init__.py
--rw-r--r--   0        0        0     5469 2023-04-26 11:26:09.322980 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
--rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
--rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_service.py
--rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/roulette.py
--rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/scheduler.py
--rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/watchman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/__init__.py
--rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/algorithm.py
--rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/coros.py
--rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/decode_integer.py
--rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/errors.py
--rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
--rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/format.py
--rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
--rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lifecycler.py
--rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/nonebot.py
--rw-r--r--   0        0        0     8753 2023-03-15 03:26:56.198873 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/shared_agen.py
--rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/__init__.py
--rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/config.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
--rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
--rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
--rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
--rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/config.py
--rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
--rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     4845 2023-03-14 09:12:27.162624 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     3346 2023-04-26 10:41:42.753891 nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
--rw-r--r--   0        0        0    18886 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.8.3/LICENSE
+-rw-r--r--   0        0        0     1825 2023-04-27 09:46:24.103248 nonebot_plugin_pixivbot-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0    17274 2023-04-27 09:52:32.622538 nonebot_plugin_pixivbot-1.8.3/README.md
+-rw-r--r--   0        0        0     1192 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/__init__.py
+-rw-r--r--   0        0        0     7793 2023-04-27 09:37:04.739003 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/config.py
+-rw-r--r--   0        0        0     4322 2023-04-26 10:41:42.734890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/context.py
+-rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/__init__.py
+-rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/errors.py
+-rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
+-rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/base.py
+-rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
+-rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
+-rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
+-rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
+-rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
+-rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
+-rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
+-rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
+-rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
+-rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
+-rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
+-rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
+-rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
+-rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
+-rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
+-rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
+-rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
+-rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
+-rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
+-rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
+-rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
+-rw-r--r--   0        0        0    18860 2023-04-27 09:37:04.734003 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
+-rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/__init__.py
+-rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
+-rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
+-rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
+-rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
+-rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
+-rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
+-rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
+-rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
+-rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
+-rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
+-rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
+-rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
+-rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
+-rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
+-rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
+-rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/base.py
+-rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
+-rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/sql.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
+-rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
+-rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
+-rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/base.py
+-rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
+-rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
+-rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/enums.py
+-rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/global_context.py
+-rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/__init__.py
+-rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/base.py
+-rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/__init__.py
+-rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/bind.py
+-rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/command.py
+-rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/help.py
+-rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
+-rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/schedule.py
+-rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
+-rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/watch.py
+-rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/__init__.py
+-rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/base.py
+-rw-r--r--   0        0        0     1629 2023-04-26 11:11:55.420381 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/illust.py
+-rw-r--r--   0        0        0     1440 2023-04-26 11:20:41.831066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/more.py
+-rw-r--r--   0        0        0     2817 2023-04-26 11:20:41.858064 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
+-rw-r--r--   0        0        0     1752 2023-04-26 11:20:41.846065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
+-rw-r--r--   0        0        0     1599 2023-04-26 11:20:41.862066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
+-rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
+-rw-r--r--   0        0        0     2089 2023-04-26 11:20:41.819065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
+-rw-r--r--   0        0        0     4204 2023-04-26 11:20:41.854065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/ranking.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
+-rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
+-rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
+-rw-r--r--   0        0        0     1380 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
+-rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
+-rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
+-rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
+-rw-r--r--   0        0        0      919 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
+-rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
+-rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
+-rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/pkg_context.py
+-rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/recorder.py
+-rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/base.py
+-rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
+-rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
+-rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
+-rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
+-rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
+-rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
+-rw-r--r--   0        0        0     1011 2023-04-26 11:20:41.843065 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
+-rw-r--r--   0        0        0     1382 2023-02-13 05:42:01.863870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/utils.py
+-rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/base.py
+-rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
+-rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
+-rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/__init__.py
+-rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/identifier.py
+-rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/illust.py
+-rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/interval_task.py
+-rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/__init__.py
+-rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_message.py
+-rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/__init__.py
+-rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
+-rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/subscription.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
+-rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/subscription.py
+-rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/tag.py
+-rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/user.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/user_preview.py
+-rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/watch_task.py
+-rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/plugin_service.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
+-rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
+-rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
+-rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/__init__.py
+-rw-r--r--   0        0        0     5469 2023-04-26 11:26:09.322980 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
+-rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
+-rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_service.py
+-rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/roulette.py
+-rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/scheduler.py
+-rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/watchman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/__init__.py
+-rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/algorithm.py
+-rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/coros.py
+-rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/decode_integer.py
+-rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/errors.py
+-rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
+-rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/format.py
+-rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
+-rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lifecycler.py
+-rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/nonebot.py
+-rw-r--r--   0        0        0     8753 2023-03-15 03:26:56.198873 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/shared_agen.py
+-rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/config.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
+-rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
+-rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
+-rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/config.py
+-rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
+-rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
+-rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
+-rw-r--r--   0        0        0     4845 2023-04-27 09:44:58.747904 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
+-rw-r--r--   0        0        0     4048 2023-04-27 09:45:35.643691 nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
+-rw-r--r--   0        0        0    18812 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.8.3/PKG-INFO
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/LICENSE` & `nonebot_plugin_pixivbot-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/pyproject.toml` & `nonebot_plugin_pixivbot-1.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-pixivbot"
-version = "1.8.2"
+version = "1.8.3"
 description = "Nonebot Plugin PixivBot"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-pixivbot"
 packages = [
     { include = "nonebot_plugin_pixivbot", from = "src" },
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/README.md` & `nonebot_plugin_pixivbot-1.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,20 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-pixivbot.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 </p>
 
 NoneBot插件，支持发送随机Pixiv插画、画师更新推送、定时订阅推送……
 
-## 开始使用
-
 适配协议：
 
 - [Onebot V11](https://onebot.adapters.nonebot.dev/)
 - [KOOK / 开黑啦](https://github.com/Tian-que/nonebot-adapter-kaiheila)
 - [Telegram](https://github.com/nonebot/adapter-telegram)
 
-没有找到需要的协议？欢迎适配。[适配指南](https://github.com/ssttkkl/nonebot-plugin-pixivbot/wiki/%E9%80%82%E9%85%8D%E6%8C%87%E5%8D%97)
-
-开箱即用的Docker镜像：[ssttkkl/PixivBot](https://github.com/ssttkkl/PixivBot)
-
 ## 触发语句
 
 ### 普通语句
 
 所有数字参数均支持中文数字和罗马数字。
 
 - **看看<类型>榜<范围>**：查看pixiv榜单（<类型>可省略，<范围>应为a-b或a）
@@ -173,15 +167,17 @@
 /ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
 ```
 
 具体可以参考[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)的文档进行权限控制。
 
 ## 常见问题
 
-**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**
+**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
+
+Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
 
 ### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
 
 没登录成功，多半是网络问题
 
 如果登录成功的话会在bot初始化后有这几句：
 
@@ -227,18 +223,20 @@
 pixiv_query_to_me_only=False  # 只响应关于Bot的查询
 pixiv_command_to_me_only=False  # 只响应关于Bot的命令
 
 pixiv_max_item_per_query=10  # 每个查询最多请求的插画数量
 
 pixiv_tag_translation_enabled=True  # 启用搜索关键字翻译功能（平时搜索时记录标签翻译，在查询时判断是否存在对应中日翻译）
 
-pixiv_block_tags=[]  # 当插画含有指定tag时会被过滤
-pixiv_block_action=no_image  # 过滤时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
+pixiv_block_tags=[]  # 当插画含有指定tag时会被阻拦
+pixiv_block_action=no_image  # 阻拦时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
+
+pixiv_exclude_ai_illusts=False  # 是否过滤AI绘图作品
 
-pixiv_watch_interval=7200  # 更新推送的查询间隔
+pixiv_watch_interval=600  # 更新推送的查询间隔（单位：秒）
 
 # 插画压缩
 pixiv_compression_enabled=False  # 启用插画压缩
 pixiv_compression_max_size=  # 插画压缩最大尺寸
 pixiv_compression_quantity=  # 插画压缩品质（0到100）
 
 # 缓存过期时间/删除时间（单位：秒）
@@ -253,15 +251,15 @@
 pixiv_user_illusts_cache_expires_in=86400
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400
 pixiv_other_cache_expires_in=21600
 
-# OneBot平台（主要是gocq）配置
+# QQ平台（主要是gocq）配置
 pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
 pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
 pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
 
 # 功能配置
 pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
 pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
```

#### html2text {}

```diff
@@ -1,18 +1,14 @@
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
-## å¼å§ä½¿ç¨ ééåè®®ï¼ - [Onebot V11](https://
-onebot.adapters.nonebot.dev/) - [KOOK / å¼é»å¦](https://github.com/Tian-que/
-nonebot-adapter-kaiheila) - [Telegram](https://github.com/nonebot/adapter-
-telegram) æ²¡ææ¾å°éè¦çåè®®ï¼æ¬¢è¿ééã[ééæå](https://
-github.com/ssttkkl/nonebot-plugin-pixivbot/wiki/
-%E9%80%82%E9%85%8D%E6%8C%87%E5%8D%97) å¼ç®±å³ç¨çDockeréåï¼[ssttkkl/
-PixivBot](https://github.com/ssttkkl/PixivBot) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
+ééåè®®ï¼ - [Onebot V11](https://onebot.adapters.nonebot.dev/) - [KOOK /
+å¼é»å¦](https://github.com/Tian-que/nonebot-adapter-kaiheila) - [Telegram]
+(https://github.com/nonebot/adapter-telegram) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
 æææ°å­åæ°åæ¯æä¸­ææ°å­åç½é©¬æ°å­ã -
 **çç<ç±»å>æ¦<èå´>**ï¼æ¥çpixivæ¦åï¼<ç±»å>å¯çç¥ï¼<èå´>åºä¸ºa-
 bæaï¼ - ç¤ºä¾ï¼ççæ¦ãççæ¥æ¦ãççæ¦1-5ãççææ¦ä¸ -
 **æ¥<æ°é>å¼ å¾**ï¼ä»æ¨èæç»éæºæ½éä¸å¼ æç»ï¼<æ°é>å¯çç¥ï¼ä¸åï¼
 - ç¤ºä¾ï¼æ¥å¼ å¾ãæ¥äºå¼ å¾ -
 **æ¥<æ°é>å¼ <å³é®å­>å¾**ï¼æç´¢å³é®å­ï¼ä»æç´¢ç»æéæºæ½éä¸å¼ æç»
 - ç¤ºä¾ï¼æ¥å¼ åé³ãã¯å¾ãæ¥äºå¼ åé³ãã¯å¾ -
@@ -113,15 +109,17 @@
 srv nonebot_plugin_pixivbot.schedule.manage --sbj all /ac permission allow --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private /ac permission
 allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin /ac
 permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
 ``` å·ä½å¯ä»¥åè[nonebot-plugin-access-control](https://github.com/
 ssttkkl/nonebot-plugin-access-control)çææ¡£è¿è¡æéæ§å¶ã ##
 å¸¸è§é®é¢ **éå°é®é¢æ¶è¯·åå°è¯æ§è¡`pip install nonebot-plugin-
-pixivbot -U`æ´æ°å°ææ°çæ¬** ### åé¨éè¯¯ï¼
+pixivbot -U`æ´æ°å°ææ°çæ¬**ã
+Issueè¯·å°½å¯è½å¸¦ä¸è¯¦ç»çæ¥å¿ãéç½®æä»¶ä¸ç¯å¢ä¿¡æ¯ãåè½è¯·æ±è¯·ç§»æ­¥Discussionã
+### åé¨éè¯¯ï¼
 pixivpy_async.error.NoTokenError'>No access_token Found!
 æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢
 å¦æç»å½æåçè¯ä¼å¨botåå§ååæè¿å å¥ï¼ ``` 03-13 11:19:36
 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new
 token expires in 3600 seconds. 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 access_token: *************** 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 refresh_token: ***************** ``` ### åé¨éè¯¯ï¼
@@ -145,20 +143,22 @@
 pixiv_simultaneous_query=8 # åPixivæ¥è¯¢çå¹¶åæ°
 pixiv_download_custom_domain= # ä½¿ç¨ååä»£çä¸è½½æç»çåå #
 æ¥è¯¢è®¾ç½® pixiv_query_to_me_only=False # åªååºå³äºBotçæ¥è¯¢
 pixiv_command_to_me_only=False # åªååºå³äºBotçå½ä»¤
 pixiv_max_item_per_query=10 # æ¯ä¸ªæ¥è¯¢æå¤è¯·æ±çæç»æ°é
 pixiv_tag_translation_enabled=True #
 å¯ç¨æç´¢å³é®å­ç¿»è¯åè½ï¼å¹³æ¶æç´¢æ¶è®°å½æ ç­¾ç¿»è¯ï¼å¨æ¥è¯¢æ¶å¤æ­æ¯å¦å­å¨å¯¹åºä¸­æ¥ç¿»è¯ï¼
-pixiv_block_tags=[] # å½æç»å«ææå®tagæ¶ä¼è¢«è¿æ»¤
-pixiv_block_action=no_image # è¿æ»¤æ¶çå¨ä½ï¼å¯éå¼ï¼no_image
+pixiv_block_tags=[] # å½æç»å«ææå®tagæ¶ä¼è¢«é»æ¦
+pixiv_block_action=no_image # é»æ¦æ¶çå¨ä½ï¼å¯éå¼ï¼no_image
 (ä¸æ¾ç¤ºæç»ï¼åå¤æç»ä¿¡æ¯), completely_block
-(åªåå¤è¿æ»¤æç¤º), no_reply(æ åå¤) pixiv_watch_interval=7200 #
-æ´æ°æ¨éçæ¥è¯¢é´é # æç»åç¼© pixiv_compression_enabled=False #
-å¯ç¨æç»åç¼© pixiv_compression_max_size= # æç»åç¼©æå¤§å°ºå¯¸
+(åªåå¤è¿æ»¤æç¤º), no_reply(æ åå¤) pixiv_exclude_ai_illusts=False #
+æ¯å¦è¿æ»¤AIç»å¾ä½å pixiv_watch_interval=600 #
+æ´æ°æ¨éçæ¥è¯¢é´éï¼åä½ï¼ç§ï¼ # æç»åç¼©
+pixiv_compression_enabled=False # å¯ç¨æç»åç¼©
+pixiv_compression_max_size= # æç»åç¼©æå¤§å°ºå¯¸
 pixiv_compression_quantity= # æç»åç¼©åè´¨ï¼0å°100ï¼ #
 ç¼å­è¿ææ¶é´/å é¤æ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_download_cache_expires_in=604800 # é»è®¤å¼ï¼7å¤©
 pixiv_illust_detail_cache_expires_in=604800
 pixiv_user_detail_cache_expires_in=604800
 pixiv_illust_ranking_cache_expires_in=21600 # é»è®¤å¼ï¼6å°æ¶
 pixiv_search_illust_cache_expires_in=86400 # é»è®¤å¼ï¼1å¤©
@@ -166,17 +166,16 @@
 pixiv_search_user_cache_expires_in=86400
 pixiv_search_user_cache_delete_in=2592000
 pixiv_user_illusts_cache_expires_in=86400
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400 pixiv_other_cache_expires_in=21600
-# OneBotå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½®
-pixiv_poke_action=random_recommended_illust #
-ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
+# QQå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½® pixiv_poke_action=random_recommended_illust
+# ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
 pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
 pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/config.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,16 @@
     pixiv_user_bookmarks_cache_delete_in = 3600 * 24 * 30
     pixiv_related_illusts_cache_expires_in = 3600 * 24
     pixiv_other_cache_expires_in = 3600 * 6
 
     pixiv_block_tags: List[str] = []
     pixiv_block_action: BlockAction = BlockAction.no_image
 
+    pixiv_exclude_ai_illusts: bool = False
+
     pixiv_download_custom_domain: Optional[str]
 
     pixiv_compression_enabled: bool = False
     pixiv_compression_max_size: Optional[int]
     pixiv_compression_quantity: Optional[float]
 
     # 不加allow_reuse跑pytest会报错
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/context.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/context.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/interval_task_repo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/interval_task_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/local_tag/sql.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/local_tag/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from asyncio import sleep, create_task, CancelledError, Semaphore, Task
 from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 from io import BytesIO
 from typing import TypeVar, Optional, Awaitable, List, Callable, Tuple, AsyncGenerator, Union
 
+from cachetools.func import rr_cache
 from nonebot import logger
 from pixivpy_async import *
 from pixivpy_async.error import TokenError
 
 from nonebot_plugin_pixivbot.config import Config
 from nonebot_plugin_pixivbot.enums import RankingMode
 from nonebot_plugin_pixivbot.global_context import context
@@ -134,14 +135,35 @@
     async def _load_raw_page(self, papi_search_func: Callable[..., Awaitable[dict]],
                              **kwargs):
         async with self._query():
             raw_result = await papi_search_func(**kwargs)
             self._check_error_in_raw_result(raw_result)
             return raw_result
 
+    @staticmethod
+    @rr_cache()  # 因为size足够就不会发生替换，所以缓存用random replacement算法最快
+    def _make_illust_filter(min_view: int = 2 ** 31 - 1, min_bookmark: int = 2 ** 31 - 1):
+        def illust_filter(illust: Illust) -> bool:
+            # 标签过滤
+            for tag in _conf.pixiv_block_tags:
+                if illust.has_tag(tag):
+                    return False
+            # 书签下限过滤
+            if illust.total_bookmarks < min_bookmark:
+                return False
+            # 浏览量下限过滤
+            if illust.total_view < min_view:
+                return False
+            # AI过滤
+            if _conf.pixiv_exclude_ai_illusts and illust.illust_ai_type != 0:
+                return False
+            return True
+
+        return illust_filter
+
     async def _load_page(self, papi_search_func: Callable[..., Awaitable[dict]],
                          element_list_name: str,
                          *, mapper: Optional[Callable[[dict], T]] = None,
                          filter_item: Optional[Callable[[T], bool]] = None,
                          **kwargs) -> Tuple[List[T], PixivRepoMetadata]:
         """
         加载一页
@@ -200,80 +222,55 @@
                 if 'viewed' in next_qs:
                     # 由于pixivpy-async的illust_recommended的bug，需要删掉这个参数
                     del next_qs['viewed']
             else:
                 break
 
     async def _get_illusts(self, papi_search_func: Callable[[], Awaitable[dict]],
-                           *, block_tags: Optional[List[str]] = None,
-                           min_bookmark: int = 0,
+                           *, min_bookmark: int = 0,
                            min_view: int = 0,
                            **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         """
         加载插画
         :param papi_search_func: PixivPy-Async的加载方法
-        :param block_tags: 要过滤的标签
         :param min_bookmark: 书签数下限
         :param min_view: 阅读数下限
         :param kwargs: 传给papi_search_func的参数
         :return:
         """
-
-        def illust_filter(illust: Illust) -> bool:
-            # 标签过滤
-            if block_tags is not None:
-                for tag in block_tags:
-                    if illust.has_tag(tag):
-                        return False
-            # 书签下限过滤
-            if illust.total_bookmarks < min_bookmark:
-                return False
-            # 浏览量下限过滤
-            if illust.total_view < min_view:
-                return False
-            return True
-
         total = 0
         broken = 0
 
         try:
             yield PixivRepoMetadata(pages=0, next_qs=kwargs)
             async for page, metadata in self._load_many_pages(papi_search_func, "illusts",
                                                               mapper=lambda x: Illust.parse_obj(x),
-                                                              filter_item=illust_filter, **kwargs):
+                                                              filter_item=self._make_illust_filter(min_view,
+                                                                                                   min_bookmark),
+                                                              **kwargs):
                 for item in page:
                     total += 1
                     if "limit_unknown_360.png" in item.image_urls.large:
                         broken += 1
                         yield LazyIllust(item.id)
                     else:
                         yield LazyIllust(item.id, item)
                 yield metadata
         finally:
             logger.debug(f"[remote] got {total} illusts, illust_detail of {broken} are missed")
 
-    async def _get_user_previews(self, papi_search_func: Callable[[], Awaitable[dict]],
-                                 *, block_tags: Optional[List[str]] = None,
-                                 **kwargs) \
+    async def _get_user_previews(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
             -> AsyncGenerator[Union[PixivRepoMetadata, UserPreview], None]:
         yield PixivRepoMetadata(pages=0, next_qs=kwargs)
         async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
                                                           mapper=lambda x: UserPreview.parse_obj(x), **kwargs):
             for item in page:
                 item: UserPreview
-                if block_tags is not None:
-                    illusts = []
-                    for x in item.illusts:
-                        for tag in block_tags:
-                            if x.has_tag(tag):
-                                break
-                        else:
-                            illusts.append(x)
-                    item.illusts = illusts
+                item.illusts = list(filter(self._make_illust_filter(), item.illusts))
                 yield item
             yield metadata
 
     async def _get_users(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
             -> AsyncGenerator[Union[PixivRepoMetadata, User], None]:
         yield PixivRepoMetadata(pages=0, next_qs=kwargs)
         async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
@@ -306,101 +303,92 @@
         yield PixivRepoMetadata()
         yield User.parse_obj(raw_result["user"])
 
     def search_illust(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[remote] search_illust {word}")
         return self._get_illusts(self._papi.search_illust,
-                                 block_tags=_conf.pixiv_block_tags,
                                  min_bookmark=_conf.pixiv_random_illust_min_bookmark,
                                  min_view=_conf.pixiv_random_illust_min_view,
                                  word=word, **kwargs)
 
     def search_user(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
         logger.debug(f"[remote] search_user {word}")
         return self._get_users(self._papi.search_user,
                                word=word, **kwargs)
 
     def search_user_with_preview(self, word: str, **kwargs) \
             -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
         logger.debug(f"[remote] search_user {word}")
         return self._get_user_previews(self._papi.search_user,
-                                       block_tags=_conf.pixiv_block_tags,
                                        word=word, **kwargs)
 
     def user_following(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
         logger.debug(f"[remote] following_users {user_id}")
         return self._get_users(self._papi.user_following,
                                user_id=user_id, **kwargs)
 
     def user_following_with_preview(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
         logger.debug(f"[remote] following_users {user_id}")
         return self._get_user_previews(self._papi.user_following,
-                                       block_tags=_conf.pixiv_block_tags,
                                        user_id=user_id, **kwargs)
 
     def user_illusts(self, user_id: int, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[remote] user_illusts {user_id}")
         return self._get_illusts(self._papi.user_illusts,
-                                 block_tags=_conf.pixiv_block_tags,
                                  min_bookmark=_conf.pixiv_random_user_illust_min_bookmark,
                                  min_view=_conf.pixiv_random_user_illust_min_view,
                                  user_id=user_id, **kwargs)
 
     def user_bookmarks(self, user_id: int = 0, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if user_id == 0:
             user_id = self.user_id
 
         logger.debug(f"[remote] user_bookmarks {user_id}")
         return self._get_illusts(self._papi.user_bookmarks_illust,
-                                 block_tags=_conf.pixiv_block_tags,
                                  min_bookmark=_conf.pixiv_random_bookmark_min_bookmark,
                                  min_view=_conf.pixiv_random_bookmark_min_view,
                                  user_id=user_id, **kwargs)
 
     # def following_illusts(self, **kwargs) \
     #         -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
     #     logger.debug(f"[remote] following_illusts")
     #     return self._get_illusts(self._papi.illust_follow,
-    #                              block_tags=_conf.pixiv_block_tags,
     #                              min_bookmark=_conf.pixiv_random_following_illust_min_bookmark,
     #                              min_view=_conf.pixiv_random_following_illust_min_view,
     #                              **kwargs)
 
     def recommended_illusts(self, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[remote] recommended_illusts")
         return self._get_illusts(self._papi.illust_recommended,
-                                 block_tags=_conf.pixiv_block_tags,
                                  min_bookmark=_conf.pixiv_random_recommended_illust_min_bookmark,
                                  min_view=_conf.pixiv_random_recommended_illust_min_view,
                                  **kwargs)
 
     def related_illusts(self, illust_id: int, **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[remote] related_illusts {illust_id}")
         return self._get_illusts(self._papi.illust_related,
-                                 block_tags=_conf.pixiv_block_tags,
                                  min_bookmark=_conf.pixiv_random_related_illust_min_bookmark,
                                  min_view=_conf.pixiv_random_related_illust_min_view,
                                  illust_id=illust_id, **kwargs)
 
     def illust_ranking(self, mode: Union[str, RankingMode], **kwargs) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         if isinstance(mode, str):
             mode = RankingMode[mode]
 
         logger.debug(f"[remote] illust_ranking {mode}")
         return self._get_illusts(self._papi.illust_ranking,
-                                 block_tags=_conf.pixiv_block_tags,
                                  mode=mode.name, **kwargs)
 
     async def _raw_image(self, illust: Illust, page: int, **kwargs) -> bytes:
         custom_domain = _conf.pixiv_download_custom_domain
 
         url = illust.page_image_url(page)
         if custom_domain is not None:
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/migration_manager.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/migration_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/mongo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/subscription/sql.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/utils/sql.pyi` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/utils/sql.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/data/watch_task/sql.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/data/watch_task/sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/enums.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/enums.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/bind.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/command.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/help.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/schedule.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/schedule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/subcommand.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/command/watch.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/command/watch.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/more.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/more.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/common/ranking.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/common/ranking.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/recorder.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/recorder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/utils.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/base.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/__init__.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/identifier.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/identifier.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/illust.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/illust.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     tags: typing.List[Tag]
     create_date: datetime.datetime
     page_count: int
     meta_single_page: MetaSinglePage
     meta_pages: typing.List[MetaPage]
     total_view: int
     total_bookmarks: int
+    illust_ai_type: int = 0  # 0为非AI作品，其他暂时不知道
 
     def has_tag(self, tag: typing.Union[str, Tag]) -> bool:
         if isinstance(tag, Tag):
             for x in self.tags:
                 if x == tag:
                     return True
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_message.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/message/illust_messages.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/message/illust_messages.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/old/subscription.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/old/subscription.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/subscription.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/subscription.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/model/watch_task.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/model/watch_task.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/plugin_service.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/plugin_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/interval_task_worker.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/interval_task_worker.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/pixiv_service.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/pixiv_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/roulette.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/roulette.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/scheduler.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/service/watchman.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/service/watchman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/decode_integer.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/errors.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/lifecycler.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/lifecycler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/nonebot.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot/utils/shared_agen.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot/utils/shared_agen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/config.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/config.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.8.2/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py` & `nonebot_plugin_pixivbot-1.8.3/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+from contextlib import asynccontextmanager
 from io import StringIO
 
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot import logger
+from nonebot.adapters.onebot.v11 import Message, MessageSegment, ActionFailed
 
 from nonebot_plugin_pixivbot.enums import BlockAction
 from nonebot_plugin_pixivbot.global_context import context
 from nonebot_plugin_pixivbot.model.message import IllustMessageModel, IllustMessagesModel
 from nonebot_plugin_pixivbot.protocol_dep.postman import Postman as BasePostman, PostmanManager
 from nonebot_plugin_pixivbot_onebot_v11.config import OnebotV11Config
 from nonebot_plugin_pixivbot_onebot_v11.protocol_dep.post_dest import PostDestination
 
 conf = context.require(OnebotV11Config)
 
 
+@asynccontextmanager
+async def feedback_on_action_failed(post_dest: PostDestination):
+    try:
+        yield
+    except ActionFailed as e:
+        logger.error("图片发送失败，可能是机器人被风控")
+        logger.error(e)
+
+        await post_dest.post_single(Message([MessageSegment.text("图片发送失败，可能是机器人被风控")]))
+
+
 @context.register_singleton()
 class Postman(BasePostman[int, int], manager=PostmanManager):
     adapter = "onebot"
 
     def make_illust_msg(self, model: IllustMessageModel) -> Message:
         msg = Message()
 
@@ -50,36 +63,39 @@
                 sio.write(f"Pixiv ID：{model.id}")
 
             msg.append(MessageSegment.text(sio.getvalue()))
         return msg
 
     async def send_plain_text(self, message: str,
                               *, post_dest: PostDestination):
-        message = Message([MessageSegment.text(message)])
-        await post_dest.post(message)
+        async with feedback_on_action_failed(post_dest):
+            message = Message([MessageSegment.text(message)])
+            await post_dest.post(message)
 
     async def send_illust(self, model: IllustMessageModel,
                           *, post_dest: PostDestination):
-        message = Message()
-        if model.header is not None:
-            message.append(MessageSegment.text(model.header + '\n'))
+        async with feedback_on_action_failed(post_dest):
+            message = Message()
+            if model.header is not None:
+                message.append(MessageSegment.text(model.header + '\n'))
 
-        message.extend(self.make_illust_msg(model))
-        await post_dest.post(message)
+            message.extend(self.make_illust_msg(model))
+            await post_dest.post(message)
 
     async def send_illusts(self, model: IllustMessagesModel,
                            *, post_dest: PostDestination):
-        if conf.pixiv_onebot_send_forward_message == 'never' or \
-                conf.pixiv_onebot_send_forward_message == 'auto' and len(model.messages) == 1:
-            for x in model.flat():
-                await self.send_illust(x, post_dest=post_dest)
-        else:
-            messages = []
-            if model.header:
-                messages.append(Message([MessageSegment.text(model.header)]))
-            for sub_model in model.messages:
-                messages.append(self.make_illust_msg(sub_model))
+        async with feedback_on_action_failed(post_dest):
+            if conf.pixiv_onebot_send_forward_message == 'never' or \
+                    conf.pixiv_onebot_send_forward_message == 'auto' and len(model.messages) == 1:
+                for x in model.flat():
+                    await self.send_illust(x, post_dest=post_dest)
+            else:
+                messages = []
+                if model.header:
+                    messages.append(Message([MessageSegment.text(model.header)]))
+                for sub_model in model.messages:
+                    messages.append(self.make_illust_msg(sub_model))
 
-            await post_dest.post(messages)
+                await post_dest.post(messages)
 
 
 __all__ = ("Postman",)
```

### Comparing `nonebot_plugin_pixivbot-1.8.2/PKG-INFO` & `nonebot_plugin_pixivbot-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pixivbot
-Version: 1.8.2
+Version: 1.8.3
 Summary: Nonebot Plugin PixivBot
 Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -65,26 +65,20 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-pixivbot.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 </p>
 
 NoneBot插件，支持发送随机Pixiv插画、画师更新推送、定时订阅推送……
 
-## 开始使用
-
 适配协议：
 
 - [Onebot V11](https://onebot.adapters.nonebot.dev/)
 - [KOOK / 开黑啦](https://github.com/Tian-que/nonebot-adapter-kaiheila)
 - [Telegram](https://github.com/nonebot/adapter-telegram)
 
-没有找到需要的协议？欢迎适配。[适配指南](https://github.com/ssttkkl/nonebot-plugin-pixivbot/wiki/%E9%80%82%E9%85%8D%E6%8C%87%E5%8D%97)
-
-开箱即用的Docker镜像：[ssttkkl/PixivBot](https://github.com/ssttkkl/PixivBot)
-
 ## 触发语句
 
 ### 普通语句
 
 所有数字参数均支持中文数字和罗马数字。
 
 - **看看<类型>榜<范围>**：查看pixiv榜单（<类型>可省略，<范围>应为a-b或a）
@@ -217,15 +211,17 @@
 /ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
 ```
 
 具体可以参考[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)的文档进行权限控制。
 
 ## 常见问题
 
-**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**
+**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
+
+Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
 
 ### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
 
 没登录成功，多半是网络问题
 
 如果登录成功的话会在bot初始化后有这几句：
 
@@ -271,18 +267,20 @@
 pixiv_query_to_me_only=False  # 只响应关于Bot的查询
 pixiv_command_to_me_only=False  # 只响应关于Bot的命令
 
 pixiv_max_item_per_query=10  # 每个查询最多请求的插画数量
 
 pixiv_tag_translation_enabled=True  # 启用搜索关键字翻译功能（平时搜索时记录标签翻译，在查询时判断是否存在对应中日翻译）
 
-pixiv_block_tags=[]  # 当插画含有指定tag时会被过滤
-pixiv_block_action=no_image  # 过滤时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
+pixiv_block_tags=[]  # 当插画含有指定tag时会被阻拦
+pixiv_block_action=no_image  # 阻拦时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
+
+pixiv_exclude_ai_illusts=False  # 是否过滤AI绘图作品
 
-pixiv_watch_interval=7200  # 更新推送的查询间隔
+pixiv_watch_interval=600  # 更新推送的查询间隔（单位：秒）
 
 # 插画压缩
 pixiv_compression_enabled=False  # 启用插画压缩
 pixiv_compression_max_size=  # 插画压缩最大尺寸
 pixiv_compression_quantity=  # 插画压缩品质（0到100）
 
 # 缓存过期时间/删除时间（单位：秒）
@@ -297,15 +295,15 @@
 pixiv_user_illusts_cache_expires_in=86400
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400
 pixiv_other_cache_expires_in=21600
 
-# OneBot平台（主要是gocq）配置
+# QQ平台（主要是gocq）配置
 pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
 pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
 pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
 
 # 功能配置
 pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
 pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.8.3 Summary:
 Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
 pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: kook
 Provides-Extra: mongo Provides-Extra: onebot Provides-Extra: postgresql
@@ -24,21 +24,17 @@
 (>=1.0.9,<2.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Project-URL: Repository,
 https://github.com/ssttkkl/nonebot-plugin-pixivbot Description-Content-Type:
 text/markdown
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
-## å¼å§ä½¿ç¨ ééåè®®ï¼ - [Onebot V11](https://
-onebot.adapters.nonebot.dev/) - [KOOK / å¼é»å¦](https://github.com/Tian-que/
-nonebot-adapter-kaiheila) - [Telegram](https://github.com/nonebot/adapter-
-telegram) æ²¡ææ¾å°éè¦çåè®®ï¼æ¬¢è¿ééã[ééæå](https://
-github.com/ssttkkl/nonebot-plugin-pixivbot/wiki/
-%E9%80%82%E9%85%8D%E6%8C%87%E5%8D%97) å¼ç®±å³ç¨çDockeréåï¼[ssttkkl/
-PixivBot](https://github.com/ssttkkl/PixivBot) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
+ééåè®®ï¼ - [Onebot V11](https://onebot.adapters.nonebot.dev/) - [KOOK /
+å¼é»å¦](https://github.com/Tian-que/nonebot-adapter-kaiheila) - [Telegram]
+(https://github.com/nonebot/adapter-telegram) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
 æææ°å­åæ°åæ¯æä¸­ææ°å­åç½é©¬æ°å­ã -
 **çç<ç±»å>æ¦<èå´>**ï¼æ¥çpixivæ¦åï¼<ç±»å>å¯çç¥ï¼<èå´>åºä¸ºa-
 bæaï¼ - ç¤ºä¾ï¼ççæ¦ãççæ¥æ¦ãççæ¦1-5ãççææ¦ä¸ -
 **æ¥<æ°é>å¼ å¾**ï¼ä»æ¨èæç»éæºæ½éä¸å¼ æç»ï¼<æ°é>å¯çç¥ï¼ä¸åï¼
 - ç¤ºä¾ï¼æ¥å¼ å¾ãæ¥äºå¼ å¾ -
 **æ¥<æ°é>å¼ <å³é®å­>å¾**ï¼æç´¢å³é®å­ï¼ä»æç´¢ç»æéæºæ½éä¸å¼ æç»
 - ç¤ºä¾ï¼æ¥å¼ åé³ãã¯å¾ãæ¥äºå¼ åé³ãã¯å¾ -
@@ -139,15 +135,17 @@
 srv nonebot_plugin_pixivbot.schedule.manage --sbj all /ac permission allow --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private /ac permission
 allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin /ac
 permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
 ``` å·ä½å¯ä»¥åè[nonebot-plugin-access-control](https://github.com/
 ssttkkl/nonebot-plugin-access-control)çææ¡£è¿è¡æéæ§å¶ã ##
 å¸¸è§é®é¢ **éå°é®é¢æ¶è¯·åå°è¯æ§è¡`pip install nonebot-plugin-
-pixivbot -U`æ´æ°å°ææ°çæ¬** ### åé¨éè¯¯ï¼
+pixivbot -U`æ´æ°å°ææ°çæ¬**ã
+Issueè¯·å°½å¯è½å¸¦ä¸è¯¦ç»çæ¥å¿ãéç½®æä»¶ä¸ç¯å¢ä¿¡æ¯ãåè½è¯·æ±è¯·ç§»æ­¥Discussionã
+### åé¨éè¯¯ï¼
 pixivpy_async.error.NoTokenError'>No access_token Found!
 æ²¡ç»å½æåï¼å¤åæ¯ç½ç»é®é¢
 å¦æç»å½æåçè¯ä¼å¨botåå§ååæè¿å å¥ï¼ ``` 03-13 11:19:36
 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new
 token expires in 3600 seconds. 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 access_token: *************** 03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot |
 refresh_token: ***************** ``` ### åé¨éè¯¯ï¼
@@ -171,20 +169,22 @@
 pixiv_simultaneous_query=8 # åPixivæ¥è¯¢çå¹¶åæ°
 pixiv_download_custom_domain= # ä½¿ç¨ååä»£çä¸è½½æç»çåå #
 æ¥è¯¢è®¾ç½® pixiv_query_to_me_only=False # åªååºå³äºBotçæ¥è¯¢
 pixiv_command_to_me_only=False # åªååºå³äºBotçå½ä»¤
 pixiv_max_item_per_query=10 # æ¯ä¸ªæ¥è¯¢æå¤è¯·æ±çæç»æ°é
 pixiv_tag_translation_enabled=True #
 å¯ç¨æç´¢å³é®å­ç¿»è¯åè½ï¼å¹³æ¶æç´¢æ¶è®°å½æ ç­¾ç¿»è¯ï¼å¨æ¥è¯¢æ¶å¤æ­æ¯å¦å­å¨å¯¹åºä¸­æ¥ç¿»è¯ï¼
-pixiv_block_tags=[] # å½æç»å«ææå®tagæ¶ä¼è¢«è¿æ»¤
-pixiv_block_action=no_image # è¿æ»¤æ¶çå¨ä½ï¼å¯éå¼ï¼no_image
+pixiv_block_tags=[] # å½æç»å«ææå®tagæ¶ä¼è¢«é»æ¦
+pixiv_block_action=no_image # é»æ¦æ¶çå¨ä½ï¼å¯éå¼ï¼no_image
 (ä¸æ¾ç¤ºæç»ï¼åå¤æç»ä¿¡æ¯), completely_block
-(åªåå¤è¿æ»¤æç¤º), no_reply(æ åå¤) pixiv_watch_interval=7200 #
-æ´æ°æ¨éçæ¥è¯¢é´é # æç»åç¼© pixiv_compression_enabled=False #
-å¯ç¨æç»åç¼© pixiv_compression_max_size= # æç»åç¼©æå¤§å°ºå¯¸
+(åªåå¤è¿æ»¤æç¤º), no_reply(æ åå¤) pixiv_exclude_ai_illusts=False #
+æ¯å¦è¿æ»¤AIç»å¾ä½å pixiv_watch_interval=600 #
+æ´æ°æ¨éçæ¥è¯¢é´éï¼åä½ï¼ç§ï¼ # æç»åç¼©
+pixiv_compression_enabled=False # å¯ç¨æç»åç¼©
+pixiv_compression_max_size= # æç»åç¼©æå¤§å°ºå¯¸
 pixiv_compression_quantity= # æç»åç¼©åè´¨ï¼0å°100ï¼ #
 ç¼å­è¿ææ¶é´/å é¤æ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_download_cache_expires_in=604800 # é»è®¤å¼ï¼7å¤©
 pixiv_illust_detail_cache_expires_in=604800
 pixiv_user_detail_cache_expires_in=604800
 pixiv_illust_ranking_cache_expires_in=21600 # é»è®¤å¼ï¼6å°æ¶
 pixiv_search_illust_cache_expires_in=86400 # é»è®¤å¼ï¼1å¤©
@@ -192,17 +192,16 @@
 pixiv_search_user_cache_expires_in=86400
 pixiv_search_user_cache_delete_in=2592000
 pixiv_user_illusts_cache_expires_in=86400
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400 pixiv_other_cache_expires_in=21600
-# OneBotå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½®
-pixiv_poke_action=random_recommended_illust #
-ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
+# QQå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½® pixiv_poke_action=random_recommended_illust
+# ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
 pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
 pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
```

