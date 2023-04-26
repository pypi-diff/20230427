# Comparing `tmp/epyt-1.0.3.tar.gz` & `tmp/epyt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyt-1.0.3.tar", last modified: Wed Apr 26 20:55:17 2023, max compression
+gzip compressed data, was "epyt-1.0.4.tar", last modified: Wed Apr 26 21:58:45 2023, max compression
```

## Comparing `epyt-1.0.3.tar` & `epyt-1.0.4.tar`

### file list

```diff
@@ -1,158 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.327432 epyt-1.0.3/
--rw-rw-rw-   0        0        0    13984 2023-04-25 21:16:32.000000 epyt-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      439 2023-04-25 21:16:32.000000 epyt-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    42656 2023-04-26 20:55:17.326436 epyt-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    41720 2023-04-25 21:17:42.000000 epyt-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.922755 epyt-1.0.3/epyt/
--rw-rw-rw-   0        0        0       55 2023-04-26 11:19:41.000000 epyt-1.0.3/epyt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.959620 epyt-1.0.3/epyt/__pycache__/
--rw-rw-rw-   0        0        0      204 2023-04-26 19:07:56.000000 epyt-1.0.3/epyt/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      208 2023-04-26 15:27:40.000000 epyt-1.0.3/epyt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0   448735 2023-04-26 19:52:17.000000 epyt-1.0.3/epyt/__pycache__/epanet.cpython-37.pyc
--rw-rw-rw-   0        0        0   447297 2023-04-26 15:27:40.000000 epyt-1.0.3/epyt/__pycache__/epanet.cpython-39.pyc
--rw-rw-rw-   0        0        0   515504 2023-04-26 20:51:30.000000 epyt-1.0.3/epyt/epanet.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.966271 epyt-1.0.3/epyt/examples/
--rw-rw-rw-   0        0        0     4154 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/examples/README.md
--rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.060541 epyt-1.0.3/epyt/examples/notebooks/
--rw-rw-rw-   0        0        0     4071 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX10_close_pipes_during_sim.ipynb
--rw-rw-rw-   0        0        0     3169 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX11_assing_new_curve_pump.ipynb
--rw-rw-rw-   0        0        0    61390 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX13c_add_cvpipe.ipynb
--rw-rw-rw-   0        0        0    26991 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX14_hydraulic_and_quality_analysis.ipynb
--rw-rw-rw-   0        0        0   744778 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX16_create_multiple_scenarios.ipynb
--rw-rw-rw-   0        0        0   211279 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX17b_add_multiple_controls_pipestatus.ipynb
--rw-rw-rw-   0        0        0   198828 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX18_change_status_pipes.ipynb
--rw-rw-rw-   0        0        0   316856 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX1_Plot_network_topology.ipynb
--rw-rw-rw-   0        0        0    67212 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX20a_external_controls.ipynb
--rw-rw-rw-   0        0        0    68755 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX20b_external_controls.ipynb
--rw-rw-rw-   0        0        0     4757 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX21_Pressure_driven_analysis_option.ipynb
--rw-rw-rw-   0        0        0     5397 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX22_Overflow_option_for_tanks.ipynb
--rw-rw-rw-   0        0        0     2619 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX23_Change_connection_links.ipynb
--rw-rw-rw-   0        0        0     2989 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX25_set_node_name_ids.ipynb
--rw-rw-rw-   0        0        0  4818817 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX2_Hydraulic_analysis.ipynb
--rw-rw-rw-   0        0        0   387195 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX3_Quality_analysis.ipynb
--rw-rw-rw-   0        0        0   417836 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX4_Plot_time_series.ipynb
--rw-rw-rw-   0        0        0   119797 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX5_Plot_values_parameters.ipynb
--rw-rw-rw-   0        0        0    80478 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX6_load_two_inp_files.ipynb
--rw-rw-rw-   0        0        0    67273 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX7_Set_Pump_Curves.ipynb
--rw-rw-rw-   0        0        0   409890 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/EX9_compare_simulations.ipynb
--rw-rw-rw-   0        0        0     4452 2023-04-26 19:33:54.000000 epyt-1.0.3/epyt/examples/notebooks/Plt_EX1_Create_Flow_gif.ipynb
--rw-rw-rw-   0        0        0     3482 2023-04-26 19:20:34.000000 epyt-1.0.3/epyt/examples/notebooks/Plt_EX2_Create_Pressure_gif.ipynb
--rw-rw-rw-   0        0        0    46523 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX2_Hydrant_rating_curve.ipynb
--rw-rw-rw-   0        0        0     4410 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX3_Minimum_chlorine_residual.ipynb
--rw-rw-rw-   0        0        0    34677 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX4_Network_Building.ipynb
--rw-rw-rw-   0        0        0    34021 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/notebooks/Toolkit_api_EX1_using_EN_functions.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.128764 epyt-1.0.3/epyt/examples/python/
--rw-rw-rw-   0        0        0     1073 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX10_close_pipes_during_sim.py
--rw-rw-rw-   0        0        0     1051 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX11_assing_new_curve_pump.py
--rw-rw-rw-   0        0        0      637 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX13c_add_cvpipe.py
--rw-rw-rw-   0        0        0     1706 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX14_hydraulic_and_quality_analysis.py
--rw-rw-rw-   0        0        0     3322 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX16_create_multiple_scenarios.py
--rw-rw-rw-   0        0        0     1795 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX17b_add_multiple_controls_pipestatus.py
--rw-rw-rw-   0        0        0     1068 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX18_change_status_pipes.py
--rw-rw-rw-   0        0        0     1381 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX1_Plot_network_topology.py
--rw-rw-rw-   0        0        0     1541 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX20a_external_controls.py
--rw-rw-rw-   0        0        0     1785 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX20b_external_controls.py
--rw-rw-rw-   0        0        0     2212 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX21_Pressure_driven_analysis_option.py
--rw-rw-rw-   0        0        0     2670 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX22_Overflow_option_for_tanks.py
--rw-rw-rw-   0        0        0      706 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX23_Change_connection_links.py
--rw-rw-rw-   0        0        0      780 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX25_set_node_name_ids.py
--rw-rw-rw-   0        0        0     2328 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX2_Hydraulic_analysis.py
--rw-rw-rw-   0        0        0     1114 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX3_Quality_analysis.py
--rw-rw-rw-   0        0        0     1926 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX4_Plot_time_series.py
--rw-rw-rw-   0        0        0      999 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX5_Plot_values_parameters.py
--rw-rw-rw-   0        0        0      907 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX6_load_two_inp_files.py
--rw-rw-rw-   0        0        0     1692 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX7_Set_Pump_Curves.py
--rw-rw-rw-   0        0        0     4114 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX9_compare_simulations.py
--rw-rw-rw-   0        0        0     2074 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/EX_to_excel_json.py
--rw-rw-rw-   0        0        0     1753 2023-04-25 21:23:54.000000 epyt-1.0.3/epyt/examples/python/Plt_EX1_Create_Flow_gif.py
--rw-rw-rw-   0        0        0     1810 2023-04-26 19:12:44.000000 epyt-1.0.3/epyt/examples/python/Plt_EX2_Create_Pressure_gif.py
--rw-rw-rw-   0        0        0     1598 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/Toolkit_EX2_Hydrant_rating_curve.py
--rw-rw-rw-   0        0        0     2141 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/Toolkit_EX3_Minimum_chlorine_residual.py
--rw-rw-rw-   0        0        0     2582 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/Toolkit_EX4_Network_Building.py
--rw-rw-rw-   0        0        0     2674 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/Toolkit_api_EX1_using_EN_functions.py
--rw-rw-rw-   0        0        0     1822 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/examples/python/desktop.ini
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.131178 epyt-1.0.3/epyt/libraries/
--rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.134947 epyt-1.0.3/epyt/libraries/glnx/
--rw-rw-rw-   0        0        0    17172 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/glnx/libepanet2_2
--rw-rw-rw-   0        0        0   385808 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/glnx/libepanet2_2.so
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.141258 epyt-1.0.3/epyt/libraries/mac/
--rw-rw-rw-   0        0        0    17172 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/mac/libepanet2_2
--rw-rw-rw-   0        0        0   325828 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/mac/libepanet2_2.dylib
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.899226 epyt-1.0.3/epyt/libraries/win/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.900634 epyt-1.0.3/epyt/libraries/win/epanet2_2/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.149853 epyt-1.0.3/epyt/libraries/win/epanet2_2/32bit/
--rw-rw-rw-   0        0        0   359936 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/win/epanet2_2/32bit/epanet2.dll
--rwxrwxrwx   0        0        0   101888 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/win/epanet2_2/32bit/epanet2.exe
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.157062 epyt-1.0.3/epyt/libraries/win/epanet2_2/64bit/
--rw-rw-rw-   0        0        0   418304 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/win/epanet2_2/64bit/epanet2.dll
--rwxrwxrwx   0        0        0   118784 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/libraries/win/epanet2_2/64bit/epanet2.exe
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.168400 epyt-1.0.3/epyt/networks/
--rw-rw-rw-   0        0        0   435227 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/BattLeDIM_Problem_Description_and_Rules.pdf
--rw-rw-rw-   0        0        0   412200 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/L-TOWN.inp
--rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.285726 epyt-1.0.3/epyt/networks/asce-tf-wdst/
--rw-rw-rw-   0        0        0    10551 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Anytown.inp
--rw-rw-rw-   0        0        0    45063 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/BWSN_Network_1.inp
--rw-rw-rw-   0        0        0  2307252 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/BWSN_Network_2.inp
--rw-rw-rw-   0        0        0   137640 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Balerma.inp
--rw-rw-rw-   0        0        0   102083 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Battle of the Calibration Networks System.inp
--rw-rw-rw-   0        0        0    10078 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Extended Hanoi.inp
--rw-rw-rw-   0        0        0    10078 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Hanoi.inp
--rw-rw-rw-   0        0        0    10169 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Jilin including water quality.inp
--rw-rw-rw-   0        0        0   419357 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/KL.inp
--rw-rw-rw-   0        0        0   408548 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/MICROPOLIS_v1.inp
--rw-rw-rw-   0        0        0    11190 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Modified New York Tunnels including water quality.inp
--rw-rw-rw-   0        0        0     6221 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1.inp
--rw-rw-rw-   0        0        0      584 2023-04-26 19:55:30.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1.txt
--rw-rw-rw-   0        0        0     6221 2023-04-26 19:55:30.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1_temp.inp
--rw-rw-rw-   0        0        0      539 2023-04-26 19:55:56.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1_temp.txt
--rw-rw-rw-   0        0        0    15603 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net2.inp
--rw-rw-rw-   0        0        0    30544 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net3.inp
--rw-rw-rw-   0        0        0    30586 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Net3_trace.inp
--rw-rw-rw-   0        0        0    10792 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/New York Tunnels including water quality.inp
--rw-rw-rw-   0        0        0   103214 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/RuralNetwork.inp
--rw-rw-rw-   0        0        0     5129 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/Sources.md
--rw-rw-rw-   0        0        0    38168 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ZJ.inp
--rw-rw-rw-   0        0        0    12327 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/foss_poly_1.inp
--rw-rw-rw-   0        0        0   215432 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky1.inp
--rw-rw-rw-   0        0        0   647316 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky10.inp
--rw-rw-rw-   0        0        0   939739 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky11.inp
--rw-rw-rw-   0        0        0   808782 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky12.inp
--rw-rw-rw-   0        0        0   277147 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky13.inp
--rw-rw-rw-   0        0        0   152077 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky14.inp
--rw-rw-rw-   0        0        0   162151 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky15.inp
--rw-rw-rw-   0        0        0   266940 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky2.inp
--rw-rw-rw-   0        0        0   104850 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky3.inp
--rw-rw-rw-   0        0        0   397447 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky4.inp
--rw-rw-rw-   0        0        0   136393 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky5.inp
--rw-rw-rw-   0        0        0   212345 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky6.inp
--rw-rw-rw-   0        0        0   197504 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky7.inp
--rw-rw-rw-   0        0        0   519148 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky8.inp
--rw-rw-rw-   0        0        0  1414844 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/asce-tf-wdst/ky9.inp
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.305071 epyt-1.0.3/epyt/networks/exeter-benchmarks/
--rw-rw-rw-   0        0        0    25904 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/Richmond_skeleton.inp
--rw-rw-rw-   0        0        0   279929 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/Richmond_standard.inp
--rw-rw-rw-   0        0        0    13227 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/anytown-exeter.inp
--rw-rw-rw-   0        0        0     5026 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/gessler1985.inp
--rw-rw-rw-   0        0        0    10099 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/hanoi-exeter.inp
--rw-rw-rw-   0        0        0     7219 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/networks/exeter-benchmarks/nytun.inp
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:17.322667 epyt-1.0.3/epyt/tests/
--rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/__init__.py
--rw-rw-rw-   0        0        0   237120 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/tests/general_unit_test.py
--rw-rw-rw-   0        0        0    22593 2023-04-25 21:17:42.000000 epyt-1.0.3/epyt/tests/net1_unit_test.py
--rw-rw-rw-   0        0        0    22064 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/testFunctions.py
--rw-rw-rw-   0        0        0     3236 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/testFunctions_2.py
--rw-rw-rw-   0        0        0    14997 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/testFunctions_ex.py
--rw-rw-rw-   0        0        0     4523 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/testGetSetLinks.py
--rw-rw-rw-   0        0        0     7475 2023-04-25 21:16:32.000000 epyt-1.0.3/epyt/tests/testGetSetNodes.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:55:16.950224 epyt-1.0.3/epyt.egg-info/
--rw-rw-rw-   0        0        0    42656 2023-04-26 20:55:16.000000 epyt-1.0.3/epyt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6026 2023-04-26 20:55:16.000000 epyt-1.0.3/epyt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:55:16.000000 epyt-1.0.3/epyt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 20:55:16.000000 epyt-1.0.3/epyt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-26 20:55:16.000000 epyt-1.0.3/epyt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-04-25 21:16:32.000000 epyt-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 20:55:17.327432 epyt-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1865 2023-04-25 19:34:47.000000 epyt-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.864019 epyt-1.0.4/
+-rw-rw-rw-   0        0        0    13984 2023-04-25 21:16:32.000000 epyt-1.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      439 2023-04-25 21:16:32.000000 epyt-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    42656 2023-04-26 21:58:45.863124 epyt-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    41720 2023-04-25 21:17:42.000000 epyt-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.564751 epyt-1.0.4/epyt/
+-rw-rw-rw-   0        0        0       55 2023-04-26 11:19:41.000000 epyt-1.0.4/epyt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.607451 epyt-1.0.4/epyt/__pycache__/
+-rw-rw-rw-   0        0        0      204 2023-04-26 19:07:56.000000 epyt-1.0.4/epyt/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      208 2023-04-26 15:27:40.000000 epyt-1.0.4/epyt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0   448735 2023-04-26 19:52:17.000000 epyt-1.0.4/epyt/__pycache__/epanet.cpython-37.pyc
+-rw-rw-rw-   0        0        0   447297 2023-04-26 15:27:40.000000 epyt-1.0.4/epyt/__pycache__/epanet.cpython-39.pyc
+-rw-rw-rw-   0        0        0   515504 2023-04-26 21:56:42.000000 epyt-1.0.4/epyt/epanet.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.611240 epyt-1.0.4/epyt/examples/
+-rw-rw-rw-   0        0        0     4154 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/examples/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.675196 epyt-1.0.4/epyt/examples/notebooks/
+-rw-rw-rw-   0        0        0     4071 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX10_close_pipes_during_sim.ipynb
+-rw-rw-rw-   0        0        0     3169 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX11_assing_new_curve_pump.ipynb
+-rw-rw-rw-   0        0        0    61390 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX13c_add_cvpipe.ipynb
+-rw-rw-rw-   0        0        0    26991 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX14_hydraulic_and_quality_analysis.ipynb
+-rw-rw-rw-   0        0        0   744778 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX16_create_multiple_scenarios.ipynb
+-rw-rw-rw-   0        0        0   211279 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX17b_add_multiple_controls_pipestatus.ipynb
+-rw-rw-rw-   0        0        0   198828 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX18_change_status_pipes.ipynb
+-rw-rw-rw-   0        0        0   316856 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX1_Plot_network_topology.ipynb
+-rw-rw-rw-   0        0        0    67212 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX20a_external_controls.ipynb
+-rw-rw-rw-   0        0        0    68755 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX20b_external_controls.ipynb
+-rw-rw-rw-   0        0        0     4757 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX21_Pressure_driven_analysis_option.ipynb
+-rw-rw-rw-   0        0        0     5397 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX22_Overflow_option_for_tanks.ipynb
+-rw-rw-rw-   0        0        0     2619 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX23_Change_connection_links.ipynb
+-rw-rw-rw-   0        0        0     2989 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX25_set_node_name_ids.ipynb
+-rw-rw-rw-   0        0        0  4818817 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX2_Hydraulic_analysis.ipynb
+-rw-rw-rw-   0        0        0   387195 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX3_Quality_analysis.ipynb
+-rw-rw-rw-   0        0        0   417836 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX4_Plot_time_series.ipynb
+-rw-rw-rw-   0        0        0   119797 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX5_Plot_values_parameters.ipynb
+-rw-rw-rw-   0        0        0    80478 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX6_load_two_inp_files.ipynb
+-rw-rw-rw-   0        0        0    67273 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX7_Set_Pump_Curves.ipynb
+-rw-rw-rw-   0        0        0   409890 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/EX9_compare_simulations.ipynb
+-rw-rw-rw-   0        0        0     3466 2023-04-26 21:06:00.000000 epyt-1.0.4/epyt/examples/notebooks/Plt_EX1_Create_Flow_gif.ipynb
+-rw-rw-rw-   0        0        0     3485 2023-04-26 21:06:00.000000 epyt-1.0.4/epyt/examples/notebooks/Plt_EX2_Create_Pressure_gif.ipynb
+-rw-rw-rw-   0        0        0    46523 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX2_Hydrant_rating_curve.ipynb
+-rw-rw-rw-   0        0        0     4410 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX3_Minimum_chlorine_residual.ipynb
+-rw-rw-rw-   0        0        0    34677 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX4_Network_Building.ipynb
+-rw-rw-rw-   0        0        0    34021 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/notebooks/Toolkit_api_EX1_using_EN_functions.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.725393 epyt-1.0.4/epyt/examples/python/
+-rw-rw-rw-   0        0        0     1073 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX10_close_pipes_during_sim.py
+-rw-rw-rw-   0        0        0     1051 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX11_assing_new_curve_pump.py
+-rw-rw-rw-   0        0        0      637 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX13c_add_cvpipe.py
+-rw-rw-rw-   0        0        0     1706 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX14_hydraulic_and_quality_analysis.py
+-rw-rw-rw-   0        0        0     3322 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX16_create_multiple_scenarios.py
+-rw-rw-rw-   0        0        0     1795 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX17b_add_multiple_controls_pipestatus.py
+-rw-rw-rw-   0        0        0     1068 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX18_change_status_pipes.py
+-rw-rw-rw-   0        0        0     1381 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX1_Plot_network_topology.py
+-rw-rw-rw-   0        0        0     1541 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX20a_external_controls.py
+-rw-rw-rw-   0        0        0     1785 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX20b_external_controls.py
+-rw-rw-rw-   0        0        0     2212 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX21_Pressure_driven_analysis_option.py
+-rw-rw-rw-   0        0        0     2670 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX22_Overflow_option_for_tanks.py
+-rw-rw-rw-   0        0        0      706 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX23_Change_connection_links.py
+-rw-rw-rw-   0        0        0      780 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX25_set_node_name_ids.py
+-rw-rw-rw-   0        0        0     2328 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX2_Hydraulic_analysis.py
+-rw-rw-rw-   0        0        0     1114 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX3_Quality_analysis.py
+-rw-rw-rw-   0        0        0     1926 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX4_Plot_time_series.py
+-rw-rw-rw-   0        0        0      999 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX5_Plot_values_parameters.py
+-rw-rw-rw-   0        0        0      907 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX6_load_two_inp_files.py
+-rw-rw-rw-   0        0        0     1692 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX7_Set_Pump_Curves.py
+-rw-rw-rw-   0        0        0     4114 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX9_compare_simulations.py
+-rw-rw-rw-   0        0        0     2074 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/EX_to_excel_json.py
+-rw-rw-rw-   0        0        0     1753 2023-04-25 21:23:54.000000 epyt-1.0.4/epyt/examples/python/Plt_EX1_Create_Flow_gif.py
+-rw-rw-rw-   0        0        0     1810 2023-04-26 19:12:44.000000 epyt-1.0.4/epyt/examples/python/Plt_EX2_Create_Pressure_gif.py
+-rw-rw-rw-   0        0        0     1598 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/Toolkit_EX2_Hydrant_rating_curve.py
+-rw-rw-rw-   0        0        0     2141 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/Toolkit_EX3_Minimum_chlorine_residual.py
+-rw-rw-rw-   0        0        0     2582 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/Toolkit_EX4_Network_Building.py
+-rw-rw-rw-   0        0        0     2674 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/Toolkit_api_EX1_using_EN_functions.py
+-rw-rw-rw-   0        0        0     1822 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/examples/python/desktop.ini
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.728478 epyt-1.0.4/epyt/libraries/
+-rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.731632 epyt-1.0.4/epyt/libraries/glnx/
+-rw-rw-rw-   0        0        0    17172 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/glnx/libepanet2_2
+-rw-rw-rw-   0        0        0   385808 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/glnx/libepanet2_2.so
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.735916 epyt-1.0.4/epyt/libraries/mac/
+-rw-rw-rw-   0        0        0    17172 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/mac/libepanet2_2
+-rw-rw-rw-   0        0        0   325828 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/mac/libepanet2_2.dylib
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.549147 epyt-1.0.4/epyt/libraries/win/
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.550139 epyt-1.0.4/epyt/libraries/win/epanet2_2/
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.739383 epyt-1.0.4/epyt/libraries/win/epanet2_2/32bit/
+-rw-rw-rw-   0        0        0   359936 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/win/epanet2_2/32bit/epanet2.dll
+-rwxrwxrwx   0        0        0   101888 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/win/epanet2_2/32bit/epanet2.exe
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.744446 epyt-1.0.4/epyt/libraries/win/epanet2_2/64bit/
+-rw-rw-rw-   0        0        0   418304 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/win/epanet2_2/64bit/epanet2.dll
+-rwxrwxrwx   0        0        0   118784 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/libraries/win/epanet2_2/64bit/epanet2.exe
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.751518 epyt-1.0.4/epyt/networks/
+-rw-rw-rw-   0        0        0   435227 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/BattLeDIM_Problem_Description_and_Rules.pdf
+-rw-rw-rw-   0        0        0   412200 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/L-TOWN.inp
+-rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.832745 epyt-1.0.4/epyt/networks/asce-tf-wdst/
+-rw-rw-rw-   0        0        0    10551 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Anytown.inp
+-rw-rw-rw-   0        0        0    45063 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/BWSN_Network_1.inp
+-rw-rw-rw-   0        0        0  2307252 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/BWSN_Network_2.inp
+-rw-rw-rw-   0        0        0   137640 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Balerma.inp
+-rw-rw-rw-   0        0        0   102083 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Battle of the Calibration Networks System.inp
+-rw-rw-rw-   0        0        0    10078 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Extended Hanoi.inp
+-rw-rw-rw-   0        0        0    10078 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Hanoi.inp
+-rw-rw-rw-   0        0        0    10169 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Jilin including water quality.inp
+-rw-rw-rw-   0        0        0   419357 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/KL.inp
+-rw-rw-rw-   0        0        0   408548 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/MICROPOLIS_v1.inp
+-rw-rw-rw-   0        0        0    11190 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Modified New York Tunnels including water quality.inp
+-rw-rw-rw-   0        0        0     6221 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1.inp
+-rw-rw-rw-   0        0        0     6221 2023-04-26 19:55:30.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1_temp.inp
+-rw-rw-rw-   0        0        0      539 2023-04-26 19:55:56.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1_temp.txt
+-rw-rw-rw-   0        0        0    15603 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net2.inp
+-rw-rw-rw-   0        0        0    30544 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net3.inp
+-rw-rw-rw-   0        0        0    30586 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Net3_trace.inp
+-rw-rw-rw-   0        0        0    10792 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/New York Tunnels including water quality.inp
+-rw-rw-rw-   0        0        0   103214 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/RuralNetwork.inp
+-rw-rw-rw-   0        0        0     5129 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/Sources.md
+-rw-rw-rw-   0        0        0    38168 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ZJ.inp
+-rw-rw-rw-   0        0        0    12327 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/foss_poly_1.inp
+-rw-rw-rw-   0        0        0   215432 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky1.inp
+-rw-rw-rw-   0        0        0   647316 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky10.inp
+-rw-rw-rw-   0        0        0   939739 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky11.inp
+-rw-rw-rw-   0        0        0   808782 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky12.inp
+-rw-rw-rw-   0        0        0   277147 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky13.inp
+-rw-rw-rw-   0        0        0   152077 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky14.inp
+-rw-rw-rw-   0        0        0   162151 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky15.inp
+-rw-rw-rw-   0        0        0   266940 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky2.inp
+-rw-rw-rw-   0        0        0   104850 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky3.inp
+-rw-rw-rw-   0        0        0   397447 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky4.inp
+-rw-rw-rw-   0        0        0   136393 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky5.inp
+-rw-rw-rw-   0        0        0   212345 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky6.inp
+-rw-rw-rw-   0        0        0   197504 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky7.inp
+-rw-rw-rw-   0        0        0   519148 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky8.inp
+-rw-rw-rw-   0        0        0  1414844 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/asce-tf-wdst/ky9.inp
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.845559 epyt-1.0.4/epyt/networks/exeter-benchmarks/
+-rw-rw-rw-   0        0        0    25904 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/Richmond_skeleton.inp
+-rw-rw-rw-   0        0        0   279929 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/Richmond_standard.inp
+-rw-rw-rw-   0        0        0    13227 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/anytown-exeter.inp
+-rw-rw-rw-   0        0        0     5026 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/gessler1985.inp
+-rw-rw-rw-   0        0        0    10099 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/hanoi-exeter.inp
+-rw-rw-rw-   0        0        0     7219 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/networks/exeter-benchmarks/nytun.inp
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.862118 epyt-1.0.4/epyt/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/__init__.py
+-rw-rw-rw-   0        0        0   237130 2023-04-26 21:41:26.000000 epyt-1.0.4/epyt/tests/general_unit_test.py
+-rw-rw-rw-   0        0        0    22593 2023-04-25 21:17:42.000000 epyt-1.0.4/epyt/tests/net1_unit_test.py
+-rw-rw-rw-   0        0        0    22064 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/testFunctions.py
+-rw-rw-rw-   0        0        0     3236 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/testFunctions_2.py
+-rw-rw-rw-   0        0        0    14997 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/testFunctions_ex.py
+-rw-rw-rw-   0        0        0     4523 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/testGetSetLinks.py
+-rw-rw-rw-   0        0        0     7475 2023-04-25 21:16:32.000000 epyt-1.0.4/epyt/tests/testGetSetNodes.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:58:45.597370 epyt-1.0.4/epyt.egg-info/
+-rw-rw-rw-   0        0        0    42656 2023-04-26 21:58:45.000000 epyt-1.0.4/epyt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5990 2023-04-26 21:58:45.000000 epyt-1.0.4/epyt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 21:58:45.000000 epyt-1.0.4/epyt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-26 21:58:45.000000 epyt-1.0.4/epyt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-26 21:58:45.000000 epyt-1.0.4/epyt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-04-25 21:16:32.000000 epyt-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 21:58:45.864019 epyt-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1865 2023-04-26 21:56:10.000000 epyt-1.0.4/setup.py
```

### Comparing `epyt-1.0.3/LICENSE.md` & `epyt-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/PKG-INFO` & `epyt-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyt
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python module for EPANET water distribution simulation libraries. The EPyT is inspired by the EPANET-Matlab Toolkit.
 Home-page: https://github.com/OpenWaterAnalytics/EPyT
 Author: KIOS CoE
 Author-email: kiriakou.marios@ucy.ac.cy
 Project-URL: Bug Tracker, https://github.com/OpenWaterAnalytics/EPyT/issues
 Keywords: epanet,water,networks,hydraulics,quality,simulations,emt,epanet matlab toolkit
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epyt Version: 1.0.3 Summary: A Python module for
+Metadata-Version: 2.1 Name: epyt Version: 1.0.4 Summary: A Python module for
 EPANET water distribution simulation libraries. The EPyT is inspired by the
 EPANET-Matlab Toolkit. Home-page: https://github.com/OpenWaterAnalytics/EPyT
 Author: KIOS CoE Author-email: kiriakou.marios@ucy.ac.cy Project-URL: Bug
 Tracker, https://github.com/OpenWaterAnalytics/EPyT/issues Keywords:
 epanet,water,networks,hydraulics,quality,simulations,emt,epanet matlab toolkit
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `epyt-1.0.3/README.md` & `epyt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/__pycache__/epanet.cpython-37.pyc` & `epyt-1.0.4/epyt/__pycache__/epanet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/__pycache__/epanet.cpython-39.pyc` & `epyt-1.0.4/epyt/__pycache__/epanet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/epanet.py` & `epyt-1.0.4/epyt/epanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
                              'STATUS', 'SETTING', 'POWER', 'TIME',
                              'CLOCKTIME', 'FILLTIME', 'DRAINTIME']
         # Constants for rule-based controls: '=', '~=', '<=' etc.
         self.RULEOPERATOR = ['=', '~=', '<=', '>=', '<', '>', 'IS',
                              'NOT', 'BELOW', 'ABOVE']
 
         # Initial attributes
-        self.classversion = '1.0.3'
+        self.classversion = '1.0.4'
         self.api = epanetapi(version)
         print(f'EPANET version {self.getVersion()} '
               f'loaded (EPyT version {self.classversion}).')
 
         # ToolkitConstants: Contains all parameters from epanet2_2.h
         self.ToolkitConstants = ToolkitConstants()
         self.api.solve = 0
```

