# Comparing `tmp/srai-0.1.0.tar.gz` & `tmp/srai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.1.0.tar", last modified: Thu Apr 27 20:53:34 2023, max compression
+gzip compressed data, was "srai-0.1.1.tar", last modified: Thu Apr 27 21:17:23 2023, max compression
```

## Comparing `srai-0.1.0.tar` & `srai-0.1.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0    10760 2023-04-27 20:53:11.370154 srai-0.1.0/LICENSE.md
--rw-r--r--   0        0        0    14631 2023-04-27 20:53:11.370154 srai-0.1.0/README.md
--rw-r--r--   0        0        0     4455 2023-04-27 20:53:34.210591 srai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      404 2023-04-27 20:53:11.382154 srai-0.1.0/srai/__init__.py
--rw-r--r--   0        0        0      155 2023-04-27 20:53:11.382154 srai-0.1.0/srai/constants.py
--rw-r--r--   0        0        0      755 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/__init__.py
--rw-r--r--   0        0        0     2722 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/_base.py
--rw-r--r--   0        0        0     8327 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     4840 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      136 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0     9413 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2369 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0     8553 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6932 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6319 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2908 2023-04-27 20:53:11.382154 srai-0.1.0/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2023-04-27 20:53:11.382154 srai-0.1.0/srai/exceptions.py
--rw-r--r--   0        0        0      531 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2023-04-27 20:53:11.382154 srai-0.1.0/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      725 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/_base.py
--rw-r--r--   0        0        0     2195 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5371 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      469 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     2011 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5324 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0     8849 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15758 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2438 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5536 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     5772 2023-04-27 20:53:11.382154 srai-0.1.0/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2777 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     4691 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0    10106 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/pbf_file_downloader.py
--rw-r--r--   0        0        0    10000 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_loaders/pbf_file_handler.py
--rw-r--r--   0        0        0      118 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7587 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    13854 2023-04-27 20:53:11.386155 srai-0.1.0/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      465 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     3679 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     2887 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     3221 2023-04-27 20:53:11.386155 srai-0.1.0/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      496 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11189 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14174 2023-04-27 20:53:11.386155 srai-0.1.0/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0      894 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/_base.py
--rw-r--r--   0        0        0    11462 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15447 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/administrative_boundary_regionizer.py
--rw-r--r--   0        0        0     6629 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/h3_regionizer.py
--rw-r--r--   0        0        0     3118 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/s2_regionizer.py
--rw-r--r--   0        0        0     4130 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/slippy_map_regionizer.py
--rw-r--r--   0        0        0     5916 2023-04-27 20:53:11.386155 srai-0.1.0/srai/regionizers/voronoi_regionizer.py
--rw-r--r--   0        0        0      654 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/_optional.py
--rw-r--r--   0        0        0      239 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/_pytorch_stubs.py
--rw-r--r--   0        0        0      999 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/download.py
--rw-r--r--   0        0        0      944 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/geocode.py
--rw-r--r--   0        0        0     2521 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/geometry.py
--rw-r--r--   0        0        0     1153 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/merge.py
--rw-r--r--   0        0        0      717 2023-04-27 20:53:11.386155 srai-0.1.0/srai/utils/typing.py
--rw-r--r--   0        0        0       29 2023-04-27 20:53:11.386155 srai-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     7806 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/conftest.py
--rw-r--r--   0        0        0      557 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2590 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2716 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2023-04-27 20:53:11.386155 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1061 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3037 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    24053 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0     8273 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3630 2023-04-27 20:53:11.390154 srai-0.1.0/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     1765 2023-04-27 20:53:11.390154 srai-0.1.0/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2529 2023-04-27 20:53:11.390154 srai-0.1.0/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4284 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     3413 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3276 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   111539 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     2811 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     8690 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3156 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3165 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3353 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
--rw-r--r--   0        0        0     2804 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
--rw-r--r--   0        0        0     3822 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
--rw-r--r--   0        0        0     5109 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
--rw-r--r--   0        0        0     3822 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
--rw-r--r--   0        0        0      629 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
--rw-r--r--   0        0        0    10789 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2181 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3176 2023-04-27 20:53:11.390154 srai-0.1.0/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4743 2023-04-27 20:53:11.390154 srai-0.1.0/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     4028 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     5668 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0     8063 2023-04-27 20:53:11.390154 srai-0.1.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0     5586 2023-04-27 20:53:11.394155 srai-0.1.0/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0     3665 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/conftest.py
--rw-r--r--   0        0        0     6469 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_administrative_boundary_regionizer.py
--rw-r--r--   0        0        0     2198 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_h3_regionizer.py
--rw-r--r--   0        0        0     1831 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_s2_regionizer.py
--rw-r--r--   0        0        0     2651 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_slippy_map_regionizer.py
--rw-r--r--   0        0        0     4957 2023-04-27 20:53:11.394155 srai-0.1.0/tests/regionizers/test_voronoi_regionizer.py
--rw-r--r--   0        0        0    16722 1970-01-01 00:00:00.000000 srai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-04-27 21:17:06.196857 srai-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0    14916 2023-04-27 21:17:06.196857 srai-0.1.1/README.md
+-rw-r--r--   0        0        0     4456 2023-04-27 21:17:23.285179 srai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-04-27 21:17:06.212857 srai-0.1.1/srai/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-27 21:17:06.212857 srai-0.1.1/srai/constants.py
+-rw-r--r--   0        0        0      755 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     2722 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/_base.py
+-rw-r--r--   0        0        0     8327 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     4840 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      136 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0     9413 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2369 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0     8553 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6932 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6319 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2908 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2023-04-27 21:17:06.212857 srai-0.1.1/srai/exceptions.py
+-rw-r--r--   0        0        0      531 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      725 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/_base.py
+-rw-r--r--   0        0        0     2195 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5371 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      469 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     2011 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5324 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0     8849 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15758 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2438 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5536 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     5772 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2777 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     4691 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0    10106 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/pbf_file_downloader.py
+-rw-r--r--   0        0        0    10000 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/pbf_file_handler.py
+-rw-r--r--   0        0        0      118 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7587 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    13854 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      465 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     3679 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     2887 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     3221 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      496 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11189 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14174 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0      894 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/_base.py
+-rw-r--r--   0        0        0    11462 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15447 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/administrative_boundary_regionizer.py
+-rw-r--r--   0        0        0     6629 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/h3_regionizer.py
+-rw-r--r--   0        0        0     3118 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/s2_regionizer.py
+-rw-r--r--   0        0        0     4130 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/slippy_map_regionizer.py
+-rw-r--r--   0        0        0     5916 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/voronoi_regionizer.py
+-rw-r--r--   0        0        0      654 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/_optional.py
+-rw-r--r--   0        0        0      239 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/_pytorch_stubs.py
+-rw-r--r--   0        0        0      999 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/download.py
+-rw-r--r--   0        0        0      944 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/geocode.py
+-rw-r--r--   0        0        0     2521 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/geometry.py
+-rw-r--r--   0        0        0     1153 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/merge.py
+-rw-r--r--   0        0        0      717 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/typing.py
+-rw-r--r--   0        0        0       29 2023-04-27 21:17:06.212857 srai-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/conftest.py
+-rw-r--r--   0        0        0      557 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2590 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2716 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1061 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3037 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    24053 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0     8273 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3630 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     1765 2023-04-27 21:17:06.216858 srai-0.1.1/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2529 2023-04-27 21:17:06.216858 srai-0.1.1/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4284 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     3413 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3276 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   111539 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     2811 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     8690 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3156 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3165 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3353 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
+-rw-r--r--   0        0        0     2804 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
+-rw-r--r--   0        0        0     3822 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
+-rw-r--r--   0        0        0     5109 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
+-rw-r--r--   0        0        0     3822 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
+-rw-r--r--   0        0        0      629 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
+-rw-r--r--   0        0        0    10789 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2181 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3176 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4743 2023-04-27 21:17:06.220857 srai-0.1.1/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     4028 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     5668 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0     8063 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     5586 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0     3665 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/conftest.py
+-rw-r--r--   0        0        0     6469 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_administrative_boundary_regionizer.py
+-rw-r--r--   0        0        0     2198 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_h3_regionizer.py
+-rw-r--r--   0        0        0     1831 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_s2_regionizer.py
+-rw-r--r--   0        0        0     2651 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_slippy_map_regionizer.py
+-rw-r--r--   0        0        0     4957 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_voronoi_regionizer.py
+-rw-r--r--   0        0        0    17007 1970-01-01 00:00:00.000000 srai-0.1.1/PKG-INFO
```

### Comparing `srai-0.1.0/LICENSE.md` & `srai-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/README.md` & `srai-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     <a href="https://pypi.org/project/srai" target="_blank">
         <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/srai">
     </a>
 </p>
 
 # Spatial Representations for Artificial Intelligence
 
