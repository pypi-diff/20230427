# Comparing `tmp/FAST-OAD-core-1.4.2.tar.gz` & `tmp/fast_oad_core-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAST-OAD-core-1.4.2.tar", max compression
+gzip compressed data, was "fast_oad_core-1.5.0.tar", max compression
```

## Comparing `FAST-OAD-core-1.4.2.tar` & `fast_oad_core-1.5.0.tar`

### file list

```diff
@@ -1,222 +1,234 @@
--rw-r--r--   0        0        0    32472 2023-01-20 07:20:00.510581 FAST-OAD-core-1.4.2/LICENSE.txt
--rw-r--r--   0        0        0     3301 2023-01-20 07:20:00.510581 FAST-OAD-core-1.4.2/README.md
--rw-r--r--   0        0        0     3968 2023-01-20 07:20:10.514472 FAST-OAD-core-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1186 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/__init__.py
--rw-r--r--   0        0        0      829 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/__init__.py
--rw-r--r--   0        0        0     1059 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/files.py
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/__init__.py
--rw-r--r--   0        0        0     2922 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/contents.py
--rw-r--r--   0        0        0     3581 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/copy.py
--rw-r--r--   0        0        0     3030 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/strings.py
--rw-r--r--   0        0        0     1858 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/_utils/testing.py
--rw-r--r--   0        0        0     2403 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/api.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/__init__.py
--rw-r--r--   0        0        0    26703 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/api.py
--rw-r--r--   0        0        0     8991 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/cli.py
--rw-r--r--   0        0        0     2994 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/cli_utils.py
--rw-r--r--   0        0        0     1477 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/exceptions.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/resources/__init__.py
--rw-r--r--   0        0        0     2460 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/cmd/resources/fastoad.yml
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/configurations/__init__.py
--rw-r--r--   0        0        0     2974 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/constants.py
--rw-r--r--   0        0        0     1675 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/exceptions.py
--rw-r--r--   0        0        0     1063 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/gui/__init__.py
--rw-r--r--   0        0        0    19063 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/gui/analysis_and_plots.py
--rw-r--r--   0        0        0      905 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/gui/exceptions.py
--rw-r--r--   0        0        0     4295 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/gui/mission_viewer.py
--rw-r--r--   0        0        0    21069 2023-01-20 07:20:00.514581 FAST-OAD-core-1.4.2/src/fastoad/gui/optimization_viewer.py
--rw-r--r--   0        0        0    16093 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/gui/variable_viewer.py
--rw-r--r--   0        0        0      898 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/__init__.py
--rw-r--r--   0        0        0      882 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/configuration/__init__.py
--rw-r--r--   0        0        0    19153 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/configuration/configuration.py
--rw-r--r--   0        0        0     3154 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/configuration/exceptions.py
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/configuration/resources/__init__.py
--rw-r--r--   0        0        0     4038 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/configuration/resources/configuration.json
--rw-r--r--   0        0        0     1558 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/formatter.py
--rw-r--r--   0        0        0     9033 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/variable_io.py
--rw-r--r--   0        0        0      976 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/__init__.py
--rw-r--r--   0        0        0     1065 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/constants.py
--rw-r--r--   0        0        0     1907 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/exceptions.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/__init__.py
--rw-r--r--   0        0        0    37628 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/legacy1.txt
--rw-r--r--   0        0        0     1476 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/remove_duplicate_variables.py
--rw-r--r--   0        0        0     4869 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/translator.py
--rw-r--r--   0        0        0     8181 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_base.py
--rw-r--r--   0        0        0     1431 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_legacy.py
--rw-r--r--   0        0        0     3966 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_standard.py
--rw-r--r--   0        0        0      888 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/model_base/__init__.py
--rw-r--r--   0        0        0    10543 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/model_base/atmosphere.py
--rw-r--r--   0        0        0     1900 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/model_base/datacls.py
--rw-r--r--   0        0        0     9544 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/model_base/flight_point.py
--rw-r--r--   0        0        0     8996 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/model_base/propulsion.py
--rw-r--r--   0        0        0      949 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/__init__.py
--rw-r--r--   0        0        0      797 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/__init__.py
--rw-r--r--   0        0        0      807 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/__init__.py
--rw-r--r--   0        0        0     4944 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/base.py
--rw-r--r--   0        0        0     1399 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/exceptions.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/__init__.py
--rw-r--r--   0        0        0      988 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/exceptions.py
--rw-r--r--   0        0        0      896 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py
--rw-r--r--   0        0        0      979 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py
--rw-r--r--   0        0        0     8751 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py
--rw-r--r--   0        0        0    19527 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py
--rw-r--r--   0        0        0    14285 2023-01-20 07:20:00.518581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py
--rw-r--r--   0        0        0     8915 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json
--rw-r--r--   0        0        0     4752 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/schema.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/__init__.py
--rw-r--r--   0        0        0     1616 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/link_mtow.py
--rw-r--r--   0        0        0    10573 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission.py
--rw-r--r--   0        0        0    11591 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission_component.py
--rw-r--r--   0        0        0     8523 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/__init__.py
--rw-r--r--   0        0        0     2229 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml
--rw-r--r--   0        0        0     5896 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml
--rw-r--r--   0        0        0     2416 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/polar.py
--rw-r--r--   0        0        0     6435 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/routes.py
--rw-r--r--   0        0        0      804 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/__init__.py
--rw-r--r--   0        0        0     7588 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/altitude_change.py
--rw-r--r--   0        0        0    24825 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/base.py
--rw-r--r--   0        0        0    10130 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/cruise.py
--rw-r--r--   0        0        0     1364 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/hold.py
--rw-r--r--   0        0        0     1635 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/mass_input.py
--rw-r--r--   0        0        0     2219 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/speed_change.py
--rw-r--r--   0        0        0     1796 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/start.py
--rw-r--r--   0        0        0     2011 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/taxi.py
--rw-r--r--   0        0        0     2869 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/transition.py
--rw-r--r--   0        0        0     2245 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/util.py
--rw-r--r--   0        0        0     1756 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/models/variable_descriptions.txt
--rw-r--r--   0        0        0      805 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/__init__.py
--rw-r--r--   0        0        0    14623 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/_bundle_loader.py
--rw-r--r--   0        0        0    14736 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/_plugins.py
--rw-r--r--   0        0        0     1442 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/constants.py
--rw-r--r--   0        0        0     6376 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/exceptions.py
--rw-r--r--   0        0        0    19567 2023-01-20 07:20:00.522581 FAST-OAD-core-1.4.2/src/fastoad/module_management/service_registry.py
--rw-r--r--   0        0        0       35 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/.gitignore
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/__init__.py
--rw-r--r--   0        0        0    14508 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/__init__.py
--rw-r--r--   0        0        0      922 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml
--rw-r--r--   0        0        0      935 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml
--rw-r--r--   0        0        0     1260 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml
--rw-r--r--   0        0        0     1227 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/__init__.py
--rw-r--r--   0        0        0    18684 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png
--rw-r--r--   0        0        0     5532 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/problem_description.png
--rw-r--r--   0        0        0   134937 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/__init__.py
--rw-r--r--   0        0        0     1988 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/displacements.py
--rw-r--r--   0        0        0     1561 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py
--rw-r--r--   0        0        0     2150 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/stresses.py
--rw-r--r--   0        0        0      540 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt
--rw-r--r--   0        0        0     1670 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/weight.py
--rw-r--r--   0        0        0       37 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/.gitignore
--rw-r--r--   0        0        0    11579 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb
--rw-r--r--   0        0        0    34406 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb
--rw-r--r--   0        0        0    13485 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb
--rw-r--r--   0        0        0    55116 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb
--rw-r--r--   0        0        0    20123 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/__init__.py
--rw-r--r--   0        0        0      461 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/source_file.xml
--rw-r--r--   0        0        0     7146 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png
--rw-r--r--   0        0        0     6097 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png
--rw-r--r--   0        0        0   113972 2023-01-20 07:20:00.526581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png
--rw-r--r--   0        0        0   125428 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/__init__.py
--rw-r--r--   0        0        0    29150 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png
--rw-r--r--   0        0        0    40682 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png
--rw-r--r--   0        0        0    46219 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png
--rw-r--r--   0        0        0    18684 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png
--rw-r--r--   0        0        0    11722 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png
--rw-r--r--   0        0        0    65293 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png
--rw-r--r--   0        0        0    32808 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/__init__.py
--rw-r--r--   0        0        0      866 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/__init__.py
--rw-r--r--   0        0        0      346 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/__init__.py
--rw-r--r--   0        0        0      485 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/mass.py
--rw-r--r--   0        0        0      982 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/__init__.py
--rw-r--r--   0        0        0      355 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/performance.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/sub_components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/__init__.py
--rw-r--r--   0        0        0     1019 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/__init__.py
--rw-r--r--   0        0        0      687 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/__init__.py
--rw-r--r--   0        0        0      860 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py
--rw-r--r--   0        0        0     2288 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
--rw-r--r--   0        0        0     1036 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/__init__.py
--rw-r--r--   0        0        0      241 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/__init__.py
--rw-r--r--   0        0        0      806 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/__init__.py
--rw-r--r--   0        0        0      695 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/__init__.py
--rw-r--r--   0        0        0      946 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py
--rw-r--r--   0        0        0      389 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe_exercise.py
--rw-r--r--   0        0        0     1539 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py
--rw-r--r--   0        0        0     1586 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/__init__.py
--rw-r--r--   0        0        0      244 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/performance.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/__init__.py
--rw-r--r--   0        0        0     1580 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/__init__.py
--rw-r--r--   0        0        0      920 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/__init__.py
--rw-r--r--   0        0        0     1101 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.530581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/__init__.py
--rw-r--r--   0        0        0      458 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_induced_drag_coefficient.py
--rw-r--r--   0        0        0     1255 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
--rw-r--r--   0        0        0      579 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/__init__.py
--rw-r--r--   0        0        0      416 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/__init__.py
--rw-r--r--   0        0        0      358 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/compute_wing_area.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/__init__.py
--rw-r--r--   0        0        0      688 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/__init__.py
--rw-r--r--   0        0        0      531 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py
--rw-r--r--   0        0        0      850 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py
--rw-r--r--   0        0        0     1942 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py
--rw-r--r--   0        0        0     1918 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/__init__.py
--rw-r--r--   0        0        0      922 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/__init__.py
--rw-r--r--   0        0        0     1052 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/__init__.py
--rw-r--r--   0        0        0      578 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/__init__.py
--rw-r--r--   0        0        0     1913 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py
--rw-r--r--   0        0        0     2102 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py
--rw-r--r--   0        0        0     1057 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py
--rw-r--r--   0        0        0     1029 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py
--rw-r--r--   0        0        0      825 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py
--rw-r--r--   0        0        0     1308 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml
--rw-r--r--   0        0        0      757 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py
--rw-r--r--   0        0        0     1283 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/README.md
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/notebooks/__init__.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/__init__.py
--rw-r--r--   0        0        0     3545 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/_utils.py
--rw-r--r--   0        0        0     1378 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/exceptions.py
--rw-r--r--   0        0        0    13363 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/problem.py
--rw-r--r--   0        0        0      758 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/resources/__init__.py
--rw-r--r--   0        0        0    11038 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/validity_checker.py
--rw-r--r--   0        0        0      893 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/__init__.py
--rw-r--r--   0        0        0    12340 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/variable.py
--rw-r--r--   0        0        0    21756 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/variable_list.py
--rw-r--r--   0        0        0     2128 2023-01-20 07:20:00.534581 FAST-OAD-core-1.4.2/src/fastoad/openmdao/whatsopt.py
--rw-r--r--   0        0        0     8893 2023-01-20 07:20:11.846734 FAST-OAD-core-1.4.2/setup.py
--rw-r--r--   0        0        0     5481 2023-01-20 07:20:11.847721 FAST-OAD-core-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-04-27 14:57:11.135288 fast_oad_core-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     3488 2023-04-27 14:57:11.135288 fast_oad_core-1.5.0/README.md
+-rw-r--r--   0        0        0     4231 2023-04-27 14:57:32.796920 fast_oad_core-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1186 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/__init__.py
+-rw-r--r--   0        0        0     1059 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/files.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/__init__.py
+-rw-r--r--   0        0        0     2922 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/contents.py
+-rw-r--r--   0        0        0     3581 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/copy.py
+-rw-r--r--   0        0        0     3030 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/strings.py
+-rw-r--r--   0        0        0     1858 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/testing.py
+-rw-r--r--   0        0        0     3375 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/api.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/cmd/__init__.py
+-rw-r--r--   0        0        0    30528 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/cmd/api.py
+-rw-r--r--   0        0        0    10473 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/cli.py
+-rw-r--r--   0        0        0     2994 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/cli_utils.py
+-rw-r--r--   0        0        0     1477 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/exceptions.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/resources/__init__.py
+-rw-r--r--   0        0        0     2460 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/resources/fastoad.yml
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/configurations/__init__.py
+-rw-r--r--   0        0        0     2974 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/constants.py
+-rw-r--r--   0        0        0     1675 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/exceptions.py
+-rw-r--r--   0        0        0     1087 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/__init__.py
+-rw-r--r--   0        0        0    23361 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/analysis_and_plots.py
+-rw-r--r--   0        0        0      905 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/exceptions.py
+-rw-r--r--   0        0        0     4073 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/mission_viewer.py
+-rw-r--r--   0        0        0    21069 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/optimization_viewer.py
+-rw-r--r--   0        0        0    16093 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/variable_viewer.py
+-rw-r--r--   0        0        0      898 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/__init__.py
+-rw-r--r--   0        0        0      882 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/__init__.py
+-rw-r--r--   0        0        0    19153 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/configuration.py
+-rw-r--r--   0        0        0     3154 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/exceptions.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/__init__.py
+-rw-r--r--   0        0        0     4038 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/configuration.json
+-rw-r--r--   0        0        0     1558 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/formatter.py
+-rw-r--r--   0        0        0     9033 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/variable_io.py
+-rw-r--r--   0        0        0      976 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/__init__.py
+-rw-r--r--   0        0        0     1065 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/constants.py
+-rw-r--r--   0        0        0     1907 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/exceptions.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/__init__.py
+-rw-r--r--   0        0        0    37628 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/legacy1.txt
+-rw-r--r--   0        0        0     1476 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/remove_duplicate_variables.py
+-rw-r--r--   0        0        0     4869 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/translator.py
+-rw-r--r--   0        0        0     8181 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_base.py
+-rw-r--r--   0        0        0     1431 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_legacy.py
+-rw-r--r--   0        0        0     3966 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_standard.py
+-rw-r--r--   0        0        0      888 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/__init__.py
+-rw-r--r--   0        0        0    10543 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/atmosphere.py
+-rw-r--r--   0        0        0     1900 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/datacls.py
+-rw-r--r--   0        0        0     9806 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/flight_point.py
+-rw-r--r--   0        0        0     8996 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/propulsion.py
+-rw-r--r--   0        0        0      949 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/__init__.py
+-rw-r--r--   0        0        0     9057 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/base.py
+-rw-r--r--   0        0        0     1705 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/exceptions.py
+-rw-r--r--   0        0        0     6217 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/__init__.py
+-rw-r--r--   0        0        0      988 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/exceptions.py
+-rw-r--r--   0        0        0      896 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py
+-rw-r--r--   0        0        0     1022 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py
+-rw-r--r--   0        0        0     8930 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py
+-rw-r--r--   0        0        0    23483 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py
+-rw-r--r--   0        0        0    15608 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py
+-rw-r--r--   0        0        0     9592 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json
+-rw-r--r--   0        0        0     5090 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/schema.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/__init__.py
+-rw-r--r--   0        0        0     9130 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/base.py
+-rw-r--r--   0        0        0     1616 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/link_mtow.py
+-rw-r--r--   0        0        0    10612 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission.py
+-rw-r--r--   0        0        0     9878 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_run.py
+-rw-r--r--   0        0        0    10152 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py
+-rw-r--r--   0        0        0    21188 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/payload_range.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/__init__.py
+-rw-r--r--   0        0        0     2229 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml
+-rw-r--r--   0        0        0     5896 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml
+-rw-r--r--   0        0        0     3624 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar.py
+-rw-r--r--   0        0        0     4019 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar_modifier.py
+-rw-r--r--   0        0        0     6561 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/routes.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/__init__.py
+-rw-r--r--   0        0        0    11836 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/base.py
+-rw-r--r--   0        0        0     4912 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/macro_segments.py
+-rw-r--r--   0        0        0     1241 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/__init__.py
+-rw-r--r--   0        0        0     7782 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/altitude_change.py
+-rw-r--r--   0        0        0    10181 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/cruise.py
+-rw-r--r--   0        0        0     2163 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/ground_speed_change.py
+-rw-r--r--   0        0        0     1486 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/hold.py
+-rw-r--r--   0        0        0     1648 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/mass_input.py
+-rw-r--r--   0        0        0     2390 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/speed_change.py
+-rw-r--r--   0        0        0     1887 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/start.py
+-rw-r--r--   0        0        0     1135 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/__init__.py
+-rw-r--r--   0        0        0     6038 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/end_of_takeoff.py
+-rw-r--r--   0        0        0     3142 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/rotation.py
+-rw-r--r--   0        0        0     2659 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/takeoff.py
+-rw-r--r--   0        0        0     2063 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/taxi.py
+-rw-r--r--   0        0        0     2873 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/transition.py
+-rw-r--r--   0        0        0    17916 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/time_step_base.py
+-rw-r--r--   0        0        0     2245 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/util.py
+-rw-r--r--   0        0        0     1695 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/variable_descriptions.txt
+-rw-r--r--   0        0        0      805 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/__init__.py
+-rw-r--r--   0        0        0    14623 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/_bundle_loader.py
+-rw-r--r--   0        0        0    18578 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/_plugins.py
+-rw-r--r--   0        0        0     1442 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/constants.py
+-rw-r--r--   0        0        0     7475 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/exceptions.py
+-rw-r--r--   0        0        0    19567 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/service_registry.py
+-rw-r--r--   0        0        0       64 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/.gitignore
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/__init__.py
+-rw-r--r--   0        0        0    14508 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/__init__.py
+-rw-r--r--   0        0        0      922 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml
+-rw-r--r--   0        0        0      935 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml
+-rw-r--r--   0        0        0     1260 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml
+-rw-r--r--   0        0        0     1227 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/__init__.py
+-rw-r--r--   0        0        0    18684 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png
+-rw-r--r--   0        0        0     5532 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/problem_description.png
+-rw-r--r--   0        0        0   134937 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/__init__.py
+-rw-r--r--   0        0        0     1988 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/displacements.py
+-rw-r--r--   0        0        0     1561 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py
+-rw-r--r--   0        0        0     2150 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/stresses.py
+-rw-r--r--   0        0        0      540 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt
+-rw-r--r--   0        0        0     1670 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/weight.py
+-rw-r--r--   0        0        0       37 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/.gitignore
+-rw-r--r--   0        0        0    11579 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb
+-rw-r--r--   0        0        0    34406 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb
+-rw-r--r--   0        0        0    13485 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb
+-rw-r--r--   0        0        0    55116 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb
+-rw-r--r--   0        0        0    20123 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/source_file.xml
+-rw-r--r--   0        0        0     7146 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png
+-rw-r--r--   0        0        0     6097 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png
+-rw-r--r--   0        0        0   113972 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png
+-rw-r--r--   0        0        0   125428 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/__init__.py
+-rw-r--r--   0        0        0    29150 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png
+-rw-r--r--   0        0        0    40682 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png
+-rw-r--r--   0        0        0    46219 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png
+-rw-r--r--   0        0        0    18684 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png
+-rw-r--r--   0        0        0    11722 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png
+-rw-r--r--   0        0        0    65293 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png
+-rw-r--r--   0        0        0    32808 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/__init__.py
+-rw-r--r--   0        0        0      346 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/mass.py
+-rw-r--r--   0        0        0      982 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/__init__.py
+-rw-r--r--   0        0        0      355 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/__init__.py
+-rw-r--r--   0        0        0      687 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py
+-rw-r--r--   0        0        0     2288 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
+-rw-r--r--   0        0        0     1036 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/__init__.py
+-rw-r--r--   0        0        0      806 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/__init__.py
+-rw-r--r--   0        0        0      946 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py
+-rw-r--r--   0        0        0      389 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe_exercise.py
+-rw-r--r--   0        0        0     1539 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py
+-rw-r--r--   0        0        0     1586 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0     1580 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/__init__.py
+-rw-r--r--   0        0        0      458 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_induced_drag_coefficient.py
+-rw-r--r--   0        0        0     1255 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
+-rw-r--r--   0        0        0      579 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/__init__.py
+-rw-r--r--   0        0        0      416 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/__init__.py
+-rw-r--r--   0        0        0      358 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/compute_wing_area.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/__init__.py
+-rw-r--r--   0        0        0      688 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py
+-rw-r--r--   0        0        0      850 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py
+-rw-r--r--   0        0        0     1942 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py
+-rw-r--r--   0        0        0     1918 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/__init__.py
+-rw-r--r--   0        0        0      922 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/__init__.py
+-rw-r--r--   0        0        0      578 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/__init__.py
+-rw-r--r--   0        0        0     1913 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py
+-rw-r--r--   0        0        0     2102 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py
+-rw-r--r--   0        0        0     1057 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/README.md
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/__init__.py
+-rw-r--r--   0        0        0     4032 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/_utils.py
+-rw-r--r--   0        0        0     1378 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/exceptions.py
+-rw-r--r--   0        0        0    12567 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/problem.py
+-rw-r--r--   0        0        0      758 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/resources/__init__.py
+-rw-r--r--   0        0        0    11038 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/validity_checker.py
+-rw-r--r--   0        0        0      877 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/__init__.py
+-rw-r--r--   0        0        0    12467 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable.py
+-rw-r--r--   0        0        0    21838 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable_list.py
+-rw-r--r--   0        0        0     2128 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/whatsopt.py
+-rw-r--r--   0        0        0      757 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/source_data_files/__init__.py
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 fast_oad_core-1.5.0/PKG-INFO
```

### Comparing `FAST-OAD-core-1.4.2/LICENSE.txt` & `fast_oad_core-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/README.md` & `fast_oad_core-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+<p align="center">
+  <img src="docs/img/FAST_OAD_logo2.jpg" alt="FAST-OAD logo" width="600">
+</p>
+
+Future Aircraft Sizing Tool - Overall Aircraft Design
+===============================================================
+
 ![Tests](https://github.com/fast-aircraft-design/FAST-OAD/workflows/Tests/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9691f1d1430c45cf9c94bc342b4c6122)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/fast-aircraft-design/FAST-OAD/branch/master/graph/badge.svg)](https://codecov.io/gh/fast-aircraft-design/FAST-OAD)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![Documentation Status](https://readthedocs.org/projects/fast-oad/badge/?version=stable)](https://fast-oad.readthedocs.io/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?urlpath=lab%2Ftree%2Fsrc%2Ffastoad%2Fnotebooks)
+[![DOI](https://zenodo.org/badge/186570813.svg)](https://zenodo.org/badge/latestdoi/186570813)
+
+
 
 
-FAST-OAD: Future Aircraft Sizing Tool - Overall Aircraft Design
-===============================================================
 
 FAST-OAD is a framework for performing rapid Overall Aircraft Design.
 
 It proposes multi-disciplinary analysis and optimisation by relying on
 the [OpenMDAO framework](https://openmdao.org/).
 
 FAST-OAD allows easy switching between models for a same discipline, and
```

### Comparing `FAST-OAD-core-1.4.2/pyproject.toml` & `fast_oad_core-1.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FAST-OAD-core"
-version = "v1.4.2" # This version number is overwritten by GitHub packaging workflow but setting 1.3 here will allow installation of CS25 models in development mode
+version = "1.5.0" # This version number is overwritten by GitHub packaging workflow but setting this version here will allow installation of CS25 models in development mode
 description = "FAST-OAD is a framework for performing rapid Overall Aircraft Design"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
     "Scott DELBECQ <Scott.DELBECQ@isae-supaero.fr>"
 ]
 packages = [
@@ -42,15 +42,15 @@
 # of poetry.lock file will modify docs/requirements.txt and make
 # the commit fail because "files were modified by this hook". In that case,
 # doing again the commit including changes in docs/requirements.txt will succeed.
 python = "^3.7"
 numpy = "^1.21.0"
 scipy = "^1.4.1"
 pandas = "^1.1.0"
-openmdao = "^3.10"
+openmdao = "^3.18"
 ipopo = "^1.0.0"
 ipywidgets = "^7.7.0"
 ipysheet = ">=0.5.0, <1"
 plotly = "^5.0.0"
 wop = "^2.2.0"
 lxml = "^4.6.5"
 tomlkit = ">=0.5.3, <1"
@@ -63,44 +63,56 @@
 jupyter-client = "!=7.0.0, !=7.0.1, !=7.0.2, !=7.0.3, !=7.0.4, !=7.0.5"  # v7.0.6 fixes issue #381
 notebook = "^6.0"
 stdatm = "0.*"
 Deprecated = "^1.2.13"
 click = "^8.0.3"
 importlib-metadata = { version = "^4.2", python = "<3.10" }
 mpi4py = {version = "^3", optional = true}
+pyDOE2 = "^1.3.0"
 
 [tool.poetry.extras]
 mpi4py = ["mpi4py"]
 
-[tool.poetry.dev-dependencies]
-fast-oad-cs25 = ">=0.1.4"
+[tool.poetry.group.dev.dependencies]
+fast-oad-cs25 = ">=0.2"
+matplotlib = "^3.1.2"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
 coverage = { extras = ["toml"], version = "^7.0" }
-pre-commit = "^2.14.1"
-black = { version = "21.9b0", extras = ["jupyter"], allow-prereleases = true }
-pylint = "^2.10.2"
 nbval = "^0.10"
+
+[tool.poetry.group.doc.dependencies]
 sphinx = "^4.1.2"
 sphinx-rtd-theme = "^1.0"
 sphinxcontrib-bibtex = "^2.3.0"
+
+[tool.poetry.group.lint.dependencies]
+pre-commit = "^2.14.1"
+black = { version = "21.9b0", extras = ["jupyter"], allow-prereleases = true }
+pylint = "^2.10.2"
 flake8 = "^4.0.1"
-matplotlib = "^3.1.2"
 nbstripout = "^0.6.0"
 
 [tool.poetry.scripts]
 fastoad = "fastoad.cmd.cli:fast_oad"
 fast-oad = "fastoad.cmd.cli:fast_oad"
 
 [tool.poetry.plugins."fastoad.plugins"]
 "bundled" = "fastoad"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov fastoad --cov-report term-missing --cov-report html --verbose"
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/files.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/files.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/contents.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/contents.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/resource_management/copy.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/copy.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/strings.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/strings.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/_utils/testing.py` & `fast_oad_core-1.5.0/src/fastoad/_utils/testing.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/api.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import shutil
 import sys
 import textwrap as tw
 from collections import defaultdict
 from collections.abc import Iterable
 from time import time
 from typing import Dict, IO, List, Union
+from enum import Enum
 
 import openmdao.api as om
 import pandas as pd
 from IPython import InteractiveShell
 from IPython.display import HTML, clear_output, display
 from tabulate import tabulate
 
@@ -52,14 +53,19 @@
 DEFAULT_WOP_URL = "https://ether.onera.fr/whatsopt"
 _LOGGER = logging.getLogger(__name__)
 
 # Used for test purposes only
 _PROBLEM_CONFIGURATOR = None
 
 
+class UserFileType(Enum):
+    CONFIGURATION = "configuration"
+    SOURCE_DATA = "source_data"
+
+
 def get_plugin_information(print_data=False) -> Dict[str, DistributionPluginDefinition]:
     """
     Provides information about available FAST-OAD plugins.
 
     :param print_data: if True, plugin data are displayed.
     :return: a dict with installed package names as keys and matching FAST-OAD
              plugin definitions as values.
@@ -133,87 +139,173 @@
             target_path = pth.join(*target_path_elements)
             os.makedirs(target_path)
             copy_resource_folder(folder_info.package_name, target_path)
 
     return destination_path
 
 
-def generate_configuration_file(
-    configuration_file_path: str,
+def _generate_user_file(
+    user_file_type: UserFileType,
+    user_file_path: str,
     overwrite: bool = False,
     distribution_name=None,
-    sample_file_name=None,
+    sample_user_file_name=None,
 ):
     """
-    Copies a sample configuration file from an available plugin.
-
-    :param configuration_file_path: the path of file to be written
+    Copies a sample user file from an available plugin. Since there are a lot of similarities
+    between the generation of source data files and configuration file, this generic method was
+    created to refactor their generation. The term user file is the generic term for
+    configuration files, source data files and inputs/outputs data files (not relevant here).
+
+    :param user_file_type: the type of user file that needs to be written, should match one
+                          available in _AVAILABLE_USER_FILE_TYPE
+    :param user_file_path: the path of the user file to be written
     :param overwrite: if True, the file will be written, even if it already exists
     :param distribution_name: the name of the installed package that provides the sample
-                             configuration file (can be omitted if only one plugin is available)
-    :param sample_file_name: the name of the sample configuration file (can be omitted if
-                             the plugin provides only one configuration file)
+                             user file (can be omitted if only one plugin is available)
+    :param sample_user_file_name: the name of the sample user file (can be omitted if the plugin
+                                 provides only one user file)
     :return: path of generated file
-    :raise FastPathExistsError: if overwrite==False and configuration_file_path already exists
+    :raise FastPathExistsError: if overwrite==False and user_file_path already exists
     """
 
     if distribution_name is None:
-        # If no distribution is specified, but only one contains configuration files, no need to
-        # specify the name
-        count_plugin_with_conf_file = 0
-        dist_with_conf_file = ""
-        plugin_config_files = {
-            name: [resource.name for resource in definition.get_configuration_file_list()]
-            for name, definition in get_plugin_information().items()
-        }
-        for plugin_name, conf_files in plugin_config_files.items():
-            # Plugin is retained if it contains conf files. Additionally, if sample_file_name
-            # is provided, plugin is retained only if sample_file_name is in provided conf files.
-            if len(conf_files) > 0 and (sample_file_name is None or sample_file_name in conf_files):
-                count_plugin_with_conf_file += 1
-                dist_with_conf_file = plugin_name
-            if count_plugin_with_conf_file > 1:
+        # If no distribution is specified, but only one contains the type of user files
+        # requested, no need to specify the name
+        count_plugin_with_user_file = 0
+        dist_with_user_file = ""
+
+        # Browse plugin and look for the type of user file requested
+        plugin_user_files = {}
+        for name, definition in get_plugin_information().items():
+            if user_file_type is UserFileType.CONFIGURATION:
+                matching_resources = [
+                    resource.name for resource in definition.get_configuration_file_list()
+                ]
+            else:
+                # Since we ensured the type is among the one we expect we can use the else,
+                # may need to be changed if other user file are added later on.
+                matching_resources = [
+                    resource.name for resource in definition.get_source_data_file_list()
+                ]
+
+            plugin_user_files[name] = matching_resources
+
+        for plugin_name, user_files in plugin_user_files.items():
+            # Plugin is retained if it contains the requested user files. Additionally, if
+            # sample_user_file_name is provided, plugin is retained only if sample_user_file_name
+            # is in provided user files.
+            if len(user_files) > 0 and (
+                sample_user_file_name is None or sample_user_file_name in user_files
+            ):
+                count_plugin_with_user_file += 1
+                dist_with_user_file = plugin_name
+            if count_plugin_with_user_file > 1:
                 break
 
         # If only one plugin has been retained, it can be used as automatically selected plugin.
-        if count_plugin_with_conf_file == 1:
-            distribution_name = dist_with_conf_file
+        if count_plugin_with_user_file == 1:
+            distribution_name = dist_with_user_file
 
     dist_definition = FastoadLoader().get_distribution_plugin_definition(distribution_name)
-    file_info = dist_definition.get_configuration_file_info(sample_file_name)
+    if user_file_type is UserFileType.CONFIGURATION:
+        file_info = dist_definition.get_configuration_file_info(sample_user_file_name)
+    else:
+        # Since we ensured the type is among the one we expect we can use the else,
+        # may need to be changed if other user file are added later on.
+        file_info = dist_definition.get_source_data_file_info(sample_user_file_name)
 
     # Check on file overwrite
-    configuration_file_path = pth.abspath(configuration_file_path)
-    if not overwrite and pth.exists(configuration_file_path):
+    user_file_path = pth.abspath(user_file_path)
+    if not overwrite and pth.exists(user_file_path):
         raise FastPathExistsError(
-            f"Configuration file {configuration_file_path} not written because it already exists. "
+            user_file_type.value.capitalize()
+            + f" {user_file_path} not written because it already exists. "
             "Use overwrite=True to bypass.",
-            configuration_file_path,
+            user_file_path,
         )
 
     # Write file
-    make_parent_dir(configuration_file_path)
-    copy_resource(file_info.package_name, file_info.name, configuration_file_path)
-    _LOGGER.info('Sample configuration written in "%s".', configuration_file_path)
+    make_parent_dir(user_file_path)
+    copy_resource(file_info.package_name, file_info.name, user_file_path)
+    _LOGGER.info(
+        'Sample %s written in "%s".', user_file_type.value.replace("_", " "), user_file_path
+    )
+
+    return user_file_path
+
+
+def generate_configuration_file(
+    configuration_file_path: str,
+    overwrite: bool = False,
+    distribution_name=None,
+    sample_file_name=None,
+):
+    """
+    Copies a sample configuration file from an available plugin.
+
+    :param configuration_file_path: the path of file to be written
+    :param overwrite: if True, the file will be written, even if it already exists
+    :param distribution_name: the name of the installed package that provides the sample
+                             configuration file (can be omitted if only one plugin is available)
+    :param sample_file_name: the name of the sample configuration file (can be omitted if
+                             the plugin provides only one configuration file)
+    :return: path of generated file
+    :raise FastPathExistsError: if overwrite==False and configuration_file_path already exists
+    """
+
+    return _generate_user_file(
+        user_file_type=UserFileType.CONFIGURATION,
+        user_file_path=configuration_file_path,
+        overwrite=overwrite,
+        distribution_name=distribution_name,
+        sample_user_file_name=sample_file_name,
+    )
+
+
+def generate_source_data_file(
+    source_data_file_path: str,
+    overwrite: bool = False,
+    distribution_name=None,
+    sample_file_name=None,
+):
+    """
+    Copies a sample source data file from an available plugin.
+
+    :param source_data_file_path: the path of file to be written
+    :param overwrite: if True, the file will be written, even if it already exists
+    :param distribution_name: the name of the installed package that provides the sample
+                             source data file (can be omitted if only one plugin is available)
+    :param sample_file_name: the name of the sample source data file (can be omitted if
+                             the plugin provides only one source data file)
+    :return: path of generated file
+    :raise FastPathExistsError: if overwrite==False and source_file_path already exists
+    """
 
-    return configuration_file_path
+    return _generate_user_file(
+        user_file_type=UserFileType.SOURCE_DATA,
+        user_file_path=source_data_file_path,
+        overwrite=overwrite,
+        distribution_name=distribution_name,
+        sample_user_file_name=sample_file_name,
+    )
 
 
 def generate_inputs(
     configuration_file_path: str,
-    source_path: str = None,
-    source_path_schema="native",
+    source_data_path: str = None,
+    source_data_path_schema="native",
     overwrite: bool = False,
 ) -> str:
     """
     Generates input file for the problem specified in configuration_file_path.
 
     :param configuration_file_path: where the path of input file to write is set
-    :param source_path: path of file data will be taken from
-    :param source_path_schema: set to 'legacy' if the source file come from legacy FAST
+    :param source_data_path: path of source data file data will be taken from
+    :param source_data_path_schema: set to 'legacy' if the source file come from legacy FAST
     :param overwrite: if True, file will be written even if one already exists
     :return: path of generated file
     :raise FastPathExistsError: if overwrite==False and configuration_file_path already exists
     """
     conf = FASTOADProblemConfigurator(configuration_file_path)
     conf._set_configuration_modifier(_PROBLEM_CONFIGURATOR)
 
@@ -221,18 +313,18 @@
     if not overwrite and pth.exists(conf.input_file_path):
         raise FastPathExistsError(
             f"Input file {input_file_path} not written because it already exists. "
             "Use overwrite=True to bypass.",
             input_file_path,
         )
 
-    if source_path_schema == "legacy":
-        conf.write_needed_inputs(source_path, VariableLegacy1XmlFormatter())
+    if source_data_path_schema == "legacy":
+        conf.write_needed_inputs(source_data_path, VariableLegacy1XmlFormatter())
     else:
-        conf.write_needed_inputs(source_path)
+        conf.write_needed_inputs(source_data_path)
 
     _LOGGER.info("Problem inputs written in %s", input_file_path)
     return input_file_path
 
 
 def list_variables(
     configuration_file_path: str,
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/cli.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 from fastoad.module_management.exceptions import (
     FastNoAvailableConfigurationFileError,
     FastNoDistPluginError,
     FastSeveralConfigurationFilesError,
     FastSeveralDistPluginsError,
     FastUnknownConfigurationFileError,
     FastUnknownDistPluginError,
+    FastNoAvailableSourceDataFileError,
+    FastSeveralSourceDataFilesError,
+    FastUnknownSourceDataFileError,
 )
 from . import api
 
 NOTEBOOK_FOLDER_NAME = "FAST-OAD_notebooks"
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
@@ -86,22 +89,63 @@
         FastSeveralConfigurationFilesError,
         FastUnknownConfigurationFileError,
         FastNoAvailableConfigurationFileError,
     ) as exc:
         click.echo(exc.args[0])
 
 
+@fast_oad.command(name="gen_source_data_file")
+@click.argument("source_data_file", nargs=1)
+@click.option(
+    "-p",
+    "--from_package",
+    nargs=1,
+    help="Name of installed package that provides the sample source data file.",
+)
+@click.option("-s", "--source", nargs=1, help="Name of original source data file.")
+@overwrite_option
+def gen_source_data_file(source_data_file, from_package, source, force):
+    """
+    Generate a sample source data file with given argument as name.
+
+    Option "--from_package" has to be used if several FAST-OAD plugins are available.
+
+    Option "--source" has to be used if the targeted plugin provides several sample
+    source data files.
+
+    Use "fastoad plugin_info" to get information about available plugins and sample
+    configuration files.
+    """
+    try:
+        manage_overwrite(
+            api.generate_source_data_file,
+            source_data_file_path=source_data_file,
+            overwrite=force,
+            distribution_name=from_package,
+            sample_file_name=source,
+        )
+    except (
+        FastNoDistPluginError,
+        FastSeveralDistPluginsError,
+        FastUnknownDistPluginError,
+        FastSeveralSourceDataFilesError,
+        FastUnknownSourceDataFileError,
+        FastNoAvailableSourceDataFileError,
+    ) as exc:
+        click.echo(exc.args[0])
+
+
 @fast_oad.command(name="gen_inputs")
 @click.argument("conf_file", nargs=1)
-@click.argument("source_file", nargs=1, required=False)
+@click.argument("source_data_file", nargs=1, required=False)
 @overwrite_option
 @click.option(
-    "--legacy", is_flag=True, help="To be used if the source XML file is in legacy format."
+    "--legacy", is_flag=True, help="To be used if the source data XML file is in legacy format."
 )
-def gen_inputs(conf_file, source_file, force, legacy):
+def gen_inputs(conf_file, source_data_file, force, legacy):
     """
     Generate the input file (specified in the configuration file) with needed variables.
 
     \b
     Examples:
     ---------
     # For the problem defined in conf_file.yml, generates the input file with default
@@ -116,16 +160,16 @@
     # Same as above, some_file.xml is formatted with the legacy FAST schema
         fastoad gen_inputs conf_file.yml some_file.xml --legacy
     """
     schema = "legacy" if legacy else "native"
     manage_overwrite(
         api.generate_inputs,
         configuration_file_path=conf_file,
-        source_path=source_file,
-        source_path_schema=schema,
+        source_data_path=source_data_file,
+        source_data_path_schema=schema,
         overwrite=force,
     )
 
 
 @fast_oad.command(name="list_modules")
 @out_file_option
 @click.option("-v", "--verbose", is_flag=True, help="Shows detailed information for each system.")
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/cli_utils.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/cli_utils.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/cmd/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/cmd/resources/fastoad.yml` & `fast_oad_core-1.5.0/src/fastoad/cmd/resources/fastoad.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/configurations/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/constants.py` & `fast_oad_core-1.5.0/src/fastoad/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/gui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 
 from .analysis_and_plots import (
     aircraft_geometry_plot,
     drag_polar_plot,
     mass_breakdown_bar_plot,
     mass_breakdown_sun_plot,
     wing_geometry_plot,
+    payload_range_plot,
 )
 from .mission_viewer import MissionViewer
 from .optimization_viewer import OptimizationViewer
 from .variable_viewer import VariableViewer
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/analysis_and_plots.py` & `fast_oad_core-1.5.0/src/fastoad/gui/analysis_and_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -445,14 +445,128 @@
     )
 
     fig.update_layout(title_text="Mass Breakdown", title_x=0.5)
 
     return fig
 
 
+def payload_range_plot(
+    aircraft_file_path: str,
+    name="Payload-Range",
+    mission_name="operational",
+    variable_of_interest: str = None,
+    variable_of_interest_legend: str = None,
+):
+    """
+    Returns a figure of the payload-range diagram.
+    The diagram contains by default only the contour but can also provide a heatmap
+    of the grid points, if variable_of_interest is not None.
+    Please note that the data for the contour are expected in the variables
+    `data:payload_range:{mission_name}:range` and `data:payload_range:{mission_name}:payload`.
+    Similarly, the data for the heatmap are expected in the variables
+    `data:payload_range:{mission_name}:grid:range`,
+    `data:payload_range:{mission_name}:grid:payload` and
+    `data:payload_range:{mission_name}:grid:{variable_of_interest}`.
+
+    :param aircraft_file_path: path of data file
+    :param name: name to give to the trace added to the figure
+    :param mission_name: name of the mission present in the data file to be plotted.
+    :param variable_of_interest: variable of interest for the heatmap.
+    :param variable_of_interest_legend: name to give to variable of interest in plot legend.
+    :return: payload-range plot figure
+    """
+    variables = VariableIO(aircraft_file_path).read()
+
+    # Contour of the payload range
+    range_ = np.asarray(variables[f"data:payload_range:{mission_name}:range"].value)
+    payload = np.asarray(variables[f"data:payload_range:{mission_name}:payload"].value)
+
+    pr_contour = go.Scatter(
+        x=convert_units(range_, "m", "NM"),
+        y=convert_units(payload, "kg", "t"),
+        mode="lines+markers",
+        line=dict(color="black", width=3),
+        showlegend=False,
+        name=name,
+    )
+
+    # Create mask for a nice payload range
+    range_mask = np.append(range_, (1.03 * max(range_), 1.03 * max(range_), 0))
+    payload_mask = np.append(payload, (0, 1.1 * max(payload), 1.1 * max(payload)))
+
+    pr_contour_mask = go.Scatter(
+        x=convert_units(range_mask, "m", "NM"),
+        y=convert_units(payload_mask, "kg", "t"),
+        mode="lines",
+        line=dict(color="#E5ECF6", width=3),
+        showlegend=False,
+        name=name,
+        fill="toself",
+        fillcolor="#E5ECF6",
+    )
+
+    fig = go.Figure()
+    fig.add_trace(pr_contour_mask)
+    fig.add_trace(pr_contour)
+
+    if variable_of_interest is not None:
+        # Grid for the payload range
+        range_grid = np.asarray(variables[f"data:payload_range:{mission_name}:grid:range"].value)
+        payload_grid = np.asarray(
+            variables[f"data:payload_range:{mission_name}:grid:payload"].value
+        )
+        variable_of_interest_grid = np.asarray(
+            variables[f"data:payload_range:{mission_name}:grid:{variable_of_interest}"].value
+        )
+
+        variable_of_interest_unit = variables[
+            f"data:payload_range:{mission_name}:grid:{variable_of_interest}"
+        ].units
+
+        if variable_of_interest_legend is None:
+            variable_of_interest_legend = variable_of_interest
+
+        x = convert_units(range_grid, "m", "NM")
+        y = convert_units(payload_grid, "kg", "t")
+        z = variable_of_interest_grid
+
+        min_z = min(z)
+        max_z = max(z)
+
+        fig.add_trace(
+            go.Contour(
+                x=x,
+                y=y,
+                z=z,
+                contours=dict(start=min_z, end=max_z, size=(max_z - min_z) / 20),
+                colorbar=dict(
+                    title=f"{variable_of_interest_legend} [{variable_of_interest_unit}]",
+                    titleside="right",
+                    titlefont=dict(size=15, family="Arial, sans-serif"),
+                    tickformat=".1e",
+                ),
+                colorscale="RdBu_r",
+                contours_coloring="heatmap",
+            )
+        )
+        fig.add_trace(go.Scatter(x=x, y=y, hovertext=z, mode="markers"))
+
+    fig.update_layout(
+        xaxis_title="Range [NM]",
+        yaxis_title="Payload [tons]",
+        yaxis_range=[0, convert_units(max(payload_mask), "kg", "t")],
+        xaxis_range=[0, convert_units(max(range_mask), "m", "NM")],
+        showlegend=False,
+        height=500,
+        width=900,
+        title={"text": name, "y": 0.9, "x": 0.5, "xanchor": "center", "yanchor": "top"},
+    )
+    return fig
+
+
 def _get_variable_values_with_new_units(
     variables: VariableList, var_names_and_new_units: Dict[str, str]
 ):
     """
     Returns the value of the requested variable names with respect to their new units in the order
     in which their were given. This function works only for variable of value with shape=1 or float.
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/gui/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/mission_viewer.py` & `fast_oad_core-1.5.0/src/fastoad/gui/mission_viewer.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     A class for facilitating the post-processing of mission and trajectories
     """
 
     def __init__(self):
         # The dataframes containing each mission
         self.missions = {}
 
-        # The figure displayed
-        self._fig = None
+        # The output widget containing the figure to display
+        self._output_widget = None
 
         # The x selector
         self._x_widget = None
 
         # The y selector
         self._y_widget = None
 
@@ -54,73 +54,69 @@
         ):
             self.missions[name] = pd.read_csv(mission_data, index_col=0)
         elif isinstance(mission_data, pd.DataFrame):
             self.missions[name] = mission_data
         else:
             raise TypeError("Unknown type for mission data, please use .csv of DataFrame")
 
-        # Initialize widgets when first mission is added
-        if len(self.missions) == 1:
-            self._initialize_widgets()
-
-    def _initialize_widgets(self):
+    def display(self):
         """
-        Initializes the widgets for selecting x and y
+        Display the user interface
+        :return the display object
         """
 
         key = list(self.missions)[0]
         keys = self.missions[key].keys()
 
+        self._output_widget = widgets.Output()
+
         # By default ground distance
         self._x_widget = widgets.Dropdown(value=keys[2], options=keys)
-        self._x_widget.observe(self.display, "value")
+        self._x_widget.observe(self._show_plot, "value")
         # By default altitude
         self._y_widget = widgets.Dropdown(value=keys[1], options=keys)
-        self._y_widget.observe(self.display, "value")
+        self._y_widget.observe(self._show_plot, "value")
+
+        self._show_plot()
+
+        toolbar = widgets.HBox(
+            [widgets.Label(value="x:"), self._x_widget, widgets.Label(value="y:"), self._y_widget]
+        )
 
-    def _build_plots(self):
+        ui = display(toolbar, self._output_widget)
+
+        return ui
+
+    # pylint: disable=unused-argument # change has to be there for observe() to work
+    def _show_plot(self, change=None):
         """
-        Add a plot of the mission
+        Updates and shows the plots
         """
 
-        x_name = self._x_widget.value
-        y_name = self._y_widget.value
+        with self._output_widget:
 
-        for name in self.missions:
-            if self._fig is None:
-                self._fig = go.Figure()
-            # pylint: disable=invalid-name # that's a common naming
-            x = self.missions[name][x_name]
-            # pylint: disable=invalid-name # that's a common naming
-            y = self.missions[name][y_name]
+            clear_output(wait=True)
 
-            scatter = go.Scatter(x=x, y=y, mode="lines", name=name)
+            x_name = self._x_widget.value
+            y_name = self._y_widget.value
 
-            self._fig.add_trace(scatter)
+            fig = None
 
-            self._fig = go.FigureWidget(self._fig)
+            for mission_name in self.missions:
 
-        self._fig.update_layout(
-            title_text="Mission", title_x=0.5, xaxis_title=x_name, yaxis_title=y_name
-        )
+                if fig is None:
+                    fig = go.Figure()
+                # pylint: disable=invalid-name # that's a common naming
+                x = self.missions[mission_name][x_name]
+                # pylint: disable=invalid-name # that's a common naming
+                y = self.missions[mission_name][y_name]
 
-    # pylint: disable=unused-argument  # args has to be there for observe() to work
-    def display(self, change=None) -> display:
-        """
-        Display the user interface
-        :return the display object
-        """
-        clear_output(wait=True)
-        self._update_plots()
-        toolbar = widgets.HBox(
-            [widgets.Label(value="x:"), self._x_widget, widgets.Label(value="y:"), self._y_widget]
-        )
-        # pylint: disable=invalid-name # that's a common naming
-        ui = widgets.VBox([toolbar, self._fig])
-        return display(ui)
+                scatter = go.Scatter(x=x, y=y, mode="lines", name=mission_name)
 
-    def _update_plots(self):
-        """
-        Update the plots
-        """
-        self._fig = None
-        self._build_plots()
+                fig.add_trace(scatter)
+
+            fig.update_layout(
+                title_text="Mission", title_x=0.5, xaxis_title=x_name, yaxis_title=y_name
+            )
+
+            fig = go.FigureWidget(fig)
+            display(fig)
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/optimization_viewer.py` & `fast_oad_core-1.5.0/src/fastoad/gui/optimization_viewer.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/gui/variable_viewer.py` & `fast_oad_core-1.5.0/src/fastoad/gui/variable_viewer.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/io/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/configuration/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/io/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/configuration/configuration.py` & `fast_oad_core-1.5.0/src/fastoad/io/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/configuration/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/io/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/configuration/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/configuration/resources/configuration.json` & `fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/configuration.json`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/formatter.py` & `fast_oad_core-1.5.0/src/fastoad/io/formatter.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/variable_io.py` & `fast_oad_core-1.5.0/src/fastoad/io/variable_io.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/constants.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/legacy1.txt` & `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/legacy1.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/resources/remove_duplicate_variables.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/remove_duplicate_variables.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/translator.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/translator.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_base.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_base.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_legacy.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_legacy.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/io/xml/variable_io_standard.py` & `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_standard.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/model_base/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/model_base/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/model_base/atmosphere.py` & `fast_oad_core-1.5.0/src/fastoad/model_base/atmosphere.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/model_base/datacls.py` & `fast_oad_core-1.5.0/src/fastoad/model_base/datacls.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/model_base/flight_point.py` & `fast_oad_core-1.5.0/src/fastoad/model_base/flight_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Structure for managing flight point data."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -86,43 +86,49 @@
     equivalent_airspeed: float = None  #: Equivalent airspeed (EAS) in m/s.
     mach: float = None  #: Mach number.
     engine_setting: EngineSetting = None  #: Engine setting.
     #: Lift coefficient.
     CL: float = None  # pylint: disable=invalid-name
     #: Drag coefficient.
     CD: float = None  # pylint: disable=invalid-name
+    lift: float = None  #: Aircraft lift in Newtons
     drag: float = None  #: Aircraft drag in Newtons.
     thrust: float = None  #: Thrust in Newtons.
     thrust_rate: float = None  #: Thrust rate (between 0. and 1.)
 
     #: If True, propulsion should match the thrust value.
     #: If False, propulsion should match thrust rate.
     thrust_is_regulated: bool = None
 
     sfc: float = None  #: Specific Fuel Consumption in kg/N/s.
     slope_angle: float = None  #: Slope angle in radians.
     acceleration: float = None  #: Acceleration value in m/s**2.
+    alpha: float = 0.0  #: angle of attack in radians
+    slope_angle_derivative: float = None  #: slope angle derivative in rad/s
     name: str = None  #: Name of current phase.
 
     _units = dict(
         time="s",
         altitude="m",
         ground_distance="m",
         mass="kg",
         true_airspeed="m/s",
         equivalent_airspeed="m/s",
         mach="-",
         CL="-",
         CD="-",
+        lift="N",
         drag="N",
         thrust="N",
         thrust_rate="-",
         sfc="kg/N/s",
         slope_angle="rad",
         acceleration="m/s**2",
+        alpha="rad",
+        slope_angle_derivative="rad/s",
     )
 
     def __post_init__(self):
         self._relative_parameters = {"ground_distance", "time"}
 
     def set_as_relative(self, field_names: Union[Sequence[str], str]):
         """
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/model_base/propulsion.py` & `fast_oad_core-1.5.0/src/fastoad/model_base/propulsion.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Exceptions for mission package."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2020  ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -27,7 +27,18 @@
     """
 
 
 class FastFlightSegmentIncompleteFlightPoint(FastError):
     """
     Raised when a segment computation encounters a FlightPoint instance without needed parameters.
     """
+
+
+class FastUnknownMissionElementError(FastError):
+    """Raised when an undeclared element type is requested."""
+
+    def __init__(self, element_type: str):
+        self.segment_type = element_type
+
+        msg = f'Element type "{element_type}" has not been declared.'
+
+        super().__init__(self, msg)
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Constants for mission builder package.
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -14,12 +14,13 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 NAME_TAG = "name"
 TYPE_TAG = "type"
 SEGMENT_TYPE_TAG = "segment_type"
 
-# FIXME: should be set in Route class
+# FIXME: should be set in classes that use these parameters.
 BASE_UNITS = {
     "range": "m",
     "distance_accuracy": "m",
+    "alpha": "rad",
 }
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py`

 * *Files 17% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
     #: Value of the "shape" openMDAO flag for input declaration.
     shape: Optional[Tuple[int]] = None
 
     #: Value of the "shape_by_conn" openMDAO flag for input declaration.
     shape_by_conn: bool = False
 
+    #: Prefix used when replacement of "~" is needed.
+    prefix: str = ""
+
     #: Used only for tests
     variable_name: InitVar[Optional[str]] = None
 
     #: Used only for tests
     use_opposite: InitVar[Optional[bool]] = None
 
     #: True if the opposite value should be used, if input is defined by a variable.
@@ -114,36 +117,38 @@
         """
         try:
             return om.convert_units(self.input_value, self.input_unit, self.output_unit)
         except TypeError:
             return self.input_value
 
     @classmethod
-    def from_dict(cls, parameter_name, definition_dict: dict, part_identifier=None):
+    def from_dict(cls, parameter_name, definition_dict: dict, part_identifier=None, prefix=None):
         """
         Instantiates InputDefinition from definition_dict.
 
         definition_dict["value"] is used as `input_value` in instantiation. It can be an actual
         value or a variable name.
 
         :param parameter_name: used if definition_dict["value"] == "~" (or "-~")
         :param definition_dict: dict with keys ("value", "unit", "default"). "unit" and "default"
                                 are optional.
         :param part_identifier: used if "~" is in definition_dict["value"]
+        :param prefix: used if "~" is in definition_dict["value"]
         """
         if "value" not in definition_dict:
             return None
 
         input_def = cls(
             parameter_name,
             definition_dict["value"],
             input_unit=definition_dict.get("unit"),
             default_value=definition_dict.get("default", np.nan),
             shape_by_conn=definition_dict.get("shape_by_conn", False),
             part_identifier=part_identifier,
+            prefix=prefix,
         )
         return input_def
 
     def set_variable_value(self, inputs: Mapping):
         """
         Sets numerical value from OpenMDAO inputs.
 
@@ -204,15 +209,15 @@
                 else:
                     # Standard case with simple tilda
                     prefix, suffix = var_name.replace(":~", "~").split("~")
                     part_identifier = self.part_identifier
 
                 if not prefix:
                     # If nothing before "~", a default value is used
-                    prefix = "data:mission"
+                    prefix = self.prefix
                 if not suffix:
                     # If nothing after "~", the parameter name is used
                     suffix = self.parameter_name
 
                 var_name = ":".join([prefix, part_identifier, suffix])
 
             self._variable_name = var_name
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Mission generator."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from collections import ChainMap, OrderedDict
+from collections import ChainMap
+from copy import deepcopy
 from dataclasses import fields
 from typing import Dict, List, Mapping, Optional, Union
 
 import pandas as pd
 
 from fastoad.constants import EngineSetting
 from fastoad.model_base import FlightPoint
@@ -34,45 +35,77 @@
     CLIMB_PARTS_TAG,
     CRUISE_PART_TAG,
     DESCENT_PARTS_TAG,
     MISSION_DEFINITION_TAG,
     MissionDefinition,
     PARTS_TAG,
     PHASE_TAG,
+    POLAR_TAG,
     RESERVE_TAG,
     ROUTE_TAG,
     SEGMENT_TAG,
 )
 from ...base import FlightSequence
+from ...mission import Mission
 from ...polar import Polar
+from ...polar_modifier import RegisterPolarModifier, UnchangedPolar
 from ...routes import RangedRoute
-from ...segments.base import AbstractFlightSegment, SegmentDefinitions
+from ...segments.base import AbstractFlightSegment, RegisterSegment
+
+
+# Rationale:
+# The way we parse the mission definition file answers several needs:
+# - Producing an executable mission instance, able to compute the mission simulation.
+# - Allowing to replace variables in the mission definition by their values, knowing the
+#   name can be contextual: a same phase definition can be used in 2 different routes or missions
+#   and variable names in this phase may depend on the parent.
+# - Allowing to know all the needed variables before knowing their values, hence before
+#   building the mission instance.
+#
+# Therefore, we have first the structure_builders package, that will provide classes to parse the
+# definition file to create a global structure of the mission, ready to implement. This structure
+# will be able to provide the actual names of the variables used in the mission, but does not
+# have to know their values.
+#
+# Then we can use the MissionBuilder below to build the mission instance and provide information
+# on the mission, once variable values have been supplied.
 
 
 class MissionBuilder:
     """
     This class builds and computes a mission from a provided definition.
     """
 
     def __init__(
         self,
         mission_definition: Union[str, MissionDefinition],
         *,
         propulsion: IPropulsion = None,
         reference_area: float = None,
+        mission_name: Optional[str] = None,
+        variable_prefix: str = "data:mission",
     ):
         """
         :param mission_definition: a file path or MissionDefinition instance
         :param propulsion: if not provided, the property :attr:`propulsion` must be
                            set before calling :meth:`build`
         :param reference_area: if not provided, the property :attr:`reference_area` must be
                                set before calling :meth:`build`
+        :param mission_name: name of chosen mission, if already decided.
+        :param variable_prefix: prefix for auto-generated variable names.
         """
         self._structure_builders: Dict[str, AbstractStructureBuilder] = {}
-        self.definition = mission_definition
+
+        self._variable_prefix: str = variable_prefix
+
+        #: The definition of missions as provided in input file.
+        self.definition: MissionDefinition = mission_definition
+
+        self._mission_name = mission_name
+
         self._base_kwargs = {"reference_area": reference_area, "propulsion": propulsion}
 
     @property
     def definition(self) -> MissionDefinition:
         """
         The mission definition instance.
 
@@ -83,21 +116,15 @@
     @definition.setter
     def definition(self, mission_definition: Union[str, MissionDefinition]):
         if isinstance(mission_definition, str):
             self._definition = MissionDefinition(mission_definition)
         else:
             self._definition = mission_definition
 
-        for mission_name in self._definition[MISSION_DEFINITION_TAG]:
-            self._structure_builders[mission_name] = MissionStructureBuilder(
-                self._definition, mission_name
-            )
-
-            if self.get_input_weight_variable_name(mission_name) is None:
-                self._add_default_taxi_takeoff(mission_name)
+        self._update_structure_builders()
 
     @property
     def propulsion(self) -> IPropulsion:
         """Propulsion model for performance computation."""
         return self._base_kwargs["propulsion"]
 
     @propulsion.setter
@@ -109,58 +136,109 @@
         """Reference area for aerodynamic polar."""
         return self._base_kwargs["reference_area"]
 
     @reference_area.setter
     def reference_area(self, reference_area: float):
         self._base_kwargs["reference_area"] = reference_area
 
-    def build(self, inputs: Optional[Mapping] = None, mission_name: str = None) -> FlightSequence:
+    @property
+    def mission_name(self):
+        """The mission name, in case it has been specified, or if it is unique in the file."""
+        if self._mission_name is None:
+            self._mission_name = self.get_unique_mission_name()
+
+        return self._mission_name
+
+    @mission_name.setter
+    def mission_name(self, value):
+        if value is None:
+            self._mission_name = None
+        elif value in self.definition[MISSION_DEFINITION_TAG]:
+            self._mission_name = value
+        else:
+            raise FastMissionFileMissingMissionNameError(
+                f'No Mission named "{value}" in provided mission file.'
+            )
+
+    @property
+    def variable_prefix(self):
+        """The prefix for auto-generated variable names."""
+        return self._variable_prefix
+
+    @variable_prefix.setter
+    def variable_prefix(self, value):
+        self._variable_prefix = value
+        self._update_structure_builders()
+
+    def build(self, inputs: Optional[Mapping] = None, mission_name: str = None) -> Mission:
         """
         Builds the flight sequence from definition file.
 
         :param inputs: if provided, any input parameter that is a string which matches
                        a key of `inputs` will be replaced by the corresponding value
-        :param mission_name: mission name (can be omitted if only one mission is defined)
+        :param mission_name: mission name (can be omitted if only one mission is defined or if
+                             :attr:`mission` has been defined)
         :return:
         """
+        if mission_name is None:
+            mission_name = self.mission_name
+
         if self.get_input_weight_variable_name(mission_name) is None:
             self._add_default_taxi_takeoff(mission_name)
 
         for input_def in self._structure_builders[mission_name].get_input_definitions():
             input_def.set_variable_value(inputs)
-        if mission_name is None:
-            mission_name = self.get_unique_mission_name()
+
         mission = self._build_mission(self._structure_builders[mission_name].structure)
         return mission
 
+    def get_route_names(self, mission_name: str = None) -> List[str]:
+        """
+
+        :param mission_name:
+        :return: a list with names of all routes in the mission, in order.
+        """
+        if mission_name is None:
+            mission_name = self.mission_name
+
+        mission_parts = self.definition[MISSION_DEFINITION_TAG][mission_name][PARTS_TAG]
+        route_names = [part[ROUTE_TAG] for part in mission_parts if ROUTE_TAG in part]
+
+        return route_names
+
     def get_route_ranges(
         self, inputs: Optional[Mapping] = None, mission_name: str = None
     ) -> List[float]:
         """
 
         :param inputs: if provided, any input parameter that is a string which matches
                        a key of `inputs` will be replaced by the corresponding value
-        :param mission_name: mission name (can be omitted if only one mission is defined)
+        :param mission_name: mission name (can be omitted if only one mission is defined or if
+                             :attr:`mission` has been defined)
         :return: list of flight ranges for each element of the flight sequence that is a route
         """
-        routes = self.build(inputs, mission_name).flight_sequence
+        if mission_name is None:
+            mission_name = self.mission_name
+
+        routes = self.build(inputs, mission_name)
         return [route.flight_distance for route in routes if isinstance(route, RangedRoute)]
 
     def get_reserve(self, flight_points: pd.DataFrame, mission_name: str = None) -> float:
         """
         Computes the reserve fuel according to definition in mission input file.
 
         :param flight_points: the dataframe returned by compute_from() method of the
                               instance returned by :meth:`build`
-        :param mission_name: mission name (can be omitted if only one mission is defined)
+        :param mission_name: mission name (can be omitted if only one mission is defined or if
+                             :attr:`mission` has been defined)
         :return: the reserve fuel mass in kg, or 0.0 if no reserve is defined.
         """
 
         if mission_name is None:
-            mission_name = self.get_unique_mission_name()
+            mission_name = self.mission_name
 
         last_part_spec = self._get_mission_part_structures(mission_name)[-1]
         if RESERVE_TAG in last_part_spec:
             ref_name = last_part_spec[RESERVE_TAG]["ref"].value
             multiplier = last_part_spec[RESERVE_TAG]["multiplier"].value
 
             route_points = flight_points.loc[
@@ -171,19 +249,20 @@
 
         return 0.0
 
     def get_input_variables(self, mission_name=None) -> VariableList:
         """
         Identify variables for a defined mission.
 
-        :param mission_name: mission name (can be omitted if only one mission is defined)
+        :param mission_name: mission name (can be omitted if only one mission is defined or if
+                             :attr:`mission` has been defined)
         :return: a VariableList instance.
         """
         if mission_name is None:
-            mission_name = self.get_unique_mission_name()
+            mission_name = self.mission_name
 
         input_definition = VariableList()
         for input_def in self._structure_builders[mission_name].get_input_definitions():
             if input_def.variable_name and input_def.variable_name not in input_definition.names():
                 input_definition.append(input_def.get_input_definition())
 
         return input_definition
@@ -199,82 +278,78 @@
         if len(self._structure_builders) == 1:
             return list(self._structure_builders.keys())[0]
 
         raise FastMissionFileMissingMissionNameError(
             "Mission name must be specified if several missions are defined in mission file."
         )
 
-    def get_input_weight_variable_name(self, mission_name: str) -> Optional[str]:
+    def get_input_weight_variable_name(self, mission_name: str = None) -> Optional[str]:
         """
         Search the mission structure for a segment that has a target absolute mass defined and
         returns the associated variable name.
 
-        :param mission_name:
+        :param mission_name: mission name (can be omitted if only one mission is defined or if
+                             :attr:`mission` has been defined)
         :return: The variable name, or None if no target mass found.
         """
+
         return self._get_input_weight_variable_name_in_structure(
             self._get_mission_part_structures(mission_name)
         )
 
-    def get_mission_start_mass_input(self, mission_name: str) -> Optional[str]:
-        """
-
-        :param mission_name:
-        :return: Target mass variable of first segment, if any.
-        """
-        part = self._get_first_segment_structure(mission_name)
-        if "mass" in part["target"]:
-            return part["target"]["mass"].variable_name
-
-        return None
-
-    def _get_first_segment_structure(self, mission_name: str):
-        part = self._get_mission_part_structures(mission_name)[0]
-        while PARTS_TAG in part:
-            part = part[PARTS_TAG][0]
-        return part
-
-    def get_mission_part_names(self, mission_name: str) -> List[str]:
-        """
+    def _update_structure_builders(self):
+        for mission_name in self._definition[MISSION_DEFINITION_TAG]:
+            self._structure_builders[mission_name] = MissionStructureBuilder(
+                self._definition, mission_name, variable_prefix=self._variable_prefix
+            )
 
-        :param mission_name:
-        :return: list of names of parts (phase or route) for specified mission.
-        """
-        return [
-            part[NAME_TAG]
-            for part in self._get_mission_part_structures(mission_name)
-            if part.get(TYPE_TAG) in [ROUTE_TAG, PHASE_TAG]
-        ]
+            if self.get_input_weight_variable_name(mission_name) is None:
+                self._add_default_taxi_takeoff(mission_name)
 
-    def _build_mission(self, mission_structure: OrderedDict) -> FlightSequence:
+    def _build_mission(self, mission_structure: dict) -> Mission:
         """
         Builds mission instance from provided structure.
 
         :param mission_structure: structure of the mission to build
         :return: the mission instance
         """
-        mission = FlightSequence()
 
         part_kwargs = self._get_part_kwargs({}, mission_structure)
 
+        mission = Mission(target_fuel_consumption=part_kwargs.get("target_fuel_consumption"))
+
         mission.name = mission_structure[NAME_TAG]
         for part_spec in mission_structure[PARTS_TAG]:
             if TYPE_TAG not in part_spec:
                 continue
             if part_spec[TYPE_TAG] == SEGMENT_TAG:
                 part = self._build_segment(part_spec, part_kwargs)
-            if part_spec[TYPE_TAG] == ROUTE_TAG:
+            elif part_spec[TYPE_TAG] == ROUTE_TAG:
                 part = self._build_route(part_spec, part_kwargs)
             elif part_spec[TYPE_TAG] == PHASE_TAG:
                 part = self._build_phase(part_spec, part_kwargs)
-            mission.flight_sequence.append(part)
+            else:
+                raise RuntimeError(
+                    "Unknown part type. This error should have been prevented "
+                    "by the JSON schema validation."
+                )
+            mission.append(part)
+
+        last_part = mission_structure[PARTS_TAG][-1]
+        if RESERVE_TAG in last_part:
+            mission.reserve_ratio = last_part[RESERVE_TAG]["multiplier"].value
+            base_route_name_definition = last_part[RESERVE_TAG].get("ref")
+            if base_route_name_definition:
+                mission.reserve_base_route_name = (
+                    f"{mission.name}:{base_route_name_definition.value}"
+                )
 
         return mission
 
-    def _build_route(self, route_structure: OrderedDict, kwargs: Mapping = None):
+    def _build_route(self, route_structure: dict, kwargs: Mapping = None):
         """
         Builds route instance.
 
         :param route_structure: structure of the route to build
         :return: the route instance
         """
         climb_phases = []
@@ -334,34 +409,46 @@
         part_kwargs = self._get_part_kwargs(kwargs, phase_structure)
 
         for part_structure in phase_structure[PARTS_TAG]:
             if part_structure[TYPE_TAG] == PHASE_TAG:
                 flight_part = self._build_phase(part_structure, part_kwargs)
             else:
                 flight_part = self._build_segment(part_structure, part_kwargs)
-            phase.flight_sequence.append(flight_part)
+            phase.append(flight_part)
 
         return phase
 
-    def _build_segment(self, segment_definition: Mapping, kwargs: Mapping) -> AbstractFlightSegment:
+    def _build_segment(self, segment_definition: Mapping, kwargs: dict) -> AbstractFlightSegment:
         """
         Builds a flight segment according to provided definition.
 
         :param segment_definition: the segment definition from mission file
         :param kwargs: a preset of keyword arguments for AbstractFlightSegment instantiation
-        :param tag: the expected tag for specifying the segment type
         :return: the FlightSegment instance
         """
-        segment_class = SegmentDefinitions.get_segment_class(segment_definition[SEGMENT_TYPE_TAG])
+        segment_class = RegisterSegment.get_class(segment_definition[SEGMENT_TYPE_TAG])
         part_kwargs = kwargs.copy()
         part_kwargs.update(segment_definition)
         part_kwargs.update(self._base_kwargs)
+        part_kwargs["polar_modifier"] = UnchangedPolar()
         for key, value in part_kwargs.items():
-            if key == "polar":
-                value = Polar(value["CL"].value, value["CD"].value)
+            if key == POLAR_TAG:
+                modifier_kwargs = deepcopy(value.get("modifier"))
+                value = Polar(
+                    cl=value["CL"].value,
+                    cd=value["CD"].value,
+                    alpha=value["alpha"].value if "alpha" in value else None,
+                )
+                if modifier_kwargs:
+                    if isinstance(modifier_kwargs, InputDefinition):
+                        modifier_kwargs = {NAME_TAG: modifier_kwargs.value}
+                    modifier_class = RegisterPolarModifier.get_class(modifier_kwargs[NAME_TAG])
+                    del modifier_kwargs[NAME_TAG]
+                    self._replace_input_definitions_by_values(modifier_kwargs)
+                    part_kwargs["polar_modifier"] = modifier_class(**modifier_kwargs)
             elif key == "target":
                 if not isinstance(value, FlightPoint):
                     target_parameters = {
                         param.parameter_name: param.value for param in value.values()
                     }
                     relative_fields = [
                         param.parameter_name for param in value.values() if param.is_relative
@@ -474,14 +561,16 @@
                             "target": {"mass": {"value": "~~:TOW", "unit": "kg"}},
                         },
                     ]
                 },
             }
         }
 
-        taxi_out = PhaseStructureBuilder(definition, "taxi_out", mission_name)
+        taxi_out = PhaseStructureBuilder(
+            definition, "taxi_out", mission_name, self._variable_prefix
+        )
         taxi_out_structure = self._structure_builders[mission_name].process_builder(taxi_out)
         self._structure_builders[mission_name].structure[PARTS_TAG].insert(0, taxi_out_structure)
 
-        takeoff = PhaseStructureBuilder(definition, "takeoff", mission_name)
+        takeoff = PhaseStructureBuilder(definition, "takeoff", mission_name, self._variable_prefix)
         takeoff_structure = self._structure_builders[mission_name].process_builder(takeoff)
         self._structure_builders[mission_name].structure[PARTS_TAG].insert(1, takeoff_structure)
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Classes for managing internal structures of missions.
 
 The mission file provides a "human" definition of the mission.
 Structures are the translation of this human definition, that is ready to
-be transformed in a Python implementation.
+be transformed into a Python implementation.
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
-from collections import OrderedDict
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field, fields
 from itertools import chain
 from typing import List, Tuple
 
 import numpy as np
 
@@ -33,19 +32,20 @@
     CLIMB_PARTS_TAG,
     CRUISE_PART_TAG,
     DESCENT_PARTS_TAG,
     MISSION_DEFINITION_TAG,
     PARTS_TAG,
     PHASE_DEFINITIONS_TAG,
     PHASE_TAG,
+    POLAR_TAG,
     ROUTE_DEFINITIONS_TAG,
     ROUTE_TAG,
     SEGMENT_TAG,
 )
