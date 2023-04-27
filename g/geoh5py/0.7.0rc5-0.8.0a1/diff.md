# Comparing `tmp/geoh5py-0.7.0rc5.tar.gz` & `tmp/geoh5py-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.7.0rc5.tar", max compression
+gzip compressed data, was "geoh5py-0.8.0a1.tar", max compression
```

## Comparing `geoh5py-0.7.0rc5.tar` & `geoh5py-0.8.0a1.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0      838 2023-04-04 17:51:20.059464 geoh5py-0.7.0rc5/geoh5py/__init__.py
--rw-r--r--   0        0        0     1486 2023-01-27 16:07:08.404026 geoh5py-0.7.0rc5/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.405036 geoh5py-0.7.0rc5/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     3948 2023-03-27 18:34:50.646957 geoh5py-0.7.0rc5/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8158 2023-04-04 17:51:20.060566 geoh5py-0.7.0rc5/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.407026 geoh5py-0.7.0rc5/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0     9612 2023-03-16 20:09:06.192137 geoh5py-0.7.0rc5/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.408028 geoh5py-0.7.0rc5/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2023-02-09 14:27:13.492642 geoh5py-0.7.0rc5/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3698 2023-03-16 20:09:06.192137 geoh5py-0.7.0rc5/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1218 2023-01-27 16:07:08.410027 geoh5py-0.7.0rc5/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2023-01-27 16:07:08.411061 geoh5py-0.7.0rc5/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     2415 2023-01-27 16:07:08.412062 geoh5py-0.7.0rc5/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     3322 2023-04-04 17:51:20.062749 geoh5py-0.7.0rc5/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1103 2023-01-27 16:07:08.413026 geoh5py-0.7.0rc5/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     1649 2023-01-27 16:07:08.413026 geoh5py-0.7.0rc5/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2023-01-27 16:07:08.414026 geoh5py-0.7.0rc5/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     4445 2023-03-16 20:09:06.193137 geoh5py-0.7.0rc5/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1571 2023-01-27 16:07:08.415027 geoh5py-0.7.0rc5/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     1587 2023-01-27 16:07:08.416026 geoh5py-0.7.0rc5/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1495 2023-01-27 16:07:08.416026 geoh5py-0.7.0rc5/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1449 2023-01-27 16:07:08.416026 geoh5py-0.7.0rc5/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1851 2023-03-16 20:09:06.194139 geoh5py-0.7.0rc5/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1498 2023-01-27 16:07:08.417027 geoh5py-0.7.0rc5/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     6311 2023-03-27 18:34:50.648948 geoh5py-0.7.0rc5/geoh5py/groups/group.py
--rw-r--r--   0        0        0     3698 2023-01-27 16:07:08.418027 geoh5py-0.7.0rc5/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     7324 2023-01-27 16:07:08.419027 geoh5py-0.7.0rc5/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.420026 geoh5py-0.7.0rc5/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1468 2023-01-27 16:07:08.420026 geoh5py-0.7.0rc5/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     4449 2023-03-16 20:09:06.195138 geoh5py-0.7.0rc5/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2023-01-27 16:07:08.421026 geoh5py-0.7.0rc5/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2129 2023-01-27 16:07:08.422027 geoh5py-0.7.0rc5/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1338 2023-01-27 16:07:08.422027 geoh5py-0.7.0rc5/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2023-01-27 16:07:08.429046 geoh5py-0.7.0rc5/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17088 2023-03-16 20:09:06.195138 geoh5py-0.7.0rc5/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    32420 2023-03-16 20:09:06.196136 geoh5py-0.7.0rc5/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     1837 2023-01-27 16:07:08.431025 geoh5py-0.7.0rc5/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9496 2023-03-16 20:09:06.197153 geoh5py-0.7.0rc5/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7803 2023-03-27 18:34:50.649448 geoh5py-0.7.0rc5/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6283 2023-03-16 20:09:06.198164 geoh5py-0.7.0rc5/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     5129 2023-03-16 20:09:06.198164 geoh5py-0.7.0rc5/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    25527 2023-03-27 18:34:50.650448 geoh5py-0.7.0rc5/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    16653 2023-03-27 18:34:50.650948 geoh5py-0.7.0rc5/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    13506 2023-03-27 18:34:50.651448 geoh5py-0.7.0rc5/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4775 2023-03-27 18:34:50.651948 geoh5py-0.7.0rc5/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1919 2023-03-16 20:09:06.201539 geoh5py-0.7.0rc5/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2977 2023-03-27 18:34:50.652448 geoh5py-0.7.0rc5/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2890 2023-03-27 18:34:50.652948 geoh5py-0.7.0rc5/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    17763 2023-03-27 18:34:50.653448 geoh5py-0.7.0rc5/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     2748 2023-01-27 16:07:08.438024 geoh5py-0.7.0rc5/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13349 2023-03-16 20:09:06.203794 geoh5py-0.7.0rc5/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5410 2023-03-27 18:34:50.653948 geoh5py-0.7.0rc5/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2023-03-16 20:09:06.204796 geoh5py-0.7.0rc5/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2023-01-27 16:07:08.440024 geoh5py-0.7.0rc5/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14570 2023-03-16 20:09:06.205794 geoh5py-0.7.0rc5/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2023-01-27 16:07:08.441024 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     9754 2023-03-16 20:09:06.206794 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    19395 2023-03-16 20:09:06.207373 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0    11028 2023-03-16 20:09:06.207373 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2832 2023-03-16 20:09:06.208379 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     8585 2023-03-27 18:34:50.654448 geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2023-01-27 16:07:08.443024 geoh5py-0.7.0rc5/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2023-03-27 18:34:50.654950 geoh5py-0.7.0rc5/geoh5py/py.typed
--rw-r--r--   0        0        0     1015 2023-01-27 16:07:08.444702 geoh5py-0.7.0rc5/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0    37812 2023-03-27 18:34:50.655448 geoh5py-0.7.0rc5/geoh5py/shared/concatenation.py
--rw-r--r--   0        0        0      937 2023-01-27 16:07:08.446085 geoh5py-0.7.0rc5/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4287 2023-01-27 16:07:08.446085 geoh5py-0.7.0rc5/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     7599 2023-01-27 16:07:08.446085 geoh5py-0.7.0rc5/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0     8083 2023-03-16 20:09:06.209634 geoh5py-0.7.0rc5/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    16876 2023-03-27 18:34:50.656448 geoh5py-0.7.0rc5/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     4275 2023-03-16 20:09:06.210634 geoh5py-0.7.0rc5/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     5732 2023-03-16 20:09:06.211635 geoh5py-0.7.0rc5/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0    14944 2023-03-27 18:34:50.656948 geoh5py-0.7.0rc5/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8483 2023-03-16 20:09:06.212634 geoh5py-0.7.0rc5/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2023-01-27 16:07:08.451084 geoh5py-0.7.0rc5/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      921 2023-01-27 16:07:08.452070 geoh5py-0.7.0rc5/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2936 2023-01-27 16:07:08.452070 geoh5py-0.7.0rc5/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0    15041 2023-03-16 20:09:06.212634 geoh5py-0.7.0rc5/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0    10307 2023-01-27 16:07:08.453070 geoh5py-0.7.0rc5/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0    10932 2023-03-16 20:09:06.213634 geoh5py-0.7.0rc5/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    11036 2023-03-16 20:09:06.214634 geoh5py-0.7.0rc5/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2023-01-27 16:07:08.455078 geoh5py-0.7.0rc5/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    42651 2023-03-28 12:54:18.623649 geoh5py-0.7.0rc5/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2023-01-27 16:07:08.456070 geoh5py-0.7.0rc5/package.rst
--rw-r--r--   0        0        0     2497 2023-04-04 17:53:56.647216 geoh5py-0.7.0rc5/pyproject.toml
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 geoh5py-0.7.0rc5/PKG-INFO
+-rw-r--r--   0        0        0      841 2023-04-27 16:38:56.715801 geoh5py-0.8.0a1/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1486 2023-01-27 16:07:08.404026 geoh5py-0.8.0a1/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.405036 geoh5py-0.8.0a1/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     3948 2023-03-27 18:34:50.646957 geoh5py-0.8.0a1/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8158 2023-04-04 17:51:20.060566 geoh5py-0.8.0a1/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.407026 geoh5py-0.8.0a1/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0     9612 2023-03-16 20:09:06.192137 geoh5py-0.8.0a1/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.408028 geoh5py-0.8.0a1/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2023-02-09 14:27:13.492642 geoh5py-0.8.0a1/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3698 2023-03-16 20:09:06.192137 geoh5py-0.8.0a1/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1218 2023-01-27 16:07:08.410027 geoh5py-0.8.0a1/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2023-01-27 16:07:08.411061 geoh5py-0.8.0a1/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     2415 2023-01-27 16:07:08.412062 geoh5py-0.8.0a1/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     3473 2023-04-27 16:38:56.716801 geoh5py-0.8.0a1/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1103 2023-01-27 16:07:08.413026 geoh5py-0.8.0a1/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     1649 2023-01-27 16:07:08.413026 geoh5py-0.8.0a1/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2023-01-27 16:07:08.414026 geoh5py-0.8.0a1/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     4445 2023-03-16 20:09:06.193137 geoh5py-0.8.0a1/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1571 2023-01-27 16:07:08.415027 geoh5py-0.8.0a1/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     1587 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1495 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1449 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1851 2023-03-16 20:09:06.194139 geoh5py-0.8.0a1/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1498 2023-01-27 16:07:08.417027 geoh5py-0.8.0a1/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     6311 2023-03-27 18:34:50.648948 geoh5py-0.8.0a1/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     3698 2023-01-27 16:07:08.418027 geoh5py-0.8.0a1/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     7324 2023-01-27 16:07:08.419027 geoh5py-0.8.0a1/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.420026 geoh5py-0.8.0a1/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1468 2023-01-27 16:07:08.420026 geoh5py-0.8.0a1/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     4449 2023-03-16 20:09:06.195138 geoh5py-0.8.0a1/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2023-01-27 16:07:08.421026 geoh5py-0.8.0a1/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2107 2023-04-27 16:38:56.717802 geoh5py-0.8.0a1/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1338 2023-01-27 16:07:08.422027 geoh5py-0.8.0a1/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2023-01-27 16:07:08.429046 geoh5py-0.8.0a1/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17088 2023-03-16 20:09:06.195138 geoh5py-0.8.0a1/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    32435 2023-04-27 16:38:56.717802 geoh5py-0.8.0a1/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2223 2023-04-27 16:38:56.718801 geoh5py-0.8.0a1/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9496 2023-03-16 20:09:06.197153 geoh5py-0.8.0a1/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7803 2023-03-27 18:34:50.649448 geoh5py-0.8.0a1/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6283 2023-03-16 20:09:06.198164 geoh5py-0.8.0a1/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     5129 2023-03-16 20:09:06.198164 geoh5py-0.8.0a1/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    25527 2023-03-27 18:34:50.650448 geoh5py-0.8.0a1/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    16653 2023-03-27 18:34:50.650948 geoh5py-0.8.0a1/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    13506 2023-03-27 18:34:50.651448 geoh5py-0.8.0a1/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4775 2023-03-27 18:34:50.651948 geoh5py-0.8.0a1/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1919 2023-03-16 20:09:06.201539 geoh5py-0.8.0a1/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2977 2023-03-27 18:34:50.652448 geoh5py-0.8.0a1/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2890 2023-03-27 18:34:50.652948 geoh5py-0.8.0a1/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    17763 2023-03-27 18:34:50.653448 geoh5py-0.8.0a1/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     2748 2023-01-27 16:07:08.438024 geoh5py-0.8.0a1/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13349 2023-03-16 20:09:06.203794 geoh5py-0.8.0a1/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5410 2023-03-27 18:34:50.653948 geoh5py-0.8.0a1/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2023-03-16 20:09:06.204796 geoh5py-0.8.0a1/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2023-01-27 16:07:08.440024 geoh5py-0.8.0a1/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14570 2023-03-16 20:09:06.205794 geoh5py-0.8.0a1/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2023-01-27 16:07:08.441024 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2023-04-27 16:38:56.718801 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2023-04-27 16:38:56.719810 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    35608 2023-04-27 16:38:56.719810 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2023-04-27 16:38:56.720802 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     7019 2023-04-27 16:38:56.720802 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2023-04-27 16:38:56.721800 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6636 2023-04-27 16:38:56.722800 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2023-01-27 16:07:08.443024 geoh5py-0.8.0a1/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2023-03-27 18:34:50.654950 geoh5py-0.8.0a1/geoh5py/py.typed
+-rw-r--r--   0        0        0     1015 2023-01-27 16:07:08.444702 geoh5py-0.8.0a1/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0    37812 2023-03-27 18:34:50.655448 geoh5py-0.8.0a1/geoh5py/shared/concatenation.py
+-rw-r--r--   0        0        0      937 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4287 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     7599 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0     8083 2023-03-16 20:09:06.209634 geoh5py-0.8.0a1/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    16876 2023-03-27 18:34:50.656448 geoh5py-0.8.0a1/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     4275 2023-03-16 20:09:06.210634 geoh5py-0.8.0a1/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     5732 2023-03-16 20:09:06.211635 geoh5py-0.8.0a1/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0    15205 2023-04-27 16:38:56.722800 geoh5py-0.8.0a1/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8969 2023-04-27 16:38:56.723802 geoh5py-0.8.0a1/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2023-01-27 16:07:08.451084 geoh5py-0.8.0a1/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      921 2023-01-27 16:07:08.452070 geoh5py-0.8.0a1/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2936 2023-01-27 16:07:08.452070 geoh5py-0.8.0a1/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0    18349 2023-04-27 16:38:56.723802 geoh5py-0.8.0a1/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0    11946 2023-04-27 16:38:56.724800 geoh5py-0.8.0a1/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0    10990 2023-04-27 16:38:56.724800 geoh5py-0.8.0a1/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    10777 2023-04-27 16:38:56.725800 geoh5py-0.8.0a1/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2023-01-27 16:07:08.455078 geoh5py-0.8.0a1/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    42630 2023-04-27 16:38:56.726801 geoh5py-0.8.0a1/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2023-01-27 16:07:08.456070 geoh5py-0.8.0a1/package.rst
+-rw-r--r--   0        0        0     2500 2023-04-27 16:51:35.348107 geoh5py-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 geoh5py-0.8.0a1/PKG-INFO
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/__init__.py` & `geoh5py-0.8.0a1/geoh5py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.7.0-rc.5"
+__version__ = "0.8.0-alpha.1"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/__init__.py` & `geoh5py-0.8.0a1/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/blob_data.py` & `geoh5py-0.8.0a1/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/color_map.py` & `geoh5py-0.8.0a1/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/data.py` & `geoh5py-0.8.0a1/geoh5py/data/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/data_association_enum.py` & `geoh5py-0.8.0a1/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/data_type.py` & `geoh5py-0.8.0a1/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/data_unit.py` & `geoh5py-0.8.0a1/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/datetime_data.py` & `geoh5py-0.8.0a1/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/filename_data.py` & `geoh5py-0.8.0a1/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/float_data.py` & `geoh5py-0.8.0a1/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.8.0a1/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/integer_data.py` & `geoh5py-0.8.0a1/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/numeric_data.py` & `geoh5py-0.8.0a1/geoh5py/data/numeric_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from warnings import warn
 
 import numpy as np
 
 from .data import Data, PrimitiveTypeEnum
 from .data_association_enum import DataAssociationEnum
 
 
