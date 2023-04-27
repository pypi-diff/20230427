# Comparing `tmp/custard-1.1.1.tar.gz` & `tmp/custard-1.1.2.tar.gz`

## Comparing `custard-1.1.1.tar` & `custard-1.1.2.tar`

### file list

```diff
@@ -1,174 +1,175 @@
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.1/.vscode/launch.json
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 custard-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.1.1/custard/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/__init__.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/async_lru.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/async_lur.md
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cache/redis.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/__init__.py
--rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/decode.py
--rw-r--r--   0        0        0    28578 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/factory.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/kerberos.py
--rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/processor.py
--rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/regular.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/snowflake.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/system.py
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/useragent.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/xml2dict.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.1.1/custard/core/xprint.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cron/__init__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.1.1/custard/cron/batch_task.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.1.1/custard/crypto/streambody.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 custard-1.1.1/custard/curl/__init__.py
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 custard-1.1.1/custard/curl/parse.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/exc.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/inspect.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/logger.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.1.1/custard/db/utils.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/__init__.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/context.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/exceptions.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/record.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.1.1/custard/expect/spacer.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/extra/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/__init__.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/callsource.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.1.1/custard/function/traverse.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.1.1/custard/hitfilter/keywords
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.1.1/custard/json/__init__.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.1.1/custard/json/jsonlogger.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.1.1/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/depends.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/enums.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.1.1/custard/limiter/execres.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/__init__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/redis_lock.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lock/thread_lock.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/arrays.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/maths.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/number.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/string.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.1.1/custard/lodash/utilities.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/__init__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/aliyun.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/enums.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/gitee.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/minio.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/qiniu.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.1/custard/minioss/tencent.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/__init__.py
--rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.1.1/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/asynchttp.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/enums.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.1.1/custard/network/httpclient.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/api.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/bases.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/default.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/pagination.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/pio/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/__init__.py
--rw-r--r--   0        0        0    49439 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/client.py
--rw-r--r--   0        0        0    24730 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/connection.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/crc.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/exceptions.py
--rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/nodemanager.py
--rw-r--r--   0        0        0    19857 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/pipeline.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/pubsub.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/utils.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/benchmarks/simple.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/authors.md
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/benchmarks.md
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/client.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/logging.md
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/readonly-mode.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/docs/scripting.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic_elasticache_password_protected.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/basic_password_protected.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/from_url_password_protected.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/generate_slot_keys.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/incr-test-writer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/pipeline-incrby.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/examples/pipeline-readonly-replicas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/__init__.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/conftest.py
--rw-r--r--   0        0        0    49667 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/redis-trib.rb
--rw-r--r--   0        0        0    37246 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_connection_pool.py
--rw-r--r--   0        0        0    21655 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_node_manager.py
--rw-r--r--   0        0        0    20837 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_cluster_obj.py
--rw-r--r--   0        0        0   103248 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_commands.py
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_commands_cluster.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_encoding.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_encoding_cluster.py
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_lock.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_monitor.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_multiprocessing_cluster.py
--rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pipeline.py
--rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pipeline_cluster.py
--rw-r--r--   0        0        0    21952 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_pubsub.py
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_scripting.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 custard-1.1.1/custard/rediscluster/tests/test_utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/compat.py
--rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/parser.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.1.1/custard/script/schema.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/socket/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/exception.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/loader.py
--rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/swagger.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.1.1/custard/swagger/utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.1/custard/system/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/dafunc.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/exceptions.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/moment.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.1.1/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/datasets.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/decorators.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 custard-1.1.1/custard/utils/text.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.1.1/examples/async_lur.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.1.1/examples/crypto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.1.1/examples/datum.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.1.1/examples/decorator.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.1.1/examples/dts.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.1.1/examples/hitfilter.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.1.1/examples/hitfilter_keyword
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.1.1/examples/json_logger.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.1.1/examples/kaptcha.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.1.1/examples/kaptcha_execution_time.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.1/examples/limiter.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.1.1/examples/mock.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.1.1/examples/pagination_async_sqlalchemy.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.1.1/examples/pagination_sqlalchemy.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 custard-1.1.1/examples/swagger_online_change.py
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 custard-1.1.1/examples/swagger_usabletest.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.1.1/examples/useragent.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.1.1/.gitignore
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.1.1/README.md
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 custard-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 custard-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 custard-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 custard-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custard-1.1.2/custard/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cache/__init__.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cache/async_lru.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cache/async_lur.md
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cache/redis.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/__init__.py
+-rw-r--r--   0        0        0   770279 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/decode.py
+-rw-r--r--   0        0        0    38952 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/factory.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/kerberos.py
+-rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/processor.py
+-rw-r--r--   0        0        0    23875 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/regular.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/snowflake.py
+-rw-r--r--   0        0        0    15668 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/system.py
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/useragent.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 custard-1.1.2/custard/core/xprint.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cron/__init__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 custard-1.1.2/custard/cron/batch_task.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 custard-1.1.2/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 custard-1.1.2/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 custard-1.1.2/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 custard-1.1.2/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 custard-1.1.2/custard/curl/parse.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 custard-1.1.2/custard/db/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 custard-1.1.2/custard/db/exc.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 custard-1.1.2/custard/db/inspect.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 custard-1.1.2/custard/db/logger.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 custard-1.1.2/custard/db/utils.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 custard-1.1.2/custard/expect/__init__.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 custard-1.1.2/custard/expect/context.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 custard-1.1.2/custard/expect/exceptions.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 custard-1.1.2/custard/expect/record.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 custard-1.1.2/custard/expect/spacer.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.2/custard/extra/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 custard-1.1.2/custard/function/__init__.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 custard-1.1.2/custard/function/callsource.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 custard-1.1.2/custard/function/traverse.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 custard-1.1.2/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 custard-1.1.2/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2020-02-02 00:00:00.000000 custard-1.1.2/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 custard-1.1.2/custard/json/__init__.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 custard-1.1.2/custard/json/jsonlogger.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2020-02-02 00:00:00.000000 custard-1.1.2/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 custard-1.1.2/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 custard-1.1.2/custard/limiter/depends.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 custard-1.1.2/custard/limiter/enums.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 custard-1.1.2/custard/limiter/execres.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lock/__init__.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lock/redis_lock.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lock/thread_lock.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/arrays.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/maths.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/number.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/string.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 custard-1.1.2/custard/lodash/utilities.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/aliyun.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/enums.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/gitee.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/minio.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/qiniu.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 custard-1.1.2/custard/minioss/tencent.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 custard-1.1.2/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 custard-1.1.2/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2020-02-02 00:00:00.000000 custard-1.1.2/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2020-02-02 00:00:00.000000 custard-1.1.2/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.2/custard/network/asynchttp.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 custard-1.1.2/custard/network/enums.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 custard-1.1.2/custard/network/httpclient.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/api.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/default.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.2/custard/pio/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/__init__.py
+-rw-r--r--   0        0        0    49439 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/client.py
+-rw-r--r--   0        0        0    24730 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/connection.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/crc.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/exceptions.py
+-rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/nodemanager.py
+-rw-r--r--   0        0        0    19857 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/pipeline.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/pubsub.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/utils.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/benchmarks/simple.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/authors.md
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/benchmarks.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/client.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/logging.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/readonly-mode.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/docs/scripting.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/basic.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/basic_elasticache_password_protected.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/basic_password_protected.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/from_url_password_protected.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/generate_slot_keys.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/incr-test-writer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/pipeline-incrby.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/examples/pipeline-readonly-replicas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/__init__.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/conftest.py
+-rw-r--r--   0        0        0    49667 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/redis-trib.rb
+-rw-r--r--   0        0        0    37246 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_cluster_connection_pool.py
+-rw-r--r--   0        0        0    21655 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_cluster_node_manager.py
+-rw-r--r--   0        0        0    20837 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_cluster_obj.py
+-rw-r--r--   0        0        0   103248 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_commands.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_commands_cluster.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_encoding.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_encoding_cluster.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_lock.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_monitor.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_multiprocessing_cluster.py
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_pipeline.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_pipeline_cluster.py
+-rw-r--r--   0        0        0    21952 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_pubsub.py
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_scripting.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 custard-1.1.2/custard/rediscluster/tests/test_utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.2/custard/script/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 custard-1.1.2/custard/script/compat.py
+-rw-r--r--   0        0        0    16449 2020-02-02 00:00:00.000000 custard-1.1.2/custard/script/parser.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 custard-1.1.2/custard/script/schema.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.2/custard/socket/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 custard-1.1.2/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 custard-1.1.2/custard/swagger/exception.py
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 custard-1.1.2/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 custard-1.1.2/custard/swagger/utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 custard-1.1.2/custard/system/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 custard-1.1.2/custard/time/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 custard-1.1.2/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 custard-1.1.2/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 custard-1.1.2/custard/time/moment.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 custard-1.1.2/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/__init__.py
+-rw-r--r--   0        0        0   164690 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/area_code.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/configparser.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/id_cards.py
+-rw-r--r--   0        0        0    87780 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/jenkins.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 custard-1.1.2/custard/utils/multi.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 custard-1.1.2/examples/async_lur.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 custard-1.1.2/examples/crypto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 custard-1.1.2/examples/datum.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 custard-1.1.2/examples/decorator.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 custard-1.1.2/examples/dts.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 custard-1.1.2/examples/hitfilter.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 custard-1.1.2/examples/hitfilter_keyword
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 custard-1.1.2/examples/json_logger.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 custard-1.1.2/examples/kaptcha.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 custard-1.1.2/examples/kaptcha_execution_time.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 custard-1.1.2/examples/limiter.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 custard-1.1.2/examples/mock.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 custard-1.1.2/examples/pagination_async_sqlalchemy.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 custard-1.1.2/examples/pagination_sqlalchemy.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 custard-1.1.2/examples/swagger_online_change.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 custard-1.1.2/examples/swagger_usabletest.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 custard-1.1.2/examples/useragent.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 custard-1.1.2/.gitignore
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 custard-1.1.2/README.md
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 custard-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 custard-1.1.2/PKG-INFO
```

