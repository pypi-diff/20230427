# Comparing `tmp/gtfs_kit-5.2.3.tar.gz` & `tmp/gtfs_kit-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_kit-5.2.3.tar", max compression
+gzip compressed data, was "gtfs_kit-5.2.5.tar", max compression
```

## Comparing `gtfs_kit-5.2.3.tar` & `gtfs_kit-5.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2020-01-13 00:12:47.252710 gtfs_kit-5.2.3/LICENSE.txt
--rw-r--r--   0        0        0     2015 2022-06-28 23:33:46.112057 gtfs_kit-5.2.3/README.rst
--rw-r--r--   0        0        0      304 2022-06-28 23:33:46.112057 gtfs_kit-5.2.3/gtfs_kit/__init__.py
--rw-r--r--   0        0        0     3426 2021-05-16 22:51:23.864327 gtfs_kit-5.2.3/gtfs_kit/calendar.py
--rw-r--r--   0        0        0    10692 2022-06-28 23:33:46.112057 gtfs_kit-5.2.3/gtfs_kit/cleaners.py
--rw-r--r--   0        0        0     6971 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/constants.py
--rw-r--r--   0        0        0    16515 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/feed.py
--rw-r--r--   0        0        0    19581 2021-05-16 22:51:23.864327 gtfs_kit-5.2.3/gtfs_kit/helpers.py
--rw-r--r--   0        0        0    35681 2021-05-16 22:51:23.864327 gtfs_kit-5.2.3/gtfs_kit/miscellany.py
--rw-r--r--   0        0        0    30514 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/routes.py
--rw-r--r--   0        0        0     6648 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/shapes.py
--rw-r--r--   0        0        0     6231 2021-05-16 22:51:23.864327 gtfs_kit-5.2.3/gtfs_kit/stop_times.py
--rw-r--r--   0        0        0    24935 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/stops.py
--rw-r--r--   0        0        0    21337 2021-05-19 03:33:08.240981 gtfs_kit-5.2.3/gtfs_kit/trips.py
--rw-r--r--   0        0        0    49077 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/gtfs_kit/validators.py
--rw-r--r--   0        0        0      815 2022-06-28 23:33:46.116057 gtfs_kit-5.2.3/pyproject.toml
--rw-r--r--   0        0        0     2834 2022-06-28 23:34:23.103805 gtfs_kit-5.2.3/setup.py
--rw-r--r--   0        0        0     2949 2022-06-28 23:34:23.104069 gtfs_kit-5.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-01-09 20:55:35.590106 gtfs_kit-5.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1937 2023-04-27 00:05:00.839952 gtfs_kit-5.2.5/README.rst
+-rw-r--r--   0        0        0      304 2023-04-27 00:05:00.839952 gtfs_kit-5.2.5/gtfs_kit/__init__.py
+-rw-r--r--   0        0        0     3426 2021-04-28 23:42:59.436692 gtfs_kit-5.2.5/gtfs_kit/calendar.py
+-rw-r--r--   0        0        0    10692 2022-04-12 04:10:10.474482 gtfs_kit-5.2.5/gtfs_kit/cleaners.py
+-rw-r--r--   0        0        0     6971 2022-01-17 03:01:47.667252 gtfs_kit-5.2.5/gtfs_kit/constants.py
+-rw-r--r--   0        0        0    16515 2022-04-13 02:04:39.526021 gtfs_kit-5.2.5/gtfs_kit/feed.py
+-rw-r--r--   0        0        0    19581 2021-11-25 21:52:10.388179 gtfs_kit-5.2.5/gtfs_kit/helpers.py
+-rw-r--r--   0        0        0    35644 2023-04-27 00:05:00.843952 gtfs_kit-5.2.5/gtfs_kit/miscellany.py
+-rw-r--r--   0        0        0    30514 2022-07-05 02:59:12.080231 gtfs_kit-5.2.5/gtfs_kit/routes.py
+-rw-r--r--   0        0        0     6648 2022-07-05 02:59:12.080231 gtfs_kit-5.2.5/gtfs_kit/shapes.py
+-rw-r--r--   0        0        0     6231 2022-04-13 02:04:39.526021 gtfs_kit-5.2.5/gtfs_kit/stop_times.py
+-rw-r--r--   0        0        0    24935 2022-04-26 01:06:51.650776 gtfs_kit-5.2.5/gtfs_kit/stops.py
+-rw-r--r--   0        0        0    21337 2021-11-25 21:52:10.392179 gtfs_kit-5.2.5/gtfs_kit/trips.py
+-rw-r--r--   0        0        0    49077 2022-04-26 21:35:43.321257 gtfs_kit-5.2.5/gtfs_kit/validators.py
+-rw-r--r--   0        0        0     1077 2023-04-27 00:05:00.847952 gtfs_kit-5.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 gtfs_kit-5.2.5/setup.py
+-rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 gtfs_kit-5.2.5/PKG-INFO
```

### Comparing `gtfs_kit-5.2.3/LICENSE.txt` & `gtfs_kit-5.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/README.rst` & `gtfs_kit-5.2.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 GTFS Kit
 ********
