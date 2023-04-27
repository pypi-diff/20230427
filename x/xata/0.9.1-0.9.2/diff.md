# Comparing `tmp/xata-0.9.1.tar.gz` & `tmp/xata-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-0.9.1.tar", max compression
+gzip compressed data, was "xata-0.9.2.tar", max compression
```

## Comparing `xata-0.9.1.tar` & `xata-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-16 10:15:31.921430 xata-0.9.1/LICENSE
--rw-r--r--   0        0        0     1156 2023-04-16 10:15:31.921430 xata-0.9.1/README.md
--rw-r--r--   0        0        0      749 2023-04-16 10:15:31.949431 xata-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      858 2023-04-16 10:15:31.949431 xata-0.9.1/xata/__init__.py
--rw-r--r--   0        0        0    31957 2023-04-16 10:15:31.949431 xata-0.9.1/xata/client.py
--rw-r--r--   0        0        0     1715 2023-04-16 10:15:31.949431 xata-0.9.1/xata/errors.py
--rw-r--r--   0        0        0    11020 2023-04-16 10:15:31.949431 xata-0.9.1/xata/helpers.py
--rw-r--r--   0        0        0     2114 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespace.py
--rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/__init__.py
--rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/__init__.py
--rw-r--r--   0        0        0     2666 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/authentication.py
--rw-r--r--   0        0        0     6182 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/databases.py
--rw-r--r--   0        0        0     6204 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/invites.py
--rw-r--r--   0        0        0     2554 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/users.py
--rw-r--r--   0        0        0     7419 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/core/workspaces.py
--rw-r--r--   0        0        0      769 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/__init__.py
--rw-r--r--   0        0        0    12315 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/branch.py
--rw-r--r--   0        0        0    10143 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/migrations.py
--rw-r--r--   0        0        0    12491 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/records.py
--rw-r--r--   0        0        0    29615 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/search_and_filter.py
--rw-r--r--   0        0        0    12792 2023-04-16 10:15:31.949431 xata-0.9.1/xata/namespaces/workspace/table.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 12:37:44.650242 xata-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1156 2023-04-27 12:37:44.650242 xata-0.9.2/README.md
+-rw-r--r--   0        0        0      749 2023-04-27 12:37:44.678241 xata-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      858 2023-04-27 12:37:44.678241 xata-0.9.2/xata/__init__.py
+-rw-r--r--   0        0        0    31960 2023-04-27 12:37:44.678241 xata-0.9.2/xata/client.py
+-rw-r--r--   0        0        0     1715 2023-04-27 12:37:44.678241 xata-0.9.2/xata/errors.py
+-rw-r--r--   0        0        0    11090 2023-04-27 12:37:44.678241 xata-0.9.2/xata/helpers.py
+-rw-r--r--   0        0        0     2114 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespace.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/__init__.py
+-rw-r--r--   0        0        0     2666 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/authentication.py
+-rw-r--r--   0        0        0     6182 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/databases.py
+-rw-r--r--   0        0        0     6204 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/invites.py
+-rw-r--r--   0        0        0     2554 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/users.py
+-rw-r--r--   0        0        0     7419 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/workspaces.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/__init__.py
+-rw-r--r--   0        0        0    12315 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/branch.py
+-rw-r--r--   0        0        0    11721 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/migrations.py
+-rw-r--r--   0        0        0    12491 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/records.py
+-rw-r--r--   0        0        0    30137 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/search_and_filter.py
+-rw-r--r--   0        0        0    12792 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/table.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.2/PKG-INFO
```

### Comparing `xata-0.9.1/LICENSE` & `xata-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/README.md` & `xata-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/pyproject.toml` & `xata-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-0.9.1/xata/__init__.py` & `xata-0.9.2/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/client.py` & `xata-0.9.2/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .namespaces.workspace.migrations import Migrations
 from .namespaces.workspace.records import Records
 from .namespaces.workspace.search_and_filter import Search_and_filter
 from .namespaces.workspace.table import Table
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
@@ -239,15 +239,15 @@
             f"No workspace ID found. Searched in `XATA_WORKSPACE_ID` env, "
             f"`{PERSONAL_API_KEY_LOCATION}`, and `{os.path.abspath('.env')}`"
         )
 
     def get_database_name_if_configured(self) -> str:
         self.ensure_config_read()
         if self.config is not None and self.config.get("databaseURL"):
-            _, _, db_name, _ = self._parse_database_url(self.config.get("databaseURL"))
+            _, _, db_name, _, _ = self._parse_database_url(self.config.get("databaseURL"))
             return db_name
         return None
 
     def get_branch_name_if_configured(self) -> str:
         # TODO: resolve branch name by the current git branch
         return os.environ.get("XATA_BRANCH")
