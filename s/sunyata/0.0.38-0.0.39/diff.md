# Comparing `tmp/sunyata-0.0.38.tar.gz` & `tmp/sunyata-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.38.tar", last modified: Fri Apr 21 02:51:42 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.39.tar", last modified: Thu Apr 27 07:15:19 2023, max compression
```

## Comparing `sunyata-0.0.38.tar` & `sunyata-0.0.39.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-21 02:51:42.000000 sunyata-0.0.38/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1399 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       70 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.38/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.38/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.38/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.38/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.38/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.38/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.38/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     1724 2023-04-20 12:48:28.000000 sunyata-0.0.38/sunyata/etcd.py
--rw-r--r--   0 root         (0) staff       (20)     3718 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     3251 2023-04-20 08:32:35.000000 sunyata-0.0.38/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.38/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.38/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.38/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.38/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.38/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.38/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-20 03:05:05.000000 sunyata-0.0.38/sunyata/http/rawserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.38/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.38/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-21 02:51:42.000000 sunyata-0.0.38/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.38/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    12146 2023-04-20 08:39:54.000000 sunyata-0.0.38/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2437 2023-04-20 06:50:23.000000 sunyata-0.0.38/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.38/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8117 2023-04-21 02:49:05.000000 sunyata-0.0.38/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.38/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.38/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.38/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)    10444 2023-04-21 02:46:28.000000 sunyata-0.0.38/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-21 02:50:58.000000 sunyata-0.0.38/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-21 02:51:42.000000 sunyata-0.0.38/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-27 07:15:19.000000 sunyata-0.0.39/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1399 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       69 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/
+-rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/db.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)      497 2023-04-20 03:17:34.000000 sunyata-0.0.39/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/orm.py
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cli/entry.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.39/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.39/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.39/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.39/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.39/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.39/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.39/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/redislock.py
+-rw-r--r--   0 root         (0) staff       (20)     2233 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/etcd.py
+-rw-r--r--   0 root         (0) staff       (20)     3599 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/consul.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)     3251 2023-04-20 08:32:35.000000 sunyata-0.0.39/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-25 07:23:36.000000 sunyata-0.0.39/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.39/sunyata/http/transport.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.39/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-13 06:36:26.000000 sunyata-0.0.39/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1639 2023-04-14 10:00:43.000000 sunyata-0.0.39/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.39/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)     3394 2023-04-20 03:05:05.000000 sunyata-0.0.39/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.39/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.39/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/cache_wrap.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/compress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-27 07:15:19.000000 sunyata-0.0.39/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      702 2023-04-20 03:17:34.000000 sunyata-0.0.39/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)    11863 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     2474 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)     7774 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     8159 2023-04-25 07:31:21.000000 sunyata-0.0.39/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.39/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.39/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.39/sunyata/wrap.py
+-rw-r--r--   0 root         (0) staff       (20)    11659 2023-04-26 09:22:35.000000 sunyata-0.0.39/README.md
+-rwxr-xr-x   0 root         (0) staff       (20)     1026 2023-04-25 09:18:13.000000 sunyata-0.0.39/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-27 07:15:19.000000 sunyata-0.0.39/setup.cfg
```

### Comparing `sunyata-0.0.38/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.39/sunyata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/db.py` & `sunyata-0.0.39/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/log.py` & `sunyata-0.0.39/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/orm.py` & `sunyata-0.0.39/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/cli/cli.py` & `sunyata-0.0.39/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.39/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/algorithm/lru.py` & `sunyata-0.0.39/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/algorithm/trie.py` & `sunyata-0.0.39/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/algorithm/hashtable.py` & `sunyata-0.0.39/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/redislock.py` & `sunyata-0.0.39/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/etcd.py` & `sunyata-0.0.39/sunyata/etcd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import ujson
-import requests
 from sunyata.util import local_ip
 from sunyata.consul import Instance
-
+import aiohttp
 
 class EtcdApi(object):
 
     def __init__(self, host: str, port: int):
         self.host = host
         self.port = port
         self.baseUrl = 'http://%s:%s' % (self.host, self.port)
         self.timeout = 5
         self.headers = {}
 
