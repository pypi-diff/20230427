# Comparing `tmp/bmkg-1.0.2.tar.gz` & `tmp/bmkg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmkg-1.0.2.tar", last modified: Sun Apr 23 17:36:26 2023, max compression
+gzip compressed data, was "bmkg-1.0.3.tar", last modified: Thu Apr 27 17:09:21 2023, max compression
```

## Comparing `bmkg-1.0.2.tar` & `bmkg-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.686850 bmkg-1.0.2/
--rw-rw-rw-   0        0        0     1066 2023-04-23 17:28:59.000000 bmkg-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-23 17:28:59.000000 bmkg-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3635 2023-04-23 17:36:26.684848 bmkg-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2077 2023-04-23 17:28:59.000000 bmkg-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.612796 bmkg-1.0.2/bmkg/
--rw-rw-rw-   0        0        0     1479 2023-04-23 17:33:35.000000 bmkg-1.0.2/bmkg/__init__.py
--rw-rw-rw-   0        0        0     2059 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/base.py
--rw-rw-rw-   0        0        0     9065 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/client.py
--rw-rw-rw-   0        0        0     1431 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/constants.py
--rw-rw-rw-   0        0        0     3914 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/earthquake.py
--rw-rw-rw-   0        0        0     4887 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/enums.py
--rw-rw-rw-   0        0        0     1248 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/errors.py
--rw-rw-rw-   0        0        0     8356 2023-04-23 17:32:32.000000 bmkg-1.0.2/bmkg/forecast.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.681847 bmkg-1.0.2/bmkg.egg-info/
--rw-rw-rw-   0        0        0     3635 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-04-23 17:33:35.000000 bmkg-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 17:36:26.687857 bmkg-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.824301 bmkg-1.0.3/
+-rw-rw-rw-   0        0        0     1066 2023-04-27 17:04:41.000000 bmkg-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-04-27 17:04:41.000000 bmkg-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6312 2023-04-27 17:09:21.824301 bmkg-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-04-27 17:04:41.000000 bmkg-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.793048 bmkg-1.0.3/bmkg/
+-rw-rw-rw-   0        0        0     1479 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/base.py
+-rw-rw-rw-   0        0        0     8862 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/client.py
+-rw-rw-rw-   0        0        0     1431 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/constants.py
+-rw-rw-rw-   0        0        0     4184 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/earthquake.py
+-rw-rw-rw-   0        0        0     6098 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/enums.py
+-rw-rw-rw-   0        0        0     1248 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/errors.py
+-rw-rw-rw-   0        0        0     8356 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.808676 bmkg-1.0.3/bmkg.egg-info/
+-rw-rw-rw-   0        0        0     6312 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1450 2023-04-27 17:08:29.000000 bmkg-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 17:09:21.824301 bmkg-1.0.3/setup.cfg
```

### Comparing `bmkg-1.0.2/LICENSE` & `bmkg-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.2/bmkg/__init__.py` & `bmkg-1.0.3/bmkg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 SOFTWARE.
 """
 
 from .enums import AreaKind, Direction, ForecastKind, MMI, Province
 from .constants import METRIC, IMPERIAL
 from .client import Client
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 __all__ = (
   'AreaKind', 'Client', 'Direction', 'ForecastKind', 'METRIC', 'MMI',
   'IMPERIAL', 'Province'
 )
```

### Comparing `bmkg-1.0.2/bmkg/base.py` & `bmkg-1.0.3/bmkg/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,31 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from enum import auto
+from enum import auto, Enum
 
 from .constants import METRIC, VALID_UNITS
 
+class BasicEnum(Enum):
+  __slots__ = ()
+  
+  def __repr__(self) -> str:
+    """:class:`str`: The string representation of this object."""
+    
+    return f'{self.__class__.__name__}.{self.name}'
+  
+  def __str__(self) -> str:
+    """:class:`str`: The stylized name for this :class:`Enum`."""
+    
+    return self.name.replace('_', ' ').title()
+
 class CustomizableUnit:
   __slots__ = ('__unit', 'english')
   
   def __init__(self, unit: auto, english: bool):
     self.unit = unit
     self.english = english
```

### Comparing `bmkg-1.0.2/bmkg/client.py` & `bmkg-1.0.3/bmkg/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 from .constants import METRIC, VALID_UNITS
 from .base import CustomizableUnit
 from .forecast import Weather
 from .enums import Province
 from .errors import Error
 
 class Client(CustomizableUnit):
-  """Represents a ``python_weather`` :class:`Client` class."""
+  """Represents a ``bmkg`` :class:`Client` class."""
   
   __slots__ = ('__session', 'english')
   
   def __init__(
     self,
     *,
     unit: Optional[auto] = METRIC,
     english: bool = False,
     session: Optional[ClientSession] = None
   ):
     """
-    Creates the python_weather client object.
+    Creates the bmkg client object.
     
     Parameters
     ----------
     unit: Optional[:class:`auto`]
       Whether to use the :term:`metric` or :term:`imperial/customary system` (:attr:`IMPERIAL`). Defaults to :attr:`METRIC`.
     english: 
       Whether to use the :term:`english language` (``True``) or the :term:`native indonesian language` (``False``). Defaults to ``False``.
@@ -66,25 +66,24 @@
       timeout=ClientTimeout(total=5000.0),
       connector=TCPConnector(verify_ssl=False)
     )
   
   def __repr__(self) -> str:
     """:class:`str`: The string representation of this object."""
     