-<p style="text-align: center;">⚠️🚧 This library is under HEAVY development. Expect breaking changes between `minor` versions 🚧⚠️</p>
+<p align="center">⚠️🚧 This library is under HEAVY development. Expect breaking changes between <i>minor</i> versions 🚧⚠️</p>
 
-<p style="text-align: center;">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
+<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
 
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting starded for installation and quick srart instructions.
 
 ## Use cases
 
 In the current state, `srai` provides the following functionalities:
 
@@ -94,15 +94,15 @@
 
 parks_gdf = loader.load(area, query)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0)"], tiles_style="CartoDB positron")
 parks_gdf.explore(m=folium_map, color="forestgreen")
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_osm_data.jpg"  style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_osm_data.jpg"  style="max-width:600px;width:100%"/>
 </p>
 
 ### Downloading road network
 
 Road network downloading is a special case of OSM data downloading. To download road network for a given area, use `OSMWayLoader` class:
 
 ```python
@@ -117,15 +117,15 @@
 nodes, edges = loader.load(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 edges[["geometry"]].explore(m=folium_map, color="seagreen")
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_road_network_data.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_road_network_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Downloading GTFS data
 
 To extract features from GTFS use `GTFSLoader`. It will extract trip count and available directions for each stop in 1h time windows.
 
 ```python