```

### Comparing `xata-0.9.1/xata/errors.py` & `xata-0.9.2/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/helpers.py` & `xata-0.9.2/xata/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,18 @@
                                 "response": r,
                             }
                         )
                         self.stats["failed_batches"] += 1
                         if self.throw_exception:
                             raise Exception(r.json())
 
-                    self.logger.debug("thread #%d: pushed a batch of %d records to table %s" % (id, len(batch["records"]), batch["table"]))
+                    self.logger.debug(
+                        "thread #%d: pushed a batch of %d records to table %s"
+                        % (id, len(batch["records"]), batch["table"])
+                    )
                     self.stats["total"] += len(batch["records"])
                     self.stats["queue"] = self.records.size()
                     if batch["table"] not in self.stats["tables"]:
                         self.stats["tables"][batch["table"]] = 0
                     self.stats["tables"][batch["table"]] += len(batch["records"])
                 except Exception as exc:
                     logging.error("thread #%d: %s" % (id, exc))
```

### Comparing `xata-0.9.1/xata/namespace.py` & `xata-0.9.2/xata/namespace.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/__init__.py` & `xata-0.9.2/xata/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/__init__.py` & `xata-0.9.2/xata/namespaces/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/authentication.py` & `xata-0.9.2/xata/namespaces/core/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/databases.py` & `xata-0.9.2/xata/namespaces/core/databases.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/invites.py` & `xata-0.9.2/xata/namespaces/core/invites.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/users.py` & `xata-0.9.2/xata/namespaces/core/users.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/core/workspaces.py` & `xata-0.9.2/xata/namespaces/core/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/workspace/__init__.py` & `xata-0.9.2/xata/namespaces/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/workspace/branch.py` & `xata-0.9.2/xata/namespaces/workspace/branch.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/workspace/migrations.py` & `xata-0.9.2/xata/namespaces/workspace/migrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,7 +246,37 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/schema/apply"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
+
+    def pushBranchMigrations(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
+        """
+        The `schema/push` API accepts a list of migrations to be applied to the current branch.  A
+        list of applicable migrations can be fetched using the `schema/history` API from another
+        branch or database.  The most recent migration must be part of the list or referenced (via
+        `parentID`) by the first migration in the list of migrations to be pushed.  Each migration
+        in the list has an `id`, `parentID`, and `checksum`. The checksum for migrations are
+        generated and verified by xata.  The operation fails if any migration in the list has an
+        invalid checksum.
+
+        Path: /db/{db_branch_name}/schema/push
+        Method: POST
+        Response status codes:
+        - 200: Schema migration response with ID and migration status.
+        - 400: Bad Request
+        - 401: Authentication Error
+        - 404: Example response
+        - 5XX: Unexpected Error
+
+        :param payload: dict content
+        :param db_name: str = None The name of the database to query. Default: database name from the client.
+        :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
+
+        :return Response
+        """
+        db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
+        url_path = f"/db/{db_branch_name}/schema/push"
+        headers = {"content-type": "application/json"}
+        return self.request("POST", url_path, headers, payload)
```

### Comparing `xata-0.9.1/xata/namespaces/workspace/records.py` & `xata-0.9.2/xata/namespaces/workspace/records.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/xata/namespaces/workspace/search_and_filter.py` & `xata-0.9.2/xata/namespaces/workspace/search_and_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,22 +154,17 @@
         "createdAt": "desc"     }   ] } ```  It is also possible to sort results randomly:
         ```json POST /db/demo:main/tables/table/query {   "sort": {     "*": "random"   } } ```
         Note that a random sort does not apply to a specific column, hence the special column name
         `"*"`.  A random sort can be combined with an ascending or descending sort on a specific
         column:  ```json POST /db/demo:main/tables/table/query {   "sort": [     {       "name":
         "desc"     },     {       "*": "random"     }   ] } ```  This will sort on the `name`
         column, breaking ties randomly.  ### Pagination  We offer cursor pagination and offset
-        pagination.  For queries that are expected to return more than 1000 records, cursor
-        pagination is needed in order to retrieve all of their results.  The offset pagination
-        method is limited to 1000 records.  Example of size + offset pagination:  ```json POST
-        /db/demo:main/tables/table/query {   "page": {     "size": 100,     "offset": 200   } }
-        ```  The `page.size` parameter represents the maximum number of records returned by this
-        query.  It has a default value of 20 and a maximum value of 200. The `page.offset`
-        parameter represents the number of matching records to skip.  It has a default value of 0
-        and a maximum value of 800.  Example of cursor pagination:  ```json POST
+        pagination.  The cursor pagination method can be used for sequential scrolling with
+        unrestricted depth.  The offset pagination can be used to skip pages and is limited to
+        1000 records.  Example of cursor pagination:  ```json POST
         /db/demo:main/tables/table/query {   "page": {
         "after":"fMoxCsIwFIDh3WP8c4amDai5hO5SJCRNfaVSeC9b6d1FD"   } } ```  In the above example,
         the value of the `page.after` parameter is the cursor returned by the previous query.  A
         sample response is shown below:  ```json {   "meta": {     "page": {       "cursor":
         "fMoxCsIwFIDh3WP8c4amDai5hO5SJCRNfaVSeC9b6d1FD",       "more": true     }   },
         "records": [...] } ```  The `page` object might contain the follow keys, in addition to
         `size` and `offset` that were introduced before:  - `after`: Return the next page 'after'