### Comparing `custard-1.1.1/.github/workflows/python-publish.yml` & `custard-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/.vscode/launch.json` & `custard-1.1.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/.vscode/settings.json` & `custard-1.1.2/.vscode/settings.json`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "files.trimTrailingWhitespace": true,
   "python.terminal.executeInFileDir": true,
   "terminal.integrated.env.osx": {
     "PYTHONPATH": "${workspaceFolder}"
   },
   "editor.fontSize": 18,
   "editor.links": false,
-  "editor.tabSize": 2,
+  "editor.tabSize": 4,
   "prettier.endOfLine": "auto",
   "window.zoomLevel": 0.01, // 窗口大小，字体大小等
   "files.autoSave": "off",
   /* "editor.formatOnSave": true,
   "editor.formatOnPaste": true, */
   "editor.formatOnType": true,
   "editor.suggestSelection": "first",
@@ -26,28 +26,35 @@
   "explorer.confirmDelete": false,
   "prettier.semi": false,
   "prettier.singleQuote": true,
   "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
   "terminal.integrated.fontSize": 16,
   "editor.guides.bracketPairs": true,
   "search.followSymlinks": false, //控制是否在搜索中跟踪符号链接。
+  "pythonTestExplorer.testFramework": "pytest",
+  "pythonTestExplorer.testplanEnabled": true,
+  "python.formatting.provider": "black",
+  "python.formatting.blackPath": "",
   "files.exclude": {
     // 不需要扫描的文件夹
     "**/node_modules": true,
     // "**/.umi": true,
     // "**/public": true,
     "**/.classpath": true,
     "**/.project": true,
     "**/.settings": true,
     "**/.factorypath": true
   },
   "editor.quickSuggestions": {
     "strings": true
   },
   /*以下为代码格式化配置*/
