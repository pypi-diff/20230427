# Comparing `tmp/srai-0.0.1.tar.gz` & `tmp/srai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.0.1.tar", last modified: Wed Nov 23 18:28:07 2022, max compression
+gzip compressed data, was "srai-0.1.0.tar", last modified: Thu Apr 27 20:53:34 2023, max compression
```

## Comparing `srai-0.0.1.tar` & `srai-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,126 @@
--rw-r--r--   0 runner    (1001) docker     (122)    11345 2022-11-23 18:27:51.568706 srai-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2022-11-23 18:27:51.568706 srai-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2782 2022-11-23 18:27:51.576706 srai-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-23 18:27:51.576706 srai-0.0.1/srai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       77 2022-11-23 18:27:51.576706 srai-0.0.1/srai/embedders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-23 18:27:51.576706 srai-0.0.1/srai/embedders/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2022-11-23 18:27:51.576706 srai-0.0.1/srai/joiners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2022-11-23 18:27:51.576706 srai-0.0.1/srai/joiners/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2022-11-23 18:27:51.576706 srai-0.0.1/srai/joiners/intersection_joiner.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2022-11-23 18:27:51.576706 srai-0.0.1/srai/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      606 2022-11-23 18:27:51.576706 srai-0.0.1/srai/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2022-11-23 18:27:51.576706 srai-0.0.1/srai/loaders/geoparquet_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2022-11-23 18:27:51.576706 srai-0.0.1/srai/regionizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10100 2022-11-23 18:27:51.576706 srai-0.0.1/srai/regionizers/_spherical_voronoi.py
--rw-r--r--   0 runner    (1001) docker     (122)    10582 2022-11-23 18:27:51.576706 srai-0.0.1/srai/regionizers/administrative_boundary_regionizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      555 2022-11-23 18:27:51.576706 srai-0.0.1/srai/regionizers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6355 2022-11-23 18:27:51.580706 srai-0.0.1/srai/regionizers/h3_regionizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2022-11-23 18:27:51.580706 srai-0.0.1/srai/regionizers/voronoi_regionizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-11-23 18:27:51.580706 srai-0.0.1/srai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2022-11-23 18:27:51.580706 srai-0.0.1/srai/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-23 18:27:51.580706 srai-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1674 2022-11-23 18:27:51.580706 srai-0.0.1/tests/joiners/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2022-11-23 18:27:51.580706 srai-0.0.1/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0 runner    (1001) docker     (122)    27801 2022-11-23 18:27:51.580706 srai-0.0.1/tests/loaders/files/example.parquet
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2022-11-23 18:27:51.580706 srai-0.0.1/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3608 2022-11-23 18:27:51.580706 srai-0.0.1/tests/regionizers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3806 2022-11-23 18:27:51.580706 srai-0.0.1/tests/regionizers/test_administrative_boundary_regionizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2022-11-23 18:27:51.580706 srai-0.0.1/tests/regionizers/test_h3_regionizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3577 2022-11-23 18:27:51.580706 srai-0.0.1/tests/regionizers/test_voronoi_regionizer.py
--rw-------   0 runner    (1001) docker     (122)     1867 2022-11-23 18:28:07.704719 srai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-04-27 20:53:11.370154 srai-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0    14631 2023-04-27 20:53:11.370154 srai-0.1.0/README.md
+-rw-r--r--   0        0        0     4455 2023-04-27 20:53:34.210591 srai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-04-27 20:53:11.382154 srai-0.1.0/srai/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-27 20:53:11.382154 srai-0.1.0/srai/constants.py
+-rw-r--r--   0        0        0      755 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     2722 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/_base.py
+-rw-r--r--   0        0        0     8327 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     4840 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      136 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0     9413 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2369 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0     8553 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6932 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6319 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2908 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2023-04-27 20:53:11.382154 srai-0.1.0/srai/exceptions.py
+-rw-r--r--   0        0        0      531 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      725 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/_base.py
+-rw-r--r--   0        0        0     2195 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5371 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      469 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     2011 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5324 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0     8849 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15758 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2438 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5536 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     5772 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2777 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     4691 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0    10106 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/pbf_file_downloader.py
+-rw-r--r--   0        0        0    10000 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/pbf_file_handler.py
+-rw-r--r--   0        0        0      118 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7587 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    13854 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      465 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     3679 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     2887 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     3221 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      496 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11189 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14174 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0      894 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/_base.py
+-rw-r--r--   0        0        0    11462 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15447 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/administrative_boundary_regionizer.py
+-rw-r--r--   0        0        0     6629 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/h3_regionizer.py
+-rw-r--r--   0        0        0     3118 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/s2_regionizer.py
+-rw-r--r--   0        0        0     4130 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/slippy_map_regionizer.py
+-rw-r--r--   0        0        0     5916 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/voronoi_regionizer.py
+-rw-r--r--   0        0        0      654 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/_optional.py
+-rw-r--r--   0        0        0      239 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/_pytorch_stubs.py
+-rw-r--r--   0        0        0      999 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/download.py
+-rw-r--r--   0        0        0      944 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/geocode.py
+-rw-r--r--   0        0        0     2521 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/geometry.py
+-rw-r--r--   0        0        0     1153 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/merge.py
+-rw-r--r--   0        0        0      717 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/typing.py
+-rw-r--r--   0        0        0       29 2023-04-27 20:53:11.386155 srai-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/conftest.py
+-rw-r--r--   0        0        0      557 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2590 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2716 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1061 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3037 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    24053 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0     8273 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3630 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     1765 2023-04-27 20:53:11.390154 srai-0.1.0/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2529 2023-04-27 20:53:11.390154 srai-0.1.0/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4284 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     3413 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3276 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   111539 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     2811 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     8690 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3156 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3165 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3353 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
+-rw-r--r--   0        0        0     2804 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
+-rw-r--r--   0        0        0     3822 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
+-rw-r--r--   0        0        0     5109 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
+-rw-r--r--   0        0        0     3822 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
+-rw-r--r--   0        0        0      629 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
+-rw-r--r--   0        0        0    10789 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2181 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3176 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4743 2023-04-27 20:53:11.390154 srai-0.1.0/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     4028 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     5668 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0     8063 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     5586 2023-04-27 20:53:11.394155 srai-0.1.0/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0     3665 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/conftest.py
+-rw-r--r--   0        0        0     6469 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_administrative_boundary_regionizer.py
+-rw-r--r--   0        0        0     2198 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_h3_regionizer.py
+-rw-r--r--   0        0        0     1831 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_s2_regionizer.py
+-rw-r--r--   0        0        0     2651 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_slippy_map_regionizer.py
+-rw-r--r--   0        0        0     4957 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_voronoi_regionizer.py
+-rw-r--r--   0        0        0    16722 1970-01-01 00:00:00.000000 srai-0.1.0/PKG-INFO
```

### Comparing `srai-0.0.1/LICENSE.md` & `srai-0.1.0/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -171,25 +171,14 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
    Copyright 2022 SRAI developers
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `srai-0.0.1/srai/joiners/base.py` & `srai-0.1.0/srai/joiners/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Base class for joiners."""
 
 import abc
 
 import geopandas as gpd
 
 
-class BaseJoiner(abc.ABC):
-    """Base abstract class for joiners."""
+class Joiner(abc.ABC):
+    """Abstract class for joiners."""
 
     @abc.abstractmethod
-    def join(self, regions: gpd.GeoDataFrame, features: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
+    def transform(
+        self,
+        regions: gpd.GeoDataFrame,
+        features: gpd.GeoDataFrame,
+    ) -> gpd.GeoDataFrame:  # pragma: no cover
         """
         Join features to regions.
 
         Args:
             regions (gpd.GeoDataFrame): regions with which features are joined
             features (gpd.GeoDataFrame): features to be joined
         Returns:
             GeoDataFrame with an intersection of regions and features, which contains
-            a MultiIndex and a geometry with the intersection
-
+            a MultiIndex and optionally a geometry with the intersection
         """
         raise NotImplementedError
```

### Comparing `srai-0.0.1/srai/loaders/base.py` & `srai-0.1.0/srai/loaders/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Base class for loaders."""
 
 import abc
-from pathlib import Path
-from typing import Union
+from typing import Any
 
 import geopandas as gpd
 
 
-class BaseLoader(abc.ABC):
-    """Base abstract class for loaders."""
+class Loader(abc.ABC):
+    """Abstract class for loaders."""
 
     @abc.abstractmethod