-    def registService(self, serviceName: str, port = 80, address=None, ttl=30):
-        url = self.baseUrl + '/v2/keys/sunyata-services/%s?dir=true&ttl=%s' % (serviceName, ttl)
-        r = requests.put(url, timeout=self.timeout, headers=self.headers)
-        if address:
-            key  = address + ':' + str(port)
-        else:
-            key = local_ip() + ':' + str(port)
-        val = key
-        url = self.baseUrl + '/v2/keys/sunyata-services/%s/%s?value=%s&ttl=%s' % (serviceName, key, val, ttl)
-        r = requests.put(url, timeout=self.timeout, headers=self.headers)
-        print(r.text, r.status_code)
+    async def registService(self, serviceName: str, port = 80, address=None, ttl=30):
+        async with aiohttp.ClientSession() as sess:
+            url = self.baseUrl + '/v2/keys/sunyata-services/%s?dir=true&ttl=%s&prevExist=true' % (serviceName, ttl)
+            async with sess.put(url, headers=self.headers, timeout=self.timeout) as r:
+                text = await r.text()
+                print('[etcd] regist dir', text, r.status)
+            if address:
+                key  = address + ':' + str(port)
+            else:
+                key = local_ip() + ':' + str(port)
+            val = key
+            url = self.baseUrl + '/v2/keys/sunyata-services/%s/%s?value=%s&ttl=%s' % (serviceName, key, val, ttl)
+            async with sess.put(url, headers=self.headers, timeout=self.timeout) as r:
+                text = await r.text()
+                print('[etcd] regist key', text, r.status)
 
-    def getServiceInstanceList(self, serviceName: str) -> list:
-        url = self.baseUrl + '/v2/keys/sunyata-services/%s' % serviceName
-        r = requests.get(url, timeout=self.timeout, headers=self.headers)
-        dic = ujson.loads(r.text)
-        nodes = dic.get('node').get('nodes', [])
-        instanceList = []
-        for node in nodes:
-            value = node.get('value')
-            ip, port = value.split(':')
-            instance = Instance(
-                service=serviceName,
-                address=ip,
-                port=int(port)
-            )
-            instanceList.append(instance)
-        return instanceList
+    async def getServiceInstanceList(self, serviceName: str) -> list:
+        async with aiohttp.ClientSession() as sess:
+            url = self.baseUrl + '/v2/keys/sunyata-services/%s' % serviceName
+            async with sess.get(url, timeout=self.timeout, headers=self.headers) as r:
+                text = await r.text()
+                dic = ujson.loads(text)
+                nodes = dic.get('node').get('nodes', [])
+                instanceList = []
+                for node in nodes:
+                    value = node.get('value')
+                    ip, port = value.split(':')
+                    instance = Instance(
+                        service=serviceName,
+                        address=ip,
+                        port=int(port)
+                    )
+                    instanceList.append(instance)
+                return instanceList
     
-    def ttlHeartbeat(self, service, address, port):
-        self.registService(serviceName=service, address=address, port=port)
+    async def ttlHeartbeat(self, service, address, port):
+        await self.registService(serviceName=service, address=address, port=port)
```

### Comparing `sunyata-0.0.38/sunyata/http/server.py` & `sunyata-0.0.39/sunyata/http/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/transport.py` & `sunyata-0.0.39/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/request.py` & `sunyata-0.0.39/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/response.py` & `sunyata-0.0.39/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/factory.py` & `sunyata-0.0.39/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/rawserver.py` & `sunyata-0.0.39/sunyata/http/rawserver.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/http/status.py` & `sunyata-0.0.39/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/cache_wrap.py` & `sunyata-0.0.39/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/rpc/serialize.py` & `sunyata-0.0.39/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/rpc/server.py` & `sunyata-0.0.39/sunyata/rpc/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,30 +156,23 @@
         func, args, kwargs = self.protocal.parseRequest(request)
         resp = self.run(func, args, kwargs)
         resp = self.protocal.serialize(resp)
         return resp
     
     async def asyncServe(self):
         tasks = []