+  "[python]": {
+    "editor.defaultFormatter": "ms-python.black-formatter"
+  },
   "[dockerfile]": {
     "editor.defaultFormatter": "ms-azuretools.vscode-docker"
   },
   "[dockercompose]": {
     "editor.defaultFormatter": "ms-azuretools.vscode-docker"
   },
   "[markdown]": {
@@ -80,14 +87,15 @@
   "cSpell.words": [
     "ADDSLOTS",
     "allready",
     "alot",
     "axios",
     "basepath",
     "basestring",
+    "behaviour",
     "BGREWRITEAOF",
     "BGSAVE",
     "BITCOUNT",
     "BITOP",
     "BITPOS",
     "brpop",
     "brpoplpush",
@@ -96,14 +104,15 @@
     "CLUSTERDOWN",
     "COUNTKEYSINSLOT",
     "CROSSSLOT",
     "DBSIZE",
     "DELSLOTS",
     "evalsha",
     "EXISTS",
+    "fdir",
     "FLUSHALL",
     "GEODIST",
     "GEOHASH",
     "GEOPOS",
     "GEORADIUS",
     "GEORADIUSBYMEMBER",
     "GET",
@@ -131,22 +140,26 @@
     "LRANGE",
     "MASTERDOWN",
     "MGET",
     "MSETNX",
     "nativestr",
     "nodemanager",
     "nslookup",
+    "numlines",
     "NUMPAT",
     "numsub",
+    "pageindex",
     "pfcount",
     "pfmerge",
     "PHPSESSID",
     "PTTL",
     "punsubscribe",
+    "pycache",
     "pydantic",
+    "pypinyin",
     "Qing",
     "RANDOMKEY",
     "randos",
     "rediscluster",
     "renamenx",
     "RESETSTAT",
     "rpoplpush",
@@ -154,28 +167,33 @@
     "SAVECONFIG",
     "SCARD",
     "SDIFF",
     "sdiffstore",
     "setslot",
     "SETUSER",
     "shold",
+    "sina",
     "SINTER",
     "sinterstore",
     "SISMEMBER",
     "SLAVEOF",
     "SLOWLOG",
     "SMEMBERS",
     "smove",
+    "sohu",
     "SRANDMEMBER",
     "STRLEN",
     "SUNION",
     "sunionstore",
+    "topdown",
     "TRYAGAIN",
     "TTL",
     "unwatch",
     "xform",
+    "xwww",
     "ZCARD",
     "ZCOUNT",
+    "ziplist",
     "ZRANGE",
     "ZSCORE"
-  ] // 启用智能提交
+] // 启用智能提交
 }
```

### Comparing `custard-1.1.1/custard/cache/async_lru.py` & `custard-1.1.2/custard/cache/async_lru.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/cache/async_lur.md` & `custard-1.1.2/custard/cache/async_lur.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/cache/redis.py` & `custard-1.1.2/custard/cache/redis.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/__init__.py` & `custard-1.1.2/custard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/decode.py` & `custard-1.1.2/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/factory.py` & `custard-1.1.2/custard/core/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,54 +5,76 @@
 @time    :  2021/8/5 5:21 pm
 @author  :  YuYanQing
 @version :  1.0
 @contact :  mryu168@163.com
 @license :  (c)copyright 2022-2026
 @desc    :  函数助手
 """
-from collections import defaultdict
 import json
 import random
 import re
 import string
 from typing import List, Dict
 from urllib.parse import quote
-
+import difflib
+import hashlib
+import json
+import logging
+from urllib.parse import unquote
+import operator
+from collections import Counter
+from functools import reduce
+from typing import Dict, Tuple
 import pypinyin
 from faker import Faker
 from requests.exceptions import InvalidURL
 from urllib3.exceptions import LocationParseError
 from urllib3.util import parse_url
 from custard.time.moment import Moment
+from custard.utils.id_cards import IdNumber
+from custard.core.system import System
 
 fake = Faker(["zh_CN"])
+logger = logging.getLogger(__name__)
 
 
 class MockHelper:
     @staticmethod
-    def hans2pinyin(hans, style="A"):
+    def rand_hans2pinyin(hans, style="A"):
         """
         汉字转拼音
         Args:
             hans: 汉字
-            style: 返回首字母还是全拼， A：全拼； F：首字母
+            style: 返回首字母还是全拼, A:全拼; F:首字母
         Returns:
         Examples:
             >>> print(MockHelper.hans2pinyin("啊哈哈哈"))
             >>> print(MockHelper.hans2pinyin("啊哈哈哈", "F"))
         """
 
         if style.upper() == "F":
             return "".join(
                 pypinyin.lazy_pinyin(hans=hans, style=pypinyin.Style.FIRST_LETTER)
             )
         else:
             return "".join(pypinyin.lazy_pinyin(hans=hans))
 
     @staticmethod
+    def rand_id_card(random_sex):
+        """
+        随机生成有效身份证
+        Args:
+            random_sex: 性别
+        Returns:
+        Examples:
+            >>> MockHelper.rand_id_card()
+        """
+        return IdNumber.get_id_card(random_sex)
+
+    @staticmethod
     def rand_mail(email_type=None, max_num=None, rad_count=None):
         """
         Args:
             email_type: 邮箱类型
             max_num: 邮箱地址最大长度
             rad_count: 所生成的数量
         Returns:
