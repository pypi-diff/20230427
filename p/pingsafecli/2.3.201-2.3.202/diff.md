# Comparing `tmp/pingsafecli-2.3.201-py3-none-any.whl.zip` & `tmp/pingsafecli-2.3.202-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8544021 bytes, number of entries: 8
+Zip file size: 8544019 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 16:55 pingsafecli/__init__.py
 -rwxr-xr-x  2.0 unx 17012674 b- defN 23-Apr-26 15:50 pingsafecli/go-rego-evaluator
--rw-r--r--  2.0 unx     1624 b- defN 23-Apr-27 12:19 pingsafecli/main.py
--rwxr-xr-x  2.0 unx      541 b- defN 23-Apr-27 12:20 pingsafecli-2.3.201.data/scripts/pingsafecli
--rw-r--r--  2.0 unx      663 b- defN 23-Apr-27 12:20 pingsafecli-2.3.201.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 12:20 pingsafecli-2.3.201.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 12:20 pingsafecli-2.3.201.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      664 b- defN 23-Apr-27 12:20 pingsafecli-2.3.201.dist-info/RECORD
-8 files, 17016270 bytes uncompressed, 8542857 bytes compressed:  49.8%
+-rw-r--r--  2.0 unx     1626 b- defN 23-Apr-27 12:22 pingsafecli/main.py
+-rwxr-xr-x  2.0 unx      541 b- defN 23-Apr-27 12:23 pingsafecli-2.3.202.data/scripts/pingsafecli
+-rw-r--r--  2.0 unx      663 b- defN 23-Apr-27 12:23 pingsafecli-2.3.202.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 12:23 pingsafecli-2.3.202.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 12:23 pingsafecli-2.3.202.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      664 b- defN 23-Apr-27 12:23 pingsafecli-2.3.202.dist-info/RECORD
+8 files, 17016272 bytes uncompressed, 8542855 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pingsafecli/go-rego-evaluator
 Comment: 
 
 Filename: pingsafecli/main.py
 Comment: 
 
-Filename: pingsafecli-2.3.201.data/scripts/pingsafecli
+Filename: pingsafecli-2.3.202.data/scripts/pingsafecli
 Comment: 
 
-Filename: pingsafecli-2.3.201.dist-info/METADATA
+Filename: pingsafecli-2.3.202.dist-info/METADATA
 Comment: 
 
-Filename: pingsafecli-2.3.201.dist-info/WHEEL
+Filename: pingsafecli-2.3.202.dist-info/WHEEL
 Comment: 
 
-Filename: pingsafecli-2.3.201.dist-info/top_level.txt
+Filename: pingsafecli-2.3.202.dist-info/top_level.txt
 Comment: 
 
-Filename: pingsafecli-2.3.201.dist-info/RECORD
+Filename: pingsafecli-2.3.202.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingsafecli/main.py

```diff
@@ -8,15 +8,15 @@
 
 
 class PingSafeCli:
     def __init__(self) -> None:
         pass
     def run(self, repo_path, rego_file_path) -> None:
         print (repo_path, rego_file_path)
-        subprocess.run(["pip3 install --upgrade pingsafecli"])
+        subprocess.run(["pip3", "install", "--upgrade",  "pingsafecli"])
         terraform_runner = TerraformRunner()
         graph = terraform_runner.generate_graph(repo_path)
         input_json_dir = os.getcwd() + "/input_json/"
         if os.path.exists(input_json_dir) == False:
             os.mkdir(input_json_dir)
         try:
             for node in graph["nodes"]:
@@ -38,12 +38,12 @@
                     os.remove(file_path)
 
 
 
 
 if __name__ == '__main__':
     ckv = PingSafeCli()
-    print ("world12345")
+    print ("v1")
     sys.exit(ckv.run("a", "b"))
```

## Comparing `pingsafecli-2.3.201.data/scripts/pingsafecli` & `pingsafecli-2.3.202.data/scripts/pingsafecli`

 * *Files identical despite different names*

## Comparing `pingsafecli-2.3.201.dist-info/METADATA` & `pingsafecli-2.3.202.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingsafecli
-Version: 2.3.201
+Version: 2.3.202
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/checkov
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Requires-Python: >=3.7
```

## Comparing `pingsafecli-2.3.201.dist-info/RECORD` & `pingsafecli-2.3.202.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pingsafecli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pingsafecli/go-rego-evaluator,sha256=wBM-aEJKmEwAGNRaKc9QRcdKjfkfP3N6weLp-FhFY30,17012674
-pingsafecli/main.py,sha256=7axGj_FZfpaAgDmWrBqundL-UYTBYmpJi7xn47g7ZSI,1624
-pingsafecli-2.3.201.data/scripts/pingsafecli,sha256=2G7hEyFP78TaQLTFeyhE_yUUcWkq8AYLMWkUIp67XdM,541
-pingsafecli-2.3.201.dist-info/METADATA,sha256=b0R26cfD1qnwkZaSt41ZWP3vlRztpfrY6MxrFel6zqQ,663
-pingsafecli-2.3.201.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pingsafecli-2.3.201.dist-info/top_level.txt,sha256=jQGXsOZMG5Xz4cC5yzJshe1hA7wgKbautrUBk5s05Ok,12
-pingsafecli-2.3.201.dist-info/RECORD,,
+pingsafecli/main.py,sha256=RrzE6cbw4hrXMHKQAGGOsFthcBkCaryWNtjj9lHYSOE,1626
+pingsafecli-2.3.202.data/scripts/pingsafecli,sha256=2G7hEyFP78TaQLTFeyhE_yUUcWkq8AYLMWkUIp67XdM,541
+pingsafecli-2.3.202.dist-info/METADATA,sha256=Ohw9CJ2Xcnk9V6e0CGtZ-WohrAzlvQBV_ZXLIN2WJpE,663
+pingsafecli-2.3.202.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pingsafecli-2.3.202.dist-info/top_level.txt,sha256=jQGXsOZMG5Xz4cC5yzJshe1hA7wgKbautrUBk5s05Ok,12
+pingsafecli-2.3.202.dist-info/RECORD,,
```

