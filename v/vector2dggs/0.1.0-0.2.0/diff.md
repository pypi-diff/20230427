# Comparing `tmp/vector2dggs-0.1.0.tar.gz` & `tmp/vector2dggs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.1.0.tar", max compression
+gzip compressed data, was "vector2dggs-0.2.0.tar", max compression
```

## Comparing `vector2dggs-0.1.0.tar` & `vector2dggs-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6312 2023-04-26 04:21:36.281503 vector2dggs-0.1.0/README.md
--rw-r--r--   0        0        0     1049 2023-04-26 22:00:52.100201 vector2dggs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 21:07:25.956152 vector2dggs-0.1.0/vector2dggs/__init__.py
--rw-r--r--   0        0        0      520 2023-04-26 00:14:53.266711 vector2dggs-0.1.0/vector2dggs/cli.py
--rw-r--r--   0        0        0     7953 2023-04-26 04:22:14.693702 vector2dggs-0.1.0/vector2dggs/h3.py
--rw-r--r--   0        0        0     2817 2023-04-26 00:14:53.266711 vector2dggs-0.1.0/vector2dggs/katana.py
--rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vector2dggs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7644 2023-04-27 01:25:13.759218 vector2dggs-0.2.0/README.md
+-rw-r--r--   0        0        0     1092 2023-04-27 01:24:44.707080 vector2dggs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 21:07:25.956152 vector2dggs-0.2.0/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      520 2023-04-26 00:14:53.266711 vector2dggs-0.2.0/vector2dggs/cli.py
+-rw-r--r--   0        0        0     9325 2023-04-27 01:25:16.919233 vector2dggs-0.2.0/vector2dggs/h3.py
+-rw-r--r--   0        0        0     2817 2023-04-26 00:14:53.266711 vector2dggs-0.2.0/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9078 1970-01-01 00:00:00.000000 vector2dggs-0.2.0/PKG-INFO
```

### Comparing `vector2dggs-0.1.0/README.md` & `vector2dggs-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # vector2dggs
 