@@ -78,16 +100,15 @@
             for i in range(0, max_num_):
                 status = random.randint(0, 1)
                 if status == 0:
                     temp.append(random.choice(string.ascii_letters))
                 else:
                     temp.append(str(random.randint(0, 1)))
             temp_str = "".join(temp)
-            # 每次转化后就丢弃temp、避免出现遍历追加['vjt000ho@qq.com',
-            # 'vjt000ho0110fm0w@qq.com'............]
+            # 每次转化后就丢弃temp、避免出现遍历追加['vjt000ho@qq.com', 'vjt000ho0110fm0w@qq.com'............]
             temp.clear()
             email_list.append(temp_str + email_type_)
             count += 1
         return email_list
 
     @staticmethod
     def rand_verify_code(max_num: int, rad_count: int):
@@ -96,39 +117,39 @@
         Args:
             max_num: 最多可生成的长度
             rad_count: 需要生成的数量
         Returns:
         Examples:
             >>> MockHelper.rand_verify_code(max_num=6, rad_count=1)
         """
-        # 注意： 这里我们生成的是0-9a-za-z的列表，当然你也可以指定这个list，这里很灵活
-        # 比如： code_list = ['p','y','t','h','o','n','t','a','b'] # pythontab的字母
+        # 注意： 这里我们生成的是0-9a-za-z的列表,当然你也可以指定这个list,这里很灵活
+        # 比如： code_list = ['p','y','t','h','o','n'] # python的字母
         count = 0
         verification_codes = []
         while count < rad_count:
             code_list = []
             for i in range(10):  # 0-9数字
                 code_list.append(str(i))
             for i in range(65, 91):  # 对应从“a”到“z”的ascii码
                 code_list.append(chr(i))
             for i in range(97, 123):  # 对应从“a”到“z”的ascii码
                 code_list.append(chr(i))
-            # 从list中随机获取6个元素，作为一个片断返回
+            # 从list中随机获取6个元素,作为一个片断返回
             my_slice = random.sample(code_list, max_num)
             verification_codes.append("".join(my_slice))  # list to string
             count += 1
         if rad_count > 1:
             return verification_codes
         else:
             return verification_codes[0]
 
     @staticmethod
     def rand_str_list(length):
         """
-        生成给定长度的字符串，返回列表格式
+        生成给定长度的字符串,返回列表格式
         Args:
             length:
         Returns:
         Examples:
             >>> MockHelper.rand_str_list(length=5)
         """
         init_chars = "".join("".join(map(str, [i for i in range(10) if i != 4])))  # 数字
@@ -189,15 +210,15 @@
             >>> MockHelper.rand_float_number(start_num=0, end_num=6, accuracy=3)
         """
         try:
             start_num = int(start_num)
             end_num = int(end_num)
             accuracy = int(accuracy)
         except ValueError:
-            raise AssertionError("调用随机整数失败，范围参数或精度有误！\n小数范围精度")
+            raise AssertionError("调用随机整数失败,范围参数或精度有误！\n小数范围精度")
         if start_num <= end_num:
             num = random.uniform(start_num, end_num)
         else:
             num = random.uniform(end_num, start_num)
         return round(num, accuracy)
 
     @staticmethod