-    def load(self, area: Union[gpd.GeoDataFrame, Path]) -> gpd.GeoDataFrame:
+    def load(self, *args: Any, **kwargs: Any) -> gpd.GeoDataFrame:  # pragma: no cover
         """
         Load data for a given area.
 
         Args:
-            area (gdf.GeoDataFrame | Path): GeoDataFrame with the area of interest or a path
-                to a file with a geometry.
+            *args: Positional arguments dependating on a specific loader.
+            **kwargs: Keyword arguments dependating on a specific loader.
 
         Returns:
             GeoDataFrame with the downloaded data.
-
         """
         raise NotImplementedError
```

### Comparing `srai-0.0.1/srai/loaders/geoparquet_loader.py` & `srai-0.1.0/srai/loaders/geoparquet_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 Geoparquet loader.
 
 This module contains geoparquet loader implementation.
-
 """
 
 from pathlib import Path
 from typing import List, Optional, Union
 
 import geopandas as gpd
 
+from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
+from srai.loaders import Loader
+
 
-class GeoparquetLoader:
+class GeoparquetLoader(Loader):
     """
     GeoparquetLoader.
 
     Geoparquet [1] loader is a wrapper for a `geopandas.read_parquet` function
     and allows for an automatic index setting and additional geometry clipping.
 
     References:
-        [1] https://github.com/opengeospatial/geoparquet
-
+        1. https://github.com/opengeospatial/geoparquet
     """
 
     def load(
         self,
         file_path: Union[Path, str],
         index_column: Optional[str] = None,
         columns: Optional[List[str]] = None,
@@ -43,26 +44,25 @@
                 If not provided, unaltered data will be returned. Defaults to None.
 
         Raises:
             ValueError: If provided index column doesn't exists in list of loaded columns.
 
         Returns:
             gpd.GeoDataFrame: Loaded geoparquet file as a GeoDataFrame.
-
         """
-        if columns and "geometry" not in columns:
-            columns.append("geometry")
+        if columns and GEOMETRY_COLUMN not in columns:
+            columns.append(GEOMETRY_COLUMN)
 
         gdf = gpd.read_parquet(path=file_path, columns=columns)
 
         if index_column:
             if index_column not in gdf.columns:
                 raise ValueError(f"Column {index_column} doesn't exist in a file.")
             gdf.set_index(index_column, inplace=True)
 
-        gdf.to_crs(epsg=4326, inplace=True)
+        gdf.to_crs(crs=WGS84_CRS, inplace=True)
 
         if area is not None:
-            area_wgs84 = area.to_crs(epsg=4326)
+            area_wgs84 = area.to_crs(crs=WGS84_CRS)
             gdf = gdf.clip(mask=area_wgs84, keep_geom_type=False)
 
         return gdf
```

### Comparing `srai-0.0.1/srai/regionizers/_spherical_voronoi.py` & `srai-0.1.0/srai/regionizers/_spherical_voronoi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 """
 Spherical voronoi utils.
 
 This module contains spherical voronoi implementation based on SphericalVoronoi function from scipy
 library.
-
 """
 
 from functools import partial
 from math import ceil, sqrt
 from multiprocessing import cpu_count
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
 import numpy.typing as npt
 from haversine import haversine
 from pymap3d import Ellipsoid, ecef2geodetic, geodetic2ecef
 from scipy.spatial import SphericalVoronoi, geometric_slerp
 from shapely.geometry import MultiPolygon, Point, Polygon, box
 from spherical_geometry.polygon import SphericalPolygon
 from tqdm import tqdm
 from tqdm.contrib.concurrent import process_map
 
-# LON: 0; LAT: 0
-POINT_FRONT = (1.0, 0.0, 0.0)
-# LON: 180; LAT: 0
-POINT_BACK = (-1.0, 0.0, 0.0)
-# LON: 0; LAT: 90
-POINT_TOP = (0.0, 0.0, 1.0)
-# LON: 0; LAT: -90
-POINT_BOTTOM = (0.0, 0.0, -1.0)
-# LON: -90; LAT: 0
-POINT_LEFT = (0.0, -1.0, 0.0)
-# LON: 90; LAT: 0
-POINT_RIGHT = (0.0, 1.0, 0.0)
-
-SPHERE_PARTS = [
-    SphericalPolygon([POINT_FRONT, POINT_TOP, POINT_BACK, POINT_RIGHT, POINT_FRONT]),
-    SphericalPolygon([POINT_FRONT, POINT_RIGHT, POINT_BACK, POINT_BOTTOM, POINT_FRONT]),
-    SphericalPolygon([POINT_FRONT, POINT_BOTTOM, POINT_BACK, POINT_LEFT, POINT_FRONT]),
-    SphericalPolygon([POINT_FRONT, POINT_LEFT, POINT_BACK, POINT_TOP, POINT_FRONT]),
-]
-SPHERE_PARTS_BOUNDING_BOXES = [
-    box(minx=0, miny=0, maxx=180, maxy=90),
-    box(minx=0, miny=-90, maxx=180, maxy=0),
-    box(minx=-180, miny=-90, maxx=0, maxy=0),
-    box(minx=-180, miny=0, maxx=0, maxy=90),
-]
+SPHERE_PARTS: List[SphericalPolygon] = []
+SPHERE_PARTS_BOUNDING_BOXES: List[Polygon] = []
+
+
+def _generate_sphere_parts() -> None:
+    global SPHERE_PARTS, SPHERE_PARTS_BOUNDING_BOXES  # noqa: PLW0603
+
+    if not SPHERE_PARTS:
+        # LON: 0; LAT: 0
+        POINT_FRONT = (1.0, 0.0, 0.0)
+        # LON: 180; LAT: 0
+        POINT_BACK = (-1.0, 0.0, 0.0)
+        # LON: 0; LAT: 90
+        POINT_TOP = (0.0, 0.0, 1.0)
+        # LON: 0; LAT: -90
+        POINT_BOTTOM = (0.0, 0.0, -1.0)
+        # LON: -90; LAT: 0
+        POINT_LEFT = (0.0, -1.0, 0.0)
+        # LON: 90; LAT: 0
+        POINT_RIGHT = (0.0, 1.0, 0.0)
+
+        SPHERE_PARTS = [
+            SphericalPolygon([POINT_FRONT, POINT_TOP, POINT_BACK, POINT_RIGHT, POINT_FRONT]),
+            SphericalPolygon([POINT_FRONT, POINT_RIGHT, POINT_BACK, POINT_BOTTOM, POINT_FRONT]),
+            SphericalPolygon([POINT_FRONT, POINT_BOTTOM, POINT_BACK, POINT_LEFT, POINT_FRONT]),
+            SphericalPolygon([POINT_FRONT, POINT_LEFT, POINT_BACK, POINT_TOP, POINT_FRONT]),
+        ]
+        SPHERE_PARTS_BOUNDING_BOXES = [
+            box(minx=0, miny=0, maxx=180, maxy=90),
+            box(minx=0, miny=-90, maxx=180, maxy=0),
+            box(minx=-180, miny=-90, maxx=0, maxy=0),
+            box(minx=-180, miny=0, maxx=0, maxy=90),
+        ]
 
 
 class SphereEllipsoid(Ellipsoid):  # type: ignore
     """A sphere ellipsoid."""
 
     def __init__(self) -> None:
         """
         Sphere ellipsoid extends Ellipsoid from pymap3d [1] library.
 
         Class is used for mapping lat/lon coordinates
         from and to cartesian x/y/z values on a unit sphere.
         Required for spherical voronoi algorithm.
 
         References:
-            [1] https://github.com/geospace-code/pymap3d
-
+            1. https://github.com/geospace-code/pymap3d
         """
         self.semimajor_axis = 1
         self.semiminor_axis = 1
         self.flattening = (self.semimajor_axis - self.semiminor_axis) / self.semimajor_axis
         self.thirdflattening = (self.semimajor_axis - self.semiminor_axis) / (
             self.semimajor_axis + self.semiminor_axis
         )
