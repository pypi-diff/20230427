# Comparing `tmp/txtai-5.5.0.tar.gz` & `tmp/txtai-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/txtai-5.5.0.tar", last modified: Thu Apr 20 14:38:40 2023, max compression
+gzip compressed data, was "dist/txtai-5.5.1.tar", last modified: Thu Apr 27 19:45:38 2023, max compression
```

## Comparing `txtai-5.5.0.tar` & `txtai-5.5.1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-20 14:38:40.000000 txtai-5.5.0/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    27709 2023-04-18 21:57:55.000000 txtai-5.5.0/README.md
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2023-04-20 14:38:40.000000 txtai-5.5.0/setup.cfg
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3353 2023-04-17 19:47:20.000000 txtai-5.5.0/setup.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      269 2023-03-06 16:30:04.000000 txtai-5.5.0/src/python/txtai/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/ann/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      148 2021-02-26 23:19:14.000000 txtai-5.5.0/src/python/txtai/ann/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2022-12-16 18:47:06.000000 txtai-5.5.0/src/python/txtai/ann/annoy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3193 2023-04-20 13:57:16.000000 txtai-5.5.0/src/python/txtai/ann/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1287 2022-09-20 16:18:14.000000 txtai-5.5.0/src/python/txtai/ann/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3926 2023-02-17 00:05:12.000000 txtai-5.5.0/src/python/txtai/ann/faiss.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3170 2022-09-12 14:07:23.000000 txtai-5.5.0/src/python/txtai/ann/hnsw.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/api/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      393 2021-11-28 02:00:12.000000 txtai-5.5.0/src/python/txtai/api/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2013 2022-03-24 13:11:27.000000 txtai-5.5.0/src/python/txtai/api/application.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3163 2023-02-06 00:08:29.000000 txtai-5.5.0/src/python/txtai/api/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     6714 2021-12-23 01:22:00.000000 txtai-5.5.0/src/python/txtai/api/cluster.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-5.5.0/src/python/txtai/api/extension.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      634 2022-09-20 17:18:44.000000 txtai-5.5.0/src/python/txtai/api/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/api/routers/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      357 2022-01-25 18:17:11.000000 txtai-5.5.0/src/python/txtai/api/routers/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      676 2023-03-21 17:12:03.000000 txtai-5.5.0/src/python/txtai/api/routers/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4195 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/embeddings.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      742 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1147 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/objects.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      704 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1123 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      738 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/tabular.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      717 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      730 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1207 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/translation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      528 2023-03-21 17:17:53.000000 txtai-5.5.0/src/python/txtai/api/routers/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/app/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-5.5.0/src/python/txtai/app/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21429 2023-04-17 13:39:45.000000 txtai-5.5.0/src/python/txtai/app/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/archive/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-5.5.0/src/python/txtai/archive/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-5.5.0/src/python/txtai/archive/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-02-19 18:17:27.000000 txtai-5.5.0/src/python/txtai/archive/compress.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-5.5.0/src/python/txtai/archive/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-02-19 00:23:52.000000 txtai-5.5.0/src/python/txtai/archive/tar.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-02-19 18:58:42.000000 txtai-5.5.0/src/python/txtai/archive/zip.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/cloud/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-5.5.0/src/python/txtai/cloud/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-5.5.0/src/python/txtai/cloud/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-5.5.0/src/python/txtai/cloud/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-5.5.0/src/python/txtai/cloud/hub.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2983 2023-02-19 00:21:57.000000 txtai-5.5.0/src/python/txtai/cloud/storage.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/console/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-5.5.0/src/python/txtai/console/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-5.5.0/src/python/txtai/console/__main__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-5.5.0/src/python/txtai/console/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/data/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-5.5.0/src/python/txtai/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-5.5.0/src/python/txtai/data/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-5.5.0/src/python/txtai/data/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-5.5.0/src/python/txtai/data/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-5.5.0/src/python/txtai/data/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-5.5.0/src/python/txtai/data/texts.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-5.5.0/src/python/txtai/data/tokens.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-04-18 15:03:48.000000 txtai-5.5.0/src/python/txtai/database/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8179 2023-04-20 11:23:56.000000 txtai-5.5.0/src/python/txtai/database/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1982 2023-04-18 22:29:58.000000 txtai-5.5.0/src/python/txtai/database/duckdb.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/encoder/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-5.5.0/src/python/txtai/database/encoder/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-5.5.0/src/python/txtai/database/encoder/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-5.5.0/src/python/txtai/database/encoder/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2022-02-09 11:29:07.000000 txtai-5.5.0/src/python/txtai/database/encoder/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      428 2022-07-21 19:55:46.000000 txtai-5.5.0/src/python/txtai/database/encoder/pickle.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1423 2023-04-20 11:15:45.000000 txtai-5.5.0/src/python/txtai/database/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16339 2023-04-18 21:23:20.000000 txtai-5.5.0/src/python/txtai/database/filedb.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/database/sql/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-5.5.0/src/python/txtai/database/sql/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-5.5.0/src/python/txtai/database/sql/aggregate.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-01-09 21:32:56.000000 txtai-5.5.0/src/python/txtai/database/sql/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13762 2022-11-19 16:44:34.000000 txtai-5.5.0/src/python/txtai/database/sql/expression.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-5.5.0/src/python/txtai/database/sql/token.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1390 2023-04-18 21:21:53.000000 txtai-5.5.0/src/python/txtai/database/sqlite.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/embeddings/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      283 2023-03-02 21:46:33.000000 txtai-5.5.0/src/python/txtai/embeddings/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24711 2023-03-10 18:45:22.000000 txtai-5.5.0/src/python/txtai/embeddings/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1882 2022-07-21 19:57:10.000000 txtai-5.5.0/src/python/txtai/embeddings/documents.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4142 2022-03-30 19:35:55.000000 txtai-5.5.0/src/python/txtai/embeddings/explain.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-03-10 18:14:43.000000 txtai-5.5.0/src/python/txtai/embeddings/functions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-5.5.0/src/python/txtai/embeddings/query.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2709 2022-12-12 13:51:32.000000 txtai-5.5.0/src/python/txtai/embeddings/reducer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6767 2022-12-12 16:52:20.000000 txtai-5.5.0/src/python/txtai/embeddings/search.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-5.5.0/src/python/txtai/embeddings/terms.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4956 2023-03-09 16:16:39.000000 txtai-5.5.0/src/python/txtai/embeddings/transform.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/graph/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-5.5.0/src/python/txtai/graph/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    15350 2023-04-20 13:59:43.000000 txtai-5.5.0/src/python/txtai/graph/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2022-09-20 16:16:49.000000 txtai-5.5.0/src/python/txtai/graph/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4994 2023-03-09 16:25:39.000000 txtai-5.5.0/src/python/txtai/graph/networkx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4595 2022-09-30 13:52:22.000000 txtai-5.5.0/src/python/txtai/graph/topics.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/models/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      195 2023-01-31 14:10:56.000000 txtai-5.5.0/src/python/txtai/models/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4424 2022-10-19 19:11:48.000000 txtai-5.5.0/src/python/txtai/models/models.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-5.5.0/src/python/txtai/models/onnx.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3747 2023-01-28 02:01:25.000000 txtai-5.5.0/src/python/txtai/models/pooling.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-5.5.0/src/python/txtai/models/registry.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-5.5.0/src/python/txtai/models/tokendetection.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      307 2021-11-28 01:42:36.000000 txtai-5.5.0/src/python/txtai/pipeline/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2022-11-29 16:35:29.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-03-11 15:52:28.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/texttospeech.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6548 2022-12-03 12:49:26.000000 txtai-5.5.0/src/python/txtai/pipeline/audio/transcription.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      536 2022-12-02 16:07:11.000000 txtai-5.5.0/src/python/txtai/pipeline/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/data/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2021-11-18 20:49:26.000000 txtai-5.5.0/src/python/txtai/pipeline/data/__init__.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3399 2021-11-22 21:19:44.000000 txtai-5.5.0/src/python/txtai/pipeline/data/segmentation.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-03-01 15:20:17.000000 txtai-5.5.0/src/python/txtai/pipeline/data/tabular.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2182 2022-03-24 17:06:47.000000 txtai-5.5.0/src/python/txtai/pipeline/data/textractor.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1632 2021-11-18 20:09:32.000000 txtai-5.5.0/src/python/txtai/pipeline/data/tokenizer.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2022-09-20 16:19:32.000000 txtai-5.5.0/src/python/txtai/pipeline/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3687 2022-12-02 16:06:16.000000 txtai-5.5.0/src/python/txtai/pipeline/hfmodel.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2299 2022-10-17 13:20:55.000000 txtai-5.5.0/src/python/txtai/pipeline/hfpipeline.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/image/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2022-03-04 16:47:13.000000 txtai-5.5.0/src/python/txtai/pipeline/image/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1503 2022-10-16 13:16:42.000000 txtai-5.5.0/src/python/txtai/pipeline/image/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2022-03-07 14:33:13.000000 txtai-5.5.0/src/python/txtai/pipeline/image/imagehash.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2706 2022-01-25 18:50:43.000000 txtai-5.5.0/src/python/txtai/pipeline/image/objects.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2021-11-19 14:42:33.000000 txtai-5.5.0/src/python/txtai/pipeline/nop.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2022-10-17 13:21:17.000000 txtai-5.5.0/src/python/txtai/pipeline/tensors.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/text/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      348 2023-01-31 14:01:28.000000 txtai-5.5.0/src/python/txtai/pipeline/text/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2599 2023-02-19 19:08:49.000000 txtai-5.5.0/src/python/txtai/pipeline/text/crossencoder.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2519 2022-01-27 11:33:22.000000 txtai-5.5.0/src/python/txtai/pipeline/text/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16184 2023-03-29 19:46:04.000000 txtai-5.5.0/src/python/txtai/pipeline/text/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2048 2023-04-14 21:51:28.000000 txtai-5.5.0/src/python/txtai/pipeline/text/generator.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2022-10-25 15:49:15.000000 txtai-5.5.0/src/python/txtai/pipeline/text/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1397 2021-11-29 23:27:03.000000 txtai-5.5.0/src/python/txtai/pipeline/text/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-01-31 14:00:05.000000 txtai-5.5.0/src/python/txtai/pipeline/text/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2237 2022-10-25 17:47:04.000000 txtai-5.5.0/src/python/txtai/pipeline/text/similarity.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2816 2022-11-18 18:40:05.000000 txtai-5.5.0/src/python/txtai/pipeline/text/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-03-11 15:52:58.000000 txtai-5.5.0/src/python/txtai/pipeline/text/translation.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/pipeline/train/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2021-11-18 20:49:46.000000 txtai-5.5.0/src/python/txtai/pipeline/train/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5438 2022-10-19 20:33:27.000000 txtai-5.5.0/src/python/txtai/pipeline/train/hfonnx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8164 2023-02-17 02:35:33.000000 txtai-5.5.0/src/python/txtai/pipeline/train/hftrainer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-03-10 21:59:48.000000 txtai-5.5.0/src/python/txtai/pipeline/train/mlonnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/scoring/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      131 2021-02-26 23:19:24.000000 txtai-5.5.0/src/python/txtai/scoring/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9258 2022-12-28 00:02:56.000000 txtai-5.5.0/src/python/txtai/scoring/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      668 2022-10-04 13:39:24.000000 txtai-5.5.0/src/python/txtai/scoring/bm25.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      875 2022-09-12 14:13:51.000000 txtai-5.5.0/src/python/txtai/scoring/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2022-10-04 13:39:24.000000 txtai-5.5.0/src/python/txtai/scoring/sif.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/util/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       56 2022-11-01 17:14:15.000000 txtai-5.5.0/src/python/txtai/util/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2022-09-20 17:08:45.000000 txtai-5.5.0/src/python/txtai/util/resolver.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/vectors/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-5.5.0/src/python/txtai/vectors/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5174 2023-04-20 14:01:08.000000 txtai-5.5.0/src/python/txtai/vectors/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      781 2022-12-12 14:03:21.000000 txtai-5.5.0/src/python/txtai/vectors/external.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1759 2022-05-12 13:38:48.000000 txtai-5.5.0/src/python/txtai/vectors/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1940 2023-02-19 18:06:08.000000 txtai-5.5.0/src/python/txtai/vectors/transformers.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6572 2023-03-02 21:45:59.000000 txtai-5.5.0/src/python/txtai/vectors/words.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/workflow/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-5.5.0/src/python/txtai/workflow/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-5.5.0/src/python/txtai/workflow/execute.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai/workflow/task/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-5.5.0/src/python/txtai/workflow/task/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-5.5.0/src/python/txtai/workflow/task/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-5.5.0/src/python/txtai/workflow/task/console.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-5.5.0/src/python/txtai/workflow/task/export.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-5.5.0/src/python/txtai/workflow/task/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-5.5.0/src/python/txtai/workflow/task/file.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-5.5.0/src/python/txtai/workflow/task/image.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1265 2021-11-29 23:29:08.000000 txtai-5.5.0/src/python/txtai/workflow/task/retrieve.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-5.5.0/src/python/txtai/workflow/task/service.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2985 2022-10-12 14:46:21.000000 txtai-5.5.0/src/python/txtai/workflow/task/storage.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-5.5.0/src/python/txtai/workflow/task/stream.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3511 2023-03-02 22:34:44.000000 txtai-5.5.0/src/python/txtai/workflow/task/template.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-5.5.0/src/python/txtai/workflow/task/url.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-5.5.0/src/python/txtai/workflow/task/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6063 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/SOURCES.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/dependency_links.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2054 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/requires.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2023-04-20 14:38:40.000000 txtai-5.5.0/src/python/txtai.egg-info/top_level.txt
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-27 19:45:38.000000 txtai-5.5.1/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    27709 2023-04-18 21:57:55.000000 txtai-5.5.1/README.md
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2023-04-27 19:45:38.000000 txtai-5.5.1/setup.cfg
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3353 2023-04-27 18:29:20.000000 txtai-5.5.1/setup.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      269 2023-04-27 18:29:29.000000 txtai-5.5.1/src/python/txtai/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/ann/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      148 2021-02-26 23:19:14.000000 txtai-5.5.1/src/python/txtai/ann/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2023-04-26 18:04:54.000000 txtai-5.5.1/src/python/txtai/ann/annoy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3193 2023-04-20 13:57:16.000000 txtai-5.5.1/src/python/txtai/ann/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1287 2022-09-20 16:18:14.000000 txtai-5.5.1/src/python/txtai/ann/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3926 2023-02-17 00:05:12.000000 txtai-5.5.1/src/python/txtai/ann/faiss.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3170 2022-09-12 14:07:23.000000 txtai-5.5.1/src/python/txtai/ann/hnsw.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/api/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      393 2021-11-28 02:00:12.000000 txtai-5.5.1/src/python/txtai/api/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2013 2022-03-24 13:11:27.000000 txtai-5.5.1/src/python/txtai/api/application.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3163 2023-02-06 00:08:29.000000 txtai-5.5.1/src/python/txtai/api/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     6714 2021-12-23 01:22:00.000000 txtai-5.5.1/src/python/txtai/api/cluster.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-5.5.1/src/python/txtai/api/extension.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      634 2022-09-20 17:18:44.000000 txtai-5.5.1/src/python/txtai/api/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/api/routers/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      357 2022-01-25 18:17:11.000000 txtai-5.5.1/src/python/txtai/api/routers/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      676 2023-03-21 17:12:03.000000 txtai-5.5.1/src/python/txtai/api/routers/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4195 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/embeddings.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      742 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1147 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      704 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1123 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      738 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      717 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      730 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1207 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/translation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      528 2023-03-21 17:17:53.000000 txtai-5.5.1/src/python/txtai/api/routers/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/app/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-5.5.1/src/python/txtai/app/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21429 2023-04-17 13:39:45.000000 txtai-5.5.1/src/python/txtai/app/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/archive/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-5.5.1/src/python/txtai/archive/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-5.5.1/src/python/txtai/archive/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-02-19 18:17:27.000000 txtai-5.5.1/src/python/txtai/archive/compress.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-5.5.1/src/python/txtai/archive/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-02-19 00:23:52.000000 txtai-5.5.1/src/python/txtai/archive/tar.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      778 2023-02-19 18:58:42.000000 txtai-5.5.1/src/python/txtai/archive/zip.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/cloud/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-5.5.1/src/python/txtai/cloud/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-5.5.1/src/python/txtai/cloud/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-5.5.1/src/python/txtai/cloud/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-5.5.1/src/python/txtai/cloud/hub.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2983 2023-02-19 00:21:57.000000 txtai-5.5.1/src/python/txtai/cloud/storage.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/console/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-5.5.1/src/python/txtai/console/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-5.5.1/src/python/txtai/console/__main__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-5.5.1/src/python/txtai/console/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/data/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-5.5.1/src/python/txtai/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-5.5.1/src/python/txtai/data/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-5.5.1/src/python/txtai/data/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-5.5.1/src/python/txtai/data/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-5.5.1/src/python/txtai/data/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-5.5.1/src/python/txtai/data/texts.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-5.5.1/src/python/txtai/data/tokens.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/database/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-04-18 15:03:48.000000 txtai-5.5.1/src/python/txtai/database/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8179 2023-04-20 11:23:56.000000 txtai-5.5.1/src/python/txtai/database/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2254 2023-04-21 15:03:45.000000 txtai-5.5.1/src/python/txtai/database/duckdb.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/database/encoder/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-5.5.1/src/python/txtai/database/encoder/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-5.5.1/src/python/txtai/database/encoder/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-5.5.1/src/python/txtai/database/encoder/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2023-04-21 14:52:54.000000 txtai-5.5.1/src/python/txtai/database/encoder/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      428 2022-07-21 19:55:46.000000 txtai-5.5.1/src/python/txtai/database/encoder/pickle.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1423 2023-04-20 11:15:45.000000 txtai-5.5.1/src/python/txtai/database/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16339 2023-04-18 21:23:20.000000 txtai-5.5.1/src/python/txtai/database/filedb.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/database/sql/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-5.5.1/src/python/txtai/database/sql/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-5.5.1/src/python/txtai/database/sql/aggregate.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-01-09 21:32:56.000000 txtai-5.5.1/src/python/txtai/database/sql/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13762 2022-11-19 16:44:34.000000 txtai-5.5.1/src/python/txtai/database/sql/expression.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-5.5.1/src/python/txtai/database/sql/token.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1390 2023-04-18 21:21:53.000000 txtai-5.5.1/src/python/txtai/database/sqlite.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/embeddings/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      283 2023-03-02 21:46:33.000000 txtai-5.5.1/src/python/txtai/embeddings/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24711 2023-03-10 18:45:22.000000 txtai-5.5.1/src/python/txtai/embeddings/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1882 2022-07-21 19:57:10.000000 txtai-5.5.1/src/python/txtai/embeddings/documents.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4142 2022-03-30 19:35:55.000000 txtai-5.5.1/src/python/txtai/embeddings/explain.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-03-10 18:14:43.000000 txtai-5.5.1/src/python/txtai/embeddings/functions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-5.5.1/src/python/txtai/embeddings/query.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2709 2022-12-12 13:51:32.000000 txtai-5.5.1/src/python/txtai/embeddings/reducer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6767 2022-12-12 16:52:20.000000 txtai-5.5.1/src/python/txtai/embeddings/search.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-5.5.1/src/python/txtai/embeddings/terms.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4956 2023-03-09 16:16:39.000000 txtai-5.5.1/src/python/txtai/embeddings/transform.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/graph/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-5.5.1/src/python/txtai/graph/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    15350 2023-04-20 13:59:43.000000 txtai-5.5.1/src/python/txtai/graph/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2022-09-20 16:16:49.000000 txtai-5.5.1/src/python/txtai/graph/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4994 2023-03-09 16:25:39.000000 txtai-5.5.1/src/python/txtai/graph/networkx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4595 2022-09-30 13:52:22.000000 txtai-5.5.1/src/python/txtai/graph/topics.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/models/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      195 2023-01-31 14:10:56.000000 txtai-5.5.1/src/python/txtai/models/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4424 2022-10-19 19:11:48.000000 txtai-5.5.1/src/python/txtai/models/models.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-5.5.1/src/python/txtai/models/onnx.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3747 2023-01-28 02:01:25.000000 txtai-5.5.1/src/python/txtai/models/pooling.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-5.5.1/src/python/txtai/models/registry.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-5.5.1/src/python/txtai/models/tokendetection.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      307 2021-11-28 01:42:36.000000 txtai-5.5.1/src/python/txtai/pipeline/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/audio/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2022-11-29 16:35:29.000000 txtai-5.5.1/src/python/txtai/pipeline/audio/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-03-11 15:52:28.000000 txtai-5.5.1/src/python/txtai/pipeline/audio/texttospeech.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6548 2022-12-03 12:49:26.000000 txtai-5.5.1/src/python/txtai/pipeline/audio/transcription.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      536 2022-12-02 16:07:11.000000 txtai-5.5.1/src/python/txtai/pipeline/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/data/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2021-11-18 20:49:26.000000 txtai-5.5.1/src/python/txtai/pipeline/data/__init__.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3399 2023-04-21 14:50:36.000000 txtai-5.5.1/src/python/txtai/pipeline/data/segmentation.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-03-01 15:20:17.000000 txtai-5.5.1/src/python/txtai/pipeline/data/tabular.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2182 2022-03-24 17:06:47.000000 txtai-5.5.1/src/python/txtai/pipeline/data/textractor.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1632 2021-11-18 20:09:32.000000 txtai-5.5.1/src/python/txtai/pipeline/data/tokenizer.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2022-09-20 16:19:32.000000 txtai-5.5.1/src/python/txtai/pipeline/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3687 2022-12-02 16:06:16.000000 txtai-5.5.1/src/python/txtai/pipeline/hfmodel.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2299 2022-10-17 13:20:55.000000 txtai-5.5.1/src/python/txtai/pipeline/hfpipeline.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/image/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2022-03-04 16:47:13.000000 txtai-5.5.1/src/python/txtai/pipeline/image/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1503 2022-10-16 13:16:42.000000 txtai-5.5.1/src/python/txtai/pipeline/image/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2022-03-07 14:33:13.000000 txtai-5.5.1/src/python/txtai/pipeline/image/imagehash.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2706 2022-01-25 18:50:43.000000 txtai-5.5.1/src/python/txtai/pipeline/image/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2021-11-19 14:42:33.000000 txtai-5.5.1/src/python/txtai/pipeline/nop.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2022-10-17 13:21:17.000000 txtai-5.5.1/src/python/txtai/pipeline/tensors.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/text/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      348 2023-01-31 14:01:28.000000 txtai-5.5.1/src/python/txtai/pipeline/text/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2599 2023-02-19 19:08:49.000000 txtai-5.5.1/src/python/txtai/pipeline/text/crossencoder.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2519 2022-01-27 11:33:22.000000 txtai-5.5.1/src/python/txtai/pipeline/text/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16184 2023-03-29 19:46:04.000000 txtai-5.5.1/src/python/txtai/pipeline/text/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2048 2023-04-14 21:51:28.000000 txtai-5.5.1/src/python/txtai/pipeline/text/generator.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2022-10-25 15:49:15.000000 txtai-5.5.1/src/python/txtai/pipeline/text/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1397 2021-11-29 23:27:03.000000 txtai-5.5.1/src/python/txtai/pipeline/text/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      213 2023-01-31 14:00:05.000000 txtai-5.5.1/src/python/txtai/pipeline/text/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2237 2022-10-25 17:47:04.000000 txtai-5.5.1/src/python/txtai/pipeline/text/similarity.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2816 2022-11-18 18:40:05.000000 txtai-5.5.1/src/python/txtai/pipeline/text/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-03-11 15:52:58.000000 txtai-5.5.1/src/python/txtai/pipeline/text/translation.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/pipeline/train/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2021-11-18 20:49:46.000000 txtai-5.5.1/src/python/txtai/pipeline/train/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5438 2022-10-19 20:33:27.000000 txtai-5.5.1/src/python/txtai/pipeline/train/hfonnx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8164 2023-02-17 02:35:33.000000 txtai-5.5.1/src/python/txtai/pipeline/train/hftrainer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-03-10 21:59:48.000000 txtai-5.5.1/src/python/txtai/pipeline/train/mlonnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/scoring/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      131 2021-02-26 23:19:24.000000 txtai-5.5.1/src/python/txtai/scoring/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9258 2022-12-28 00:02:56.000000 txtai-5.5.1/src/python/txtai/scoring/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      668 2022-10-04 13:39:24.000000 txtai-5.5.1/src/python/txtai/scoring/bm25.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      875 2022-09-12 14:13:51.000000 txtai-5.5.1/src/python/txtai/scoring/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2022-10-04 13:39:24.000000 txtai-5.5.1/src/python/txtai/scoring/sif.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/util/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       56 2022-11-01 17:14:15.000000 txtai-5.5.1/src/python/txtai/util/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2022-09-20 17:08:45.000000 txtai-5.5.1/src/python/txtai/util/resolver.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/vectors/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-5.5.1/src/python/txtai/vectors/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5174 2023-04-20 14:01:08.000000 txtai-5.5.1/src/python/txtai/vectors/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      781 2022-12-12 14:03:21.000000 txtai-5.5.1/src/python/txtai/vectors/external.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1759 2022-05-12 13:38:48.000000 txtai-5.5.1/src/python/txtai/vectors/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1940 2023-02-19 18:06:08.000000 txtai-5.5.1/src/python/txtai/vectors/transformers.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6572 2023-03-02 21:45:59.000000 txtai-5.5.1/src/python/txtai/vectors/words.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/workflow/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-5.5.1/src/python/txtai/workflow/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-5.5.1/src/python/txtai/workflow/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-5.5.1/src/python/txtai/workflow/execute.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-5.5.1/src/python/txtai/workflow/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai/workflow/task/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-5.5.1/src/python/txtai/workflow/task/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-5.5.1/src/python/txtai/workflow/task/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-5.5.1/src/python/txtai/workflow/task/console.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-5.5.1/src/python/txtai/workflow/task/export.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-5.5.1/src/python/txtai/workflow/task/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-5.5.1/src/python/txtai/workflow/task/file.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-5.5.1/src/python/txtai/workflow/task/image.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1265 2021-11-29 23:29:08.000000 txtai-5.5.1/src/python/txtai/workflow/task/retrieve.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-5.5.1/src/python/txtai/workflow/task/service.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2985 2022-10-12 14:46:21.000000 txtai-5.5.1/src/python/txtai/workflow/task/storage.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-5.5.1/src/python/txtai/workflow/task/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3511 2023-03-02 22:34:44.000000 txtai-5.5.1/src/python/txtai/workflow/task/template.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-5.5.1/src/python/txtai/workflow/task/url.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-5.5.1/src/python/txtai/workflow/task/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    30293 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6063 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2054 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/requires.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2023-04-27 19:45:38.000000 txtai-5.5.1/src/python/txtai.egg-info/top_level.txt
```

### Comparing `txtai-5.5.0/PKG-INFO` & `txtai-5.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 5.5.0
+Version: 5.5.1
 Summary: Semantic search and workflows powered by language models
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: txtai Version: 5.5.0 Summary: Semantic search and
+Metadata-Version: 2.1 Name: txtai Version: 5.5.1 Summary: Semantic search and
 workflows powered by language models Home-page: https://github.com/neuml/txtai
 Author: NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue
 Tracker, https://github.com/neuml/txtai/issues Project-URL: Source Code, https:
 //github.com/neuml/txtai Description:
         [https://raw.githubusercontent.com/neuml/txtai/master/logo.png]
       **** Semantic search and workflows powered by language models ****
```

### Comparing `txtai-5.5.0/README.md` & `txtai-5.5.1/README.md`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/setup.py` & `txtai-5.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     + extras["pipeline"]
     + extras["similarity"]
     + extras["workflow"]
 )
 
 setup(
     name="txtai",
-    version="5.5.0",
+    version="5.5.1",
     author="NeuML",
     description="Semantic search and workflows powered by language models",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/neuml/txtai",
     project_urls={
         "Documentation": "https://github.com/neuml/txtai",
```

### Comparing `txtai-5.5.0/src/python/txtai/ann/annoy.py` & `txtai-5.5.1/src/python/txtai/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/ann/base.py` & `txtai-5.5.1/src/python/txtai/ann/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/ann/factory.py` & `txtai-5.5.1/src/python/txtai/ann/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/ann/faiss.py` & `txtai-5.5.1/src/python/txtai/ann/faiss.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/ann/hnsw.py` & `txtai-5.5.1/src/python/txtai/ann/hnsw.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/application.py` & `txtai-5.5.1/src/python/txtai/api/application.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/base.py` & `txtai-5.5.1/src/python/txtai/api/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/cluster.py` & `txtai-5.5.1/src/python/txtai/api/cluster.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/factory.py` & `txtai-5.5.1/src/python/txtai/api/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/caption.py` & `txtai-5.5.1/src/python/txtai/api/routers/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/embeddings.py` & `txtai-5.5.1/src/python/txtai/api/routers/embeddings.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/entity.py` & `txtai-5.5.1/src/python/txtai/api/routers/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/extractor.py` & `txtai-5.5.1/src/python/txtai/api/routers/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/labels.py` & `txtai-5.5.1/src/python/txtai/api/routers/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/objects.py` & `txtai-5.5.1/src/python/txtai/api/routers/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/segmentation.py` & `txtai-5.5.1/src/python/txtai/api/routers/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/similarity.py` & `txtai-5.5.1/src/python/txtai/api/routers/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/summary.py` & `txtai-5.5.1/src/python/txtai/api/routers/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/tabular.py` & `txtai-5.5.1/src/python/txtai/api/routers/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/textractor.py` & `txtai-5.5.1/src/python/txtai/api/routers/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/transcription.py` & `txtai-5.5.1/src/python/txtai/api/routers/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/translation.py` & `txtai-5.5.1/src/python/txtai/api/routers/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/api/routers/workflow.py` & `txtai-5.5.1/src/python/txtai/api/routers/workflow.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/app/base.py` & `txtai-5.5.1/src/python/txtai/app/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/archive/base.py` & `txtai-5.5.1/src/python/txtai/archive/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/archive/compress.py` & `txtai-5.5.1/src/python/txtai/archive/compress.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/archive/tar.py` & `txtai-5.5.1/src/python/txtai/archive/tar.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/archive/zip.py` & `txtai-5.5.1/src/python/txtai/archive/zip.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/cloud/base.py` & `txtai-5.5.1/src/python/txtai/cloud/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/cloud/factory.py` & `txtai-5.5.1/src/python/txtai/cloud/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/cloud/hub.py` & `txtai-5.5.1/src/python/txtai/cloud/hub.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/cloud/storage.py` & `txtai-5.5.1/src/python/txtai/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/console/base.py` & `txtai-5.5.1/src/python/txtai/console/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/base.py` & `txtai-5.5.1/src/python/txtai/data/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/labels.py` & `txtai-5.5.1/src/python/txtai/data/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/questions.py` & `txtai-5.5.1/src/python/txtai/data/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/sequences.py` & `txtai-5.5.1/src/python/txtai/data/sequences.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/texts.py` & `txtai-5.5.1/src/python/txtai/data/texts.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/data/tokens.py` & `txtai-5.5.1/src/python/txtai/data/tokens.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/base.py` & `txtai-5.5.1/src/python/txtai/database/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/duckdb.py` & `txtai-5.5.1/src/python/txtai/database/duckdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,36 @@
 DuckDB module
 """
 
 import os
 
 from tempfile import TemporaryDirectory
 
-import duckdb
+# Conditional import
+try:
+    import duckdb
+
+    DUCKDB = True
+except ImportError:
+    DUCKDB = False
 
 from .filedb import FileDB
 
 
 class DuckDB(FileDB):
     """
     Database instance backed by DuckDB.
     """
 
+    def __init__(self, config):
+        super().__init__(config)
+
+        if not DUCKDB:
+            raise ImportError('DuckDB is not available - install "database" extra to enable')
+
     def connect(self, path=":memory:"):
         # Create connection and start a transaction
         # pylint: disable=I1101
         connection = duckdb.connect(path)
         connection.begin()
 
         return connection
```

### Comparing `txtai-5.5.0/src/python/txtai/database/encoder/base.py` & `txtai-5.5.1/src/python/txtai/database/encoder/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/encoder/factory.py` & `txtai-5.5.1/src/python/txtai/database/encoder/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/encoder/image.py` & `txtai-5.5.1/src/python/txtai/database/encoder/image.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 ImageEncoder module
 """
 
 from io import BytesIO
 
-from .base import Encoder
-
 # Conditional import
 try:
     from PIL import Image
 
     PIL = True
 except ImportError:
     PIL = False
 
+from .base import Encoder
+
 
 class ImageEncoder(Encoder):
     """
     Encodes and decodes Image objects as compressed binary content, using the original image's algorithm.
     """
 
     def __init__(self):
```

### Comparing `txtai-5.5.0/src/python/txtai/database/factory.py` & `txtai-5.5.1/src/python/txtai/database/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/filedb.py` & `txtai-5.5.1/src/python/txtai/database/filedb.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/sql/aggregate.py` & `txtai-5.5.1/src/python/txtai/database/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/sql/base.py` & `txtai-5.5.1/src/python/txtai/database/sql/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/sql/expression.py` & `txtai-5.5.1/src/python/txtai/database/sql/expression.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/sql/token.py` & `txtai-5.5.1/src/python/txtai/database/sql/token.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/database/sqlite.py` & `txtai-5.5.1/src/python/txtai/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/base.py` & `txtai-5.5.1/src/python/txtai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/documents.py` & `txtai-5.5.1/src/python/txtai/embeddings/documents.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/explain.py` & `txtai-5.5.1/src/python/txtai/embeddings/explain.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/functions.py` & `txtai-5.5.1/src/python/txtai/embeddings/functions.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/query.py` & `txtai-5.5.1/src/python/txtai/embeddings/query.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/reducer.py` & `txtai-5.5.1/src/python/txtai/embeddings/reducer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/search.py` & `txtai-5.5.1/src/python/txtai/embeddings/search.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/terms.py` & `txtai-5.5.1/src/python/txtai/embeddings/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/embeddings/transform.py` & `txtai-5.5.1/src/python/txtai/embeddings/transform.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/graph/base.py` & `txtai-5.5.1/src/python/txtai/graph/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/graph/factory.py` & `txtai-5.5.1/src/python/txtai/graph/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/graph/networkx.py` & `txtai-5.5.1/src/python/txtai/graph/networkx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/graph/topics.py` & `txtai-5.5.1/src/python/txtai/graph/topics.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/models/models.py` & `txtai-5.5.1/src/python/txtai/models/models.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/models/onnx.py` & `txtai-5.5.1/src/python/txtai/models/onnx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/models/pooling.py` & `txtai-5.5.1/src/python/txtai/models/pooling.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/models/registry.py` & `txtai-5.5.1/src/python/txtai/models/registry.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/models/tokendetection.py` & `txtai-5.5.1/src/python/txtai/models/tokendetection.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/audio/texttospeech.py` & `txtai-5.5.1/src/python/txtai/pipeline/audio/texttospeech.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/audio/transcription.py` & `txtai-5.5.1/src/python/txtai/pipeline/audio/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/base.py` & `txtai-5.5.1/src/python/txtai/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/data/segmentation.py` & `txtai-5.5.1/src/python/txtai/pipeline/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/data/tabular.py` & `txtai-5.5.1/src/python/txtai/pipeline/data/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/data/textractor.py` & `txtai-5.5.1/src/python/txtai/pipeline/data/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/data/tokenizer.py` & `txtai-5.5.1/src/python/txtai/pipeline/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/factory.py` & `txtai-5.5.1/src/python/txtai/pipeline/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/hfmodel.py` & `txtai-5.5.1/src/python/txtai/pipeline/hfmodel.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/hfpipeline.py` & `txtai-5.5.1/src/python/txtai/pipeline/hfpipeline.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/image/caption.py` & `txtai-5.5.1/src/python/txtai/pipeline/image/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/image/imagehash.py` & `txtai-5.5.1/src/python/txtai/pipeline/image/imagehash.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/image/objects.py` & `txtai-5.5.1/src/python/txtai/pipeline/image/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/tensors.py` & `txtai-5.5.1/src/python/txtai/pipeline/tensors.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/crossencoder.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/crossencoder.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/entity.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/extractor.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/generator.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/generator.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/labels.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/questions.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/similarity.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/summary.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/text/translation.py` & `txtai-5.5.1/src/python/txtai/pipeline/text/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/train/hfonnx.py` & `txtai-5.5.1/src/python/txtai/pipeline/train/hfonnx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/train/hftrainer.py` & `txtai-5.5.1/src/python/txtai/pipeline/train/hftrainer.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/pipeline/train/mlonnx.py` & `txtai-5.5.1/src/python/txtai/pipeline/train/mlonnx.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/scoring/base.py` & `txtai-5.5.1/src/python/txtai/scoring/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/scoring/bm25.py` & `txtai-5.5.1/src/python/txtai/scoring/bm25.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/scoring/factory.py` & `txtai-5.5.1/src/python/txtai/scoring/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/scoring/sif.py` & `txtai-5.5.1/src/python/txtai/scoring/sif.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/util/resolver.py` & `txtai-5.5.1/src/python/txtai/util/resolver.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/vectors/base.py` & `txtai-5.5.1/src/python/txtai/vectors/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/vectors/external.py` & `txtai-5.5.1/src/python/txtai/vectors/external.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/vectors/factory.py` & `txtai-5.5.1/src/python/txtai/vectors/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/vectors/transformers.py` & `txtai-5.5.1/src/python/txtai/vectors/transformers.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/vectors/words.py` & `txtai-5.5.1/src/python/txtai/vectors/words.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/base.py` & `txtai-5.5.1/src/python/txtai/workflow/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/execute.py` & `txtai-5.5.1/src/python/txtai/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/factory.py` & `txtai-5.5.1/src/python/txtai/workflow/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/base.py` & `txtai-5.5.1/src/python/txtai/workflow/task/base.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/export.py` & `txtai-5.5.1/src/python/txtai/workflow/task/export.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/factory.py` & `txtai-5.5.1/src/python/txtai/workflow/task/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/file.py` & `txtai-5.5.1/src/python/txtai/workflow/task/file.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/image.py` & `txtai-5.5.1/src/python/txtai/workflow/task/image.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/retrieve.py` & `txtai-5.5.1/src/python/txtai/workflow/task/retrieve.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/service.py` & `txtai-5.5.1/src/python/txtai/workflow/task/service.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/storage.py` & `txtai-5.5.1/src/python/txtai/workflow/task/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/stream.py` & `txtai-5.5.1/src/python/txtai/workflow/task/stream.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai/workflow/task/template.py` & `txtai-5.5.1/src/python/txtai/workflow/task/template.py`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai.egg-info/PKG-INFO` & `txtai-5.5.1/src/python/txtai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 5.5.0
+Version: 5.5.1
 Summary: Semantic search and workflows powered by language models
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: txtai Version: 5.5.0 Summary: Semantic search and
+Metadata-Version: 2.1 Name: txtai Version: 5.5.1 Summary: Semantic search and
 workflows powered by language models Home-page: https://github.com/neuml/txtai
 Author: NeuML License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai Project-URL: Issue
 Tracker, https://github.com/neuml/txtai/issues Project-URL: Source Code, https:
 //github.com/neuml/txtai Description:
         [https://raw.githubusercontent.com/neuml/txtai/master/logo.png]
       **** Semantic search and workflows powered by language models ****
```

### Comparing `txtai-5.5.0/src/python/txtai.egg-info/SOURCES.txt` & `txtai-5.5.1/src/python/txtai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txtai-5.5.0/src/python/txtai.egg-info/requires.txt` & `txtai-5.5.1/src/python/txtai.egg-info/requires.txt`

 * *Files identical despite different names*