@@ -652,17 +673,17 @@
             return var.decode() if isinstance(var, bytes) else var
         else:
             raise ModuleNotFoundError("暂时仅支持：%s" % (", ".join(func_list)))
 
     @staticmethod
     def cite(name: str):
         """
-        函数助手，输出以下常用随机数，返回结果值。支持的函数详情见func_dict:
+        函数助手,输出以下常用随机数,返回结果值。支持的函数详情见func_dict:
         Args:
-            name:  函数名，需要在func_dict存在的key值
+            name:  函数名,需要在func_dict存在的key值
         Returns:  随机函数调用结果 or None
         Examples:
             >>> MockHelper.cite('${rand_int_number()}')
             >>> MockHelper.cite('${rand_int_number(1,55)}')
             >>> MockHelper.cite('${rand_lowercase_letter(5)}')
             >>> MockHelper.cite('${rand_sample(1235)}')
             >>> MockHelper.cite("${get_user_vars()}")
@@ -680,14 +701,18 @@
         rand_no_vars = re.match("\\$\\{rand_(.*)\\}", str(name))  # 无参数
         dynamic_vars = re.match("\\$\\{get(.*)\\((.*)\\)\\}", str(name))  # 动态自定义
         own_vars = re.match("\\{\\{(.*)\\}\\}", str(name))  # 动态自定义
         extract_vars = re.match("\\$var_(.*)", str(name).upper())  # 后置提取参数
         lock_vars = re.match("\\$enc_(.*)", str(name))  # 带参数
         pattern = rand_vars if rand_vars is not None else dynamic_vars
         func_dict = {
+            "mum": MockHelper.rand_mum,
+            "hans2pinyin": MockHelper.rand_hans2pinyin,
+            "id_card": MockHelper.rand_id_card,
+            "mail": MockHelper.rand_mail,
             "int_number": MockHelper.rand_int_number,
             "float_number": MockHelper.rand_float_number,
             "compute_time": MockHelper.rand_compute_time,
             "lowercase_letter": MockHelper.rand_lowercase_letter,
             "uppercase_letter": MockHelper.rand_uppercase_letter,
             "sample": MockHelper.rand_sample,
             "mobile_number": MockHelper.rand_mobile_number,
@@ -775,26 +800,298 @@
                 else:
                     dict_map[key] = MockHelper.cite(dict_map[key])
             return dict_map
         elif dict_map is None:  # fix：为空的时候raise 异常导致其它函数调用失败
             pass
 
 
+class DataKitHelper:
+    @classmethod
+    def add_dicts(cls, *args: Tuple[Dict, ...]) -> Dict:
+        """
+        Adds two or more dicts together. Common keys will have their values added.
+
+        Returns:
+        Example:
+            >>> t1 = {'a':1, 'b':2}
+            >>> t2 = {'b':1, 'c':3}
+            >>> t3 = {'d':5}
+            >>> DataKit.add_dicts(t1, t2, t3)
+            {'a': 1, 'c': 3, 'b': 3, 'd': 5}
+        """
+
+        counters = [Counter(arg) for arg in args]
+        return dict(reduce(operator.add, counters))
+
+    @classmethod
+    def get_target_value(
+        cls, dict_map: dict, separate: str = "$.", result: dict = None
+    ):
+        if result is None:
+            result = dict()
+        """
+        递归获取所有的TargetValue
+        :param dict_map: 初始data dict类型
+        :param separate: 临时节点 str类型
+        :param result:  用于存储所有遍历出来的结果 list集合
+        :return: {xx,xx,xx} 以字典形式追加
+        Example::
+            >>> DataKit.get_target_value(dict_map={"TEST_001": "TEST_VALUE001","TEST_002": [{"TEST_VALUE002-001": "VALUE"}, {"TEST_VALUE002-002": "VALUE"}]})
+        """
+        if isinstance(dict_map, dict):
+            for key, value in dict_map.items():
+                temp = separate + key + "."
+                # 若类型为list 后面还有一维或二位数组类型数据递归找
+                if isinstance(value, list):
+                    for i in range(len(value)):
+                        cls.get_target_value(
+                            dict_map=value[i], separate=temp + str(i) + "."
+                        )
+                # 若类型还是dict，继续遍历
+                elif isinstance(value, dict):
+                    cls.get_target_value(dict_map=value, separate=temp)
+                # str或者int类型时就基本上判定为具体的xxx值
+                elif str(value).isdigit():
+                    result.update({separate + key: int(value)})
+                elif isinstance(value, str):
+                    result.update({separate + key: value})
+            return result
+        else:
+            raise TypeError("传入的参数不是dict类型 %s" % (type(dict_map)))
+
+    @classmethod
+    def convert_type(cls, dict_map: dict, disable_data: list = []) -> dict:
+        """
+        将只有数字的键值给强转类型为int
+        :param dict_map: 初始data dict类型
+        :param disable: 不用处理的键值对
+        Example::
+            >>> DataKit.convert_type({'product': {'brand_id': None, 'category_id': '15888'}})
+            >>> DataKit.convert_type({'product': {'brand_id': None, 'category_id': '15888'}},["category_id"])
+        """
+        if isinstance(dict_map, dict):
+            for key in list(dict_map.keys()):
+                if isinstance(dict_map[key], list):
+                    for i in range(len(dict_map[key])):
+                        dict_map[key][i] = cls.convert_type(
+                            dict_map=dict_map[key][i], disable_data=disable_data
+                        )
+                elif isinstance(dict_map[key], dict):
+                    dict_map[key] = cls.convert_type(
+                        dict_map=dict_map[key], disable_data=disable_data
+                    )
+                elif str(dict_map[key]).isdigit() and str(key) not in disable_data:
+                    dict_map[key] = int(dict_map[key])
+                elif str(dict_map[key]) == "null":  # 统一处理str无法转化None
+                    dict_map[key] = None
+            return (
+                json.dumps(dict_map, ensure_ascii=False)
+                .replace('\\"', '"')
+                .replace('"{', "{")
+                .replace('}"', "}")
+            )  # 临时打个补丁 后续若报错则需再次做兼容
+        else:
+            raise TypeError("传入的参数不是dict类型 %s" % (type(dict_map)))
+
+    @classmethod
+    def dict_to_from(cls, post_data):
+        """
+        字典转xwww-from格式
+        :param post_data: dict {"a": 1, "b":2}
+        :return: str: a=1&b=2
+        """
+        if isinstance(post_data, dict):
+            return "&".join(
+                ["{}={}".format(key, value) for key, value in post_data.items()]
+            )
+        else:
+            return post_data
+
+    @classmethod
+    def form_to_dict(cls, post_data):
+        """
+        x-www-from格式转字典
+        :param post_data (str): a=1&b=2
+        :return dict: {"a":1, "b":2}
+        """
+        if isinstance(post_data, str):
+            converted_dict = {}
+            for k_v in post_data.split("&"):
+                try:
+                    key, value = k_v.split("=")
+                except ValueError:
+                    raise Exception(
+                        "Invalid x_www_form_urlencoded data format: {}".format(
+                            post_data
+                        )
+                    )
+                converted_dict[key] = unquote(value)
+            return converted_dict
+        else:
+            return post_data
+
+    @classmethod
+    def list_sub_dict(cls, origin_list):
+        """
+        list转dict
+        :param origin_list: (list) [{"name": "v", "value": "1"},{"name": "w", "value": "2"}]
+        :return: dict:{"v": "1", "w": "2"}
+        """
+        return {item["name"]: item.get("value") for item in origin_list}
+
+    @classmethod
+    def dict_capital_to_lower(cls, dict_map):
+        """
+        dict中的key转换小写
+        :param dict_map:
+        :return:
+        """
+        new_dict = {}
+        for key in list(dict_map.keys()):
+            new_dict[key.lower()] = dict_map[key]
+        return new_dict
+
+    @classmethod
+    def capital_lower_to_dict(cls, dict_map):
+        """
+        dict中的key转换大写
+        :param dict_map:
+        :return:
+        """
+        new_dict = {}
+        for key in list(dict_map.keys()):
+            new_dict[key.upper()] = dict_map[key]
+        return new_dict
+
+    @classmethod
+    def diffJson(cls, filename1, filename2, targetPath):
+        """
+        比较两个文件内容的md5值并输出到html文件中
+        :param filename1:
+        :param filename2:
+        :param targetPath:
+        :return:
+        """
+        file1Md5 = hashlib.md5.new(filename1.read()).digest()
+        file2Md5 = hashlib.md5.new(filename2.read()).digest()
+        if file1Md5 != file2Md5:
+            text1_lines = System.load_file(filename1, "json")
+            text2_lines = System.load_file(filename2, "json")
+            d = difflib.HtmlDiff()
+            # context=True时只显示差异的上下文，默认显示5行，由numlines参数控制，context=False显示全文，差异部分颜色高亮，默认为显示全文
+            result = d.make_file(
+                text1_lines, text2_lines, filename1, filename2, context=True
+            )
+            # 内容保存到result.html文件中
+            try:
+                with open(targetPath, "a", encoding="utf-8") as result_file:
+                    result_file.write(result)
+            except Exception as e:
+                logger.error("写入文件失败:" + e)
+
+    @classmethod
+    def is_json_format(cls, raw_data):
+        """
+        用于判断一个字符串是否符合Json格式
+        :param raw_data:
+        :return:
+        """
+        if isinstance(raw_data, str):
+            try:
+                json.loads(raw_data, encoding="utf-8")
+            except ValueError:
+                return False
+            else:
+                return True
+        else:
+            return False
+
+    @classmethod
+    def json_to_dict(cls, data):
+        """
+        Json转字典
+        :param data: 数据来源
+        :return:
+        """
+        return json.loads(data)
+
+    @classmethod
+    def dict_to_json(
+        cls, data, sort_keys=False, ensure_ascii=False, indent=4, separators=(",", ": ")
+    ):
+        """
+        字典转Json
+        :param data: 数据来源
+        :return:
+        """
+        return json.dumps(
+            data,
+            ensure_ascii=ensure_ascii,
+            sort_keys=sort_keys,
+            indent=indent,
+            separators=separators,
+        )
+
+    @classmethod
+    def json_to_schema(cls, data, result=None):
+        """
+        json递归生成schema
+        :param data:
+        :param result:
+        :return:
+        Example::
+            >>> data = {"code": 200, "message": "Success", "error": "",
+            ... "ShopInfoList": [{"shop_id": "ML0057", "shop_name": "" }]}
+            >>> DataKit.json_to_schema(data=data)
+        """
+        if result is None:
+            result = list()
+        if isinstance(data, dict):
+            is_null = True
+            result.append("{")
+            result.append("'type': 'object',")
+            result.append("'properties': {")
+            for k, v in data.items():
+                is_null = False
+                result.append("'%s':" % k)
+                cls.json_to_schema(v, result)
+                result.append(",")
+            if not is_null:
+                result.pop()
+            result.append("}")
+            result.append("}")
+        elif isinstance(data, list):
+            result.append("{")
+            result.append("'type': 'array',")
+            result.append("'items': ")
+            cls.json_to_schema(data[0], result)
+            result.append("}")
+        elif isinstance(data, int):
+            result.append("{")
+            result.append("'type': 'number'")
+            result.append("}")
+        elif isinstance(data, str):
+            result.append("{")
+            result.append("'type': 'string'")
+            result.append("}")
+        return json.dumps("".join(result), indent=4)
+
+
 class AutoVivification(dict):
     def __getitem__(self, item):
         try:
             return dict.__getitem__(self, item)
         except KeyError:
             value = self[item] = type(self)()
         return value
 
 
 class MsHelper(object):
-    GLOBAL_PAGE_INDEX = ["page_index" "pageindex"]
-    GLOBAL_PAGE_SIZE = ["page_size" "pagesize"]
+    GLOBAL_PAGE_INDEX = ["page_index", "pageindex"]
+    GLOBAL_PAGE_SIZE = ["page_size", "pagesize"]
 
     @classmethod
     def __property__(cls, prop):
         """
         数据转换
         Args:
             prop:
@@ -827,58 +1124,57 @@
         type_err = TypeError("类型错误、仅支持dict")
         if isinstance(data, support_type):
             raise type_err
         if isinstance(data, str):
             try:
                 return json.loads(data)
             except json.decoder.JSONDecodeError as decoder_err:
-                raise decoder_err
+                raise Exception(decoder_err)
         if isinstance(data, dict):
             return data
 
     @classmethod
     def sub_kv(cls, data: List):
         """
         合并key value
         Args:
             data:
         Returns:
         Examples:
             >>> data_ = ["a1=5","a3=6"]
-            >>> dinct_data_ = ["a2=6","a2=6"]
+            >>> dint_data_ = ["a2=6","a2=6"]
             >>> MsHelper.sub_kv(data_)
-            >>> MsHelper.sub_kv(dinct_data_)
+            >>> MsHelper.sub_kv(dint_data_)
         """
         temp_dict = {}
         for index in range(len(data)):
             present = data[index]
             if "=" in present:
                 pr_ = present.split("=")
                 temp_dict.update({pr_[0]: pr_[1]})
             else:
                 temp_dict.update({present: ""})
             # 相同数据跳出
-            if index < len(data) - 1:
-                if present == data[index + 1]:
-                    break
+            if index < len(data) - 1 and present == data[index + 1]:
+                break
         return temp_dict
 
     @classmethod