-.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/run_tests.yml/badge.svg
+.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg
 
 GTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.
 It uses Pandas and Shapely to do the heavy lifting.
 
-This project supersedes `GTFSTK <https://github.com/mrcagney/gtfstk>`_.
-
 
 Installation
 =============
 ``poetry add gtfs_kit``.
 
 
 Examples
```

### Comparing `gtfs_kit-5.2.3/gtfs_kit/calendar.py` & `gtfs_kit-5.2.5/gtfs_kit/calendar.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/cleaners.py` & `gtfs_kit-5.2.5/gtfs_kit/cleaners.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/constants.py` & `gtfs_kit-5.2.5/gtfs_kit/constants.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/feed.py` & `gtfs_kit-5.2.5/gtfs_kit/feed.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/helpers.py` & `gtfs_kit-5.2.5/gtfs_kit/helpers.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/miscellany.py` & `gtfs_kit-5.2.5/gtfs_kit/miscellany.py`

 * *Files 2% similar despite different names*

```diff
@@ -860,25 +860,26 @@
       the scren line; one trip could cross multiple times
     - ``'crossing_direction'``: 1 or -1; 1 indicates trip travel from the
       left side to the right side of the screen line;
       -1 indicates trip travel in the  opposite direction
 
     Notes:
 
-    - Assume the Feed's stop times DataFrame has an accurate ``shape_dist_traveled`` column.
+    - Assume the Feed's stop times DataFrame has an accurate ``shape_dist_traveled``
+      column.
     - Assume that trips travel in the same direction as their shapes, an assumption
       that is part of the GTFS.
     - Assume that the screen line is straight and simple.
     - Probably does not give correct results for trips with self-intersecting shapes.
     - The algorithm works as follows
 
         1. Find the trip shapes that intersect the screen lines.