-from ...segments.base import SegmentDefinitions
+from ...segments.base import RegisterSegment
 
 
 @dataclass
 class AbstractStructureBuilder(ABC):
     """
     Base class for building structures of mission parts.
 
@@ -61,37 +61,39 @@
     be used to ensure a correct processing of the global structure, especially to get a correct
     resolution of :attr:`input_definitions`.
     """
 
     definition: InitVar[dict]
     name: str
     parent_name: str = None
+    variable_prefix: str = ""
 
-    _structure: OrderedDict = field(default=None, init=False)
+    _structure: dict = field(default=None, init=False)
 
     _input_definitions: List[InputDefinition] = field(default_factory=list, init=False)
     _builders: List[Tuple["AbstractStructureBuilder", dict]] = field(
         default_factory=list, init=False
     )
 
     #: Defined by subclass
     type = None
 
     def __init_subclass__(cls, *, structure_type=None):
         cls.type = structure_type
 
     def __post_init__(self, definition):
         self._structure = self._build(definition)
-        self._structure[NAME_TAG] = self.qualified_name
         if self.__class__.type:
             self._structure[TYPE_TAG] = self.__class__.type
+        self._structure[NAME_TAG] = self.qualified_name
+        self._process_polar(self._structure)
         self._parse_inputs(self._structure, self._input_definitions)
 
     @property