@@ -186,30 +181,41 @@
         both cursors to use the same filters and sort settings, plus we require `page.after <
         page.before`. The range query returns a new cursor.  If the range encompass multiple pages
         the next page in the range can be queried by update `page.after` to the returned cursor
         while keeping the `page.before` cursor from the first range query.  The `filter` ,
         `columns`, `sort` , and `page.size` configuration will be encoded with the cursor.  The
         pagination request will be invalid if `filter` or `sort` is set.  The columns returned and
         page size can be changed anytime by passing the `columns` or `page.size` settings to the
-        next query.  **Special cursors:**  - `page.after=end`: Result points past the last entry.
-        The list of records   returned is empty, but `page.meta.cursor` will include a cursor that
-        can be   used to "tail" the table from the end waiting for new data to be inserted.  -
-        `page.before=end`: This cursor returns the last page.  - `page.start=<cursor>`: Start at
-        the beginning of the result set of the <cursor> query.  This is equivalent to querying the
-        first page without a cursor but applying `filter` and `sort` . Yet the `page.start`
-        cursor can be convenient at times as user code does not need to remember the   filter,
-        sort, columns or page size configuration.  All these information are   read from the
-        cursor.  - `page.end=<cursor>`: Move to the end of the result set of the <cursor> query.
-        This is equivalent to querying the   last page with `page.before=end`, `filter`, and
-        `sort` . Yet the   `page.end` cursor can be more convenient at times as user code does not
-        need to remember the filter, sort, columns or page size configuration.  All   these
-        information are read from the cursor.  When using special cursors like `page.after="end"`
-        or `page.before="end"`, we still allow `filter` and `sort` to be set.  Example of getting
-        the last page:  ```json POST /db/demo:main/tables/table/query {   "page": {     "size":
-        10,     "before": "end"   } } ```
+        next query.  In the following example of size + offset pagination we retrieve the third
+        page of up to 100 results:  ```json POST /db/demo:main/tables/table/query {   "page": {
+        "size": 100,     "offset": 200   } } ```  The `page.size` parameter represents the maximum
+        number of records returned by this query.  It has a default value of 20 and a maximum
+        value of 200. The `page.offset` parameter represents the number of matching records to
+        skip.  It has a default value of 0 and a maximum value of 800.  Cursor pagination also
+        works in combination with offset pagination.  For example, starting from a specific cursor
+        position, using a page size of 200 and an offset of 800, you can skip up to 5 pages of 200
+        records forwards or backwards from the cursor's position:  ```json POST
+        /db/demo:main/tables/table/query {   "page": {     "size": 200,     "offset": 800,
+        "after": "fMoxCsIwFIDh3WP8c4amDai5hO5SJCRNfaVSeC9b6d1FD"   } } ```  **Special cursors:**
+        - `page.after=end`: Result points past the last entry.  The list of records   returned is
+        empty, but `page.meta.cursor` will include a cursor that can be   used to "tail" the table
+        from the end waiting for new data to be inserted.  - `page.before=end`: This cursor
+        returns the last page.  - `page.start=<cursor>`: Start at the beginning of the result set
+        of the <cursor> query.  This is equivalent to querying the   first page without a cursor
+        but applying `filter` and `sort` . Yet the `page.start`   cursor can be convenient at
+        times as user code does not need to remember the   filter, sort, columns or page size
+        configuration.  All these information are   read from the cursor.  - `page.end=<cursor>`:
+        Move to the end of the result set of the <cursor> query.  This is equivalent to querying
+        the   last page with `page.before=end`, `filter`, and `sort` . Yet the   `page.end` cursor
+        can be more convenient at times as user code does not   need to remember the filter, sort,
+        columns or page size configuration.  All   these information are read from the cursor.
+        When using special cursors like `page.after="end"` or `page.before="end"`, we still allow
+        `filter` and `sort` to be set.  Example of getting the last page:  ```json POST
+        /db/demo:main/tables/table/query {   "page": {     "size": 10,     "before": "end"   } }
+        ```
 
         Path: /db/{db_branch_name}/tables/{table_name}/query
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
```

### Comparing `xata-0.9.1/xata/namespaces/workspace/table.py` & `xata-0.9.2/xata/namespaces/workspace/table.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.1/PKG-INFO` & `xata-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