@@ -79,19 +80,23 @@
 
         :returns: values: An array of float values of length n_values or None
         """
         if self.n_values is not None:
             if values is None:
                 return values
 
+            if values.ndim > 1:
+                values = np.ravel(values)
+                warn("Input 'values' converted to a 1D array.")
+
             if len(values) < self.n_values:
                 full_vector = np.ones(self.n_values, dtype=type(self.ndv))
                 full_vector *= np.nan if isinstance(self.ndv, float) else self.ndv
                 full_vector[: len(np.ravel(values))] = np.ravel(values)
                 return full_vector
 
-            if len(values) > self.n_values or values.ndim > 1:
+            if len(values) > self.n_values:
                 raise ValueError(
                     f"Input 'values' of shape({self.n_values},) expected. "
                     f"Array of shape{values.shape} provided.)"
                 )
         return values
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.8.0a1/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/reference_value_map.py` & `geoh5py-0.8.0a1/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/referenced_data.py` & `geoh5py-0.8.0a1/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/text_data.py` & `geoh5py-0.8.0a1/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/data/unknown_data.py` & `geoh5py-0.8.0a1/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/__init__.py` & `geoh5py-0.8.0a1/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/container_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/custom_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/drillhole_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/giftools_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/group.py` & `geoh5py-0.8.0a1/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/group_type.py` & `geoh5py-0.8.0a1/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/integrator_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/maps_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/notype_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/property_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/root_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/simpeg_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/simpeg_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,12 @@
         if self._options is None:
             self._options = {}
 
         return self._options
 
     @options.setter
     def options(self, value: dict | None):
-        if value is not None:
-            assert isinstance(
-                value, dict
-            ), f"Input 'options' must be of type {dict} or None"
+        if not isinstance(value, (dict, type(None))):
+            raise ValueError(f"Input 'options' must be of type {dict} or None")
 
         self._options = value
         self.workspace.update_attribute(self, "options")
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/groups/survey_group.py` & `geoh5py-0.8.0a1/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/io/__init__.py` & `geoh5py-0.8.0a1/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/io/h5_reader.py` & `geoh5py-0.8.0a1/geoh5py/io/h5_reader.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/io/h5_writer.py` & `geoh5py-0.8.0a1/geoh5py/io/h5_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,25 +261,27 @@
             except KeyError:
                 pass
 
             dict_values = getattr(entity, attribute)
 
             if channel in dict_values:
                 values = dict_values[channel]
-                if isinstance(values, np.ndarray) and values.dtype == np.float64:
+                if isinstance(values, np.ndarray) and values.dtype in (
+                    np.float64,
+                    np.float32,
+                ):
                     values[np.isnan(values)] = FLOAT_NDV
                     values = values.astype(np.float32)
 
-                if len(values) > 0:
-                    attr_handle.create_dataset(
-                        name,
-                        data=values,
-                        compression="gzip",
-                        compression_opts=9,
-                    )
+                attr_handle.create_dataset(
+                    name,
+                    data=values,
+                    compression="gzip",
+                    compression_opts=9,
+                )
 
     @classmethod
     def update_field(
         cls, file: str | h5py.File, entity, attribute: str, **kwargs
     ) -> None:
         """
         Update the attributes of an :obj:`~geoh5py.shared.entity.Entity`.
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/__init__.py` & `geoh5py-0.8.0a1/geoh5py/objects/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,30 @@
 from .notype_object import NoTypeObject
 from .object_base import ObjectBase
 from .object_type import ObjectType
 from .octree import Octree
 from .points import Points
 from .surface import Surface
 from .surveys.direct_current import CurrentElectrode, PotentialElectrode
