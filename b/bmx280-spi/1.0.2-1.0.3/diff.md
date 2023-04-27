# Comparing `tmp/bmx280_spi-1.0.2.tar.gz` & `tmp/bmx280_spi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmx280_spi-1.0.2.tar", last modified: Wed Mar 15 22:07:26 2023, max compression
+gzip compressed data, was "bmx280_spi-1.0.3.tar", last modified: Thu Apr 27 05:33:37 2023, max compression
```

## Comparing `bmx280_spi-1.0.2.tar` & `bmx280_spi-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-15 22:07:26.235523 bmx280_spi-1.0.2/
--rw-r--r--   0 pi        (1000) pi        (1000)     1069 2023-03-05 05:55:39.000000 bmx280_spi-1.0.2/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     2715 2023-03-15 22:07:26.235523 bmx280_spi-1.0.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1914 2023-03-15 22:05:22.000000 bmx280_spi-1.0.2/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-15 22:07:26.235523 bmx280_spi-1.0.2/bmx280_spi/
--rw-r--r--   0 pi        (1000) pi        (1000)    31099 2023-03-15 22:03:27.000000 bmx280_spi-1.0.2/bmx280_spi/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8081 2023-03-07 02:45:16.000000 bmx280_spi-1.0.2/bmx280_spi/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-15 22:07:26.235523 bmx280_spi-1.0.2/bmx280_spi.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2715 2023-03-15 22:07:26.000000 bmx280_spi-1.0.2/bmx280_spi.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-03-15 22:07:26.000000 bmx280_spi-1.0.2/bmx280_spi.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-03-15 22:07:26.000000 bmx280_spi-1.0.2/bmx280_spi.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       29 2023-03-15 22:07:26.000000 bmx280_spi-1.0.2/bmx280_spi.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-03-15 22:07:26.000000 bmx280_spi-1.0.2/bmx280_spi.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      927 2023-03-15 22:06:18.000000 bmx280_spi-1.0.2/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-03-15 22:07:26.235523 bmx280_spi-1.0.2/setup.cfg
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 05:33:37.919878 bmx280_spi-1.0.3/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1069 2023-03-05 05:55:39.000000 bmx280_spi-1.0.3/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     2715 2023-04-27 05:33:37.915878 bmx280_spi-1.0.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1914 2023-03-15 22:05:22.000000 bmx280_spi-1.0.3/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 05:33:37.907878 bmx280_spi-1.0.3/bmx280_spi/
+-rw-r--r--   0 pi        (1000) pi        (1000)    31359 2023-04-27 05:30:35.000000 bmx280_spi-1.0.3/bmx280_spi/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     8081 2023-03-07 02:45:16.000000 bmx280_spi-1.0.3/bmx280_spi/__main__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 05:33:37.915878 bmx280_spi-1.0.3/bmx280_spi.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2715 2023-04-27 05:33:37.000000 bmx280_spi-1.0.3/bmx280_spi.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-04-27 05:33:37.000000 bmx280_spi-1.0.3/bmx280_spi.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-27 05:33:37.000000 bmx280_spi-1.0.3/bmx280_spi.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       29 2023-04-27 05:33:37.000000 bmx280_spi-1.0.3/bmx280_spi.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-27 05:33:37.000000 bmx280_spi-1.0.3/bmx280_spi.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      927 2023-04-27 05:31:44.000000 bmx280_spi-1.0.3/pyproject.toml
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-27 05:33:37.919878 bmx280_spi-1.0.3/setup.cfg
```

### Comparing `bmx280_spi-1.0.2/LICENSE` & `bmx280_spi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmx280_spi-1.0.2/PKG-INFO` & `bmx280_spi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmx280_spi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module to use the SPI bus to read bmp280/bme280 sensors
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/bmx280_spi/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/bmx280_spi/issues
 Project-URL: Source Code, https://github.com/LearningToPi/bmx280_spi
 Keywords: bmp280,bme280,spi
 Classifier: Topic :: System :: Logging