-    return f'<{self.__class__.__name__} {self.__session!r}>'
+    return f'<{self.__class__.__name__} [{self.__session!r}]>'
   
   async def get_forecast(
     self,
-    province: Optional[Union[
-      str, Province]] = Province.INDONESIA,  # indonesia is not a province wtf
+    province: Optional[Union[str, Province]] = Province.INDONESIA,
     *,
     unit: Optional[auto] = None
-  ) -> Weather:
+  ) -> Weather: # yapf: disable
     """|coro|
-    Fetches a weather forecast for a specific province.
+    Fetches a weather forecast of a specific province.
     
     Parameters
     ----------
     province: Optional[Union[:class:`str`, :class:`Province`]]
       The requested :class:`Province` :class:`Enum` or province name in the form of a :class:`str` for said weather forecast. Defaults to :attr:`Province.INDONESIA`.
     unit: Optional[:class:`auto`]
       Overrides the :term:`metric` or :term:`imperial/customary system` (:attr:`IMPERIAL`) used by the :class:`Client` object. Defaults to ``None`` (uses the one from the :class:`Client`).
@@ -102,33 +101,33 @@
     :class:`Weather`
       The requested weather forecast.
     """
     
     if self.__session.closed:
       raise Error('Client is already closed')
     
-    province = province if isinstance(province,
-                                      Province) else Province(province)
+    province = province if isinstance(province, Province) else Province(province) # yapf: disable
     
     if unit not in VALID_UNITS:
       unit = self._CustomizableUnit__unit
     
     async with self.__session.get(
       f'https://data.bmkg.go.id/DataMKG/MEWS/DigitalForecast/DigitalForecast-{province.value}.xml'
     ) as resp:
       return Weather(
         fromstring(await resp.text()).find('forecast'), unit, self.english
       )
   
-  async def get_felt_earthquakes(self,
-                                 *,
-                                 unit: Optional[auto] = None
-                                 ) -> Iterable[FeltEarthquake]:
+  async def get_felt_earthquakes(
+    self,
+    *,
+    unit: Optional[auto] = None
+  ) -> Iterable[FeltEarthquake]: # yapf: disable
     """|coro|
-    Fetches the recent earthquakes regardless of their magnitude.
+    Fetches the most recent earthquakes regardless of their magnitude.
     
     Parameters
     ----------
     unit: Optional[:class:`auto`]
       Overrides the :term:`metric` or :term:`imperial/customary system` (:attr:`IMPERIAL`) used by the :class:`Client` object. Defaults to ``None`` (uses the one from the :class:`Client`).
     
     Raises
@@ -152,20 +151,21 @@
     ) as resp:
       json = await resp.json()
       return (
         FeltEarthquake(earthquake, unit, self.english)
         for earthquake in json['Infogempa']['gempa']
       )
   
-  async def get_recent_earthquakes(self,
-                                   *,
-                                   unit: Optional[auto] = None
-                                   ) -> Iterable[RecentEarthquake]:
+  async def get_recent_earthquakes(
+    self,
+    *,
+    unit: Optional[auto] = None
+  ) -> Iterable[RecentEarthquake]: # yapf: disable
     """|coro|
-    Fetches the recent earthquakes with the magnitude >= 5.0.
+    Fetches the most recent earthquakes magnitude 5 or higher.
     
     Parameters
     ----------
     unit: Optional[:class:`auto`]
       Overrides the :term:`metric` or :term:`imperial/customary system` (:attr:`IMPERIAL`) used by the :class:`Client` object. Defaults to ``None`` (uses the one from the :class:`Client`).
     
     Raises
```

### Comparing `bmkg-1.0.2/bmkg/constants.py` & `bmkg-1.0.3/bmkg/constants.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.2/bmkg/earthquake.py` & `bmkg-1.0.3/bmkg/earthquake.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,19 @@
   __slots__ = ('__inner',)
   
   def __init__(self, inner: dict, unit: auto, english: bool):
     super().__init__(unit, english)
     
     self.__inner = inner
   
+  def __repr__(self) -> str:
+    """:class:`str`: The string representation of this object."""
+    
+    return f'<{self.__class__.__name__} date={self.date!r} latitude={self.latitude!r} longitude={self.longitude!r} magnitude={self.magnitude!r} depth={self.depth!r}>'
+  
   @property
   def date(self) -> datetime:
     """:class:`datetime`: The date when this earthquake happened in UTC."""
     
     return datetime.fromisoformat(self.__inner['DateTime'])
   
   @property
```

### Comparing `bmkg-1.0.2/bmkg/errors.py` & `bmkg-1.0.3/bmkg/errors.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.2/bmkg/forecast.py` & `bmkg-1.0.3/bmkg/forecast.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.2/pyproject.toml` & `bmkg-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "bmkg"
-version = "1.0.2"
+version = "1.0.3"
 description = "Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
-keywords = ["weather", "bmkg", "indonesia", "wrapper"]
+keywords = ["weather", "forecast", "indonesia", "weather-api", "weather-forecast", "bmkg"]
 dependencies = ["aiohttp>=3.0.0"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: aiohttp",
   "Framework :: AsyncIO",
   "Intended Audience :: Education",
   "Intended Audience :: Developers",
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/bmkg"
-download_url = "https://github.com/null8626/bmkg/archive/1.0.2.tar.gz"
+download_url = "https://github.com/null8626/bmkg/archive/1.0.3.tar.gz"
```

