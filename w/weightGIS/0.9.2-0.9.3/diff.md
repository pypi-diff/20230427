# Comparing `tmp/weightGIS-0.9.2-py3-none-any.whl.zip` & `tmp/weightGIS-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 37553 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat    24281 b- defN 21-Feb-25 09:24 weightGIS/FormatExternal.py
+Zip file size: 37885 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat    25639 b- defN 21-Feb-26 16:09 weightGIS/FormatExternal.py
 -rw-rw-rw-  2.0 fat     4370 b- defN 21-Jan-11 12:24 weightGIS/GeoLookup.py
--rw-rw-rw-  2.0 fat    19512 b- defN 21-Feb-24 17:37 weightGIS/PlaceReference.py
+-rw-rw-rw-  2.0 fat    19517 b- defN 21-Feb-25 13:18 weightGIS/PlaceReference.py
 -rw-rw-rw-  2.0 fat      727 b- defN 21-Feb-24 14:39 weightGIS/__init__.py
 -rw-rw-rw-  2.0 fat     8635 b- defN 21-Feb-24 17:14 weightGIS/weighting/AdjustWeights.py
 -rw-rw-rw-  2.0 fat    11380 b- defN 21-Feb-23 09:25 weightGIS/weighting/AssignWeights.py
 -rw-rw-rw-  2.0 fat    22985 b- defN 21-Feb-23 09:25 weightGIS/weighting/ConstructWeights.py
 -rw-rw-rw-  2.0 fat    15630 b- defN 21-Feb-24 10:13 weightGIS/weighting/WeightExternal.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Jan-11 14:02 weightGIS/weighting/__init__.py
 -rw-rw-rw-  2.0 fat    11303 b- defN 21-Jan-15 11:38 weightGIS/weighting/Access/SQLParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Jan-11 14:01 weightGIS/weighting/Access/__init__.py
--rw-rw-rw-  2.0 fat     1509 b- defN 21-Jan-11 14:43 weightGIS/weighting/Access/access_weighted.py
--rw-rw-rw-  2.0 fat     1090 b- defN 21-Feb-25 09:24 weightGIS-0.9.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1059 b- defN 21-Feb-25 09:24 weightGIS-0.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 21-Feb-25 09:24 weightGIS-0.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 21-Feb-25 09:24 weightGIS-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1477 b- defN 21-Feb-25 09:24 weightGIS-0.9.2.dist-info/RECORD
-17 files, 124065 bytes uncompressed, 35105 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1489 b- defN 21-Feb-26 14:40 weightGIS/weighting/Access/access_weighted.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 21-Feb-26 16:12 weightGIS-0.9.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1059 b- defN 21-Feb-26 16:12 weightGIS-0.9.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 21-Feb-26 16:12 weightGIS-0.9.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 21-Feb-26 16:12 weightGIS-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1477 b- defN 21-Feb-26 16:12 weightGIS-0.9.3.dist-info/RECORD
+17 files, 125408 bytes uncompressed, 35437 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: weightGIS/weighting/Access/__init__.py
 Comment: 
 
 Filename: weightGIS/weighting/Access/access_weighted.py
 Comment: 
 
-Filename: weightGIS-0.9.2.dist-info/LICENSE
+Filename: weightGIS-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: weightGIS-0.9.2.dist-info/METADATA
+Filename: weightGIS-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: weightGIS-0.9.2.dist-info/WHEEL
+Filename: weightGIS-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: weightGIS-0.9.2.dist-info/top_level.txt
+Filename: weightGIS-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: weightGIS-0.9.2.dist-info/RECORD
+Filename: weightGIS-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## weightGIS/FormatExternal.py