-    def form2json(cls, url):
+    def url_to_json(cls, url):
         """
         form-data 转换为 Json
         Args:
             url:
         Returns:
         Examples:
             >>> form_data_ = ""
             >>> for index in range(10000):
             ...     form_data_ += f"&a{index}={index}"
             >>> url_ = f"http://localhost?{form_data_}"
-            >>> output_ = MsHelper.form2json(url_)
+            >>> output_ = MsHelper.url_to_json(url_)
             >>> print(output_)
         """
         try:
             scheme, auth, host, port, path, query, fragment = parse_url(url)
         except LocationParseError as e:
             raise InvalidURL(*e.args)
         output = {}
@@ -952,14 +1248,14 @@
                 else:
                     source_data = cls.json2vars(
                         target_data=value, source_data=source_data, replace=replace
                     )
         elif isinstance(target_data, list):
             for index in range(len(target_data)):
                 target_data_ = target_data[index]
-                # 启用该行数据不会去重，有多少条就产生多少
+                # 启用该行数据不会去重,有多少条就产生多少
                 # source_data = cls.json2vars(target_data=target_data_, source_data=source_data, replace=replace)
                 # 以下方式会去重
                 return cls.json2vars(
                     target_data=target_data_, source_data=source_data, replace=replace
                 )
         return source_data
```

### Comparing `custard-1.1.1/custard/core/kerberos.py` & `custard-1.1.2/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/processor.py` & `custard-1.1.2/custard/core/processor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/regular.py` & `custard-1.1.2/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/snowflake.py` & `custard-1.1.2/custard/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/useragent.py` & `custard-1.1.2/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/xml2dict.py` & `custard-1.1.2/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/core/xprint.py` & `custard-1.1.2/custard/core/xprint.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/cron/batch_task.py` & `custard-1.1.2/custard/cron/batch_task.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/crypto/crypto.py` & `custard-1.1.2/custard/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/crypto/streambody.py` & `custard-1.1.2/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/curl/parse.py` & `custard-1.1.2/custard/curl/parse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/db/inspect.py` & `custard-1.1.2/custard/db/inspect.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/db/logger.py` & `custard-1.1.2/custard/db/logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/db/utils.py` & `custard-1.1.2/custard/db/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/expect/context.py` & `custard-1.1.2/custard/expect/context.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/expect/exceptions.py` & `custard-1.1.2/custard/expect/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/expect/record.py` & `custard-1.1.2/custard/expect/record.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/expect/spacer.py` & `custard-1.1.2/custard/expect/spacer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/function/callsource.py` & `custard-1.1.2/custard/function/callsource.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/function/traverse.py` & `custard-1.1.2/custard/function/traverse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/hitfilter/hitfilter.py` & `custard-1.1.2/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/hitfilter/keywords` & `custard-1.1.2/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/json/jsonlogger.py` & `custard-1.1.2/custard/json/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/kaptcha/captcha.py` & `custard-1.1.2/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/kaptcha/font1.ttf` & `custard-1.1.2/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/kaptcha/font2.ttf` & `custard-1.1.2/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/kaptcha/font3.ttf` & `custard-1.1.2/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/kaptcha/font4.ttf` & `custard-1.1.2/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/limiter/__init__.py` & `custard-1.1.2/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/limiter/depends.py` & `custard-1.1.2/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lock/redis_lock.py` & `custard-1.1.2/custard/lock/redis_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lock/thread_lock.py` & `custard-1.1.2/custard/lock/thread_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/README.md` & `custard-1.1.2/custard/lodash/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/__init__.py` & `custard-1.1.2/custard/lodash/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/arrays.py` & `custard-1.1.2/custard/lodash/arrays.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/maths.py` & `custard-1.1.2/custard/lodash/maths.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/number.py` & `custard-1.1.2/custard/lodash/number.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/string.py` & `custard-1.1.2/custard/lodash/string.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/lodash/utilities.py` & `custard-1.1.2/custard/lodash/utilities.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/mock/__init__.py` & `custard-1.1.2/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/mock/mini_racer.py` & `custard-1.1.2/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/mock/mock.min.js` & `custard-1.1.2/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/mock/mock.old.min.js` & `custard-1.1.2/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/network/httpclient.py` & `custard-1.1.2/custard/network/httpclient.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/__init__.py` & `custard-1.1.2/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/api.py` & `custard-1.1.2/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/async_sqlalchemy.py` & `custard-1.1.2/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/bases.py` & `custard-1.1.2/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/default.py` & `custard-1.1.2/custard/pagination/default.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/iterables.py` & `custard-1.1.2/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/limit_offset.py` & `custard-1.1.2/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/pagination.py` & `custard-1.1.2/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/paginator.py` & `custard-1.1.2/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.2/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/__init__.py` & `custard-1.1.2/custard/rediscluster/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/client.py` & `custard-1.1.2/custard/rediscluster/client.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/connection.py` & `custard-1.1.2/custard/rediscluster/connection.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/crc.py` & `custard-1.1.2/custard/rediscluster/crc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/exceptions.py` & `custard-1.1.2/custard/rediscluster/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/nodemanager.py` & `custard-1.1.2/custard/rediscluster/nodemanager.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/pipeline.py` & `custard-1.1.2/custard/rediscluster/pipeline.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/pubsub.py` & `custard-1.1.2/custard/rediscluster/pubsub.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/utils.py` & `custard-1.1.2/custard/rediscluster/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/benchmarks/simple.py` & `custard-1.1.2/custard/rediscluster/benchmarks/simple.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/authors.md` & `custard-1.1.2/custard/rediscluster/docs/authors.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/benchmarks.md` & `custard-1.1.2/custard/rediscluster/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/client.md` & `custard-1.1.2/custard/rediscluster/docs/client.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/logging.md` & `custard-1.1.2/custard/rediscluster/docs/logging.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/readonly-mode.md` & `custard-1.1.2/custard/rediscluster/docs/readonly-mode.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/docs/scripting.md` & `custard-1.1.2/custard/rediscluster/docs/scripting.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/examples/basic_elasticache_password_protected.py` & `custard-1.1.2/custard/rediscluster/examples/basic_elasticache_password_protected.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/examples/generate_slot_keys.py` & `custard-1.1.2/custard/rediscluster/examples/generate_slot_keys.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/examples/pipeline-incrby.py` & `custard-1.1.2/custard/rediscluster/examples/pipeline-incrby.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/examples/pipeline-readonly-replicas.py` & `custard-1.1.2/custard/rediscluster/examples/pipeline-readonly-replicas.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/conftest.py` & `custard-1.1.2/custard/rediscluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/redis-trib.rb` & `custard-1.1.2/custard/rediscluster/tests/redis-trib.rb`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_cluster_connection_pool.py` & `custard-1.1.2/custard/rediscluster/tests/test_cluster_connection_pool.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_cluster_node_manager.py` & `custard-1.1.2/custard/rediscluster/tests/test_cluster_node_manager.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_cluster_obj.py` & `custard-1.1.2/custard/rediscluster/tests/test_cluster_obj.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_commands.py` & `custard-1.1.2/custard/rediscluster/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_commands_cluster.py` & `custard-1.1.2/custard/rediscluster/tests/test_commands_cluster.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_encoding.py` & `custard-1.1.2/custard/rediscluster/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_encoding_cluster.py` & `custard-1.1.2/custard/rediscluster/tests/test_encoding_cluster.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_lock.py` & `custard-1.1.2/custard/rediscluster/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_monitor.py` & `custard-1.1.2/custard/rediscluster/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_multiprocessing.py` & `custard-1.1.2/custard/rediscluster/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_multiprocessing_cluster.py` & `custard-1.1.2/custard/rediscluster/tests/test_multiprocessing_cluster.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_pipeline.py` & `custard-1.1.2/custard/rediscluster/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_pipeline_cluster.py` & `custard-1.1.2/custard/rediscluster/tests/test_pipeline_cluster.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_pubsub.py` & `custard-1.1.2/custard/rediscluster/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_scripting.py` & `custard-1.1.2/custard/rediscluster/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/rediscluster/tests/test_utils.py` & `custard-1.1.2/custard/rediscluster/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/script/compat.py` & `custard-1.1.2/custard/script/compat.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/script/parser.py` & `custard-1.1.2/custard/script/parser.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/script/schema.py` & `custard-1.1.2/custard/script/schema.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/swagger/__init__.py` & `custard-1.1.2/custard/swagger/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,33 @@
 @Time    :  2022/7/18 10:16
 @Author  :  YuYanQing
 @Version :  1.0
 @Contact :  mryu168@163.com
 @License :  (C)Copyright 2022-2026
 @Desc    :  None
 """
+from urllib import request
+from custard.core.system import System
 from .swagger import Swagger2
 from .exception import ParseMethodError
-from .loader import load_file, load_url
+
+
+def load_url(url, method="get", **kwargs):
+    """
+    通过url加载json
+    Args:
+        url:
+        method:
+        **kwargs:
+
+    Returns:
+
+    """
+    return request.request(url=url, method=method, **kwargs).json()
+
 
 def swagger_parse(url=None, file=None, deep=5, **kwargs):
     """
     解析swagger
     Args:
         url:
         file:
@@ -24,11 +40,11 @@
 
     Returns:
 
     """
     if url:
         source = load_url(url, **kwargs)
     elif file:
-        source = load_file(file)
+        source = System.load_file(file, "json")
     else:
         raise ParseMethodError("解析方式错误")
     return Swagger2(source, deep=deep)
```