@@ -143,15 +143,15 @@
 features = loader.load(gtfs_file)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 features[["trips_at_8", "geometry"]].explore("trips_at_8", m=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Regionization
 
 Regionization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
 
 * `H3Regionizer` - regionization using [Uber's H3 library](https://github.com/uber/h3)
@@ -171,15 +171,15 @@
 regions = regionizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_regions(regions_gdf=regions, map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Embedding
 
 Embedding is a process of mapping regions into a vector space. This can be done in a variety of ways:
 
 * `Hex2VecEmbedder` - embedding using hex2vec[1] algorithm
@@ -212,15 +212,15 @@
 embeddings = embedder.transform(regions, features, joint)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, "amenity_bicycle_parking", map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/embedding_count_embedder.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_count_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 `CountEmbedder` is a simple method, which does not require fitting. Other methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and can be used in a similar way to `scikit-learn` estimators:
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
@@ -253,15 +253,15 @@
 embeddings = embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, 0, map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Plotting, utilities and more
 
 We also provide utilities for different spatial operations and plotting functions adopted to data formats used in `srai` For a full list of available methods, please refer to the [documentation](https://srai-lab.github.io/srai).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
  [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
-â ï¸ð§ This library is under HEAVY development. Expect breaking changes
-between `minor` versions ð§â ï¸
-ð¬ Feel free to open an issue if you find anything confusing or not working
-ð¨ï¸
+  â ï¸ð§ This library is under HEAVY development. Expect breaking changes
+                       between minor versions ð§â ï¸
+ ð¬ Feel free to open an issue if you find anything confusing or not working
+                                    ð¨ï¸
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims
 to provide simple and efficient solutions to geospatial problems that are
 accessible to everybody and reusable in various contexts where geospatial data
 can be used. It is a Python module integrating many geo-related algorithms in a
 single package with unified API. Please see getting starded for installation
 and quick srart instructions. ## Use cases In the current state, `srai`
 provides the following functionalities: * **OSM data download** - downloading
@@ -47,49 +47,53 @@
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
 import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
 srai.plotting import plot_regions query = {"leisure": "park"} area =
 geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader() parks_gdf
 = loader.load(area, query) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore(m=folium_map,
 color="forestgreen") ```
-                [./docs/assets/images/downloading_osm_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                           downloading_osm_data.jpg]
 ### Downloading road network Road network downloading is a special case of OSM
 data downloading. To download road network for a given area, use `OSMWayLoader`
 class: ```python from srai.loaders import OSMWayLoader from
 srai.loaders.osm_way_loader import NetworkType from srai.utils import
 geocode_to_region_gdf from srai.plotting import plot_regions area =
 geocode_to_region_gdf("Utrecht, Netherlands") loader = OSMWayLoader
 (NetworkType.BIKE) nodes, edges = loader.load(area) folium_map = plot_regions
 (area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") edges[
 ["geometry"]].explore(m=folium_map, color="seagreen") ```
-           [./docs/assets/images/downloading_road_network_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                      downloading_road_network_data.jpg]
 ### Downloading GTFS data To extract features from GTFS use `GTFSLoader`. It
 will extract trip count and available directions for each stop in 1h time
 windows. ```python from pathlib import Path from srai.loaders import GTFSLoader
 from srai.utils import geocode_to_region_gdf, download_file from srai.plotting
 import plot_regions area = geocode_to_region_gdf("Vienna, Austria") gtfs_file =
 Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
 888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
 loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
 "geometry"]].explore("trips_at_8", m=folium_map) ```
-               [./docs/assets/images/downloading_gtfs_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                          downloading_gtfs_data.jpg]
 ### Regionization Regionization is a process of dividing a given area into
 smaller regions. This can be done in a variety of ways: * `H3Regionizer` -
 regionization using [Uber's H3 library](https://github.com/uber/h3) *
 `S2Regionizer` - regionization using [Google's S2 library](https://github.com/
 google/s2geometry) * `VoronoiRegionizer` - regionization using Voronoi diagram
 * `AdministativeBoundaryRegionizer` - regionization using administrative
 boundaries Example: ```python from srai.regionizers import H3Regionizer from
 srai.utils import geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
 Germany") regionizer = H3Regionizer(resolution=7) regions =
 regionizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
 (regions_gdf=regions, map=folium_map) ```
-                   [./docs/assets/images/regionization.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                              regionization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
@@ -103,15 +107,16 @@
 IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
 geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
 regions = regionizer.transform(area) joint = joiner.transform(regions,
 features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
 features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
 tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
 "amenity_bicycle_parking", map=folium_map) ```
-              [./docs/assets/images/embedding_count_embedder.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                         embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
@@ -124,15 +129,16 @@
 = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3])
 # Option 1: fit and transform # embedder.fit(regions, features, joint,
 neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
 features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
 (regions, features, joint, neighbourhood, batch_size=128) folium_map =
 plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
 positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
-             [./docs/assets/images/embedding_hex2vec_embedder.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                        embedding_hex2vec_embedder.jpg]
 ### Plotting, utilities and more We also provide utilities for different
 spatial operations and plotting functions adopted to data formats used in
 `srai` For a full list of available methods, please refer to the
 [documentation](https://srai-lab.github.io/srai). ## Contributing If you are
 willing to contribute to `srai`, feel free to do so! Visit [our contributing
 guide](./CONTRIBUTING.md) for more details. ## Publications Some of the methods
 implemented in `srai` have been published in scientific journals and
```

### Comparing `srai-0.1.0/pyproject.toml` & `srai-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.1.0"
+version = "0.1.1"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "srai", email = "spatialrepresentationsforai@gmail.com" },
 ]
 dependencies = [
     "pandas",
     "geopandas",
@@ -191,19 +191,19 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore: bump version {old_version} -> {new_version}"
 commit = true
-tag = true
+tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     "current_version = \"{version}\"",
     "version = \"{version}\"",
 ]
```

### Comparing `srai-0.1.0/srai/embedders/__init__.py` & `srai-0.1.1/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/_base.py` & `srai-0.1.1/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/contextual_count_embedder.py` & `srai-0.1.1/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/count_embedder.py` & `srai-0.1.1/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/gtfs2vec/embedder.py` & `srai-0.1.1/srai/embedders/gtfs2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/gtfs2vec/model.py` & `srai-0.1.1/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/hex2vec/embedder.py` & `srai-0.1.1/srai/embedders/hex2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/hex2vec/model.py` & `srai-0.1.1/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.1.1/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/highway2vec/embedder.py` & `srai-0.1.1/srai/embedders/highway2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/embedders/highway2vec/model.py` & `srai-0.1.1/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/exceptions.py` & `srai-0.1.1/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/joiners/__init__.py` & `srai-0.1.1/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/joiners/_base.py` & `srai-0.1.1/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/joiners/intersection_joiner.py` & `srai-0.1.1/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/__init__.py` & `srai-0.1.1/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/_base.py` & `srai-0.1.1/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/geoparquet_loader.py` & `srai-0.1.1/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/gtfs_loader.py` & `srai-0.1.1/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/_base.py` & `srai-0.1.1/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.1.1/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.1.1/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.1.1/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.1.1/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.1.1/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.1.1/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.1.1/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.1.1/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.1.1/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/pbf_file_downloader.py` & `srai-0.1.1/srai/loaders/osm_loaders/pbf_file_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_loaders/pbf_file_handler.py` & `srai-0.1.1/srai/loaders/osm_loaders/pbf_file_handler.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_way_loader/constants.py` & `srai-0.1.1/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.1.1/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/neighbourhoods/_base.py` & `srai-0.1.1/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.1.1/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.1.1/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/plotting/folium_wrapper.py` & `srai-0.1.1/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/plotting/plotly_wrapper.py` & `srai-0.1.1/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/__init__.py` & `srai-0.1.1/srai/regionizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/_base.py` & `srai-0.1.1/srai/regionizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/_spherical_voronoi.py` & `srai-0.1.1/srai/regionizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/administrative_boundary_regionizer.py` & `srai-0.1.1/srai/regionizers/administrative_boundary_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/h3_regionizer.py` & `srai-0.1.1/srai/regionizers/h3_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/s2_regionizer.py` & `srai-0.1.1/srai/regionizers/s2_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/slippy_map_regionizer.py` & `srai-0.1.1/srai/regionizers/slippy_map_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/regionizers/voronoi_regionizer.py` & `srai-0.1.1/srai/regionizers/voronoi_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/__init__.py` & `srai-0.1.1/srai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/_optional.py` & `srai-0.1.1/srai/utils/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/download.py` & `srai-0.1.1/srai/utils/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/geocode.py` & `srai-0.1.1/srai/utils/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/geometry.py` & `srai-0.1.1/srai/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/merge.py` & `srai-0.1.1/srai/utils/merge.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/srai/utils/typing.py` & `srai-0.1.1/srai/utils/typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/conftest.py` & `srai-0.1.1/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/constants.py` & `srai-0.1.1/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/generation.py` & `srai-0.1.1/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_embedder.py` & `srai-0.1.1/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_model.py` & `srai-0.1.1/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.1.1/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/test_contextual_count_embedder.py` & `srai-0.1.1/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/test_count_embedder.py` & `srai-0.1.1/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.1.1/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/embedders/test_highway2vec_embedder.py` & `srai-0.1.1/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/joiners/conftest.py` & `srai-0.1.1/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/joiners/test_intersection_joiner.py` & `srai-0.1.1/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/conftest.py` & `srai-0.1.1/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/conftest.py` & `srai-0.1.1/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.1.1/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.1.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.1.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.1.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.1.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.1.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.1.1/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.1.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.1.1/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.1.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl` & `srai-0.1.1/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.1.1/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/test_files/example.parquet` & `srai-0.1.1/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/test_geoparquet_loader.py` & `srai-0.1.1/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/loaders/test_gtfs_loader.py` & `srai-0.1.1/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.1.1/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.1.1/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.1.1/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.1.1/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.1.1/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/conftest.py` & `srai-0.1.1/tests/regionizers/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/test_administrative_boundary_regionizer.py` & `srai-0.1.1/tests/regionizers/test_administrative_boundary_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/test_h3_regionizer.py` & `srai-0.1.1/tests/regionizers/test_h3_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/test_s2_regionizer.py` & `srai-0.1.1/tests/regionizers/test_s2_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/test_slippy_map_regionizer.py` & `srai-0.1.1/tests/regionizers/test_slippy_map_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/tests/regionizers/test_voronoi_regionizer.py` & `srai-0.1.1/tests/regionizers/test_voronoi_regionizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.0/PKG-INFO` & `srai-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of python modules for geospatial machine learning and data mining
 Author-Email: srai <spatialrepresentationsforai@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -87,17 +87,17 @@
     <a href="https://pypi.org/project/srai" target="_blank">
         <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/srai">
     </a>
 </p>
 
 # Spatial Representations for Artificial Intelligence
 
-<p style="text-align: center;">⚠️🚧 This library is under HEAVY development. Expect breaking changes between `minor` versions 🚧⚠️</p>
+<p align="center">⚠️🚧 This library is under HEAVY development. Expect breaking changes between <i>minor</i> versions 🚧⚠️</p>
 
-<p style="text-align: center;">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
+<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
 
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting starded for installation and quick srart instructions.
 
 ## Use cases
 
 In the current state, `srai` provides the following functionalities:
 
@@ -157,15 +157,15 @@
 
 parks_gdf = loader.load(area, query)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0)"], tiles_style="CartoDB positron")
 parks_gdf.explore(m=folium_map, color="forestgreen")
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_osm_data.jpg"  style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_osm_data.jpg"  style="max-width:600px;width:100%"/>
 </p>
 
 ### Downloading road network
 
 Road network downloading is a special case of OSM data downloading. To download road network for a given area, use `OSMWayLoader` class:
 
 ```python
@@ -180,15 +180,15 @@
 nodes, edges = loader.load(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 edges[["geometry"]].explore(m=folium_map, color="seagreen")
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_road_network_data.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_road_network_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Downloading GTFS data
 
 To extract features from GTFS use `GTFSLoader`. It will extract trip count and available directions for each stop in 1h time windows.
 
 ```python
