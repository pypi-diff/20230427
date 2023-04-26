# Comparing `tmp/doorloop-0.0.5.tar.gz` & `tmp/doorloop-0.0.6.tar.gz`

## Comparing `doorloop-0.0.5.tar` & `doorloop-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 doorloop-0.0.5/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/__init__.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/accounts.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/base.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/communications.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/draft_leases.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/expenses.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/files.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/lease_charges.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/lease_credits.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/lease_payments.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/lease_returned_payments.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/leases.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/main.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/notes.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/owners.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/portfolios.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/properties.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/reports.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/tasks.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/tenants.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/units.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/users.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/vendor_bills.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/vendor_credits.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 doorloop-0.0.5/src/doorloop/vendors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/base.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_accounts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_communications.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_draft_leases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_expenses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_lease_charges.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_lease_credits.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_lease_payments.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_leases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_notes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_owners.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_portfolios.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_properties.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_reports.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_tasks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_tenants.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_units.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_vendor_bills.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_vendor_credits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.5/tests/test_vendors.py
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 doorloop-0.0.5/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 doorloop-0.0.5/LICENSE
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 doorloop-0.0.5/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 doorloop-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 doorloop-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 doorloop-0.0.6/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/accounts.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/base.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/communications.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/draft_leases.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/expenses.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/files.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/lease_charges.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/lease_credits.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/lease_payments.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/lease_returned_payments.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/leases.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/main.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/notes.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/owners.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/portfolios.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/properties.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/reports.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/tasks.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/tenants.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/units.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/users.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/vendor_bills.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/vendor_credits.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 doorloop-0.0.6/src/doorloop/vendors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/base.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test-file.pdf
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_accounts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_communications.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_draft_leases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_expenses.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_lease_charges.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_lease_credits.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_lease_payments.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_leases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_notes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_owners.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_portfolios.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_properties.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_reports.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_tasks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_tenants.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_units.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_vendor_bills.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_vendor_credits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doorloop-0.0.6/tests/test_vendors.py
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 doorloop-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 doorloop-0.0.6/LICENSE
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 doorloop-0.0.6/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 doorloop-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 doorloop-0.0.6/PKG-INFO
```

### Comparing `doorloop-0.0.5/.DS_Store` & `doorloop-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/accounts.py` & `doorloop-0.0.6/src/doorloop/accounts.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/base.py` & `doorloop-0.0.6/src/doorloop/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,16 +77,19 @@
 
             query_params = None
             if kwargs.get('query_params'):
                 query_params = kwargs['query_params']
                 del kwargs['query_params']
 
             if data:
-                # Convert data to json before sending
-                kwargs['data'] = json.dumps(data)
+                if kwargs['headers'].get('Content-Type') == 'application/json':
+                    # Convert data to json before sending
+                    kwargs['data'] = json.dumps(data)
+                else:
+                    kwargs['data'] = data
             return DoorLoopConnector.api_call(upper_name, self.get_url(endpoint, query_params), **kwargs)
 
         return f
 
     @staticmethod
     def api_call(upper_name, api_endpoint, **kwargs):
         def f(method_name, endpoint, **fkwargs):
```

### Comparing `doorloop-0.0.5/src/doorloop/communications.py` & `doorloop-0.0.6/src/doorloop/communications.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/draft_leases.py` & `doorloop-0.0.6/src/doorloop/draft_leases.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/expenses.py` & `doorloop-0.0.6/src/doorloop/expenses.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/files.py` & `doorloop-0.0.6/src/doorloop/leases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,45 @@
 from .base import DoorLoopBase
 
 
-class DoorLoopFile(DoorLoopBase):
-    endpoint_base = '/files'
-    RESOURCE_TYPES = [
-        'TENANT',
-        'OWNER',
-        'VENDOR',
-        'PROPERTY',
-        'UNIT',
-        'LEASE',
-        'LEASE_DRAFT',
-        'TASK',
-        'RENTAL_APPLICATION',
-    ]
+class DoorLoopLease(DoorLoopBase):
+    endpoint_base = '/leases'
 
     def list(self, **kwargs):
         '''
-        List all Files
-        https://api.doorloop.com/reference/get-files
+        List all Leases
+        https://api.doorloop.com/reference/get-leases
         '''
         response = self.connector.get(f'{self.endpoint_base}', **kwargs)
         return self.validator(response).validate()
 
-    def upload(self, data, **kwargs):
+    def retrieve(self, lease_id, **kwargs):
         '''
-        Upload a File
-        https://api.doorloop.com/reference/post-files
+        Retrieve a Lease
+        https://api.doorloop.com/reference/get-lease
         '''
