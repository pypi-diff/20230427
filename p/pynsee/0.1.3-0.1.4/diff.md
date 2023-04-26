# Comparing `tmp/pynsee-0.1.3.tar.gz` & `tmp/pynsee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynsee-0.1.3.tar", last modified: Mon Feb 27 21:47:27 2023, max compression
+gzip compressed data, was "pynsee-0.1.4.tar", last modified: Wed Apr 26 22:24:06 2023, max compression
```

## Comparing `pynsee-0.1.3.tar` & `pynsee-0.1.4.tar`

### file list

```diff
@@ -1,176 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.173883 pynsee-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-02-27 21:47:21.000000 pynsee-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-02-27 21:47:27.169883 pynsee-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8496 2023-02-27 21:47:21.000000 pynsee-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.137882 pynsee-0.1.3/pynsee/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.141882 pynsee-0.1.3/pynsee/download/
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_check_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_download_pb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_download_store_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_get_dict_data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_get_file_list_internal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_get_value_label.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_import_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4435 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_load_data_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/_unzip_pb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.141882 pynsee-0.1.3/pynsee/download/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    94572 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/data/liste_donnees.zip
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/download_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/get_column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/download/get_file_list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.145882 pynsee-0.1.3/pynsee/geodata/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/GeoFrDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_add_insee_dep.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_convert_polygon.py
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_extract_bounds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_geojson_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_bbox_list.py
--rw-r--r--   0 runner    (1001) docker     (122)    18718 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_bbox_list_full.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_data_with_bbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_full_list_wfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_geodata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_get_geom.py
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_make_offshore_points.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/_rescale_geom.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/get_geodata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/get_geodata_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/get_geom.py
--rw-r--r--   0 runner    (1001) docker     (122)     4717 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/translate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/geodata/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.145882 pynsee-0.1.3/pynsee/localdata/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2506 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_find_latest_local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_get_geo_list_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_get_geo_relation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_get_insee_local_onegeo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_get_insee_one_area.py
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/_warning_local_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.145882 pynsee-0.1.3/pynsee/localdata/data/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    31240 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/data/local_metadata.zip
--rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_area_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_ascending_area.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_descending_area.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_geo_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_included_area.py
--rw-r--r--   0 runner    (1001) docker     (122)     5656 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_local_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_local_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_new_city.py
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_nivgeo_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_old_city.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/localdata/get_population.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.149882 pynsee-0.1.3/pynsee/macrodata/
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_add_numeric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_build_series_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_download_idbank_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_dwn_idbank_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_dataset_dimension.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_dataset_list_internal.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_dataset_metadata_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_date.py
--rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_idbank_internal_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_idbank_internal_data_harmonized.py
--rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/_get_insee.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.149882 pynsee-0.1.3/pynsee/macrodata/data/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/data/dataset_list_internal.zip
--rw-r--r--   0 runner    (1001) docker     (122)  9061009 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/data/idbank_list_internal.zip
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_column_title.py
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_dataset_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_last_release.py
--rw-r--r--   0 runner    (1001) docker     (122)     5733 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_series.py
--rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_series_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/get_series_title.py
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/macrodata/search_macrodata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.165882 pynsee-0.1.3/pynsee/metadata/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/_add_A17_activity.py
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/_add_A5_activity.py
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/_get_naf.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/_get_nomenclature_agreg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.165882 pynsee-0.1.3/pynsee/metadata/data/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   422269 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/data/definition.zip
--rw-r--r--   0 runner    (1001) docker     (122)    77211 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/data/naf.zip
--rw-r--r--   0 runner    (1001) docker     (122)     9167 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/get_activity_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/get_definition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/get_definition_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/get_legal_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/metadata/get_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.165882 pynsee-0.1.3/pynsee/sirene/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/SireneDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7393 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_clean_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_employee_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_get_location_openstreetmap.py
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_make_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_request_sirene.py
--rw-r--r--   0 runner    (1001) docker     (122)     3649 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/_street_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/get_dimension_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     6804 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/get_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/get_sirene_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/get_sirene_relatives.py
--rw-r--r--   0 runner    (1001) docker     (122)     8418 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/sirene/search_sirene.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/pynsee/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_clean_insee_folder.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_clean_str.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_create_insee_folder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_envir_token.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_temp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_get_token_from_insee.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_make_dataframe_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_move_col_after.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_paste.py
--rw-r--r--   0 runner    (1001) docker     (122)     5120 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_request_insee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_wait_api_query_limit.py
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/_warning_cached_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/clear_all_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-02-27 21:47:21.000000 pynsee-0.1.3/pynsee/utils/init_conn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.137882 pynsee-0.1.3/pynsee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-02-27 21:47:27.000000 pynsee-0.1.3/pynsee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-02-27 21:47:27.000000 pynsee-0.1.3/pynsee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 21:47:27.000000 pynsee-0.1.3/pynsee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-02-27 21:47:27.000000 pynsee-0.1.3/pynsee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-02-27 21:47:27.000000 pynsee-0.1.3/pynsee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-02-27 21:47:21.000000 pynsee-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-27 21:47:27.173883 pynsee-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-02-27 21:47:21.000000 pynsee-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/download/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/download/test_pynsee_download.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/geodata/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/geodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/geodata/test_pynsee_geodata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/localdata/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/localdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10611 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/localdata/test_pynsee_localdata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/macrodata/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/macrodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/macrodata/test_pynsee_macrodata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/metadata/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/metadata/test_pynsee_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/sirene/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/sirene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9220 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/sirene/test_pynsee_sirene.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:47:27.169883 pynsee-0.1.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4757 2023-02-27 21:47:21.000000 pynsee-0.1.3/tests/utils/test_pynsee_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.559404 pynsee-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-04-26 22:24:00.000000 pynsee-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-04-26 22:24:06.559404 pynsee-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8496 2023-04-26 22:24:00.000000 pynsee-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.531404 pynsee-0.1.4/pynsee/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.531404 pynsee-0.1.4/pynsee/download/
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_check_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_download_pb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_download_store_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_get_dict_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_get_file_list_internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_get_value_label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_import_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4435 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_load_data_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/_unzip_pb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.531404 pynsee-0.1.4/pynsee/download/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    94572 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/data/liste_donnees.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/get_column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/download/get_file_list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.535404 pynsee-0.1.4/pynsee/geodata/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/GeoFrDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_add_insee_dep.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_convert_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_extract_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_find_wfs_closest_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_geojson_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_bbox_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18718 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_bbox_list_full.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4252 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_data_with_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_full_list_wfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7548 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_geodata_with_backup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_get_geom.py
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_make_offshore_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/_rescale_geom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/get_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/get_geodata_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/get_geom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4717 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/geodata/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.535404 pynsee-0.1.4/pynsee/localdata/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2506 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_find_latest_local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_get_geo_list_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_get_geo_relation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_get_insee_local_onegeo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_get_insee_one_area.py
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/_warning_local_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.535404 pynsee-0.1.4/pynsee/localdata/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31240 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/data/local_metadata.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_area_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_ascending_area.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_descending_area.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_geo_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_included_area.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5656 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_local_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_new_city.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_nivgeo_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_old_city.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/localdata/get_population.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.539404 pynsee-0.1.4/pynsee/macrodata/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_add_numeric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_build_series_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_download_idbank_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_dwn_idbank_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_dataset_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_dataset_list_internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_dataset_metadata_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_idbank_internal_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_idbank_internal_data_harmonized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_get_insee.py
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/_load_dataset_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.539404 pynsee-0.1.4/pynsee/macrodata/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/data/dataset_list_internal.zip
+-rw-r--r--   0 runner    (1001) docker     (122)  9061009 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/data/idbank_list_internal.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_column_title.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_dataset_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_last_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_series.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_series_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/get_series_title.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/macrodata/search_macrodata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.551404 pynsee-0.1.4/pynsee/metadata/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/_add_A17_activity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/_add_A5_activity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/_get_naf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/_get_nomenclature_agreg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.551404 pynsee-0.1.4/pynsee/metadata/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   422269 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/data/definition.zip
+-rw-r--r--   0 runner    (1001) docker     (122)    77211 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/data/naf.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     9167 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/get_activity_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/get_definition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/get_definition_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/get_legal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/metadata/get_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.551404 pynsee-0.1.4/pynsee/sirene/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/SireneDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7393 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_clean_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_employee_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_get_location_openstreetmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_make_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_request_sirene.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3649 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/_street_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/get_dimension_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6804 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/get_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/get_sirene_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/get_sirene_relatives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8418 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/sirene/search_sirene.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/pynsee/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_clean_insee_folder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_clean_str.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_create_insee_folder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_envir_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_temp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_get_token_from_insee.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_make_dataframe_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_move_col_after.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_paste.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_request_insee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_wait_api_query_limit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/_warning_cached_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/clear_all_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-04-26 22:24:00.000000 pynsee-0.1.4/pynsee/utils/init_conn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.531404 pynsee-0.1.4/pynsee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-04-26 22:24:06.000000 pynsee-0.1.4/pynsee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-04-26 22:24:06.000000 pynsee-0.1.4/pynsee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 22:24:06.000000 pynsee-0.1.4/pynsee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-26 22:24:06.000000 pynsee-0.1.4/pynsee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-26 22:24:06.000000 pynsee-0.1.4/pynsee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-26 22:24:00.000000 pynsee-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 22:24:06.559404 pynsee-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-04-26 22:24:00.000000 pynsee-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/download/test_pynsee_download.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/geodata/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/geodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6329 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/geodata/test_pynsee_geodata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/localdata/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/localdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10611 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/localdata/test_pynsee_localdata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/macrodata/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/macrodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10305 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/macrodata/test_pynsee_macrodata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.555405 pynsee-0.1.4/tests/metadata/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/metadata/test_pynsee_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.559404 pynsee-0.1.4/tests/sirene/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/sirene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9220 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/sirene/test_pynsee_sirene.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:24:06.559404 pynsee-0.1.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4757 2023-04-26 22:24:00.000000 pynsee-0.1.4/tests/utils/test_pynsee_utils.py
```

### Comparing `pynsee-0.1.3/LICENSE.md` & `pynsee-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/PKG-INFO` & `pynsee-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynsee
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools to Easily Search and Download French Data From INSEE and IGN APIs
 Home-page: https://pynsee.readthedocs.io/en/latest/
 Author: Hadrien Leclerc, Lino Galiana
 Author-email: leclerc.hadrien@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/InseeFrLab/pynsee/issues
 Description: .. role:: raw-html-m2r(raw)