### Comparing `epyt-1.0.3/epyt/examples/README.md` & `epyt-1.0.4/epyt/examples/README.md`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX10_close_pipes_during_sim.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX10_close_pipes_during_sim.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX11_assing_new_curve_pump.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX11_assing_new_curve_pump.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX13c_add_cvpipe.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX13c_add_cvpipe.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX14_hydraulic_and_quality_analysis.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX14_hydraulic_and_quality_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX16_create_multiple_scenarios.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX16_create_multiple_scenarios.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX17b_add_multiple_controls_pipestatus.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX17b_add_multiple_controls_pipestatus.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX18_change_status_pipes.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX18_change_status_pipes.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX1_Plot_network_topology.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX1_Plot_network_topology.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX20a_external_controls.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX20a_external_controls.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX20b_external_controls.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX20b_external_controls.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX21_Pressure_driven_analysis_option.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX21_Pressure_driven_analysis_option.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX22_Overflow_option_for_tanks.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX22_Overflow_option_for_tanks.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX23_Change_connection_links.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX23_Change_connection_links.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX25_set_node_name_ids.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX25_set_node_name_ids.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX2_Hydraulic_analysis.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX2_Hydraulic_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX3_Quality_analysis.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX3_Quality_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX4_Plot_time_series.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX4_Plot_time_series.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX5_Plot_values_parameters.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX5_Plot_values_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX6_load_two_inp_files.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX6_load_two_inp_files.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX7_Set_Pump_Curves.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX7_Set_Pump_Curves.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/EX9_compare_simulations.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/EX9_compare_simulations.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Plt_EX1_Create_Flow_gif.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Plt_EX1_Create_Flow_gif.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9685763888888889%*

 * *Differences: {"'cells'": "{1: {'execution_count': 5, 'outputs': {0: {'text': {insert: [(0, 'EPANET version "*

 * *            "20200 loaded (EPyT version 0.0.1).\\n')], delete: [0]}}}}, 2: {'execution_count': "*

 * *            "None, 'outputs': []}, delete: [4]}"}*