-    def structure(self) -> OrderedDict:
+    def structure(self) -> dict:
         """A dictionary that is ready to be translated to the matching implementation."""
         for builder, placeholder in self._builders:
             placeholder.update(builder.structure)
             self._input_definitions += builder.get_input_definitions()
         self._builders = []  # Builders have been used and can be forgotten.
         return self._structure
 
@@ -119,15 +121,15 @@
         """
 
         placeholder = {}
         self._builders.append((builder, placeholder))
         return placeholder
 
     @abstractmethod
-    def _build(self, definition: dict) -> OrderedDict:
+    def _build(self, definition: dict) -> dict:
         """
         This method creates the needed structure dict.
 
         Keys "name" and "type" are not needed, as they will be written later on in the process.
 
         .. Important::
 
@@ -166,26 +168,26 @@
         :param structure:
         :param parent:
         :param part_identifier:
         :return: amended definition
         """
 
         if isinstance(structure, dict):
-            if "polar" in structure:
-                structure["polar"] = self._process_polar(structure["polar"])
-
             if "value" in structure:
                 input_definition = InputDefinition.from_dict(
-                    parent, structure, part_identifier=part_identifier
+                    parent, structure, part_identifier=part_identifier, prefix=self.variable_prefix
                 )
                 input_definitions.append(input_definition)
                 return input_definition
 
             part_identifier = structure.get(NAME_TAG, part_identifier)
-            segment_class = SegmentDefinitions.get_segment_class(structure.get(SEGMENT_TYPE_TAG))
+            if SEGMENT_TYPE_TAG in structure:
+                segment_class = RegisterSegment.get_class(structure[SEGMENT_TYPE_TAG])
+            else:
+                segment_class = None
             for key, value in structure.items():
                 if key in [
                     NAME_TAG,
                     TYPE_TAG,
                     SEGMENT_TYPE_TAG,
                     PARTS_TAG,
                     CLIMB_PARTS_TAG,
@@ -208,169 +210,210 @@
                     part_identifier=part_identifier,
                     segment_class=segment_class,
                 )
             return structure
 
         # Here structure is not a dict, hence a directly given value.
         key, value = parent, structure
-        input_definition = InputDefinition(key, value, part_identifier=part_identifier)
+        if key == POLAR_TAG:
+            return None
+        input_definition = InputDefinition(
+            key, value, part_identifier=part_identifier, prefix=self.variable_prefix
+        )
         if segment_class and isinstance(value, str):
             input_definition.shape_by_conn = self._is_shape_by_conn(key, segment_class)
         input_definitions.append(input_definition)
         return input_definition
 
     @staticmethod
     def _is_shape_by_conn(key, segment_class) -> bool:
         """
         Here variables that are expected to be arrays or lists in the provided segment class are
         attributed the "shape_by_conn=True" property.
         """
         segment_fields = [fld for fld in fields(segment_class) if fld.name == key]
         return len(segment_fields) == 1 and issubclass(segment_fields[0].type, (list, np.ndarray))
 
-    @staticmethod
-    def _process_polar(polar_structure):
+    def _process_polar(self, structure):
         """