```

### Comparing `pynsee-0.1.3/README.rst` & `pynsee-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_check_url.py` & `pynsee-0.1.4/pynsee/download/_check_url.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_download_pb.py` & `pynsee-0.1.4/pynsee/download/_download_pb.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_download_store_file.py` & `pynsee-0.1.4/pynsee/download/_download_store_file.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_get_dict_data_source.py` & `pynsee-0.1.4/pynsee/download/_get_dict_data_source.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_get_value_label.py` & `pynsee-0.1.4/pynsee/download/_get_value_label.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_import_options.py` & `pynsee-0.1.4/pynsee/download/_import_options.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_load_data_from_schema.py` & `pynsee-0.1.4/pynsee/download/_load_data_from_schema.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/_unzip_pb.py` & `pynsee-0.1.4/pynsee/download/_unzip_pb.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/data/liste_donnees.zip` & `pynsee-0.1.4/pynsee/download/data/liste_donnees.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/download_file.py` & `pynsee-0.1.4/pynsee/download/download_file.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/get_column_metadata.py` & `pynsee-0.1.4/pynsee/download/get_column_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/download/get_file_list.py` & `pynsee-0.1.4/pynsee/download/get_file_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_add_insee_dep.py` & `pynsee-0.1.4/pynsee/geodata/_add_insee_dep.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tqdm import trange
 from pandas.api.types import CategoricalDtype
 
 from pynsee.geodata._get_geodata import _get_geodata
