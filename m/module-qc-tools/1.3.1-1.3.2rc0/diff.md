# Comparing `tmp/module_qc_tools-1.3.1.tar.gz` & `tmp/module_qc_tools-1.3.2rc0.tar.gz`

## Comparing `module_qc_tools-1.3.1.tar` & `module_qc_tools-1.3.2rc0.tar`

### file list

```diff
@@ -1,53 +1,49 @@
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/.flake8
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/.gitmodules
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/tbump.toml
--rw-r--r--   0        0        0    40206 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/Measurements/ADC_CALIBRATION/2023-03-29_151138/20UPGXM1234567.json
--rw-r--r--   0        0        0   185470 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/Measurements/ANALOG_READBACK/2023-03-29_151125/20UPGXM1234567.json
--rw-r--r--   0        0        0    22334 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/Measurements/INJECTION_CAPACITANCE/2023-03-29_151134/20UPGXM1234567.json
--rw-r--r--   0        0        0    75466 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/Measurements/SLDO/2023-03-29_151117/20UPGXM1234567.json
--rw-r--r--   0        0        0   140154 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/Measurements/VCAL_CALIBRATION/2023-03-29_151134/20UPGXM1234567.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/emulator/README.md
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     8743 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L0.json
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L1.json
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L2.json
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/example_merged_vmux_L0.json
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/example_merged_vmux_L1.json
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/example_merged_vmux_L2.json
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/configs/example_separate_vmux_L2.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/LICENSE
--rw-r--r--   0        0        0    24587 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/README.md
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 module_qc_tools-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.flake8
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitmodules
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/tbump.toml
+-rw-r--r--   0        0        0    40218 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/ADC_CALIBRATION/2023-04-27_204040/20UPGXM1234567.json
+-rw-r--r--   0        0        0   311634 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/ANALOG_READBACK/2023-04-27_204048/20UPGXM1234567.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/INJECTION_CAPACITANCE/2023-04-27_204052/20UPGXM1234567.json
+-rw-r--r--   0        0        0    75478 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/SLDO/2023-04-27_204051/20UPGXM1234567.json
+-rw-r--r--   0        0        0   140202 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/VCAL_CALIBRATION/2023-04-27_204053/20UPGXM1234567.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/emulator/README.md
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/LICENSE
+-rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/README.md
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/pyproject.toml
+-rw-r--r--   0        0        0    25933 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/PKG-INFO
```

### Comparing `module_qc_tools-1.3.1/.gitlab-ci.yml` & `module_qc_tools-1.3.2rc0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 SLDO:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running SLDO with toy emulator..."
     - measurement-SLDO -c $(module-qc-tools
-      --prefix)/configs/emulator_merged_vmux_L2.json -o ./
+      --prefix)/configs/emulator_merged_vmux.json -o ./
     - for file in Measurements/SLDO/*/*; do echo $file; jsonschema --instance
       $file $(module-qc-tools --prefix)/schema/common.json; done
     - for file in Measurements/SLDO/*/*; do echo $file; jsonschema --instance
       $file $(module-qc-tools --prefix)/schema/SLDO.json; done
   artifacts:
     paths:
       - Measurements/SLDO/*/*.json
@@ -56,15 +56,15 @@
 
 VCAL_CALIBRATION:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running VCAL_CALIBRATION with the toy emulator..."
     - measurement-VCAL-CALIBRATION -c $(module-qc-tools
-      --prefix)/configs/emulator_merged_vmux_L2.json -o ./
+      --prefix)/configs/emulator_merged_vmux.json -o ./
     - for file in Measurements/VCAL_CALIBRATION/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/common.json; done
     - for file in Measurements/VCAL_CALIBRATION/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/VCAL_CALIBRATION.json;
       done
   artifacts:
     paths:
@@ -73,15 +73,15 @@
 
 ANALOG_READBACK:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running ANALOG_READBACK with toy emulator..."
     - measurement-ANALOG-READBACK -c $(module-qc-tools
-      --prefix)/configs/emulator_merged_vmux_L2.json -o ./
+      --prefix)/configs/emulator_merged_vmux.json -o ./
     - for file in Measurements/ANALOG_READBACK/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/common.json; done
     - for file in Measurements/ANALOG_READBACK/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/ANALOG_READBACK.json;
       done
   artifacts:
     paths:
@@ -90,15 +90,15 @@
 
 ADC_CALIBRATION:
   stage: test
   script:
     - python3 -m pip install . --no-cache-dir
     - echo "Running ADC_CALIBRATION with the toy emulator..."
     - measurement-ADC-CALIBRATION -c $(module-qc-tools
-      --prefix)/configs/emulator_merged_vmux_L2.json -o ./
+      --prefix)/configs/emulator_merged_vmux.json -o ./
     - for file in Measurements/ADC_CALIBRATION/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/common.json; done
     - for file in Measurements/ADC_CALIBRATION/*/*; do echo $file; jsonschema
       --instance $file $(module-qc-tools --prefix)/schema/ADC_CALIBRATION.json;
       done
   artifacts:
     paths:
@@ -107,15 +107,15 @@
 
 INJECTION_CAPACITANCE:
   stage: test
   script:
     - python3 -m pip install . --no-cache-dir
     - echo "Running INJECTION-CAPACITANCE with the toy emulator..."
     - measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
-      --prefix)/configs/emulator_merged_vmux_L2.json -o ./
+      --prefix)/configs/emulator_merged_vmux.json -o ./
     - for file in Measurements/INJECTION_CAPACITANCE/*/*; do echo $file;
       jsonschema --instance $file $(module-qc-tools
       --prefix)/schema/common.json; done
     - for file in Measurements/INJECTION_CAPACITANCE/*/*; do echo $file;
       jsonschema --instance $file $(module-qc-tools
       --prefix)/schema/INJECTION_CAPACITANCE.json; done
   artifacts:
```

### Comparing `module_qc_tools-1.3.1/.pre-commit-config.yaml` & `module_qc_tools-1.3.2rc0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     hooks:
       - id: check-json
       - id: trailing-whitespace
       # broken in old git from 2013
       # - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
-      - id: no-commit-to-branch
-        args: [--branch, main]
       - id: check-case-conflict
       - id: debug-statements
       - id: mixed-line-ending
       - id: check-symlinks
       - id: check-toml
       - id: check-yaml
       - id: requirements-txt-fixer
@@ -72,15 +70,15 @@
   - repo: https://github.com/asottile/blacken-docs
     rev: v1.12.1
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.3.0]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
         # args: ["-a", "from __future__ import annotations"] # Python 3.7+
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.1.0
     hooks:
```

### Comparing `module_qc_tools-1.3.1/tbump.toml` & `module_qc_tools-1.3.2rc0/tbump.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 220a 0a23 2045  t = "1.3.1"..# E
-00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
-00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
-00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
-00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
-00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
-00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
-00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
-00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
-000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
-000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
-000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
-000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
-000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
-000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
-00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
-00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
-00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
-00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 312e 332e  mp version: 1.3.
-00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
-00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
-00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
-00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
-00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
-000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
-000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
-000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
-000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
-00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
-00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
-00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
-00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
-00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
-00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
-00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
-00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
-00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
-00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
-000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
-000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
-000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
-000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
-000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
-000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
-00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
-00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
-00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
-00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
-00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
-00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
-00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
+00000010: 7420 3d20 2231 2e33 2e32 7263 3022 0a0a  t = "1.3.2rc0"..
+00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
+00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
+00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
+00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
+00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
+00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
+00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
+00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
+000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
+000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
+000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
+000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
+000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
+000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
+00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
+00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
+00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
+00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
+00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
+00000150: 2e33 2e32 7263 3020 e286 9220 7b6e 6577  .3.2rc0 ... {new
+00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
+00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
+00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
+00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
+000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
+000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
+000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
+000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
+000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
+00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
+00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
+00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
+00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
+00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
+00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
+00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
+00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
+00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
+00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
+000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
+000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
+000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
+000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
+000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
+000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
+00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
+00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
+00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
+00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
+00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
+00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
+00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
+00000380: 2222 0a                                  "".
```

### Comparing `module_qc_tools-1.3.1/Measurements/ADC_CALIBRATION/2023-03-29_151138/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc0/Measurements/ADC_CALIBRATION/2023-04-27_204040/20UPGXM1234567.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628042, 'TimeEnd': 1682628225}}}}",*

 * * '1': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628042, 'TimeEnd': 1682628225}}}}",*

 * * '2': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628042, 'TimeEnd': 1682628225}}}}",*

 * * '3': "{0: {'results […]*

