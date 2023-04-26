# Comparing `tmp/module_qc_analysis_tools-1.3.1rc2.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc3.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc2.tar` & `module_qc_analysis_tools-1.3.1rc3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MINIMUM_HEALTH.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/PIXEL_FAILURE.py
--rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/TUNING_PERFORMANCE.py
--rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     5382 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/LICENSE
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/README.md
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/pyproject.toml
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0     9228 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/LICENSE
+-rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/README.md
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/pyproject.toml
+-rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/tbump.toml` & `module_qc_analysis_tools-1.3.1rc3/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3222 0a0a  t = "1.3.1rc2"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3322 0a0a  t = "1.3.1rc3"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3220 e286 9220 7b6e 6577  .3.1rc2 ... {new
+00000150: 2e33 2e31 7263 3320 e286 9220 7b6e 6577  .3.1rc3 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MINIMUM_HEALTH.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-import json
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import typer
 from module_qc_data_tools import (
     convert_serial_to_name,
+    get_layer_from_sn,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
@@ -21,18 +21,21 @@
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     get_layer,
     perform_qc_analysis,
 )
 from module_qc_analysis_tools.utils.classification import (
+    check_input_yarr_config,
+    check_input_yarr_data,
     classify_pixels,
     count_pixels,
     format_pixel_input,
     print_pixel_classification,
+    read_json,
 )
 from module_qc_analysis_tools.utils.misc import (
     bcolors,
     get_qc_config,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
@@ -41,15 +44,14 @@
 
 
 @app.command()
 def main(
     input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     pixel_classification_path: Path = OPTIONS["pixel_classification"],
-    layer: str = OPTIONS["layer"],
     base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log.setLevel(verbosity.value)
 
     test_type = Path(__file__).stem
@@ -61,46 +63,48 @@
     log.info(" ====================================================")
     log.info("")
 
     time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    # TODO check contents of json in JSONchecker-like object
-    input_data = json.loads(input_yarr.read_text())
+    input_data = read_json(input_yarr)
+    check_input_yarr_config(input_data, path=input_yarr)
     datadir = input_data["datadir"]
+    module_sn = input_data["module"]["serialNumber"]
+    layer = get_layer_from_sn(module_sn)
 
-    # TODO check contents of json in JSONchecker-like object
-    pixel_classification = json.loads(pixel_classification_path.read_text())
+    pixel_classification = read_json(pixel_classification_path)
+
+    if not pixel_classification.get(test_type):
+        log.error(
+            bcolors.BADRED
+            + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
+            + bcolors.ENDC
+        )
+        raise RuntimeError()
 
     alloutput = []
     for c in input_data["chip"]:
         chipSN = c["serialNumber"]
         chipName = convert_serial_to_name(chipSN)
         filepaths = c["filepaths"]
         results = {}
+        skip_chip = False
 
         # Initialize array to track pixel failures
         pix_fail = np.zeros(153600, dtype=np.uint16)
 
         # Initialize int to track which classifications have been checked
         record_fail = 0
 
         log.debug(
             f"Performing minimum health test analysis on chip {c['serialNumber']}"
         )
 
-        if not pixel_classification.get(test_type):
-            log.error(
-                bcolors.BADRED
-                + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
-                + bcolors.ENDC
-            )
-            raise RuntimeError()
-
         """ Prepare output json file """
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_serial_num(chipSN)
         data = qcDataFrame()
         data.add_property(
             "ANALYSIS_VERSION",
@@ -127,45 +131,53 @@
                         + bcolors.ENDC
                     )
                     continue
                 test_params = layer_bounds
 
             # Check if we have data for that test
             if test_input not in filepaths.keys():
-                log.warning(
+                log.info(
                     bcolors.WARNING
-                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}), skipping test"
+                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). MINIMUM_HEALTH_TEST cannot be performed on this chip. Exiting."
                     + bcolors.ENDC
                 )
-                continue
+                skip_chip = True
+                break
 
             # Read input YARR scan
             input_data_path = datadir + "/" + filepaths[test_input]
-            with Path(input_data_path).open() as serialized:
-                input_data = json.load(serialized)
+            input_data = read_json(Path(input_data_path))
+            check_input_yarr_data(input_data, path=input_data_path)
 
             pix_data, pix_index = format_pixel_input(input_data.get("Data"))
 
             # Calculate relevant quantities
             if test_method == "mean":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 mean = np.mean(pix_data)
                 results.update({test_name: mean})
                 data.add_parameter("MIN_HEALTH_" + test_name, round(mean, 3))
             elif test_method == "rms":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 rms = np.std(pix_data)
                 results.update({test_name: rms})
                 data.add_parameter("MIN_HEALTH_" + test_name, round(rms, 3))
             else:
                 # Count passing pixels
                 pix_fail, record_fail = classify_pixels(
                     pix_data, pix_fail, record_fail, test_name, test_method, test_params
                 )
                 if np.isscalar(pix_fail):
                     continue
 
+        if skip_chip:
+            continue
+
         test_names = pixel_classification.get(test_type).keys()
         failure_summary = count_pixels(pix_fail, record_fail, test_names)
         for fname, nfail in failure_summary.items():
             data.add_parameter("MIN_HEALTH_" + fname, round(nfail.get("dependent"), 3))
 
         print_pixel_classification(failure_summary)
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/PIXEL_FAILURE.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-import json
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import typer
 from module_qc_data_tools import (
     convert_serial_to_name,
+    get_layer_from_sn,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
@@ -21,18 +21,21 @@
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     get_layer,
     perform_qc_analysis,
 )
 from module_qc_analysis_tools.utils.classification import (
+    check_input_yarr_config,
+    check_input_yarr_data,
     classify_pixels,
     count_pixels,
     format_pixel_input,
     print_pixel_classification,
+    read_json,
 )
 from module_qc_analysis_tools.utils.misc import (
     bcolors,
     get_qc_config,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
@@ -41,15 +44,14 @@
 
 
 @app.command()
 def main(
     input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     pixel_classification_path: Path = OPTIONS["pixel_classification"],
-    layer: str = OPTIONS["layer"],
     base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log.setLevel(verbosity.value)
 
     test_type = Path(__file__).stem
@@ -61,46 +63,47 @@
     log.info(" ====================================================")
     log.info("")
 
     time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    # TODO check contents of json in JSONchecker-like object
-    input_data = json.loads(input_yarr.read_text())
+    input_data = read_json(input_yarr)
+    check_input_yarr_config(input_data, path=input_yarr)
     datadir = input_data["datadir"]
+    module_sn = input_data["module"]["serialNumber"]
+    layer = get_layer_from_sn(module_sn)
 
-    # TODO check contents of json in JSONchecker-like object
-    pixel_classification = json.loads(pixel_classification_path.read_text())
+    pixel_classification = read_json(pixel_classification_path)
+    if not pixel_classification.get(test_type):
+        log.error(
+            bcolors.BADRED
+            + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
+            + bcolors.ENDC
+        )
+        raise RuntimeError()
 
     alloutput = []
     for c in input_data["chip"]:
         chipSN = c["serialNumber"]
         chipName = convert_serial_to_name(chipSN)
         filepaths = c["filepaths"]
         results = {}
+        skip_chip = False
 
         # Initialize array to track pixel failures
         pix_fail = np.zeros(153600, dtype=np.uint16)
 
         # Initialize int to track which classifications have been checked
         record_fail = 0
 
         log.debug(
             f"Performing minimum health test analysis on chip {c['serialNumber']}"
         )
 
-        if not pixel_classification.get(test_type):
-            log.error(
-                bcolors.BADRED
-                + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
-                + bcolors.ENDC
-            )
-            raise RuntimeError()
-
         """ Prepare output json file """
         outputDF = outputDataFrame()
         outputDF.set_test_type(test_type)
         outputDF.set_serial_num(chipSN)
         data = qcDataFrame()
         data.add_property(
             "ANALYSIS_VERSION",
@@ -127,41 +130,49 @@
                         + bcolors.ENDC
                     )
                     continue
                 test_params = layer_bounds
 
             # Check if we have data for that test
             if test_input not in filepaths.keys():
-                log.warning(
+                log.info(
                     bcolors.WARNING
-                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}), skipping test"
+                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). PIXEL_FAILURE_ANALYSIS cannot be performed on this chip. Exiting."
                     + bcolors.ENDC
                 )
-                continue
+                skip_chip = True
+                break
 
             # Read input YARR scan
             input_data_path = datadir + "/" + filepaths[test_input]
-            with Path(input_data_path).open() as serialized:
-                input_data = json.load(serialized)
+            input_data = read_json(Path(input_data_path))
+            check_input_yarr_data(input_data, path=input_data_path)
 
             pix_data, pix_index = format_pixel_input(input_data.get("Data"))
 
             # Calculate relevant quantities
             if test_method == "mean":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 results.update({"PIXEL_FAILURE_" + test_name: np.mean(pix_data)})
             elif test_method == "rms":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 results.update({"PIXEL_FAILURE_" + test_name: np.std(pix_data)})
             else:
                 log.debug(f"Classifying pixels failing {test_name}")
                 pix_fail, record_fail = classify_pixels(
                     pix_data, pix_fail, record_fail, test_name, test_method, test_params
                 )
                 if np.isscalar(pix_fail):
                     continue
 
+        if skip_chip:
+            continue
+
         test_names = pixel_classification.get(test_type).keys()
         failure_summary = count_pixels(pix_fail, record_fail, test_names)
         for fname, nfail in failure_summary.items():
             data.add_parameter(
                 "PIXEL_FAILURE_" + fname, round(nfail.get("dependent"), 3)
             )
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/TUNING_PERFORMANCE.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-import json
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import typer
 from module_qc_data_tools import (
     convert_serial_to_name,
+    get_layer_from_sn,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
@@ -21,18 +21,21 @@
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     get_layer,
     perform_qc_analysis,
 )
 from module_qc_analysis_tools.utils.classification import (
+    check_input_yarr_config,
+    check_input_yarr_data,
     classify_pixels,
     count_pixels,
     format_config_input,
     format_pixel_input,
+    read_json,
 )
 from module_qc_analysis_tools.utils.misc import (
     bcolors,
     get_qc_config,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
@@ -41,15 +44,14 @@
 
 
 @app.command()
 def main(
     input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     pixel_classification_path: Path = OPTIONS["pixel_classification"],
-    layer: str = OPTIONS["layer"],
     base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log.setLevel(verbosity.value)
 
     test_type = Path(__file__).stem
@@ -61,48 +63,49 @@
     log.info(" ====================================================")
     log.info("")
 
     time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    # TODO check contents of json in JSONchecker-like object
-    input_data = json.loads(input_yarr.read_text())
+    input_data = read_json(input_yarr)
+    check_input_yarr_config(input_data, path=input_yarr)
     datadir = input_data["datadir"]
+    module_sn = input_data["module"]["serialNumber"]
+    layer = get_layer_from_sn(module_sn)
 
-    # TODO check contents of json in JSONchecker-like object
-    pixel_classification = json.loads(pixel_classification_path.read_text())
+    pixel_classification = read_json(pixel_classification_path)
+    if not pixel_classification.get(test_type):
+        log.error(
+            bcolors.BADRED
+            + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
+            + bcolors.ENDC
+        )
+        raise RuntimeError()
 
     alloutput = []
     for c in input_data["chip"]:
         chipSN = c["serialNumber"]
         chipName = convert_serial_to_name(chipSN)
         filepaths = c["filepaths"]
         results = {}
+        skip_chip = False
 
         # Initialize array to track pixel failures
         pix_fail_tuned = np.zeros(153600, dtype=np.uint16)
         pix_fail_untuned = np.zeros(153600, dtype=np.uint16)
 
         # Initialize int to track which classifications have been checked
         record_fail_tuned = 0
         record_fail_untuned = 0
 
         log.debug(
             f"Performing minimum health test analysis on chip {c['serialNumber']}"
         )
 
-        if not pixel_classification.get(test_type):
-            log.error(
-                bcolors.BADRED
-                + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
-                + bcolors.ENDC
-            )
-            raise RuntimeError()
-
         # Loop through pixel failure tests from config file
         for test_name, params in pixel_classification.get(test_type).items():
             log.debug(f"Performing {test_name}")
 
             test_input = params.get("input")
             test_method = params.get("method")
             test_params = params.get("params")
@@ -118,39 +121,47 @@
                         + bcolors.ENDC
                     )
                     continue
                 test_params = layer_bounds
 
             # Check if we have data for that test
             if test_input not in filepaths.keys():
-                log.warning(
+                log.info(
                     bcolors.WARNING
-                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}), skipping test"
+                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). TUNING cannot be performed on this chip. Exiting."
                     + bcolors.ENDC
                 )