-        Polar data are handled specifically, as it a particular parameter of segments (
+        Polar data are handled specifically, as it is a particular parameter of segments (
         a Polar class).
 
         If "foo:bar:baz" is provided as `polar_structure`, it is replaced by the dict
         { "CL": {value:"foo:bar:baz:CL", "shape_by_conn": True},
           "CD": {value:"foo:bar:baz:CD", "shape_by_conn": True}}
 
         Also, even if `polar_structure` is a dict, it is ensured that it has the structure above.
         """
 
-        if isinstance(polar_structure, str):
-            polar_structure = OrderedDict(
-                {
-                    "CL": {"value": polar_structure + ":CL", "shape_by_conn": True},
-                    "CD": {"value": polar_structure + ":CD", "shape_by_conn": True},
-                }
+        if POLAR_TAG in structure:
+            builder = PolarStructureBuilder(
+                structure[POLAR_TAG], "", self.qualified_name, self.variable_prefix
             )
-        elif isinstance(polar_structure, dict):
-            for key in ["CL", "CD"]:
-                if isinstance(polar_structure[key], str):
-                    polar_structure[key] = {"value": polar_structure[key], "shape_by_conn": True}
-                elif isinstance(polar_structure[key], dict):
-                    polar_structure[key]["shape_by_conn"] = True
-
-        return polar_structure
+            structure[POLAR_TAG] = self.process_builder(builder)
 
 
 class DefaultStructureBuilder(AbstractStructureBuilder):
     """
     Builder for structures that do not need to process the given definition.
 
     :param definition: the definition for the part only
     """
 
-    def _build(self, definition: dict) -> OrderedDict:
-        return OrderedDict(deepcopy(definition))
+    def _build(self, definition: dict) -> dict:
+        return deepcopy(definition)
+
+
+class PolarStructureBuilder(AbstractStructureBuilder, structure_type=POLAR_TAG):
+    """
+    Structure builder for polar definition.
+
+    :param definition: the definition for the polar only
+    """
+
+    def _build(self, definition: dict) -> dict:
+        polar_structure = {}
+        if isinstance(definition, str):
+            polar_structure = {
+                "CL": {"value": definition + ":CL", "shape_by_conn": True},
+                "CD": {"value": definition + ":CD", "shape_by_conn": True},
+            }
+
+        elif isinstance(definition, dict):
+            polar_structure = deepcopy(definition)
+            for key in ["CL", "CD", "alpha"]:
+                if key in polar_structure:
+                    if isinstance(polar_structure[key], str):
+                        polar_structure[key] = {
+                            "value": polar_structure[key],
+                            "shape_by_conn": True,
+                        }
+                    elif isinstance(polar_structure[key], dict):
+                        polar_structure[key]["shape_by_conn"] = True
+
+        return polar_structure
 
 
 class SegmentStructureBuilder(AbstractStructureBuilder, structure_type=SEGMENT_TAG):
     """
     Structure builder for segment definition.
 
     :param definition: the definition for the segment only
     """
 
-    def _build(self, definition: dict) -> OrderedDict:
-        segment_structure = OrderedDict(deepcopy(definition))
+    def _build(self, definition: dict) -> dict:
+        segment_structure = deepcopy(definition)
         del segment_structure[SEGMENT_TAG]
         segment_structure[SEGMENT_TYPE_TAG] = definition[SEGMENT_TAG]
 
         return segment_structure
 
 
 class PhaseStructureBuilder(AbstractStructureBuilder, structure_type=PHASE_TAG):
     """
     Structure builder for phase definition.
 
     :param definition: the whole content of definition file
     """
 
-    def _build(self, definition: dict) -> OrderedDict:
+    def _build(self, definition: dict) -> dict:
         phase_definition = definition[PHASE_DEFINITIONS_TAG][self.name]
-        phase_structure = OrderedDict(deepcopy(phase_definition))
+        phase_structure = deepcopy(phase_definition)
 
         for i, part in enumerate(phase_definition[PARTS_TAG]):
             if PHASE_TAG in part:
-                builder = PhaseStructureBuilder(definition, part[PHASE_TAG], self.qualified_name)
+                builder = PhaseStructureBuilder(
+                    definition, part[PHASE_TAG], self.qualified_name, self.variable_prefix
+                )
             elif SEGMENT_TAG in part:
-                builder = SegmentStructureBuilder(part, "", self.qualified_name)
+                builder = SegmentStructureBuilder(
+                    part, "", self.qualified_name, self.variable_prefix
+                )
             else:
                 raise RuntimeError(f"Unexpected structure in definition of phase {self.name}")
 
-            phase_structure[PARTS_TAG][i] = {}
             phase_structure[PARTS_TAG][i] = self.process_builder(builder)
 
         return phase_structure
 
 
 class RouteStructureBuilder(AbstractStructureBuilder, structure_type=ROUTE_TAG):
     """
     Structure builder for route definition.
 
     :param definition: the whole content of definition file
     """
 
-    def _build(self, definition: dict) -> OrderedDict:
+    def _build(self, definition: dict) -> dict:
         route_definition = definition[ROUTE_DEFINITIONS_TAG][self.name]
-        route_structure = OrderedDict(deepcopy(route_definition))
+        route_structure = deepcopy(route_definition)
 
         route_structure[CLIMB_PARTS_TAG] = self._get_route_climb_or_descent_structure(
             definition, route_definition[CLIMB_PARTS_TAG]
         )
 
         builder = SegmentStructureBuilder(
-            route_definition[CRUISE_PART_TAG], "cruise", self.qualified_name
+            route_definition[CRUISE_PART_TAG], "cruise", self.qualified_name, self.variable_prefix
         )
         route_structure[CRUISE_PART_TAG] = self.process_builder(builder)
 
         route_structure[DESCENT_PARTS_TAG] = self._get_route_climb_or_descent_structure(
             definition, route_definition[DESCENT_PARTS_TAG]
         )
 
+        if POLAR_TAG in route_structure:
+            builder = PolarStructureBuilder(
+                route_structure[POLAR_TAG], "", self.qualified_name, self.variable_prefix
+            )
+            route_structure[POLAR_TAG] = self.process_builder(builder)
         return route_structure
 
     def _get_route_climb_or_descent_structure(self, global_definition, parts_definition):
         parts = []
         for part_definition in parts_definition:
             phase_name = part_definition["phase"]
-            builder = PhaseStructureBuilder(global_definition, phase_name, self.qualified_name)
+            builder = PhaseStructureBuilder(
+                global_definition, phase_name, self.qualified_name, self.variable_prefix
+            )
             phase_structure = self.process_builder(builder)
             parts.append(phase_structure)
         return parts
 
 
 class MissionStructureBuilder(AbstractStructureBuilder, structure_type="mission"):
     """
     Structure builder for mission definition.
 
     :param definition: the whole content of definition file
     """
 
-    def _build(self, definition: dict) -> OrderedDict:
+    def _build(self, definition: dict) -> dict:
         mission_definition = definition[MISSION_DEFINITION_TAG][self.name]
-        mission_structure = OrderedDict(deepcopy(mission_definition))
+        mission_structure = deepcopy(mission_definition)
 
         mission_parts = []
         for part_definition in mission_definition[PARTS_TAG]:
             if ROUTE_TAG in part_definition:
                 route_name = part_definition[ROUTE_TAG]
-                builder = RouteStructureBuilder(definition, route_name, self.qualified_name)
+                builder = RouteStructureBuilder(
+                    definition, route_name, self.qualified_name, self.variable_prefix
+                )
             elif PHASE_TAG in part_definition:
                 phase_name = part_definition[PHASE_TAG]
-                builder = PhaseStructureBuilder(definition, phase_name, self.qualified_name)
+                builder = PhaseStructureBuilder(
+                    definition, phase_name, self.qualified_name, self.variable_prefix
+                )
             elif SEGMENT_TAG in part_definition:
-                builder = SegmentStructureBuilder(part_definition, "", self.qualified_name)
+                builder = SegmentStructureBuilder(
+                    part_definition, "", self.qualified_name, self.variable_prefix
+                )
             else:
-                builder = DefaultStructureBuilder(part_definition, "", self.qualified_name)
+                builder = DefaultStructureBuilder(
+                    part_definition, "", self.qualified_name, self.variable_prefix
+                )
 
             part_structure = self.process_builder(builder)
             mission_parts.append(part_structure)
 
         mission_structure[PARTS_TAG] = mission_parts
 
         return mission_structure
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944256136096414%*

 * *Differences: {"'definitions'": "{'polar': {'properties': {'CL': {'$ref': '#/definitions/polar_value'}, 'CD': "*

 * *                  "{'$ref': '#/definitions/polar_value'}, 'alpha': OrderedDict([('$ref', "*

 * *                  "'#/definitions/polar_value')]), 'modifier': OrderedDict([('type', ['string', "*

 * *                  "'object']), ('properties', OrderedDict([('name', OrderedDict([('$ref', "*

 * *                  "'#/definitions/string_parameter_value')])), ('additionalProperties', "*

 * *                  "True)]))])}}, 'base_part […]*

```diff
@@ -1,21 +1,12 @@
 {
     "$id": "http://example.com/product.schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "definitions": {
-        "CL_CD": {
-            "items": {
-                "type": "number"
-            },
-            "type": [
-                "string",
-                "array"
-            ]
-        },
         "base_part": {
             "properties": {
                 "climb_thrust_rate": {
                     "$ref": "#/definitions/parameter_value_without_unit"
                 },
                 "engine_setting": {
                     "$ref": "#/definitions/string_parameter_value"
@@ -25,14 +16,17 @@
                 },
                 "maximum_flight_level": {
                     "$ref": "#/definitions/parameter_value_without_unit"
                 },
                 "polar": {
                     "$ref": "#/definitions/polar"
                 },
+                "polar_modifier": {
+                    "$ref": "#/definitions/polar_modifier"
+                },
                 "reserve_mass_ratio": {
                     "$ref": "#/definitions/parameter_value_without_unit"
                 },
                 "thrust_rate": {
                     "$ref": "#/definitions/parameter_value_without_unit"
                 },
                 "time_step": {
@@ -111,14 +105,20 @@
                             },
                             {
                                 "$ref": "#/definitions/mission_reserve"
                             }
                         ]
                     },
                     "type": "array"
+                },
+                "target_fuel_consumption": {
+                    "$ref": "#/definitions/parameter_value_with_unit"
+                },
+                "use_all_block_fuel": {
+                    "$ref": "#/definitions/boolean_parameter_value"
                 }
             },
             "required": [
                 "parts"
             ],
             "type": "object"
         },
@@ -246,29 +246,53 @@
             ],
             "description": "Specification of a flight phase"
         },
         "polar": {
             "additionalProperties": false,
             "properties": {
                 "CD": {
-                    "$ref": "#/definitions/CL_CD"
+                    "$ref": "#/definitions/polar_value"
                 },
                 "CL": {
-                    "$ref": "#/definitions/CL_CD"
+                    "$ref": "#/definitions/polar_value"
+                },
+                "alpha": {
+                    "$ref": "#/definitions/polar_value"
+                },
+                "modifier": {
+                    "properties": {
+                        "additionalProperties": true,
+                        "name": {
+                            "$ref": "#/definitions/string_parameter_value"
+                        }
+                    },
+                    "type": [
+                        "string",
+                        "object"
+                    ]
                 }
             },
             "required": [
                 "CL",
                 "CD"
             ],
             "type": [
                 "string",
                 "object"
             ]
         },
+        "polar_value": {
+            "items": {
+                "type": "number"
+            },
+            "type": [
+                "string",
+                "array"
+            ]
+        },
         "route": {
             "additionalProperties": false,
             "properties": {
                 "climb_parts": {
                     "$ref": "#/definitions/route_parts",
                     "description": "Flight phases before cruise"
                 },
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/mission_definition/schema.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,29 +72,36 @@
             data = yaml.load(yaml_file)
 
         with open_text(resources, JSON_SCHEMA_NAME) as json_file:
             json_schema = json.loads(json_file.read())
         validate(data, json_schema)
 
         self._validate(data)
+        self._convert_none_values(data)
+
         self.update(data)
 
+        for mission_name in self[MISSION_DEFINITION_TAG]:
+            if self[MISSION_DEFINITION_TAG][mission_name].get("use_all_block_fuel"):
+                self.force_all_block_fuel_usage(mission_name)
+
+    def force_all_block_fuel_usage(self, mission_name):
+        """Sets target fuel consumption to variable "~:block_fuel"."""
+        mission_definitions = self[MISSION_DEFINITION_TAG]
+        if mission_name in mission_definitions:
+            mission_definitions[mission_name]["target_fuel_consumption"] = {
+                "value": "~:block_fuel",
+                "unit": "kg",
+            }
+
     @classmethod
     def _validate(cls, content: dict):
         """
         Does a second pass validation of file content.
 
-        Also applies thess features:
-            * None values are set back to "~".
-            *       - polar: foo:bar
-                is translated to:
-                    - polar:
-                        CL: foo:bar:CL
-                        CD: foo:bar:CD
-
         Errors are raised if file content is incorrect.
 
         :param content:
         """
         phase_names = set(content[PHASE_DEFINITIONS_TAG].keys())
 
         if ROUTE_DEFINITIONS_TAG in content:
@@ -116,16 +123,14 @@
                     reserve_count += 1
                     Ensure(value["ref"]).is_in(content[ROUTE_DEFINITIONS_TAG].keys())
             Ensure(reserve_count).is_less_than_or_equal_to(1)
             if reserve_count == 1:
                 # reserve definition should be the last part
                 Ensure(part_type).equals(RESERVE_TAG)
 
-        cls._convert_none_values(content)
-
     @classmethod
     def _convert_none_values(cls, struct: Union[dict, list]):
         """
         Recursively transforms any None value in struct to "~"
         """
         if isinstance(struct, dict):
             for key, value in struct.items():
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/link_mtow.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/link_mtow.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,54 @@
 """
 FAST-OAD model for mission computation.
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
-from importlib.resources import path
+from enum import EnumMeta
 
+import numpy as np
 import openmdao.api as om
 import pandas as pd
 
 from fastoad.module_management.constants import ModelDomain
 from fastoad.module_management.service_registry import RegisterOpenMDAOSystem
-from . import resources
-from .mission_component import MissionComponent, _get_variable_name_provider
-from .mission_wrapper import MissionWrapper
-from ..mission_definition.schema import MissionDefinition
+from .base import BaseMissionComp, NeedsOWE
+from .mission_run import AdvancedMissionComp
 
 _LOGGER = logging.getLogger(__name__)  # Logger for this module
 
 
 @RegisterOpenMDAOSystem("fastoad.performances.mission", domain=ModelDomain.PERFORMANCE)
-class Mission(om.Group):
+class OMMission(om.Group, BaseMissionComp, NeedsOWE):
     """
     Computes a mission as specified in mission input file.
     """
 
     def initialize(self):
-        self.options.declare(
-            "propulsion_id",
-            default="",
-            types=str,
-            desc="(mandatory) The identifier of the propulsion wrapper.",
-        )
+        super().initialize()
         self.options.declare(
             "out_file",
             default="",
             types=str,
             desc="If provided, a csv file will be written at provided path with all computed "
             "flight points.",
         )
         self.options.declare(
-            "mission_file_path",
-            default="::sizing_mission",
-            types=(str, MissionDefinition),
-            allow_none=True,
-            desc="The path to file that defines the mission.\n"
-            'If can also begin with two colons "::" to use pre-defined missions:\n'
-            '  - "::sizing_mission" : design mission for CeRAS-01\n'
-            '  - "::breguet" : a simple mission with Breguet formula for cruise, and input\n'
-            "    coefficients for fuel reserve and fuel consumption during climb and descent",
-        )
-        self.options.declare(
-            "mission_name",
-            default=None,
-            types=str,
-            allow_none=True,
-            desc="The mission name. Required if mission file defines several missions.",
-        )
-        self.options.declare(
             "use_initializer_iteration",
             default=True,
             types=bool,
             desc="During first solver loop, a complete mission computation can fail or consume "
             "useless CPU-time.\n"
             "When activated, this option ensures the first iteration is done using a simple,\n"
             "dummy, formula instead of the specified mission.\n"
@@ -93,18 +69,19 @@
             types=bool,
             desc="If True, input weight will be deduced from block fuel.\n"
             "If False, block fuel will be deduced from input weight.\n"
             "Not used (actually forced to True) if adjust_fuel is True.",
         )
         self.options.declare(
             "compute_TOW",
-            default=False,
+            default=None,
             types=bool,
-            desc="(Deprecated. Replaced by compute_input_weight)\n"
-            "If True, TakeOff Weight will be computed from onboard fuel at takeoff and ZFW.\n"
+            deprecation='Option "compute_TOW" is deprecated for mission module. '
+            'Please use "compute_input_weight" instead.',
+            desc="If True, TakeOff Weight will be computed from onboard fuel at takeoff and ZFW.\n"
             "If False, block fuel will be computed from ramp weight and ZFW.\n"
             "Not used (actually forced to True) if adjust_fuel is True.",
         )
         self.options.declare(
             "add_solver",
             default=False,
             types=bool,
@@ -117,137 +94,183 @@
         self.options.declare(
             "is_sizing",
             default=False,
             types=bool,
             desc="If True, TOW will be considered equal to MTOW and mission payload will be "
             "considered equal to design payload.",
         )
-        self.options.declare(
-            "reference_area_variable",
-            default="data:geometry:wing:area",
-            types=str,
-            desc="Defines the name of the variable for providing aircraft reference surface area.",
-        )
 
     def setup(self):
-        self.options["compute_input_weight"] = self.options["compute_TOW"]
+        super().setup()
 
-        if "::" in self.options["mission_file_path"]:
-            # The configuration file parser will have added the working directory before
-            # the file name. But as the user-provided string begins with "::", we just
-            # have to ignore all before "::".
-            i = self.options["mission_file_path"].index("::")
-            file_name = self.options["mission_file_path"][i + 2 :] + ".yml"
-            with path(resources, file_name) as mission_input_file:
-                self.options["mission_file_path"] = MissionDefinition(mission_input_file)
-        self._mission_wrapper = MissionWrapper(self.options["mission_file_path"])
-        if self.options["mission_name"] is None:
-            self.options["mission_name"] = self._mission_wrapper.get_unique_mission_name()
+        if self.options["compute_TOW"] is not None:
+            self.options["compute_input_weight"] = self.options["compute_TOW"]
 
-        mission_name = self.options["mission_name"]
-        self._name_provider = _get_variable_name_provider(mission_name)
+        mission_options = {
+            key: val for key, val in self.options.items() if key in AdvancedMissionComp().options
+        }
+        mission_component = AdvancedMissionComp(**mission_options)
 
-        self.add_subsystem("ZFW_computation", self._get_zfw_component(mission_name), promotes=["*"])
+        self.add_subsystem("ZFW_computation", self._get_zfw_component(), promotes=["*"])
 
         if self.options["adjust_fuel"]:
             self.options["compute_input_weight"] = True
             self.connect(
-                self._name_provider.NEEDED_BLOCK_FUEL.value,
-                self._name_provider.BLOCK_FUEL.value,
+                self.name_provider.NEEDED_BLOCK_FUEL.value,
+                self.name_provider.BLOCK_FUEL.value,
             )
         if self.options["add_solver"]:
             self.nonlinear_solver = om.NonlinearBlockGS(maxiter=30, rtol=1.0e-4, iprint=0)
             self.linear_solver = om.DirectSolver()
 
         if self.options["compute_input_weight"]:
             self.add_subsystem(
                 "input_mass_computation",
-                self._get_input_weight_component(mission_name),
+                self._get_input_weight_component(),
                 promotes=["*"],
             )
 
-        mission_options = dict(self.options.items())
-        del mission_options["adjust_fuel"]
-        del mission_options["compute_input_weight"]
-        del mission_options["compute_TOW"]
-        del mission_options["add_solver"]
-        del mission_options["mission_file_path"]
-        mission_options["mission_wrapper"] = self._mission_wrapper
-        mission_options["mission_name"] = mission_name
-
-        self.add_subsystem(
-            "mission_computation", MissionComponent(**mission_options), promotes=["*"]
-        )
+        self.add_subsystem("mission_computation", mission_component, promotes=["*"])
         if not self.options["compute_input_weight"]:
             self.add_subsystem(
                 "block_fuel_computation",
-                self._get_block_fuel_component(mission_name),
+                self._get_block_fuel_component(),
                 promotes=["*"],
             )
 
+        self.add_subsystem(
+            "specific_burned_fuel",
+            SpecificBurnedFuelComputation(
+                name_provider=self.name_provider,
+                mission_name=self.mission_name,
+                first_route_name=self.first_route_name,
+                payload_variable=self._get_payload_variable(),
+            ),
+            promotes=["*"],
+        )
+
     @property
     def flight_points(self) -> pd.DataFrame:
         """Dataframe that lists all computed flight point data."""
         return self.mission_computation.flight_points
 
-    def _get_zfw_component(self, mission_name: str) -> om.AddSubtractComp:
+    def _get_zfw_component(self) -> om.AddSubtractComp:
         """
 
-        :param mission_name:
         :return: component that computes Zero Fuel Weight from OWE and mission payload
         """
-        if self.options["is_sizing"]:
-            payload_var = "data:weight:aircraft:payload"
-        else:
-            payload_var = self._name_provider.PAYLOAD.value
+        payload_var = self._get_payload_variable()
 
         zfw_computation = om.AddSubtractComp()
         zfw_computation.add_equation(
-            self._name_provider.ZFW.value,
-            ["data:weight:aircraft:OWE", payload_var],
+            self.name_provider.ZFW.value,
+            [self.options["OWE_variable"], payload_var],
             units="kg",
-            desc=f'Zero Fuel Weight for mission "{mission_name}"',
+            desc=f'Zero Fuel Weight for mission "{self.mission_name}"',
         )
         return zfw_computation
 
-    def _get_input_weight_component(self, mission_name: str):
-        input_weight_variable = self._mission_wrapper.get_input_weight_variable_name(mission_name)
+    def _get_input_weight_component(self):
+        """
+
+        :return: component that computes input weight
+        """
+        input_weight_variable = self._mission_wrapper.get_input_weight_variable_name(
+            self.mission_name
+        )
         if not input_weight_variable:
             return None
 
         computation = om.AddSubtractComp()
         computation.add_equation(
             output_name=input_weight_variable,
             input_names=[
-                self._name_provider.ZFW.value,
-                self._name_provider.BLOCK_FUEL.value,
-                self._name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
+                self.name_provider.ZFW.value,
+                self.name_provider.BLOCK_FUEL.value,
+                self.name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
             ],
             units="kg",
             scaling_factors=[1, 1, -1],
-            desc=f'Loaded fuel at beginning for mission "{mission_name}"',
+            desc=f'Loaded fuel at beginning for mission "{self.mission_name}"',
         )
 
         return computation
 
-    def _get_block_fuel_component(self, mission_name: str) -> om.AddSubtractComp:
+    def _get_block_fuel_component(self) -> om.AddSubtractComp:
         """
 
-        :param mission_name:
         :return: component that computes block fuel from ramp weight and ZFW
         """
-        input_weight_variable = self._mission_wrapper.get_input_weight_variable_name(mission_name)
+        input_weight_variable = self._mission_wrapper.get_input_weight_variable_name(
+            self.mission_name
+        )
 
         block_fuel_computation = om.AddSubtractComp()
         block_fuel_computation.add_equation(
             output_name=self._name_provider.BLOCK_FUEL.value,
             input_names=[
                 input_weight_variable,
-                self._name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
-                self._name_provider.ZFW.value,
+                self.name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
+                self.name_provider.ZFW.value,
             ],
             units="kg",
             scaling_factors=[1, 1, -1],
-            desc=f'Loaded fuel at beginning for mission "{mission_name}"',
+            desc=f'Loaded fuel at beginning for mission "{self.mission_name}"',
         )
 
         return block_fuel_computation
+
+    def _get_payload_variable(self):
+        if self.options["is_sizing"]:
+            return "data:weight:aircraft:payload"
+
+        return self.name_provider.PAYLOAD.value
+
+
+class SpecificBurnedFuelComputation(
+    om.ExplicitComponent,
+):
+    """Computation of specific burned fuel (mission fuel / payload / mission range)."""
+
+    def initialize(self):
+        self.options.declare("name_provider", types=EnumMeta)
+        self.options.declare("mission_name", types=str)
+        self.options.declare("first_route_name", types=str)
+        self.options.declare("payload_variable", types=str)
+
+    @property
+    def range_variable(self):
+        """Name of range variable."""
+        return (
+            "data:mission:"
+            f"{self.options['mission_name']}:{self.options['first_route_name']}:"
+            "distance"
+        )
+
+    @property
+    def burned_fuel_variable(self):
+        """Name of burned fuel variable."""
+        return self.options["name_provider"].NEEDED_BLOCK_FUEL.value
+
+    @property
+    def specific_burned_fuel_variable(self):
+        """Name of specific burned fuel variable (mission fuel / payload / mission range)."""
+        return self.options["name_provider"].SPECIFIC_BURNED_FUEL.value
+
+    @property
+    def payload_variable(self):
+        """Name of payload variable."""
+        return self.options["payload_variable"]
+
+    def setup(self):
+        self.add_input(self.payload_variable, units="kg")
+        self.add_input(self.burned_fuel_variable, val=np.nan, units="kg")
+        self.add_input(self.range_variable, val=np.nan, units="NM")
+        self.add_output(self.specific_burned_fuel_variable, units="NM**-1")
+
+    def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
+        burned_fuel = inputs[self.burned_fuel_variable]
+        # Denominators may be null at first iterations, so we avoid that.
+        payload = np.maximum(1.0, inputs[self.payload_variable])
+        mission_range = np.maximum(1.0, inputs[self.range_variable])
+
+        outputs[self.specific_burned_fuel_variable] = burned_fuel / payload / mission_range
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission_component.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,214 @@
-"""
-OpenMDAO component for time-step computation of missions.
-"""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
-from enum import Enum
 from os import makedirs, path as pth
+from typing import Optional
 
 import numpy as np
 from openmdao import api as om
 
 from fastoad.model_base import FlightPoint
 from fastoad.model_base.propulsion import IOMPropulsionWrapper
-from fastoad.models.performances.mission.openmdao.mission_wrapper import MissionWrapper
-from fastoad.models.performances.mission.polar import Polar
-from fastoad.models.performances.mission.segments.cruise import BreguetCruiseSegment
 from fastoad.module_management.service_registry import RegisterPropulsion
+from .base import BaseMissionComp
+from ..polar import Polar
+from ..segments.registered.cruise import BreguetCruiseSegment
 
 _LOGGER = logging.getLogger(__name__)  # Logger for this module
 
 
-class MissionComponent(om.ExplicitComponent):
+class MissionComp(om.ExplicitComponent, BaseMissionComp):
     """
-    Computes a mission as specified in mission input file
-
-    Options:
-      - propulsion_id: (mandatory) the identifier of the propulsion wrapper.
-      - out_file: if provided, a csv file will be written at provided path with all computed
-                  flight points.
-      - mission_wrapper: the MissionWrapper instance that defines the mission.
-      - use_initializer_iteration: During first solver loop, a complete mission computation can
-                                   fail or consume useless CPU-time. When activated, this option
-                                   ensures the first iteration is done using a simple, dummy,
-                                   formula instead of the specified mission.
-                                   Set this option to False if you do expect this model to be
-                                   computed only once.
-      - is_sizing: if True, TOW will be considered equal to MTOW and mission payload will be
-                   considered equal to design payload.
-      - reference_area_variable: Defines the name of the variable for providing aircraft
-                                 reference surface area.
+    Computes a mission as specified in mission input file.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.flight_points = None
-        self._engine_wrapper = None
-        self._mission_wrapper: MissionWrapper = None
-        self._name_provider = None
         self._input_weight_variable_name = ""
+        self._engine_wrapper = None
 
     def initialize(self):
-        self.options.declare("propulsion_id", default="", types=str)
-        self.options.declare("out_file", default="", types=str)
-        self.options.declare("use_initializer_iteration", default=True, types=bool)
-        self.options.declare("mission_wrapper", types=MissionWrapper)
-        self.options.declare("mission_name", types=str)
-        self.options.declare("is_sizing", default=False, types=bool)
+        super().initialize()
         self.options.declare(
-            "reference_area_variable", default="data:geometry:wing:area", types=str
+            "out_file",
+            default="",
+            types=str,
+            desc="if provided, a csv file will be written at provided path with "
+            "all computed flight points.",
         )
 
     def setup(self):
-        self._engine_wrapper = self._get_engine_wrapper()
+        super().setup()
+
+        self._engine_wrapper = self.get_engine_wrapper()
         self._engine_wrapper.setup(self)
-        self._mission_wrapper = self.options["mission_wrapper"]
-        self._mission_wrapper.setup(self, self.options["mission_name"])
 
-        mission_name = self.options["mission_name"]
+        self._mission_wrapper.setup(self)
 
-        self._name_provider = _get_variable_name_provider(mission_name)
         self._input_weight_variable_name = self._mission_wrapper.get_input_weight_variable_name(
-            self.options["mission_name"]
+            self.mission_name
         )
 
         try:
             self.add_input(self.options["reference_area_variable"], np.nan, units="m**2")
         except ValueError:
             pass
 
         # Global mission outputs
         self.add_output(
-            self._name_provider.NEEDED_BLOCK_FUEL.value,
+            self.name_provider.NEEDED_BLOCK_FUEL.value,
             units="kg",
-            desc=f'Needed fuel to complete mission "{mission_name}", including reserve fuel',
+            desc=f'Needed fuel to complete mission "{self.mission_name}", including reserve fuel',
         )
         self.add_output(
-            self._name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
+            self.name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value,
             units="kg",
-            desc=f'consumed fuel quantity before target mass defined for "{mission_name}",'
+            desc=f'consumed fuel quantity before target mass defined for "{self.mission_name}",'
             f" if any (e.g. TakeOff Weight)",
         )
-        if self.options["is_sizing"]:
-            self.add_output("data:weight:aircraft:sizing_block_fuel", units="kg")
-            self.add_output("data:weight:aircraft:sizing_onboard_fuel_at_input_weight", units="kg")
 
     def setup_partials(self):
         self.declare_partials(["*"], ["*"], method="fd")
 
     def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
+        propulsion_model = self._engine_wrapper.get_model(inputs)
+        reference_area = inputs[self.options["reference_area_variable"]]
+
+        self._mission_wrapper.propulsion = propulsion_model
+        self._mission_wrapper.reference_area = reference_area
+
+        # This is the default start point, that can be overridden by using the "start"
+        # segment in the mission definition.
+        start_flight_point = FlightPoint(
+            altitude=0.0, mass=inputs[self._input_weight_variable_name], true_airspeed=0.0
+        )
+
+        self.flight_points = self._mission_wrapper.compute(start_flight_point, inputs, outputs)
+
+        self._compute_outputs(outputs, self.flight_points)
+
+        self._postprocess_flight_points(self.flight_points)
+
+    def _postprocess_flight_points(self, flight_points):
+        def as_scalar(value):
+            if isinstance(value, np.ndarray):
+                return value.item()
+            return value
+
+        flight_points = flight_points.applymap(as_scalar)
+        rename_dict = {
+            field_name: f"{field_name} [{unit}]"
+            for field_name, unit in FlightPoint.get_units().items()
+        }
+        flight_points.rename(columns=rename_dict, inplace=True)
+        if self.options["out_file"]:
+            makedirs(pth.dirname(self.options["out_file"]), exist_ok=True)
+            flight_points.to_csv(self.options["out_file"])
+
+        return flight_points
+
+    def _compute_outputs(self, outputs, flight_points):
+        # Final ================================================================
+        start_of_mission = FlightPoint.create(flight_points.iloc[0])
+        end_of_mission = FlightPoint.create(flight_points.iloc[-1])
+        outputs[self.name_provider.NEEDED_BLOCK_FUEL.value] = (
+            start_of_mission.mass - end_of_mission.mass
+        )
+        reserve_var_name = self._mission_wrapper.get_reserve_variable_name()
+        if reserve_var_name in outputs:
+            outputs[self.name_provider.NEEDED_BLOCK_FUEL.value] += outputs[
+                self._mission_wrapper.get_reserve_variable_name()
+            ]
+        outputs[
+            self.name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value
+        ] = self._mission_wrapper.consumed_fuel_before_input_weight
+
+    def get_engine_wrapper(self) -> Optional[IOMPropulsionWrapper]:
+        """
+        Overloading this method allows to define the engine without relying on the propulsion
+        option.
+
+        (useful for tests)
+
+        :return: the engine wrapper instance
+        """
+        if self.options["propulsion_id"]:
+            return RegisterPropulsion.get_provider(self.options["propulsion_id"])
+
+        return None
+
+
+class AdvancedMissionComp(MissionComp):
+    """
+    Computes a mission as specified in mission input file.
+
+    Compared to :class:`MissionComp`, it allows:
+        - to use an initializer iteration (simple Breguet) at first call.
+        - to use the mission as the design mission for the sizing process.
+    """
+
+    def initialize(self):
+        super().initialize()
+        self.options.declare("use_initializer_iteration", default=True, types=bool)
+        self.options.declare("is_sizing", default=False, types=bool)
+
+    def setup(self):
+        super().setup()
+
+        if self.options["is_sizing"]:
+            self.add_output("data:weight:aircraft:sizing_block_fuel", units="kg")
+            self.add_output("data:weight:aircraft:sizing_onboard_fuel_at_input_weight", units="kg")
+
+    def compute(self, inputs, outputs, discrete_inputs=None, discrete_outputs=None):
         iter_count = self.iter_count_without_approx
         message_prefix = f"Mission computation - iteration {iter_count:d} : "
         if iter_count == 0 and self.options["use_initializer_iteration"]:
             _LOGGER.info(
                 "%sUsing initializer computation. OTHER ITERATIONS NEEDED.", message_prefix
             )
             self._compute_breguet(inputs, outputs)
         else:
             _LOGGER.info("%sUsing mission definition.", message_prefix)
-            self._compute_mission(inputs, outputs)
+            super().compute(inputs, outputs, discrete_inputs, discrete_outputs)
+            if self.options["is_sizing"]:
+                outputs["data:weight:aircraft:sizing_block_fuel"] = outputs[
+                    self.name_provider.NEEDED_BLOCK_FUEL.value
+                ]
+                outputs["data:weight:aircraft:sizing_onboard_fuel_at_input_weight"] = (
+                    outputs[self.name_provider.NEEDED_BLOCK_FUEL.value]
+                    - self._mission_wrapper.consumed_fuel_before_input_weight
+                )
 
     def _compute_breguet(self, inputs, outputs):
         """
         Computes mission using simple Breguet formula at altitude==100m and Mach 0.1
         (but max L/D ratio is assumed anyway)
 
         Useful only for initiating the computation.
 
         :param inputs: OpenMDAO input vector
         :param outputs: OpenMDAO output vector
         """
         propulsion_model = self._engine_wrapper.get_model(inputs)
 
         high_speed_polar = self._get_initial_polar(inputs)
-        distance = np.sum(
-            self._mission_wrapper.get_route_ranges(inputs, self.options["mission_name"])
-        ).item()
+        distance = np.sum(self._mission_wrapper.get_route_ranges(inputs)).item()
 
         altitude = 100.0
         cruise_mach = 0.1
 
         breguet = BreguetCruiseSegment(
             target=FlightPoint(ground_distance=distance),
             propulsion=propulsion_model,
@@ -149,15 +218,15 @@
         start_point = FlightPoint(
             mass=inputs[self._input_weight_variable_name],
             altitude=altitude,
             mach=cruise_mach,
         )
         flight_points = breguet.compute_from(start_point)
         end_point = FlightPoint.create(flight_points.iloc[-1])
-        outputs[self._name_provider.NEEDED_BLOCK_FUEL.value] = start_point.mass - end_point.mass
+        outputs[self.name_provider.NEEDED_BLOCK_FUEL.value] = start_point.mass - end_point.mass
 
     @staticmethod
     def _get_initial_polar(inputs) -> Polar:
         """
         At computation start, polar may be irrelevant and give a very low lift/drag ratio.
 
         In that case, this method returns a fake polar that has 10.0 as max lift drag ratio.
@@ -177,99 +246,7 @@
         except ZeroDivisionError:
             use_minimum_l_d_ratio = True
         if use_minimum_l_d_ratio:
             # We replace by a polar that has at least 10.0 as max L/D ratio
             high_speed_polar = Polar(np.array([0.0, 0.5, 1.0]), np.array([0.1, 0.05, 1.0]))
 
         return high_speed_polar
-
-    def _compute_mission(self, inputs, outputs):
-        """
-        Computes mission using time-step integration.
-
-        :param inputs: OpenMDAO input vector
-        :param outputs: OpenMDAO output vector
-        """
-        propulsion_model = self._engine_wrapper.get_model(inputs)
-        reference_area = inputs[self.options["reference_area_variable"]]
-
-        self._mission_wrapper.propulsion = propulsion_model
-        self._mission_wrapper.reference_area = reference_area
-
-        # This is the default start point, that can be overridden by using the "start"
-        # segment in the mission definition.
-        start_flight_point = FlightPoint(
-            altitude=0.0, mass=inputs[self._input_weight_variable_name], true_airspeed=0.0
-        )
-
-        self.flight_points = self._mission_wrapper.compute(start_flight_point, inputs, outputs)
-
-        # Final ================================================================
-        start_of_mission = FlightPoint.create(self.flight_points.iloc[0])
-        end_of_mission = FlightPoint.create(self.flight_points.iloc[-1])
-        reserve = self._mission_wrapper.get_reserve(
-            self.flight_points, self.options["mission_name"]
-        )
-        reserve_name = self._mission_wrapper.get_reserve_variable_name()
-        if reserve_name in outputs:
-            outputs[reserve_name] = reserve
-        outputs[self._name_provider.NEEDED_BLOCK_FUEL.value] = (
-            start_of_mission.mass - end_of_mission.mass + reserve
-        )
-
-        outputs[
-            self._name_provider.CONSUMED_FUEL_BEFORE_INPUT_WEIGHT.value
-        ] = self._mission_wrapper.consumed_fuel_before_input_weight
-
-        if self.options["is_sizing"]:
-            outputs["data:weight:aircraft:sizing_block_fuel"] = outputs[
-                self._name_provider.NEEDED_BLOCK_FUEL.value
-            ]
-            outputs["data:weight:aircraft:sizing_onboard_fuel_at_input_weight"] = (
-                outputs[self._name_provider.NEEDED_BLOCK_FUEL.value]
-                - self._mission_wrapper.consumed_fuel_before_input_weight
-            )
-
-        def as_scalar(value):
-            if isinstance(value, np.ndarray):
-                return value.item()
-            return value
-
-        self.flight_points = self.flight_points.applymap(as_scalar)
-        rename_dict = {
-            field_name: f"{field_name} [{unit}]"
-            for field_name, unit in FlightPoint.get_units().items()
-        }
-        self.flight_points.rename(columns=rename_dict, inplace=True)
-
-        if self.options["out_file"]:
-            makedirs(pth.dirname(self.options["out_file"]), exist_ok=True)
-            self.flight_points.to_csv(self.options["out_file"])
-
-    def _get_engine_wrapper(self) -> IOMPropulsionWrapper:
-        """
-        Overloading this method allows to define the engine without relying on the propulsion
-        option.
-
-        (useful for tests)
-
-        :return: the engine wrapper instance
-        """
-        return RegisterPropulsion.get_provider(self.options["propulsion_id"])
-
-
-def _get_variable_name_provider(mission_name):
-    """Factory for enum class that provide mission variable names."""
-
-    def get_variable_name(suffix):
-        return f"data:mission:{mission_name}:{suffix}"
-
-    class VariableNames(Enum):
-        """Enum with mission-related variable names."""
-
-        ZFW = get_variable_name("ZFW")
-        PAYLOAD = get_variable_name("payload")
-        BLOCK_FUEL = get_variable_name("block_fuel")
-        NEEDED_BLOCK_FUEL = get_variable_name("needed_block_fuel")
-        CONSUMED_FUEL_BEFORE_INPUT_WEIGHT = get_variable_name("consumed_fuel_before_input_weight")
-
-    return VariableNames
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,105 @@
 """
 Mission wrapper.
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 import openmdao.api as om
 import pandas as pd
 from openmdao.vectors.vector import Vector
 
 from fastoad.model_base import FlightPoint
+from fastoad.model_base.propulsion import IPropulsion
 from ..mission_definition.mission_builder import MissionBuilder
+from ..mission_definition.mission_builder.constants import NAME_TAG, TYPE_TAG
 from ..mission_definition.schema import (
     CLIMB_PARTS_TAG,
     DESCENT_PARTS_TAG,
-    MISSION_DEFINITION_TAG,
+    MissionDefinition,
     PARTS_TAG,
     PHASE_TAG,
     RESERVE_TAG,
-    ROUTE_DEFINITIONS_TAG,
     ROUTE_TAG,
 )
 
 
 class MissionWrapper(MissionBuilder):
     """
     Wrapper around
     :class:`~fastoad.models.performances.mission.mission_definition.mission_builder.MissionBuilder`
     for using with OpenMDAO.
+
+    Unlike its parent class, the `mission_name` argument is mandatory at instantiation, unless
+    there is only one mission in the definition file.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.mission_name = None
+    def __init__(
+        self,
+        mission_definition: Union[str, MissionDefinition],
+        *,
+        propulsion: IPropulsion = None,
+        reference_area: float = None,
+        mission_name: Optional[str] = None,
+        variable_prefix: str = "data:mission",
+        force_all_block_fuel_usage: bool = False,
+    ):
+        """
+        :param mission_definition: a file path or MissionDefinition instance
+        :param propulsion: if not provided, the property :attr:`propulsion` must be
+                           set before calling :meth:`build`
+        :param reference_area: if not provided, the property :attr:`reference_area` must be
+                               set before calling :meth:`build`
+        :param mission_name: name of chosen mission. Can be omitted if definition file contains
+                             only one mission.
+        :param variable_prefix: prefix for auto-generated variable names.
+        :param force_all_block_fuel_usage: if True and if `mission_name` is provided, the mission
+                                           definition will be modified to set the target fuel
+                                           consumption to variable  "~:block_fuel"
+        """
+        super().__init__(
+            mission_definition,
+            propulsion=propulsion,
+            reference_area=reference_area,
+            mission_name=mission_name,
+            variable_prefix=variable_prefix,
+        )
         self.consumed_fuel_before_input_weight = 0.0
+        if force_all_block_fuel_usage:
+            self.force_all_block_fuel_usage()
+
+    def force_all_block_fuel_usage(self):
+        """Modifies mission definition to set block fuel as target fuel consumption."""
+        if self.mission_name:
+            self.definition.force_all_block_fuel_usage(self.mission_name)
+            self._update_structure_builders()
 
-    def setup(self, component: om.ExplicitComponent, mission_name: str = None):
+    def setup(self, component: om.ExplicitComponent):
         """
         To be used during setup() of provided OpenMDAO component.
 
         It adds input and output variables deduced from mission definition file.
 
         :param component: the OpenMDAO component where the setup is done.
-        :param mission_name: mission name (can be omitted if only one mission is defined)
         """
 
-        if mission_name is None:
-            mission_name = self.get_unique_mission_name()
-        self.mission_name = mission_name
-        input_definition = self.get_input_variables(mission_name)
+        input_definition = self.get_input_variables(self.mission_name)
         output_definition = self._identify_outputs()
         output_definition = {
             name: value
             for name, value in output_definition.items()
             if name not in input_definition.names()
         }
         for variable in input_definition:
@@ -108,82 +143,81 @@
             flight_points["name2"] = [":".join(n.split(":")[: i + 1]) for n in flight_points.name]
             grouped_points = flight_points.groupby("name2")
 
             part_names = pd.unique(flight_points.name2)
             for part_name1, part_name2 in zip(part_names[:-1], part_names[1:]):
                 part1 = grouped_points.get_group(part_name1)
                 part2 = grouped_points.get_group(part_name2)
-                _compute_vars(f"data:mission:{part_name2}", part1.iloc[-1], part2.iloc[-1])
+                _compute_vars(
+                    f"{self.variable_prefix}:{part_name2}", part1.iloc[-1], part2.iloc[-1]
+                )
 
             start_part_name = part_names[0]
             start_part = grouped_points.get_group(start_part_name)
             _compute_vars(
-                f"data:mission:{start_part_name}", start_part.iloc[0], start_part.iloc[-1]
+                f"{self.variable_prefix}:{start_part_name}", start_part.iloc[0], start_part.iloc[-1]
             )
-
         del flight_points["name2"]
+
         self.consumed_fuel_before_input_weight = mission.consumed_mass_before_input_weight
+        if mission.reserve_ratio:
+            outputs[self.get_reserve_variable_name()] = mission.get_reserve_fuel()
+
         return flight_points
 
     def get_reserve_variable_name(self) -> str:
         """
         :return: the name of OpenMDAO variable for fuel reserve. This name is among the declared
                  outputs in :meth:`setup`.
         """
-        return f"{self._variable_prefix}:reserve:fuel"
+        return f"{self.variable_prefix}:{self.mission_name}:reserve:fuel"
 
     def _identify_outputs(self) -> Dict[str, Tuple[str, str]]:
         """
         Builds names of OpenMDAO outputs from names of mission, route and phases.
 
         :return: dictionary with variable name as key and unit, description as value
         """
         output_definition = {}
 
         output_definition.update(self._add_vars(self.mission_name))
 
-        for part in self.definition[MISSION_DEFINITION_TAG][self.mission_name][PARTS_TAG]:
-            if PHASE_TAG in part:
-                phase_name = part[PHASE_TAG]
-                output_definition.update(self._add_vars(self.mission_name, phase_name=phase_name))
-            elif ROUTE_TAG in part:
-                route_name = part[ROUTE_TAG]
-                output_definition.update(self._add_vars(self.mission_name, route_name))
-                route_definition = self.definition[ROUTE_DEFINITIONS_TAG][route_name]
-                for part_definition in list(
-                    route_definition[CLIMB_PARTS_TAG] + route_definition[DESCENT_PARTS_TAG]
-                ):
-                    phase_name = part_definition[PHASE_TAG]
-                    output_definition.update(
-                        self._add_vars(self.mission_name, route_name, phase_name)
-                    )
-                output_definition.update(self._add_vars(self.mission_name, route_name, "cruise"))
-            elif RESERVE_TAG in part:
+        for part in self._structure_builders[self.mission_name].structure[PARTS_TAG]:
+            if RESERVE_TAG in part:
                 output_definition[self.get_reserve_variable_name()] = (
                     "kg",
                     f'reserve fuel for mission "{self.mission_name}"',
                 )
+            elif part[TYPE_TAG] == PHASE_TAG:
+                subpart_name = part[NAME_TAG]
+                output_definition.update(self._add_vars(subpart_name))
+            elif part[TYPE_TAG] == ROUTE_TAG:
+                route_name = part[NAME_TAG]
+                output_definition.update(self._add_vars(route_name))
+                for subpart in part[CLIMB_PARTS_TAG] + part[DESCENT_PARTS_TAG]:
+                    subpart_name = subpart[NAME_TAG]
+                    output_definition.update(self._add_vars(subpart_name))
+                output_definition.update(self._add_vars(route_name + ":cruise"))
 
         return output_definition
 
-    @staticmethod
-    def _add_vars(mission_name, route_name=None, phase_name=None) -> dict:
+    def _add_vars(self, part_name) -> dict:
         """
         Builds names of OpenMDAO outputs for provided mission, route and phase names.
 
-        :param mission_name:
-        :param route_name:
-        :param phase_name:
+        :param part_name: part name in the form <mission_name>:<route_name:<phase_name>, route_name
+        and phase_name being independently optional.
         :return: dictionary with variable name as key and unit, description as value
         """
         output_definition = {}
 
-        name_root = ":".join(
-            name for name in ["data:mission", mission_name, route_name, phase_name] if name
-        )
+        name_root = ":".join(name for name in [f"{self.variable_prefix}", part_name] if name)
+
+        names = part_name.split(":")
+        mission_name, route_name, phase_name = names + [""] * (3 - len(names))
         if route_name and phase_name:
             flight_part_desc = (
                 f'phase "{phase_name}" of route "{route_name}" in mission "{mission_name}"'
             )
 
         elif route_name:
             flight_part_desc = f'route "{route_name}" in mission "{mission_name}"'
@@ -196,11 +230,7 @@
         output_definition[name_root + ":fuel"] = ("kg", f"burned fuel during {flight_part_desc}")
         output_definition[name_root + ":distance"] = (
             "m",
             f"covered ground distance during {flight_part_desc}",
         )
 
         return output_definition
-
-    @property
-    def _variable_prefix(self):
-        return f"data:mission:{self.mission_name}"
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/polar.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,97 @@
 """Aerodynamic polar data."""
+
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2021 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 from numpy import ndarray
 from scipy.interpolate import interp1d
 from scipy.optimize import fmin
 
 
 class Polar:
-    def __init__(self, cl: ndarray, cd: ndarray):
-
+    def __init__(self, cl: ndarray, cd: ndarray, alpha: ndarray = None):
         """
         Class for managing aerodynamic polar data.
 
         Links drag coefficient (CD) to lift coefficient (CL).
         It is defined by two vectors with CL and CD values.
+        If a vector of angle of attack (alpha) is given, it links alpha and CL
 
         Once defined, for any CL value, CD can be obtained using :meth:`cd`.
+        For any alpha given, CL is obtained using :meth:'cl'.
 
         :param cl: a N-elements array with CL values
         :param cd: a N-elements array with CD values that match CL
+        :param alpha: a N-elements array with angle of attack corresponding to CL values
+
         """
+
         self._definition_CL = cl
-        self._cd = interp1d(cl, cd, kind="quadratic", fill_value="extrapolate")
+        self._definition_CD = cd
+
+        # Interpolate cd
+        self._cd_vs_cl = interp1d(cl, cd, kind="quadratic", fill_value="extrapolate")
+
+        # CL as a function of AoA
+        self._definition_alpha = alpha
+        if alpha is not None:
+            self._cl_vs_alpha = interp1d(alpha, cl, kind="linear", fill_value="extrapolate")
 
         def _negated_lift_drag_ratio(lift_coeff):
             """Returns -CL/CD."""
             return -lift_coeff / self.cd(lift_coeff)
 
         self._optimal_CL = fmin(_negated_lift_drag_ratio, cl[0], disp=0)
 
     @property
     def definition_cl(self):
         """The vector that has been used for defining lift coefficient."""
         return self._definition_CL
 
     @property
+    def definition_cd(self):
+        """The vector that has been used for defining drag coefficient."""
+        return self._definition_CD
+
+    @property
+    def definition_alpha(self):
+        """The vector that has been used for defining AoA."""
+        return self._definition_alpha
+
+    @property
     def optimal_cl(self):
         """The CL value that provides larger lift/drag ratio."""
         return self._optimal_CL
 
     def cd(self, cl=None):
         """
         Computes drag coefficient (CD) by interpolation in definition data.
 
         :param cl: lift coefficient (CL) values. If not provided, the CL definition vector will be
                    used (i.e. CD definition vector will be returned)
         :return: CD values for each provide CL values
         """
         if cl is None:
-            return self._cd(self._definition_CL)
-        return self._cd(cl)
+            return self._cd_vs_cl(self._definition_CL)
+        return self._cd_vs_cl(cl)
+
+    def cl(self, alpha):
+        """
+        The lift coefficient corresponding to alpha (rad)
+
+        :param alpha: the angle of attack at which CL is evaluated
+        :return: CL value for each alpha.
+        """
+        if self._definition_alpha is None:
+            raise ValueError("Polar was instantiated without alpha vector.")
+
+        return self._cl_vs_alpha(alpha)
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/routes.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Classes for computation of routes (i.e. assemblies of climb, cruise and descent phases).
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -19,121 +19,121 @@
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import root_scalar
 
 from fastoad.model_base import FlightPoint
 from fastoad.model_base.datacls import MANDATORY_FIELD
-from fastoad.models.performances.mission.base import FlightSequence, IFlightPart
-from fastoad.models.performances.mission.segments.base import AbstractFlightSegment
-from fastoad.models.performances.mission.segments.cruise import CruiseSegment
+from .base import FlightSequence, IFlightPart
+from .segments.base import AbstractFlightSegment
+from .segments.registered.cruise import CruiseSegment
 
 
 @dataclass
-class SimpleRoute(FlightSequence):
+class RangedRoute(FlightSequence):
     """
-    Computes a simple route.
+    Computes a route so that it covers the specified ground distance.
 
     The computed route will be made of:
         - any number of climb phases
         - one cruise segment
         - any number of descent phases.
+
     """
 
     #: Any number of flight phases that will occur before cruise.
     climb_phases: List[FlightSequence] = MANDATORY_FIELD
 
     #: The cruise phase.
     cruise_segment: CruiseSegment = MANDATORY_FIELD
 
     #: Any number of flight phases that will occur after cruise.
     descent_phases: List[FlightSequence] = MANDATORY_FIELD
 
+    #: Target ground distance for whole route
+    flight_distance: float = MANDATORY_FIELD
+
+    #: Accuracy on actual total ground distance for the solver. In meters
+    distance_accuracy: float = 0.5e3
+
+    #: If True, cruise distance will be adjusted to match :attr:`flight_distance`
+    solve_distance: bool = True
+
     def __post_init__(self):
         super().__post_init__()
-        self.flight_sequence.extend(self._get_flight_sequence())
+        self.extend(self._get_flight_sequence())
+
+        # We will use this to keep data along root_scalar process (see _solve_cruise_distance() )
+        self._flight_points = None
 
     @property
     def cruise_distance(self):
         """
         Ground distance to be covered during cruise, as set in target of :attr:`cruise_segment`.
         """
-        return self.cruise_segment.target
+        return self.cruise_segment.target.ground_distance
 
     @cruise_distance.setter
     def cruise_distance(self, cruise_distance):
         self.cruise_segment.target.ground_distance = float(cruise_distance)
         self.cruise_segment.target.set_as_relative("ground_distance")
 
     @property
     def cruise_speed(self) -> Optional[Tuple[str, float]]:
         """
         Type (among `true_airspeed`, `equivalent_airspeed` and `mach`) and value of cruise speed.
         """
         climb_segments = []
         for phase in self.climb_phases:
-            climb_segments += phase.flight_sequence
+            climb_segments += phase
 
         climb_segments.reverse()
         for segment in climb_segments:
             for speed_param in ["true_airspeed", "equivalent_airspeed", "mach"]:
                 speed_value = getattr(segment.target, speed_param)
                 if speed_value and speed_value != AbstractFlightSegment.CONSTANT_VALUE:
                     return speed_param, speed_value
 
         return None
 
-    def _get_flight_sequence(self) -> List[IFlightPart]:
-        # The preliminary climb segment of the cruise segment is set to the
-        # last segment before cruise.
-        cruise_climb = self.climb_phases[-1]
-        while isinstance(cruise_climb, FlightSequence):
-            cruise_climb = cruise_climb.flight_sequence[-1]
-        self.cruise_segment.climb_segment = cruise_climb
-
-        return self.climb_phases + [self.cruise_segment] + self.descent_phases
-
-
-@dataclass
-class RangedRoute(SimpleRoute):
-    """
-    Computes a route so that it covers the specified ground distance.
-    """
-
-    #: Target ground distance for whole route
-    flight_distance: float = MANDATORY_FIELD
-
-    #: Accuracy on actual total ground distance for the solver. In meters
-    distance_accuracy: float = 0.5e3
-
-    def __post_init__(self):
-        super().__post_init__()
-
-        # We will use this to keep data along root_scalar process (see _solve_cruise_distance() )
-        self._flight_points = None
-
     def compute_from(self, start: FlightPoint) -> pd.DataFrame:
         # In very simple cases, climb and descent phases can have fixed
         # covered ground distance. In that case, cruise distance is easy to
         # obtain from flight_distance.
         # In other cases, cruise distance is obtained using a solver.
         climb_descent_distances = []
         for phase in self.climb_phases + self.descent_phases:
             climb_descent_distances.extend(self._get_ground_distances(phase))
 
+        # Using the input target distance for cruise
+        if not self.solve_distance:
+            return super().compute_from(start)
+
+        # Solving the needed cruise distance to get target flight distance
         if 0.0 in climb_descent_distances:
             return self._solve_cruise_distance(start)
 
+        # climb and descent distances are provided, cruise distance can be obtained easily.
         self.cruise_distance = self.flight_distance - np.sum(climb_descent_distances)
         return super().compute_from(start)
 
+    def _get_flight_sequence(self) -> List[IFlightPart]:
+        # The preliminary climb segment of the cruise segment is set to the
+        # last segment before cruise.
+        cruise_climb = self.climb_phases[-1]
+        while isinstance(cruise_climb, FlightSequence):
+            cruise_climb = cruise_climb[-1]
+        self.cruise_segment.climb_segment = cruise_climb
+
+        return self.climb_phases + [self.cruise_segment] + self.descent_phases
+
     @classmethod
     def _get_ground_distances(cls, phase: FlightSequence) -> list:
         ground_distances = []
-        for flight_part in phase.flight_sequence:
+        for flight_part in phase:
             if isinstance(flight_part, AbstractFlightSegment):
                 ground_distances.append(flight_part.target.ground_distance)
             else:
                 ground_distances.extend(cls._get_ground_distances(flight_part))
 
         return ground_distances
 
@@ -156,15 +156,15 @@
 
     def _compute_flight(self, cruise_distance, start: FlightPoint):
         """
         Computes flight for provided cruise distance
 
         :param cruise_distance:
         :param start:
-        :return: difference between computes distance and self.flight_distance
+        :return: difference between computed distance and self.flight_distance
         """
         self.cruise_distance = cruise_distance
         self._flight_points = super().compute_from(start)
         obtained_distance = (
             self._flight_points.iloc[-1].ground_distance
             - self._flight_points.iloc[0].ground_distance
         )
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-"""Classes for simulating flight segments."""
+"""
+Management of modules using Pelix/iPOPO
+"""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2020  ONERA & ISAE-SUPAERO
+#  Copyright (C) 2021 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/altitude_change.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/altitude_change.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes for climb/descent segments."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -17,26 +17,27 @@
 from dataclasses import dataclass
 from typing import List, Tuple
 
 import pandas as pd
 from scipy.constants import foot, g
 
 from fastoad.model_base import FlightPoint
-from .base import AbstractManualThrustSegment
-from ..exceptions import FastFlightSegmentIncompleteFlightPoint
-from ..util import get_closest_flight_level
+from fastoad.models.performances.mission.exceptions import FastFlightSegmentIncompleteFlightPoint
+from fastoad.models.performances.mission.segments.base import (
+    RegisterSegment,
+)
+from fastoad.models.performances.mission.segments.time_step_base import AbstractManualThrustSegment
+from fastoad.models.performances.mission.util import get_closest_flight_level
 
 _LOGGER = logging.getLogger(__name__)  # Logger for this module
 
 
+@RegisterSegment("altitude_change")
 @dataclass
-class AltitudeChangeSegment(
-    AbstractManualThrustSegment,
-    mission_file_keyword="altitude_change",
-):
+class AltitudeChangeSegment(AbstractManualThrustSegment):
     """
     Computes a flight path segment where altitude is modified with constant speed.
 
     .. note:: **Setting speed**
 
         Constant speed may be:
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/cruise.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/cruise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes for simulating cruise segments."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -17,17 +17,20 @@
 from typing import List
 
 import numpy as np
 import pandas as pd
 from scipy.constants import foot, g
 
 from fastoad.model_base import FlightPoint
+from fastoad.models.performances.mission.segments.base import (
+    RegisterSegment,
+)
+from fastoad.models.performances.mission.util import get_closest_flight_level
 from .altitude_change import AltitudeChangeSegment
-from .base import AbstractRegulatedThrustSegment, AbstractTimeStepFlightSegment
-from ..util import get_closest_flight_level
+from ..time_step_base import AbstractRegulatedThrustSegment, AbstractTimeStepFlightSegment
 
 
 @dataclass
 class CruiseSegment(AbstractRegulatedThrustSegment):
     """
     Class for computing cruise flight segment at constant altitude and speed.
 
@@ -52,16 +55,17 @@
     def get_distance_to_target(
         self, flight_points: List[FlightPoint], target: FlightPoint
     ) -> float:
         current = flight_points[-1]
         return target.ground_distance - current.ground_distance
 
 
+@RegisterSegment("optimal_cruise")
 @dataclass
-class OptimalCruiseSegment(CruiseSegment, mission_file_keyword="optimal_cruise"):
+class OptimalCruiseSegment(CruiseSegment):
     """
     Class for computing cruise flight segment at maximum lift/drag ratio.
 
     Altitude is set **at every point** to get the optimum CL according to current mass.
     Target is a specified ground_distance. The target definition indicates
     the ground_distance to be covered during the segment, independently of
     the initial value.
@@ -76,16 +80,17 @@
 
     def _compute_next_altitude(self, next_point: FlightPoint, previous_point: FlightPoint):
         next_point.altitude = self._get_optimal_altitude(
             next_point.mass, previous_point.mach, altitude_guess=previous_point.altitude
         )
 
 
+@RegisterSegment("cruise")
 @dataclass
-class ClimbAndCruiseSegment(CruiseSegment, mission_file_keyword="cruise"):
+class ClimbAndCruiseSegment(CruiseSegment):
     """
     Class for computing cruise flight segment at constant altitude.
 
     Target is a specified ground_distance. The target definition indicates
     the ground_distance to be covered during the segment, independently of
     the initial value.
     Target should also specify a speed parameter set to "constant", among `mach`,
@@ -188,20 +193,17 @@
 
         cruise_start = FlightPoint.create(climb_points.iloc[-1])
         cruise_points = cruise_segment.compute_from(cruise_start)
 
         return pd.concat([climb_points, cruise_points]).reset_index(drop=True)
 
 
+@RegisterSegment("breguet")
 @dataclass
-class BreguetCruiseSegment(
-    CruiseSegment,
-    mission_file_keyword="breguet",
-    attribute_units=dict(climb_and_descent_distance="m"),
-):
+class BreguetCruiseSegment(CruiseSegment):
     """
     Class for computing cruise flight segment at constant altitude using Breguet-Leduc formula.
 
     As formula relies on SFC, the :attr:`propulsion` model must be able to fill FlightPoint.sfc
     when FlightPoint.thrust is provided.
     """
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/hold.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/hold.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Class for simulating hold segment."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 
-from .base import (
+from fastoad.models.performances.mission.segments.base import (
+    RegisterSegment,
+)
+from fastoad.models.performances.mission.segments.time_step_base import (
     AbstractFixedDurationSegment,
     AbstractRegulatedThrustSegment,
 )
 
 
+@RegisterSegment("holding")
 @dataclass
-class HoldSegment(
-    AbstractRegulatedThrustSegment,
-    AbstractFixedDurationSegment,
-    mission_file_keyword="holding",
-):
+class HoldSegment(AbstractRegulatedThrustSegment, AbstractFixedDurationSegment):
     """
     Class for computing hold flight segment.
 
     Mach is considered constant, equal to Mach at starting point.
     Altitude is constant.
     Target is a specified time. The target definition indicates
     the time duration of the segment, independently of the initial time value.
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/mass_input.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/mass_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Class for specifying input mass at "any" point in the mission."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -13,19 +13,20 @@
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 
 import pandas as pd
 
 from fastoad.model_base import FlightPoint
-from fastoad.models.performances.mission.segments.base import AbstractFlightSegment
+from fastoad.models.performances.mission.segments.base import AbstractFlightSegment, RegisterSegment
 
 
+@RegisterSegment("mass_input")
 @dataclass
-class MassTargetSegment(AbstractFlightSegment, mission_file_keyword="mass_input"):
+class MassTargetSegment(AbstractFlightSegment):
     """
     Class that simply sets a target mass.
 
     :meth:`compute_from` returns a 1-row dataframe that is the start point with mass
     set to provided target mass.
 
     class:`~fastoad.models.performances.mission.base.FlightSequence` ensures that
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/speed_change.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/speed_change.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes for acceleration/deceleration segments."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -13,22 +13,26 @@
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from dataclasses import dataclass
 from typing import List, Tuple
 
 from fastoad.model_base import FlightPoint
-from .base import AbstractManualThrustSegment
-from ..exceptions import FastFlightSegmentIncompleteFlightPoint
+from fastoad.models.performances.mission.exceptions import FastFlightSegmentIncompleteFlightPoint
+from fastoad.models.performances.mission.segments.base import (
+    RegisterSegment,
+)
+from fastoad.models.performances.mission.segments.time_step_base import AbstractManualThrustSegment
 
 _LOGGER = logging.getLogger(__name__)  # Logger for this module
 
 
+@RegisterSegment("speed_change")
 @dataclass
-class SpeedChangeSegment(AbstractManualThrustSegment, mission_file_keyword="speed_change"):
+class SpeedChangeSegment(AbstractManualThrustSegment):
     """
     Computes a flight path segment where speed is modified with no change in altitude.
 
     The target must define a speed value among true_airspeed, equivalent_airspeed
     and mach.
     """
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/start.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Class for mission start point."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -13,20 +13,21 @@
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 
 import pandas as pd
 
 from fastoad.model_base import FlightPoint
-from .base import AbstractFlightSegment
-from ..exceptions import FastFlightSegmentIncompleteFlightPoint
+from fastoad.models.performances.mission.exceptions import FastFlightSegmentIncompleteFlightPoint
+from fastoad.models.performances.mission.segments.base import AbstractFlightSegment, RegisterSegment
 
 
+@RegisterSegment("start")
 @dataclass
-class Start(AbstractFlightSegment, mission_file_keyword="start"):
+class Start(AbstractFlightSegment):
     """
     Provides a starting point for a mission.
 
     :meth:`compute_from` will return only 1 flight points that matches the target.
     """
 
     def compute_from_start_to_target(self, start: FlightPoint, target: FlightPoint) -> pd.DataFrame:
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/taxi.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/taxi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes for Taxi sequences."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -14,28 +14,27 @@
 
 from dataclasses import dataclass
 from typing import Tuple
 
 import pandas as pd
 
 from fastoad.model_base import FlightPoint
+from fastoad.models.performances.mission.polar import Polar
 from fastoad.models.performances.mission.segments.base import (
+    RegisterSegment,
+)
+from fastoad.models.performances.mission.segments.time_step_base import (
     AbstractFixedDurationSegment,
+    AbstractManualThrustSegment,
 )
-from .base import AbstractManualThrustSegment
-from ..polar import Polar
 
 
+@RegisterSegment("taxi")
 @dataclass
-class TaxiSegment(
-    AbstractManualThrustSegment,
-    AbstractFixedDurationSegment,
-    mission_file_keyword="taxi",
-    attribute_units=dict(true_airspeed="m/s"),
-):
+class TaxiSegment(AbstractManualThrustSegment, AbstractFixedDurationSegment):
     """
     Class for computing Taxi phases.
 
     Taxi phase has a target duration (target.time should be provided) and is at
     constant altitude, speed and thrust rate.
     """
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/segments/transition.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/transition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Class for very simple transition in some flight phases."""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -14,21 +14,20 @@
 
 from copy import deepcopy
 from dataclasses import dataclass
 
 import pandas as pd
 
 from fastoad.model_base import FlightPoint
-from fastoad.models.performances.mission.segments.base import (
-    AbstractFlightSegment,
-)
+from fastoad.models.performances.mission.segments.base import AbstractFlightSegment, RegisterSegment
 
 
+@RegisterSegment("transition")
 @dataclass
-class DummyTransitionSegment(AbstractFlightSegment, mission_file_keyword="transition"):
+class DummyTransitionSegment(AbstractFlightSegment):
     """
     Computes a transient flight part in a very quick and dummy way.
 
     :meth:`compute_from` will return only 2 or 3 flight points.
 
     The second flight point is the end of transition. Its parameters are equal to those provided
     in :attr:`~fastoad.models.performances.mission.segments.base.FlightSegment.target`.
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/performances/mission/util.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/util.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/models/variable_descriptions.txt` & `fast_oad_core-1.5.0/src/fastoad/models/variable_descriptions.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Documentation of variables used in FAST-OAD models
-# Each line shoud be like:
+# Each line should be like:
 # my:variable||The description of my:variable, as long as needed, but on one line.
 # The separator "||" can be surrounded with spaces (that will be ignored)
-test:test_variable || for testing (do not remove, keep first)
 data:TLAR:cruise_mach || top-level requirement: cruise Mach number
 data:TLAR:range || top-level requirement: design range
 data:aerodynamics:aircraft:cruise:CD || drag coefficient in cruise conditions w.r.t. data:aerodynamics:aircraft:cruise:CL
 data:aerodynamics:aircraft:cruise:CL || scale of lift coefficient values for drag computations in cruise conditions
 data:geometry:wing:area || wing reference area
 data:weight:aircraft:CG:aft:MAC_position || most aft X-position of center of gravity as ratio of mean aerodynamic chord
 data:weight:aircraft:CG:aft:x || most aft X-position of aircraft center of gravity
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-"""
-Management of modules using Pelix/iPOPO
-"""
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2021 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/_bundle_loader.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/_bundle_loader.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/_plugins.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/_plugins.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 from .exceptions import (
     FastNoAvailableConfigurationFileError,
     FastNoDistPluginError,
     FastSeveralConfigurationFilesError,
     FastSeveralDistPluginsError,
     FastUnknownConfigurationFileError,
     FastUnknownDistPluginError,
+    FastNoAvailableSourceDataFileError,
+    FastUnknownSourceDataFileError,
+    FastSeveralSourceDataFilesError,
 )
 from .._utils.resource_management.contents import PackageReader
 
 if sys.version_info >= (3, 10):
     import importlib.metadata as importlib_metadata
 else:
     import importlib_metadata
@@ -49,19 +52,22 @@
 
 class SubPackageNames(Enum):
     """Enumeration of possible plugin subpackages."""
 
     MODELS = "models"
     NOTEBOOKS = "notebooks"
     CONFIGURATIONS = "configurations"
+    SOURCE_DATA_FILES = "source_data_files"
 
 
 @dataclass
 class ResourceInfo:
-    """Class for storing information about configuration files provided by plugins."""
+    """
+    Class for storing information about configuration and source data files provided by plugins.
+    """
 
     name: str
     dist_name: str
     plugin_name: str
     package_name: str
 
 
@@ -101,14 +107,32 @@
                 )
                 for file in PackageReader(self.subpackages[SubPackageNames.CONFIGURATIONS]).contents
                 if pth.splitext(file)[1] in [".yml", ".yaml"]
             ]
 
         return []
 
+    def get_source_data_file_list(self) -> List[ResourceInfo]:
+
+        if SubPackageNames.SOURCE_DATA_FILES in self.subpackages:
+            return [
+                ResourceInfo(
+                    name=file,
+                    dist_name=self.dist_name,
+                    plugin_name=self.plugin_name,
+                    package_name=self.subpackages[SubPackageNames.SOURCE_DATA_FILES],
+                )
+                for file in PackageReader(
+                    self.subpackages[SubPackageNames.SOURCE_DATA_FILES]
+                ).contents
+                if pth.splitext(file)[1] in [".xml"]
+            ]
+
+        return []
+
 
 @dataclass()
 class DistributionPluginDefinition(dict):
     """
     Stores and provides data for FAST-OAD plugins provided by a Python distribution.
     """
 
@@ -140,14 +164,63 @@
                 DeprecationWarning,
             )
             self[entry_point.name].subpackages[SubPackageNames.MODELS] = entry_point.module
 
         if group == MODEL_PLUGIN_ID:
             self[entry_point.name].detect_subfolders()
 