```diff
@@ -246,20 +246,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102970,
-                    "TimeStart": 1680102700
+                    "TimeEnd": 1682628225,
+                    "TimeStart": 1682628042
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -510,20 +510,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102970,
-                    "TimeStart": 1680102700
+                    "TimeEnd": 1682628225,
+                    "TimeStart": 1682628042
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -774,20 +774,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102970,
-                    "TimeStart": 1680102701
+                    "TimeEnd": 1682628225,
+                    "TimeStart": 1682628042
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -1038,20 +1038,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102970,
-                    "TimeStart": 1680102701
+                    "TimeEnd": 1682628225,
+                    "TimeStart": 1682628042
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.1/Measurements/INJECTION_CAPACITANCE/2023-03-29_151134/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc0/Measurements/INJECTION_CAPACITANCE/2023-04-27_204052/20UPGXM1234567.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628054, 'TimeEnd': 1682628115}}}}",*

 * * '1': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628054, 'TimeEnd': 1682628115}}}}",*

 * * '2': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628054, 'TimeEnd': 1682628115}}}}",*

 * * ' […]*

```diff
@@ -120,20 +120,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102749,
-                    "TimeStart": 1680102696
+                    "TimeEnd": 1682628115,
+                    "TimeStart": 1682628054
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -258,20 +258,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102749,
-                    "TimeStart": 1680102696
+                    "TimeEnd": 1682628115,
+                    "TimeStart": 1682628054
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -396,20 +396,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102749,
-                    "TimeStart": 1680102696
+                    "TimeEnd": 1682628115,
+                    "TimeStart": 1682628054
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -534,20 +534,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102749,
-                    "TimeStart": 1680102696
+                    "TimeEnd": 1682628115,
+                    "TimeStart": 1682628055
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ]
```

### Comparing `module_qc_tools-1.3.1/Measurements/SLDO/2023-03-29_151117/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc0/Measurements/SLDO/2023-04-27_204051/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909855769230769%*

 * *Differences: {'0': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc0'}, 'Metadata': "*

 * *      "{'TimeStart': 1682628051, 'TimeEnd': 1682628486}}}}",*

 * * '1': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc0'}, 'Metadata': "*

 * *      "{'TimeStart': 1682628052, 'TimeEnd': 1682628486}}}}",*

 * * '2': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc0'}, 'Metadata': "*

 * *      "{'TimeStart': 1682628052, 'TimeEnd': 1682628486}}}}",*

 * * '3': "{0: {'results': {'property': {'SLDO_MEASUREMEN […]*

```diff
@@ -466,20 +466,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103143,
-                    "TimeStart": 1680102678
+                    "TimeEnd": 1682628486,
+                    "TimeStart": 1682628051
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.1"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -950,20 +950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103143,
-                    "TimeStart": 1680102678
+                    "TimeEnd": 1682628486,
+                    "TimeStart": 1682628052
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.1"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1434,20 +1434,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103143,
-                    "TimeStart": 1680102678
+                    "TimeEnd": 1682628486,
+                    "TimeStart": 1682628052
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.1"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1918,20 +1918,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103143,
-                    "TimeStart": 1680102678
+                    "TimeEnd": 1682628486,
+                    "TimeStart": 1682628052
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.1"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "SLDO"
         }
     ]
```

### Comparing `module_qc_tools-1.3.1/Measurements/VCAL_CALIBRATION/2023-03-29_151134/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc0/Measurements/VCAL_CALIBRATION/2023-04-27_204053/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, "*

 * *      "'Metadata': {'TimeStart': 1682628057, 'TimeEnd': 1682628074}}}, 1: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, 'Metadata': {'TimeStart': 1682628074, "*

 * *      "'TimeEnd': 1682628090}}}, 2: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc0'}, 'Metadata': {'TimeStart': 1682628090, "*

 * *      "'TimeEnd': 1682628107}}}, 3: {'results': {'prop […]*

```diff
@@ -202,20 +202,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102717,
-                    "TimeStart": 1680102698
+                    "TimeEnd": 1682628074,
+                    "TimeStart": 1682628057
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -420,20 +420,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102743,
-                    "TimeStart": 1680102717
+                    "TimeEnd": 1682628090,
+                    "TimeStart": 1682628074
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -638,20 +638,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102766,
-                    "TimeStart": 1680102743
+                    "TimeEnd": 1682628107,
+                    "TimeStart": 1682628090
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -856,20 +856,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102788,
-                    "TimeStart": 1680102766
+                    "TimeEnd": 1682628123,
+                    "TimeStart": 1682628107
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1076,20 +1076,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102808,
-                    "TimeStart": 1680102788
+                    "TimeEnd": 1682628140,
+                    "TimeStart": 1682628123
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1294,20 +1294,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102831,
-                    "TimeStart": 1680102808
+                    "TimeEnd": 1682628156,
+                    "TimeStart": 1682628140
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1512,20 +1512,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102856,
-                    "TimeStart": 1680102831
+                    "TimeEnd": 1682628173,
+                    "TimeStart": 1682628156
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1730,20 +1730,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102879,
-                    "TimeStart": 1680102856
+                    "TimeEnd": 1682628189,
+                    "TimeStart": 1682628173
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1950,20 +1950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102899,
-                    "TimeStart": 1680102879
+                    "TimeEnd": 1682628206,
+                    "TimeStart": 1682628189
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2168,20 +2168,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102923,
-                    "TimeStart": 1680102899
+                    "TimeEnd": 1682628222,
+                    "TimeStart": 1682628206
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2386,20 +2386,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102947,
-                    "TimeStart": 1680102923
+                    "TimeEnd": 1682628239,
+                    "TimeStart": 1682628222
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2604,20 +2604,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102969,
-                    "TimeStart": 1680102947
+                    "TimeEnd": 1682628256,
+                    "TimeStart": 1682628239
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -2824,20 +2824,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680102991,
-                    "TimeStart": 1680102969
+                    "TimeEnd": 1682628273,
+                    "TimeStart": 1682628256
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3042,20 +3042,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103011,
-                    "TimeStart": 1680102991
+                    "TimeEnd": 1682628290,
+                    "TimeStart": 1682628273
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3260,20 +3260,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103033,
-                    "TimeStart": 1680103011
+                    "TimeEnd": 1682628307,
+                    "TimeStart": 1682628290
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3478,20 +3478,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1680103054,
-                    "TimeStart": 1680103033
+                    "TimeEnd": 1682628323,
+                    "TimeStart": 1682628307
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.1/emulator/README.md` & `module_qc_tools-1.3.2rc0/emulator/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
 from module_qc_data_tools import (
+    get_env,
+    get_layer_from_sn,
     get_sn_from_connectivity,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
@@ -62,30 +64,30 @@
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
 
-def run(data, adc_calib_config, ps, yr, meter):
+def run(data, adc_calib_config, ps, yr, meter, layer):
     """The function which does the ADC calibration.
 
     Args:
         data (list): data[chip_id].
         adc_calib_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
     if yr.running_emulator():
         ps.on(
-            adc_calib_config["v_max"], adc_calib_config["i_config"]
+            adc_calib_config["v_max"], adc_calib_config["i_config"][layer]
         )  # Only for emulator do the emulation of power on/off
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     status = yr.configure()
     assert status >= 0
 
     InjVcalRange = adc_calib_config["InjVcalRange"]
@@ -140,26 +142,32 @@
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
         raise RuntimeError(
             "must supply path to connectivity file [-m --module-connectivity]"
         )
 
-    adc_calib_config = config["tasks"]["ADC_CALIBRATION"]
+    adc_calib_config = config["tasks"]["GENERAL"]
+    adc_calib_config.update(config["tasks"]["ADC_CALIBRATION"])
+
     ps = power_supply(config["power_supply"], verbose=args.verbose)
     yr = yarr(config["yarr"], verbose=args.verbose)
-
     meter = multimeter(config["multimeter"], verbose=args.verbose)
-    ps.set(v=adc_calib_config["v_max"], i=adc_calib_config["i_config"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = os.path.basename(__file__).split(".py")[0]
+    institution = get_env("INSTITUTION")
+    if institution is None:
+        institution = ""
+
+    ps.set(v=adc_calib_config["v_max"], i=adc_calib_config["i_config"][layer])
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
@@ -189,27 +197,28 @@
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].add_property(
             test_type + "_MEASUREMENT_VERSION",
             pkg_resources.get_distribution("module-qc-tools").version,
         )
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
+        data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
         data[chip]._meta_data["ChipConfigs"]["RD53B"]["GlobalConfig"][
             "InjVcalRange"
         ] = InjVcalRange
         data[chip].set_x("DACs_input", True)
 
     logging.basicConfig(level=logging.DEBUG)
     logger = logging.getLogger(__name__)
 
     try:
-        run(data, adc_calib_config, ps, yr, meter)
+        run(data, adc_calib_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         logger.exception(err)
         sys.exit(1)
 
     log.info(
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import pkg_resources
 from module_qc_data_tools import (
+    get_env,
+    get_layer_from_sn,
     get_sn_from_connectivity,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
@@ -63,15 +65,15 @@
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
 
-def run_vmeas(data, analog_readback_config, ps, yr, meter):
+def run_vmeas(data, analog_readback_config, ps, yr, meter, layer):
     """
     This function measures given internal voltages by going through all VMUX and IMUX settings provided in the config.
 
     Args:
         data (list): data[chip_id][vmux/imux_type].
         analog_readback_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
@@ -85,15 +87,15 @@
     log.info(
         f"[run_AnalogReadBack] TimeStart: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
     if yr.running_emulator():
         ps.on(
             analog_readback_config["v_max"],
-            analog_readback_config["i_config"],
+            analog_readback_config["i_config"][layer],
         )  # Only for emulator do the emulation of power on/off.
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # Reset other chips
     reset = analog_readback_config["share_vmux"]
 
     # Set and measure current for power supply
@@ -129,15 +131,15 @@
 
     log.info("[run_AnalogReadBack] V scan done!")
     log.info(
         f"[run_AnalogReadBack] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
 
-def run_tmeas(data, analog_readback_config, ps, yr, meter, nt):
+def run_tmeas(data, analog_readback_config, ps, yr, meter, nt, layer):
     """
     This function measures temperature of the NTC nad MOS sensor though VMUX and IMUX settings provided in the config.
 
     Args:
         data (list): data[chip_id][vmux/imux_type or bias/dem].
         analog_readback_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
@@ -151,15 +153,15 @@
     log.info(
         f"[run_AnalogReadBack] TimeStart: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
     if yr.running_emulator():
         ps.on(
             analog_readback_config["v_max"],
-            analog_readback_config["i_config"],
+            analog_readback_config["i_config"][layer],
         )  # Only for emulator do the emulation of power on/off.
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # Reset other chips
     reset = analog_readback_config["share_vmux"]
 
     # Chip config mapping
@@ -247,15 +249,15 @@
 
     log.info("[run_AnalogReadBack] T measurement done!")
     log.info(
         f"[run_AnalogReadBack] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
 
-def run_vdda_vddd_vs_trim(data, analog_readback_config, ps, yr, meter):
+def run_vdda_vddd_vs_trim(data, analog_readback_config, ps, yr, meter, layer):
     """
     This function measures how VDDA and VDDD changes with Trim.
 
     Args:
         data (list): data[chip_id][vmux/imux_type or bias/dem].
         analog_readback_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
@@ -269,15 +271,15 @@
     log.info(
         f"[run_AnalogReadBack] TimeStart: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
     if yr.running_emulator():
         ps.on(
             analog_readback_config["v_max"],
-            analog_readback_config["i_config"],
+            analog_readback_config["i_config"][layer],
         )  # Only for emulator do the emulation of power on/off.
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # Reset other chips
     reset = analog_readback_config["share_vmux"]
 
     # Trim to Vmux mapping
@@ -302,18 +304,28 @@
                     reset_other_chips=reset,
                 )
                 mea, status = meter.measure_dcv(
                     channel=analog_readback_config["v_mux_channels"][chip]
                 )
                 # Reset i_mea[chip]
                 i_mea[chip] = {}
-                # Record vmux, bias, and dem.
+
+                # Record vmux and trim.
                 i_mea[chip][f"Vmux{v_mux}"] = [mea]
                 i_mea[chip][trim_maps[v_mux]] = [trim]
 
+                # Read ROSC vs trim
+                if v_mux == 38:
+                    chip_name = data[chip]._meta_data["Name"]
+                    mea, status = yr.read_ringosc(name=chip_name, chip_position=chip)
+                    rosc_mea = [float(num) for num in mea.split()]
+                    for i in range(len(rosc_mea)):
+                        i_mea[chip][f"ROSC{i}"] = [rosc_mea[i]]
+
+                # Update output dataframe
                 data[chip].add_data(i_mea[chip])
 
         # Mwasure ground 16 times.
         max_n_measure = len(data[chip]["Vmux34"])
         n_measure = 0
         while n_measure < max_n_measure:
             i_mea[chip] = {}
@@ -333,19 +345,20 @@
 
     log.info("[run_AnalogReadBack] VDDA/VDDD measurement done!")
     log.info(
         f"[run_AnalogReadBack] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
 
-def add_identifier_metadata(data, yr, module_serial):
+def add_identifier_metadata(data, yr, module_serial, institution):
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
+        data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
 
 
 def add_time_end_identifier(yr, data):
     for chip in range(yr._number_of_chips):
@@ -371,29 +384,36 @@
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
         raise RuntimeError(
             "must supply path to connectivity file [-m --module-connectivity]"
         )
 
-    analog_readback_config = config["tasks"]["ANALOG_READBACK"]
+    analog_readback_config = config["tasks"]["GENERAL"]
+    analog_readback_config.update(config["tasks"]["ANALOG_READBACK"])
+
     ps = power_supply(config["power_supply"], verbose=args.verbose)
     yr = yarr(config["yarr"], verbose=args.verbose)
-
     meter = multimeter(config["multimeter"], verbose=args.verbose)
     nt = ntc(config["ntc"], verbose=args.verbose)
-    ps.set(v=analog_readback_config["v_max"], i=analog_readback_config["i_config"])
-
-    yr.configure()
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = os.path.basename(__file__).split(".py")[0]
+    institution = get_env("INSTITUTION")
+    if institution is None:
+        institution = ""
+
+    ps.set(
+        v=analog_readback_config["v_max"], i=analog_readback_config["i_config"][layer]
+    )
+    yr.configure()
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
@@ -448,49 +468,50 @@
         load_json(input_file)
         if input_file
         else qcDataFrame(
             columns=["Vmux34"]
             + ["Vmux38"]
             + ["Vmux30"]
             + ["SldoTrimA"]
-            + ["SldoTrimD"],
-            units=["V"] + ["V"] + ["V"] + ["-"] + ["-"],
+            + ["SldoTrimD"]
+            + [f"ROSC{i}" for i in range(42)],
+            units=["V"] + ["V"] + ["V"] + ["-"] + ["-"] + ["MHz" for i in range(42)],
         )
         for input_file in input_files
     ]
 
     # Measure internal vmux
-    add_identifier_metadata(data, yr, module_serial)
+    add_identifier_metadata(data, yr, module_serial, institution)
     try:
-        run_vmeas(data, analog_readback_config, ps, yr, meter)
+        run_vmeas(data, analog_readback_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring all vmux values.")
         log.exception(err)
         sys.exit(1)
     add_time_end_identifier(yr, data)
 
     # Measure temperature
-    add_identifier_metadata(data_tempmeas, yr, module_serial)
+    add_identifier_metadata(data_tempmeas, yr, module_serial, institution)
     try:
-        run_tmeas(data_tempmeas, analog_readback_config, ps, yr, meter, nt)
+        run_tmeas(data_tempmeas, analog_readback_config, ps, yr, meter, nt, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring temperature.")
         log.exception(err)
         sys.exit(1)
     add_time_end_identifier(yr, data_tempmeas)
 
     # Measure vdda/vddd vs trim
-    add_identifier_metadata(data_vdda_vddd_vs_trim, yr, module_serial)
+    add_identifier_metadata(data_vdda_vddd_vs_trim, yr, module_serial, institution)
     try:
         run_vdda_vddd_vs_trim(
-            data_vdda_vddd_vs_trim, analog_readback_config, ps, yr, meter
+            data_vdda_vddd_vs_trim, analog_readback_config, ps, yr, meter, layer
         )
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.info("Error in measuring VDDA/VDDD vs trim.")
         log.exception(err)
         sys.exit(1)
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import pkg_resources
 from module_qc_data_tools import (
+    get_env,
+    get_layer_from_sn,
     get_sn_from_connectivity,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
@@ -61,30 +63,30 @@
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
 
-def run(data, inj_cap_config, ps, yr, meter):
+def run(data, inj_cap_config, ps, yr, meter, layer):
     """The function which does the injection capacitance measurement.
 
     Args:
         data (list): data[chip_id].
         inj_cap_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
     if yr.running_emulator():
         ps.on(
-            inj_cap_config["v_max"], inj_cap_config["i_config"]
+            inj_cap_config["v_max"], inj_cap_config["i_config"][layer]
         )  # Only for emulator do the emulation of power on/off
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # This sends global pulse
     status = yr.configure()
     assert status >= 0
 
@@ -150,26 +152,32 @@
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
         raise RuntimeError(
             "must supply path to connectivity file [-m --module-connectivity]"
         )
 
-    inj_cap_config = config["tasks"]["INJECTION_CAPACITANCE"]
+    inj_cap_config = config["tasks"]["GENERAL"]
+    inj_cap_config.update(config["tasks"]["INJECTION_CAPACITANCE"])
+
     ps = power_supply(config["power_supply"], verbose=args.verbose)
     yr = yarr(config["yarr"], verbose=args.verbose)
-
     meter = multimeter(config["multimeter"], verbose=args.verbose)
-    ps.set(v=inj_cap_config["v_max"], i=inj_cap_config["i_config"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = os.path.basename(__file__).split(".py")[0]
+    institution = get_env("INSTITUTION")
+    if institution is None:
+        institution = ""
+
+    ps.set(v=inj_cap_config["v_max"], i=inj_cap_config["i_config"][layer])
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
@@ -195,23 +203,24 @@
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].add_property(
             test_type + "_MEASUREMENT_VERSION",
             pkg_resources.get_distribution("module-qc-tools").version,
         )
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
+        data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
 
     logging.basicConfig(level=logging.DEBUG)
     logger = logging.getLogger(__name__)
 
     try:
-        run(data, inj_cap_config, ps, yr, meter)
+        run(data, inj_cap_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         logger.exception(err)
         sys.exit(1)
 
     log.info(
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/SLDO.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
 from module_qc_data_tools import (
+    get_env,
+    get_layer_from_sn,
     get_sn_from_connectivity,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
@@ -64,26 +66,26 @@
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 parser.add_argument("--verbose", action="store_true", help="verbose mode")
 args = parser.parse_args()
 
 
-def run(data, SLDOVI_config, ps, yr, meter, nt):
+def run(data, SLDOVI_config, ps, yr, meter, nt, layer):
     # turn on power supply and configure all chips
-    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"])
+    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
     status = yr.configure()
 
     currents = sorted(
         np.concatenate(
             [
                 np.linspace(
-                    SLDOVI_config["i_min"],
-                    SLDOVI_config["i_max"],
-                    SLDOVI_config["n_points"],
+                    SLDOVI_config["i_min"][layer],
+                    SLDOVI_config["i_max"][layer],
+                    SLDOVI_config["n_points"][layer],
                 ),
                 np.array(SLDOVI_config["extra_i"]),
             ]
         ),
         reverse=True,
     )
     for i in currents:
@@ -125,15 +127,15 @@
             log.info(
                 "--------------------------------------------------------------------------"
             )
             log.info(f"Chip-{chip+1}")
             log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
 
     # Return to initial state
-    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"])
+    ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
 
 
 def main():
 
     log.info("[run_SLDOVI] Start VI scan!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_SLDOVI] TimeStart: {timestart}")
@@ -147,26 +149,31 @@
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
         raise RuntimeError(
             "must supply path to connectivity file [-m --module-connectivity]"
         )
 
-    SLDOVI_config = config["tasks"]["SLDO"]
+    SLDOVI_config = config["tasks"]["GENERAL"]
+    SLDOVI_config.update(config["tasks"]["SLDO"])
     ps = power_supply(config["power_supply"], verbose=args.verbose)
     yr = yarr(config["yarr"], verbose=args.verbose)
 
     meter = multimeter(config["multimeter"], verbose=args.verbose)
     nt = ntc(config["ntc"], verbose=args.verbose)
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = os.path.basename(__file__).split(".py")[0]
+    institution = get_env("INSTITUTION")
+    if institution is None:
+        institution = ""
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
@@ -191,24 +198,25 @@
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         data[chip].set_x("Current", True)
         data[chip]._meta_data = get_identifiers(yr.get_config(chip))
+        data[chip].add_meta_data("Institution", institution)
         data[chip].add_meta_data("ModuleSN", module_serial)
         data[chip].add_meta_data("TimeStart", round(datetime.timestamp(datetime.now())))
         data[chip]._meta_data.update(get_meta_data(yr.get_config(chip)))
         data[chip].add_property(
             test_type + "_MEASUREMENT_VERSION",
             pkg_resources.get_distribution("module-qc-tools").version,
         )
 
     try:
-        run(data, SLDOVI_config, ps, yr, meter, nt)
+        run(data, SLDOVI_config, ps, yr, meter, nt, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.exception(err)
         sys.exit(1)
 
     for chip in range(yr._number_of_chips):
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
 from module_qc_data_tools import (
+    get_env,
+    get_layer_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_tools import data
@@ -59,30 +61,30 @@
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
 
-def run(data, vcal_calib_config, ps, yr, meter):
+def run(data, vcal_calib_config, ps, yr, meter, layer):
     """The function which does the VCal calibration for VCal_Med and VCal_Hi in both large and small range.
 
     Args:
         data (list): data[chip_id][vcal_type]. 4 vcal_type in total.
         vcal_calib_config (dict): An subdict dumped from json including the task information.
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
     if yr.running_emulator():
         ps.on(
-            vcal_calib_config["v_max"], vcal_calib_config["i_config"]
+            vcal_calib_config["v_max"], vcal_calib_config["i_config"][layer]
         )  # Only for emulator do the emulation of power on/off
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     status = (
         yr.configure()
     )  # Should always be 0. Essentially it calls send_command() in the hardware_control_base where protection is added.
     assert status >= 0
@@ -186,30 +188,36 @@
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
         raise RuntimeError(
             "must supply path to connectivity file [-m --module-connectivity]"
         )
 
-    vcal_calib_config = config["tasks"]["VCAL_CALIBRATION"]
+    vcal_calib_config = config["tasks"]["GENERAL"]
+    vcal_calib_config.update(config["tasks"]["VCAL_CALIBRATION"])
+
     ps = power_supply(config["power_supply"], verbose=args.verbose)
     yr = yarr(config["yarr"], verbose=args.verbose)
-
     meter = multimeter(config["multimeter"], verbose=args.verbose)
-    ps.set(v=vcal_calib_config["v_max"], i=vcal_calib_config["i_config"])
-
-    MonitorV = vcal_calib_config["MonitorV"]
-    InjVcalRange = vcal_calib_config["InjVcalRange"]
-    vmux_value_GNDA = vcal_calib_config["MonitorV_GND"]
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = os.path.basename(__file__).split(".py")[0]
+    institution = get_env("INSTITUTION")
+    if institution is None:
+        institution = ""
+
+    ps.set(v=vcal_calib_config["v_max"], i=vcal_calib_config["i_config"][layer])
+
+    MonitorV = vcal_calib_config["MonitorV"]
+    InjVcalRange = vcal_calib_config["InjVcalRange"]
+    vmux_value_GNDA = vcal_calib_config["MonitorV_GND"]
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
@@ -232,14 +240,15 @@
                 data.add_property(
                     test_type + "_MEASUREMENT_VERSION",
                     pkg_resources.get_distribution("module-qc-tools").version,
                 )
 
                 data.set_x(x_label, True)
                 data._meta_data = get_identifiers(yr.get_config(chip))
+                data.add_meta_data("Institution", institution)
                 data.add_meta_data("ModuleSN", module_serial)
                 data._meta_data.update(get_meta_data(yr.get_config(chip)))
 
                 data._meta_data["ChipConfigs"]["RD53B"]["GlobalConfig"][
                     "MonitorEnable"
                 ] = 1
                 data._meta_data["ChipConfigs"]["RD53B"]["GlobalConfig"][
@@ -249,15 +258,15 @@
                     "InjVcalRange"
                 ] = vcalrange
 
                 qcdata_list.append(data)
         chip_data.append(qcdata_list)
 
     try:
-        run(chip_data, vcal_calib_config, ps, yr, meter)
+        run(chip_data, vcal_calib_config, ps, yr, meter, layer)
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
     except Exception as err:
         log.exception(err)
         sys.exit(1)
 
     log.info(
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,14 +195,16 @@
         module_state[f"Chip{chip+1}"]["ADCcalSlope"] = ADCcalPar[1] * 0.001
 
         # Update Vmux
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     update_module_state(module_state)
 
+    return 1
+
 
 def write_register():
     """
     This function emulates the effect of running YARR write-register
     Currently only emulates register MonitorI, MonitorV. One needs to add a new if statement for a new register name.
     """
     parser = argparse.ArgumentParser()
@@ -419,14 +421,49 @@
         else:
             v = module_state[f"Chip{chip+1}"]["Vmux"]
             u = "V"
         sys.stdout.write(f"{v} {u}")
     sys.exit(0)
 
 
+def read_ringosc():
+    """
+    This function emulates the effect of ROSC reading
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument("name", type=str, help="Name")
+    parser.add_argument(
+        "-r",
+        "--controller",
+        default=data / "emulator/configs/controller/specCfg-rd53b-16x1.json",
+        help="Controller",
+    )
+    parser.add_argument(
+        "-c",
+        "--connectivity",
+        default=data / "emulator" / _MODULE_CONNECTIVITY_FILE,
+        help="Connectivity",
+    )
+    parser.add_argument("-i", "--chip_position", type=int, help="chip position")
+    args = parser.parse_args()
+
+    with open(args.connectivity) as path:
+        spec_connectivity = json.load(path)
+
+    nChips = len(spec_connectivity["chips"])
+
+    for chip in range(nChips):
+        if args.chip_position is not None and chip is not args.chip_position:
+            continue
+
+        rosc_freq = "500 " * 42
+        sys.stdout.write(rosc_freq)
+    sys.exit(0)
+
+
 def measureT():
     """
     This function emulates the effect of NTC (measure module temperature)
     """
     module_state = get_module_state()
 
     T = module_state["temperature"]
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/main.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/upload_localdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import argparse
 import json
 import logging
+import sys
+import time
 from pathlib import Path
 
 import requests
 
 logging.basicConfig(level=logging.DEBUG)
 log = logging.getLogger(__name__)
 
@@ -32,25 +34,31 @@
 parser.add_argument(
     "-n",
     "--dry-run",
     default=False,
     action="store_true",
     help="Dry-run, do not submit to localDB.",
 )
+parser.add_argument(
+    "--out",
+    default="tmp.json",
+    help="Analysis output result json file path to save in the local host",
+)
 args = parser.parse_args()
 
 
 def main():
     """
     Walk through the specified directory (recursively) and attempt to submit all json files to LocalDB as the QC measurement
 
     Args:
         path (str or pathlib.Path): root directory to walk through
         host (str): localDB server host
         port (int): localDB server port
+        out  (str): analysis output result json file path to save in the local host
 
     Returns:
         None: The files are uploaded to localDB.
     """
 
     log.info("Searching candidate RAW json files...")
     flist = list(Path(args.path).rglob("*.json"))
@@ -60,29 +68,63 @@
         log.info(f"  - {path}")
         with path.open(encoding="utf-8") as fpointer:
             pack.extend(json.load(fpointer))
 
     log.info(f"Extracted {len(pack)} tests from {len(flist)} input files.")
     log.info("==> Submitting RAW results pack...")
 
+    protocol = "http" if args.port != "443" else "https"
+
     if not args.dry_run:
-        response = requests.post(
-            f"http://{args.host}:{args.port}/localdb/qc_uploader_post", json=pack
-        )
-        response.raise_for_status()
 
-        data = response.json()
+        try:
+            response = requests.post(
+                f"{protocol}://{args.host}:{args.port}/localdb/qc_uploader_post",
+                json=pack,
+            )
+            response.raise_for_status()
+
+            data = response.json()
+
+            log.info(data)
+
+        except Exception as e:
+            log.error("failure in uploading!")
+            log.error(e)
+            sys.exit(1)
+
         log.info(
             f"\nDone! LocalDB has accepted the following {len(data)} TestRun results"
         )
         for testRun in data:
             if testRun is None:
                 log.info("A test run is already uploaded and will be skipped.")
                 continue
 
             log.info(
                 f'SerialNumber: {testRun["serialNumber"]}, Stage: {testRun["stage"]}, TestType: {testRun["testType"]}, QC-passed: {testRun["passed"]}'
             )
 
+        try:
+
+            with open(args.out, "w") as f:
+                json.dump(data, f, indent=4)
+                log.info(f"Saved the output TestRun to {args.out}")
+
+        except Exception:
+
+            log.warning(f"Failed to saved the output TestRun to {args.out}")
+            altFilePath = f"/var/tmp/module-qc-tools-record-{int(time.time())}.json"
+
+            try:
+
+                with open(altFilePath, "w") as f:
+                    json.dump(data, f, indent=4)
+                log.info(f"Saved the output TestRun to {altFilePath}")
+
+            except Exception:
+                log.warning(f"Failed to saved the output TestRun to {altFilePath}")
+                pass
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L0.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6867759881730471%*

 * *Differences: {"'multimeter'": "{'run_dir': '../labRemote', 'dcv_cmd': ['./build/bin/meter -e "*

 * *                 "./src/configs/input-hw.json -n myVmuxMeter -c 0 meas-voltage'], 'n_try': 0, "*

 * *                 "'success_code': 0}",*

 * * "'ntc'": "{'run_dir': '../labRemote', 'cmd': './build/bin/TfromNTC -e ./src/configs/input-hw.json "*

 * *          "-n myNtcMeter -c 0 meas-from-r', 'n_try': 0, 'success_code': 0}",*

 * * "'power_supply'": "{'run_dir': '../labRemote', 'on_cmd': './build/bin/powersupply -e "*

 * *                   "./src/con […]*

```diff
@@ -1,47 +1,44 @@
 {
     "multimeter": {
         "dcv_cmd": [
-            "emulator-measureV"
+            "./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 0 meas-voltage"
         ],
-        "run_dir": "emulator"
+        "n_try": 0,
+        "run_dir": "../labRemote",
+        "success_code": 0
     },
     "ntc": {
-        "cmd": "emulator-measureT",
-        "run_dir": "emulator"
+        "cmd": "./build/bin/TfromNTC -e ./src/configs/input-hw.json -n myNtcMeter -c 0 meas-from-r",
+        "n_try": 0,
+        "run_dir": "../labRemote",
+        "success_code": 0
     },
     "power_supply": {
-        "getI_cmd": "emulator-control-ps -a getI",
-        "getV_cmd": "emulator-control-ps -a getI",
-        "off_cmd": "emulator-control-ps -a off",
-        "on_cmd": "emulator-control-ps -i {i} -v {v} -a on",
-        "run_dir": "emulator",
-        "set_cmd": "emulator-control-ps -i {i} -v {v} -a on"
+        "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
+        "getV_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-voltage",
+        "n_try": 0,
+        "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
+        "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
+        "run_dir": "../labRemote",
+        "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
+        "success_code": 0
     },
     "tasks": {
         "ADC_CALIBRATION": {
             "InjVcalRange": 1,
             "MonitorV": [
                 8,
                 30
             ],
             "Range": {
                 "start": 500,
                 "step": 100,
                 "stop": 3500
-            },
-            "i_config": 5.55,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
                 2,
                 3,
@@ -138,15 +135,14 @@
                 10,
                 11,
                 12,
                 13,
                 14,
                 15
             ],
-            "i_config": 5.55,
             "i_mux": [
                 0,
                 1,
                 2,
                 3,
                 4,
                 5,
@@ -175,16 +171,14 @@
                 31,
                 63
             ],
             "i_mux_ntc": [
                 9,
                 63
             ],
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -204,81 +198,84 @@
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ],
             "v_mux_ntc": [
                 2,
                 30
             ],
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
+        "GENERAL": {
+            "i_config": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
+            "share_vmux": true,
+            "v_max": 3.0,
+            "v_mux_channels": [
+                0,
+                0,
+                0,
+                0
+            ]
+        },
         "INJECTION_CAPACITANCE": {
-            "i_config": 5.55,
             "i_mux": [
                 10,
                 11,
                 63
             ],
             "n_meas": 5,
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 4,
                 30
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "SLDO": {
             "extra_i": [],
-            "i_config": 5.55,
-            "i_max": 9.75,
-            "i_min": 5.55,
+            "i_max": {
+                "L0": 9.75,
+                "L1": 10.6,
+                "L2": 9.48
+            },
+            "i_min": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
             "i_mux": [
                 0,
                 28,
                 29,
                 30,
                 31,
                 63
             ],
-            "n_points": 22,
-            "share_vmux": true,
-            "v_max": 3.0,
+            "n_points": {
+                "L0": 22,
+                "L1": 21,
+                "L2": 19
+            },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
                 38,
                 36,
                 32
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
@@ -292,28 +289,19 @@
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
                 "step": 100,
                 "stop": 4000
-            },
-            "i_config": 5.55,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         }
     },
     "yarr": {
-        "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
-        "controller": "configs/controller/emuCfg_rd53a.json",
-        "read_adc_exe": "emulator-read-adc",
-        "run_dir": "emulator",
-        "scanConsole_exe": "emulator-scanConsole",
-        "write_register_exe": "emulator-write-register"
+        "controller": "configs/controller/specCfg-rd53b-16x1.json",
+        "read_adc_exe": "./bin/read-adc",
+        "read_ringosc_exe": "./bin/rd53bReadRingosc",
+        "run_dir": "../Yarr",
+        "scanConsole_exe": "./bin/scanConsole",
+        "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L1.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9492759881730471%*

 * *Differences: {"'tasks'": "{'ADC_CALIBRATION': {delete: ['v_max', 'i_config', 'share_vmux', 'v_mux_channels']}, "*

 * *            "'SLDO': {'i_min': {replace: OrderedDict([('L0', 5.55), ('L1', 6.6), ('L2', 5.88)])}, "*

 * *            "'i_max': {replace: OrderedDict([('L0', 9.75), ('L1', 10.6), ('L2', 9.48)])}, "*

 * *            "'n_points': {replace: OrderedDict([('L0', 22), ('L1', 21), ('L2', 19)])}, delete: "*

 * *            "['v_max', 'i_config', 'share_vmux', 'v_mux_channels']}, 'VCAL_CALIBRATION': {delete: "*

 * *            "['v_max',  […]*

```diff
@@ -24,24 +24,15 @@
                 8,
                 30
             ],
             "Range": {
                 "start": 500,
                 "step": 100,
                 "stop": 3500
-            },
-            "i_config": 6.6,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
                 2,
                 3,
@@ -138,15 +129,14 @@
                 10,
                 11,
                 12,
                 13,
                 14,
                 15
             ],
-            "i_config": 6.6,
             "i_mux": [
                 0,
                 1,
                 2,
                 3,
                 4,
                 5,
@@ -175,16 +165,14 @@
                 31,
                 63
             ],
             "i_mux_ntc": [
                 9,
                 63
             ],
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -204,81 +192,84 @@
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ],
             "v_mux_ntc": [
                 2,
                 30
             ],
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
+        "GENERAL": {
+            "i_config": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
+            "share_vmux": true,
+            "v_max": 3.0,
+            "v_mux_channels": [
+                0,
+                0,
+                0,
+                0
+            ]
+        },
         "INJECTION_CAPACITANCE": {
-            "i_config": 6.6,
             "i_mux": [
                 10,
                 11,
                 63
             ],
             "n_meas": 5,
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 4,
                 30
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "SLDO": {
             "extra_i": [],
-            "i_config": 6.6,
-            "i_max": 10.6,
-            "i_min": 6.6,
+            "i_max": {
+                "L0": 9.75,
+                "L1": 10.6,
+                "L2": 9.48
+            },
+            "i_min": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
             "i_mux": [
                 0,
                 28,
                 29,
                 30,
                 31,
                 63
             ],
-            "n_points": 21,
-            "share_vmux": true,
-            "v_max": 3.0,
+            "n_points": {
+                "L0": 22,
+                "L1": 21,
+                "L2": 19
+            },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
                 38,
                 36,
                 32
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
@@ -292,28 +283,20 @@
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
                 "step": 100,
                 "stop": 4000
-            },
-            "i_config": 6.6,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         }
     },
     "yarr": {
         "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
         "controller": "configs/controller/emuCfg_rd53a.json",
         "read_adc_exe": "emulator-read-adc",
+        "read_ringosc_exe": "emulator-read-ringosc",
         "run_dir": "emulator",
         "scanConsole_exe": "emulator-scanConsole",
         "write_register_exe": "emulator-write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/configs/emulator_merged_vmux_L2.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6867759881730471%*

 * *Differences: {"'multimeter'": "{'run_dir': '../labRemote', 'dcv_cmd': ['./build/bin/meter -e "*

 * *                 "./src/configs/input-hw.json -n myVmuxMeter -c 0 meas-voltage', "*

 * *                 "'./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 1 "*

 * *                 "meas-voltage', './build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter "*

 * *                 "-c 2 meas-voltage', './build/bin/meter -e ./src/configs/input-hw.json -n "*

 * *                 "myVmuxMeter -c 3 meas-voltage'], 'n_try': 0, ' […]*

```diff
@@ -1,47 +1,47 @@
 {
     "multimeter": {
         "dcv_cmd": [
-            "emulator-measureV"
+            "./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 0 meas-voltage",
+            "./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 1 meas-voltage",
+            "./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 2 meas-voltage",
+            "./build/bin/meter -e ./src/configs/input-hw.json -n myVmuxMeter -c 3 meas-voltage"
         ],
-        "run_dir": "emulator"
+        "n_try": 0,
+        "run_dir": "../labRemote",
+        "success_code": 0
     },
     "ntc": {
-        "cmd": "emulator-measureT",
-        "run_dir": "emulator"
+        "cmd": "./build/bin/TfromNTC -e ./src/configs/input-hw.json -n myNtcMeter -c 0 meas-from-r",
+        "n_try": 0,
+        "run_dir": "../labRemote",
+        "success_code": 0
     },
     "power_supply": {
-        "getI_cmd": "emulator-control-ps -a getI",
-        "getV_cmd": "emulator-control-ps -a getI",
-        "off_cmd": "emulator-control-ps -a off",
-        "on_cmd": "emulator-control-ps -i {i} -v {v} -a on",
-        "run_dir": "emulator",
-        "set_cmd": "emulator-control-ps -i {i} -v {v} -a on"
+        "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
+        "getV_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-voltage",
+        "n_try": 0,
+        "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
+        "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
+        "run_dir": "../labRemote",
+        "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
+        "success_code": 0
     },
     "tasks": {
         "ADC_CALIBRATION": {
             "InjVcalRange": 1,
             "MonitorV": [
                 8,
                 30
             ],
             "Range": {
                 "start": 500,
                 "step": 100,
                 "stop": 3500
-            },
-            "i_config": 5.88,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
                 2,
                 3,
@@ -138,15 +138,14 @@
                 10,
                 11,
                 12,
                 13,
                 14,
                 15
             ],
-            "i_config": 5.88,
             "i_mux": [
                 0,
                 1,
                 2,
                 3,
                 4,
                 5,
@@ -175,16 +174,14 @@
                 31,
                 63
             ],
             "i_mux_ntc": [
                 9,
                 63
             ],
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -204,81 +201,84 @@
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ],
             "v_mux_ntc": [
                 2,
                 30
             ],
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
+        "GENERAL": {
+            "i_config": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
+            "share_vmux": false,
+            "v_max": 3.0,
+            "v_mux_channels": [
+                0,
+                1,
+                2,
+                3
+            ]
+        },
         "INJECTION_CAPACITANCE": {
-            "i_config": 5.88,
             "i_mux": [
                 10,
                 11,
                 63
             ],
             "n_meas": 5,
-            "share_vmux": true,
-            "v_max": 3.0,
             "v_mux": [
                 4,
                 30
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "SLDO": {
             "extra_i": [],
-            "i_config": 5.88,
-            "i_max": 9.48,
-            "i_min": 5.88,
+            "i_max": {
+                "L0": 9.75,
+                "L1": 10.6,
+                "L2": 9.48
+            },
+            "i_min": {
+                "L0": 5.55,
+                "L1": 6.6,
+                "L2": 5.88
+            },
             "i_mux": [
                 0,
                 28,
                 29,
                 30,
                 31,
                 63
             ],
-            "n_points": 19,
-            "share_vmux": true,
-            "v_max": 3.0,
+            "n_points": {
+                "L0": 22,
+                "L1": 21,
+                "L2": 19
+            },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
                 38,
                 36,
                 32
-            ],
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
             ]
         },
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
@@ -292,28 +292,19 @@
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
                 "step": 100,
                 "stop": 4000
-            },
-            "i_config": 5.88,
-            "share_vmux": true,
-            "v_max": 3.0,
-            "v_mux_channels": [
-                0,
-                0,
-                0,
-                0
-            ]
+            }
         }
     },
     "yarr": {
-        "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
-        "controller": "configs/controller/emuCfg_rd53a.json",
-        "read_adc_exe": "emulator-read-adc",
-        "run_dir": "emulator",
-        "scanConsole_exe": "emulator-scanConsole",
-        "write_register_exe": "emulator-write-register"
+        "controller": "configs/controller/specCfg-rd53b-16x1.json",
+        "read_adc_exe": "./bin/read-adc",
+        "read_ringosc_exe": "./bin/rd53bReadRingosc",
+        "run_dir": "../Yarr",
+        "scanConsole_exe": "./bin/scanConsole",
+        "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999264649549%*

 * *Differences: {"'items'": "{'items': {'properties': {'results': {'properties': {'Measurements': {'oneOf': {2: "*

 * *            "{'required': {insert: [(2, 'Vmux30'), (5, 'ROSC0'), (6, 'ROSC1'), (7, 'ROSC2'), (8, "*

 * *            "'ROSC3'), (9, 'ROSC4'), (10, 'ROSC5'), (11, 'ROSC6'), (12, 'ROSC7'), (13, 'ROSC8'), "*

 * *            "(14, 'ROSC9'), (15, 'ROSC10'), (16, 'ROSC11'), (17, 'ROSC12'), (18, 'ROSC13'), (19, "*

 * *            "'ROSC14'), (20, 'ROSC15'), (21, 'ROSC16'), (22, 'ROSC17'), (23, 'ROSC18'), (24, "*

 * *            "'ROSC19') […]*

```diff
@@ -136,16 +136,59 @@
                                             ],
                                             "type": "object"
                                         }
                                     },
                                     "required": [
                                         "Vmux34",
                                         "Vmux38",
+                                        "Vmux30",
                                         "SldoTrimA",
-                                        "SldoTrimD"
+                                        "SldoTrimD",
+                                        "ROSC0",
+                                        "ROSC1",
+                                        "ROSC2",
+                                        "ROSC3",
+                                        "ROSC4",
+                                        "ROSC5",
+                                        "ROSC6",
+                                        "ROSC7",
+                                        "ROSC8",
+                                        "ROSC9",
+                                        "ROSC10",
+                                        "ROSC11",
+                                        "ROSC12",
+                                        "ROSC13",
+                                        "ROSC14",
+                                        "ROSC15",
+                                        "ROSC16",
+                                        "ROSC17",
+                                        "ROSC18",
+                                        "ROSC19",
+                                        "ROSC20",
+                                        "ROSC21",
+                                        "ROSC22",
+                                        "ROSC23",
+                                        "ROSC24",
+                                        "ROSC25",
+                                        "ROSC26",
+                                        "ROSC27",
+                                        "ROSC28",
+                                        "ROSC29",
+                                        "ROSC30",
+                                        "ROSC31",
+                                        "ROSC32",
+                                        "ROSC33",
+                                        "ROSC34",
+                                        "ROSC35",
+                                        "ROSC36",
+                                        "ROSC37",
+                                        "ROSC38",
+                                        "ROSC39",
+                                        "ROSC40",
+                                        "ROSC41"
                                     ]
                                 }
                             ],
                             "type": "object"
                         }
                     },
                     "type": "object"
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,29 +26,34 @@
 
         if self.run_dir == "emulator":
             self.run_dir = os.getcwd()
         else:
             self.run_dir = Path(self.run_dir)
 
     def send_command(
-        self, cmd, purpose="send command", extra_error_messages=None, pause=0
+        self,
+        cmd,
+        purpose="send command",
+        extra_error_messages=None,
+        pause=0,
+        success_code=0,
     ):
         extra_error_messages = extra_error_messages or []
 
         os.chdir(self._wd)
         os.chdir(self.run_dir)
         result = subprocess.run(
             cmd,
             shell=True,
             stdout=None if log.getEffectiveLevel() < logging.INFO else subprocess.PIPE,
             stderr=None if log.getEffectiveLevel() < logging.INFO else subprocess.PIPE,
         )
         os.chdir(self._wd)
 
-        if result.returncode < 0:
+        if result.returncode != success_code:
             for extra_error_message in extra_error_messages:
                 log.info(f"[{self._name}] {extra_error_message}")
             raise RuntimeError(f"[{self._name}] fail to {purpose}!!")
         log.info(f"[{self._name}] {purpose}")
 
         time.sleep(pause)
 
@@ -58,14 +63,15 @@
         self,
         cmd,
         type=float,
         purpose="send command and read",
         unit="",
         extra_error_messages=None,
         max_nTry=0,
+        success_code=0,
     ):
 
         extra_error_messages = extra_error_messages or []
         os.chdir(self._wd)
         os.chdir(self.run_dir)
         result = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
         os.chdir(self._wd)
@@ -82,14 +88,14 @@
             log.info(f"Try again. Send command and read attempt {nTry} time(s).")
             os.chdir(self._wd)
             os.chdir(self.run_dir)
             result = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
             os.chdir(self._wd)
             log.info(result.stdout.decode())
 
-        if result.returncode != 0:
+        if result.returncode != success_code:
             raise RuntimeError(f"[{self._name}] fail to {purpose}!!")
         value = type(result.stdout.decode())
         for _extra_error_message in extra_error_messages:
             log.info(f"[{self._name}] {purpose}: {value}{unit}")
 
         return value, result.returncode
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/utils/misc.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/multimeter.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 log = logging.getLogger(__name__)
 
 
 class multimeter(hardware_control_base):
     def __init__(self, config, name="multimeter", *args, **kwargs):
         self.dcv_cmd = []
         self.n_try = 0
+        self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
         if any(["emulator" in dcv_cmd for dcv_cmd in self.dcv_cmd]):
             log.info(f"[{name}] running multimeter emulator!!")
 
     def measure_dcv(self, channel=0):
 
         return self.send_command_and_read(
             self.dcv_cmd[channel],
             purpose=f"read voltage channel {channel}",
             unit="V",
             max_nTry=self.n_try,
+            success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/ntc.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 log = logging.getLogger(__name__)
 
 
 class ntc(hardware_control_base):
     def __init__(self, config, name="ntc", *args, **kwargs):
         self.cmd = ""
         self.n_try = 0
+        self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.cmd:
             log.info(f"[{name}] running NTC emulator!!")
 
     def read(self):
 
         return self.send_command_and_read(
-            self.cmd, purpose="read temperature", unit="C", max_nTry=self.n_try
+            self.cmd,
+            purpose="read temperature",
+            unit="C",
+            max_nTry=self.n_try,
+            success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.1/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/power_supply.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,48 +13,65 @@
     def __init__(self, config, name="power_supply", *args, **kwargs):
         self.on_cmd = ""
         self.off_cmd = ""
         self.set_cmd = ""
         self.getV_cmd = ""
         self.getI_cmd = ""
         self.n_try = 0
+        self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.on_cmd:
             log.info(f"[{name}] running power supply emulator!!")
 
     def on(self, v=None, i=None):
 
         cmd = f'{self.on_cmd.replace("{v}", str(v)).replace("{i}", str(i))}'
 
-        return self.send_command(cmd, purpose=f"turn on power supply with {v}V, {i}A")
+        return self.send_command(
+            cmd,
+            purpose=f"turn on power supply with {v}V, {i}A",
+            success_code=self.success_code,
+        )
 
     def set(self, v=None, i=None):
 
         cmd = f'{self.set_cmd.replace("{v}", str(v)).replace("{i}", str(i))}'
 
         return self.send_command(
-            cmd, purpose=f"set power supply to {v}V, {i}A", pause=1
+            cmd,
+            purpose=f"set power supply to {v}V, {i}A",
+            pause=1,
+            success_code=self.success_code,
         )
 
     def off(self):
 
         return self.send_command(
             self.off_cmd,
             purpose="turn off power supply",
             extra_error_messages=[
                 f"Run directory: `{self.run_dir}`"
                 f"Off command: `{self.off_cmd}`"
                 "Please manually turn off power supply!!"
             ],
+            success_code=self.success_code,
         )
 
     def getV(self):
 
         return self.send_command_and_read(
-            self.getV_cmd, purpose="read voltage", unit="V", max_nTry=self.n_try
+            self.getV_cmd,
+            purpose="read voltage",
+            unit="V",
+            max_nTry=self.n_try,
+            success_code=self.success_code,
         )
 
     def getI(self):
 
         return self.send_command_and_read(
-            self.getI_cmd, purpose="read current", unit="A", max_nTry=self.n_try
+            self.getI_cmd,
+            purpose="read current",
+            unit="A",
+            max_nTry=self.n_try,
+            success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.1/.gitignore` & `module_qc_tools-1.3.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/LICENSE` & `module_qc_tools-1.3.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.1/README.md` & `module_qc_tools-1.3.2rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,50 @@
-# module-qc-tools v1.3.1
+Metadata-Version: 2.1
+Name: module_qc_tools
+Version: 1.3.2rc0
+Summary: Module qc tools
+Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
+Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
+Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
+Author-email: Jay Chan <jay.chan@cern.ch>
+Maintainer-email: Giordon Stark <gstark@cern.ch>
+License: Copyright (c) 2018 The Python Packaging Authority
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: importlib-resources; python_version < '3.9'
+Requires-Dist: jsonschema
+Requires-Dist: module-qc-data-tools>=1.0.5
+Requires-Dist: numpy
+Requires-Dist: pre-commit
+Requires-Dist: requests
+Requires-Dist: tabulate
+Description-Content-Type: text/markdown
+
+# module-qc-tools v1.3.2rc0
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -63,15 +105,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.1
+python -m pip install -U pip module-qc-tools==1.3.2rc0
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -82,27 +124,25 @@
 The first step in using this package is to set up the
 [Configuration and external commands](#configuration-and-external-commands)
 input json file. This json file is then passed as input to the scripts used to
 run the [Measurements](#measurements).
 
 ## Configuration and external commands
 
-All the configuration/settings are defined in a single json file. Examples are
-provided in `$(module-qc-tools --prefix)/configs/':
+All the configuration/settings are defined in a single json file. The layer
+information needed for the different power settings is extracted from the
+module's serial number. Examples are provided in `$(module-qc-tools
+--prefix)/configs/':
 
 ```
-example_merged_vmux_L0.json --> Layer 0
-example_merged_vmux_L1.json --> Layer 1
-example_merged_vmux_L2.json --> Layer 2
+example_merged_vmux.json
+example_separate_vmux.json
 ```
 
-Please choose the correct layer so that the measurements are performed properly.
-This is especially important for the SLDO test.
-
-<details> <summary> $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json </summary>
+<details> <summary> $(module-qc-tools --prefix)/configs/example_merged_vmux.json </summary>
 
 ```json
 {
         "yarr": {
                 "run_dir": "../Yarr",
                 "controller": "configs/controller/specCfg-rd53b-16x1.json",
                 "scanConsole_exe": "./bin/scanConsole",
@@ -112,34 +152,38 @@
         "power_supply": {
                 "run_dir": "../labRemote",
                 "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
                 "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
                 "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
                 "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
                 "getV_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-voltage",
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "multimeter": {
                 "run_dir": "../labRemote",
                 "dcv_cmd": [
                         "./build/bin/meter -e ./src/configs/input-hw-min_marija.json -n myVmuxMeter -c 0 meas-voltage"
                 ],
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "ntc": {
                 "run_dir": "../labremote_devel/scripts",
                 "cmd": "python measureT.py",
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "tasks": {
-                "SLDO": {...}
-		"VCAL_CALIBRATION": {...}
-		"ANALOG_READBACK": {...}
-		"ADC_CALIBRATION": {...}
-		"INJECTION_CAPACITANCE": {...}
+                "GENERAL": {...},
+                "ADC_CALIBRATION": {...},
+                "ANALOG_READBACK": {...},
+                "SLDO": {...},
+		            "VCAL_CALIBRATION": {...},
+		            "INJECTION_CAPACITANCE": {...}
         }
 }
 ```
 
 </details>
 
 The major blocks (e.g. `yarr`, `power_supply`, `multimeter`, `ntc`) correspond
@@ -153,20 +197,25 @@
 
 The `yarr` block specifies the path to the `YARR` repository as well as the
 corresponding YARR configuration files.
 
 - `run_dir`: path (relative or absolute) to the directory where `YARR` commands
   should be run
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
-- `scanConsole_exe`": path (relative to `run_dir` or absolute) to the
+- `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
-- `write_register_exe`": path (relative to `run_dir` or absolute) to the
+- `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
-- `read_adc_exe`": path (relative to `run_dir` or absolute) to the `read_adc`
+- `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
+- `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
+  `read_ringosc_exe` executable
+- `success_code`: exit status that indicates success. The default is 0 besides
+  `configure`, which has exit status 1 for success. The user do not need to set
+  the `success_code` as the default in QC software is synchronized with YARR.
 
 ### power_supply
 
 The `power_supply` block specifies the path and the commands for handling the
 power supply
 
 - `run_dir`: path (relative or absolute) to the directory where `power_supply`
@@ -184,14 +233,15 @@
   `5.2`.
 - `getV_cmd`: command to measure voltage of the power supply. This command shall
   return a std output which represents the value of the voltage (float in the
   unit of [V]). For example, when V = 1.8A, `getV_cmd` returns std output =
   `1.8`.
 - `n_try`: number of re-tries in case the script fails to read from the power
   supply
+- `success_code`: exit status that indicates success. The default is 0.
 
 ### multimeter
 
 The `multimeter` block specifies the path and the commands for handling the
 multimeter
 
 - `run_dir`: path (relative or absolute) to the directory where `multimeter`
@@ -199,25 +249,42 @@
 - `dcv_cmd`: list of commands to measure voltage from the multimeter. Each
   command corresponds to a single multimeter channel (only the used channels
   need to be listed). Each command returns a std output which represents the
   value of measured voltage (float in the unit of [V]). For example, when V =
   0.352V, `dcv_cmd` returns std output = `0.352`.
 - `n_try`: number of re-tries in case the script fails to read from the
   multimeter
+- `success_code`: exit status that indicates success. The default is 0.
 
 ### ntc
 
 The `ntc` block specifies the path and the commands for handling the NTC
 
 - `run_dir`: path (relative or absolute) to the directory where `ntc` commands
   should be run
 - `cmd`: command to measure temperature from the module NTC. The command returns
   a std output which represents the value of measured temperature (float in the
   unit of [C]). For example: when T = 36.2C, `cmd` returns std output = `36.2`.
 - `n_try`: number of re-tries in case the script fails to read from the ntc
+- `success_code`: exit status that indicates success. The default is 0.
+
+### tasks
+
+The `tasks` block starts with the `GENERAL` section that specifies the
+layer-dependent power settings:
+
+- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
+  the power supply should operate in constant current)
+- `i_config`: the current at which the module should be configured
+- `share_vmux`: whether to merge the Vmux channels or not
+- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
+  (correspond to each element in the dcv_cmd in the multimeter block)
+
+The main part of the `tasks` block is to specify all
+[measurements](#measurements) as listed below.
 
 ## Measurements
 
 An overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
@@ -226,28 +293,22 @@
 
 ### ADC calibration
 
 `measurement-ADC-CALIBRATION`
 
 This script will run the ADC calibration (`task = ADC_CALIBRATION`) as specified
 in the input configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `MonitorV`: list of Vmux channels to be measured
 - `InjVcalRange`: the range of the calibration injection circuit(1: a large
   range and 0: a small range i.e. half the large range but a finer step)
 - `Range`: the DACs scan range ["start", "stop", "step"]
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-ADC-CALIBRATION --help
@@ -268,59 +329,52 @@
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
-measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
+measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
-measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 ```
 
 </details>
 
 ### Analog readback
 
 `measurement-ANALOG-READBACK`
 
 This script will measure all internal voltages available through VMUX and IMUX,
-measure the chip temperature, and measure VDDA/VDDD vs Trim. channels. The scan
-settings are defined in the `task = ANALOG_READBACK` block of the input
+measure the chip temperature, and measure VDDA/VDDD/ROSC vs Trim. channels. The
+scan settings are defined in the `task = ANALOG_READBACK` block of the input
 configuration file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`). The NTC