-        tasks.append(self.app.asyncServe())
+        tasks.append(asyncio.create_task(self.app.asyncServe()))
         if self.discovery and self.discoveryConfig:
             registTask = asyncio.create_task(self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True))
             tasks.append(registTask)
         await asyncio.wait(tasks)
 
     def serve(self):
-        asyncio.run(self.asyncServe())
-        """
-        tRegist = None
-        if self.discovery and self.discoveryConfig:
-            self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
-        self.printLogo()
         print('http rpc running on http://%s:%s' % (self.host, self.port) )
-        self.app.serve()
-        """
+        asyncio.run(self.asyncServe())
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
         self.host = host
```

### Comparing `sunyata-0.0.38/sunyata/rpc/discovery.py` & `sunyata-0.0.39/sunyata/rpc/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,37 +30,37 @@
         if self.consulHost and self.consulPort:
             self.api = ConsulApi(consulHost, consulPort, consulToken)
         if self.etcdHost and self.etcdPort:
             self.api = EtcdApi(etcdHost, etcdPort)
         self.instanceList = []
         self.heartbeatInterval = 15
 
-    def doHeartbeat(self, service, address, port, interval):
-        while 1:
-            try:
-                self.api.ttlHeartbeat(service, address, port)
-            except:
-                pass
-            time.sleep(interval)
+    #def doHeartbeat(self, service, address, port, interval):
+    #    while 1:
+    #        try:
+    #            self.api.ttlHeartbeat(service, address, port)
+    #        except:
+    #            pass
+    #        time.sleep(interval)
     
     async def asyncDoHeartbeat(self, service, address, port, interval):
         while 1:
             try:
-                self.api.ttlHeartbeat(service, address, port)
+                await self.api.ttlHeartbeat(service, address, port)
             except:
                 pass
             await asyncio.sleep(interval)
 
-    def regist(self, service, address, port, ttlHeartBeat = True):
-        self.api.registService(serviceName = service, address = address, port=port)
-        if ttlHeartBeat:
-            t = threading.Thread(target=self.doHeartbeat, args=(service, address, port, self.heartbeatInterval))
-            t.setDaemon(True)
-            t.start()
+    #def regist(self, service, address, port, ttlHeartBeat = True):
+    #    self.api.registService(serviceName = service, address = address, port=port)
+    #    if ttlHeartBeat:
+    #        t = threading.Thread(target=self.doHeartbeat, args=(service, address, port, self.heartbeatInterval))
+    #        t.setDaemon(True)
+    #        t.start()
 
     async def asyncRegist(self, service, address, port, ttlHeartBeat = True):
-        self.api.registService(serviceName = service, address = address, port=port)
+        await self.api.registService(serviceName = service, address = address, port=port)
         await self.asyncDoHeartbeat(service, address, port, self.heartbeatInterval)
 
-    def getInstanceList(self, service):
-        instanceList = self.api.getServiceInstanceList(service)
+    async def getInstanceList(self, service):
+        instanceList = await self.api.getServiceInstanceList(service)
         return instanceList
```

### Comparing `sunyata-0.0.38/sunyata/rpc/transport.py` & `sunyata-0.0.39/sunyata/rpc/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from socket import *
 import struct
-import requests
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from sunyata.rpc.const import SERVER_TIMEOUT
 from sunyata.rpc.compress import RpcCompress
+import aiohttp
 
 
 class RpcTransport(object): 
 
     def close(self):
         pass
 
@@ -219,37 +218,30 @@
         UdpTransport.__init__(self, host, port)
         self.timeout = timeout
         self.socket.settimeout(self.timeout)
 
 
 class HttpTransport(RpcTransport):
 
-    __slots__ = ('host', 'port', 'timeout', 'poolConnection', 'poolMaxSize', 'maxRetries', 'requestSession', 'url', 'headers')
-
     def __init__(self, host, port, timeout = 10, poolConnection=20, poolMaxSize=20, maxRetries=2):
         RpcTransport.__init__(self)
         self.host = host
         self.port = port
         self.timeout = timeout