-        # TODO convert file to string / binary file
-        response = self.connector.post(f'{self.endpoint_base}', data, **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/{lease_id}', **kwargs)
         return self.validator(response).validate()
 
-    def retrieve(self, file_id, **kwargs):
+    def move_in_tenant(self, data, **kwargs):
         '''
-        Retrieve a File
-        https://api.doorloop.com/reference/get-file
+        Move in Tenant
+        https://api.doorloop.com/reference/post-leases-move-in
         '''
-        response = self.connector.get(f'{self.endpoint_base}/{file_id}', **kwargs)
+        response = self.connector.post(f'{self.endpoint_base}/move-in', data, **kwargs)
         return self.validator(response).validate()
 
-    def update(self, file_id, data, **kwargs):
+    def move_out_tenant(self, data, **kwargs):
         '''
-        Update a File
-        https://api.doorloop.com/reference/put-file
+        Move out Tenant
+        https://api.doorloop.com/reference/post-leases-move-out
         '''
-        response = self.connector.put(f'{self.endpoint_base}/{file_id}', data, **kwargs)
+        response = self.connector.post(f'{self.endpoint_base}/move-out', data, **kwargs)
         return self.validator(response).validate()
 
-    def delete(self, file_id, **kwargs):
+    def list_lease_tenants(self, **kwargs):
         '''
-        Delete a File
-        https://api.doorloop.com/reference/delete-file
+        List all Lease Tenants
+        https://api.doorloop.com/reference/get-lease-tenants
         '''
-        response = self.connector.delete(f'{self.endpoint_base}/{file_id}', **kwargs)
-        return self.validator(response).validate()
-
-    def download(self, file_id, **kwargs):
-        '''
-        Download a File
-        https://api.doorloop.com/reference/download-file
-        '''
-        response = self.connector.get(f'{self.endpoint_base}/{file_id}/download', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/tenants', **kwargs)
         return self.validator(response).validate()
```

### Comparing `doorloop-0.0.5/src/doorloop/lease_charges.py` & `doorloop-0.0.6/src/doorloop/lease_charges.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/lease_credits.py` & `doorloop-0.0.6/src/doorloop/lease_credits.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/lease_payments.py` & `doorloop-0.0.6/src/doorloop/lease_payments.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/lease_returned_payments.py` & `doorloop-0.0.6/src/doorloop/lease_returned_payments.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/leases.py` & `doorloop-0.0.6/src/doorloop/reports.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 from .base import DoorLoopBase
 
 
-class DoorLoopLease(DoorLoopBase):
-    endpoint_base = '/leases'
+class DoorLoopReport(DoorLoopBase):
+    endpoint_base = '/reports'
 
-    def list(self, **kwargs):
+    def rent_roll(self, **kwargs):
         '''
-        List all Leases
-        https://api.doorloop.com/reference/get-leases
+        Rent Roll
+        https://api.doorloop.com/reference/get-reports-rent-roll
         '''
-        response = self.connector.get(f'{self.endpoint_base}', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/rent-roll', **kwargs)
         return self.validator(response).validate()
 
-    def retrieve(self, lease_id, **kwargs):
+    def profit_and_loss(self, **kwargs):
         '''
-        Retrieve a Lease
-        https://api.doorloop.com/reference/get-lease
+        Profit & Loss
+        https://api.doorloop.com/reference/get-reports-profit-and-loss
         '''
-        response = self.connector.get(f'{self.endpoint_base}/{lease_id}', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/profit-and-loss-summary', **kwargs)
         return self.validator(response).validate()
 
-    def move_in_tenant(self, data, **kwargs):
+    def cash_flow_statement(self, **kwargs):
         '''
-        Move in Tenant
-        https://api.doorloop.com/reference/post-leases-move-in
+        Cash Flow Statement
+        https://api.doorloop.com/reference/get-reports-cash-flow-statement
         '''
-        response = self.connector.post(f'{self.endpoint_base}/move-in', data, **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/cash-flow-statement', **kwargs)
         return self.validator(response).validate()
 
-    def move_out_tenant(self, data, **kwargs):
+    def balance_sheet(self, **kwargs):
         '''
-        Move out Tenant
-        https://api.doorloop.com/reference/post-leases-move-out
+        Balance Sheet
+        https://api.doorloop.com/reference/get-reports-balance-sheet
         '''
-        response = self.connector.post(f'{self.endpoint_base}/move-out', data, **kwargs)
-        return self.validator(response).validate()
-
-    def list_lease_tenants(self, **kwargs):
-        '''
-        List all Lease Tenants
-        https://api.doorloop.com/reference/get-lease-tenants
-        '''
-        response = self.connector.get(f'{self.endpoint_base}/tenants', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/balance-sheet-summary', **kwargs)
         return self.validator(response).validate()
```

### Comparing `doorloop-0.0.5/src/doorloop/main.py` & `doorloop-0.0.6/src/doorloop/main.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/notes.py` & `doorloop-0.0.6/src/doorloop/notes.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/owners.py` & `doorloop-0.0.6/src/doorloop/owners.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/portfolios.py` & `doorloop-0.0.6/src/doorloop/portfolios.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/properties.py` & `doorloop-0.0.6/src/doorloop/properties.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/reports.py` & `doorloop-0.0.6/src/doorloop/vendors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from .base import DoorLoopBase
 
 
-class DoorLoopReport(DoorLoopBase):
-    endpoint_base = '/reports'
+class DoorLoopVendor(DoorLoopBase):
+    endpoint_base = '/vendors'
 
-    def rent_roll(self, **kwargs):
+    def list(self, **kwargs):
         '''
-        Rent Roll
-        https://api.doorloop.com/reference/get-reports-rent-roll
+        List all Vendors
+        https://api.doorloop.com/reference/get-vendors
         '''
-        response = self.connector.get(f'{self.endpoint_base}/rent-roll', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}', **kwargs)
         return self.validator(response).validate()
 
-    def profit_and_loss(self, **kwargs):
+    def create(self, data, **kwargs):
         '''
-        Profit & Loss
-        https://api.doorloop.com/reference/get-reports-profit-and-loss
+        Create a Vendor
+        https://api.doorloop.com/reference/post-vendor
         '''
-        response = self.connector.get(f'{self.endpoint_base}/profit-and-loss-summary', **kwargs)
+        response = self.connector.post(f'{self.endpoint_base}', data, **kwargs)
         return self.validator(response).validate()
 
-    def cash_flow_statement(self, **kwargs):
+    def retrieve(self, vendor_id, **kwargs):
         '''
-        Cash Flow Statement
-        https://api.doorloop.com/reference/get-reports-cash-flow-statement
+        Retrieve a Vendor
+        https://api.doorloop.com/reference/get-vendor
         '''
-        response = self.connector.get(f'{self.endpoint_base}/cash-flow-statement', **kwargs)
+        response = self.connector.get(f'{self.endpoint_base}/{vendor_id}', **kwargs)
         return self.validator(response).validate()
 
-    def balance_sheet(self, **kwargs):
+    def update(self, vendor_id, data, **kwargs):
         '''
-        Balance Sheet
-        https://api.doorloop.com/reference/get-reports-balance-sheet
+        Update a Vendor
+        https://api.doorloop.com/reference/put-vendor
         '''
-        response = self.connector.get(f'{self.endpoint_base}/balance-sheet-summary', **kwargs)
+        response = self.connector.put(f'{self.endpoint_base}/{vendor_id}', data, **kwargs)
+        return self.validator(response).validate()
+
+    def delete(self, vendor_id, **kwargs):
+        '''
+        Delete a Vendor
+        https://api.doorloop.com/reference/delete-vendor
+        '''
+        response = self.connector.delete(f'{self.endpoint_base}/{vendor_id}', **kwargs)
         return self.validator(response).validate()
```

### Comparing `doorloop-0.0.5/src/doorloop/tasks.py` & `doorloop-0.0.6/src/doorloop/tasks.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/tenants.py` & `doorloop-0.0.6/src/doorloop/tenants.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/units.py` & `doorloop-0.0.6/src/doorloop/units.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/users.py` & `doorloop-0.0.6/src/doorloop/users.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/vendor_bills.py` & `doorloop-0.0.6/src/doorloop/vendor_bills.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/src/doorloop/vendor_credits.py` & `doorloop-0.0.6/src/doorloop/vendor_credits.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_accounts.py` & `doorloop-0.0.6/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_draft_leases.py` & `doorloop-0.0.6/tests/test_draft_leases.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_lease_payments.py` & `doorloop-0.0.6/tests/test_lease_payments.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             'paymentMethod': 'CASH',
             'lease': self.lease_id,
             'depositToAccount': self.deposit_account_id,
             'autoApplyPaymentOnCharges': True,
             'date': date.today().isoformat(),
         }
         response = self.dl.lease_payments.create(payload)
+        print(response.data)
         self.new_lease_payment_id = response['id']
         return response
 
     def test_list_lease_payments(self):
         response = self.dl.lease_payments.list()
         assert isinstance(response, dict)
         assert response['data'][0].get('reference')
```

### Comparing `doorloop-0.0.5/tests/test_leases.py` & `doorloop-0.0.6/tests/test_leases.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_properties.py` & `doorloop-0.0.6/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_tenants.py` & `doorloop-0.0.6/tests/test_tenants.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_units.py` & `doorloop-0.0.6/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/tests/test_users.py` & `doorloop-0.0.6/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/.gitignore` & `doorloop-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/LICENSE` & `doorloop-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/README.md` & `doorloop-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `doorloop-0.0.5/pyproject.toml` & `doorloop-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = [
     "hatchling",
-    "requests==2.0.0",
+    "requests>=2.0.1",
+    "requests-toolbelt==0.9.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "doorloop"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Colin McFaul", email="colinjmcfaul@gmail.com" },
 ]
 description = "This library provides a pure python interface to interact with the DoorLoop API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.0.0"
```

### Comparing `doorloop-0.0.5/PKG-INFO` & `doorloop-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doorloop
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library provides a pure python interface to interact with the DoorLoop API
 Project-URL: Homepage, https://github.com/cjmcfaul/doorloop
 Project-URL: Bugtracker, https://github.com/cjmcfaul/doorloop/issues
 Project-URL: Documentation, https://api.doorloop.com/reference/introduction
 Author-email: Colin McFaul <colinjmcfaul@gmail.com>
 License: Copyright (c) 2022 Colin J. McFaul
```