-needs to be set in order to run this script, so that the temperature can be
-read.
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`). The NTC needs
+to be set in order to run this script, so that the temperature can be read.
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
 - `v_mux_ntc`: list of Vmux channels to be measured for ntc temperature
 - `i_mux_ntc`: list of Imux channels to be measured for ntc temperature
 - `v_mux_tempsens`: list of Vmux channels to be measured for 3 temperature
   sensors
 - `MonSensSldoDigSelBias`: Bias 0 and 1 for MOS sensor near digital SLDO
 - `MonSensSldoAnaSelBias`: Bias 0 and 1 for MOS sensor near analog SLDO
 - `MonSensAcbSelBias`: Bias 0 and 1 for MOS sensor near center
 - `MonSensSldoDigDem`: Dem 0-15 for MOS sensor near digital SLDO
 - `MonSensSldoAnaDem`: Dem 0-15 for MOS sensor near analog SLDO
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR]
@@ -343,54 +397,48 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-ANALOG-READBACK -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-ANALOG-READBACK -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
 
 ```
 
 </details>
 
 ### SLDOVI
 
 `measurement-SLDO`
 
 This script will run the VI scans (`task = SLDO`) as specified in the input
 configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `i_min`: the minimum current of the VI scan
 - `i_max`: the maximum current of the VI scan
 - `n_points`: how many points should be measured (equally spread between the max
   of the min currents)
 - `extra_i`: extra current points to be measured
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-SLDO --help
@@ -413,49 +461,43 @@
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
-measurement-SLDO -c $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
+measurement-SLDO -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
-measurement-SLDO -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs
+measurement-SLDO -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
 ```
 
 </details>
 
 ### VCal calibration
 
 `measurement-VCAL-CALIBRATION`
 
 This script will run the VCal calibration (`task = VCAL_CALIBRATION`) as
 specified in the input configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `InjVcalRange`: the range of the calibration injection circuit(1: a large
   range and 0: a small range i.e. half the large range but a finer step)
 - `MonitorV`: two DACs VMUX assignments Vcal_med(8) and Vcal_high(7)
 - `MonitorV_GND`: the GNDA VMUX assignment 30
 - `Large_Range`: the large DACs scan range ["start", "stop", "step"]
 - `Small_Range`: the small DACs scan range ["start", "stop", "step"]
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-VCAL-CALIBRATION --help
@@ -476,50 +518,44 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-VCAL-CALIBRATION -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-VCAL-CALIBRATION -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
 ### Injection capacitance
 
 `measurement-INJECTION-CAPACITANCE`
 
 This script will run the injection capacitance measurement
 (`task = INJECTION_CAPACITANCE`) as specified in the input configuration json
-file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `n_meas`: number of measurements to perform
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]]
@@ -543,26 +579,26 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
 ## Output data
```