```diff
@@ -16,15 +16,15 @@
         # The name for this particular sub set of data
         self._data_name = data_name
 
         # Number of cores to use for multi-core enabled methods
         self._cpu_cores = cpu_cores
 
         # Match lists to standardise names to, set the number of match types, -1 is from removing GID
-        self._matcher, self._reference_types = self._construct_match_list()
+        self._matcher, self._reference_types, self.isolates = self._construct_match_list()
         self._match_types = len(self._matcher[0]) - 1
 
         # If there is a correction file, validate it exists, then load it; else None.
         if correction_path:
             self._corrections = self._set_corrections(correction_path)
         else:
             self._corrections = None
@@ -48,28 +48,31 @@
 
         :return: A list of lists, where sub lists contain the gid of the place, and then sub lists of strings for each
             place type
         """
 
         # Isolate the place types within the reference file
         reference_types = [header for header in self._reference.headers
-                           if "GID" not in header and not self.has_numbers(header)]
+                           if "GID" not in header and not self._has_numbers(header)]
 
         # Set the indexes for each area
         type_indexes = [[index for index, header in enumerate(self._reference.headers) if area in header]
                         for area in reference_types]
 
+        # Construct validation lookup
         validation = []
         for place in self._reference.row_data:
             validation.append([place[0]] + [self._place_type_names(place, place_type) for place_type in type_indexes])
 
-        return validation, ["GID"] + reference_types
+        # Isolate the min values for each category
+        isolates = [self._reference.headers.index("GID")] + [min(i) for i in type_indexes]
+        return validation, ["GID"] + reference_types, isolates
 
     @staticmethod
-    def has_numbers(string):
+    def _has_numbers(string):
         """
         Check to see if the string as a digit within it
 
         Source: https://stackoverflow.com/questions/19859282/check-if-a-string-contains-a-number
         """
         return any(char.isdigit() for char in string)
 
@@ -514,7 +517,34 @@
         dict and set the mater database to contain an entry equal to the name.
         """
         try:
             return [attr for attr in master_database[assign_name]]
         except KeyError:
             master_database[assign_name] = {}
             return []
+
+    def places_into_dates(self, cleaned_data, write_directory, file_gid=0):
+        """
+        Sometimes you may have data that is not missing in dates, but just wasn't recorded. This places every place in
+        into ever date.
+        """
+
+        # Format the reference into lower case
+        formatted = [[r.lower() for r in row] for row in self._reference.row_data]
+
+        for file in directory_iterator(cleaned_data):
+            # Load the file as a csv object
+            loaded_file = CsvObject(Path(cleaned_data, file))
+
+            # Isolate the GID: Row relation from the file
+            gid = {row[file_gid]: row for row in loaded_file.row_data}
+
+            # If the place exists in our file, use the file row, else use set to zero's
+            all_places = []
+            for row in formatted:
+                if row[file_gid] in gid:
+                    all_places.append(gid[row[file_gid]])
+                else:
+                    all_places.append([row[i] for i in self.isolates] + [0, 0, 0, 0])
+
+            write_csv(write_directory, loaded_file.file_name, loaded_file.headers, all_places)
+
```

## weightGIS/PlaceReference.py

```diff
@@ -262,15 +262,15 @@
                 if self._set_name(rec, others_name_indexes) not in relationships:
                     relationships.append(self._set_name(rec, others_name_indexes))
         return relationships
 
     @staticmethod
     def _set_name(record, indexes):
         """Set the name of a place via indexing the records of the shapefile"""
-        return "".join([rec for i, rec in enumerate(record) if i in indexes])
+        return "".join([str(rec) for i, rec in enumerate(record) if i in indexes])
 
     def write_linked_unique(self, ambiguity=True, ambiguity_file_name="SetAmbiguous.csv"):
         """
         Construct a base lookup-file to append alternative names to as well as lists of unique name files
 
         :param ambiguity: If there is ambiguity in the file system
         :type ambiguity: bool
```

## weightGIS/weighting/Access/access_weighted.py

```diff
@@ -3,31 +3,34 @@
 
 def access_weighted(data_extraction_set, data_requested, name_index=0):
     """
     This will use a set of keys provided by the user within data_requested to access and write out the data in a
     weighted manner
 
     """
+    all_dates = []
+    for place, attributes in zip(data_extraction_set.keys(), data_extraction_set.values()):
+        all_dates.append(
+            flatten([list(attributes[data].keys()) for data in data_requested if data in attributes.keys()]))
+
+    common_dates = sorted(list(set(flatten(all_dates))))
+
     row_data = []
     for place, attributes in zip(data_extraction_set.keys(), data_extraction_set.values()):
 
         # Whilst the first element is likely an ID, we may want to extract another index instead
         place = place.split("__")[name_index]
 
-        # Not all places will have the same dates, so we need to get a common sorted list of them
-        common_dates = sorted(list(set(flatten([attributes[data]["Dates"] for data in data_requested
-                                                if data in attributes.keys()]))))
-
         # Then for each date we setup our first two columns of place-date
         for date in common_dates:
             date_values = [place, date]
 
             # And for each attribute requested, we extract the value if the date is valid, else NA
-            for data in data_requested:
-                if (data in attributes.keys()) and (date in attributes[data]["Dates"]):
-                    date_values.append(attributes[data]["Values"][attributes[data]["Dates"].index(date)])
+            for attr in data_requested:
+                if (attr in attributes.keys()) and (date in attributes[attr].keys()):
+                    date_values.append(attributes[attr][date])
                 else:
                     date_values.append("NA")
             row_data.append(date_values)
 
     print(f"Retrieved Weighted Data {terminal_time()}")
-    return row_data
+    return row_data
```

## Comparing `weightGIS-0.9.2.dist-info/LICENSE` & `weightGIS-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `weightGIS-0.9.2.dist-info/METADATA` & `weightGIS-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightGIS
-Version: 0.9.2
+Version: 0.9.3
 Summary: Weight ESRI shapefiles attributes
 Home-page: UNKNOWN
 Author: Samuel Baker
 Author-email: samuelbaker.researcher@gmail.com
 Maintainer: Samuel Baker
 Maintainer-email: samuelbaker.researcher@gmail.com
 License: MIT
```