@@ -75,35 +81,35 @@
 def map_to_geocentric(lon: float, lat: float, ell: Ellipsoid) -> Tuple[float, float, float]:
     """
     Wrapper for a geodetic2ecef function from pymap3d library.
 
     Args:
         lon (float): longitude of a point in a wgs84 crs.
         lat (float): latitude of a point in a wgs84 crs.
+        ell (Ellipsoid): an ellipsoid.
 
     Returns:
         Tuple[float, float, float]: (x, y, z) coordinates tuple.
-
     """
     x, y, z = geodetic2ecef(lat, lon, 0, ell=ell)
     return x, y, z
 
 
 def map_from_geocentric(x: float, y: float, z: float, ell: Ellipsoid) -> Tuple[float, float]:
     """
     Wrapper for a ecef2geodetic function from pymap3d library.
 
     Args:
         x (float): X cartesian coordinate.
         y (float): Y cartesian coordinate.
         z (float): Z cartesian coordinate.
+        ell (Ellipsoid): an ellipsoid.
 
     Returns:
         Tuple[float, float]: longitude and latitude coordinates in a wgs84 crs.
-
     """
     lat, lon, _ = ecef2geodetic(x, y, z, ell=ell)
     return lon, lat
 
 
 def _fix_lat_lon(
     lon: float,
@@ -120,15 +126,14 @@
     Args:
         lon (float): Longitude of a point.
         lat (float): Latitude of a point.
         bbox (Tuple[float, float, float, float]): Current sphere octant bounding box.
 
     Returns:
         Tuple[float, float]: Longitude and latitude of a point.
-
     """
     min_lon, min_lat, max_lon, max_lat = bbox
 
     # round imperfections
     lon = round(lon, 8)
     lat = round(lat, 8)
 
@@ -142,15 +147,15 @@
     elif lat and abs(lat) == abs(max_lat):
         lat = max_lat
 
     return lon, lat
 
 
 def _create_polygon(
-    spherical_polygon_points: npt.NDArray,
+    spherical_polygon_points: npt.NDArray[np.float32],
     bbox: Polygon,
     se: SphereEllipsoid,
     max_step: int,
 ) -> Polygon:
     """
     Map polygon from a sphere to Shapely polygon.
 
@@ -161,15 +166,14 @@
         spherical_polygon_points (npt.NDArray): List of spherical points.
         bbox (Polygon): Current sphere octant bounding box.
         se (SphereEllipsoid): SphereEllipsoid object.
         max_step (int): Max step between interpolated points on an arc.
 
     Returns:
         Polygon: Mapped polygon in wgs84 crs.
-
     """
     polygon_points = []
     prev_lon = None
     prev_lat = None
     n = len(spherical_polygon_points)
     bbox_bounds = bbox.bounds
     for i in range(n):
@@ -210,20 +214,20 @@
         sv (SphericalVoronoi): SphericalVoronoi object.
         se (SphereEllipsoid): SphereEllipsoid object.
         max_meters_between_points (int): maximal distance between points
             during interpolation of two vertices on a sphere.
 
     Returns:
         MultiPolygon: Parsed region in WGS84 coordinates.
-
     """
     region = sv.regions[region_id]
     region_vertices = [v for v in sv.vertices[region]]
     sph_pol = SphericalPolygon(region_vertices)
     sphere_intersection_parts = []
+    _generate_sphere_parts()
     for sphere_part, sphere_part_bbox in zip(SPHERE_PARTS, SPHERE_PARTS_BOUNDING_BOXES):
         if sph_pol.intersects_poly(sphere_part):
             intersection = sph_pol.intersection(sphere_part)
             sphere_intersection_parts.append((intersection, sphere_part_bbox))
 
     multi_polygon_parts: List[Polygon] = []
     for sphere_intersection_part, bbox in sphere_intersection_parts:
@@ -237,40 +241,55 @@
             multi_polygon_parts.append(polygon)
 
     multi_polygon = MultiPolygon(multi_polygon_parts)
     return multi_polygon
 
 
 def generate_voronoi_regions(
-    seeds: List[Point], max_meters_between_points: int, allow_multiprocessing: bool
+    seeds: List[Point],
+    max_meters_between_points: int,
+    num_of_multiprocessing_workers: int = -1,
+    multiprocessing_activation_threshold: Optional[int] = None,
 ) -> List[MultiPolygon]:
     """
     Generate Thessien polygons for a given list of seeds.
 
     Function generates Thessien polygons on a sphere using
     SphericalVoronoi algorithm from scipy library.
 
     Args:
         seeds (List[Point]): List of seeds used for generating regions.
         max_meters_between_points (int): maximal distance between points
             during interpolation of two vertices on a sphere.
-        allow_multiprocessing (bool): Whether to allow usage of multiprocessing for
-            accelerating the calculation for more than 100 seeds.
+        num_of_multiprocessing_workers (int): Number of workers used for multiprocessing.
+            Defaults to -1 which results in a total number of available cpu threads.
+            `0` and `1` values disable multiprocessing.
+            Similar to `n_jobs` parameter from `scikit-learn` library.
+        multiprocessing_activation_threshold (int, optional): Number of seeds required to start
+            processing on multiple processes. Activating multiprocessing for a small
+            amount of points might not be feasible. Defaults to 100.
 
     Returns:
         List[MultiPolygon]: List of regions cut into up to 8 polygons based
         on 8 parts of a sphere.
 
     Raises:
         ValueError: If less than 4 seeds are provided.
-
     """
     if len(seeds) < 4:
         raise ValueError("Minimum 4 seeds are required.")
 
+    if num_of_multiprocessing_workers == 0:
+        num_of_multiprocessing_workers = 1
+    elif num_of_multiprocessing_workers < 0:
+        num_of_multiprocessing_workers = cpu_count()
+
+    if not multiprocessing_activation_threshold:
+        multiprocessing_activation_threshold = 100
+
     se = SphereEllipsoid()
     mapped_points = [map_to_geocentric(pt.x, pt.y, se) for pt in seeds]
     sphere_points = np.array([[pt[0], pt[1], pt[2]] for pt in mapped_points])
 
     radius = 1
     center = np.array([0, 0, 0])
     sv = SphericalVoronoi(sphere_points, radius, center, threshold=1e-8)
@@ -279,25 +298,23 @@
     create_regions_func = partial(
         _create_region, sv=sv, se=se, max_meters_between_points=max_meters_between_points
     )
 
     total_regions = len(sv.regions)
     region_ids = list(range(total_regions))
 
-    num_workers = cpu_count() - 1
-
     generated_regions: List[MultiPolygon] = []
-    if allow_multiprocessing and total_regions >= 100:
+    if num_of_multiprocessing_workers > 1 and total_regions >= multiprocessing_activation_threshold:
         generated_regions.extend(
             process_map(
                 create_regions_func,
                 region_ids,
                 desc="Generating regions",
-                max_workers=num_workers,
-                chunksize=ceil(total_regions / (4 * num_workers)),
+                max_workers=num_of_multiprocessing_workers,
+                chunksize=ceil(total_regions / (4 * num_of_multiprocessing_workers)),
             )
         )
     else:
         generated_regions.extend(
             create_regions_func(region_id=region_id)
             for region_id in tqdm(region_ids, desc="Generating regions")
         )
```

### Comparing `srai-0.0.1/srai/regionizers/administrative_boundary_regionizer.py` & `srai-0.1.0/srai/regionizers/administrative_boundary_regionizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,117 @@
 """
 Administrative Boundary Regionizer.
 
 This module contains administrative boundary regionizer implementation.
-
 """
-
-from typing import Any, Dict, List, Union
+import time
+from typing import Any, Dict, List, Optional, Union
 
 import geopandas as gpd
 import topojson as tp
-from functional import seq
-from osmnx import geocode_to_gdf
-from OSMPythonTools.overpass import Element, Overpass, overpassQueryBuilder
 from shapely.geometry import MultiPolygon, Point, Polygon
-from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
+from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from shapely.validation import make_valid
 from tqdm import tqdm
 
+from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
+from srai.regionizers import Regionizer
+from srai.utils import flatten_geometry_series
+from srai.utils._optional import import_optional_dependencies
+
 
-class AdministrativeBoundaryRegionizer:
+class AdministrativeBoundaryRegionizer(Regionizer):
     """
     AdministrativeBoundaryRegionizer.
 
     Administrative boundary regionizer allows the given geometries to be divided
     into boundaries from OpenStreetMap on a given `admin_level` [1].
 
-    Downloads those boundaries online using `OSMPythonTools` and `osmnx` library.
+    Downloads those boundaries online using `overpass` and `osmnx` libraries.
 
     Note: offline .pbf loading will be implemented in the future.
     Note: option to download historic data will be implemented in the future.
 
     References:
-        [1] https://wiki.openstreetmap.org/wiki/Key:admin_level
-
+        1. https://wiki.openstreetmap.org/wiki/Key:admin_level
     """
 
+    EMPTY_REGION_NAME = "EMPTY"
+
     def __init__(
         self,
         admin_level: int,
         clip_regions: bool = True,
         return_empty_region: bool = False,
         prioritize_english_name: bool = True,
         toposimplify: Union[bool, float] = True,
+        remove_artefact_regions: bool = True,
     ) -> None:
         """
         Init AdministrativeBoundaryRegionizer.
 
         Args:
             admin_level (int): OpenStreetMap admin_level value. See [1] for detailed description of
                 available values.
-            clip_regions (bool, optional): Whether to to clip regions using a provided mask.
+            clip_regions (bool, optional): Whether to clip regions using a provided mask.
                 Turning it off can an be useful when trying to load regions using list a of points.
                 Defaults to True.
             return_empty_region (bool, optional): Whether to return an empty region to fill
                 remaining space or not. Defaults to False.
             prioritize_english_name (bool, optional): Whether to use english area name if available
                 as a region id first. Defaults to True.
             toposimplify (Union[bool, float], optional): Whether to simplify topology to reduce
                 geometries size or not. Value is passed to `topojson` library for topology-aware
                 simplification. Since provided values are treated like degrees, values between
                 1e-4 and 1.0 are recommended. Defaults to True (which results in value equal 1e-4).
+            remove_artefact_regions (bool, optional): Whether to remove small regions barely
+                intersecting queried area. Turning it off can sometimes load unnecessary boundaries
+                that touch on the edge. It removes regions that intersect with an area smaller
+                than 1% of total self. Takes into consideration if provided query GeoDataFrame
+                contains points and then skips calculating area when intersects any point.
+                Defaults to True.
 
         Raises:
             ValueError: If admin_level is outside available range (1-11). See [2] for list of
                 values with `in_wiki` selected.
 
         References:
-            [1] https://wiki.openstreetmap.org/wiki/Tag:boundary=administrative#10_admin_level_values_for_specific_countries
-            [2] https://taginfo.openstreetmap.org/keys/admin_level#values
-
+            1. https://wiki.openstreetmap.org/wiki/Tag:boundary=administrative#10_admin_level_values_for_specific_countries
+            2. https://taginfo.openstreetmap.org/keys/admin_level#values
         """  # noqa: W505, E501
+        import_optional_dependencies(
+            dependency_group="osm",
+            modules=["osmnx", "overpass"],
+        )
+        from overpass import API
+
         if admin_level < 1 or admin_level > 11:
             raise ValueError("admin_level outside of available range.")
 
         self.admin_level = admin_level
         self.prioritize_english_name = prioritize_english_name
         self.clip_regions = clip_regions
         self.return_empty_region = return_empty_region
+        self.remove_artefact_regions = remove_artefact_regions
 
-        if isinstance(toposimplify, float):
+        if isinstance(toposimplify, (int, float)) and toposimplify > 0:
             self.toposimplify = toposimplify
-        elif toposimplify:
+        elif isinstance(toposimplify, bool) and toposimplify:
             self.toposimplify = 1e-4
         else:
             self.toposimplify = False
 
-        self.overpass = Overpass()
+        self.overpass_api = API(timeout=60)
 
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
         Regionize a given GeoDataFrame.
 
-        Will query Overpass [1] server using `OSMPythonTools` [2] library for closed administrative
+        Will query Overpass [1] server using `overpass` [2] library for closed administrative
         boundaries on a given admin_level and then download geometries for each relation using
         `osmnx` [3] library.
 
         If `prioritize_english_name` is set to `True`, method will try to extract the `name:en` tag
         first before resorting to the `name` tag. If boundary doesn't have a `name` tag, an `id`
         will be used.
 
@@ -115,141 +130,240 @@
             gpd.GeoDataFrame: GeoDataFrame with the regionized data cropped using input
                 GeoDataFrame.
 
         Raises:
             RuntimeError: If simplification can't preserve a topology.
 
         References:
-            [1] https://wiki.openstreetmap.org/wiki/Overpass_API
-            [2] https://github.com/mocnik-science/osm-python-tools
-            [3] https://github.com/gboeing/osmnx
-            [4] https://github.com/mattijn/topojson
-
+            1. https://wiki.openstreetmap.org/wiki/Overpass_API
+            2. https://github.com/mvexel/overpass-api-python-wrapper
+            3. https://github.com/gboeing/osmnx
+            4. https://github.com/mattijn/topojson
         """
-        gdf_wgs84 = gdf.to_crs(epsg=4326)
+        gdf_wgs84 = gdf.to_crs(crs=WGS84_CRS)
 
         regions_dicts = self._generate_regions_from_all_geometries(gdf_wgs84)
 
-        regions_gdf = gpd.GeoDataFrame(data=regions_dicts, crs="EPSG:4326").set_index("region_id")
+        if not regions_dicts:
+            import warnings
+
+            warnings.warn(
+                (
+                    "Couldn't find any administrative boundaries with"
+                    f" `admin_level`={self.admin_level}."
+                ),
+                RuntimeWarning,
+                stacklevel=2,
+            )
+
+            return self._get_empty_geodataframe(gdf_wgs84)
+
+        regions_gdf = gpd.GeoDataFrame(data=regions_dicts, crs=WGS84_CRS).set_index(REGIONS_INDEX)
         regions_gdf = self._toposimplify_gdf(regions_gdf)
 
+        if self.remove_artefact_regions:
+            points_collection: Optional[BaseGeometry] = gdf_wgs84[
+                gdf_wgs84.geom_type == "Point"
+            ].geometry.unary_union
+            clipping_polygon_area: Optional[BaseGeometry] = gdf_wgs84[
+                gdf_wgs84.geom_type != "Point"
+            ].geometry.unary_union
+
+            regions_to_keep = [
+                region_id
+                for region_id, row in regions_gdf.iterrows()
+                if self._check_intersects_with_points(row["geometry"], points_collection)
+                or self._calculate_intersection_area_fraction(
+                    row["geometry"], clipping_polygon_area
+                )
+                > 0.01
+            ]
+            regions_gdf = regions_gdf.loc[regions_to_keep]
+
         if self.clip_regions:
             regions_gdf = regions_gdf.clip(mask=gdf_wgs84, keep_geom_type=False)
 
         if self.return_empty_region:
             empty_region = self._generate_empty_region(mask=gdf_wgs84, regions_gdf=regions_gdf)
             if not empty_region.is_empty:
-                regions_gdf.loc["EMPTY", "geometry"] = empty_region
+                regions_gdf.loc[
+                    AdministrativeBoundaryRegionizer.EMPTY_REGION_NAME, GEOMETRY_COLUMN
+                ] = empty_region
+
         return regions_gdf
 
     def _generate_regions_from_all_geometries(
         self, gdf_wgs84: gpd.GeoDataFrame
     ) -> List[Dict[str, Any]]:
         """Query and optimize downloading data from Overpass."""
         elements_ids = set()
-        generated_regions: List[Dict[str, Any]] = list()
+        generated_regions: List[Dict[str, Any]] = []
 
-        all_geometries = (
-            seq([self._flatten_geometries(g) for g in gdf_wgs84.geometry]).flatten().list()
-        )
+        all_geometries = flatten_geometry_series(gdf_wgs84.geometry)
 
         with tqdm(desc="Loading boundaries") as pbar:
             for geometry in all_geometries:
-                unary_geometry = unary_union([r["geometry"] for r in generated_regions])
-                if not geometry.within(unary_geometry):
+                unary_geometry = unary_union([r[GEOMETRY_COLUMN] for r in generated_regions])
+                if not geometry.covered_by(unary_geometry):
                     query = self._generate_query_for_single_geometry(geometry)
-                    boundaries = self.overpass.query(query, timeout=60, shallow=False)
-                    boundaries_list = list(boundaries.relations()) if boundaries.relations() else []
+                    boundaries_list = self._query_overpass(query)
                     for boundary in boundaries_list:
-                        if boundary.id() not in elements_ids:
-                            elements_ids.add(boundary.id())
+                        if boundary["id"] not in elements_ids:
+                            elements_ids.add(boundary["id"])
                             generated_regions.append(self._parse_overpass_element(boundary))
                             pbar.update(1)
 
         return generated_regions
 
-    def _flatten_geometries(self, g: BaseGeometry) -> List[BaseGeometry]:
-        """Flatten all geometries into a list of BaseGeometries."""
-        if isinstance(g, BaseMultipartGeometry):
-            return list(
-                seq([self._flatten_geometries(sub_geom) for sub_geom in g.geoms]).flatten().list()
-            )
-        return [g]
+    def _query_overpass(self, query: str) -> List[Dict[str, Any]]:
+        """
+        Query Overpass and catch exceptions.
+
+        Since `overpass` library doesn't have useful http error wrapping like `osmnx` does [1],
+        this method allows for retry after waiting some time. Additionally, caching mechanism
+        uses `osmnx` internal methods built for this purpose.
+
+        Args:
+            query (str): Overpass query.
+
+        Raises:
+            ex: If exception is different than urllib.request.HTTPError or
+                HTTP code is different than 429 or 504.
+
+        Returns:
+            List[Dict[str, Any]]: Query elements result from Overpass.
+
+        References:
+            1. https://github.com/gboeing/osmnx/blob/main/osmnx/downloader.py#L712
+        """
+        from osmnx.downloader import _retrieve_from_cache, _save_to_cache
+        from overpass import MultipleRequestsError, ServerLoadError
+
+        while True:
+            try:
+                query_result = _retrieve_from_cache(url=query, check_remark=False)
+                if query_result is None:
+                    query_result = self.overpass_api.get(
+                        query, verbosity="ids tags", responseformat="json"
+                    )
+                    _save_to_cache(url=query, response_json=query_result, sc=200)
+                elements: List[Dict[str, Any]] = query_result["elements"]
+                return elements
+            except (MultipleRequestsError, ServerLoadError):
+                time.sleep(60)
 
     def _generate_query_for_single_geometry(self, g: BaseGeometry) -> str:
         """Generate Overpass query for a geometry."""
         if isinstance(g, Point):
             query = (
                 f"is_in({g.y},{g.x});"
                 'area._["boundary"="administrative"]'
                 '["type"~"boundary|multipolygon"]'
                 f'["admin_level"="{self.admin_level}"];'
-                "relation(pivot); out ids tags;"
+                "relation(pivot);"
             )
         else:
             raw_gdf_bounds = g.bounds
             overpass_bbox = (
                 raw_gdf_bounds[1],
                 raw_gdf_bounds[0],
                 raw_gdf_bounds[3],
                 raw_gdf_bounds[2],
             )
-            query = overpassQueryBuilder(
-                bbox=overpass_bbox,
-                elementType="relation",
-                selector=[
-                    '"boundary"="administrative"',
-                    '"type"~"boundary|multipolygon"',
-                    f'"admin_level"="{self.admin_level}"',
-                ],
-                out="ids tags",
-                includeGeometry=False,
+            query = (
+                '(relation["boundary"="administrative"]'
+                '["type"~"boundary|multipolygon"]'
+                f'["admin_level"="{self.admin_level}"]'
+                f"({overpass_bbox[0]},{overpass_bbox[1]},{overpass_bbox[2]},{overpass_bbox[3]}););"
             )
         return query
 
-    def _parse_overpass_element(self, element: Element) -> Dict[str, Any]:
+    def _parse_overpass_element(self, element: Dict[str, Any]) -> Dict[str, Any]:
         """Parse single Overpass Element and return a region."""
+        element_tags = element.get("tags", {})
         region_id = None
         if self.prioritize_english_name:
-            region_id = element.tag("name:en")
+            region_id = element_tags.get("name:en")
         if not region_id:
-            region_id = element.tag("name")
+            region_id = element_tags.get("name")
         if not region_id:
-            region_id = str(element.id())
+            region_id = str(element["id"])
 
         return {
-            "geometry": self._get_boundary_geometry(element.id()),
-            "region_id": region_id,
+            GEOMETRY_COLUMN: self._get_boundary_geometry(element["id"]),
+            REGIONS_INDEX: region_id,
         }
 
-    def _get_boundary_geometry(self, relation_id: int) -> BaseGeometry:
+    def _get_boundary_geometry(self, relation_id: str) -> BaseGeometry:
         """Download a geometry of a relation using `osmnx` library."""
+        from osmnx import geocode_to_gdf
+
         return geocode_to_gdf(query=[f"R{relation_id}"], by_osmid=True).geometry[0]
 
     def _toposimplify_gdf(self, regions_gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """Create a topology to ensure proper boundaries between regions and simplify it."""
         topo = tp.Topology(
             regions_gdf,
             prequantize=False,
             presimplify=False,
             toposimplify=self.toposimplify,
             simplify_algorithm="dp",
             prevent_oversimplify=True,
         )
-        regions_gdf = topo.to_gdf(winding_order="CW_CCW", crs="EPSG:4326", validate=True)
-        regions_gdf.index.rename("region_id", inplace=True)
+        regions_gdf = topo.to_gdf(winding_order="CW_CCW", crs=WGS84_CRS, validate=True)
+        regions_gdf.index.rename(REGIONS_INDEX, inplace=True)
         regions_gdf.geometry = regions_gdf.geometry.apply(make_valid)
         for idx, r in regions_gdf.iterrows():
             if not isinstance(r.geometry, (Polygon, MultiPolygon)):
                 raise RuntimeError(
                     f"Simplification couldn't preserve geometry for region: {idx}."
                     " Try lowering toposimplify value."
                 )
         return regions_gdf
 
     def _generate_empty_region(
         self, mask: gpd.GeoDataFrame, regions_gdf: gpd.GeoDataFrame
     ) -> BaseGeometry:
         """Generate a region filling the space between regions and full clipping mask."""
-        joined_mask = unary_union(mask.geometry)
-        joined_geometry = unary_union(regions_gdf.geometry)
+        joined_mask = mask.geometry.unary_union
+        joined_geometry = regions_gdf.geometry.unary_union
         return joined_mask.difference(joined_geometry)
+
+    def _get_empty_geodataframe(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
+        """Get empty GeoDataFrame when zero boundaries have been found."""
+        if self.return_empty_region:
+            regions_gdf = gpd.GeoDataFrame(
+                data={
+                    GEOMETRY_COLUMN: [gdf.geometry.unary_union],
+                    REGIONS_INDEX: [AdministrativeBoundaryRegionizer.EMPTY_REGION_NAME],
+                },
+                crs=WGS84_CRS,
+            ).set_index(REGIONS_INDEX)
+        else:
+            regions_gdf = gpd.GeoDataFrame(
+                data={
+                    GEOMETRY_COLUMN: [],
+                    REGIONS_INDEX: [],
+                },
+                crs=WGS84_CRS,
+            )
+        return regions_gdf
+
+    def _check_intersects_with_points(
+        self, region_geometry: BaseGeometry, points_collection: Optional[BaseGeometry]
+    ) -> bool:
+        """Check if region intersects with any point in query regions."""
+        return (
+            points_collection is not None
+            and not points_collection.is_empty
+            and region_geometry.intersects(points_collection)
+        )
+
+    def _calculate_intersection_area_fraction(
+        self, region_geometry: BaseGeometry, clipping_polygon_area: Optional[BaseGeometry]
+    ) -> float:
+        """Calculate intersection area fraction to check if it's big enough."""
+        if clipping_polygon_area is None or clipping_polygon_area.is_empty:
+            return 0
+        full_area = float(region_geometry.area)
+        clip_area = float(region_geometry.intersection(clipping_polygon_area).area)
+        return clip_area / full_area
```

### Comparing `srai-0.0.1/srai/regionizers/base.py` & `srai-0.1.0/srai/regionizers/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 """Base class for regionizers."""
 
 import abc
 
 import geopandas as gpd
 
 
-class BaseRegionizer(abc.ABC):
-    """Base abstract class for regionizers."""
+class Regionizer(abc.ABC):
+    """Abstract class for regionizers."""
 
     @abc.abstractmethod
-    def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
+    def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:  # pragma: no cover
         """
         Regionize a given GeoDataFrame.
 
         This one should treat the input as a single region.
 
         Args:
             gdf (gpd.GeoDataFrame): GeoDataFrame to be regionized.
 
         Returns:
             GeoDataFrame with the regionized data.
-
         """
         raise NotImplementedError
+
+    def _explode_multipolygons(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
+        """
+        Explode multipolygons into multiple polygons.
+
+        Args:
+            gdf (gpd.GeoDataFrame): GeoDataFrame to be exploded.
+
+        Returns:
+            GeoDataFrame with exploded multipolygons.
+        """
+        return gdf.explode(index_parts=True).reset_index(drop=True)
```

### Comparing `srai-0.0.1/srai/regionizers/h3_regionizer.py` & `srai-0.1.0/srai/regionizers/h3_regionizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 This module exposes Uber's H3 Hexagonal Hierarchical Geospatial Indexing System [1] as a regionizer.
 
 Note:
     The default API [2] was chosen (basic_str) to ease the implementation.
     It may be beneficial to try the NumPy API for computationally-heavy work.
 
 References:
-    [1] https://uber.github.io/h3-py/
-    [2] https://uber.github.io/h3-py/api_comparison
-
+    1. https://uber.github.io/h3-py/
+    2. https://uber.github.io/h3-py/api_comparison
 """
 
 from typing import List
 
 import geopandas as gpd
 import h3
 from functional import seq
 from shapely import geometry
 
-from . import BaseRegionizer
+from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
+from srai.regionizers import Regionizer
+from srai.utils import buffer_geometry
 
 
-class H3Regionizer(BaseRegionizer):
+class H3Regionizer(Regionizer):
     """
     H3 Regionizer.
 
     H3 Regionizer allows the given geometries to be divided
     into H3 cells - hexagons with pentagons as a very rare exception
-
     """
 
     def __init__(self, resolution: int, buffer: bool = True) -> None:
         """
         Init H3Regionizer.
 
         Args:
@@ -41,16 +41,15 @@
             buffer (bool, optional): Whether to fully cover the geometries with
                 H3 Cells (visible on the borders). Defaults to True.
 
         Raises:
             ValueError: If resolution is not between 0 and 15.
 
         References:
-            [1] https://h3geo.org/docs/core-library/restable/
-
+            1. https://h3geo.org/docs/core-library/restable/
         """
         if not (0 <= resolution <= 15):
             raise ValueError(f"Resolution {resolution} is not between 0 and 15.")
 
         self.resolution = resolution
         self.buffer = buffer
 
@@ -65,51 +64,52 @@
             gdf (gpd.GeoDataFrame): (Multi)Polygons to be regionized.
 
         Returns:
             gpd.GeoDataFrame: H3 cells.
 
         Raises:
             ValueError: If provided GeoDataFrame has no crs defined.
-
         """
-        gdf_wgs84 = gdf.to_crs(epsg=4326)
+        gdf_wgs84 = gdf.to_crs(crs=WGS84_CRS)
 
-        # transform multipolygons to multiple polygons
-        gdf_exploded = gdf_wgs84.explode(index_parts=True).reset_index(drop=True)
+        gdf_exploded = self._explode_multipolygons(gdf_wgs84)
         gdf_buffered = self._buffer(gdf_exploded) if self.buffer else gdf_exploded
 
         h3_indexes = (
-            seq(gdf_buffered["geometry"])
+            seq(gdf_buffered[GEOMETRY_COLUMN])
             .map(self._polygon_shapely_to_h3)
             .flat_map(lambda polygon: h3.polygon_to_cells(polygon, self.resolution))
             .distinct()
             .to_list()
         )
 
         gdf_h3 = self._gdf_from_h3_indexes(h3_indexes)
 
         # there may be too many cells because of too big buffer
-        gdf_h3_clipped = (
-            gdf_h3.sjoin(gdf_exploded[["geometry"]]).drop(columns="index_right").drop_duplicates()
-            if self.buffer
-            else gdf_h3
-        )
+        if self.buffer:
+            gdf_h3_clipped = gdf_h3.sjoin(gdf_exploded[[GEOMETRY_COLUMN]]).drop(
+                columns="index_right"
+            )
+            gdf_h3_clipped = gdf_h3_clipped[~gdf_h3_clipped.index.duplicated(keep="first")]
+        else:
+            gdf_h3_clipped = gdf_h3
+
+        gdf_h3_clipped.index.name = REGIONS_INDEX
 
         return gdf_h3_clipped.to_crs(gdf.crs)
 
     def _polygon_shapely_to_h3(self, polygon: geometry.Polygon) -> h3.Polygon:
         """
         Convert Shapely Polygon to H3 Polygon.
 
         Args:
             polygon (geometry.Polygon): Shapely polygon to be converted.
 
         Returns:
             h3.Polygon: Converted polygon.
-
         """
         exterior = [coord[::-1] for coord in list(polygon.exterior.coords)]
         interiors = [
             [coord[::-1] for coord in list(interior.coords)] for interior in polygon.interiors
         ]
         return h3.Polygon(exterior, *interiors)
 
@@ -118,46 +118,43 @@
         Convert H3 Indexes to GeoDataFrame with geometries.
 
         Args:
             h3_indexes (List[str]): H3 Indexes.
 
         Returns:
             gpd.GeoDataFrame: H3 cells.
-
         """
         return gpd.GeoDataFrame(
             None,
             index=h3_indexes,
             geometry=[self._h3_index_to_shapely_polygon(h3_index) for h3_index in h3_indexes],
-            crs="epsg:4326",
+            crs=WGS84_CRS,
         )
 
     def _h3_index_to_shapely_polygon(self, h3_index: str) -> geometry.Polygon:
         """
         Convert H3 Index to Shapely polygon.
 
         Args:
             h3_index (str): H3 Index to be converted.
 
         Returns:
             geometry.Polygon: Converted polygon.
-
         """
         return self._polygon_h3_to_shapely(h3.cells_to_polygons([h3_index])[0])
 
     def _polygon_h3_to_shapely(self, polygon: h3.Polygon) -> geometry.Polygon:
         """
         Convert H3 Polygon to Shapely Polygon.
 
         Args:
             polygon (h3.Polygon): H3 Polygon to be converted.
 
         Returns:
             geometry.Polygon: Converted polygon.
-
         """
         return geometry.Polygon(
             shell=[coord[::-1] for coord in polygon.outer],
             holes=[[coord[::-1] for coord in hole] for hole in polygon.holes],
         )
 
     def _buffer(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
@@ -181,18 +178,18 @@
         Args:
             gdf (gpd.GeoDataFrame): Geometries.
 
         Returns:
             gpd.GeoDataFrame: Geometries buffered around the edges.
 
         References:
-            [1] https://h3geo.org/docs/core-library/restable/#hexagon-min-and-max-areas
-
+            1. https://h3geo.org/docs/core-library/restable/#hexagon-min-and-max-areas
         """
+        buffer_distance_meters = 2 * h3.average_hexagon_edge_length(self.resolution, unit="m")
+        buffered_geometries = gdf.geometry.apply(
+            lambda polygon: buffer_geometry(polygon, buffer_distance_meters)
+        )
+
         return gpd.GeoDataFrame(
-            geometry=(
-                gdf.to_crs(epsg=3395)
-                .buffer(2 * h3.average_hexagon_edge_length(self.resolution, unit="m"))
-                .to_crs(epsg=4326)
-            ),
+            geometry=buffered_geometries,
             index=gdf.index,
         )
```

### Comparing `srai-0.0.1/srai/utils/merge.py` & `srai-0.1.0/srai/utils/merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,43 +2,41 @@
 
 from typing import List, Union
 
 import geopandas as gpd
 from shapely.geometry import MultiPolygon, Polygon
 
 
-def _merge_disjointed_polygons(polygons: List[Union[Polygon, MultiPolygon]]) -> MultiPolygon:
+def merge_disjointed_polygons(polygons: List[Union[Polygon, MultiPolygon]]) -> MultiPolygon:
     """
     Merges all polygons into a single MultiPolygon.
 
     Input polygons are expected to be disjointed.
 
     Args:
         polygons (List[Union[Polygon, MultiPolygon]]): List of polygons to merge
 
     Returns:
         MultiPolygon: Merged polygon
-
     """
     single_polygons = []
     for geom in polygons:
         if type(geom) is Polygon:
             single_polygons.append(geom)
         else:
             single_polygons.extend(geom.geoms)
     return MultiPolygon(single_polygons)
 
 
-def _merge_disjointed_gdf_geometries(gdf: gpd.GeoDataFrame) -> MultiPolygon:
+def merge_disjointed_gdf_geometries(gdf: gpd.GeoDataFrame) -> MultiPolygon:
     """
     Merges geometries from a GeoDataFrame into a single MultiPolygon.
 
     Input geometries are expected to be disjointed.
 
     Args:
         gdf (gpd.GeoDataFrame): GeoDataFrame with geometries to merge.
 
     Returns:
         MultiPolygon: Merged polygon
-
     """
-    return _merge_disjointed_polygons(list(gdf.geometry))
+    return merge_disjointed_polygons(list(gdf.geometry))
```

### Comparing `srai-0.0.1/tests/joiners/conftest.py` & `srai-0.1.0/tests/joiners/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Conftest for Joiners."""
 
 import geopandas as gpd
 import pandas as pd
 import pytest
 from shapely import geometry
 
+from srai.constants import FEATURES_INDEX, REGIONS_INDEX, WGS84_CRS
+
 
 @pytest.fixture  # type: ignore
 def no_geometry_gdf() -> gpd.GeoDataFrame:
     """Get empty GeoDataFrame."""
     return gpd.GeoDataFrame()
 
 
@@ -24,33 +26,34 @@
     regions = gpd.GeoDataFrame(
         geometry=[
             geometry.Polygon([(-1, 0), (-1, -1), (0, -1), (0, 0)]),
             geometry.Polygon([(1, 0), (1, 1), (0, 1), (0, 0)]),
             geometry.Polygon([(-2, -1), (-2, -2), (-1, -2), (-1, -1)]),
             geometry.Polygon([(-2, 0.5), (-2, -0.5), (-1, -0.5), (-1, 0.5)]),
         ],
-        crs="epsg:4326",
+        crs=WGS84_CRS,
     )
     return regions
 
 
 @pytest.fixture  # type: ignore
 def features_gdf() -> gpd.GeoDataFrame:
     """Get GeoDataFrame with example features."""
     features = gpd.GeoDataFrame(
+        [1, 2, 3, 4],
         geometry=[
             geometry.Polygon([(-1.5, 0.5), (-1.5, 0), (-0.5, 0), (-0.5, 0.5)]),
             geometry.Polygon([(-1.5, -1.5), (-1.5, -2.5), (-0.5, -2.5), (-0.5, -1.5)]),
             geometry.Point((0, 0)),
             geometry.Point((-0.5, -0.5)),
         ],
-        crs="epsg:4326",
+        crs=WGS84_CRS,
     )
     return features
 
 
 @pytest.fixture  # type: ignore
 def joint_multiindex() -> pd.MultiIndex:
     """Get MultiIndex for joint GeoDataFrame."""
     return pd.MultiIndex.from_tuples(
-        [(0, 2), (0, 3), (1, 2), (0, 0), (3, 0), (2, 1)], names=["region_id", "feature_id"]
+        [(0, 2), (0, 3), (1, 2), (0, 0), (3, 0), (2, 1)], names=[REGIONS_INDEX, FEATURES_INDEX]
     )
```

### Comparing `srai-0.0.1/tests/loaders/files/example.parquet` & `srai-0.1.0/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.0.1/tests/loaders/test_geoparquet_loader.py` & `srai-0.1.0/tests/loaders/test_geoparquet_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 """Geoparquet loader tests."""
 from pathlib import Path
 
 import geopandas as gpd
 import pytest
 from shapely.geometry import box
 
+from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
 from srai.loaders import GeoparquetLoader
 
 bbox = box(minx=-180, maxx=180, miny=-90, maxy=90)
-bbox_gdf = gpd.GeoDataFrame({"geometry": [bbox]})
+bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [bbox]})
 
 
 def test_wrong_path_error() -> None:
     """Test checks if cannot load nonexistent file."""
     with pytest.raises(FileNotFoundError):
-        GeoparquetLoader().load(file_path=Path(__file__).parent / "files" / "non_existent.parquet")
+        GeoparquetLoader().load(
+            file_path=Path(__file__).parent / "test_files" / "non_existent.parquet"
+        )
 
 
 def test_correct_path() -> None:
     """Test checks if can load proper file."""
-    gdf = GeoparquetLoader().load(file_path=Path(__file__).parent / "files" / "example.parquet")
+    gdf = GeoparquetLoader().load(
+        file_path=Path(__file__).parent / "test_files" / "example.parquet"
+    )
     assert len(gdf.index) == 5
     assert gdf.crs.to_epsg() == 4326
 
 
 def test_wrong_index_value_error() -> None:
     """Test checks if cannot set nonexistent index."""
     with pytest.raises(ValueError):
         GeoparquetLoader().load(
-            file_path=Path(__file__).parent / "files" / "example.parquet",
+            file_path=Path(__file__).parent / "test_files" / "example.parquet",
             index_column="test_column",
         )
 
 
 def test_clipped_columns() -> None:
     """Test if returned a subset of columns."""
     gdf = GeoparquetLoader().load(
-        file_path=Path(__file__).parent / "files" / "example.parquet", columns=["continent", "name"]
+        file_path=Path(__file__).parent / "test_files" / "example.parquet",
+        columns=["continent", "name"],
     )
     assert len(gdf.columns == 3)
 
 
 def test_setting_index() -> None:
     """Test if properly set the index."""
     gdf = GeoparquetLoader().load(
-        file_path=Path(__file__).parent / "files" / "example.parquet", index_column="name"
+        file_path=Path(__file__).parent / "test_files" / "example.parquet", index_column="name"
     )
     expected_index = {"Canada", "Fiji", "Tanzania", "United States of America", "W. Sahara"}
     assert expected_index == set(gdf.index)
 
 
 def test_clipping() -> None:
     """Test if properly clips the data."""
     bbox = box(minx=-106.645646, maxx=-93.508292, miny=25.837377, maxy=36.500704)
-    bbox_gdf = gpd.GeoDataFrame({"geometry": [bbox]}, crs="EPSG:4326")
+    bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [bbox]}, crs=WGS84_CRS)
     gdf = GeoparquetLoader().load(
-        file_path=Path(__file__).parent / "files" / "example.parquet", area=bbox_gdf
+        file_path=Path(__file__).parent / "test_files" / "example.parquet", area=bbox_gdf
     )
     assert len(gdf.index) == 1
```

### Comparing `srai-0.0.1/tests/regionizers/conftest.py` & `srai-0.1.0/tests/regionizers/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Conftest for Regionizers."""
 
 import geopandas as gpd
 import pytest
 from shapely import geometry
 
+from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
+
 
 @pytest.fixture  # type: ignore
 def gdf_empty() -> gpd.GeoDataFrame:
     """Get empty GeoDataFrame."""
     return gpd.GeoDataFrame()
 
 
@@ -49,15 +51,15 @@
                         (0.8, 0.3),
                         (0.5, 0.4),
                     ]
                 ],
             ),
             geometry.Polygon(shell=[(-0.25, 0), (0.25, 0), (0, 0.2)]),
         ],
