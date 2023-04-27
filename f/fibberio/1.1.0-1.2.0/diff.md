# Comparing `tmp/fibberio-1.1.0.tar.gz` & `tmp/fibberio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibberio-1.1.0.tar", max compression
+gzip compressed data, was "fibberio-1.2.0.tar", max compression
```

## Comparing `fibberio-1.1.0.tar` & `fibberio-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      542 2023-03-23 01:55:41.100242 fibberio-1.1.0/fibberio/__init__.py
--rw-r--r--   0        0        0     1475 2023-03-16 21:21:09.835323 fibberio-1.1.0/fibberio/cli.py
--rw-r--r--   0        0        0     6401 2023-03-23 01:55:41.100242 fibberio-1.1.0/fibberio/distribution.py
--rw-r--r--   0        0        0     1306 2023-03-23 01:55:41.101245 fibberio-1.1.0/fibberio/helpers.py
--rw-r--r--   0        0        0     5273 2022-06-08 19:04:17.083401 fibberio-1.1.0/fibberio/range.py
--rw-r--r--   0        0        0      739 2023-01-20 04:17:07.962396 fibberio-1.1.0/fibberio/source.py
--rw-r--r--   0        0        0     1931 2023-03-23 01:55:41.102245 fibberio-1.1.0/fibberio/task.py
--rw-r--r--   0        0        0     1067 2022-06-07 16:53:28.112514 fibberio-1.1.0/LICENSE.md
--rw-r--r--   0        0        0      948 2023-03-23 01:55:41.103242 fibberio-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11251 2023-01-20 04:17:07.958890 fibberio-1.1.0/README.md
--rw-r--r--   0        0        0    12096 2023-03-23 02:04:05.568846 fibberio-1.1.0/setup.py
--rw-r--r--   0        0        0    11459 2023-03-23 02:04:05.568846 fibberio-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-04-27 19:29:50.283687 fibberio-1.2.0/fibberio/__init__.py
+-rw-r--r--   0        0        0     1475 2023-03-16 21:21:09.835323 fibberio-1.2.0/fibberio/cli.py
+-rw-r--r--   0        0        0     6401 2023-04-27 19:29:50.284689 fibberio-1.2.0/fibberio/distribution.py
+-rw-r--r--   0        0        0     1306 2023-04-27 19:29:50.284689 fibberio-1.2.0/fibberio/helpers.py
+-rw-r--r--   0        0        0     5273 2022-06-08 19:04:17.083401 fibberio-1.2.0/fibberio/range.py
+-rw-r--r--   0        0        0      739 2023-01-20 04:17:07.962396 fibberio-1.2.0/fibberio/source.py
+-rw-r--r--   0        0        0     1991 2023-04-27 19:29:50.285688 fibberio-1.2.0/fibberio/task.py
+-rw-r--r--   0        0        0     1067 2022-06-07 16:53:28.112514 fibberio-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0      948 2023-04-27 19:29:50.287940 fibberio-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11251 2023-01-20 04:17:07.958890 fibberio-1.2.0/README.md
+-rw-r--r--   0        0        0    12096 2023-04-27 19:30:36.712636 fibberio-1.2.0/setup.py
+-rw-r--r--   0        0        0    11459 2023-04-27 19:30:36.712636 fibberio-1.2.0/PKG-INFO
```

### Comparing `fibberio-1.1.0/fibberio/__init__.py` & `fibberio-1.2.0/fibberio/__init__.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/cli.py` & `fibberio-1.2.0/fibberio/cli.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/distribution.py` & `fibberio-1.2.0/fibberio/distribution.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/helpers.py` & `fibberio-1.2.0/fibberio/helpers.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/range.py` & `fibberio-1.2.0/fibberio/range.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/source.py` & `fibberio-1.2.0/fibberio/source.py`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/fibberio/task.py` & `fibberio-1.2.0/fibberio/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         sources = [Item.build(s, path) for s in task["sources"]]
         self.sources = {id: o for id, o in sources}
 
         # load features
         features = [Item.build(s) for s in task["features"]]
         self.features = {id: o for id, o in features}
 
+        self.validate()
+
+    def validate(self) -> None:
         # hidrate "source" features
         for k in self.features.keys():
             # set up referential integrity
             self.features[k].id = k
             if type(self.features[k]) == Source:
                 if self.features[k].src in self.sources:
                     self.features[k].source = self.sources[self.features[k].src]
```