### Comparing `module_qc_tools-1.3.1/pyproject.toml` & `module_qc_tools-1.3.2rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "tabulate",
     "pre-commit",
     "jsonschema",
-    "module-qc-data-tools >= 1.0.1",
+    "module-qc-data-tools >= 1.0.5",
     'importlib_resources; python_version < "3.9"',
     "requests",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -36,14 +36,15 @@
 "Source" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools"
 
 [project.scripts]
 module-qc-tools = "module_qc_tools.cli.main:main"
 emulator-scanConsole = "module_qc_tools.cli.hardware_emulator:scanConsole"
 emulator-write-register = "module_qc_tools.cli.hardware_emulator:write_register"
 emulator-read-adc = "module_qc_tools.cli.hardware_emulator:read_adc"
+emulator-read-ringosc = "module_qc_tools.cli.hardware_emulator:read_ringosc"
 emulator-control-ps = "module_qc_tools.cli.hardware_emulator:control_PS"
 emulator-measureV = "module_qc_tools.cli.hardware_emulator:measureV"
 emulator-measureT = "module_qc_tools.cli.hardware_emulator:measureT"
 measurement-ADC-CALIBRATION = "module_qc_tools.cli.ADC_CALIBRATION:main"
 measurement-ANALOG-READBACK = "module_qc_tools.cli.ANALOG_READBACK:main"
 measurement-SLDO = "module_qc_tools.cli.SLDO:main"
 measurement-VCAL-CALIBRATION = "module_qc_tools.cli.VCAL_CALIBRATION:main"