+    def get_source_data_file_list(self, plugin_name=None) -> List[ResourceInfo]:
+        """
+        :param plugin_name: If provided, only file names provided by the plugin in
+                            the distribution will be returned, or an empty list if
+                            the plugin is not in the distribution.
+        :return:  List of source data file information that are provided by the distribution.
+        """
+        file_list = []
+        if plugin_name:
+            if plugin_name in self:
+                file_list = self[plugin_name].get_source_data_file_list()
+        else:
+            for plugin in self.values():
+                file_list += plugin.get_source_data_file_list()
+
+        return file_list
+
+    def get_source_data_file_info(self, file_name=None, plugin_name=None) -> ResourceInfo:
+        """
+        :param file_name: can be None if only one configuration file is provided in the
+                          distribution (or in the plugin if `plugin_name` is provided)
+        :param plugin_name:
+        :return: information for specified configuration file name.
+        :raise FastSeveralSourceDataFilesError: if several source data files are available but
+                                               `file_name` has not been provided.
+        :raise FastUnknownSourceDataFileError: if the specified source data file is not available.
+        :raise FastNoAvailableSourceDataFileError: if there a no source data file in the plugin.
+        """
+
+        source_data_file_list = self.get_source_data_file_list(plugin_name)
+        if not source_data_file_list:
+            raise FastNoAvailableSourceDataFileError()
+
+        if file_name is None:
+            if len(source_data_file_list) > 1:
+                raise FastSeveralSourceDataFilesError(self.dist_name)
+            file_info = source_data_file_list[0]
+        else:
+            matching_list = list(filter(lambda item: item.name == file_name, source_data_file_list))
+            if len(matching_list) == 0:
+                raise FastUnknownSourceDataFileError(file_name, self.dist_name)
+
+            # Here we implicitly assume that plugin developers will ensure that there will be
+            # no duplicates in conf file names (possible if several plugins are in the
+            # same installed package, but such practice is discouraged).
+            file_info = matching_list[0]
+
+        return file_info
+
     def get_configuration_file_list(self, plugin_name=None) -> List[ResourceInfo]:
         """
         :param plugin_name: If provided, only file names provided by the plugin in
                             the distribution will be returned, or an empty list if
                             the plugin is not in the distribution.
         :return:  List of configuration file information that are provided by the distribution.
         """