-        self.poolConnection = poolConnection
-        self.poolMaxSize = poolMaxSize
-        self.maxRetries = maxRetries
-        self.requestSession = requests.Session()
-        self.requestSession.mount('http://', requests.adapters.HTTPAdapter(pool_connections=self.poolConnection, pool_maxsize=self.poolMaxSize, max_retries=self.maxRetries))
         self.url = self.makeUrl()
         self.headers = {
             'Content-type' : 'application/octet-stream'
         }
-        requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
     def makeUrl(self):
         return "http://%s:%s/" % (self.host, self.port)
 
-    def send(self, msg):
+    async def send(self, msg):
         isEnableCompress = b'0'
         if len(msg) >= RpcCompress.enableCompressLen:
             isEnableCompress = b'1'
             msg = RpcCompress.compress(msg)
         msg = isEnableCompress + msg
-        r = self.requestSession.post(self.url, headers = {}, data=msg, timeout = self.timeout)
-        resp = r.content
-        return resp
+        async with aiohttp.ClientSession() as sess:
+            async with sess.post(self.url, headers = {}, data=msg, timeout = self.timeout) as r:
+                content = await r.read()
+                return content
```

### Comparing `sunyata-0.0.38/sunyata/rpc/client.py` & `sunyata-0.0.39/sunyata/rpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from sunyata.rpc.protocal import TcpProtocal, UdpProtocal, HttpProtocal, RpcProtocal, ClientUdpProtocal
 from sunyata.rpc.exception import FuncNotFoundException
 from sunyata.rpc.discovery import DiscoveryConfig
 from sunyata.rpc.discovery import RpcDiscovery
 from sunyata.wrap import retryTimes
 import socket
+import asyncio
+
 
 class Address(object):
 
     __slots__ = ('host', 'port')
 
     def __init__(self, host, port):
         self.host = host
@@ -45,15 +47,15 @@
         self.serversCount = len(self.servers)
         self.serversProtocalMap = {}
         self.serverIndex = 0
         self.lastServer = ''
         self.timeout = 10
 
     def getInstance(self):
-        instanceList = self.discovery.getInstanceList(self.discoveryConfig.serviceName)
+        instanceList = asyncio.run(self.discovery.getInstanceList(self.discoveryConfig.serviceName))
         instanceLength  = len(instanceList)
         if instanceLength == 0:
             raise Exception('no instance found')
         index = self.instanceIndex % instanceLength
         self.instanceIndex = self.instanceIndex + 1
         return instanceList[index]
 
@@ -209,15 +211,15 @@
         self.beforeCall()
         package = {
             'func' : func,
             'args' : args,
             'kwargs' : kwargs,
         }
         msg = self.protocal.serialize(package)
-        respmsg = self.protocal.transport.send(msg)
+        respmsg = asyncio.run(self.protocal.transport.send(msg))
         resp = self.protocal.unserialize(respmsg)
         if isinstance(resp, FuncNotFoundException):
             raise resp
         return resp
 
     def getProtocalInstance(self, instance):
         key = "%s:%s:%s" % (instance.service, instance.address, instance.port)
