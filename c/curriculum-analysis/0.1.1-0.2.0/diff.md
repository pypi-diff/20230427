# Comparing `tmp/curriculum_analysis-0.1.1.tar.gz` & `tmp/curriculum_analysis-0.2.0.tar.gz`

## Comparing `curriculum_analysis-0.1.1.tar` & `curriculum_analysis-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/index.html
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/index.js
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/curriculum_analysis/html/style.css
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/LICENCE
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 curriculum_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/js_exporter.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/data.js
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/module.html
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/module.js
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/style.css
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/LICENCE
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/PKG-INFO
```

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/analysis.py` & `curriculum_analysis-0.2.0/curriculum_analysis/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,8 +16,11 @@
             for section in result:
                 self.summary[kw] += len(result[section])
 
     def check_for_keyword(self, keyword, **kwargs):
         return {
             section: c.delemmatized_concordance_list(keyword, **kwargs) 
             for section, c in self.corpora.items()
-        }
+        }
+    
+    def raw(self):
+        return {section: self.corpora[section].raw_string for section in self.corpora.keys()}
```

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/corpus.py` & `curriculum_analysis-0.2.0/curriculum_analysis/corpus.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.2.0/curriculum_analysis/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.2.0/curriculum_analysis/json_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/main.py` & `curriculum_analysis-0.2.0/curriculum_analysis/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from pathlib import Path
 from argparse import ArgumentParser
 
 from .keywords import load_keywords_file
 from .txt_parser import file_factory
 from .csv_exporter import CSVExporter
 from .json_exporter import JSONExporter
+from .js_exporter import JSExporter
 
 exporters = {
     'csv': CSVExporter,
     'json': JSONExporter,    
+    'js': JSExporter,    
 }
 
 def main(filename, conf):
     # check the provided config file exists
     conf_path = Path(conf).expanduser()
     if not conf_path.exists():
         print(f"Wait! We are missing the configuration file at {conf_path}")
```

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.2.0/curriculum_analysis/txt_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Details of the structure of txt files, extract data into objects with properties"""
+import logging
+
+log = logging.getLogger(__name__)
 
 def extractData(path, split_string):
     with path.open('r', encoding='utf8') as f:
         data = f.read()
         chunks = data.split(split_string)
         chunks = [ch.splitlines() for ch in chunks]
         # chunks = [[line.strip() for line in ch if line.strip()] for ch in chunks]
@@ -13,16 +16,18 @@
 
 
 def file_factory(path):
     with path.open('r', encoding='utf8') as f:
         header = f.readlines()[2].strip()
     assert header in ["Module Specification", "Programme Specification"]
     if header == "Module Specification":
+        log.info("detected module file")
         return ModuleFile(path)
     else:
+        log.info("detected programme file")
         return ProgrammeFile(path)
 
 
 
 def aggregate_until(data, end_item):
     result = []
     while True:
@@ -92,15 +97,17 @@
         data = data[12:]
         assert data[0].strip() == 'Module Details (across all module groups):'
 
         keys = data[1].split('\t')
         data = data[2:]
         values = aggregate_until(data, 'Any programme-specific differences or regulations:')
         self.modules = [{k: v for k, v in zip(keys, v.split('\t'))} for v in values]
-        assert data == ['Any programme-specific differences or regulations:', '', '']
+        # assert data == ['Any programme-specific differences or regulations:', '', '']
+        assert data[0].strip() == 'Any programme-specific differences or regulations:'
+        self.differences = [dif for dif in data[1:] if dif]
 
     def __str__(self):
         return f"Programme({self.code})"
 
     def corpora(self):
         return {
             "description": self.description,
@@ -195,15 +202,16 @@
 
     def corpora(self):
         """
         This method should return the main corpus for this module.
         Make adjustments here to control what we actually analyse.
         """
         return {
-            "description": self.description
+            "description": self.description,
+            "learning_outcomes": self.learning_outcomes
         }
 
     def __str__(self):
         return f"Module({self.code})"
 
 
 class DataFile:
```

### Comparing `curriculum_analysis-0.1.1/curriculum_analysis/html/index.html` & `curriculum_analysis-0.2.0/curriculum_analysis/html/module.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-<!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Document</title>
-    <link rel="stylesheet" href="style.css">
-    <script src="index.js" type="module"></script>
-</head>
-<body>
-    <header>
-        <h1>Curriculum Analysis</h1>
-    </header>
-    <main>
-        <table id="target">
-            <tr>
-                <th id="code_header">Code</th>
-                <th id="title_header">Title</th>
-            </tr>
-        </table>
-    </main>
-</body>
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Module</title>
+    <link rel="stylesheet" href="style.css">
+</head>
+<body>
+    <header>
+        <div>
+            <h1 id="itemCode">Module</h1>
+            <p id="itemName"></p>
+        </div>
+        <a href="index.html">Back</a>
+    </header>
+    <main id="target"></main>
+    <script src="data.js"></script>
+    <script src="module.js"></script>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,4 @@
 
 
-****** Curriculum Analysis ******
-
-Code Title
+****** Module ******
+Back
```

### Comparing `curriculum_analysis-0.1.1/LICENCE` & `curriculum_analysis-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.1.1/README.md` & `curriculum_analysis-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 keywords_path = ~/.curriculumAnalysis/keywords.txt
 outpath = ~/.curriculumAnalysis/output
 format = json
 ```
 
 Changing these values will influence the default settings.
 
-# Example usage
+## Example usage
 
 ```
 curriculum-analysis modules.txt
 ```
```

### Comparing `curriculum_analysis-0.1.1/pyproject.toml` & `curriculum_analysis-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "curriculum_analysis/config.cfg.default",
   "curriculum_analysis/html/*",
   "**/*.py",  
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
   { name="Tom Harrison" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `curriculum_analysis-0.1.1/PKG-INFO` & `curriculum_analysis-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
@@ -44,13 +44,13 @@
 keywords_path = ~/.curriculumAnalysis/keywords.txt
 outpath = ~/.curriculumAnalysis/output
 format = json
 ```
 
 Changing these values will influence the default settings.
 
-# Example usage
+## Example usage
 
 ```
 curriculum-analysis modules.txt
 ```
```