-        crs="epsg:4326",
+        crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_multipolygon() -> gpd.GeoDataFrame:
     """Get GeoDataFrame with multipolygon."""
     return gpd.GeoDataFrame(
@@ -86,34 +88,34 @@
                     (
                         [(-0.25, 0), (0.25, 0), (0, 0.2)],
                         (),
                     ),
                 ]
             )
         ],
-        crs="epsg:4326",
+        crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_earth_poles() -> gpd.GeoDataFrame:
     """Get GeoDataFrame with 6 Earth poles."""
     return gpd.GeoDataFrame(
         {
-            "geometry": [
+            GEOMETRY_COLUMN: [
                 geometry.Point(0, 0),
                 geometry.Point(90, 0),
                 geometry.Point(180, 0),
                 geometry.Point(-90, 0),
                 geometry.Point(0, 90),
                 geometry.Point(0, -90),
             ]
         },
         index=[1, 2, 3, 4, 5, 6],
-        crs="EPSG:4326",
+        crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_poland() -> gpd.GeoDataFrame:
     """Get Poland GeoDataFrame."""
     world = gpd.read_file(gpd.datasets.get_path("naturalearth_lowres"))
@@ -126,8 +128,8 @@
     """Get full bounding box GeoDataFrame."""
     return geometry.box(minx=-180, maxx=180, miny=-90, maxy=90)
 
 
 @pytest.fixture  # type: ignore
 def gdf_earth_bbox(earth_bbox) -> gpd.GeoDataFrame:
     """Get full bounding box GeoDataFrame."""
-    return gpd.GeoDataFrame({"geometry": [earth_bbox]}, crs="EPSG:4326")
+    return gpd.GeoDataFrame({GEOMETRY_COLUMN: [earth_bbox]}, crs=WGS84_CRS)
```

### Comparing `srai-0.0.1/tests/regionizers/test_h3_regionizer.py` & `srai-0.1.0/tests/regionizers/test_h3_regionizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Tests for H3Regionizer."""
 from contextlib import nullcontext as does_not_raise
-from typing import Any, List
+from typing import TYPE_CHECKING, Any, List
 from unittest import TestCase
 
-import geopandas as gpd
 import pytest
 
+from srai.constants import GEOMETRY_COLUMN
 from srai.regionizers import H3Regionizer
 
+if TYPE_CHECKING:
+    import geopandas as gpd
+
+
 ut = TestCase()
 H3_RESOLUTION = 3
 
 
 @pytest.fixture  # type: ignore
 def expected_h3_indexes() -> List[str]:
     """Get expected h3 indexes."""
@@ -22,33 +26,43 @@
         "837541fffffffff",
         "83755dfffffffff",
         "837543fffffffff",
         "83754afffffffff",
     ]
 
 
+@pytest.fixture  # type: ignore
+def expected_unbuffered_h3_indexes() -> List[str]:
+    """Get expected h3 index for the unbuffered case."""
+    return [
+        "83754efffffffff",
+    ]
+
+
 @pytest.mark.parametrize(  # type: ignore
-    "gdf_fixture,expected_h3_indexes_fixture,resolution,expectation",
+    "gdf_fixture,expected_h3_indexes_fixture,resolution,buffer,expectation",
     [
-        ("gdf_polygons", "expected_h3_indexes", H3_RESOLUTION, does_not_raise()),
-        ("gdf_multipolygon", "expected_h3_indexes", H3_RESOLUTION, does_not_raise()),
-        ("gdf_empty", "expected_h3_indexes", H3_RESOLUTION, pytest.raises(AttributeError)),
-        ("gdf_polygons", "expected_h3_indexes", -1, pytest.raises(ValueError)),
-        ("gdf_polygons", "expected_h3_indexes", 16, pytest.raises(ValueError)),
-        ("gdf_no_crs", "expected_h3_indexes", H3_RESOLUTION, pytest.raises(ValueError)),
+        ("gdf_polygons", "expected_h3_indexes", H3_RESOLUTION, True, does_not_raise()),
+        ("gdf_polygons", "expected_unbuffered_h3_indexes", H3_RESOLUTION, False, does_not_raise()),
+        ("gdf_multipolygon", "expected_h3_indexes", H3_RESOLUTION, True, does_not_raise()),
+        ("gdf_empty", "expected_h3_indexes", H3_RESOLUTION, True, pytest.raises(AttributeError)),
+        ("gdf_polygons", "expected_h3_indexes", -1, True, pytest.raises(ValueError)),
+        ("gdf_polygons", "expected_h3_indexes", 16, True, pytest.raises(ValueError)),
+        ("gdf_no_crs", "expected_h3_indexes", H3_RESOLUTION, True, pytest.raises(ValueError)),
     ],
 )
 def test_transform(
     gdf_fixture: str,
     expected_h3_indexes_fixture: str,
     resolution: int,
+    buffer: bool,
     expectation: Any,
     request: Any,
 ) -> None:
     """Test transform of H3Regionizer."""
     gdf: gpd.GeoDataFrame = request.getfixturevalue(gdf_fixture)
     h3_indexes: List[str] = request.getfixturevalue(expected_h3_indexes_fixture)
     with expectation:
-        gdf_h3 = H3Regionizer(resolution).transform(gdf)
+        gdf_h3 = H3Regionizer(resolution, buffer=buffer).transform(gdf)
 
         ut.assertCountEqual(first=gdf_h3.index.to_list(), second=h3_indexes)
-        assert "geometry" in gdf_h3
+        assert GEOMETRY_COLUMN in gdf_h3
```

### Comparing `srai-0.0.1/tests/regionizers/test_voronoi_regionizer.py` & `srai-0.1.0/tests/regionizers/test_voronoi_regionizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,123 @@
 """Voronoi regionizer tests."""
 from typing import Any
 
 import geopandas as gpd
+import numpy as np
 import pytest
-from shapely.geometry import Point
+from shapely.geometry import Point, Polygon
 
+from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
 from srai.regionizers import VoronoiRegionizer
-from srai.utils import _merge_disjointed_gdf_geometries
+from srai.regionizers._spherical_voronoi import generate_voronoi_regions
+from srai.utils import merge_disjointed_gdf_geometries
 
 
-def test_empty_gdf_value_error(gdf_empty) -> None:  # type: ignore
+def test_empty_gdf_attribute_error(gdf_empty: gpd.GeoDataFrame) -> None:
     """Test checks if empty GeoDataFrames are disallowed."""
-    with pytest.raises(ValueError):
+    with pytest.raises(AttributeError):
         VoronoiRegionizer(seeds=gdf_empty)
 
 
-def test_no_crs_gdf_value_error(gdf_earth_poles, gdf_no_crs) -> None:  # type: ignore
+def test_no_crs_gdf_value_error(
+    gdf_earth_poles: gpd.GeoDataFrame, gdf_no_crs: gpd.GeoDataFrame
+) -> None:
     """Test checks if GeoDataFrames without crs are disallowed."""
     with pytest.raises(ValueError):
         vr = VoronoiRegionizer(seeds=gdf_earth_poles)
         vr.transform(gdf=gdf_no_crs)
 
 
 def test_duplicate_seeds_value_error() -> None:
     """Test checks if duplicate points are disallowed."""
     with pytest.raises(ValueError):
         seeds_gdf = gpd.GeoDataFrame(
-            {"geometry": [Point(0, 0), Point(0, 0), Point(-1, -1), Point(2, 2)]},
+            {GEOMETRY_COLUMN: [Point(0, 0), Point(0, 0), Point(-1, -1), Point(2, 2)]},
             index=[1, 2, 3, 4],
-            crs="EPSG:4326",
+            crs=WGS84_CRS,
         )
         VoronoiRegionizer(seeds=seeds_gdf)
 
 
 def test_single_seed_region() -> None:
     """Test checks if single seed is disallowed."""
     with pytest.raises(ValueError):
         seeds_gdf = gpd.GeoDataFrame(
-            {"geometry": [Point(0, 0)]},
+            {GEOMETRY_COLUMN: [Point(0, 0)]},
             index=[1],
-            crs="EPSG:4326",
+            crs=WGS84_CRS,
         )
         VoronoiRegionizer(seeds=seeds_gdf)
 
 
-def test_multiple_seeds_regions(  # type: ignore
-    gdf_earth_poles, gdf_earth_bbox, earth_bbox
+def test_single_seed_algorithm_error() -> None:
+    """Test checks if single seed is disallowed."""
+    with pytest.raises(ValueError):
+        generate_voronoi_regions(seeds=[Point(0, 0)], max_meters_between_points=10_000)
+
+
+def test_multiple_seeds_regions(
+    gdf_earth_poles: gpd.GeoDataFrame, gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon
 ) -> None:
     """Test checks if regions are generated correctly."""
     vr = VoronoiRegionizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=gdf_earth_bbox)
     assert len(result_gdf.index) == 6
-    assert _merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
+    assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
+
+
+def test_big_number_of_seeds_regions(gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
+    """Test checks if regions are generated correctly and multiprocessing working."""
+    number_of_points = 1000
+    minx, miny, maxx, maxy = earth_bbox.bounds
+    rng = np.random.default_rng()
+    randx = rng.uniform(minx, maxx, number_of_points)
+    randy = rng.uniform(miny, maxy, number_of_points)
+    coords = np.vstack((randx, randy)).T
+
+    pts = [p for p in list(map(Point, coords)) if p.covered_by(earth_bbox)]
+
+    random_points_gdf = gpd.GeoDataFrame(
+        {GEOMETRY_COLUMN: pts},
+        index=list(range(len(pts))),
+        crs=WGS84_CRS,
+    )
+
+    vr = VoronoiRegionizer(seeds=random_points_gdf)
+    result_gdf = vr.transform(gdf=gdf_earth_bbox)
+    assert len(result_gdf.index) == number_of_points
+    assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
-def test_four_close_seed_region(gdf_earth_bbox, earth_bbox) -> None:  # type: ignore
+def test_four_close_seed_region(gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
     """Test checks if four close seeds are properly evaluated."""
     seeds_gdf = gpd.GeoDataFrame(
         {
-            "geometry": [
+            GEOMETRY_COLUMN: [
                 Point(17.014997869227177, 51.09919872601259),
                 Point(16.935542631959215, 51.09380600286582),
                 Point(16.900425, 51.1162552343),
                 Point(16.932700, 51.166251),
             ]
         },
         index=[1, 2, 3, 4],
-        crs="EPSG:4326",
+        crs=WGS84_CRS,
     )
     vr = VoronoiRegionizer(seeds=seeds_gdf)
     result_gdf = vr.transform(gdf=gdf_earth_bbox)
     assert len(result_gdf.index) == 4
-    assert _merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
+    assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
-def test_default_parameter(gdf_earth_poles, earth_bbox) -> None:  # type: ignore
+def test_default_parameter(gdf_earth_poles: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
     """Test checks if regions are generated correctly with a default mask."""
     vr = VoronoiRegionizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=None)
     assert len(result_gdf.index) == 6
-    assert _merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
+    assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
 @pytest.mark.parametrize(  # type: ignore
     "gdf_fixture",
     [
         "gdf_multipolygon",
         "gdf_poland",
@@ -95,8 +129,8 @@
     request: Any,
 ) -> None:
     """Test checks if regions are clipped correctly with a provided mask."""
     gdf: gpd.GeoDataFrame = request.getfixturevalue(gdf_fixture)
     gdf_earth_poles: gpd.GeoDataFrame = request.getfixturevalue("gdf_earth_poles")
     vr = VoronoiRegionizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=gdf)
-    assert _merge_disjointed_gdf_geometries(result_gdf).difference(gdf.iloc[0].geometry).is_empty
+    assert merge_disjointed_gdf_geometries(result_gdf).difference(gdf.iloc[0].geometry).is_empty
```