-
+from pynsee.geodata._get_geodata_with_backup import _get_geodata_with_backup
 
 def _add_insee_dep(df):
 
     df = df.reset_index(drop=True)
 
     # option 1 : get insee_dep from id_com colum
     df = _add_insee_dep_from_id_com(df)
@@ -22,57 +22,67 @@
 
 def _add_insee_dep_region(df):
 
     try:
         if "insee_dep_geometry" not in df.columns:
             if "id" in df.columns:
                 if all(df.id.str.contains("^REGION")):
-                    dep = _get_geodata("ADMINEXPRESS-COG.LATEST:departement")
+                    dataset_id = "ADMINEXPRESS-COG-CARTO.LATEST:departement"
+                    dep = _get_geodata_with_backup(dataset_id)
+                        
                     dep = dep[["insee_dep", "insee_reg", "geometry"]]
                     dep = dep.rename(columns={"geometry": "insee_dep_geometry"})
                     df = df.merge(dep, on="insee_reg", how="left")
 
-    except:
+    except Exception as e:
+        #print(e)
         pass
 
     return df
 
 
 def _add_insee_dep_from_id_com(df):
 
     try:
 
         if ("id_com" in df.columns) and ("insee_dep_geometry" not in df.columns):
-            com = _get_geodata("ADMINEXPRESS-COG-CARTO.LATEST:commune")
+            dataset_id = "ADMINEXPRESS-COG-CARTO.LATEST:commune"
+            com = _get_geodata_with_backup(dataset_id)
+                     
             com = com[["id", "insee_dep"]]
             com = com.rename(columns={"id": "id_com"})
             df = df.merge(com, on="id_com", how="left")
 
-            dep = _get_geodata("ADMINEXPRESS-COG.LATEST:departement")
+            dataset_id = "ADMINEXPRESS-COG-CARTO.LATEST:departement"
+            dep = _get_geodata_with_backup(dataset_id)
+            
             dep = dep[["insee_dep", "geometry"]]
             dep = dep.rename(columns={"geometry": "insee_dep_geometry"})
 
             df = df.merge(dep, on="insee_dep", how="left")
-    except:
+    except Exception as e:
+        #print(e)
         pass
 
     return df
 
 
 def _add_insee_dep_from_geodata(df):
 
     try:
         if "insee_dep_geometry" not in df.columns:
 
             df = df.reset_index(drop=True)
 
             list_dep = []
             list_dep_geo = []
-
-            dep_list = _get_geodata("ADMINEXPRESS-COG.LATEST:departement")
+            
+            dataset_id = "ADMINEXPRESS-COG-CARTO.LATEST:departement"
+            dep_list = _get_geodata_with_backup(dataset_id)
+            
             list_ovdep = ["971", "972", "974", "973", "976"]
             list_other_dep = [d for d in dep_list.insee_dep if d not in list_ovdep]
             dep_order = list_ovdep + list_other_dep
 
             dep_list["insee_dep"] = dep_list["insee_dep"].astype(
                 CategoricalDtype(categories=dep_order, ordered=True)
             )
@@ -96,11 +106,12 @@
                     pass
 
                 list_dep += [dep]
                 list_dep_geo += [depgeo]
 
             df["insee_dep"] = list_dep
             df["insee_dep_geometry"] = list_dep_geo
-    except:
+    except Exception as e:
+        #print(e)
         pass
 
     return df
```

### Comparing `pynsee-0.1.3/pynsee/geodata/_distance.py` & `pynsee-0.1.4/pynsee/geodata/_distance.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_geojson_parser.py` & `pynsee-0.1.4/pynsee/geodata/_geojson_parser.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_bbox_list.py` & `pynsee-0.1.4/pynsee/geodata/_get_bbox_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_bbox_list_full.py` & `pynsee-0.1.4/pynsee/geodata/_get_bbox_list_full.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_capabilities.py` & `pynsee-0.1.4/pynsee/geodata/_get_capabilities.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_center.py` & `pynsee-0.1.4/pynsee/geodata/_get_center.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_data_with_bbox.py` & `pynsee-0.1.4/pynsee/geodata/_get_data_with_bbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,17 @@
         try:
             data_json = r.json()
         except Exception:
             print(
                 f"!!! The following query failed, some data might be missing !!!\n{link_query}"
             )
             return pd.DataFrame()
-
+        
+    session.close()
+    
     if "features" in data_json.keys():
 
         json = data_json["features"]
 
         if len(json) > 0:
 
             if len(json) == 1000:
