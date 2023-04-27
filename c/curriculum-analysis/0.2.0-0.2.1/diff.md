# Comparing `tmp/curriculum_analysis-0.2.0.tar.gz` & `tmp/curriculum_analysis-0.2.1.tar.gz`

## Comparing `curriculum_analysis-0.2.0.tar` & `curriculum_analysis-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/js_exporter.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/data.js
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/index.html
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/index.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/module.html
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/module.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/curriculum_analysis/html/style.css
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/LICENCE
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/js_exporter.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/data.js
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/module.html
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/module.js
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/curriculum_analysis/html/style.css
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/LICENCE
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.1/PKG-INFO
```

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/analysis.py` & `curriculum_analysis-0.2.1/curriculum_analysis/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from collections import defaultdict
+import logging
 
 from .corpus import Corpus
 
+log = logging.getLogger(__name__)
 
 class Analysis:
     def __init__(self, obj):
+        self.name = str(obj)
         self.corpora = {section: Corpus(section, text) for section, text in obj.corpora().items()}
         self.results = {}
         self.summary = defaultdict(int)
 
     def analyse(self, keywords, **kwargs):
         for kw in keywords:
             result = self.check_for_keyword(kw, **kwargs)
             self.results[kw] = result
             for section in result:
                 self.summary[kw] += len(result[section])
+        if sum(self.summary.values()):
+            log.debug(f"found '{sum(self.summary.values())}' keywords in {self.name}")
 
     def check_for_keyword(self, keyword, **kwargs):
         return {
             section: c.delemmatized_concordance_list(keyword, **kwargs) 
             for section, c in self.corpora.items()
         }
```

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/corpus.py` & `curriculum_analysis-0.2.1/curriculum_analysis/corpus.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.2.1/curriculum_analysis/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/js_exporter.py` & `curriculum_analysis-0.2.1/curriculum_analysis/js_exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
 from pathlib import Path
 from distutils.dir_util import copy_tree
+import logging
 
 from .analysis import Analysis
 
+log = logging.getLogger(__name__)
+
 class JSExporter:
     def __init__(self, file, output_path):
         self.file = file
         self.output_path = output_path
         self.output_path.mkdir(exist_ok=True)
         self.code_header = f"{self.file.type} code"
         self.name_header = f"{self.file.type} full title"
@@ -28,10 +31,11 @@
             result.append(record)
         json_string = json.dumps(result)
         js_string = f"""
         async function loadJSON() {{ 
             return {json_string}; 
         }}
         """
+        log.info(f"exporting results as HTML to {self.output_path.absolute()}")
         copy_tree(str(Path(__file__).parent / 'html'), str(self.output_path), update=True)
         with self.data_path.open('w') as data_script:
             data_script.write(js_string)
```

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.2.1/curriculum_analysis/json_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/main.py` & `curriculum_analysis-0.2.1/curriculum_analysis/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 """This is the main command line interface"""
 
 from configparser import ConfigParser
 from pathlib import Path
 from argparse import ArgumentParser
+import logging
 
 from .keywords import load_keywords_file
 from .txt_parser import file_factory
 from .csv_exporter import CSVExporter
 from .json_exporter import JSONExporter
 from .js_exporter import JSExporter
 
+logging.basicConfig(level="INFO")
+
 exporters = {
     'csv': CSVExporter,
     'json': JSONExporter,    
     'js': JSExporter,    
 }
 
 def main(filename, conf):
     # check the provided config file exists
     conf_path = Path(conf).expanduser()
+    conf_path.parent.mkdir(exist_ok=True)
     if not conf_path.exists():
         print(f"Wait! We are missing the configuration file at {conf_path}")
         default = (Path(__file__).parent / 'config.cfg.default').read_text()
         conf_path.write_text(default);
         print(f"We added this configuration to the file for you.\n")
         print(default)
         print(f"For now, we are aborting.")
         print(f"Please check/edit the configuration before running again.")
         exit()
 
     # load the config file
     config = ConfigParser()
+
     config.read(conf_path)
 
     # Load keywords
     keyword_path = Path(config.get("curriculumAnalysis", "keywords_path")).expanduser()
     if not keyword_path.exists():
         default = (Path(__file__).parent / 'keywords.txt').read_text()
         keyword_path.write_text(default);
-        
     keywords = load_keywords_file(keyword_path)
 
     # load the data
     file = file_factory(Path(filename).expanduser())
 
     # Generate an analysis
     outpath = Path(config.get("curriculumAnalysis", "outpath")).expanduser()
```

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.2.1/curriculum_analysis/txt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,23 @@
         chunks[0] = ['deleteme', '', *chunks[0]]
         chunks = [ch[1:] for ch in chunks][:-1]
         for chunk in chunks:
             yield chunk
 
 
 def file_factory(path):
+    log.info(f"Inspecting file: {path.absolute()}")
     with path.open('r', encoding='utf8') as f:
         header = f.readlines()[2].strip()
     assert header in ["Module Specification", "Programme Specification"]
     if header == "Module Specification":
-        log.info("detected module file")
+        log.info("Looks like a list of modules")
         return ModuleFile(path)
     else:
-        log.info("detected programme file")
+        log.info("Looks like a list of programmes")
         return ProgrammeFile(path)
 
 
 
 def aggregate_until(data, end_item):
     result = []
     while True:
```

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/html/index.html` & `curriculum_analysis-0.2.1/curriculum_analysis/html/index.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/html/index.js` & `curriculum_analysis-0.2.1/curriculum_analysis/html/index.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/html/module.html` & `curriculum_analysis-0.2.1/curriculum_analysis/html/module.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/html/module.js` & `curriculum_analysis-0.2.1/curriculum_analysis/html/module.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/curriculum_analysis/html/style.css` & `curriculum_analysis-0.2.1/curriculum_analysis/html/style.css`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/LICENCE` & `curriculum_analysis-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/README.md` & `curriculum_analysis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.0/pyproject.toml` & `curriculum_analysis-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "curriculum_analysis/config.cfg.default",
   "curriculum_analysis/html/*",
+  "curriculum_analysis/keywords.txt",
   "**/*.py",  
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
   { name="Tom Harrison" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `curriculum_analysis-0.2.0/PKG-INFO` & `curriculum_analysis-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

