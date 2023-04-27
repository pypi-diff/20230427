# Comparing `tmp/fw_gdrive-0.3.2-py3-none-any.whl.zip` & `tmp/fw_gdrive-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9381 bytes, number of entries: 7
+Zip file size: 9280 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      316 b- defN 80-Jan-01 00:00 fw_gdrive/__init__.py
--rw-r--r--  2.0 unx    17796 b- defN 80-Jan-01 00:00 fw_gdrive/gapi.py
+-rw-r--r--  2.0 unx    17236 b- defN 80-Jan-01 00:00 fw_gdrive/gapi.py
 -rw-r--r--  2.0 unx     6569 b- defN 80-Jan-01 00:00 fw_gdrive/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3223 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.2.dist-info/RECORD
-7 files, 29599 bytes uncompressed, 8455 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3223 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gdrive-0.3.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 fw_gdrive-0.3.3.dist-info/RECORD
+7 files, 29039 bytes uncompressed, 8354 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: fw_gdrive/gapi.py
 Comment: 
 
 Filename: fw_gdrive/utils.py
 Comment: 
 
-Filename: fw_gdrive-0.3.2.dist-info/LICENSE
+Filename: fw_gdrive-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gdrive-0.3.2.dist-info/METADATA
+Filename: fw_gdrive-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: fw_gdrive-0.3.2.dist-info/WHEEL
+Filename: fw_gdrive-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gdrive-0.3.2.dist-info/RECORD
+Filename: fw_gdrive-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gdrive/gapi.py

```diff
@@ -350,103 +350,92 @@
                 raise RuntimeError("Uncaught Exception.") from exc
             else:
                 uploaded = True
                 file_id = file.get("id")
                 return GoogleDocsFile(file_id, self.api_client.doc_service)
         return None
 
-    def get_file_list_from_folder(self, sub_folder_id: str = None) -> t.List[t.Dict]:
-        """Retrieve a list of file object that is stored in the Google Drive Folder."""
-        file_list = list()
+    def list_folders_in_drive(self) -> t.List[t.Dict]:
+        """Retrieve folders in specified folder"""
+        folders_list = list()
         # Access the files in folder
-        if not sub_folder_id:
-            # find files in the base level of the shared drive folder if not provided
-            sub_folder_id = self.folder_id
-        query = f"'{sub_folder_id}' in parents and mimeType = 'application/vnd.google-apps.file'"
-
-        try:
-            response = (
-                self.folder_cred.files()
-                .list(
-                    q=query,
-                    corpora="drive",
-                    driveId=self.folder_id,
-                    includeItemsFromAllDrives=True,
-                    supportsAllDrives=True,
-                )
-                .execute()
-            )
-
-            file_list = response.get("files")
-            nextPageToken = response.get("nextPageToken")
+        query = (
+            f"'{self.folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder' and trashed "
+            f"= false "
+        )
+        page_token = None
 
-            while nextPageToken:
+        while True:
+            try:
                 response = (
                     self.folder_cred.files()
                     .list(
                         q=query,
-                        corpora="drive",
-                        driveId=self.folder_id,
                         includeItemsFromAllDrives=True,
                         supportsAllDrives=True,
+                        fields="nextPageToken, "
+                        "files(id, name, mimeType, driveId, teamDriveId)",
+                        pageToken=page_token,
                     )
                     .execute()
                 )
-                file_list.extend(response.get("files"))
-                nextPageToken = response.get("nextPageToken")
-        except HttpError as e:
-            reason = str(e._get_reason).split('"')[-2]
-            raise RuntimeError(f"Error occurred. Reason: {reason}")
-        except Exception as exc:
-            raise Exception("Uncaught Exception.") from exc
+                folders_list.extend(response.get("files", []))
+                page_token = response.get("nextPageToken", None)
+                if page_token is None:
+                    break
+            except HttpError as e:
+                reason = str(e._get_reason).split('"')[-2]
+                raise RuntimeError(f"Error occurred. Reason: {reason}")
+            except Exception as exc:
+                raise Exception("Uncaught Exception.") from exc
 
-        return file_list
+        return folders_list
 
-    def list_folders_in_folder(self, sub_folder_id: str = None):
-        folders_list = list()
+    def list_files_in_folder(self) -> t.List[t.Dict]:
+        """Retrieve all files stored under specified folder"""
+        file_list = list()
         # Access the files in folder
-        if not sub_folder_id:
-            # find files in original shared drive or shared folder if not provided
-            sub_folder_id = self.folder_id
-
-        query = f"'{sub_folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder'"
+        query = (
+            f"'{self.folder_id}' in parents  and mimeType = 'application/vnd.google-apps.document' and trashed = "
+            f"false "
+        )
 
         page_token = None
-
         while True:
             try:
                 response = (
                     self.folder_cred.files()
                     .list(
                         q=query,
-                        corpora="drive",
-                        driveId=self.folder_id,
                         includeItemsFromAllDrives=True,
                         supportsAllDrives=True,
-                        fields="nextPageToken, " "files(id, name, mimeType)",
+                        fields="nextPageToken, "
+                        "files(id, name, mimeType, driveId, teamDriveId)",
                         pageToken=page_token,
                     )
                     .execute()
                 )
-                folders_list.extend(response.get("files", []))
+
+                file_list.extend(response.get("files", []))
                 page_token = response.get("nextPageToken", None)
                 if page_token is None:
                     break
+
             except HttpError as e:
                 reason = str(e._get_reason).split('"')[-2]
                 raise RuntimeError(f"Error occurred. Reason: {reason}")
             except Exception as exc:
                 raise Exception("Uncaught Exception.") from exc
 
-        return folders_list
+        return file_list
 
-    def get_file_id_by_name(self, file_name: str, sub_folder_id: str = None) -> list:
+    def get_file_id_by_name(self, file_name: str) -> list:
         """Retrieve file ID based on provided file name."""
         # if sub_folder_id not provided it will look at the base level of the shared drive/folder (self.folder_id)
-        file_list = self.get_file_list_from_folder(sub_folder_id)
+        file_list = self.list_files_in_folder()
         f_ids = list()
         for file in file_list:
             if file.get("name") == file_name:
                 f_id = file.get("id")
                 f_ids.append(f_id)
         return f_ids
```

## Comparing `fw_gdrive-0.3.2.dist-info/LICENSE` & `fw_gdrive-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gdrive-0.3.2.dist-info/METADATA` & `fw_gdrive-0.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-gdrive
-Version: 0.3.2
+Version: 0.3.3
 Summary: Flyweheel Google Drive Integration Tools
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-gdrive
 License: MIT
 Keywords: Flywheel
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.7,<4.0
```