```

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_full_list_wfs.py` & `pynsee-0.1.4/pynsee/geodata/_get_full_list_wfs.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_geodata.py` & `pynsee-0.1.4/pynsee/geodata/_get_geodata.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,14 @@
         link = link0 + BBOX
     else:
         link = link0
 
     insee_folder = _create_insee_folder()
     file_name = insee_folder + "/" + _hash(link)
 
-    session = requests.Session()
-    retry = Retry(connect=3, backoff_factor=1)
-    adapter = HTTPAdapter(max_retries=retry)
-    session.mount("http://", adapter)
-    session.mount("https://", adapter)
-
     try:
         home = str(Path.home())
         user_agent = os.path.basename(home)
     except:
         user_agent = ""
 
     headers = {"User-Agent": "python_package_pynsee_" + user_agent.replace("/", "")}
@@ -118,21 +112,29 @@
     try:
         proxies = {"http": os.environ["http_proxy"], "https": os.environ["https_proxy"]}
     except:
         proxies = {"http": "", "https": ""}
 
     if (not os.path.exists(file_name)) | (update is True):
         
+        session = requests.Session()
+        retry = Retry(connect=3, backoff_factor=1)
+        adapter = HTTPAdapter(max_retries=retry)
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+        
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         data = session.get(link, proxies=proxies, headers=headers, verify=False)
 
         if data.status_code == 502:
             time.sleep(1)
             data = session.get(link, proxies=proxies, headers=headers)
-
+            
+        session.close()
+        
         if data.status_code != 200:
             print("Query:\n%s" % link)
             print(data)
             print(data.text)
             return pd.DataFrame(
                 {"status": data.status_code, "comment": data.text}, index=[0]
             )
@@ -229,9 +231,9 @@
             data_all_clean = _get_geodata(
                 id=id, polygon=polygon, crsPolygon=crsPolygon, crs=crs, update=True
             )
         else:
             _warning_cached_data(file_name)
 
     data_all_clean["crsCoord"] = crs
-
+    
     return data_all_clean
```

### Comparing `pynsee-0.1.3/pynsee/geodata/_get_geom.py` & `pynsee-0.1.4/pynsee/geodata/_get_geom.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_make_offshore_points.py` & `pynsee-0.1.4/pynsee/geodata/_make_offshore_points.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/_rescale_geom.py` & `pynsee-0.1.4/pynsee/geodata/_rescale_geom.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/get_geodata.py` & `pynsee-0.1.4/pynsee/geodata/get_geodata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/get_geodata_list.py` & `pynsee-0.1.4/pynsee/geodata/get_geodata_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/get_geom.py` & `pynsee-0.1.4/pynsee/geodata/get_geom.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/translate.py` & `pynsee-0.1.4/pynsee/geodata/translate.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/geodata/zoom.py` & `pynsee-0.1.4/pynsee/geodata/zoom.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/__init__.py` & `pynsee-0.1.4/pynsee/localdata/__init__.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/_find_latest_local_dataset.py` & `pynsee-0.1.4/pynsee/localdata/_find_latest_local_dataset.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/_get_geo_list_simple.py` & `pynsee-0.1.4/pynsee/localdata/_get_geo_list_simple.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/_get_geo_relation.py` & `pynsee-0.1.4/pynsee/localdata/_get_geo_relation.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/_get_insee_local_onegeo.py` & `pynsee-0.1.4/pynsee/localdata/_get_insee_local_onegeo.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/_get_insee_one_area.py` & `pynsee-0.1.4/pynsee/localdata/_get_insee_one_area.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/data/local_metadata.zip` & `pynsee-0.1.4/pynsee/localdata/data/local_metadata.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_area_list.py` & `pynsee-0.1.4/pynsee/localdata/get_area_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_ascending_area.py` & `pynsee-0.1.4/pynsee/localdata/get_ascending_area.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_descending_area.py` & `pynsee-0.1.4/pynsee/localdata/get_descending_area.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_geo_list.py` & `pynsee-0.1.4/pynsee/localdata/get_geo_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_included_area.py` & `pynsee-0.1.4/pynsee/localdata/get_included_area.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_local_data.py` & `pynsee-0.1.4/pynsee/localdata/get_local_data.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_local_metadata.py` & `pynsee-0.1.4/pynsee/localdata/get_local_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_new_city.py` & `pynsee-0.1.4/pynsee/localdata/get_new_city.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_nivgeo_list.py` & `pynsee-0.1.4/pynsee/localdata/get_nivgeo_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/localdata/get_old_city.py` & `pynsee-0.1.4/pynsee/localdata/get_old_city.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/__init__.py` & `pynsee-0.1.4/pynsee/macrodata/__init__.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_add_numeric_metadata.py` & `pynsee-0.1.4/pynsee/macrodata/_add_numeric_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_build_series_list.py` & `pynsee-0.1.4/pynsee/macrodata/_build_series_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_download_idbank_list.py` & `pynsee-0.1.4/pynsee/macrodata/_download_idbank_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_dwn_idbank_files.py` & `pynsee-0.1.4/pynsee/macrodata/_dwn_idbank_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import tempfile
 import os
 import requests
 import zipfile
 import re
 import pandas as pd
 import urllib3
-
+from requests.adapters import HTTPAdapter
+from requests.packages.urllib3.util.retry import Retry
 
 def _dwn_idbank_files():
 
     # creating the date object of today's date
     todays_date = date.today()
 
     main_link_en = "https://www.insee.fr/en/statistiques/fichier/2868055/"