@@ -206,15 +206,15 @@
 features = loader.load(gtfs_file)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 features[["trips_at_8", "geometry"]].explore("trips_at_8", m=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Regionization
 
 Regionization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
 
 * `H3Regionizer` - regionization using [Uber's H3 library](https://github.com/uber/h3)
@@ -234,15 +234,15 @@
 regions = regionizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_regions(regions_gdf=regions, map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Embedding
 
 Embedding is a process of mapping regions into a vector space. This can be done in a variety of ways:
 
 * `Hex2VecEmbedder` - embedding using hex2vec[1] algorithm
@@ -275,15 +275,15 @@
 embeddings = embedder.transform(regions, features, joint)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, "amenity_bicycle_parking", map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/embedding_count_embedder.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_count_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 `CountEmbedder` is a simple method, which does not require fitting. Other methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and can be used in a similar way to `scikit-learn` estimators:
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
@@ -316,15 +316,15 @@
 embeddings = embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, 0, map=folium_map)
 ```
 
 <p align="center">
-  <img src="./docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Plotting, utilities and more
 
 We also provide utilities for different spatial operations and plotting functions adopted to data formats used in `srai` For a full list of available methods, please refer to the [documentation](https://srai-lab.github.io/srai).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srai Version: 0.1.0 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.1.1 Summary: A set of python
 modules for geospatial machine learning and data mining Author-Email: srai
 gmail.com> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -31,18 +31,18 @@
 torch Provides-Extra: all Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
-â ï¸ð§ This library is under HEAVY development. Expect breaking changes
-between `minor` versions ð§â ï¸
-ð¬ Feel free to open an issue if you find anything confusing or not working
-ð¨ï¸
+  â ï¸ð§ This library is under HEAVY development. Expect breaking changes
+                       between minor versions ð§â ï¸
+ ð¬ Feel free to open an issue if you find anything confusing or not working
+                                    ð¨ï¸
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims
 to provide simple and efficient solutions to geospatial problems that are
 accessible to everybody and reusable in various contexts where geospatial data
 can be used. It is a Python module integrating many geo-related algorithms in a
 single package with unified API. Please see getting starded for installation
 and quick srart instructions. ## Use cases In the current state, `srai`
 provides the following functionalities: * **OSM data download** - downloading
@@ -78,49 +78,53 @@
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
 import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
 srai.plotting import plot_regions query = {"leisure": "park"} area =
 geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader() parks_gdf
 = loader.load(area, query) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore(m=folium_map,
 color="forestgreen") ```
-                [./docs/assets/images/downloading_osm_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                           downloading_osm_data.jpg]
 ### Downloading road network Road network downloading is a special case of OSM
 data downloading. To download road network for a given area, use `OSMWayLoader`
 class: ```python from srai.loaders import OSMWayLoader from
 srai.loaders.osm_way_loader import NetworkType from srai.utils import
 geocode_to_region_gdf from srai.plotting import plot_regions area =
 geocode_to_region_gdf("Utrecht, Netherlands") loader = OSMWayLoader
 (NetworkType.BIKE) nodes, edges = loader.load(area) folium_map = plot_regions
 (area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") edges[
 ["geometry"]].explore(m=folium_map, color="seagreen") ```
-           [./docs/assets/images/downloading_road_network_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                      downloading_road_network_data.jpg]
 ### Downloading GTFS data To extract features from GTFS use `GTFSLoader`. It
 will extract trip count and available directions for each stop in 1h time
 windows. ```python from pathlib import Path from srai.loaders import GTFSLoader
 from srai.utils import geocode_to_region_gdf, download_file from srai.plotting
 import plot_regions area = geocode_to_region_gdf("Vienna, Austria") gtfs_file =
 Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
 888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
 loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
 "geometry"]].explore("trips_at_8", m=folium_map) ```
-               [./docs/assets/images/downloading_gtfs_data.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                          downloading_gtfs_data.jpg]
 ### Regionization Regionization is a process of dividing a given area into
 smaller regions. This can be done in a variety of ways: * `H3Regionizer` -
 regionization using [Uber's H3 library](https://github.com/uber/h3) *
 `S2Regionizer` - regionization using [Google's S2 library](https://github.com/
 google/s2geometry) * `VoronoiRegionizer` - regionization using Voronoi diagram
 * `AdministativeBoundaryRegionizer` - regionization using administrative
 boundaries Example: ```python from srai.regionizers import H3Regionizer from
 srai.utils import geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
 Germany") regionizer = H3Regionizer(resolution=7) regions =
 regionizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
 (regions_gdf=regions, map=folium_map) ```
-                   [./docs/assets/images/regionization.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                              regionization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
@@ -134,15 +138,16 @@
 IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
 geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
 regions = regionizer.transform(area) joint = joiner.transform(regions,
 features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
 features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
 tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
 "amenity_bicycle_parking", map=folium_map) ```
-              [./docs/assets/images/embedding_count_embedder.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                         embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
@@ -155,15 +160,16 @@
 = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3])
 # Option 1: fit and transform # embedder.fit(regions, features, joint,
 neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
 features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
 (regions, features, joint, neighbourhood, batch_size=128) folium_map =
 plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
 positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
-             [./docs/assets/images/embedding_hex2vec_embedder.jpg]
+   [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
+                        embedding_hex2vec_embedder.jpg]
 ### Plotting, utilities and more We also provide utilities for different
 spatial operations and plotting functions adopted to data formats used in
 `srai` For a full list of available methods, please refer to the
 [documentation](https://srai-lab.github.io/srai). ## Contributing If you are
 willing to contribute to `srai`, feel free to do so! Visit [our contributing
 guide](./CONTRIBUTING.md) for more details. ## Publications Some of the methods
 implemented in `srai` have been published in scientific journals and
```