```

### Comparing `module_qc_tools-1.3.1/PKG-INFO` & `module_qc_tools-1.3.2rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,8 @@
-Metadata-Version: 2.1
-Name: module_qc_tools
-Version: 1.3.1
-Summary: Module qc tools
-Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
-Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
-Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
-Author-email: Jay Chan <jay.chan@cern.ch>
-Maintainer-email: Giordon Stark <gstark@cern.ch>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: jsonschema
-Requires-Dist: module-qc-data-tools>=1.0.1
-Requires-Dist: numpy
-Requires-Dist: pre-commit
-Requires-Dist: requests
-Requires-Dist: tabulate
-Description-Content-Type: text/markdown
-
-# module-qc-tools v1.3.1
+# module-qc-tools v1.3.2rc0
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -105,15 +63,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.1
+python -m pip install -U pip module-qc-tools==1.3.2rc0
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -124,27 +82,25 @@
 The first step in using this package is to set up the
 [Configuration and external commands](#configuration-and-external-commands)
 input json file. This json file is then passed as input to the scripts used to
 run the [Measurements](#measurements).
 
 ## Configuration and external commands
 
-All the configuration/settings are defined in a single json file. Examples are
-provided in `$(module-qc-tools --prefix)/configs/':
+All the configuration/settings are defined in a single json file. The layer
+information needed for the different power settings is extracted from the
+module's serial number. Examples are provided in `$(module-qc-tools
+--prefix)/configs/':
 
 ```
-example_merged_vmux_L0.json --> Layer 0
-example_merged_vmux_L1.json --> Layer 1
-example_merged_vmux_L2.json --> Layer 2
+example_merged_vmux.json
+example_separate_vmux.json
 ```
 
-Please choose the correct layer so that the measurements are performed properly.
-This is especially important for the SLDO test.
-
-<details> <summary> $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json </summary>
+<details> <summary> $(module-qc-tools --prefix)/configs/example_merged_vmux.json </summary>
 
 ```json
 {
         "yarr": {
                 "run_dir": "../Yarr",
                 "controller": "configs/controller/specCfg-rd53b-16x1.json",
                 "scanConsole_exe": "./bin/scanConsole",
@@ -154,34 +110,38 @@
         "power_supply": {
                 "run_dir": "../labRemote",
                 "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
                 "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
                 "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
                 "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
                 "getV_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-voltage",
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "multimeter": {
                 "run_dir": "../labRemote",
                 "dcv_cmd": [
                         "./build/bin/meter -e ./src/configs/input-hw-min_marija.json -n myVmuxMeter -c 0 meas-voltage"
                 ],
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "ntc": {
                 "run_dir": "../labremote_devel/scripts",
                 "cmd": "python measureT.py",
-                "n_try": 0
+                "n_try": 0,
+                "success_code": 0
         },
         "tasks": {
-                "SLDO": {...}
-		"VCAL_CALIBRATION": {...}
-		"ANALOG_READBACK": {...}
-		"ADC_CALIBRATION": {...}
-		"INJECTION_CAPACITANCE": {...}
+                "GENERAL": {...},
+                "ADC_CALIBRATION": {...},
+                "ANALOG_READBACK": {...},
+                "SLDO": {...},
+		            "VCAL_CALIBRATION": {...},
+		            "INJECTION_CAPACITANCE": {...}
         }
 }
 ```
 
 </details>
 
 The major blocks (e.g. `yarr`, `power_supply`, `multimeter`, `ntc`) correspond
@@ -195,20 +155,25 @@
 
 The `yarr` block specifies the path to the `YARR` repository as well as the
 corresponding YARR configuration files.
 
 - `run_dir`: path (relative or absolute) to the directory where `YARR` commands
   should be run
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
-- `scanConsole_exe`": path (relative to `run_dir` or absolute) to the
+- `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
-- `write_register_exe`": path (relative to `run_dir` or absolute) to the
+- `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
-- `read_adc_exe`": path (relative to `run_dir` or absolute) to the `read_adc`
+- `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
+- `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
+  `read_ringosc_exe` executable
+- `success_code`: exit status that indicates success. The default is 0 besides
+  `configure`, which has exit status 1 for success. The user do not need to set
+  the `success_code` as the default in QC software is synchronized with YARR.
 
 ### power_supply
 
 The `power_supply` block specifies the path and the commands for handling the
 power supply
 
 - `run_dir`: path (relative or absolute) to the directory where `power_supply`
@@ -226,14 +191,15 @@
   `5.2`.
 - `getV_cmd`: command to measure voltage of the power supply. This command shall
   return a std output which represents the value of the voltage (float in the
   unit of [V]). For example, when V = 1.8A, `getV_cmd` returns std output =
   `1.8`.
 - `n_try`: number of re-tries in case the script fails to read from the power
   supply
+- `success_code`: exit status that indicates success. The default is 0.
 
 ### multimeter
 
 The `multimeter` block specifies the path and the commands for handling the
 multimeter
 
 - `run_dir`: path (relative or absolute) to the directory where `multimeter`
@@ -241,25 +207,42 @@
 - `dcv_cmd`: list of commands to measure voltage from the multimeter. Each
   command corresponds to a single multimeter channel (only the used channels
   need to be listed). Each command returns a std output which represents the
   value of measured voltage (float in the unit of [V]). For example, when V =
   0.352V, `dcv_cmd` returns std output = `0.352`.
 - `n_try`: number of re-tries in case the script fails to read from the
   multimeter
+- `success_code`: exit status that indicates success. The default is 0.
 
 ### ntc
 
 The `ntc` block specifies the path and the commands for handling the NTC
 
 - `run_dir`: path (relative or absolute) to the directory where `ntc` commands
   should be run
 - `cmd`: command to measure temperature from the module NTC. The command returns
   a std output which represents the value of measured temperature (float in the
   unit of [C]). For example: when T = 36.2C, `cmd` returns std output = `36.2`.
 - `n_try`: number of re-tries in case the script fails to read from the ntc
+- `success_code`: exit status that indicates success. The default is 0.
+
+### tasks
+
+The `tasks` block starts with the `GENERAL` section that specifies the
+layer-dependent power settings:
+
+- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
+  the power supply should operate in constant current)
+- `i_config`: the current at which the module should be configured
+- `share_vmux`: whether to merge the Vmux channels or not
+- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
+  (correspond to each element in the dcv_cmd in the multimeter block)
+
+The main part of the `tasks` block is to specify all
+[measurements](#measurements) as listed below.
 
 ## Measurements
 
 An overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
@@ -268,28 +251,22 @@
 
 ### ADC calibration
 
 `measurement-ADC-CALIBRATION`
 
 This script will run the ADC calibration (`task = ADC_CALIBRATION`) as specified
 in the input configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `MonitorV`: list of Vmux channels to be measured
 - `InjVcalRange`: the range of the calibration injection circuit(1: a large
   range and 0: a small range i.e. half the large range but a finer step)
 - `Range`: the DACs scan range ["start", "stop", "step"]
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-ADC-CALIBRATION --help
@@ -310,59 +287,52 @@
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
-measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
+measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
-measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+measurement-ADC-CALIBRATION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 ```
 
 </details>
 
 ### Analog readback
 
 `measurement-ANALOG-READBACK`
 
 This script will measure all internal voltages available through VMUX and IMUX,
-measure the chip temperature, and measure VDDA/VDDD vs Trim. channels. The scan
-settings are defined in the `task = ANALOG_READBACK` block of the input
+measure the chip temperature, and measure VDDA/VDDD/ROSC vs Trim. channels. The
+scan settings are defined in the `task = ANALOG_READBACK` block of the input
 configuration file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`). The NTC
-needs to be set in order to run this script, so that the temperature can be
-read.
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`). The NTC needs
+to be set in order to run this script, so that the temperature can be read.
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
 - `v_mux_ntc`: list of Vmux channels to be measured for ntc temperature
 - `i_mux_ntc`: list of Imux channels to be measured for ntc temperature
 - `v_mux_tempsens`: list of Vmux channels to be measured for 3 temperature
   sensors
 - `MonSensSldoDigSelBias`: Bias 0 and 1 for MOS sensor near digital SLDO
 - `MonSensSldoAnaSelBias`: Bias 0 and 1 for MOS sensor near analog SLDO
 - `MonSensAcbSelBias`: Bias 0 and 1 for MOS sensor near center
 - `MonSensSldoDigDem`: Dem 0-15 for MOS sensor near digital SLDO
 - `MonSensSldoAnaDem`: Dem 0-15 for MOS sensor near analog SLDO
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR]
@@ -385,54 +355,48 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-ANALOG-READBACK -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-ANALOG-READBACK -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
 
 ```
 
 </details>
 
 ### SLDOVI
 
 `measurement-SLDO`
 
 This script will run the VI scans (`task = SLDO`) as specified in the input
 configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `i_min`: the minimum current of the VI scan
 - `i_max`: the maximum current of the VI scan
 - `n_points`: how many points should be measured (equally spread between the max
   of the min currents)
 - `extra_i`: extra current points to be measured
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-SLDO --help
@@ -455,49 +419,43 @@
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
-measurement-SLDO -c $(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
+measurement-SLDO -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
-measurement-SLDO -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs
+measurement-SLDO -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
 ```
 
 </details>
 
 ### VCal calibration
 
 `measurement-VCAL-CALIBRATION`
 
 This script will run the VCal calibration (`task = VCAL_CALIBRATION`) as
 specified in the input configuration json file (i.e.
-`$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `InjVcalRange`: the range of the calibration injection circuit(1: a large
   range and 0: a small range i.e. half the large range but a finer step)
 - `MonitorV`: two DACs VMUX assignments Vcal_med(8) and Vcal_high(7)
 - `MonitorV_GND`: the GNDA VMUX assignment 30
 - `Large_Range`: the large DACs scan range ["start", "stop", "step"]
 - `Small_Range`: the small DACs scan range ["start", "stop", "step"]
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-VCAL-CALIBRATION --help
@@ -518,50 +476,44 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-VCAL-CALIBRATION -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-VCAL-CALIBRATION -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
 ### Injection capacitance
 
 `measurement-INJECTION-CAPACITANCE`
 
 This script will run the injection capacitance measurement
 (`task = INJECTION_CAPACITANCE`) as specified in the input configuration json
-file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux_L2.json`).
+file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
 
 <details> <summary> Configuration settings </summary>
 
-- `v_max`: the voltage to be set to the power supply (i.e. the max voltage since
-  the power supply should operate in constant current)
-- `i_config`: the current at which the module should be configured
 - `n_meas`: number of measurements to perform
 - `v_mux`: list of Vmux channels to be measured
 - `i_mux`: list of Imux channels to be measured
-- `share_vmux`: whether to merge the Vmux channels or not
-- `v_mux_channels`: multimeter channel to measure the Vmux for each chip
-  (correspond to each element in the dcv_cmd in the multimeter block)
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]]
@@ -585,26 +537,26 @@
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
---prefix)/configs/example_merged_vmux_L2.json -m
+--prefix)/configs/example_merged_vmux.json -m
 ~/module_data/20UPGR91301046/20UPGR91301046_L2_warm.json
 
 ```
 
 </details>
 
 <details> <summary> Example command to run on the toy emulator </summary>
 
 ```
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
---prefix)/configs/emulator_merged_vmux_L2.json -o emulator/outputs/
+--prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
 ## Output data
```