@@ -55,40 +56,47 @@
             pynsee_idbank_loop_url = os.environ["PYNSEE_IDBANK_LOOP_URL"]
             if (pynsee_idbank_loop_url == "False") or (
                 pynsee_idbank_loop_url == "FALSE"
             ):
                 pynsee_idbank_loop_url = False
         except:
             pass
+    
+    session = requests.Session()
+    retry = Retry(connect=3, backoff_factor=1, status_forcelist=[502])
+    adapter = HTTPAdapter(max_retries=retry)
+    session.mount("http://", adapter)
+    session.mount("https://", adapter)
 
     if pynsee_idbank_loop_url:
         while idbank_file_not_found & (i <= len(files) - 1):
             try:
-                data = _dwn_idbank_file(file_to_dwn=files[i])
+                data = _dwn_idbank_file(file_to_dwn=files[i], session=session)
             except:
                 # print(f'!!! File not found:\n{files[i]}')
                 idbank_file_not_found = True
             else:
                 idbank_file_not_found = False
             i += 1
 
     return data
 
 
-def _dwn_idbank_file(file_to_dwn):
+def _dwn_idbank_file(file_to_dwn, session):
 
     separator = ";"
 
     try:
         proxies = {"http": os.environ["http_proxy"], "https": os.environ["https_proxy"]}
     except:
         proxies = {"http": "", "https": ""}
 
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-    results = requests.get(file_to_dwn, proxies=proxies, verify=False)
+    
+    results = session.get(file_to_dwn, proxies=proxies, verify=False)
 
     dirpath = tempfile.mkdtemp()
 
     if not os.path.exists(dirpath):
         os.makedirs(dirpath)
 
     idbank_zip_file = dirpath + "\\idbank_list.zip"
```

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_dataset_dimension.py` & `pynsee-0.1.4/pynsee/macrodata/_get_dataset_dimension.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_dataset_list_internal.py` & `pynsee-0.1.4/pynsee/macrodata/_get_dataset_list_internal.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_dataset_metadata.py` & `pynsee-0.1.4/pynsee/macrodata/_get_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_dataset_metadata_core.py` & `pynsee-0.1.4/pynsee/macrodata/_get_dataset_metadata_core.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_date.py` & `pynsee-0.1.4/pynsee/macrodata/_get_date.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_dimension_values.py` & `pynsee-0.1.4/pynsee/macrodata/_get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_idbank_internal_data.py` & `pynsee-0.1.4/pynsee/macrodata/_get_idbank_internal_data.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_idbank_internal_data_harmonized.py` & `pynsee-0.1.4/pynsee/macrodata/_get_idbank_internal_data_harmonized.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/_get_insee.py` & `pynsee-0.1.4/pynsee/macrodata/_get_insee.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,31 +64,35 @@
             col = list(dict_obs.keys())
 
             df = pd.DataFrame(dict_obs, columns=col, index=[0])
 
             list_obs.append(df)
 
         if len(list_obs) > 0:
-            obs_series = pd.concat(list_obs)
+            obs_series = pd.concat(list_obs).reset_index(drop=True)
 
         #
         # collect attributes values from the series
         #
 
         attr_series = data._attrs
 
         dict_attr = {}
         for a in attr_series:
             dict_attr[a] = attr_series[a]._value
 
         col_attr = list(dict_attr.keys())
-        attr_series = pd.DataFrame(dict_attr, columns=col_attr, index=[0])
+        attr_series = pd.DataFrame(dict_attr, columns=col_attr, index=[0]).reset_index(drop=True)
 
         if len(list_obs) > 0:
-            data_series = pd.concat([obs_series, attr_series], axis=1)
+            data_series = obs_series
+            if len(dict_attr.keys()) > 0:
+                for k in dict_attr.keys():
+                    data_series[k] = dict_attr[k]
+            # data_series = pd.concat([obs_series, attr_series], axis=1)
         else:
             data_series = pd.concat([attr_series], axis=1)
 
         #
         # add date column
         #
```

### Comparing `pynsee-0.1.3/pynsee/macrodata/data/dataset_list_internal.zip` & `pynsee-0.1.4/pynsee/macrodata/data/dataset_list_internal.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/data/idbank_list_internal.zip` & `pynsee-0.1.4/pynsee/macrodata/data/idbank_list_internal.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_column_title.py` & `pynsee-0.1.4/pynsee/macrodata/get_column_title.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_dataset.py` & `pynsee-0.1.4/pynsee/macrodata/get_dataset.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_dataset_list.py` & `pynsee-0.1.4/pynsee/macrodata/get_dataset_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_last_release.py` & `pynsee-0.1.4/pynsee/macrodata/get_last_release.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_series.py` & `pynsee-0.1.4/pynsee/macrodata/get_series.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas
 import math
 
 from pynsee.macrodata._get_insee import _get_insee
 from pynsee.macrodata.get_series_list import get_series_list
 from pynsee.macrodata.search_macrodata import search_macrodata
 from pynsee.macrodata._add_numeric_metadata import _add_numeric_metadata
+from pynsee.macrodata._load_dataset_data import _load_dataset_data
 from pynsee.utils._paste import _paste
 
 
 def get_series(
     *idbanks,
     metadata=True,
     startPeriod=None,
@@ -126,44 +127,34 @@
             api_query=api_query,  # api_query
             sdmx_query=sdmx_query,
             step=str("{0}/{1}").format(q + 1, max_seq_idbank),
         )
 
         list_data.append(df)
 
