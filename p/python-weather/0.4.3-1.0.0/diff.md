# Comparing `tmp/python-weather-0.4.3.tar.gz` & `tmp/python-weather-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-weather-0.4.3.tar", last modified: Sun Oct 23 13:08:22 2022, max compression
+gzip compressed data, was "python-weather-1.0.0.tar", last modified: Thu Apr 27 17:25:51 2023, max compression
```

## Comparing `python-weather-0.4.3.tar` & `python-weather-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-10-23 13:08:22.632822 python-weather-0.4.3/
--rw-rw-rw-   0        0        0     1139 2022-10-23 12:50:07.000000 python-weather-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     2308 2022-10-23 13:08:22.632822 python-weather-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1446 2022-10-23 12:50:07.000000 python-weather-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-23 13:08:22.601575 python-weather-0.4.3/python_weather/
--rw-rw-rw-   0        0        0     1433 2022-10-23 13:03:10.000000 python-weather-0.4.3/python_weather/__init__.py
--rw-rw-rw-   0        0        0     2918 2022-10-23 12:50:07.000000 python-weather-0.4.3/python_weather/client.py
--rw-rw-rw-   0        0        0      506 2022-10-23 12:50:07.000000 python-weather-0.4.3/python_weather/constants.py
--rw-rw-rw-   0        0        0     4749 2022-10-23 12:50:07.000000 python-weather-0.4.3/python_weather/enums.py
--rw-rw-rw-   0        0        0      933 2022-10-23 12:50:07.000000 python-weather-0.4.3/python_weather/errors.py
--rw-rw-rw-   0        0        0    16328 2022-10-23 13:02:03.000000 python-weather-0.4.3/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2022-10-23 13:08:22.632822 python-weather-0.4.3/python_weather.egg-info/
--rw-rw-rw-   0        0        0     2308 2022-10-23 13:08:22.000000 python-weather-0.4.3/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2022-10-23 13:08:22.000000 python-weather-0.4.3/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-23 13:08:22.000000 python-weather-0.4.3/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-10-23 13:08:22.000000 python-weather-0.4.3/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-10-23 13:08:22.000000 python-weather-0.4.3/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-10-23 13:08:22.632822 python-weather-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1060 2022-10-23 13:03:22.000000 python-weather-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.886263 python-weather-1.0.0/
+-rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3760 2023-04-27 17:25:51.886263 python-weather-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2023-04-27 17:25:05.000000 python-weather-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1437 2023-04-27 17:12:14.000000 python-weather-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.839392 python-weather-1.0.0/python_weather/
+-rw-rw-rw-   0        0        0     1503 2023-04-24 06:22:15.000000 python-weather-1.0.0/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     5663 2023-04-24 15:06:57.000000 python-weather-1.0.0/python_weather/base.py
+-rw-rw-rw-   0        0        0     5697 2023-04-23 09:54:58.000000 python-weather-1.0.0/python_weather/client.py
+-rw-rw-rw-   0        0        0     1313 2023-04-23 08:55:28.000000 python-weather-1.0.0/python_weather/constants.py
+-rw-rw-rw-   0        0        0    10164 2023-04-24 15:21:41.000000 python-weather-1.0.0/python_weather/enums.py
+-rw-rw-rw-   0        0        0     1262 2023-04-16 12:24:11.000000 python-weather-1.0.0/python_weather/errors.py
+-rw-rw-rw-   0        0        0    12805 2023-04-24 15:16:05.000000 python-weather-1.0.0/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.886263 python-weather-1.0.0/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3760 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 17:25:51.886263 python-weather-1.0.0/setup.cfg
```

### Comparing `python-weather-0.4.3/LICENSE` & `python-weather-1.0.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2021-2022 null (http://github.com/null8626/python-weather)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2021-2023 null (https://github.com/null8626)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `python-weather-0.4.3/python_weather/__init__.py` & `python-weather-1.0.0/python_weather/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-"""
-python-weather
-a free and asynchronous python API Wrapper of the Weather API.
-
-The MIT License (MIT)
-
-Copyright (c) 2021-2022 null (http://github.com/null8626/python-weather)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from .client import Client
-from .errors import Error, InvalidArg
-from .constants import METRIC, IMPERIAL
-
-__version__ = "0.4.3"
-__all__ = ('METRIC', 'IMPERIAL', 'Client', 'Error', 'InvalidArg')
+"""
+python-weather
+A free and asynchronous weather API wrapper made in Python, for Python.
+
+The MIT License (MIT)
+
+Copyright (c) 2021-2023 null (https://github.com/null8626)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the 'Software'), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from .enums import Kind, Locale, Phase, Ultraviolet, WindDirection
+from .constants import METRIC, IMPERIAL
+from .client import Client
+from .errors import Error
+
+__version__ = '1.0.0'
+__all__ = (
+  'METRIC', 'IMPERIAL', 'Client', 'Error', 'Kind', 'Locale', 'Phase',
+  'Ultraviolet', 'WindDirection'
+)
```