+from .surveys.electromagnetics.airborne_fem import (
+    AirborneFEMReceivers,
+    AirborneFEMTransmitters,
+)
 from .surveys.electromagnetics.airborne_tem import (
     AirborneTEMReceivers,
     AirborneTEMTransmitters,
 )
+from .surveys.electromagnetics.ground_fem import (
+    LargeLoopGroundFEMReceivers,
+    LargeLoopGroundFEMTransmitters,
+    MovingLoopGroundFEMReceivers,
+    MovingLoopGroundFEMTransmitters,
+)
 from .surveys.electromagnetics.ground_tem import (
-    GroundTEMReceiversLargeLoop,
-    GroundTEMTransmittersLargeLoop,
+    LargeLoopGroundTEMReceivers,
+    LargeLoopGroundTEMTransmitters,
+    MovingLoopGroundTEMReceivers,
+    MovingLoopGroundTEMTransmitters,
 )
 from .surveys.electromagnetics.magnetotellurics import MTReceivers
 from .surveys.electromagnetics.tipper import TipperBaseStations, TipperReceivers
 from .surveys.magnetics import AirborneMagnetics
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/block_model.py` & `geoh5py-0.8.0a1/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/cell_object.py` & `geoh5py-0.8.0a1/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/curve.py` & `geoh5py-0.8.0a1/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/drape_model.py` & `geoh5py-0.8.0a1/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/drillhole.py` & `geoh5py-0.8.0a1/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/geo_image.py` & `geoh5py-0.8.0a1/geoh5py/objects/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/grid2d.py` & `geoh5py-0.8.0a1/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/grid_object.py` & `geoh5py-0.8.0a1/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/integrator.py` & `geoh5py-0.8.0a1/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/label.py` & `geoh5py-0.8.0a1/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/notype_object.py` & `geoh5py-0.8.0a1/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/object_base.py` & `geoh5py-0.8.0a1/geoh5py/objects/object_base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/object_type.py` & `geoh5py-0.8.0a1/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/octree.py` & `geoh5py-0.8.0a1/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/points.py` & `geoh5py-0.8.0a1/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surface.py` & `geoh5py-0.8.0a1/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,30 +18,24 @@
 from __future__ import annotations
 
 import uuid
 
 from geoh5py.objects.object_base import ObjectType
 from geoh5py.objects.points import Points
 
-from .base import BaseEMSurvey
+from .base import FEMSurvey
 
 
-class MTReceivers(BaseEMSurvey, Points):
+class MTReceivers(FEMSurvey, Points):
     """
     A magnetotellurics survey object.
     """
 
     __TYPE_UID = uuid.UUID("{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}")
     __TYPE = "Receivers"
-    __UNITS = [
-        "Hertz (Hz)",
-        "KiloHertz (kHz)",
-        "MegaHertz (MHz)",
-        "Gigahertz (GHz)",
-    ]
     __INPUT_TYPE = ["Rx only"]
 
     def __init__(self, object_type: ObjectType, name="Magnetotellurics rx", **kwargs):
         super().__init__(object_type, name=name, **kwargs)
 
     @property
     def default_input_types(self) -> list[str]:
@@ -74,25 +68,26 @@
     @property
     def default_transmitter_type(self):
         """
         :return: Transmitter class
         """
         return type(None)
 
+    @property
+    def base_receiver_type(self):
+        return Points
+
+    @property
+    def base_transmitter_type(self):
+        return type(None)
+
     @classmethod
     def default_type_uid(cls) -> uuid.UUID:
         """
         :return: Default unique identifier
         """
         return cls.__TYPE_UID
 
     @property
-    def default_units(self) -> list[str]:
-        """Accepted time units. Must be one of "Seconds (s)",
-        "Milliseconds (ms)", "Microseconds (us)" or "Nanoseconds (ns)"
-        """
-        return self.__UNITS
-
-    @property
     def type(self):
         """Survey element type"""
         return self.__TYPE
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,28 +23,24 @@
 
 import numpy as np
 
 from geoh5py.objects.curve import Curve
 from geoh5py.objects.object_type import ObjectType
 from geoh5py.objects.points import Points
 
-from .base import BaseEMSurvey
+from .base import AirborneEMSurvey, FEMSurvey
 
+# pylint: disable=too-many-ancestors
 
-class BaseTipper(BaseEMSurvey):
+
+class TipperSurvey(FEMSurvey, AirborneEMSurvey):
     """
     Base tipper survey class.
     """
 