+[![pypi](https://img.shields.io/pypi/v/vector2dggs?label=vector2dggs)](https://pypi.org/project/vector2dggs/)
+
 Python-based CLI tool to index raster files to DGGS in parallel, writing out to Parquet.
 
 This is the vector equivalent of [raster2dggs](https://github.com/manaakiwhenua/raster2dggs).
 
 Currently only supports H3 DGGS, and probably has other limitations since it has been developed for a specific internal use case, though it is intended as a general-purpose abstraction. Contributions, suggestions, bug reports and strongly worded letters are all welcome.
 
 Currently only supports polygons.
@@ -14,48 +16,66 @@
 
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
 
-  VECTOR_INPUT is the path to input vector geospatial data.
-  OUTPUT_DIRECTORY should be a directorty, not a file, as it will be the
-  write location for an Apache Parquet data store.
+  VECTOR_INPUT is the path to input vector geospatial data. OUTPUT_DIRECTORY
+  should be a directory, not a file, as it will be the write location for an
+  Apache Parquet data store.
 
 Options:
-  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO
-                                  or DEBUG  [default: INFO]
+  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
+                                  DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
-  -a, --all_attributes            Retain attributes in output. The
-                                  default is to create an output that
-                                  only includes H3 cell ID and the ID(s)
-                                  given by the -id field (or the default
-                                  index ID).
-  -p, --partitions INTEGER        Geo-partitioning, currently only
-                                  available in Hilbert method  [default:
-                                  50; required]
-  -s, --spatial-sorting [hilbert|morton|geohash]
-                                  Spatial sorting method  [default:
-                                  hilbert]
-  -crs, --cut_crs INTEGER         Set crs(epsg) to input layer (used for
-                                  cutting), defaults to input crs
-  -c, --cut_threshold INTEGER     Cutting up large polygons into target
-                                  length (meters)  [default: 5000;
+  -k, --keep_attributes           Retain attributes in output. The default is
+                                  to create an output that only includes H3
+                                  cell ID and the ID given by the -id field
+                                  (or the default index ID).
+  -p, --partitions INTEGER        The number of partitions to create.
+                                  Recommendation: at least as many partitions
+                                  as there are available `--threads`.
+                                  Partitions are processed in parallel once
+                                  they have been formed.  [default: 50;
                                   required]
+  -s, --spatial_sorting [hilbert|morton|geohash]
+                                  Spatial sorting method when perfoming
+                                  spatial partitioning.  [default: hilbert]
+  -crs, --cut_crs INTEGER         Set the coordinate reference system (CRS)
+                                  used for cutting large polygons (see `--cur-
+                                  threshold`). Defaults to the same CRS as the
+                                  input. Should be a valid EPSG code.
+  -c, --cut_threshold INTEGER     Cutting up large polygons into smaller
+                                  pieces based on a target length. Units are
+                                  assumed to match the input CRS units unless
+                                  the `--cut_crs` is also given, in which case
+                                  units match the units of the supplied CRS.
+                                  [default: 5000; required]
   -t, --threads INTEGER           Amount of threads used for operation
                                   [default: 7]
+  -tbl, --table TEXT              Name of the table to read when using a
+                                  spatial database connection as input
+  -g, --geom_col TEXT             Column name to use when using a spatial
+                                  database connection as input  [default:
+                                  geom]
   -o, --overwrite
   --help                          Show this message and exit.
+
 ```
 
+### Example 
+
+
+
+
 ## Visualising output
 
 Output is in the Apache Parquet format, a directory with one file per partition.
 
 For a quick view of your output, you can read Apache Parquet with pandas, and then use h3-pandas and geopandas to convert this into a GeoPackage or GeoParquet for visualisation in a desktop GIS, such as QGIS. The Apache Parquet output is indexed by an ID column (which you can specify), so it should be ready for two intended use-cases:
 - Joining attribute data from the original feature-level data onto computer DGGS cells.
 - Joining other data to this output on the H3 cell ID. (The output has a column like `h3_\d{2}`, e.g. `h3_09` or `h3_12` according to the target resolution.)
@@ -101,28 +121,38 @@
 #### Code formatting
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Please run `black .` before committing.
 
 ## Example commands
+
+With a local GPKG:
+
+```bash
+vector2dggs h3 -v DEBUG -id title_no -r 12 -o ~/Downloads/nz-property-titles.gpkg ~/Downloads/nz-property-titles.parquet
+
+```
+
+With a PostgreSQL/PostGIS connection:
+
 ```bash
-vector2dggs h3 -id title_no -r 12 -o ~/Downloads/nz-property-titles.gpkg ~/Downloads/nz-property-titles.parquet
+vector2dggs h3 -v DEBUG -id ogc_fid -r 9 -p 5 -t 4 --overwrite -tbl topo50_lake postgresql://user:password@host:port/db ./topo50_lake.parquet
 ```
 
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.1.0},
+  version={0.2.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.1.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs 
+> Ardo, J., & Law, R. (2023). vector2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.1.0/pyproject.toml` & `vector2dggs-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.1.0"
+version = "0.2.0"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
@@ -23,14 +23,16 @@
 dask = "^2023.3.0"
 click = "^8.1.3"
 tqdm = "^4.65.0"
 click-log = "^0.4.0"
 pyarrow = "^11.0.0"
 pygeos = "^0.14"
 pyproj = "^3.5.0"
+sqlalchemy = "^2.0.10"
+psycopg2 = "^2.9.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "*"
 
 [tool.poetry.scripts]
 vector2dggs = "vector2dggs.cli:main"
```

### Comparing `vector2dggs-0.1.0/vector2dggs/cli.py` & `vector2dggs-0.2.0/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.1.0/vector2dggs/h3.py` & `vector2dggs-0.2.0/vector2dggs/h3.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import dask.dataframe as dd
 import dask_geopandas as dgpd
 import geopandas as gpd
 import h3pandas
 import pandas as pd
 import pyproj
 from shapely.geometry import GeometryCollection
+import sqlalchemy
 from tqdm import tqdm
 from tqdm.dask import TqdmCallback
 
 from . import katana
 
 LOGGER = logging.getLogger(__name__)
 click_log.basic_config(LOGGER)
@@ -62,39 +63,55 @@
     return polyfill(*args)
 
 
 def _index(
     input_file: Union[Path, str],
     output_directory: Union[Path, str],
     resolution: int,
-    all_attributes: bool,
+    keep_attributes: bool,
     npartitions: int,
     spatial_sorting: str,
     cut_threshold: int,
     processes: int,
     id_field: str = None,
     cut_crs: pyproj.CRS = None,
+    con: Union[sqlalchemy.engine.Connection, sqlalchemy.engine.Engine] = None,
+    table: str = None,
+    geom_col: str = "geom",
 ) -> Path:
     """
     Performs multi-threaded H3 polyfilling on (multi)polygons.
     """
 
-    df = gpd.read_file(input_file)
+    if table and con:
+        # Database connection
+        if keep_attributes:
+            q = sqlalchemy.text(f"SELECT * FROM {table}")
+        elif id_field and not keep_attributes:
+            q = sqlalchemy.text(f"SELECT {id_field}, {geom_col} FROM {table}")
+        else:
+            q = sqlalchemy.text(f"SELECT {geom_col} FROM {table}")
+        df = gpd.read_postgis(q, con.connect(), geom_col=geom_col).rename_geometry(
+            "geometry"
+        )
+    else:
+        # Read file
+        df = gpd.read_file(input_file)
 
     if cut_crs:
         df = df.to_crs(cut_crs)
     LOGGER.info("Cutting with CRS: %s", df.crs)
 
     if id_field:
         df = df.set_index(id_field)
     else:
         df = df.reset_index()
         df = df.rename(columns={"index": "fid"}).set_index("fid")
 
-    if not all_attributes:
+    if not keep_attributes:
         # Remove all attributes except the geometry
         df = df.loc[:, ["geometry"]]
 
     LOGGER.info("Watch out for ninjas! (Cutting polygons)")
     with tqdm(total=df.shape[0]) as pbar:
         for index, row in df.iterrows():
             df.loc[index, "geometry"] = GeometryCollection(
@@ -158,15 +175,15 @@
     default=None,
     type=str,
     help="Field to use as an ID; defaults to a constructed single 0...n index on the original feature order.",
     nargs=1,
 )
 @click.option(
     "-k",
-    "--keep-attributes",
+    "--keep_attributes",
     is_flag=True,
     show_default=True,
     default=False,
     help="Retain attributes in output. The default is to create an output that only includes H3 cell ID and the ID given by the -id field (or the default index ID).",
 )
 @click.option(
     "-p",
@@ -175,15 +192,15 @@
     type=int,
     default=50,
     help="The number of partitions to create. Recommendation: at least as many partitions as there are available `--threads`. Partitions are processed in parallel once they have been formed.",
     nargs=1,
 )
 @click.option(
     "-s",
-    "--spatial-sorting",
+    "--spatial_sorting",
     type=click.Choice(["hilbert", "morton", "geohash"]),
     default="hilbert",
     help="Spatial sorting method when perfoming spatial partitioning.",
 )
 @click.option(
     "-crs",
     "--cut_crs",
@@ -207,36 +224,61 @@
     "--threads",
     required=False,
     default=7,
     type=int,
     help="Amount of threads used for operation",
     nargs=1,
 )
+@click.option(
+    "-tbl",
+    "--table",
+    required=False,
+    default=None,
+    type=str,
+    help="Name of the table to read when using a spatial database connection as input",
+    nargs=1,
+)
+@click.option(
+    "-g",
+    "--geom_col",
+    required=False,
+    default="geom",
+    type=str,
+    help="Column name to use when using a spatial database connection as input",
+    nargs=1,
+)
 @click.option("-o", "--overwrite", is_flag=True)
 def h3(
     vector_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
     id_field: str,
-    all_attributes: bool,
+    keep_attributes: bool,
     partitions: int,
     spatial_sorting: str,
     cut_crs: int,
     cut_threshold: int,
     threads: int,
+    table: str,
+    geom_col: str,
     overwrite: bool,
 ):
     """
     Ingest a vector dataset and index it to the H3 DGGS.
 
     VECTOR_INPUT is the path to input vector geospatial data.
-    OUTPUT_DIRECTORY should be a directorty, not a file, as it will be the write location for an Apache Parquet data store.
+    OUTPUT_DIRECTORY should be a directory, not a file or database table, as it willinstead be the write location for an Apache Parquet data store.
     """
-    if not Path(vector_input).exists():
-        if not urlparse(vector_input).scheme:
+    con: sqlalchemy.engine.Connection = None
+    scheme: str = urlparse(vector_input).scheme
+    if scheme is not None and scheme != "file":
+        # Assume database connection
+        con = sqlalchemy.create_engine(vector_input)
+    elif not Path(vector_input).exists():
+        if not scheme:
             LOGGER.warning(
                 f"Input vector {vector_input} does not exist, and is not recognised as a remote URI"
             )
             raise FileNotFoundError(
                 errno.ENOENT, os.strerror(errno.ENOENT), vector_input
             )
         vector_input = str(vector_input)
@@ -257,15 +299,18 @@
     if cut_crs is not None:
         cut_crs = pyproj.CRS.from_user_input(cut_crs)
 
     _index(
         vector_input,
         output_directory,
         int(resolution),
-        all_attributes,
+        keep_attributes,
         partitions,
         spatial_sorting,
         cut_threshold,
         threads,
         cut_crs=cut_crs,
         id_field=id_field,
+        con=con,
+        table=table,
+        geom_col=geom_col,
     )
```

### Comparing `vector2dggs-0.1.0/vector2dggs/katana.py` & `vector2dggs-0.2.0/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.1.0/PKG-INFO` & `vector2dggs-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.1.0
+Version: 0.2.0
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -20,23 +20,27 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: dask (>=2023.3.0,<2024.0.0)
 Requires-Dist: dask-geopandas (>=0.3.0,<0.4.0)
 Requires-Dist: gdal (>=3.6.2,<4.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: h3pandas (>=0.2.3,<0.3.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pygeos (>=0.14,<0.15)
 Requires-Dist: pyproj (>=3.5.0,<4.0.0)
+Requires-Dist: sqlalchemy (>=2.0.10,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/manaakiwhenua/vector2dggs
 Description-Content-Type: text/markdown
 
 # vector2dggs
 
+[![pypi](https://img.shields.io/pypi/v/vector2dggs?label=vector2dggs)](https://pypi.org/project/vector2dggs/)
+
 Python-based CLI tool to index raster files to DGGS in parallel, writing out to Parquet.
 
 This is the vector equivalent of [raster2dggs](https://github.com/manaakiwhenua/raster2dggs).
 
 Currently only supports H3 DGGS, and probably has other limitations since it has been developed for a specific internal use case, though it is intended as a general-purpose abstraction. Contributions, suggestions, bug reports and strongly worded letters are all welcome.
 
 Currently only supports polygons.
@@ -47,48 +51,66 @@
 
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
 
-  VECTOR_INPUT is the path to input vector geospatial data.
-  OUTPUT_DIRECTORY should be a directorty, not a file, as it will be the
-  write location for an Apache Parquet data store.
+  VECTOR_INPUT is the path to input vector geospatial data. OUTPUT_DIRECTORY
+  should be a directory, not a file, as it will be the write location for an
+  Apache Parquet data store.
 
 Options:
-  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO
-                                  or DEBUG  [default: INFO]
+  -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
+                                  DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
-  -a, --all_attributes            Retain attributes in output. The
-                                  default is to create an output that
-                                  only includes H3 cell ID and the ID(s)
-                                  given by the -id field (or the default
-                                  index ID).
-  -p, --partitions INTEGER        Geo-partitioning, currently only
-                                  available in Hilbert method  [default:
-                                  50; required]
-  -s, --spatial-sorting [hilbert|morton|geohash]
-                                  Spatial sorting method  [default:
-                                  hilbert]
-  -crs, --cut_crs INTEGER         Set crs(epsg) to input layer (used for
-                                  cutting), defaults to input crs
-  -c, --cut_threshold INTEGER     Cutting up large polygons into target
-                                  length (meters)  [default: 5000;
+  -k, --keep_attributes           Retain attributes in output. The default is
+                                  to create an output that only includes H3
+                                  cell ID and the ID given by the -id field
+                                  (or the default index ID).
+  -p, --partitions INTEGER        The number of partitions to create.
+                                  Recommendation: at least as many partitions
+                                  as there are available `--threads`.
+                                  Partitions are processed in parallel once
+                                  they have been formed.  [default: 50;
                                   required]
+  -s, --spatial_sorting [hilbert|morton|geohash]
+                                  Spatial sorting method when perfoming
+                                  spatial partitioning.  [default: hilbert]
+  -crs, --cut_crs INTEGER         Set the coordinate reference system (CRS)
+                                  used for cutting large polygons (see `--cur-
+                                  threshold`). Defaults to the same CRS as the
+                                  input. Should be a valid EPSG code.
+  -c, --cut_threshold INTEGER     Cutting up large polygons into smaller
+                                  pieces based on a target length. Units are
+                                  assumed to match the input CRS units unless
+                                  the `--cut_crs` is also given, in which case
+                                  units match the units of the supplied CRS.
+                                  [default: 5000; required]
   -t, --threads INTEGER           Amount of threads used for operation
                                   [default: 7]
+  -tbl, --table TEXT              Name of the table to read when using a
+                                  spatial database connection as input
+  -g, --geom_col TEXT             Column name to use when using a spatial
+                                  database connection as input  [default:
+                                  geom]
   -o, --overwrite
   --help                          Show this message and exit.
+
 ```
 
+### Example 
+
+
+
+
 ## Visualising output
 
 Output is in the Apache Parquet format, a directory with one file per partition.
 
 For a quick view of your output, you can read Apache Parquet with pandas, and then use h3-pandas and geopandas to convert this into a GeoPackage or GeoParquet for visualisation in a desktop GIS, such as QGIS. The Apache Parquet output is indexed by an ID column (which you can specify), so it should be ready for two intended use-cases:
 - Joining attribute data from the original feature-level data onto computer DGGS cells.
 - Joining other data to this output on the H3 cell ID. (The output has a column like `h3_\d{2}`, e.g. `h3_09` or `h3_12` according to the target resolution.)
@@ -134,29 +156,39 @@
 #### Code formatting
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Please run `black .` before committing.
 
 ## Example commands
+
+With a local GPKG:
+
+```bash
+vector2dggs h3 -v DEBUG -id title_no -r 12 -o ~/Downloads/nz-property-titles.gpkg ~/Downloads/nz-property-titles.parquet
+
+```
+
+With a PostgreSQL/PostGIS connection:
+
 ```bash
-vector2dggs h3 -id title_no -r 12 -o ~/Downloads/nz-property-titles.gpkg ~/Downloads/nz-property-titles.parquet
+vector2dggs h3 -v DEBUG -id ogc_fid -r 9 -p 5 -t 4 --overwrite -tbl topo50_lake postgresql://user:password@host:port/db ./topo50_lake.parquet
 ```
 
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.1.0},
+  version={0.2.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.1.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs 
+> Ardo, J., & Law, R. (2023). vector2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