### Comparing `custard-1.1.1/custard/swagger/swagger.py` & `custard-1.1.2/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/swagger/utils.py` & `custard-1.1.2/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/time/dafunc.py` & `custard-1.1.2/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/time/exceptions.py` & `custard-1.1.2/custard/time/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/time/moment.py` & `custard-1.1.2/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/custard/time/stoppable_thread.py` & `custard-1.1.2/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/async_lur.py` & `custard-1.1.2/examples/async_lur.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/decorator.py` & `custard-1.1.2/examples/decorator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/dts.py` & `custard-1.1.2/examples/dts.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/hitfilter.py` & `custard-1.1.2/examples/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/json_logger.py` & `custard-1.1.2/examples/json_logger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/kaptcha.py` & `custard-1.1.2/examples/kaptcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/kaptcha_execution_time.py` & `custard-1.1.2/examples/kaptcha_execution_time.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/limiter.py` & `custard-1.1.2/examples/limiter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/mock.py` & `custard-1.1.2/examples/mock.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/pagination_async_sqlalchemy.py` & `custard-1.1.2/examples/pagination_async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/pagination_sqlalchemy.py` & `custard-1.1.2/examples/pagination_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/swagger_online_change.py` & `custard-1.1.2/examples/swagger_online_change.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/swagger_usabletest.py` & `custard-1.1.2/examples/swagger_usabletest.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/examples/useragent.py` & `custard-1.1.2/examples/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/README.md` & `custard-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/pyproject.toml` & `custard-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `custard-1.1.1/PKG-INFO` & `custard-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.1.1
+Version: 1.1.2
 Summary: custard easy to learn, fast to code, ready for production
 Project-URL: Homepage, https://github.com/kamalyes/custard
 Author-email: Kamalyes <mryu168@163.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