@@ -225,19 +298,21 @@
         has_models = np.any(
             [SubPackageNames.MODELS in definition.subpackages for definition in self.values()]
         )
         has_notebooks = np.any(
             [SubPackageNames.NOTEBOOKS in definition.subpackages for definition in self.values()]
         )
         conf_files = [item.name for item in self.get_configuration_file_list()]
+        source_data_files = [item.name for item in self.get_source_data_file_list()]
         return dict(
             installed_package=self.dist_name,
             has_models=has_models,
             has_notebooks=has_notebooks,
             configurations=sorted(conf_files),
+            source_data_files=sorted(source_data_files),
         )
 
 
 class FastoadLoader(BundleLoader):
     """
     Specialized :class:`BundleLoader` that will load plugins at first instantiation.
 
@@ -297,14 +372,25 @@
                  or an empty list if the specified distribution is not available
         """
         return self._get_resource_list(
             DistributionPluginDefinition.get_configuration_file_list,
             dist_name,
         )
 
+    def get_source_data_file_list(self, dist_name: str) -> List[ResourceInfo]:
+        """
+        :param dist_name: the distribution to inspect
+        :return: list of source data files available for named distribution, or an empty list if the
+                 specified distribution is not available
+        """
+        return self._get_resource_list(
+            DistributionPluginDefinition.get_source_data_file_list,
+            dist_name,
+        )
+
     def get_notebook_folder_list(self, dist_name: str = None) -> List[ResourceInfo]:
         """
         Returns the list of notebook folders available for named distribution
         and optionally the named plugin of this distribution.
 
         :param dist_name: the distribution to inspect
         :return: list of notebook folders available for named distribution,
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/constants.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/constants.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -189,7 +189,39 @@
 
     def __init__(self, dist_name):
         self.dist_name = dist_name
         super().__init__(
             f'Installed package "{dist_name}" provides several configuration files. '
             "One must be specified."
         )
+
+
+class FastNoAvailableSourceDataFileError(FastError):
+    """Raised when a source data file is requested, but none is available in plugins."""
+
+    def __init__(self):
+        super().__init__("No source data file provided with currently installed plugins.")
+
+
+class FastUnknownSourceDataFileError(FastError):
+    """Raised when a source data file is not found for named distribution."""
+
+    def __init__(self, source_data_file, dist_name):
+        self.source_data_file = source_data_file
+        self.dist_name = dist_name
+        super().__init__(
+            f'Source data file "{source_data_file}" not provided with '
+            f'installed package "{dist_name}".'
+        )
+
+
+class FastSeveralSourceDataFilesError(FastError):
+    """
+    Raised when no source data file has been specified but several source data files are
+    provided with the distribution."""
+
+    def __init__(self, dist_name):
+        self.dist_name = dist_name
+        super().__init__(
+            f'Installed package "{dist_name}" provides several source data files. '
+            "One must be specified."
+        )
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/module_management/service_registry.py` & `fast_oad_core-1.5.0/src/fastoad/module_management/service_registry.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/problem_description.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/problem_description.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/displacements.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/displacements.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/stresses.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/stresses.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/01_Quick_start/modules/weight.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/weight.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml` & `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/README.md` & `fast_oad_core-1.5.0/src/fastoad/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/notebooks/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/_utils.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Utility functions for OpenMDAO classes/instances
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -43,19 +43,29 @@
     """
     # An actual MPI communicator will make the deepcopy crash if an MPI
     # library is installed.
 
     actual_comm = problem.comm
     problem.comm = FakeComm()
 