-    data = pandas.concat(list_data)
+    data = pandas.concat(list_data).reset_index(drop=True)
 
     if metadata:
         try:
-            all_idbank = search_macrodata()
-            list_all_idbank = all_idbank.IDBANK.to_list()
+            metadata_df = _load_dataset_data()
 
-            list_data_idbank = data.IDBANK.unique()
-            idbank_available_bool = [
-                (idb in list_all_idbank) for idb in list_data_idbank
-            ]
-
-            if any(idbank_available_bool):
-
-                idbank_available = list_data_idbank[idbank_available_bool]
-                list_dataset = all_idbank[all_idbank.IDBANK.isin(idbank_available)]
-                list_dataset = list(list_dataset.DATASET.unique())
-
-                idbank_list = get_series_list(list_dataset)
-                newcol = [
-                    col for col in idbank_list.columns if col not in data.columns
-                ] + ["IDBANK"]
-                idbank_list = idbank_list[newcol]
+            if metadata_df is not None:
+                
+                metadata_df = metadata_df.rename(columns={'idbank' : 'IDBANK'})
+                
+                list_idbank_data = list(data.IDBANK.unique())
+                metadata_df = metadata_df[metadata_df['IDBANK'].isin(list_idbank_data)].reset_index(drop=True)
 
-                data = data.merge(idbank_list, on="IDBANK", how="left")
+                data = data.merge(metadata_df, on="IDBANK", how="left")
 
                 # remove all na columns
                 data = data.dropna(axis=1, how="all")
-        except:
+        except Exception as e:
+            #print(e)
             pass
 
-        try:
+        try:            
             data = _add_numeric_metadata(data)
         except:
             pass
 
     return data
```

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_series_list.py` & `pynsee-0.1.4/pynsee/macrodata/get_series_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/get_series_title.py` & `pynsee-0.1.4/pynsee/macrodata/get_series_title.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/macrodata/search_macrodata.py` & `pynsee-0.1.4/pynsee/macrodata/search_macrodata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/_add_A17_activity.py` & `pynsee-0.1.4/pynsee/metadata/_add_A17_activity.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/_add_A5_activity.py` & `pynsee-0.1.4/pynsee/metadata/_add_A5_activity.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/_get_naf.py` & `pynsee-0.1.4/pynsee/metadata/_get_naf.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/_get_nomenclature_agreg.py` & `pynsee-0.1.4/pynsee/metadata/_get_nomenclature_agreg.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/data/definition.zip` & `pynsee-0.1.4/pynsee/metadata/data/definition.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/data/naf.zip` & `pynsee-0.1.4/pynsee/metadata/data/naf.zip`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/get_activity_list.py` & `pynsee-0.1.4/pynsee/metadata/get_activity_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/get_definition.py` & `pynsee-0.1.4/pynsee/metadata/get_definition.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/get_definition_list.py` & `pynsee-0.1.4/pynsee/metadata/get_definition_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/get_legal_entity.py` & `pynsee-0.1.4/pynsee/metadata/get_legal_entity.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/metadata/get_operation.py` & `pynsee-0.1.4/pynsee/metadata/get_operation.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_clean_data.py` & `pynsee-0.1.4/pynsee/sirene/_clean_data.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_employee_metadata.py` & `pynsee-0.1.4/pynsee/sirene/_employee_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_get_location_openstreetmap.py` & `pynsee-0.1.4/pynsee/sirene/_get_location_openstreetmap.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_make_dataframe.py` & `pynsee-0.1.4/pynsee/sirene/_make_dataframe.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_request_sirene.py` & `pynsee-0.1.4/pynsee/sirene/_request_sirene.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/_street_metadata.py` & `pynsee-0.1.4/pynsee/sirene/_street_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/get_dimension_list.py` & `pynsee-0.1.4/pynsee/sirene/get_dimension_list.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/get_location.py` & `pynsee-0.1.4/pynsee/sirene/get_location.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/get_sirene_data.py` & `pynsee-0.1.4/pynsee/sirene/get_sirene_data.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/get_sirene_relatives.py` & `pynsee-0.1.4/pynsee/sirene/get_sirene_relatives.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/sirene/search_sirene.py` & `pynsee-0.1.4/pynsee/sirene/search_sirene.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_clean_insee_folder.py` & `pynsee-0.1.4/pynsee/utils/_clean_insee_folder.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_create_insee_folder.py` & `pynsee-0.1.4/pynsee/utils/_create_insee_folder.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_get_credentials.py` & `pynsee-0.1.4/pynsee/utils/_get_credentials.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_get_envir_token.py` & `pynsee-0.1.4/pynsee/utils/_get_envir_token.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_get_token.py` & `pynsee-0.1.4/pynsee/utils/_get_token.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_get_token_from_insee.py` & `pynsee-0.1.4/pynsee/utils/_get_token_from_insee.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_make_dataframe_from_dict.py` & `pynsee-0.1.4/pynsee/utils/_make_dataframe_from_dict.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_move_col_after.py` & `pynsee-0.1.4/pynsee/utils/_move_col_after.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/_request_insee.py` & `pynsee-0.1.4/pynsee/utils/_request_insee.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright : INSEE, 2021
 
 import os
 import requests
 import urllib3