-                continue
+                skip_chip = True
+                break
 
             # Read input YARR scan
             input_data_path = datadir + "/" + filepaths[test_input]
-            with Path(input_data_path).open() as serialized:
-                input_data = json.load(serialized)
+            input_data = read_json(Path(input_data_path))
 
             if "TDAC" in test_name:
+                check_input_yarr_data(input_data, input_data_path, config=True)
                 pix_data, pix_index = format_config_input(
                     input_data.get("RD53B").get("PixelConfig")
                 )
             else:
+                check_input_yarr_data(input_data, input_data_path, config=False)
                 pix_data, pix_index = format_pixel_input(input_data.get("Data"))
 
             # Calculate relevant quantities
             if test_method == "mean":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 results.update({test_name: np.mean(pix_data)})
             elif test_method == "rms":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 results.update({test_name: np.std(pix_data)})
             elif test_method == "percentile":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
                 bound = (100 - test_params[0]) / 2.0
                 lower, upper = np.percentile(pix_data, [bound, 100 - bound])
                 results.update({test_name + "_LOW": lower})
                 results.update({test_name + "_HIGH": upper})
             else:
                 log.debug(f"Classifying pixels failing {test_name}")
                 if test_name == "TUNED_THRESHOLD_FAILED_FITS":
@@ -172,19 +183,20 @@
                         "THRESHOLD_FAILED_FITS",
                         test_method,
                         test_params,
                     )
                     if np.isscalar(pix_fail_untuned):
                         continue
                 else:
-                    log.error(
-                        "TUNING_PERFORMANCE not equipped to test for {test_name}. Please fix"
-                    )
+                    log.error("TUNING not equipped to test for {test_name}. Please fix")
                     raise RuntimeError()
 
+        if skip_chip:
+            continue
+
         failure_summary_tuned = count_pixels(
             pix_fail_tuned, record_fail_tuned, ["THRESHOLD_FAILED_FITS"]
         )
         results.update(
             {
                 "TUNED_THRESHOLD_FAILED_FITS": failure_summary_tuned.get(
                     "THRESHOLD_FAILED_FITS"
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 OPTIONS["layer"]: str = typer.Option(
     "Unknown",
     "-l",
     "--layer",
     help="Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2 (default)",
 )
 OPTIONS["moduleSN"]: str = typer.Option(
-    "Unknown",
+    ...,
     "-m",
     "--moduleSN",
     help="Module serial number",
 )
 OPTIONS["permodule"]: bool = typer.Option(
     False, help="Store results in one file per module (default: one file per chip)"
 )
@@ -176,19 +176,25 @@
     False,
     help="Update chip configuration even if the chip failed QC",
 )
 OPTIONS["output_yarr"]: str = typer.Option(
     None,
     "-o",
     "--output-yarr",
-    help="output directory to put info.json which will be used as input to YARR scan analysis",
+    help="output directory to put info_{TEST_NAME}.json which will be used as input to YARR scan analysis",
     exists=False,
     writable=True,
     resolve_path=True,
 )
+OPTIONS["test_name"]: Path = typer.Option(
+    ...,
+    "-t",
+    "--test-name",
+    help="Test name (MIN_HEALTH_TEST, TUNING, or PIXEL_FAILURE_ANALYSIS)",
+)
 OPTIONS["digitalscan"]: Path = typer.Option(
     None,
     "-ds",
     "--digital-scan",
     help="path to the digital scan output directory to use in YARR analysis",
     exists=True,
     readable=True,
@@ -213,7 +219,15 @@
     None,
     "-hd",
     "--threshold-scan-hd",
     help="path to the threshold scan (high-def) output directory to use in YARR analysis",
     exists=True,
     readable=True,
 )
+OPTIONS["noisescan"]: Path = typer.Option(
+    None,
+    "-ns",
+    "--noise-scan",
+    help="path to the noise scan output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS
 from module_qc_analysis_tools.cli.INJECTION_CAPACITANCE import (
     main as injection_capacitance,
 )
 from module_qc_analysis_tools.cli.IV_MEASURE import main as iv_measure
 from module_qc_analysis_tools.cli.load_yarr_scans import main as load_yarr_scans
 from module_qc_analysis_tools.cli.MASS_MEASUREMENT import main as mass
-from module_qc_analysis_tools.cli.MINIMUM_HEALTH import main as minimum_health
+from module_qc_analysis_tools.cli.MIN_HEALTH_TEST import main as min_health_test
 from module_qc_analysis_tools.cli.overwrite_config import main as overwrite_config
-from module_qc_analysis_tools.cli.PIXEL_FAILURE import main as pixel_failure
+from module_qc_analysis_tools.cli.PIXEL_FAILURE_ANALYSIS import (
+    main as pixel_failure_analysis,
+)
 from module_qc_analysis_tools.cli.SLDO import main as sldo
-from module_qc_analysis_tools.cli.TUNING_PERFORMANCE import main as tuning_performance
+from module_qc_analysis_tools.cli.TUNING import main as tuning
 from module_qc_analysis_tools.cli.update_chip_config import main as update_chip_config
 from module_qc_analysis_tools.cli.VCAL_CALIBRATION import main as vcal_calibration
 from module_qc_analysis_tools.cli.VISUAL_INSPECTION import main as visual_inspection
 
 # subcommands
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 app_analysis = typer.Typer(context_settings=CONTEXT_SETTINGS)
@@ -57,13 +59,13 @@
 app_analysis.command("vcal-calibration")(vcal_calibration)
 app_analysis.command("mass-measurement")(mass)
 app_analysis.command("iv-measure")(iv_measure)
 app_analysis.command("visual-inspection")(visual_inspection)
 app_config.command("overwrite")(overwrite_config)
 app_config.command("update")(update_chip_config)
 app_config.command("load-yarr-scans")(load_yarr_scans)
-app_config.command("minimum-health")(minimum_health)
-app_config.command("tuning-performance")(tuning_performance)
-app_config.command("pixel-failure")(pixel_failure)
+app_config.command("min-health-test")(min_health_test)
+app_config.command("tuning")(tuning)
+app_config.command("pixel-failure-analysis")(pixel_failure_analysis)
 
 # for generating documentation using mkdocs-click
 typer_click_object = typer.main.get_command(app)
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'MIN_HEALTH_TEST'": "OrderedDict([('BAD_ANALOG_INTEGRATED', [0, 153.6]), "*

 * *                      "('THRESHOLD_FAILED_FITS_INDEPENDENT', [0, 1536]), ('HIGH_ENC_INDEPENDENT', "*

 * *                      '[0, 1536])])',*

 * * "'PIXEL_FAILURE_ANALYSIS'": "OrderedDict([('ELECTRICALLY_FAILED', [0, 153.6])])",*

 * * "'TUNING'": "OrderedDict([('UNTUNED_THRESHOLD_MEAN', [1700, 2700]), "*

 * *             "('UNTUNED_THRESHOLD_FAILED_FITS', [0, 1536]), ('UNTUNED_THRESHOLD_SIGMA', [0, 400]), "*

 * *             "('TUNED_THRESHOLD_MEAN', Ord […]*

```diff
@@ -168,29 +168,29 @@
     "INJECTION_CAPACITANCE": {
         "INJ_CAPACITANCE": [
             6.74,
             9.0
         ]
     },
     "MASS_MEASUREMENT": {},
-    "MINIMUM_HEALTH": {
+    "MIN_HEALTH_TEST": {
         "BAD_ANALOG_INTEGRATED": [
             0,
             153.6
         ],
         "HIGH_ENC_INDEPENDENT": [
             0,
             1536
         ],
         "THRESHOLD_FAILED_FITS_INDEPENDENT": [
             0,
             1536
         ]
     },
-    "PIXEL_FAILURE": {
+    "PIXEL_FAILURE_ANALYSIS": {
         "ELECTRICALLY_FAILED": [
             0,
             153.6
         ]
     },
     "SLDO": {
         "SLDO_IINA": {
@@ -308,15 +308,15 @@
             ],
             "LZero": [
                 1.09,
                 1.11
             ]
         }
     },
-    "TUNING_PERFORMANCE": {
+    "TUNING": {
         "TUNED_TDAC_MEAN": [
             -1,
             1
         ],
         "TUNED_TDAC_SIGMA": [
             8.5,
             12.5
@@ -335,14 +335,22 @@
                 1100
             ]
         },
         "TUNED_THRESHOLD_SIGMA": [
             0,
             50
         ],
+        "TUNED_TOT_MEAN": [
+            6,
+            8
+        ],
+        "TUNED_TOT_SIGMA": [
+            0,
+            1
+        ],
         "UNTUNED_THRESHOLD_FAILED_FITS": [
             0,
             1536
         ],
         "UNTUNED_THRESHOLD_MEAN": [
             1700,
             2700
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('MIN_HEALTH_TEST', OrderedDict([('DEAD_DIGITAL', OrderedDict([('input', "*

 * *            "'digitalscan_OccupancyMap'), ('method', 'MinBound'), ('params', [1])])), "*

 * *            "('BAD_DIGITAL', OrderedDict([('input', 'digitalscan_OccupancyMap'), ('method', "*

 * *            "'MinMaxBound'), ('params', [98, 102])])), ('DEAD_ANALOG', OrderedDict([('input', "*

 * *            "'analogscan_OccupancyMap'), ('method', 'MinBound'), ('params', [1])])), "*

 * *            "('BAD_ANALOG', OrderedDict([('inp […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "MINIMUM_HEALTH": {
+    "MIN_HEALTH_TEST": {
         "BAD_ANALOG": {
             "input": "analogscan_OccupancyMap",
             "method": "MinMaxBound",
             "params": [
                 98,
                 102
             ]
@@ -67,17 +67,27 @@
             "method": "mean",
             "params": "null"
         },
         "THRESHOLD_SIGMA": {
             "input": "thresholdscan_hr_ThresholdMap",
             "method": "rms",
             "params": "null"
+        },
+        "TOT_MEAN": {
+            "input": "totscan_MeanTotMap",
+            "method": "mean",
+            "params": "null"
+        },
+        "TOT_SIGMA": {
+            "input": "totscan_MeanTotMap",
+            "method": "rms",
+            "params": "null"
         }
     },
-    "PIXEL_FAILURE": {
+    "PIXEL_FAILURE_ANALYSIS": {
         "BAD_ANALOG": {
             "input": "analogscan_OccupancyMap",
             "method": "MinMaxBound",
             "params": [
                 98,
                 102
             ]
@@ -100,19 +110,14 @@
         "DEAD_DIGITAL": {
             "input": "digitalscan_OccupancyMap",
             "method": "MinBound",
             "params": [
                 1
             ]
         },
-        "HIGH_CROSSTALK": {
-            "input": "",
-            "method": "",
-            "params": ""
-        },
         "HIGH_ENC": {
             "input": "thresholdscan_hd_NoiseMap",
             "method": "MaxBound",
             "params": {
                 "LOne": [
                     300
                 ],
@@ -121,27 +126,46 @@
                 ],
                 "LZero": [
                     200
                 ]
             }
         },
         "HIGH_NOISE": {
-            "input": "",
-            "method": "",
-            "params": ""
+            "input": "noisescan_NoiseOccupancy",
+            "method": "MaxBound",
+            "params": [
+                1e-05
+            ]
         },
         "TUNING_BAD": {
             "input": "thresholdscan_hd_ThresholdMap",
             "method": "Outlier",
             "params": [
                 200
             ]
         }
     },
-    "TUNING_PERFORMANCE": {
+    "TUNING": {
+        "TUNED_NOISE_95": {
+            "input": "thresholdscan_hd_NoiseMap",
+            "method": "percentile",
+            "params": [
+                95
+            ]
+        },
+        "TUNED_NOISE_MEAN": {
+            "input": "thresholdscan_hd_NoiseMap",
+            "method": "mean",
+            "params": "null"
+        },
+        "TUNED_NOISE_SIGMA": {
+            "input": "thresholdscan_hd_NoiseMap",
+            "method": "rms",
+            "params": "null"
+        },
         "TUNED_TDAC_MEAN": {
             "input": "thresholdscan_hd_Config",
             "method": "mean",
             "params": "null"
         },
         "TUNED_TDAC_SIGMA": {
             "input": "thresholdscan_hd_Config",
@@ -168,14 +192,48 @@
             "params": "null"
         },
         "TUNED_THRESHOLD_SIGMA": {
             "input": "thresholdscan_hd_ThresholdMap",
             "method": "rms",
             "params": "null"
         },
+        "TUNED_TOT_95": {
+            "input": "totscan_MeanTotMap",
+            "method": "percentile",
+            "params": [
+                95
+            ]
+        },
+        "TUNED_TOT_MEAN": {
+            "input": "totscan_MeanTotMap",
+            "method": "mean",
+            "params": "null"
+        },
+        "TUNED_TOT_SIGMA": {
+            "input": "totscan_MeanTotMap",
+            "method": "rms",
+            "params": "null"
+        },
+        "UNTUNED_NOISE_95": {
+            "input": "thresholdscan_hr_NoiseMap",
+            "method": "percentile",
+            "params": [
+                95
+            ]
+        },
+        "UNTUNED_NOISE_MEAN": {
+            "input": "thresholdscan_hr_NoiseMap",
+            "method": "mean",
+            "params": "null"
+        },
+        "UNTUNED_NOISE_SIGMA": {
+            "input": "thresholdscan_hr_NoiseMap",
+            "method": "rms",
+            "params": "null"
+        },
         "UNTUNED_TDAC_MEAN": {
             "input": "thresholdscan_hr_Config",
             "method": "mean",
             "params": "null"
         },
         "UNTUNED_TDAC_SIGMA": {
             "input": "thresholdscan_hr_Config",
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/.gitignore` & `module_qc_analysis_tools-1.3.1rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/LICENSE` & `module_qc_analysis_tools-1.3.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc2/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "Module qc analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "matplotlib",
-    "module-qc-data-tools >= 1.0.4",
+    "module-qc-data-tools >= 1.0.5rc0",
     "typer",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -43,17 +43,17 @@
 analysis-VCAL-CALIBRATION = "module_qc_analysis_tools.cli.VCAL_CALIBRATION:app"
 analysis-MASS-MEASUREMENT = "module_qc_analysis_tools.cli.MASS_MEASUREMENT:app"
 analysis-IV-MEASURE = "module_qc_analysis_tools.cli.IV_MEASURE:app"
 analysis-VISUAL-INSPECTION = "module_qc_analysis_tools.cli.VISUAL_INSPECTION:app"
 analysis-overwrite-config = "module_qc_analysis_tools.cli.overwrite_config:app"
 analysis-update-chip-config = "module_qc_analysis_tools.cli.update_chip_config:app"
 analysis-load-yarr-scans = "module_qc_analysis_tools.cli.load_yarr_scans:app"
-analysis-MINIMUM-HEALTH = "module_qc_analysis_tools.cli.MINIMUM_HEALTH:app"
-analysis-TUNING-PERFORMANCE = "module_qc_analysis_tools.cli.TUNING_PERFORMANCE:app"
-analysis-PIXEL-FAILURE = "module_qc_analysis_tools.cli.PIXEL_FAILURE:app"
+analysis-MIN-HEALTH-TEST = "module_qc_analysis_tools.cli.MIN_HEALTH_TEST:app"
+analysis-TUNING = "module_qc_analysis_tools.cli.TUNING:app"
+analysis-PIXEL-FAILURE-ANALYSIS = "module_qc_analysis_tools.cli.PIXEL_FAILURE_ANALYSIS:app"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
```

### Comparing `module_qc_analysis_tools-1.3.1rc2/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc2
+Version: 1.3.1rc3
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -29,31 +29,51 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
-Requires-Dist: module-qc-data-tools>=1.0.4
+Requires-Dist: module-qc-data-tools>=1.0.5rc0
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc2
+# module-qc-analysis-tools v1.3.1rc3
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
 data. The measurement data should be collected using the
 [module-qc-measurement-tools](https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools)
 package.
 
+## Table of contents
+
+1. [Requirements](#requirements)
+2. [Installation](#installation)
+3. [Scripts](#scripts)
+   1. [ADC calibration](#adc_calibration)
+   2. [Analog readback](#analog_readback)
+   3. [SLDOVI](#sldo)
+   4. [VCal calibration](#vcal_calibration)
+   5. [Injection capacitance](#injection_capacitance)
+   6. [Minimum health](#minimum_health)
+   7. [Tuning performance](#tuning_performance)
+   8. [Pixel failure](#pixel_failure)
+4. [Notes](#notes)
+   1. [Submit QC results](#submit-qc-results)
+   2. [Example commands](#example-commands-for-a-chip-in-a-quad-module-L2)
+   3. [Update chip config](#update-chip-config)
+   4. [Load YARR scans](#load-yarr-scans)
+5. [For developer](#for-developer)
+
 ## Requirements
 
 This tool requires users to have >python3.6 with the following packages
 installed:
 
 - `numpy`
 - `scipy`
@@ -89,24 +109,24 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc2
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc3
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
 
-### `Analyze ADC Calibration`
+### `ADC_CALIBRATION`
 
 This analysis script performs the ADC calibration. It produces several
 diagnostic plots and an output file with the ADC calibration slope and offset.
 
 <details> <summary> analysis-ADC-CALIBRATION --help </summary>
 
 ```
@@ -130,15 +150,15 @@
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
 
-### `Analyze Analog Readback`
+### `ANALOG_READBACK`
 
 This analysis script performs the Analog Readback. It produces an output file
 with the calculated internal biases, temperature from the internal and external
 temperature sensor, and VDDA/VDDD vs Trim, including diagnostic plots with slope
 and offset.
 
 <details> <summary> analysis-ANALOG-READBACK --help </summary>
@@ -166,15 +186,15 @@
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
   --verbose             verbose mode
 
 ```
 
 </details>
 
-### `Analyze SLDO`
+### `SLDO`
 
 This script analyses the SLDO curve. It produces several diagnostic plots and an
 output file with several parameters extracted from the SLDO curves.
 
 <details> <summary> analysis-SLDO --help </summary>
 
 ```
@@ -203,15 +223,15 @@
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
   --lp-enable           low power mode
 
 ```
 
 </details>
 
-### `Analyze VCal Calibration`
+### `VCAL_CALIBRATION`
 
 This analysis script performs the VCal calibration. It produces several
 diagnostic plots and an output file with the VCal calibration slope and offset.
 
 <details> <summary> analysis-VCAL-CALIBRATION --help </summary>
 
 ```
@@ -235,15 +255,15 @@
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
 
-### `Analyze Injection capacitance`
+### `INJECTION_CAPACITANCE`
 
 This analysis script performs the injection capacitance. It produces several
 diagnostic plots and an output file with the measured pixel injection
 capacitance.
 
 <details> <summary> analysis-INJECTION-CAPACITANCE --help </summary>
 
@@ -266,14 +286,142 @@
   --permodule           Store results in one file per module (default: one file per chip)
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
 
+### `MIN_HEALTH_TEST`
+
+This analysis script performs the minimum health analysis of YARR Scans. It
+produces an output file with key parameters (number of dead/bad pixels, ...).
+Note that the YARR scans to be used in the analysis should be identified with
+`analysis-load-yarr-scans`, see [Load Yarr Scans](#load-yarr-scans).
+
+<details> <summary> analysis-MIN_HEALTH_TEST --help </summary>
+
+```
+$ analysis-MIN-HEALTH-TEST -h
+Usage: analysis-MIN-HEALTH-TEST [OPTIONS]
+
+Options:
+  -i, --input-yarr-config PATH    path to the json config file containing
+                                  paths to YARR scan outputs. Run analysis-
+                                  load-yarr-scans.py to generate.  [default:
+                                  info.json]
+  -q, --qc-criteria PATH          path to json file with QC selection criteria
+                                  [default: /home/eathompson/module-qc-
+                                  analysis-tools/src/module_qc_analysis_tools/
+                                  data/analysis_cuts.json]
+  -p, --pixel-failure-config PATH
+                                  path to json file with pixel failure
+                                  selection criteria  [default:
+                                  /home/eathompson/module-qc-analysis-tools/sr
+                                  c/module_qc_analysis_tools/data/pixel_classi
+                                  fication.json]
+  -l, --layer TEXT                Layer of module, used for applying correct
+                                  QC criteria settings. Options: L0, L1, L2
+                                  (default)  [default: Unknown]
+  -o, --output-dir PATH           output directory  [default: outputs]
+  --permodule / --no-permodule    Store results in one file per module
+                                  (default: one file per chip)  [default: no-
+                                  permodule]
+  -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
+                                  Log level [options: DEBUG, INFO (default)
+                                  WARNING, ERROR]  [default: LogLevel.info]
+```
+
+</details>
+
+### `TUNING`
+
+This analysis script analyzes the tuning performance from YARR scans. It
+produces an output file with key parameters (threshold before/after tuning,
+...). Note that the YARR scans to be used in the analysis should be identified
+with `analysis-load-yarr-scans`, see [Load Yarr Scans](#load-yarr-scans).
+
+<details> <summary> analysis-TUNING --help </summary>
+
+```
+$ analysis-TUNING -h
+Usage: analysis-TUNING [OPTIONS]
+
+Options:
+  -i, --input-yarr-config PATH    path to the json config file containing
+                                  paths to YARR scan outputs. Run analysis-
+                                  load-yarr-scans.py to generate.  [default:
+                                  info.json]
+  -q, --qc-criteria PATH          path to json file with QC selection criteria
+                                  [default: /home/eathompson/module-qc-
+                                  analysis-tools/src/module_qc_analysis_tools/
+                                  data/analysis_cuts.json]
+  -p, --pixel-failure-config PATH
+                                  path to json file with pixel failure
+                                  selection criteria  [default:
+                                  /home/eathompson/module-qc-analysis-tools/sr
+                                  c/module_qc_analysis_tools/data/pixel_classi
+                                  fication.json]
+  -l, --layer TEXT                Layer of module, used for applying correct
+                                  QC criteria settings. Options: L0, L1, L2
+                                  (default)  [default: Unknown]
+  -o, --output-dir PATH           output directory  [default: outputs]
+  --permodule / --no-permodule    Store results in one file per module
+                                  (default: one file per chip)  [default: no-
+                                  permodule]
+  -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
+                                  Log level [options: DEBUG, INFO (default)
+                                  WARNING, ERROR]  [default: LogLevel.info]
+```
+
+</details>
+
+### `PIXEL_FAILURE_ANALYSIS`
+
+This analysis script classifies pixel failures and performs the pixel failure
+analysis. It produces an output file with several key parameters (number of
+pixels failing each category, total failing pixels, ...). Note that the YARR
+scans to be used in the analysis should be identified with
+`analysis-load-yarr-scans`, see [Load Yarr Scans](#load-yarr-scans).
+
+<details> <summary> analysis-PIXEL-FAILURE-ANALYSIS --help </summary>
+
+```
+$ analysis-PIXEL-FAILURE-ANALYSIS -h
+Usage: analysis-PIXEL-FAILURE-ANALYSIS [OPTIONS]
+
+Options:
+  -i, --input-yarr-config PATH    path to the json config file containing
+                                  paths to YARR scan outputs. Run analysis-
+                                  load-yarr-scans.py to generate.  [default:
+                                  info.json]
+  -q, --qc-criteria PATH          path to json file with QC selection criteria
+                                  [default: /home/eathompson/module-qc-
+                                  analysis-tools/src/module_qc_analysis_tools/
+                                  data/analysis_cuts.json]
+  -p, --pixel-failure-config PATH
+                                  path to json file with pixel failure
+                                  selection criteria  [default:
+                                  /home/eathompson/module-qc-analysis-tools/sr
+                                  c/module_qc_analysis_tools/data/pixel_classi
+                                  fication.json]
+  -l, --layer TEXT                Layer of module, used for applying correct
+                                  QC criteria settings. Options: L0, L1, L2
+                                  (default)  [default: Unknown]
+  -o, --output-dir PATH           output directory  [default: outputs]
+  --permodule / --no-permodule    Store results in one file per module
+                                  (default: one file per chip)  [default: no-
+                                  permodule]
+  -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
+                                  Log level [options: DEBUG, INFO (default)
+                                  WARNING, ERROR]  [default: LogLevel.info]
+
+```
+
+</details>
+
 ## Notes
 
 ### `Submit QC results`
 
 To submit the QC results, supply the --submit option to the analysis. You also
 need to supply the site where the testing took place, as written in production
 DB (i.e. LBNL_PIXEL_MODULES for LBNL, IRFU for Paris-Saclay, ...). This will
@@ -283,15 +431,15 @@
 can be viewed here:
 https://docs.google.com/spreadsheets/d/1pw_07F94fg2GJQr8wlvhaRUV63uhsAuBt_S1FEFBzBU/view
 . While all submitted results will be recorded, only the latest results for each
 chip / test will be analyzed. If a mistake was realized in the submitted
 results, one can re-run the analysis and re-submit the results to overwrite the
 original results.
 
-### `Example commands for a chip in a quad module (L2):`
+### `Example commands for a chip in a quad module L2`
 
 ```
 analysis-ADC-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/ADC_CALIBRATION/1000000001/ --layer L2
 analysis-SLDO -i ../module-qc-tools/emulator/outputs/Measurements/SLDO/1000000001/ --layer L2
 analysis-ANALOG-READBACK -i ../module-qc-tools/emulator/outputs/Measurements/ANALOG_READBACK/1000000001/ --layer L2
 analysis-VCAL-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/VCAL_CALIBRATION/1000000001/ --layer L2
 analysis-INJECTION-CAPACITANCE -i ../module-qc-tools/emulator/outputs/Measurements/INJECTION_CAPACITANCE/1000000001/ --layer L2
@@ -304,24 +452,49 @@
 ```
 analysis-update-chip-config -i <path to analysis output directory> -c <path to YARR config directory> -t <config type>
 ```
 
 This script reads the analysis test type and update the corresponding parameters
 in the chip config.
 
-### `JsonChecker and DataExtractor`
+### `Load YARR Scans`
 
-Two classes are designed for general purposes of the module qc analysis tool.
+Before running analysis of YARR scans (`MIN_HEALTH_TEST`, `TUNING`,
+`PIXEL_FAILURE_ANALYSIS`), the YARR scans to be analyzed need to be identified.
+This is done locally using the following script:
+
+<details> <summary> analysis-load-yarr-scans --help </summary>
+
+```
+$ analysis-load-yarr-scans -h
+Options:
+  -i, --input-yarr-scans PATH     path to the json config file containing
+                                  paths to YARR scan outputs. Run analysis-
+                                  load-yarr-scans.py to generate.
+  -o, --output-yarr PATH          output directory to put info.json which will
+                                  be used as input to YARR scan analysis
+  -m, --moduleSN TEXT             Module serial number  [default: Unknown]
+  -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
+                                  Log level [options: DEBUG, INFO (default)
+                                  WARNING, ERROR]  [default: LogLevel.info]
+  -ds, --digital-scan PATH        path to the digital scan output directory to
+                                  use in YARR analysis
+  -as, --analog-scan PATH         path to the analog scan output directory to
+                                  use in YARR analysis
+  -hr, --threshold-scan-hr PATH   path to the threshold scan (high-range)
+                                  output directory to use in YARR analysis
+  -hd, --threshold-scan-hd PATH   path to the threshold scan (high-def) output
+                                  directory to use in YARR analysis
+```
 
-1. `JsonChecker` a. Check whether the test type is implemented b. For a specific
-   task, check if required keywords exist c. Check if lengths of measurements
-   are identical d. Check if there are negative numbers of measurements
+</details>
 
-2. `DataExtractor` This class finds measurements by Vmux value and convert them
-   to quantites.
+Given a directory with YARR scans, the script will identify the latest YARR
+scans needed for all analyses. Alternatively, the paths to YARR scans for each
+type of scan can be supplied to the script.
 
 ## For Developer
 
 ### python version
 
 A python version higher than 3.7 is needed for this repository. Check the local
 python version with `python -V`.
```