+    metadata_were_added = False
     try:
+        if not problem._metadata:
+            # Adding temporarily this attribute ensures that the post-hook for N2 reports
+            # will not crash. Indeed, due to the copy, it tries to post-process
+            # the 'problem' instance at the end of setup of the 'problem_copy' instance.
+            problem._metadata = {"saved_errors": []}
+            metadata_were_added = True
         problem_copy = deepcopy(problem)
         problem_copy.comm = problem.comm
+
         yield problem_copy
     finally:
+        if metadata_were_added:
+            problem._metadata = None
         problem.comm = actual_comm
 
 
 @deprecated(
     version="1.3.0",
     reason="Will be removed in version 2.0. Please use VariableList.from_problem() instead",
 )
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/exceptions.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/exceptions.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/problem.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/problem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-import os
-import warnings
 from copy import deepcopy
 from typing import Tuple
 
 import numpy as np
-import openmdao
 import openmdao.api as om
 from openmdao.core.constants import _SetupStatus
-from openmdao.core.system import _MetadataDict
-from packaging import version
+from openmdao.core.system import System
 
 from fastoad.io import DataFile, VariableIO
 from fastoad.module_management.service_registry import RegisterSubmodel
 from fastoad.openmdao.validity_checker import ValidityDomainChecker
 from fastoad.openmdao.variables import VariableList
 from ._utils import problem_without_mpi
 from .exceptions import FASTOpenMDAONanInInputFile