```

### Comparing `sunyata-0.0.38/sunyata/rpc/method.py` & `sunyata-0.0.39/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/rpc/protocal.py` & `sunyata-0.0.39/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/table_writer.py` & `sunyata-0.0.39/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/sunyata/wrap.py` & `sunyata-0.0.39/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.38/README.md` & `sunyata-0.0.39/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - [服务发现](#服务发现)
   - [健康检查](#健康检查)
   - [快速开始](#快速开始-1)
   - [完整的服务端示例 (UDP/HTTP调用方式相同)](#完整的服务端示例-udphttp调用方式相同)
   - [完整的客户端示例（UDP/HTTP调用方式相同）](#完整的客户端示例udphttp调用方式相同)
 - [数据压缩](#数据压缩)
 - [内置Web框架](#内置web框架)
+- [微服务案例](#微服务案例)
 
 ## 简介
 sunyata是一个Python3 RPC框架，client和server既可以直连，也可以通过Consul或ETCD做服务注册发现。
 
 ## 特性
 - 像本地函数一样调用
 - 使用简单，用户只需要关注业务即可
@@ -249,15 +250,15 @@
 > 2.ServiceName 参数用于标记服务端名称，并通过服务名称进行服务发现，需要保证全局唯一 
 > 3.serviceHost和servicePort参数指定服务端监听的端口和地址
 
 - 第二步、调用setDiscoverConfig()方法将DiscoveryConfig对象传入
 - 第三步，调用serve()方法，开始处理请求
 
 ### 完整的服务端示例
-```
+```python
 from sunyata.rpc.server import HttpRpcServer
 from sunyata.rpc.discovery import DiscoveryConfig
 from sunyata.util import local_ip
 
 def sayHello(name): 
     return 'hello ' + name
 
@@ -270,15 +271,15 @@
     servicePort = 10031
 )
 server.setDiscoverConfig(disconf)
 server.regist(sayHello)
 server.serve()
 ```
 ### 完整的客户端示例
-```
+```python
 from sunyata.rpc.client import HttpRpcClient
 from sunyata.rpc.discovery import DiscoveryConfig
 
 client = HttpRpcClient()
 disconf = DiscoveryConfig(
     etcdHost='192.168.19.103',
     etcdPort=2379,
@@ -308,11 +309,50 @@
     name = request.data.get('name', '')
     return 'Hello ' + name
 
 hs = HttpServer(bind='0.0.0.0', port=9989)
 hs.serve()
 ```
 
+## 微服务案例
+下面是一个dns查询场景的微服务案例,dns_service.py负责提供底层dns查询服务,dns_web.py启动http api负责提供对外接口。dns_web与dns_service之间通过rpc进行通信。
+
+dns_service.py
+```python
+from sunyata.rpc.server import HttpRpcServer, rpc
+
+@rpc
+class DnsService(object):
+
+    def query(self, domain):
+        print('domain', domain)
+        return domain + ' A IN 192.168.1.1'
+
+rpcServer = HttpRpcServer(host='0.0.0.0', port=9988)
+rpcServer.serve()
+```
+
+dns_web.py
+```python
+from sunyata.http.server import HttpServer, route
+from sunyata.rpc.client import HttpRpcClient
+
+@route('/query', methods=['GET'])
+def query(request):
+    domain = request.data.get('domain')
+    cli = HttpRpcClient('127.0.0.1', 9988)
+    ip = cli.DnsService.query(domain)
+    return ip
+
+app = HttpServer()
+app.serve()
+```
+
+请求dns_web curl 'http://127.0.0.1:9989/query?domain=www.a.com' 返回  www.a.com A IN 192.168.1.1
+
+### 局限性
+由于底层通过python特有的pickle方式进行序列化，目前只支持python语言编写的服务之间的rpc通信，暂不支持其他语言。好处是不需要
+编写protobuf文件。
 
 [![Stargazers repo roster for @lycclsltt/sunyata](https://reporoster.com/stars/lycclsltt/sunyata)](https://github.com/lycclsltt/sunyata/stargazers)
 
 [![Forkers repo roster for @lycclsltt/sunyata](https://reporoster.com/forks/lycclsltt/sunyata)](https://github.com/lycclsltt/sunyata/network/members)
```

### Comparing `sunyata-0.0.38/setup.py` & `sunyata-0.0.39/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-DEFINE_VERSION = '0.0.38'
+DEFINE_VERSION = '0.0.39'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
-    'requests==2.25.1',
     'ujson==1.35',
-    'uvloop==0.19.0'
-    'uvicorn==0.18.0'
+    'uvloop==0.19.0',
+    'uvicorn==0.18.0',
+    'aiohttp==3.8.4',
     #'PyMySQL==0.10.1',
     #'DBUtils==1.3',
 ]
 
 setup(
     name='sunyata',
     version=DEFINE_VERSION,
```