```

### Comparing `bmx280_spi-1.0.2/README.md` & `bmx280_spi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bmx280_spi-1.0.2/bmx280_spi/__init__.py` & `bmx280_spi-1.0.3/bmx280_spi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,16 +307,14 @@
             True - Settings were successful
             False - An error occured
         '''
         if not self.set_filter(filter):
             return False
         if not self.set_sleep_duration_value(sleep_duration):
             return False
-        if not self.set_power_mode(mode):
-            return False
         if temp_enable:
             if not self.set_temp_oversample(temp_oversample if temp_oversample >= 1 else 1):
                 return False
         else:
             if not self.set_temp_oversample(0):
                 return False
         if pressure_enable:
@@ -328,14 +326,16 @@
         if self.model == 'BME280':
             if humidity_enable:
                 if not self.set_humidity_oversample(humidity_oversample if humidity_oversample >= 1 else 1):
                     return False
             else:
                 if not self.set_humidity_oversample(0):
                     return False
+        if not self.set_power_mode(mode):
+            return False
         return True
 
     def _read_reg(self, reg:int, count=1) -> int:
         ''' Read a register and return the value '''
         with self._lock:
             self._cs.low()
             self._spi.xfer([reg])
@@ -425,14 +425,17 @@
     def set_power_mode(self, value) -> bool:
         ''' Write the power mode. 0 = Standby, 1/2 = Forced, 3 = Normal '''
         if value in MODE_VALUES:
             ctrl_meas = self._read_reg(REG_CTRL_MEAS)
             press_ovsmpl = ctrl_meas & REG_CTRL_MEAS_PRESS_OVERSMPL
             temp_ovsmpl = ctrl_meas & REG_CTRL_MEAS_TEMP_OVERSMPL
             self._logger.debug(f"{self.info_str}: Setting Power Mode to: {value}.  Existing: {(ctrl_meas & REG_CTRL_MEAS_POWER) >> get_trailing_bits(REG_CTRL_MEAS_POWER)}")
+            if value == MODE_FORCED:
+                self._write_single_reg(REG_CTRL_MEAS, temp_ovsmpl + press_ovsmpl + (value if value in MODE_VALUES else 1), check_reply=False if value == MODE_FORCED else True)
+                return True
             return self._write_single_reg(REG_CTRL_MEAS, temp_ovsmpl + press_ovsmpl + (value if value in MODE_VALUES else 1), check_reply=False if value == MODE_FORCED else True)
 
     def set_temp_oversample(self, value) -> bool:
         ''' Write the oversample rate for the temp sensor.  Values 0,1,2,4,8,16 supported.  Returns True/False if successful '''
         if value in OVERSAMPLE_VALUES:
             ctrl_meas = self._read_reg(REG_CTRL_MEAS)
             press_ovsmpl = ctrl_meas & REG_CTRL_MEAS_PRESS_OVERSMPL
@@ -475,15 +478,15 @@
     @property
     def updating(self) -> bool:
         ''' Returns True/False if the sensor is currently writing an update '''
         return (self._read_reg(REG_STATUS) & REG_STATUS_UPDATE) >> get_trailing_bits(REG_STATUS_UPDATE)
 
     def reset_device(self):
         ''' Send a reset command to the device '''
-        self._write_single_reg(REG_RESET, REG_RESET_VALUE)
+        self._write_single_reg(REG_RESET, REG_RESET_VALUE, check_reply=False)
 
     def update_readings(self, timeout=2):
         ''' Update the temp/pressure/humidity readings (depending on platform)
             If in standby - set to force and get reading
             If in normal - collect the last readings from the register
             Returns an instance of Bmx280Readings containing the readings '''
         if self.get_power_mode() == MODE_STANDBY:
```

### Comparing `bmx280_spi-1.0.2/bmx280_spi/__main__.py` & `bmx280_spi-1.0.3/bmx280_spi/__main__.py`

 * *Files identical despite different names*

### Comparing `bmx280_spi-1.0.2/bmx280_spi.egg-info/PKG-INFO` & `bmx280_spi-1.0.3/bmx280_spi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmx280-spi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module to use the SPI bus to read bmp280/bme280 sensors
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/bmx280_spi/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/bmx280_spi/issues
 Project-URL: Source Code, https://github.com/LearningToPi/bmx280_spi
 Keywords: bmp280,bme280,spi
 Classifier: Topic :: System :: Logging
```

### Comparing `bmx280_spi-1.0.2/pyproject.toml` & `bmx280_spi-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bmx280_spi"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python module to use the SPI bus to read bmp280/bme280 sensors"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["bmp280", "bme280", "spi"]
 readme = "README.md"
 requires-python =">=3.6"
 classifiers = [
     "Topic :: System :: Logging",
```