@@ -43,23 +39,17 @@
 
     It also runs :class:`~fastoad.openmdao.validity_checker.ValidityDomainChecker`
     after each :meth:`run_model` or :meth:`run_driver`
     (but it does nothing if no check has been registered).
     """
 
     def __init__(self, *args, **kwargs):
-        if (
-            version.parse(openmdao.__version__) >= version.parse("3.17")
-            and "OPENMDAO_REPORTS" not in os.environ
-            and "reports" not in kwargs
-            and len(args) < 5
-        ):
-            # Automatic reports are deactivated for FAST-OAD, unless OPENMDAO_REPORTS env
-            # variable is set.
-            kwargs["reports"] = None
+        # Automatic reports are deactivated for FAST-OAD, unless OPENMDAO_REPORTS env
+        # variable is set.
+        kwargs["reports"] = None
         super().__init__(*args, **kwargs)
 
         #: File path where :meth:`read_inputs` will read inputs
         self.input_file_path = None
         #: File path where :meth:`write_outputs` will write outputs
         self.output_file_path = None
 
@@ -230,66 +220,29 @@
 
         :param problem:
         """
         # First all outputs are identified. If a dynamically shaped input is fed by a matching
         # output, its shaped will be determined.
         output_var_names = []
         for system in problem.model.system_iter(recurse=False):
-            io_metadata = cls._get_io_metadata(system, "output")
+            io_metadata = system.get_io_metadata("output")
             output_var_names += [meta["prom_name"] for meta in io_metadata.values()]
 
         dynamic_vars = {}
         for system in problem.model.system_iter(recurse=False):
-            io_metadata = cls._get_io_metadata(system, "input")
+            io_metadata = system.get_io_metadata("input")
             dynamic_vars.update(
                 {
                     meta["prom_name"]: meta
                     for name, meta in io_metadata.items()
                     if meta["shape_by_conn"] and meta["prom_name"] not in output_var_names
                 }
             )
         return dynamic_vars
 
-    @staticmethod
-    def _get_io_metadata(
-        system,
-        iotypes,
-    ):
-        # In OpenMDAO >3.16, get_io_metadata() won't complain after dynamically shaped, non-
-        # connected inputs.
-        if version.parse(openmdao.__version__) >= version.parse("3.17"):
-            return system.get_io_metadata(iotypes)
-
-        # For OpenMDAO<=3.16, we try the vanilla get_io_metadata() and if it fails, we
-        # try with our simplified implementation.
-        try:
-            return system.get_io_metadata(iotypes)
-        except RuntimeError:
-            prefix = system.pathname + "." if system.pathname else ""
-            rel_idx = len(prefix)
-            if isinstance(iotypes, str):
-                iotypes = (iotypes,)
-
-            result = {}
-            for iotype in iotypes:
-                for abs_name, prom in system._var_abs2prom[iotype].items():
-                    rel_name = abs_name[rel_idx:]
-                    meta = system._var_allprocs_abs2meta[iotype].get(abs_name)
-                    ret_meta = _MetadataDict(meta) if meta is not None else None
-                    if ret_meta is not None:
-                        ret_meta["prom_name"] = prom
-                        result[rel_name] = ret_meta
-
-            warnings.warn(
-                "Dynamically shaped problem inputs are better managed with OpenMDAO>3.16 "
-                "Upgrade is recommended.",
-                DeprecationWarning,
-            )
-            return result
-
 
 class AutoUnitsDefaultGroup(om.Group):
     """
     OpenMDAO group that automatically use self.set_input_defaults() to resolve declaration
     conflicts in variable units.
     """
 
@@ -323,7 +276,34 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         #: Definition of active submodels that will be applied during setup()
         self.active_submodels = {}
 
     def setup(self):
         RegisterSubmodel.active_models.update(self.active_submodels)
+
+
+def get_variable_list_from_system(
+    system: System,
+    get_promoted_names: bool = True,
+    promoted_only: bool = True,
+    io_status: str = "all",
+) -> "VariableList":
+    """
+    Creates a VariableList instance containing inputs and outputs of any OpenMDAO System.
+
+    Convenience method that creates a FASTOADProblem problem with only provided `system`
+    and uses :meth:`~fastoad.openmdao.variables.variable.VariableList.from_problem()`.
+    """
+    # Dev note:
+    # This method is not a class method of VariableList because it would
+    # create a circular import because of the usage of FASTOADProblem.
+    # And usage of FASTOADProblem instead of om.Problem avoids failure in case
+    # there are shape_by_conn inputs.
+    problem = FASTOADProblem()
+    problem.model.add_subsystem("comp", system, promotes=["*"])
+    return VariableList.from_problem(
+        problem,
+        get_promoted_names=get_promoted_names,
+        promoted_only=promoted_only,
+        io_status=io_status,
+    )
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/resources/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/validity_checker.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/validity_checker.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/__init__.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,9 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# flake8: noqa
-
 from .variable import Variable
 from .variable_list import VariableList
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/variable.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,18 @@
                 del my_metadata[key]
             if key in other_metadata:
                 del other_metadata[key]
 
         return (
             isinstance(other, Variable)
             and self.name == other.name
-            and np.all(np.isclose(my_value, other_value, equal_nan=True))
+            and (
+                np.all(my_value == other_value)  # This condition is for val of type string
+                or np.all(np.isclose(my_value, other_value, equal_nan=True))
+            )
             and my_metadata == other_metadata
         )
 
     def __repr__(self):
         return "Variable(name=%s, metadata=%s)" % (self.name, self.metadata)
 
     def __hash__(self) -> int:
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/variables/variable_list.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Class for managing a list of OpenMDAO variables.
 """
 #  This file is part of FAST-OAD : A framework for rapid Overall Aircraft Design
-#  Copyright (C) 2022 ONERA & ISAE-SUPAERO
+#  Copyright (C) 2023 ONERA & ISAE-SUPAERO
 #  FAST is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -149,23 +149,23 @@
 
         :return: a pandas DataFrame instance with all variables from current list
         """
         var_dict = {"name": []}
         var_dict.update({metadata_name: [] for metadata_name in self.metadata_keys()})
 
         for variable in self:
-            value = self._as_list_or_float(variable.value)
+            value = self._as_list_or_item(variable.value)
             var_dict["name"].append(variable.name)
             for metadata_name in self.metadata_keys():
                 if metadata_name == "val":
                     var_dict["val"].append(value)
                 else:
                     # TODO: make this more generic
                     if metadata_name in ["val", "initial_value", "lower", "upper"]:
-                        metadata = self._as_list_or_float(variable.metadata[metadata_name])
+                        metadata = self._as_list_or_item(variable.metadata[metadata_name])
                     else:
                         metadata = variable.metadata[metadata_name]
                     var_dict[metadata_name].append(metadata)
 
         df = pd.DataFrame.from_dict(var_dict)
 
         return df
@@ -193,30 +193,33 @@
         Creates a VariableList instance from an OpenMDAO IndepVarComp instance
 
         :param ivc: an IndepVarComp instance
         :return: a VariableList instance
         """
         variables = cls()
 
+        # Need setup on ivc to have get_io_metadata() working
         ivc = deepcopy(ivc)
-        om.Problem(ivc).setup()  # Need setup to have get_io_metadata working
+        problem = om.Problem()
+        problem.model.add_subsystem("ivc", ivc)
+        problem.setup()
 
         for name, metadata in ivc.get_io_metadata(
             metadata_keys=["val", "units", "upper", "lower"]
         ).items():
             metadata = metadata.copy()
             value = metadata.pop("val")
-            value = cls._as_list_or_float(value)
+            value = cls._as_list_or_item(value)
             metadata.update({"val": value})
             variables[name] = metadata
 
         return variables
 
     @classmethod
-    def _as_list_or_float(cls, value):
+    def _as_list_or_item(cls, value):
         value = np.asarray(value)
         if np.size(value) == 1:
             value = value.item()
             try:
                 value = float(value)
             except (TypeError, ValueError):
                 pass
@@ -238,15 +241,15 @@
         column_names = [name for name in df.columns]
 
         def _get_variable(row):
             var_as_dict = {key: val for key, val in zip(column_names, row)}
             # TODO: make this more generic
             for key, val in var_as_dict.items():
                 if key in ["val", "initial_value", "lower", "upper"]:
-                    var_as_dict[key] = cls._as_list_or_float(val)
+                    var_as_dict[key] = cls._as_list_or_item(val)
                 else:
                     pass
             return Variable(**var_as_dict)
 
         return cls([_get_variable(row) for row in df[column_names].values])
 
     @classmethod
```

### Comparing `FAST-OAD-core-1.4.2/src/fastoad/openmdao/whatsopt.py` & `fast_oad_core-1.5.0/src/fastoad/openmdao/whatsopt.py`

 * *Files identical despite different names*

### Comparing `FAST-OAD-core-1.4.2/PKG-INFO` & `fast_oad_core-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-oad-core
-Version: 1.4.2
+Version: 1.5.0
 Summary: FAST-OAD is a framework for performing rapid Overall Aircraft Design
 Home-page: https://github.com/fast-aircraft-design/FAST-OAD
 License: GPL-3.0-only
 Keywords: aircraft,design,multi-disciplinary
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
 Requires-Python: >=3.7,<4.0
@@ -14,58 +14,71 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: mpi4py
 Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: aenum (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: ensure (>=1.0.0,<2.0.0)
-Requires-Dist: importlib-metadata (>=4.2,<5.0); python_version < "3.10"
+Requires-Dist: importlib-metadata (>=4.2,<5.0) ; python_version < "3.10"
 Requires-Dist: ipopo (>=1.0.0,<2.0.0)
 Requires-Dist: ipysheet (>=0.5.0,<1)
 Requires-Dist: ipywidgets (>=7.7.0,<8.0.0)
 Requires-Dist: jsonschema (>=3.2.0,<5)
 Requires-Dist: jupyter-client (!=7.0.0,!=7.0.1,!=7.0.2,!=7.0.3,!=7.0.4,!=7.0.5)
 Requires-Dist: jupyterlab (>=3.3.0,<4.0.0)
 Requires-Dist: lxml (>=4.6.5,<5.0.0)
-Requires-Dist: mpi4py (>=3,<4); extra == "mpi4py"
+Requires-Dist: mpi4py (>=3,<4) ; extra == "mpi4py"
 Requires-Dist: notebook (>=6.0,<7.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: openmdao (>=3.10,<4.0)
+Requires-Dist: openmdao (>=3.18,<4.0)
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: plotly (>=5.0.0,<6.0.0)
+Requires-Dist: pyDOE2 (>=1.3.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.15.78,<0.18)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Requires-Dist: stdatm (<1.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tomlkit (>=0.5.3,<1)
 Requires-Dist: wop (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
+<p align="center">
+  <img src="docs/img/FAST_OAD_logo2.jpg" alt="FAST-OAD logo" width="600">
+</p>
+
+Future Aircraft Sizing Tool - Overall Aircraft Design
+===============================================================
+
 ![Tests](https://github.com/fast-aircraft-design/FAST-OAD/workflows/Tests/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9691f1d1430c45cf9c94bc342b4c6122)](https://www.codacy.com/gh/fast-aircraft-design/FAST-OAD?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fast-aircraft-design/FAST-OAD&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/fast-aircraft-design/FAST-OAD/branch/master/graph/badge.svg)](https://codecov.io/gh/fast-aircraft-design/FAST-OAD)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![Documentation Status](https://readthedocs.org/projects/fast-oad/badge/?version=stable)](https://fast-oad.readthedocs.io/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fast-aircraft-design/FAST-OAD.git/latest-release?urlpath=lab%2Ftree%2Fsrc%2Ffastoad%2Fnotebooks)
+[![DOI](https://zenodo.org/badge/186570813.svg)](https://zenodo.org/badge/latestdoi/186570813)
+
+
 
 
-FAST-OAD: Future Aircraft Sizing Tool - Overall Aircraft Design
-===============================================================
 
 FAST-OAD is a framework for performing rapid Overall Aircraft Design.
 
 It proposes multi-disciplinary analysis and optimisation by relying on
 the [OpenMDAO framework](https://openmdao.org/).
 
 FAST-OAD allows easy switching between models for a same discipline, and
```