-    __UNITS = [
-        "Hertz (Hz)",
-        "KiloHertz (kHz)",
-        "MegaHertz (MHz)",
-        "Gigahertz (GHz)",
-    ]
     __INPUT_TYPE = ["Rx and base stations"]
     _base_stations = None
     _receivers = None
 
     def __init__(
         self,
         object_type: ObjectType,
@@ -93,72 +89,14 @@
             raise AttributeError(
                 "The input 'base_stations' should have n_vertices equal to 1, n_receivers or None."
             )
 
         self._base_stations = base
         self.edit_metadata({"Base stations": base.uid})
 
-    def copy(
-        self,
-        parent=None,
-        copy_children: bool = True,
-        clear_cache: bool = False,
-        mask: np.ndarray | None = None,
-        cell_mask: np.ndarray | None = None,
-        **kwargs,
-    ):
-        """
-        Sub-class extension of :func:`~geoh5py.objects.cell_object.CellObject.copy`.
-        """
-        if parent is None:
-            parent = self.parent
-
-        omit_list = [
-            "_metadata",
-            "_receivers",
-            "_base_stations",
-        ]
-        metadata = self.metadata.copy()
-        new_entity = super().copy(
-            parent=parent,
-            clear_cache=clear_cache,
-            copy_children=copy_children,
-            mask=mask,
-            cell_mask=cell_mask,
-            omit_list=omit_list,
-            **kwargs,
-        )
-
-        metadata["EM Dataset"][new_entity.type] = new_entity.uid
-
-        complement: TipperBaseStations | TipperReceivers = (
-            self.base_stations  # type: ignore
-            if isinstance(self, TipperReceivers)
-            else self.receivers
-        )
-        base_class: type[Points] | type[Curve] = (
-            Points if isinstance(self, TipperReceivers) else Curve  # type: ignore
-        )
-
-        if complement is not None:
-            # Reset mask
-            new_complement = super(base_class, complement).copy(  # type: ignore
-                parent=parent,
-                omit_list=omit_list,
-                copy_children=copy_children,
-                clear_cache=clear_cache,
-            )
-
-            setattr(new_entity, complement.type, new_complement)
-            metadata["EM Dataset"][complement.type] = new_complement.uid
-            new_complement.metadata = metadata
-
-        new_entity.metadata = metadata
-        return new_entity
-
     def copy_from_extent(
         self,
         extent: np.ndarray,
         parent=None,
         copy_children: bool = True,
         clear_cache: bool = False,
         inverse: bool = False,
@@ -176,24 +114,14 @@
             parent=parent,
             copy_children=copy_children,
             clear_cache=clear_cache,
             mask=indices,
             **kwargs,
         )
 
-        complement: TipperBaseStations | TipperReceivers = (
-            new_entity.base_stations  # type: ignore
-            if isinstance(self, TipperReceivers)
-            else new_entity.receivers
-        )
-
-        indices = complement.mask_by_extent(extent)
-        if indices is not None:
-            complement.remove_vertices(indices)
-
         return new_entity
 
     @property
     def default_input_types(self) -> list[str]:
         """Choice of survey creation types."""
         return self.__INPUT_TYPE
 
@@ -208,14 +136,22 @@
     def default_transmitter_type(self):
         """
         :return: Transmitter class
         """
         return type(None)
 
     @property
+    def base_receiver_type(self):
+        return Curve
+
+    @property
+    def base_transmitter_type(self):
+        return Points
+
+    @property
     def default_metadata(self) -> dict:
         """
         :return: Default unique identifier
         """
         return {
             "EM Dataset": {
                 "Base stations": None,
@@ -232,51 +168,59 @@
     def default_units(self) -> list[str]:
         """Accepted time units. Must be one of "Seconds (s)",
         "Milliseconds (ms)", "Microseconds (us)" or "Nanoseconds (ns)"
         """
         return self.__UNITS
 
 
-class TipperReceivers(BaseTipper, Curve):  # pylint: disable=too-many-ancestors
+class TipperReceivers(TipperSurvey, Curve):  # pylint: disable=too-many-ancestors
     """
     A z-tipper EM survey object.
     """
 
     __TYPE_UID = uuid.UUID("{0b639533-f35b-44d8-92a8-f70ecff3fd26}")
     __TYPE = "Receivers"
 
     def __init__(self, object_type: ObjectType, name="Tipper rx", **kwargs):
         self._base_stations: TipperBaseStations | None = None
 
         super().__init__(object_type, name=name, **kwargs)
 
+    @property
+    def complement(self):
+        return self.base_stations
+
     @classmethod
     def default_type_uid(cls) -> uuid.UUID:
         """
         :return: Default unique identifier
         """
         return cls.__TYPE_UID
 
     @property
     def type(self):
         """Survey element type"""
         return self.__TYPE
 
 
-class TipperBaseStations(BaseTipper, Points):
+class TipperBaseStations(TipperSurvey, Points):
     """
     A z-tipper EM survey object.
     """
 
     __TYPE_UID = uuid.UUID("{f495cd13-f09b-4a97-9212-2ea392aeb375}")
     __TYPE = "Base stations"
 
     def __init__(self, object_type: ObjectType, name="Tipper base", **kwargs):
         super().__init__(object_type, name=name, **kwargs)
 
+    @property
+    def complement(self):
+        return self.receivers
+
     @classmethod
     def default_type_uid(cls) -> uuid.UUID:
         """
         :return: Default unique identifier
         """
         return cls.__TYPE_UID
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.8.0a1/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/__init__.py` & `geoh5py-0.8.0a1/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/concatenation.py` & `geoh5py-0.8.0a1/geoh5py/shared/concatenation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.8.0a1/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/conversion/base.py` & `geoh5py-0.8.0a1/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.8.0a1/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.8.0a1/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/entity.py` & `geoh5py-0.8.0a1/geoh5py/shared/entity.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/entity_type.py` & `geoh5py-0.8.0a1/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/exceptions.py` & `geoh5py-0.8.0a1/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/utils.py` & `geoh5py-0.8.0a1/geoh5py/shared/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     from .entity import Entity
 
 
 @contextmanager
 def fetch_active_workspace(workspace: Workspace | None, mode: str = "r"):
     """
     Open a workspace in the requested 'mode'.
+
     If receiving an opened Workspace instead, merely return the given workspace.
 
     :param workspace: A Workspace class
     :param mode: Set the h5 read/write mode
 
     :return h5py.File: Handle to an opened Workspace.
     """
@@ -352,34 +353,41 @@
 def as_str_if_utf8_bytes(value) -> str:
     """Convert bytes to string"""
     if isinstance(value, bytes):
         value = value.decode("utf-8")
     return value
 
 
-def dict_mapper(
-    val, string_funcs: list[Callable], *args, omit: dict | None = None
-) -> dict:
+def dict_mapper(val, string_funcs: list[Callable], *args, omit: dict | None = None):
     """
     Recursion through nested dictionaries and applies mapping functions to values.
 
     :param val: Value (could be another dictionary) to apply transform functions.
     :param string_funcs: Functions to apply on values within the input dictionary.
     :param omit: Dictionary of functions to omit.
 
     :return val: Transformed values
     """
-    if omit is None:
-        omit = {}
     if isinstance(val, dict):
         for key, values in val.items():
-            val[key] = dict_mapper(
-                values,
-                [fun for fun in string_funcs if fun not in omit.get(key, [])],
-            )
+            short_list = string_funcs.copy()
+            if omit is not None:
+                short_list = [
+                    fun for fun in string_funcs if fun not in omit.get(key, [])
+                ]
+
+            val[key] = dict_mapper(values, short_list)
+
+    if isinstance(val, list):
+        out = []
+        for elem in val:
+            for fun in string_funcs:
+                elem = fun(elem, *args)
+            out += [elem]
+        return out
 
     for fun in string_funcs:
         val = fun(val, *args)
     return val
 
 
 def box_intersect(extent_a: np.ndarray, extent_b: np.ndarray) -> bool:
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/validators.py` & `geoh5py-0.8.0a1/geoh5py/shared/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  This file is part of geoapps.
 #
 #  geoapps is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 
 from __future__ import annotations
 
+import warnings
 from abc import ABC, abstractmethod
 from typing import Any
 from uuid import UUID
 
 import numpy as np
 
 from geoh5py import Workspace
@@ -113,14 +114,20 @@
         :param name: Parameter identifier.
         :param value: Input parameter value.
         :param valid: Expected value shape
         """
         if valid is None:
             return
 
+        if isinstance(valid, list):
+            warnings.warn(
+                "Data associated with multiSelect dependent is not supported. Validation ignored."
+            )
+            return
+
         if not isinstance(valid, (Entity, Workspace)):
             raise ValueError(
                 "'AssociationValidator.validate' requires a 'valid'"
                 " input of type 'Entity', 'Workspace' or None. "
                 f"Provided '{valid}' or type {type(valid)} for parameter '{name}'"
             )
 
@@ -193,38 +200,46 @@
         :param name: Parameter identifier.
         :param value: Input parameter value.
         :param valid: Expected value shape
         """
         if value is None:
             return
 
-        pshape = np.array(value).shape
+        if isinstance(value, np.ndarray):
+            pshape = value.shape
+        elif isinstance(value, list):
+            pshape = (len(value),)
+        else:
+            pshape = (1,)
+
         if pshape != valid:
             raise ShapeValidationError(name, pshape, valid)
 
 
 class TypeValidator(BaseValidator):
     """
     Validate the value type from a list of valid types.
     """
 
     validator_type = "types"
 
     @classmethod
-    def validate(cls, name: str, value: Any, valid: list[type] | type) -> None:
+    def validate(cls, name: str, value: Any, valid: type | list[type]) -> None:
         """
         :param name: Parameter identifier.
         :param value: Input parameter value.
         :param valid: List of accepted value types
         """
-
         if isinstance(valid, type):
             valid = [valid]
 
-        if not iterable(value) or list in valid:
+        if not isinstance(valid, list):
+            raise TypeError("Input `valid` options must be a type or list of types.")
+
+        if not iterable(value):
             value = (value,)
 
         for val in value:
             if not isinstance(val, tuple(valid)):
                 valid_names = [t.__name__ for t in valid if hasattr(t, "__name__")]
                 type_name = type(val).__name__
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/shared/weakref_utils.py` & `geoh5py-0.8.0a1/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/__init__.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/constants.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/input_file.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/input_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,45 +7,48 @@
 
 from __future__ import annotations
 
 import json
 import os
 import warnings
 from copy import deepcopy
+from pathlib import Path
 from typing import Any
 from uuid import UUID
 
 from geoh5py import Workspace
 from geoh5py.shared import Entity
 from geoh5py.shared.exceptions import BaseValidationError, JSONParameterValidationError
 from geoh5py.shared.validators import AssociationValidator
 
 from ..shared.utils import (
     as_str_if_uuid,
     dict_mapper,
     entity2uuid,
+    fetch_active_workspace,
     str2uuid,
     uuid2entity,
 )
 from .constants import base_validations, ui_validations
 from .utils import (
     container_group2name,
     flatten,
     inf2str,
     list2str,
     none2str,
     path2workspace,
     set_enabled,
     str2inf,
-    str2list,
     str2none,
     workspace2path,
 )
 from .validation import InputValidation
 
+# pylint: disable=simplifiable-if-expression, too-many-instance-attributes
+
 
 class InputFile:
     """
     Handles loading ui.json input files.
 
     Attributes
     ----------
@@ -67,34 +70,35 @@
     _name: str | None = None
     _data: dict[str, Any] | None
     _ui_json: dict[str, Any] | None
     _ui_validators: InputValidation = InputValidation(
         validations=ui_validations,
         validation_options={"ignore_list": ("value",)},
     )
+    _validate = True
     _validators = None
     _validations: dict | None
+    _validation_options: dict | None = None
     association_validator = AssociationValidator()
 
     def __init__(
         self,
         data: dict[str, Any] | None = None,
         ui_json: dict[str, Any] | None = None,
+        validate: bool = True,
         validations: dict | None = None,
         validation_options: dict | None = None,
     ):
-        self._workspace = None
-        self._validation_options = validation_options
+        self._geoh5 = None
+        self.validation_options = validation_options
+        self.validate = validate
         self.validations = validations
         self.ui_json = ui_json
         self.data = data
 
-        if isinstance(self.workspace, Workspace):
-            self.workspace.close()
-
     @property
     def data(self):
         if getattr(self, "_data", None) is None and self.ui_json is not None:
             self.data = flatten(self.ui_json)
 
         return self._data
 
@@ -109,23 +113,24 @@
 
             if len(value) != len(self._ui_json):
                 raise ValueError(
                     "The number of input values for 'data' must "
                     "equal the number of parameters in 'ui_json'."
                 )
 
-            if self.workspace is None and "geoh5" in value:
-                self.workspace = value["geoh5"]
+            if self._geoh5 is None and "geoh5" in value:
+                self.geoh5 = value["geoh5"]
 
-            value = self._promote(value)
+            with fetch_active_workspace(self._geoh5):
+                value = self.promote(value)
 
-            if self.validators is not None and not self.validation_options.get(
-                "disabled", False
-            ):
-                self.validators.validate_data(value)
+                if self.validators is not None and self.validate:
+                    self.validators.validate_data(value)
+
+            self.update_ui_values(value)
 
         self._data = value
 
     @property
     def name(self) -> str | None:
         """
         Name of ui.json file.
@@ -138,26 +143,21 @@
     @name.setter
     def name(self, name: str):
         if ".ui.json" not in name:
             name += ".ui.json"
 
         self._name = name
 
-    def load(self, input_dict: dict[str, Any]):
-        """Load data from dictionary and validate."""
-        self.ui_json = input_dict
-        self.data = flatten(self.ui_json)
-
     @property
     def path(self) -> str | None:
         """
         Directory for the input/output ui.json file.
         """
-        if getattr(self, "_path", None) is None and self.workspace is not None:
-            self.path = os.path.dirname(self.workspace.h5file)
+        if getattr(self, "_path", None) is None and self.geoh5 is not None:
+            self.path = os.path.dirname(self.geoh5.h5file)
 
         return self._path
 
     @path.setter
     def path(self, path: str):
         if not os.path.isdir(path):
             raise ValueError(f"The specified path: '{path}' does not exist.")
@@ -168,92 +168,97 @@
     def path_name(self) -> str | None:
         if self.path is not None and self.name is not None:
             return os.path.join(self.path, self.name)
 
         return None
 
     @staticmethod
-    def read_ui_json(json_file: str, **kwargs):
+    def read_ui_json(json_file: str | Path, **kwargs):
         """
         Read and create an InputFile from ui.json
         """
+        if isinstance(json_file, Path):
+            json_file = str(json_file)
 
-        if "ui.json" not in json_file:
-            raise ValueError("Input file should have the extension *.ui.json")
+        if not isinstance(json_file, str) or not json_file.endswith(".ui.json"):
+            raise ValueError(
+                "Input file should be a str or Path with extension *.ui.json"
+            )
 
         input_file = InputFile(**kwargs)
         input_file.path = os.path.dirname(os.path.abspath(json_file))
         input_file.name = os.path.basename(json_file)
 
         with open(json_file, encoding="utf-8") as file:
-            input_file.load(json.load(file))
+            input_file.ui_json = json.load(file)
 
-        if isinstance(input_file.workspace, Workspace):
-            input_file.workspace.close()
+        if isinstance(input_file.geoh5, Workspace):
+            input_file.geoh5.close()
 
         return input_file
 
     @property
     def ui_json(self) -> dict | None:
         """
         Dictionary representing the ui.json file with promoted values.
         """
         return self._ui_json
 
     @ui_json.setter
     def ui_json(self, value: dict[str, Any]):
-        if value is not None and self.validations is not None:
+        if value is not None:
             if not isinstance(value, dict):
                 raise ValueError("Input 'ui_json' must be of type dict or None.")
 
             self._ui_json = self.numify(value.copy())
-            default_validations = InputValidation.infer_validations(self._ui_json)
-            for key, validations in default_validations.items():
+            infered_validations = InputValidation.infer_validations(self._ui_json)
+
+            if self.validations is None:
+                self.validations = {}
+
+            for key, validations in infered_validations.items():
                 if key in self.validations:
                     validations = {**validations, **self.validations[key]}
                 self.validations[key] = validations
+
         else:
             self._ui_json = None
+            self._validations = None
+
         self._validators = None
 
     @classmethod
     def ui_validation(cls, ui_json: dict[str, Any]):
         """Validation of the ui_json forms"""
         cls._ui_validators(ui_json)
 
-    def update_ui_values(self, data: dict, none_map=None):
+    def update_ui_values(self, data: dict):
         """
         Update the ui.json values and enabled status from input data.
 
         :param data: Key and value pairs expected by the ui_json.
-        :param none_map: Map parameter 'None' values to non-null numeric types.
-            The parameters in the dictionary are mapped to optional and disabled.
 
-        :raises UserWarning: If attempting to set None value to non-optional parameter.
+        :raises AttributeError: If attempting to set None value to non-optional parameter.
         """
         if self.ui_json is None:
-            raise UserWarning("InputFile requires a 'ui_json' to be defined.")
-
-        if none_map is None:
-            none_map = {}
+            raise AttributeError("InputFile requires a 'ui_json' to be defined.")
 
         for key, value in data.items():
             if isinstance(self.ui_json[key], dict):
-                if value is None:
-                    value = none_map.get(key, None)
-                    enabled = False
-                else:
-                    enabled = True
-
-                was_group_enabled = set_enabled(self.ui_json, key, enabled)
-                if was_group_enabled:
-                    warnings.warn(
-                        f"Setting all member of group: {self.ui_json[key]['group']} "
-                        f"to enabled: {enabled}."
-                    )
+                enabled = self.ui_json[key].get("enabled", None)
+                if enabled is not None:
+                    if self.validation_options.get("update_enabled", True):
+                        enabled = False if value is None else True
+
+                    was_group_enabled = set_enabled(self.ui_json, key, enabled)
+                    if was_group_enabled:
+                        warnings.warn(
+                            f"Setting all member of group: {self.ui_json[key]['group']} "
+                            f"to enabled: {enabled}."
+                        )
 
                 member = "value"
                 if "isValue" in self.ui_json[key]:
                     if isinstance(value, (Entity, UUID)):
                         self.ui_json[key]["isValue"] = False
                         member = "property"
                     else:
@@ -264,23 +269,66 @@
 
                 self.ui_json[key][member] = value
 
             else:
                 self.ui_json[key] = value
 
     @property
+    def validate(self):
+        """Option to run validations."""
+        return self._validate
+
+    @validate.setter
+    def validate(self, value: bool):
+        if not isinstance(value, bool):
+            raise ValueError("Input value for `validate` should be True or False.")
+
+        self._validate = value
+
+    @property
     def validation_options(self):
-        """Pass validation options to the validators."""
+        """
+        Pass validation options to the validators.
+
+        The following options are supported:
+
+        - update_enabled: bool
+            If True, the enabled status of the ui_json will be updated based on the
+            value provided. Default is True.
+        - ignore_list: tuple
+            List of keys to ignore when validating the ui_json. Default is empty tuple.
+
+        """
         if self._validation_options is None:
-            return {}
+            return {
+                "update_enabled": True,
+                "ignore_list": (),
+            }
+
         return self._validation_options
 
+    @validation_options.setter
+    def validation_options(self, value: dict):
+        if not isinstance(value, (dict, type(None))):
+            raise ValueError("Input value for `validation_options` should be a dict.")
+
+        if value is not None:
+            for key in value:
+                if key not in self.validation_options:
+                    raise KeyError(
+                        f"Input key '{key}' not supported. "
+                        f"Supported keys: {list(self.validation_options.keys())}"
+                    )
+
+        self._validation_options = value
+
     @property
     def validations(self) -> dict | None:
-        if getattr(self, "_validations", None) is None:
+        """Dictionary of validations for the ui_json."""
+        if self._validations is None:
             self._validations = deepcopy(base_validations)
 
         return self._validations
 
     @validations.setter
     def validations(self, valid_dict: dict | None):
         if not isinstance(valid_dict, (dict, type(None))):
@@ -302,47 +350,48 @@
                 validations=self.validations,
                 validation_options=self.validation_options,
             )
 
         return self._validators
 
     @property
-    def workspace(self):
-        return self._workspace
-
-    @workspace.setter
-    def workspace(self, workspace: Workspace | None):
-        if workspace is not None:
-            if self._workspace is not None:
+    def geoh5(self):
+        """Geoh5 workspace."""
+        if self._geoh5 is None and self.data is not None:
+            self._geoh5 = self.data["geoh5"]
+        return self._geoh5
+
+    @geoh5.setter
+    def geoh5(self, geoh5: Workspace | None):
+        if geoh5 is not None:
+            if self._geoh5 is not None:
                 raise UserWarning(
-                    "Attribute 'workspace' already set. "
+                    "Attribute 'geoh5' already set. "
                     "Consider creating a new InputFile from arguments."
                 )
 
-            if not isinstance(workspace, Workspace):
+            if not isinstance(geoh5, Workspace):
                 raise ValueError(
-                    "Input 'workspace' must be a valid :obj:`geoh5py.workspace.Workspace`."
+                    "Input 'geoh5' must be a valid :obj:`geoh5py.workspace.Workspace`."
                 )
 
-        self._workspace = workspace
+        self._geoh5 = geoh5
 
         if self.validators is not None:
-            self.validators.workspace = workspace
+            self.validators.geoh5 = geoh5
 
     def write_ui_json(
         self,
         name: str | None = None,
-        none_map: dict[str, Any] | None = None,
-        path: str | None = None,
+        path: str | Path | None = None,
     ):
         """
         Writes a formatted ui.json file from InputFile data
 
         :param name: Name of the file
-        :param none_map: Map parameter None values to non-null numeric types.
         :param path: Directory to write the ui.json to.
         """
 
         if name is not None:
             self.name = name
 
         if path is not None:
@@ -355,33 +404,60 @@
 
         if self.ui_json is None:
             raise AttributeError(
                 "The input file requires 'ui_json' and 'data' to be set before writing out."
             )
 
         if self.data is not None:
-            self.update_ui_values(self.data, none_map=none_map)
+            self.update_ui_values(self.data)
 
         with open(self.path_name, "w", encoding="utf-8") as file:
-            json.dump(self._stringify(self._demote(self.ui_json)), file, indent=4)
+            json.dump(self.stringify(self.demote(self.ui_json)), file, indent=4)
 
         return self.path_name
 
+    def set_data_value(self, key: str, value):
+        """
+        Set the data and json form values from a dictionary.
+
+        :param key: Parameter name to update.
+        :param value: Value to update with.
+        """
+        if self.validate and self.validations is not None and key in self.validations:
+            if "association" in self.validations[key]:
+                validations = deepcopy(self.validations[key])
+                parent = self.data[self.validations[key]["association"]]
+                if isinstance(parent, UUID):
+                    parent = self.geoh5.get_entity(parent)[0]
+                validations["association"] = parent
+            else:
+                validations = self.validations[key]
+
+            validations = {k: v for k, v in validations.items() if k != "one_of"}
+            self.validators.validate(key, value, validations)
+
+        self.data[key] = value
+
+        if key == "geoh5":
+            self.geoh5 = value
+
+        self.update_ui_values({key: value})
+
     @staticmethod
-    def _stringify(var: dict[str, Any]) -> dict[str, Any]:
+    def stringify(var: dict[str, Any]) -> dict[str, Any]:
         """
         Convert inf, none, and list types to strings within a dictionary
 
         :param var: Dictionary containing ui.json keys, values, fields
 
         :return: Dictionary with inf, none and list types converted to string
             representations in json format.
         """
         for key, value in var.items():
-            exclude = ["choiceList", "meshType", "dataType", "association"]
+            exclude = ["choiceList", "meshType", "dataType", "groupType", "association"]
             mappers = (
                 [list2str, inf2str, as_str_if_uuid, none2str]
                 if key not in exclude
                 else [inf2str, as_str_if_uuid, none2str]
             )
             var[key] = dict_mapper(
                 value, mappers, omit={ex: [list2str] for ex in exclude}
@@ -413,42 +489,71 @@
                 try:
                     cls.ui_validation(value)
                 except tuple(BaseValidationError.__subclasses__()) as error:
                     raise JSONParameterValidationError(key, error.args[0]) from error
 
                 value = cls.numify(value)
 
-            mappers = (
-                [str2none, str2inf, str2uuid, path2workspace]
-                if key == "ignore_values"
-                else [str2list, str2none, str2inf, str2uuid, path2workspace]
-            )
+            mappers = [str2none, str2inf, str2uuid, path2workspace]
             ui_json[key] = dict_mapper(value, mappers)
 
         return ui_json
 
-    def _demote(self, var: dict[str, Any]) -> dict[str, str]:
+    @classmethod
+    def demote(cls, var: dict[str, Any]) -> dict[str, str]:
         """Converts promoted parameter values to their string representations."""
         mappers = [entity2uuid, as_str_if_uuid, workspace2path, container_group2name]
         for key, value in var.items():
             if isinstance(value, dict):
-                var[key] = self._demote(value)
+                var[key] = cls.demote(value)
+
             elif isinstance(value, (list, tuple)):
                 var[key] = [dict_mapper(val, mappers) for val in value]
             else:
                 var[key] = dict_mapper(value, mappers)
 
         return var
 
-    def _promote(self, var: dict[str, Any]) -> dict[str, Any]:
+    def promote(self, var: dict[str, Any]) -> dict[str, Any]:
         """Convert uuids to entities from the workspace."""
-        if self.workspace is None:
+        if self._geoh5 is None:
             return var
 
         for key, value in var.items():
             if isinstance(value, dict):
-                var[key] = self._promote(value)
-            elif isinstance(value, UUID):
-                self.association_validator(key, value, self.workspace)
-                var[key] = uuid2entity(value, self.workspace)
+                var[key] = self.promote(value)
+            else:
+                if isinstance(value, list):
+                    var[key] = [self._uid_promotion(key, val) for val in value]
+                else:
+                    var[key] = self._uid_promotion(key, value)
 
         return var
+
+    def _uid_promotion(self, key, value):
+        """
+        Check if the value needs to be promoted.
+        """
+        if isinstance(value, UUID) and self._geoh5 is not None:
+            self.association_validator(key, value, self._geoh5)
+            value = uuid2entity(value, self._geoh5)
+
+        return value
+
+    @property
+    def workspace(self) -> Workspace | None:
+        """Return the workspace associated with the input file."""
+
+        warnings.warn(
+            "The 'workspace' property is deprecated. Use 'geoh5' instead.",
+            DeprecationWarning,
+        )
+
+        return self._geoh5
+
+    @workspace.setter
+    def workspace(self, value):
+        warnings.warn(
+            "The 'workspace' property is deprecated. Use 'geoh5' instead.",
+            DeprecationWarning,
+        )
+        self.geoh5 = value
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/templates.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,29 @@
 # pylint: disable=R0913
 
 from __future__ import annotations
 
 import inspect
 from uuid import UUID
 
-from .. import objects
+from .. import groups, objects
 from ..shared import Entity
 
-known_types = [
+known_object_types = [
     member.default_type_uid()
     for _, member in inspect.getmembers(objects)
     if hasattr(member, "default_type_uid") and member.default_type_uid() is not None
 ]
 
+known_group_types = [
+    member.default_type_uid()
+    for _, member in inspect.getmembers(groups)
+    if hasattr(member, "default_type_uid") and member.default_type_uid() is not None
+]
+
 
 def optional_parameter(state: str) -> dict[str, bool]:
     """
     Returns dictionary to make existing ui optional via .update() method.
 
     :param state: Initial state of optional parameter. Can be 'enabled' or 'disabled'.
     """
@@ -71,16 +77,16 @@
     }
 
 
 def integer_parameter(
     main: bool = True,
     label: str = "Integer data",
     value: int = 1,
-    vmin: int = 0,
-    vmax: int = 100,
+    vmin: int | None = None,
+    vmax: int | None = None,
     optional: str | None = None,
 ) -> dict:
     """
     Input box for integer value.
 
     :param main: Show ui in main.
     :param label: Label identifier.
@@ -89,26 +95,31 @@
     :param vmax: Maximum value allowed.
     :param optional: Make optional if not None. Initial state provided by not None
         value.  Can be either 'enabled' or 'disabled'.
 
 
     :returns: Ui_json compliant dictionary.
     """
-    form = {"main": main, "label": label, "value": value, "min": vmin, "max": vmax}
+    form = {"main": main, "label": label, "value": value}
+
+    for prop, val in {"vmin": vmin, "vmax": vmax}.items():
+        if val is not None:
+            form[prop] = val
+
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
 
 
 def float_parameter(
     main: bool = True,
     label: str = "Float data",
     value: float = 1.0,
-    vmin: float = 0.0,
-    vmax: float = 100.0,
+    vmin: float | None = None,
+    vmax: float | None = None,
     precision: int = 2,
     line_edit: bool = True,
     optional: str | None = None,
 ) -> dict:
     """
     Input box for float value.
 
@@ -123,22 +134,25 @@
 
     :returns: Ui_json compliant dictionary.
     """
     form = {
         "main": main,
         "label": label,
         "value": value,
-        "min": vmin,
         "precision": precision,
         "lineEdit": line_edit,
-        "max": vmax,
     }
 
+    for prop, val in {"vmin": vmin, "vmax": vmax}.items():
+        if val is not None:
+            form[prop] = val
+
     if optional is not None:
         form.update(optional_parameter(optional))
+
     return form
 
 
 def string_parameter(
     main: bool = True,
     label: str = "String data",
     value: str = "data",
@@ -159,33 +173,41 @@
 
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
 
 
 def choice_string_parameter(
-    main: bool = True,
-    label: str = "String data",
     choice_list: tuple = ("Option A", "Option B"),
-    value: str = "Option A",
+    label: str = "String data",
+    main: bool = True,
+    multi_select: bool = False,
     optional: str | None = None,
+    value: str = "Option A",
 ) -> dict:
     """
     Dropdown menu of string choices.
 
     :param main: Show form in main.
+    :param choice_list: List of options.
     :param label: Label identifier.
+    :param multi_select: Option to select multiple choices.
     :param value: Input value.
-    :param choice_list: List of options.
     :param optional: Make optional if not None. Initial state provided by not None
         value.  Can be either 'enabled' or 'disabled'.
 
     :returns: Ui_json compliant dictionary.
     """
-    form = {"main": main, "label": label, "value": value, "choiceList": choice_list}
+    form = {
+        "main": main,
+        "multiSelect": multi_select,
+        "label": label,
+        "value": value,
+        "choiceList": choice_list,
+    }
 
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
 
 
 def file_parameter(
@@ -218,34 +240,68 @@
     }
 
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
 
 
+def group_parameter(
+    main: bool = True,
+    label: str = "Object",
+    group_type: tuple = tuple(known_group_types),
+    value: str | None = None,
+    optional: str | None = None,
+) -> dict:
+    """
+    Dropdown menu of groups of specific types.
+
+    :param main: Show form in main.
+    :param label: Label identifier.
+    :param value: Input value.
+    :param group_type: Type of selectable groups.
+    :param optional: Make optional if not None. Initial state provided by not None
+        value.  Can be either 'enabled' or 'disabled'.
+
+    :returns: Ui_json compliant dictionary.
+    """
+    form = {"main": main, "label": label, "value": value, "groupType": group_type}
+
+    if optional is not None:
+        form.update(optional_parameter(optional))
+    return form
+
+
 def object_parameter(
     main: bool = True,
     label: str = "Object",
-    mesh_type: tuple = tuple(known_types),
+    mesh_type: tuple = tuple(known_object_types),
+    multi_select: bool = False,
     value: str | None = None,
     optional: str | None = None,
 ) -> dict:
     """
     Dropdown menu of objects of specific types.
 
     :param main: Show form in main.
     :param label: Label identifier.
     :param value: Input value.
+    :param multi_select: Option to select multiple choices.
     :param mesh_type: Type of selectable objects.
     :param optional: Make optional if not None. Initial state provided by not None
         value.  Can be either 'enabled' or 'disabled'.
 
     :returns: Ui_json compliant dictionary.
     """
-    form = {"main": main, "label": label, "value": value, "meshType": mesh_type}
+    form = {
+        "main": main,
+        "label": label,
+        "value": value,
+        "multiSelect": multi_select,
+        "meshType": mesh_type,
+    }
 
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
 
 
 def data_parameter(
@@ -267,14 +323,15 @@
     :param association: Data association type from 'Vertex' or 'Cell'.
     :param data_type: Type of data selectable from 'Float', 'Integer' or 'Reference'.
     :param data_group_type: [Optional] Select from property_groups of type.
         '3D vector',
         'Dip direction & dip',
         'Strike & dip',
         or 'Multi-element'.
+    :param multi_select: Option to select multiple choices.
     :param parent: Parameter name corresponding to the parent object.
     :param optional: Make optional if not None. Initial state provided by not None
         value.  Can be either 'enabled' or 'disabled'.
 
     :returns: Ui_json compliant dictionary.
     """
     form = {
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/utils.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,17 @@
     if isinstance(value, Workspace):
         return value.h5file
     return value
 
 
 def path2workspace(value):
     if isinstance(value, str) and ".geoh5" in value:
-        return Workspace(value, mode="r")
+        workspace = Workspace(value, mode="r")
+        workspace.close()
+        return workspace
     return value
 
 
 def container_group2name(value):
     if isinstance(value, ContainerGroup):
         return value.name
     return value
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/ui_json/validation.py` & `geoh5py-0.8.0a1/geoh5py/ui_json/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any, cast
 from uuid import UUID
 
-from geoh5py import Workspace
 from geoh5py.groups import PropertyGroup
 from geoh5py.shared import Entity
 from geoh5py.shared.exceptions import RequiredValidationError
 from geoh5py.shared.validators import (
     AssociationValidator,
     AtLeastOneValidator,
     BaseValidator,
@@ -43,34 +42,31 @@
 class InputValidation:
     """
     Validations on dictionary of parameters.
 
     Attributes
     ----------
     validations : Validations dictionary with matching set of input parameter keys.
-    workspace (optional) : Workspace instance needed to validate uuid types.
     ignore_requirements (optional): Omit raising error on 'required' validator.
 
     Methods
     -------
     validate_data(data)
         Validates data of params and contents/type/shape/keys/reqs of values.
     """
 
     def __init__(
         self,
         validators: dict[str, BaseValidator] | None = None,
         validations: dict[str, Any] | None = None,
-        workspace: Workspace | None = None,
         ui_json: dict[str, Any] | None = None,
         validation_options: dict[str, Any] | None = None,
     ):
         self.validations = self.infer_validations(ui_json, validations=validations)
         self.validators: dict[str, BaseValidator] = validators
-        self.workspace: Workspace | None = workspace
 
         if validation_options is None:
             validation_options = {}
 
         self.ignore_list: tuple = validation_options.get("ignore_list", ())
         self.ignore_requirements: bool = validation_options.get(
             "ignore_requirements", False
@@ -97,24 +93,14 @@
 
         if self.validations is not None:
             required_validators = InputValidation._required_validators(self.validations)
             val = dict(required_validators, **val)
 
         self._validators = val
 
-    @property
-    def workspace(self):
-        return self._workspace
-
-    @workspace.setter
-    def workspace(self, value: Workspace | None):
-        if value is not None:
-            TypeValidator.validate("workspace", value, Workspace)
-        self._workspace = value
-
     @staticmethod
     def _unique_validators(validations: dict[str, Any]) -> list[str]:
         """Return names of validators required by a validations dictionary."""
         return list({key for item in validations.values() for key in item})
 
     @staticmethod
     def _required_validators(validations):
@@ -153,15 +139,15 @@
                     "types": [str],
                     "values": item["choiceList"],
                 }
             elif "fileType" in item:
                 validations[key] = {
                     "types": [str],
                 }
-            elif "meshType" in item:
+            elif "meshType" in item or "groupType" in item:
                 validations[key] = {
                     "types": [str, UUID, Entity],
                     "association": "geoh5",
                     "uuid": None,
                 }
             elif "parent" in item:
                 validations[key] = {
@@ -169,29 +155,32 @@
                     "association": item["parent"],
                     "uuid": None,
                 }
                 if "dataGroupType" in item:
                     validations[key]["property_group_type"] = item["dataGroupType"]
                     validations[key]["types"] = [str, UUID, PropertyGroup]
             elif "value" in item:
-                if item["value"] is None:
-                    check_type = str
-                else:
+                check_type = str
+                if item["value"] is not None:
                     check_type = cast(Any, type(item["value"]))
 
                 validations[key] = {
-                    "types": [check_type],
+                    "types": [check_type, Entity]
+                    if check_type is UUID
+                    else [check_type],
                 }
-                if check_type is UUID:
-                    validations[key]["types"].append(Entity)
 
             validations[key].update({"optional": not requires_value(ui_json, key)})
 
-            if not requires_value(ui_json, key) and "types" in validations[key]:
-                validations[key]["types"].append(type(None))
+            if "types" in validations[key]:
+                if not requires_value(ui_json, key):
+                    validations[key]["types"] += [type(None)]
+
+                if item.get("multiSelect", False):
+                    validations[key]["types"] += [list]
 
         return validations
 
     @staticmethod
     def infer_validations(
         ui_json: dict[str, Any] | None, validations: dict[str, dict] | None = None
     ) -> dict:
@@ -238,16 +227,16 @@
 
             validations = self.validations[name]
 
         for validator in [
             RequiredValidator,
             AtLeastOneValidator,
             OptionalValidator,
-            UUIDValidator,
             TypeValidator,
+            UUIDValidator,
             AssociationValidator,
             PropertyGroupValidator,
             ValueValidator,
             ShapeValidator,
         ]:
             val = str(validator.validator_type)
             if (
@@ -257,15 +246,17 @@
             ):
                 continue
 
             self.validators[val](name, value, validations[val])
 
     def validate_data(self, data: dict[str, Any]) -> None:
         """
-        Calls validate method on individual key/value pairs in input.
+        Calls validate method on ui.json data structure for cross-dependencies.
+
+        Individual key, value pairs are validated for expected type.
 
         :param data: Input data with known validations.
         """
 
         one_of_validations: dict[str, Any] = {}
         local_validations = self.validations.copy()
         for param, validations in local_validations.items():
@@ -280,16 +271,17 @@
                 val = {param: data[param] is not None}
                 if one_of_group in one_of_validations:
                     one_of_validations[one_of_group].update(val)
                 else:
                     one_of_validations[one_of_group] = val
 
             if "association" in validations and validations["association"] in data:
-                validations["association"] = data[validations["association"]]
-                self.validate(param, data[param], validations)
+                valid = validations.copy()
+                valid["association"] = data[validations["association"]]
+                self.validate(param, data[param], valid)
             else:
                 self.validate(param, data.get(param, None), validations)
 
         for name, val in one_of_validations.items():
             self.validate(name, val, {"one_of": None})
 
     def __call__(self, data, *args):
```

### Comparing `geoh5py-0.7.0rc5/geoh5py/workspace/__init__.py` & `geoh5py-0.8.0a1/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/geoh5py/workspace/workspace.py` & `geoh5py-0.8.0a1/geoh5py/workspace/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         self._ga_version = "1"
         self._version = 2.1
         self._name = "GEOSCIENCE"
         self._types: dict[uuid.UUID, ReferenceType[EntityType]] = {}
         self._groups: dict[uuid.UUID, ReferenceType[group.Group]] = {}
         self._objects: dict[uuid.UUID, ReferenceType[object_base.ObjectBase]] = {}
         self._data: dict[uuid.UUID, ReferenceType[data.Data]] = {}
-        self._geoh5: h5py.File | None = None
+        self._geoh5: h5py.File | bool = False
         self.h5file: str | Path | io.BytesIO = h5file
 
         for attr, item in kwargs.items():
             if attr in self._attribute_map:
                 attr = self._attribute_map[attr]
 
             if getattr(self, attr, None) is None:
@@ -172,15 +172,15 @@
         """
         return self._attribute_map
 
     def close(self):
         """
         Close the file and clear properties for future open.
         """
-        if self._geoh5 is None:
+        if not self._geoh5:
             return
 
         if self.geoh5.mode in ["r+", "a"]:
             for entity in self.groups:
                 if isinstance(entity, Concatenator) and self.repack:
                     self.update_attribute(entity, "concatenated_attributes")
 
@@ -202,16 +202,14 @@
                 os.remove(self.h5file)
                 shutil.move(temp_file, self.h5file)
             except CalledProcessError:
                 pass
 
             self.repack = False
 
-        self._geoh5 = None
-
     @property
     def contributors(self) -> np.ndarray:
         """
         :obj:`numpy.array` of :obj:`str` List of contributors name.
         """
         return self._contributors
 
@@ -922,15 +920,15 @@
         return self._all_groups()
 
     @property
     def geoh5(self) -> h5py.File:
         """
         Instance of h5py.File.
         """
-        if self._geoh5 is None:
+        if not self._geoh5:
             raise Geoh5FileClosedError
 
         return self._geoh5
 
     @property
     def h5file(self) -> str | Path | io.BytesIO:
         """
@@ -1058,15 +1056,15 @@
     def open(self, mode: str | None = None) -> Workspace:
         """
         Open a geoh5 file and load the tree structure.
 
         :param mode: Optional mode of h5py.File. Defaults to 'r+'.
         :return: `self`
         """
-        if isinstance(self._geoh5, h5py.File):
+        if isinstance(self._geoh5, h5py.File) and self._geoh5:
             warnings.warn(f"Workspace already opened in mode {self._geoh5.mode}.")
             return self
 
         if mode is None:
             mode = self._mode
 
         try:
```

### Comparing `geoh5py-0.7.0rc5/package.rst` & `geoh5py-0.8.0a1/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.7.0rc5/pyproject.toml` & `geoh5py-0.8.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.7.0-rc.5"
+version = "0.8.0-alpha.1"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 documentation = "https://geoh5py.readthedocs.io/en/latest/"
 homepage = "https://mirageoscience.com"
 readme = "package.rst"
```

### Comparing `geoh5py-0.7.0rc5/PKG-INFO` & `geoh5py-0.8.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.7.0rc5
+Version: 0.8.0a1
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://mirageoscience.com
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.8,<3.11
```

