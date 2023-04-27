# Comparing `tmp/plantuml_markdown-3.9.0-py3-none-any.whl.zip` & `tmp/plantuml_markdown-3.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17410 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    30751 b- defN 23-Apr-23 18:07 plantuml_markdown.py
--rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    17482 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/RECORD
-6 files, 50157 bytes uncompressed, 16474 bytes compressed:  67.2%
+Zip file size: 17557 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    31183 b- defN 23-Apr-27 05:38 plantuml_markdown.py
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    17482 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/RECORD
+6 files, 50589 bytes uncompressed, 16621 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: plantuml_markdown.py
 Comment: 
 
-Filename: plantuml_markdown-3.9.0.dist-info/LICENSE
+Filename: plantuml_markdown-3.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: plantuml_markdown-3.9.0.dist-info/METADATA
+Filename: plantuml_markdown-3.9.1.dist-info/METADATA
 Comment: 
 
-Filename: plantuml_markdown-3.9.0.dist-info/WHEEL
+Filename: plantuml_markdown-3.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: plantuml_markdown-3.9.0.dist-info/top_level.txt
+Filename: plantuml_markdown-3.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: plantuml_markdown-3.9.0.dist-info/RECORD
+Filename: plantuml_markdown-3.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plantuml_markdown.py

```diff
@@ -56,14 +56,15 @@
 """
 
 import os
 import re
 import base64
 import zlib
 import string
+import urllib3
 from subprocess import Popen, PIPE
 from typing import Dict, List, Optional, Tuple
 from zlib import adler32
 
 import logging
 import markdown
 import uuid
@@ -452,22 +453,30 @@
             # insert an include directive for the config file as the first statement
             plantuml_code = re.sub(r'^\s*(@start\w+\n)?', r'\1!include '+self._config_path+'\n', plantuml_code)
 
         # build the whole source diagram, executing include directives
         temp_file = PlantUMLIncluder(self._lang, not not self._kroki_server,
                                      self.config['server_include_whitelist'],
                                      False).readFile(plantuml_code, self._base_dir)
+        ssl_verify = not self.config['insecure']
+
+        if not ssl_verify:
+            # urllib3 gives a warning is an insecure connection is made, and the warning is included in the output page
+            # not the best solution, but it works
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+            # alternative solution
+            # requests.packages.urllib3.disable_warnings()
 
         # Use GET if preferred, use POST with GET as fallback if POST fails
         if self._http_method == "POST":
             # image_url for POST attempt first
             image_url = "%s/%s/" % (self._server, img_format)
             # download manually the image to be able to continue in case of errors
             r = session.post(image_url, data=temp_file, headers={"Content-Type": 'text/plain; charset=utf-8'},
-                             verify=not self.config['insecure'])
+                             verify=ssl_verify)
 
             if r.ok:
                 return r.content, None
 
             logger.warning(f'WARNING in "uml" directive: remote server has returned error {r.status_code} on POST')
             if self._fallback_to_get:
                 logger.warning('Falling back to GET')
@@ -475,15 +484,15 @@
                 return self._handle_response(r)
 
         if self._kroki_server:
             image_url = self._server + "/plantuml/" + img_format + "/" + self._compress_and_encode(temp_file)
         else:
             image_url = self._server+"/"+img_format+"/"+self._deflate_and_encode(temp_file)
 
-        return self._handle_response(session.get(image_url, verify=not self.config['insecure']))
+        return self._handle_response(session.get(image_url, verify=ssl_verify))
 
     def _handle_response(self, resp: Response) -> Tuple[Optional[bytes], Optional[str]]:
         if not resp.ok and self._kroki_server:
             # Kroki sends and HTTP 400 with a text description of the error
             logger.warning(f'WARNING in "uml" directive: remote server has returned error {resp.status_code} on GET: '
                            f'{resp.content.decode("utf-8")}')
             return None, resp.content.decode('utf-8')
@@ -518,15 +527,16 @@
         self._diagram_type = 'uml'
 
     # Given a PlantUML source, replace any "!include" directive with the included code, recursively
     def readFile(self, plantuml_code: str, directory: str) -> str:
         lines = plantuml_code.splitlines()
         # Wrap the whole combined text between startuml and enduml tags as recursive processing would have removed them
         # This is necessary for it to work correctly with plamtuml POST processing
-        return "@start"+self._diagram_type+"\n" + "\n".join(self._readFileRec(lines, directory)) + "\n@end"+self._diagram_type+"\n"
+        all_lines = self._readFileRec(lines, directory)
+        return "@start"+self._diagram_type+"\n" + "\n".join(all_lines) + "\n@end"+self._diagram_type+"\n"
 
     # Reads the file recursively
     def _readFileRec(self, lines: List[str], directory: str) -> List[str]:
         result: List[str] = []
 
         for line in lines:
             line_striped = line.strip()
```

## Comparing `plantuml_markdown-3.9.0.dist-info/LICENSE` & `plantuml_markdown-3.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plantuml_markdown-3.9.0.dist-info/METADATA` & `plantuml_markdown-3.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.9.0
+Version: 3.9.1
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro@email.it
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `plantuml_markdown-3.9.0.dist-info/RECORD` & `plantuml_markdown-3.9.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-plantuml_markdown.py,sha256=8CRDGh--anSjMWzZLQ4QgKh0_2YHwJCiPj0MhZtAbQI,30751
-plantuml_markdown-3.9.0.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
-plantuml_markdown-3.9.0.dist-info/METADATA,sha256=3PmFJaDFK54aTSJRBucihibvyh4PfGoyWYoFIHw_nSk,17482
-plantuml_markdown-3.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-plantuml_markdown-3.9.0.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
-plantuml_markdown-3.9.0.dist-info/RECORD,,
+plantuml_markdown.py,sha256=hZlbDH9RDvX_3dbbD_6vnz7r-bxXFXOOxinRfGA2WGk,31183
+plantuml_markdown-3.9.1.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
+plantuml_markdown-3.9.1.dist-info/METADATA,sha256=7sv4OGAqq_kg0CVxnZ27IGkb-X685Bc2npFn8CRWeMM,17482
+plantuml_markdown-3.9.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+plantuml_markdown-3.9.1.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
+plantuml_markdown-3.9.1.dist-info/RECORD,,
```