-        2. For each such shape and screen line, compute the intersection points, the distance
-           of the point along the shape, and the orientation of the screen line relative to
-           the shape.
+        2. For each such shape and screen line, compute the intersection points,
+           the distance of the point along the shape, and the orientation of the screen
+           line relative to the shape.
         3. For each given date, restrict to trips active on the
            date and interpolate a stop time for the intersection point using
            the ``shape_dist_traveled`` column.
         4. Use that interpolated time as the crossing time of the trip vehicle.
 
     """
     dates = feed.subset_dates(dates)
@@ -893,61 +894,61 @@
     screen_lines = screen_lines.to_crs(crs)
 
     # Create screen line IDs if necessary
     n = screen_lines.shape[0]
     if "screen_line_id" not in screen_lines.columns:
         screen_lines["screen_line_id"] = hp.make_ids(n, "sl")
 
-    # Make a vector in the direction of each screen line to calculate crossing orientation.
-    # Does not work in case of a bent screen line.
-    p1 = screen_lines.geometry.map(lambda x: np.array(x.coords[0]))
-    p2 = screen_lines.geometry.map(lambda x: np.array(x.coords[-1]))
+    # Make a vector in the direction of each screen line to calculate crossing
+    # orientation. Does not work in case of a bent screen line.
+    p1 = screen_lines["geometry"].map(lambda x: np.array(x.coords[0]))
+    p2 = screen_lines["geometry"].map(lambda x: np.array(x.coords[-1]))
     screen_lines["screen_line_vector"] = p2 - p1
 
     # Get intersection points of shapes and screen lines
     g0 = (
         # Only keep shapes that intersect screen lines to reduce computations
         gp.sjoin(shapes_g, screen_lines.filter(["screen_line_id", "geometry"])).merge(
             screen_lines, on="screen_line_id"
         )
         # Compute intersection points
         .assign(
-            int_point=lambda x: gp.GeoSeries(x.geometry_x, crs=crs).intersection(
-                gp.GeoSeries(x.geometry_y, crs=crs)
+            int_point=lambda x: gp.GeoSeries(x["geometry_x"], crs=crs).intersection(
+                gp.GeoSeries(x["geometry_y"], crs=crs)
             )
         )
     )
 
     # Unpack multipoint intersections to yield a new GeoDataFrame
     records = []
     for row in g0.itertuples(index=False):
         if isinstance(row.int_point, sg.Point):
             intersections = [row.int_point]
         else:
-            intersections = row.int_point
+            intersections = row.int_point.geoms
         for int_point in intersections:
             record = {
                 "shape_id": row.shape_id,
                 "screen_line_id": row.screen_line_id,
                 "geometry": row.geometry_x,
                 "int_point": int_point,
                 "screen_line_vector": row.screen_line_vector,
             }
             records.append(record)
 
     g = gp.GeoDataFrame.from_records(records)
     g.crs = crs
 
     # Get distance (in meters) of each intersection point along shape
-    g["crossing_dist"] = g.apply(lambda x: x.geometry.project(x.int_point), axis=1)
+    g["crossing_dist"] = g.apply(lambda x: x["geometry"].project(x.int_point), axis=1)
 
     # Build a tiny vector along each shape
-    p2 = g.apply(lambda x: x.geometry.interpolate(x.crossing_dist + 1), axis=1).map(
-        lambda x: np.array(x.coords[0])
-    )
+    p2 = g.apply(
+        lambda x: x["geometry"].interpolate(x["crossing_dist"] + 1), axis=1
+    ).map(lambda x: np.array(x.coords[0]))
     p1 = g.int_point.map(lambda x: np.array(x.coords[0]))
     g["shape_vector"] = p2 - p1
 
     # Compute crossing direction by taking the vector cross product of
     # the shape vector and the screen line vector
     det = g.apply(
         lambda x: np.linalg.det(np.array([x.shape_vector, x.screen_line_vector])),
@@ -966,55 +967,53 @@
         .sort_values(
             ["shape_id", "crossing_dist"]
         )  # Need this sorting for interpolation to work
     )
 
     # Get stop times of trips whose shapes lie in h
     st = (
-        feed.trips.loc[lambda x: x.shape_id.isin(h.index)]
+        feed.trips.loc[lambda x: x["shape_id"].isin(h.index)]
         # Merge in route short names and stop times
         .merge(feed.routes[["route_id", "route_short_name"]]).merge(feed.stop_times)
         # Keep only non-NaN departure times
-        .loc[lambda x: x.departure_time.notna()]
+        .loc[lambda x: x["departure_time"].notna()]
         # Convert to seconds past midnight
-        .assign(departure_time=lambda x: x.departure_time.map(hp.timestr_to_seconds))
+        .assign(departure_time=lambda x: x["departure_time"].map(hp.timestr_to_seconds))
     )
 
     # Compute crossing times by date
     records = []
     ta = feed.compute_trip_activity(dates)
     for date in dates:
         # Subset to trips active on date and merge with g
         ids = ta.loc[lambda x: x[date] == 1, "trip_id"]
-        f = st.loc[lambda x: x.trip_id.isin(ids)].sort_values(
+        f = st.loc[lambda x: x["trip_id"].isin(ids)].sort_values(
             ["trip_id", "shape_dist_traveled"]
         )  # Need this sorting for interpolation to work
 
         # Get crossing time for each trip
         for tid, group in f.groupby("trip_id"):
             sid = group["shape_id"].iat[0]
-            rid = group["route_id"].iat[0]
-            rsn = group["route_short_name"].iat[0]
             dists = group["shape_dist_traveled"].values
             times = group["departure_time"].values
             crossing_dists = h.loc[[sid], "crossing_dist"].values
             crossing_times = np.interp(crossing_dists, dists, times)
             for i, row in enumerate(h.loc[[sid]].itertuples(index=False)):
                 record = {
                     "date": date,
                     "trip_id": tid,
-                    "route_id": group.route_id.iat[0],
-                    "route_short_name": group.route_short_name.iat[0],
-                    "shape_id": group.shape_id.iat[0],
+                    "route_id": group["route_id"].iat[0],
+                    "route_short_name": group["route_short_name"].iat[0],
+                    "shape_id": group["shape_id"].iat[0],
                     "screen_line_id": row.screen_line_id,
                     "crossing_direction": row.crossing_direction,
                     "crossing_distance": row.crossing_dist,
                     "crossing_time": crossing_times[i],
                 }
                 records.append(record)
 
     result = pd.DataFrame.from_records(records).assign(
-        crossing_time=lambda x: x.crossing_time.map(
+        crossing_time=lambda x: x["crossing_time"].map(
             lambda x: hp.timestr_to_seconds(x, inverse=True)
         )
     )
     return result
```

### Comparing `gtfs_kit-5.2.3/gtfs_kit/routes.py` & `gtfs_kit-5.2.5/gtfs_kit/routes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/shapes.py` & `gtfs_kit-5.2.5/gtfs_kit/shapes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/stop_times.py` & `gtfs_kit-5.2.5/gtfs_kit/stop_times.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/stops.py` & `gtfs_kit-5.2.5/gtfs_kit/stops.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/trips.py` & `gtfs_kit-5.2.5/gtfs_kit/trips.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/gtfs_kit/validators.py` & `gtfs_kit-5.2.5/gtfs_kit/validators.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.3/pyproject.toml` & `gtfs_kit-5.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 [tool.poetry]
 name = "gtfs_kit"
-version = "5.2.3"
+version = "5.2.5"
 description = "A Python 3.8+ library for analyzing GTFS feeds."
 authors = ["Alex Raichev <araichev@mrcagney.com>"]
 readme = "README.rst"
 license = "MIT"
 repository = "https://github.com/mrcagney/gtfs_kit"
 documentation = "https://mrcagney.github.io/gtfs_kit_docs"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 pandas = ">=1"
-shapely = ">=1"
+shapely = ">=1.8"
 pycountry = ">=19"
 utm = ">=0"
 json2html = ">=1"
 geopandas = ">=0"
 rtree = ">=0"
 folium = ">=0"
 requests = ">=2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 jupyter = "*"
 pytest = ">=6"
 sphinx = ">=3"
 pre-commit = ">=0"
-black = ">22"
-publish_sphinx_docs = ">=1.0"
 matplotlib = ">=1"
 pytest-socket = ">=0"
+black = ">22"
 nbstripout = ">=0.5"
+ruff = ">=0.0.257"
+publish_sphinx_docs = ">=1.0"
 
 [build-system]
 requires = ["poetry>=1"]
 build-backend = "poetry.masonry.api"
 
+[tool.pytest.ini_options]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+    "serial",
+]
+
+[tool.ruff]
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+ignore = ["F403"]
```

### Comparing `gtfs_kit-5.2.3/setup.py` & `gtfs_kit-5.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ['folium>=0',
  'geopandas>=0',
  'json2html>=1',
  'pandas>=1',
  'pycountry>=19',
  'requests>=2',
  'rtree>=0',
- 'shapely>=1',
+ 'shapely>=1.8',
  'utm>=0']
 
 setup_kwargs = {
     'name': 'gtfs-kit',
-    'version': '5.2.3',
+    'version': '5.2.5',
     'description': 'A Python 3.8+ library for analyzing GTFS feeds.',
-    'long_description': "GTFS Kit\n********\n.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/run_tests.yml/badge.svg\n\nGTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.\nIt uses Pandas and Shapely to do the heavy lifting.\n\nThis project supersedes `GTFSTK <https://github.com/mrcagney/gtfstk>`_.\n\n\nInstallation\n=============\n``poetry add gtfs_kit``.\n\n\nExamples\n========\nYou can find examples in the Jupyter notebook ``notebooks/examples.ipynb``.\n\n\nAuthors\n=========\n- Alex Raichev (2019-09), maintainer\n\n\nDocumentation\n=============\nDocumentation is built via Sphinx from the source code in the ``docs`` directory then published to Github Pages at `mrcagney.github.io/gtfs_kit_docs <https://mrcagney.github.io/gtfs_kit_docs>`_.\n\n\nNotes\n=====\n- This project's development status is Alpha.\n  I use GTFS Kit for work and change it breakingly to suit my needs.\n- This project uses semantic versioning.\n- I aim for GTFS Kit to handle `the current GTFS <https://developers.google.com/transit/gtfs/reference>`_.\n  In particular, i avoid handling `GTFS extensions <https://developers.google.com/transit/gtfs/reference/gtfs-extensions>`_.\n  That is the most reasonable scope boundary i can draw at present, given this project's tiny budget.\n  If you would like to fund me to expand that scope, feel free to email me.\n- Thanks to `MRCagney <http://www.mrcagney.com/>`_ for periodically donating to this project.\n- Constructive feedback and contributions are welcome.\n  Please issue pull requests from a feature branch into the ``develop`` branch and include tests.\n- GTFS time is measured relative noon minus 12 hours, which can mess things up when crossing into daylight savings time.\n  I don't think this issue causes any bugs in GTFS Kit, but you and i have been warned.\n  Thanks to user derhuerst for bringing this to my attention in `closed Issue 8 <https://github.com/mrcagney/gtfs_kit/issues/8#issue-1063633457>`_.\n",
+    'long_description': "GTFS Kit\n********\n.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg\n\nGTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.\nIt uses Pandas and Shapely to do the heavy lifting.\n\n\nInstallation\n=============\n``poetry add gtfs_kit``.\n\n\nExamples\n========\nYou can find examples in the Jupyter notebook ``notebooks/examples.ipynb``.\n\n\nAuthors\n=========\n- Alex Raichev (2019-09), maintainer\n\n\nDocumentation\n=============\nDocumentation is built via Sphinx from the source code in the ``docs`` directory then published to Github Pages at `mrcagney.github.io/gtfs_kit_docs <https://mrcagney.github.io/gtfs_kit_docs>`_.\n\n\nNotes\n=====\n- This project's development status is Alpha.\n  I use GTFS Kit for work and change it breakingly to suit my needs.\n- This project uses semantic versioning.\n- I aim for GTFS Kit to handle `the current GTFS <https://developers.google.com/transit/gtfs/reference>`_.\n  In particular, i avoid handling `GTFS extensions <https://developers.google.com/transit/gtfs/reference/gtfs-extensions>`_.\n  That is the most reasonable scope boundary i can draw at present, given this project's tiny budget.\n  If you would like to fund me to expand that scope, feel free to email me.\n- Thanks to `MRCagney <http://www.mrcagney.com/>`_ for periodically donating to this project.\n- Constructive feedback and contributions are welcome.\n  Please issue pull requests from a feature branch into the ``develop`` branch and include tests.\n- GTFS time is measured relative noon minus 12 hours, which can mess things up when crossing into daylight savings time.\n  I don't think this issue causes any bugs in GTFS Kit, but you and i have been warned.\n  Thanks to user derhuerst for bringing this to my attention in `closed Issue 8 <https://github.com/mrcagney/gtfs_kit/issues/8#issue-1063633457>`_.\n",
     'author': 'Alex Raichev',
     'author_email': 'araichev@mrcagney.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mrcagney/gtfs_kit',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4',
 }
```

### Comparing `gtfs_kit-5.2.3/PKG-INFO` & `gtfs_kit-5.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: gtfs-kit
-Version: 5.2.3
+Version: 5.2.5
 Summary: A Python 3.8+ library for analyzing GTFS feeds.
 Home-page: https://github.com/mrcagney/gtfs_kit
 License: MIT
 Author: Alex Raichev
 Author-email: araichev@mrcagney.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: folium (>=0)
 Requires-Dist: geopandas (>=0)
 Requires-Dist: json2html (>=1)
 Requires-Dist: pandas (>=1)
 Requires-Dist: pycountry (>=19)
 Requires-Dist: requests (>=2)
 Requires-Dist: rtree (>=0)
-Requires-Dist: shapely (>=1)
+Requires-Dist: shapely (>=1.8)
 Requires-Dist: utm (>=0)
 Project-URL: Documentation, https://mrcagney.github.io/gtfs_kit_docs
 Project-URL: Repository, https://github.com/mrcagney/gtfs_kit
 Description-Content-Type: text/x-rst
 
 GTFS Kit
 ********
-.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/run_tests.yml/badge.svg
+.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg
 
 GTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.
 It uses Pandas and Shapely to do the heavy lifting.
 
-This project supersedes `GTFSTK <https://github.com/mrcagney/gtfstk>`_.
-
 
 Installation
 =============
 ``poetry add gtfs_kit``.
 
 
 Examples
```