```diff
@@ -18,68 +18,42 @@
                 "* Create pngs for every timepoint.\n",
                 "* Create gif from all the pngs.\n",
                 "* Unload library.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 5,
             "id": "6c4b2e12",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "EPANET version 20200 loaded (EPyT version 1.0.2).\n",
+                        "EPANET version 20200 loaded (EPyT version 0.0.1).\n",
                         "Input File Net1.inp loaded successfully.\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "from epyt import epanet\n",
                 "# Load network Net1\n",
                 "d = epanet('Net1.inp')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "id": "87c16580",
             "metadata": {
                 "scrolled": true
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\n",
-                        "Creating flow gif...\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "C:\\Users\\mkiri\\AppData\\Local\\Temp\\ipykernel_1860\\1967043197.py:37: DeprecationWarning: Starting with ImageIO v3 the behavior of this function will switch to that of iio.v3.imread. To keep the current behavior (and make this warning disappear) use `import imageio.v2 as imageio` or call `imageio.v2.imread` directly.\n",
-                        "  image = imageio.imread(fig)\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Net1_flows.gif has created.\n",
-                        "Close toolkit for the input file \"Net1\". EPANET Toolkit is unloaded.\n",
-                        "\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "from PIL import Image\n",
                 "import imageio\n",
                 "import os\n",
                 "\n",
                 "# Set gif name \n",
@@ -131,23 +105,14 @@
         {
             "cell_type": "markdown",
             "id": "0c4c207d",
             "metadata": {},
             "source": [
                 "![SegmentLocal](Net1_flows.gif \"segment\")"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {
-                "collapsed": false
-            },
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Plt_EX2_Create_Pressure_gif.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Plt_EX2_Create_Pressure_gif.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998914930555556%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(8, '# Run Hyraulic analysis    \\n')], delete: [8]}}}"}*

```diff
@@ -55,15 +55,15 @@
                 "from PIL import Image\n",
                 "import imageio\n",
                 "import os\n",
                 "\n",
                 "# Set gif name \n",
                 "new_gif_name = f'{d.netName[:-4]}_pressures.gif'\n",
                 "\n",