+import time
 
 from pynsee.utils._get_token import _get_token
 from pynsee.utils._get_credentials import _get_credentials
 from pynsee.utils._wait_api_query_limit import _wait_api_query_limit
 
 CODES = {
     # 200:"Opération réussie",
@@ -86,16 +87,26 @@
             
             results = requests.get(api_url, proxies=proxies, headers=headers, verify=False)
 
             success = True
 
             code = results.status_code
             
-            if "status_code" not in dir(results):
+            if "status_code" not in dir(results):            
                 success = False
+            elif code == 429:
+                
+                time.sleep(10)
+
+                request_again = _request_insee(api_url=api_url, 
+                sdmx_url=sdmx_url, file_format=file_format,
+                print_msg=print_msg)
+
+                return request_again
+
             elif code in CODES:
                 msg = f"Error {code} - {CODES[code]}\nQuery:\n{api_url}"
                 raise requests.exceptions.RequestException(msg)
             elif code != 200:
                 success = False
 
             if success is True:
```

### Comparing `pynsee-0.1.3/pynsee/utils/_wait_api_query_limit.py` & `pynsee-0.1.4/pynsee/utils/_wait_api_query_limit.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @lru_cache(maxsize=None)
 def _warning_query_limit():
     print("\nAPI query number limit reached - function might be slowed down")
 
 
 def _wait_api_query_limit(query):
 
-    max_query_insee_api = 30
+    max_query_insee_api = 29
     timespan_insee_api = 60
 
     insee_folder = _create_insee_folder()
 
     file = insee_folder + "/" + _hash("queries_count")
 
     date_time_now = datetime.now()
```

### Comparing `pynsee-0.1.3/pynsee/utils/clear_all_cache.py` & `pynsee-0.1.4/pynsee/utils/clear_all_cache.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee/utils/init_conn.py` & `pynsee-0.1.4/pynsee/utils/init_conn.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/pynsee.egg-info/PKG-INFO` & `pynsee-0.1.4/pynsee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynsee
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools to Easily Search and Download French Data From INSEE and IGN APIs
 Home-page: https://pynsee.readthedocs.io/en/latest/
 Author: Hadrien Leclerc, Lino Galiana
 Author-email: leclerc.hadrien@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/InseeFrLab/pynsee/issues
 Description: .. role:: raw-html-m2r(raw)
```

### Comparing `pynsee-0.1.3/pynsee.egg-info/SOURCES.txt` & `pynsee-0.1.4/pynsee.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 pynsee/download/data/liste_donnees.zip
 pynsee/geodata/GeoFrDataFrame.py
 pynsee/geodata/__init__.py
 pynsee/geodata/_add_insee_dep.py
 pynsee/geodata/_convert_polygon.py
 pynsee/geodata/_distance.py
 pynsee/geodata/_extract_bounds.py
+pynsee/geodata/_find_wfs_closest_match.py
 pynsee/geodata/_geojson_parser.py
 pynsee/geodata/_get_bbox_list.py
 pynsee/geodata/_get_bbox_list_full.py
 pynsee/geodata/_get_capabilities.py
 pynsee/geodata/_get_center.py
 pynsee/geodata/_get_data_with_bbox.py
 pynsee/geodata/_get_full_list_wfs.py
 pynsee/geodata/_get_geodata.py
+pynsee/geodata/_get_geodata_with_backup.py
 pynsee/geodata/_get_geom.py
 pynsee/geodata/_make_offshore_points.py
 pynsee/geodata/_rescale_geom.py
 pynsee/geodata/get_geodata.py
 pynsee/geodata/get_geodata_list.py
 pynsee/geodata/get_geom.py
 pynsee/geodata/translate.py
@@ -75,14 +77,15 @@
 pynsee/macrodata/_get_dataset_metadata.py
 pynsee/macrodata/_get_dataset_metadata_core.py
 pynsee/macrodata/_get_date.py
 pynsee/macrodata/_get_dimension_values.py
 pynsee/macrodata/_get_idbank_internal_data.py
 pynsee/macrodata/_get_idbank_internal_data_harmonized.py
 pynsee/macrodata/_get_insee.py
+pynsee/macrodata/_load_dataset_data.py
 pynsee/macrodata/get_column_title.py
 pynsee/macrodata/get_dataset.py
 pynsee/macrodata/get_dataset_list.py
 pynsee/macrodata/get_last_release.py
 pynsee/macrodata/get_series.py
 pynsee/macrodata/get_series_list.py
 pynsee/macrodata/get_series_title.py
```

### Comparing `pynsee-0.1.3/setup.py` & `pynsee-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynsee",
-    version="0.1.3",
+    version="0.1.4",
     author="Hadrien Leclerc, Lino Galiana",
     author_email="leclerc.hadrien@gmail.com",
     description="Tools to Easily Search and Download French Data From INSEE and IGN APIs",
     long_description=long_description,
     url="https://pynsee.readthedocs.io/en/latest/",
     project_urls={
         'Bug Tracker': 'https://github.com/InseeFrLab/pynsee/issues'
@@ -31,15 +31,15 @@
     license_files=('LICENSE.md',),
     install_requires=[
             "pandas>=0.24.2",
             "tqdm>=4.56.0",
             "requests>=2.23",
             "appdirs>=1.4.4",
             "unidecode>=1.1.0",
-            "shapely>=1.8.0,<2.0",
+            "shapely>=2.0.0",
             "urllib3"],
     extras_require={
         'full': ['openpyxl<=3.1.0', "xlrd>=2.0.1"]
     },
     package_data={
         "": ["*.zip"]},
     python_requires='>=3.7',
```

### Comparing `pynsee-0.1.3/tests/download/test_pynsee_download.py` & `pynsee-0.1.4/tests/download/test_pynsee_download.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/tests/geodata/test_pynsee_geodata.py` & `pynsee-0.1.4/tests/geodata/test_pynsee_geodata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # -*- coding: utf-8 -*-
 # Copyright : INSEE, 2022
 
 from unittest import TestCase
 import pandas as pd
 import sys
 import requests
+import unittest
 
 from shapely.geometry import Polygon, MultiPolygon, MultiLineString, MultiPoint, Point
 
 from pynsee.geodata.get_geodata_list import get_geodata_list
 from pynsee.geodata.get_geodata import get_geodata
 from pynsee.geodata._get_geodata import _get_geodata
 from pynsee.geodata._get_bbox_list import _get_bbox_list
 from pynsee.geodata.GeoFrDataFrame import GeoFrDataFrame
 from pynsee.geodata._get_data_with_bbox import _get_data_with_bbox, _set_global_var
+from pynsee.geodata._get_geodata_with_backup import _get_geodata_with_backup
 
 # manual commands for testing only on geodata module
 # coverage run -m unittest tests/geodata/test_pynsee_geodata.py
 # coverage report --omit=*/utils/*,*/macrodata/*,*/localdata/*,*/download/*,*/sirene/*,*/metadata/* -m
 
 class TestFunction(TestCase):
 
     version_3_7 = (sys.version_info[0] == 3) & (sys.version_info[1] == 7)
 
     if version_3_7 is False:
+        
+        def test_get_geodata_with_backup(self):
+            df = _get_geodata_with_backup("ADMINEXPRESS-COG.LATEST:departement")
+            self.assertTrue(isinstance(df, pd.DataFrame))  
+            
         def test_get_geodata_short(self):
             
             global session
             session = requests.Session()
             list_bbox = (-2, 43.0, 6.0, 44.5)
             for crs in ["EPSG:4326"]:
                 link= f"https://wxs.ign.fr/administratif/geoportail/wfs?SERVICE=WFS&VERSION=2.0.0&REQUEST=GetFeature&TYPENAME=ADMINEXPRESS-COG-CARTO.LATEST:commune&srsName={crs}&OUTPUTFORMAT=application/json&COUNT=1000"
@@ -116,41 +123,10 @@
                
             bbox = _get_bbox_list(polygon=geo13, update=True, crsPolygon="EPSG:3857")
             self.assertTrue(isinstance(bbox, list))
             
             data = get_geodata(id='test', update=True) 
             self.assertTrue(isinstance(data, pd.DataFrame))
             
-    if False:
-
-        def test_get_geodata_all(self):
-            df = get_geodata_list(update=True)
-            ids = df.Identifier.to_list()
-
-            list_geom_type = []
-            # ident = 'LIMITES_ADMINISTRATIVES_EXPRESS.LATEST:epci'
-            # ident = 'ADMINEXPRESS-COG-CARTO.LATEST:commune'
-
-            data = get_geodata(id='ADMINEXPRESS-COG-CARTO.LATEST:commune', update=True) 
-            list_geom_type += [type(data.get_geom())]
-
-            dep29 = get_geodata(id='ADMINEXPRESS-COG-CARTO.LATEST:departement', update=True)
-            dep29 = dep29[dep29["insee_dep"] == "29"]
-            geodep29 = dep29.get_geom()   
-            list_geom_type += [type(geodep29)]         
-        
-            for id in range(len(ids)):
-                
-                ident = ids[id]
-                print("%s %s" % (id, ident))
-
-                data = get_geodata(id=ident, update=True, polygon=geodep29)
-
-                if type(data) == GeoFrDataFrame:    
-                    geom = data.get_geom()
-                    list_geom_type += [type(geom)]
-
-            print(list_geom_type)            
-            
-            test = all([typegeo in [Polygon, MultiPolygon, MultiLineString, MultiPoint] for typegeo in list_geom_type])
-
-            self.assertTrue(test)
+if __name__ == '__main__':
+    unittest.main()
+    #python test_pynsee_geodata.py
```

### Comparing `pynsee-0.1.3/tests/localdata/test_pynsee_localdata.py` & `pynsee-0.1.4/tests/localdata/test_pynsee_localdata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/tests/macrodata/test_pynsee_macrodata.py` & `pynsee-0.1.4/tests/macrodata/test_pynsee_macrodata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright : INSEE, 2021
 
+import unittest
 from unittest import TestCase
 from pandas import pandas as pd
 import os
 import sys
 from datetime import datetime
 from datetime import timedelta
 
@@ -239,7 +240,15 @@
                 self.assertTrue(isinstance(data, pd.DataFrame))
 
             # def test_build_series_list(self):
             #     df = _build_series_list()
             #     test = isinstance(df, pd.DataFrame)
             #     os.environ['pynsee_use_sdmx'] = "False"
             #     self.assertTrue(test)
+
+
+if __name__ == '__main__':
+    unittest.main()
+    #python test_pynsee_macrodata.py TestFunction.test_get_series_2
+    #python test_pynsee_macrodata.py TestFunction.test_get_column_title_1
+
+
```

### Comparing `pynsee-0.1.3/tests/metadata/test_pynsee_metadata.py` & `pynsee-0.1.4/tests/metadata/test_pynsee_metadata.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/tests/sirene/test_pynsee_sirene.py` & `pynsee-0.1.4/tests/sirene/test_pynsee_sirene.py`

 * *Files identical despite different names*

### Comparing `pynsee-0.1.3/tests/utils/test_pynsee_utils.py` & `pynsee-0.1.4/tests/utils/test_pynsee_utils.py`

 * *Files identical despite different names*