### Comparing `fibberio-1.1.0/LICENSE.md` & `fibberio-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/pyproject.toml` & `fibberio-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fibberio"
-version = "1.1.0"
+version = "1.2.0"
 description = ""
 authors = ["sethjuarez <me@sethjuarez.com>"]
 readme = "README.md"
 homepage = "https://github.com/sethjuarez/fibberio"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fibberio-1.1.0/README.md` & `fibberio-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fibberio-1.1.0/setup.py` & `fibberio-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'parsimonious>=0.8.1,<0.9.0']
 
 entry_points = \
 {'console_scripts': ['fibber = fibberio.cli:cli']}
 
 setup_kwargs = {
     'name': 'fibberio',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': '',
     'long_description': '# fibber\n\n(This is still under development)\n\nTeaching machine learning things is hard. The idea behind this library is to generate data in such a way that certain principles can be highlighted without resorting to "finding" the perfect dataset to do so.\n\nCurrently the library can be installed using `pip`:\n\n```\npip install fibberio\n```\n\nOnce the library is installed in your python environment, you can start generating data by:\n\n```\nfibber -t .\\tests\\data\\programmers.json -o .\\sandbox\\programmers.csv -c 10000\n```\n\nwhere `-t` is the Task Description file and `-o` is the output file. To specify the record count, the `-c` flag is used. Successfully running the command should show the following:\n\n```\nGenerating 10000 items using "programmers.json"\n-----------------------------------------------\n\n       FirstName  LastName           age  style          desc accept\ncount      10000     10000  10000.000000  10000  10000.000000  10000\nunique       966      1000           NaN      2           NaN      2\ntop         Remy  Anthony            NaN   tabs           NaN  False\nfreq          29        21           NaN   6642           NaN   5378\nmean         NaN       NaN     35.985700    NaN     21.736883    NaN\nstd          NaN       NaN      4.983832    NaN     10.526532    NaN\nmin          NaN       NaN     18.000000    NaN      5.010000    NaN\n25%          NaN       NaN     33.000000    NaN     12.580000    NaN\n50%          NaN       NaN     36.000000    NaN     20.070000    NaN\n75%          NaN       NaN     39.000000    NaN     34.660000    NaN\nmax          NaN       NaN     57.000000    NaN     36.800000    NaN\n\nSaving csv to C:\\projects\\fibberio\\sandbox\\programmers.csv\nTask complete\n```\n\nThe [programmers.json](./tests/data/programmers.json) file is a good starting point for understanding task descriptions.\n\n# Task Description\n\nThe best way to understand how it works is to look at a task description:\n\n```json\n{\n    "sources": [\n        {\n            "id": "names",\n            "pandas": {\n                "path": "./full_names.csv",\n                "read_csv": {\n                    "encoding": "unicode_escape",\n                    "engine": "python"\n                }\n            }\n        }\n    ],\n    "features": [\n        {\n            "id": "first_name",\n            "source": {\n                "id": "names",\n                "target": "FirstName"\n            }\n        },\n        {\n            "id": "age",\n            "normal": {\n                "mean": 36,\n                "stddev": 5,\n                "precision": 0\n            }\n        },\n        {\n            "id": "style",\n            "discrete": {\n                "tabs": 2,\n                "spaces": 1\n            }\n        },\n    ]\n}\n```\n\nThere are two specific sections:\n\n1. **Sources** - external reference data\n2. **Features** - columns to generate\n\n## Sources\n\nThe `sources` section contains a dictionary containing references to external files with data that can be sampled later as features.\n\n```json\n{\n    "id": "names",\n    "pandas": {\n        "path": "./full_names.csv",\n        "read_csv": {\n            "encoding": "unicode_escape",\n            "engine": "python"\n        }\n    }\n}\n```\n\nThe `id` is the identifier used to reference this data source later in the features. [`read_csv`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html) in this case is the call to the pandas [`read_csv`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html) function call with the enclosed dictionary representing the `**kwargs` passed to that function. In theory, any pandas call to load any file type can be used here (although as of the time of this writing, `read_csv` is the only one that has been tried).\n\nThe `path` to the data file (in the case above [./full_names.csv](./tests/data/full_names.csv)) is *in relation to the task description file* unless the full path is specified.\n\n## Features\n\nThe `features` section contains the features the system should generate along with their corresponding distributions:\n\n```json\n"features": [\n    {\n        "id": "first_name",\n        "source": {\n            "id": "names",\n            "target": "FirstName"\n        }\n    },\n    {\n        "id": "age",\n        "normal": {\n            "mean": 36,\n            "stddev": 5,\n            "precision": 0\n        }\n    },\n    {\n        "id": "style",\n        "discrete": {\n            "tabs": 2,\n            "spaces": 1\n        }\n    }\n]\n```\n\nIn this example there are exactly three features:\n\n1. **first_name** - this references the `names` source and samples from the `FirstName` column\n2. **age** - this samples from the `normal` distribution with three parameters passed in to the `Normal` class as `**kwargs`\n3. **style** - this samples from a discrete distribution that will generate `tabs` and `spaces` in a 2 to 1 ratio\n\nThe standard definition for a feature therefore consists of:\n\n```json\n{\n    "id": "feature_id"\n    "distribution_class": {\n      [... distribution args ...]\n    }\n}\n```\n\nWhere the `feature_id` represents the id of the feature and the column name (this can be overriden in certain samplers). The `distribution_class` is the name of a `Distribution` class which is instantiated with the corresponding args.\n\nEssentially, if the Distribution class is instantiated by:\n\n```\ndistribution_class(prop1=2, prop2=seismic)\n```\n\nthen the corresponding `kwargs` should look like\n\n```\n{\n  "prop1": 2,\n  "prop2": "seismic"\n}\n```\n\nand get instantiated by\n\n```\ndistribution_class(**kwargs)\n```\n\nI am optimizing for readibility as opposed to brevity. This requires the class to have an `__init()__` with default named parameters.\n\nThe optional `conditional` part of the feature is described next.\n\n## Conditionals\n\nFeature conditionals allow for conditional sampling based on the parent distribution. Here\'s an example:\n\n```json\n"features": [\n    {\n        "id": "age",\n        "normal": {\n            "mean": 36,\n            "stddev": 5,\n            "precision": 0\n        }\n    },\n    {\n        "id": "score",\n        "conditional": {\n            "marginal": "age",\n            "posterior": [\n                {\n                    "value": "[14, 65)",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                },\n                {\n                    "value": "[65, *)",\n                    "normal": {\n                        "mean": 35,\n                        "stddev": 0.5\n                    }\n                },\n                {\n                    "value": "*",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                }\n            ]\n        }\n    }\n]\n```\n\nThis describes `score` feature conditioned on the `age` feature (as the marginal). Since the parent distribution is continuous, the conditional subdivisions should be represented by ranges:\n\n- $[a, b]$ the closed interval ${ x \\in \\mathbb{R}: a \\le x \\le b }$\n- $[a, b)$ the interval ${ x \\in \\mathbb{R}: a \\le x \\lt b }$\n- $(a, b]$ the interval ${ x \\in \\mathbb{R}: a \\lt x \\le b }$\n- $(a, b)$ the open interval ${ x \\in \\mathbb{R}: a \\lt x \\lt b }$\n\nwith `*` representing a catch within the range interval or as the "catch-all" - these are processed in order and an exception is raised if none of the criteria fit.\n\nThe task processes each top level feature and then passes the generated value to the conditional which evaluates each range and generates from the distribution which "catches" the generated top level value.\n\nThis also is true for discrete probability distributions:\n\n```json\n"features": [\n    {\n        "id": "style",\n        "discrete": {\n            "tabs": 234,\n            "spaces": 2332,\n            "agile": 21,\n            "scrum": 128\n        },\n    },\n    {\n        "id": "score",\n        "conditional": {\n            "marginal": "score",\n            "posterior": [\n                {\n                    "value": "tabs",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                },\n                {\n                    "value": "*",\n                    "normal": {\n                        "mean": 12,\n                        "stddev": 3\n                    }\n                }\n            ]\n        }\n    }\n]\n```\n\nIn this case, the conditional `score` feature will sample from the `uniform` distribution if "tabs" is generated for the `style` feature, otherwise the catch-all `*` will sample from the `normal` distribution.\n\nThese dependencies can be chained:\n\n```json\n"features": [\n    {\n        "id": "style",\n        "discrete": {\n            "tabs": 234,\n            "spaces": 2332,\n            "agile": 21,\n            "scrum": 128\n        },\n    },\n    {\n        "id": "score",\n        "conditional": {\n            "marginal": "style",\n            "posterior": [\n                {\n                    "value": "tabs",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                },\n                {\n                    "value": "*",\n                    "normal": {\n                        "mean": 12,\n                        "stddev": 3\n                    }\n                }\n            ]\n        }\n    },\n    {\n        "id": "accepted",\n        "conditional": {\n            "marginal": "score",\n            "posterior": [\n                {\n                    "value": "[14, 65)",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                },\n                {\n                    "value": "[65, *)",\n                    "normal": {\n                        "mean": 35,\n                        "stddev": 0.5\n                    }\n                },\n                {\n                    "value": "*",\n                    "uniform": {\n                        "low": 5,\n                        "high": 25,\n                        "itype": "float",\n                        "precision": 2\n                    }\n                }\n            ]\n        }\n    }\n]\n```\n\nNotice that in this case, the first conditional required discrete values while the second used ranges. An exception is raised if there is a mismatch.\n\nThe main idea is that every Feature has a `distribution` and optional dependant `conditional`\n\n\n',
     'author': 'sethjuarez',
     'author_email': 'me@sethjuarez.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sethjuarez/fibberio',
```

### Comparing `fibberio-1.1.0/PKG-INFO` & `fibberio-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibberio
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Home-page: https://github.com/sethjuarez/fibberio
 Author: sethjuarez
 Author-email: me@sethjuarez.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