-                "# Run Hydraulic analysis\n",
+                "# Run Hyraulic analysis    \n",
                 "comp_analysis_vals = d.getComputedTimeSeries()\n",
                 "pressures = comp_analysis_vals.Pressure\n",
                 "Time = comp_analysis_vals.Time/3600\n",
                 "\n",
                 "# Set the colorbar values based on the min/max of all the Pressure values\n",
                 "minPressure = d.min(pressures)\n",
                 "maxPressure = d.max(pressures)\n",
```

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX2_Hydrant_rating_curve.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX2_Hydrant_rating_curve.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX3_Minimum_chlorine_residual.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX3_Minimum_chlorine_residual.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Toolkit_EX4_Network_Building.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Toolkit_EX4_Network_Building.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/notebooks/Toolkit_api_EX1_using_EN_functions.ipynb` & `epyt-1.0.4/epyt/examples/notebooks/Toolkit_api_EX1_using_EN_functions.ipynb`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX10_close_pipes_during_sim.py` & `epyt-1.0.4/epyt/examples/python/EX10_close_pipes_during_sim.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX11_assing_new_curve_pump.py` & `epyt-1.0.4/epyt/examples/python/EX11_assing_new_curve_pump.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX13c_add_cvpipe.py` & `epyt-1.0.4/epyt/examples/python/EX13c_add_cvpipe.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX14_hydraulic_and_quality_analysis.py` & `epyt-1.0.4/epyt/examples/python/EX14_hydraulic_and_quality_analysis.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX16_create_multiple_scenarios.py` & `epyt-1.0.4/epyt/examples/python/EX16_create_multiple_scenarios.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX17b_add_multiple_controls_pipestatus.py` & `epyt-1.0.4/epyt/examples/python/EX17b_add_multiple_controls_pipestatus.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX18_change_status_pipes.py` & `epyt-1.0.4/epyt/examples/python/EX18_change_status_pipes.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX1_Plot_network_topology.py` & `epyt-1.0.4/epyt/examples/python/EX1_Plot_network_topology.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX20a_external_controls.py` & `epyt-1.0.4/epyt/examples/python/EX20a_external_controls.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX20b_external_controls.py` & `epyt-1.0.4/epyt/examples/python/EX20b_external_controls.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX21_Pressure_driven_analysis_option.py` & `epyt-1.0.4/epyt/examples/python/EX21_Pressure_driven_analysis_option.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX22_Overflow_option_for_tanks.py` & `epyt-1.0.4/epyt/examples/python/EX22_Overflow_option_for_tanks.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX23_Change_connection_links.py` & `epyt-1.0.4/epyt/examples/python/EX23_Change_connection_links.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX25_set_node_name_ids.py` & `epyt-1.0.4/epyt/examples/python/EX25_set_node_name_ids.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX2_Hydraulic_analysis.py` & `epyt-1.0.4/epyt/examples/python/EX2_Hydraulic_analysis.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX3_Quality_analysis.py` & `epyt-1.0.4/epyt/examples/python/EX3_Quality_analysis.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX4_Plot_time_series.py` & `epyt-1.0.4/epyt/examples/python/EX4_Plot_time_series.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX5_Plot_values_parameters.py` & `epyt-1.0.4/epyt/examples/python/EX5_Plot_values_parameters.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX6_load_two_inp_files.py` & `epyt-1.0.4/epyt/examples/python/EX6_load_two_inp_files.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX7_Set_Pump_Curves.py` & `epyt-1.0.4/epyt/examples/python/EX7_Set_Pump_Curves.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX9_compare_simulations.py` & `epyt-1.0.4/epyt/examples/python/EX9_compare_simulations.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/EX_to_excel_json.py` & `epyt-1.0.4/epyt/examples/python/EX_to_excel_json.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Plt_EX1_Create_Flow_gif.py` & `epyt-1.0.4/epyt/examples/python/Plt_EX1_Create_Flow_gif.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Plt_EX2_Create_Pressure_gif.py` & `epyt-1.0.4/epyt/examples/python/Plt_EX2_Create_Pressure_gif.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Toolkit_EX2_Hydrant_rating_curve.py` & `epyt-1.0.4/epyt/examples/python/Toolkit_EX2_Hydrant_rating_curve.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Toolkit_EX3_Minimum_chlorine_residual.py` & `epyt-1.0.4/epyt/examples/python/Toolkit_EX3_Minimum_chlorine_residual.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Toolkit_EX4_Network_Building.py` & `epyt-1.0.4/epyt/examples/python/Toolkit_EX4_Network_Building.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/Toolkit_api_EX1_using_EN_functions.py` & `epyt-1.0.4/epyt/examples/python/Toolkit_api_EX1_using_EN_functions.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/examples/python/desktop.ini` & `epyt-1.0.4/epyt/examples/python/desktop.ini`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/glnx/libepanet2_2` & `epyt-1.0.4/epyt/libraries/glnx/libepanet2_2`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/glnx/libepanet2_2.so` & `epyt-1.0.4/epyt/libraries/glnx/libepanet2_2.so`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/mac/libepanet2_2` & `epyt-1.0.4/epyt/libraries/mac/libepanet2_2`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/mac/libepanet2_2.dylib` & `epyt-1.0.4/epyt/libraries/mac/libepanet2_2.dylib`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/win/epanet2_2/32bit/epanet2.dll` & `epyt-1.0.4/epyt/libraries/win/epanet2_2/32bit/epanet2.dll`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/win/epanet2_2/32bit/epanet2.exe` & `epyt-1.0.4/epyt/libraries/win/epanet2_2/32bit/epanet2.exe`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/win/epanet2_2/64bit/epanet2.dll` & `epyt-1.0.4/epyt/libraries/win/epanet2_2/64bit/epanet2.dll`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/libraries/win/epanet2_2/64bit/epanet2.exe` & `epyt-1.0.4/epyt/libraries/win/epanet2_2/64bit/epanet2.exe`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/BattLeDIM_Problem_Description_and_Rules.pdf` & `epyt-1.0.4/epyt/networks/BattLeDIM_Problem_Description_and_Rules.pdf`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/L-TOWN.inp` & `epyt-1.0.4/epyt/networks/L-TOWN.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Anytown.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Anytown.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/BWSN_Network_1.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/BWSN_Network_1.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/BWSN_Network_2.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/BWSN_Network_2.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Balerma.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Balerma.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Battle of the Calibration Networks System.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Battle of the Calibration Networks System.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Extended Hanoi.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Extended Hanoi.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Hanoi.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Hanoi.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Jilin including water quality.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Jilin including water quality.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/KL.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/KL.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/MICROPOLIS_v1.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/MICROPOLIS_v1.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Modified New York Tunnels including water quality.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Modified New York Tunnels including water quality.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1.txt` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1_temp.txt`

 * *Files 25% similar despite different names*

```diff
@@ -4,9 +4,7 @@
   *                           E P A N E T                          *
   *                   Hydraulic and Water Quality                  *
   *                   Analysis for Pipe Networks                   *
   *                         Version 2.2                            *
   ******************************************************************
   
   Analysis begun Wed Apr 26 22:55:30 2023
-
-  Analysis ended Wed Apr 26 22:55:30 2023
```

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net1_temp.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net1_temp.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net2.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net2.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net3.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net3.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Net3_trace.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Net3_trace.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/New York Tunnels including water quality.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/New York Tunnels including water quality.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/RuralNetwork.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/RuralNetwork.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/Sources.md` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/Sources.md`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ZJ.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ZJ.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/foss_poly_1.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/foss_poly_1.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky1.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky1.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky10.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky10.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky11.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky11.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky12.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky12.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky13.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky13.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky14.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky14.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky15.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky15.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky2.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky2.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky3.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky3.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky4.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky4.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky5.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky5.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky6.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky6.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky7.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky7.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky8.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky8.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/asce-tf-wdst/ky9.inp` & `epyt-1.0.4/epyt/networks/asce-tf-wdst/ky9.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/Richmond_skeleton.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/Richmond_skeleton.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/Richmond_standard.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/Richmond_standard.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/anytown-exeter.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/anytown-exeter.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/gessler1985.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/gessler1985.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/hanoi-exeter.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/hanoi-exeter.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/networks/exeter-benchmarks/nytun.inp` & `epyt-1.0.4/epyt/networks/exeter-benchmarks/nytun.inp`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/general_unit_test.py` & `epyt-1.0.4/epyt/tests/general_unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,15 +982,15 @@
                          'Wrong Initial quality value')
 
     def test_getNodeJunctionData(self):
         """ ---getNodeJunctionDemandIndex---    """
         d = epanet('BWSN_Network_1.inp')
         err_msg = 'Wrong Junction Demand Index output'
         self.assertEqual(d.getNodeJunctionDemandIndex(1, ''), 1, err_msg)
-        self.assertEqual(d.getNodeJunctionDemandIndex([1, 2, 3]), [[0, 0, 0], [1, 1, 1]], err_msg)
+        self.assertEqual(d.getNodeJunctionDemandIndex([1, 2, 3]), [[1, 1, 1], [1, 1, 1]], err_msg)
         d.unload()
 
         """ ---getNodeJunctionDemandName---    """
         err_msg = 'Wrong Junction Demand Name ID output'
         self.assertDictEqual(self.epanetClass.getNodeJunctionDemandName(), {1: ['', '', '', '', '', '', '', '', '']},
                              err_msg)
 
@@ -1262,15 +1262,15 @@
         actual_quality_info_dict = self.epanetClass.getQualityInfo().to_dict()
         self.assertDictEqual(actual_quality_info_dict, desired_quality_info_dict, 'Wrong Quality Info Output')
 
     def test_getRuleInfo(self):
         d = epanet('BWSN_Network_1.inp')
 
         """ ---getRuleID---    """
-        self.assertEqual(d.getRuleID(), ['RULE-0', 'RULE-1', 'RULE-3'], 'Wrong Rule ID Output')
+        self.assertEqual(d.getRuleID(), ['RULE-0', 'RULE-1', 'RULE-3', 'RULE-4'], 'Wrong Rule ID Output')
 
         """ ---getRuleInfo---    """
         desired_rule_info = {'Index': [1, 2, 3, 4], 'Premises': [1, 1, 1, 1], 'ThenActions': [1, 1, 1, 1],
                              'ElseActions': [0, 0, 0, 0], 'Priority': [1.0, 1.0, 1.0, 1.0]}
         actual_rule_info = d.getRuleInfo().to_dict()
         self.assertDictEqual(actual_rule_info, desired_rule_info, 'Wrong Rule Info Output')
```

### Comparing `epyt-1.0.3/epyt/tests/net1_unit_test.py` & `epyt-1.0.4/epyt/tests/net1_unit_test.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/testFunctions.py` & `epyt-1.0.4/epyt/tests/testFunctions.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/testFunctions_2.py` & `epyt-1.0.4/epyt/tests/testFunctions_2.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/testFunctions_ex.py` & `epyt-1.0.4/epyt/tests/testFunctions_ex.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/testGetSetLinks.py` & `epyt-1.0.4/epyt/tests/testGetSetLinks.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt/tests/testGetSetNodes.py` & `epyt-1.0.4/epyt/tests/testGetSetNodes.py`

 * *Files identical despite different names*

### Comparing `epyt-1.0.3/epyt.egg-info/PKG-INFO` & `epyt-1.0.4/epyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyt
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python module for EPANET water distribution simulation libraries. The EPyT is inspired by the EPANET-Matlab Toolkit.
 Home-page: https://github.com/OpenWaterAnalytics/EPyT
 Author: KIOS CoE
 Author-email: kiriakou.marios@ucy.ac.cy
 Project-URL: Bug Tracker, https://github.com/OpenWaterAnalytics/EPyT/issues
 Keywords: epanet,water,networks,hydraulics,quality,simulations,emt,epanet matlab toolkit
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epyt Version: 1.0.3 Summary: A Python module for
+Metadata-Version: 2.1 Name: epyt Version: 1.0.4 Summary: A Python module for
 EPANET water distribution simulation libraries. The EPyT is inspired by the
 EPANET-Matlab Toolkit. Home-page: https://github.com/OpenWaterAnalytics/EPyT
 Author: KIOS CoE Author-email: kiriakou.marios@ucy.ac.cy Project-URL: Bug
 Tracker, https://github.com/OpenWaterAnalytics/EPyT/issues Keywords:
 epanet,water,networks,hydraulics,quality,simulations,emt,epanet matlab toolkit
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `epyt-1.0.3/epyt.egg-info/SOURCES.txt` & `epyt-1.0.4/epyt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 epyt/networks/asce-tf-wdst/Extended Hanoi.inp
 epyt/networks/asce-tf-wdst/Hanoi.inp
 epyt/networks/asce-tf-wdst/Jilin including water quality.inp
 epyt/networks/asce-tf-wdst/KL.inp
 epyt/networks/asce-tf-wdst/MICROPOLIS_v1.inp
 epyt/networks/asce-tf-wdst/Modified New York Tunnels including water quality.inp
 epyt/networks/asce-tf-wdst/Net1.inp
-epyt/networks/asce-tf-wdst/Net1.txt
 epyt/networks/asce-tf-wdst/Net1_temp.inp
 epyt/networks/asce-tf-wdst/Net1_temp.txt
 epyt/networks/asce-tf-wdst/Net2.inp
 epyt/networks/asce-tf-wdst/Net3.inp
 epyt/networks/asce-tf-wdst/Net3_trace.inp
 epyt/networks/asce-tf-wdst/New York Tunnels including water quality.inp
 epyt/networks/asce-tf-wdst/RuralNetwork.inp
```

### Comparing `epyt-1.0.3/setup.py` & `epyt-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 packages.append(module_name)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=module_name,
-    version="1.0.3",
+    version="1.0.4",
     author="KIOS CoE",
     author_email="kiriakou.marios@ucy.ac.cy",
     description='A Python module for EPANET water distribution simulation libraries. The EPyT is inspired by the '
                 'EPANET-Matlab Toolkit.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/OpenWaterAnalytics/EPyT',
```

