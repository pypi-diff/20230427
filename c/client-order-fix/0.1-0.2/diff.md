# Comparing `tmp/client_order_fix-0.1.tar.gz` & `tmp/client_order_fix-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_order_fix-0.1.tar", last modified: Wed Apr 19 07:45:31 2023, max compression
+gzip compressed data, was "client_order_fix-0.2.tar", last modified: Thu Apr 27 11:00:15 2023, max compression
```

## Comparing `client_order_fix-0.1.tar` & `client_order_fix-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:45:31.259752 client_order_fix-0.1/
--rw-rw-rw-   0        0        0      149 2023-04-19 07:45:31.255713 client_order_fix-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 07:45:31.225327 client_order_fix-0.1/client_order_fix/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-0.1/client_order_fix/__init__.py
--rw-rw-rw-   0        0        0     7409 2023-04-19 06:24:32.000000 client_order_fix-0.1/client_order_fix/client_order.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:45:31.250258 client_order_fix-0.1/client_order_fix.egg-info/
--rw-rw-rw-   0        0        0      149 2023-04-19 07:45:30.000000 client_order_fix-0.1/client_order_fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-19 07:45:30.000000 client_order_fix-0.1/client_order_fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:45:30.000000 client_order_fix-0.1/client_order_fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-19 07:45:30.000000 client_order_fix-0.1/client_order_fix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 07:45:31.259752 client_order_fix-0.1/setup.cfg
--rw-rw-rw-   0        0        0      153 2023-04-19 07:43:16.000000 client_order_fix-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:15.582230 client_order_fix-0.2/
+-rw-rw-rw-   0        0        0      149 2023-04-27 11:00:15.578321 client_order_fix-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:15.542168 client_order_fix-0.2/client_order_fix/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-0.2/client_order_fix/__init__.py
+-rw-rw-rw-   0        0        0     8510 2023-04-27 07:57:26.000000 client_order_fix-0.2/client_order_fix/client_order.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:15.572221 client_order_fix-0.2/client_order_fix.egg-info/
+-rw-rw-rw-   0        0        0      149 2023-04-27 11:00:15.000000 client_order_fix-0.2/client_order_fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-27 11:00:15.000000 client_order_fix-0.2/client_order_fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:00:15.000000 client_order_fix-0.2/client_order_fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-27 11:00:15.000000 client_order_fix-0.2/client_order_fix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 11:00:15.583229 client_order_fix-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      153 2023-04-27 10:59:54.000000 client_order_fix-0.2/setup.py
```

### Comparing `client_order_fix-0.1/client_order_fix/client_order.py` & `client_order_fix-0.2/client_order_fix/client_order.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from typing import List
 import quickfix
 from datetime import datetime
 from random import randint
 
+ACCOUNT_DEV = 'muhua'
+PARTY_ID_DEV = 'muhua'
+ACCOUNT_UAT = 'TRC_TEST_ACT1'
+PARTY_ID_UAT = 'trc_test_trd1'
+
 
 class ClientOrder:
     __client_order_id = None
+    __quote_request_id = None
     __data_row = None
 
-    def __init__(self, client_order_id: str, data_row: dict):
-        self.__client_order_id = client_order_id
+    def __init__(self, unique_id: str, data_row: dict):
+        self.__client_order_id = unique_id
+        self.__quote_request_id = unique_id
         self.__data_row = data_row
 
-    def get_client_order_id(self) -> str:
-        return self.__client_order_id
+    def get_quote_request_id(self) -> str:
+        return self.__quote_request_id
 
     def get_test_fields(self) -> List[str]:
         return self.__data_row['testField'].split(',')
 
     def get_message_type(self) -> str:
         return self.__data_row['msgType']
 
@@ -26,85 +33,97 @@
 
     def get_value(self, fieldName: str):
         return self.__data_row[fieldName]
 
     def has_value(self, fieldName: str) -> bool:
         return fieldName in self.__data_row
 
-    def create_fix_msg(self):
+    def create_fix_msg(self, env='DEV'):
         message = quickfix.Message()
         header = message.getHeader()
 
         if self.__data_row.get('msgType'):
             if self.__data_row['msgType'] == 'empty':
                 header.setField(quickfix.MsgType(''))
             else:
                 header.setField(quickfix.MsgType(self.__data_row['msgType']))
 
         if self.__data_row.get('account'):
             if self.__data_row['account'] == 'empty':
                 message.setField(quickfix.Account(''))
+            elif self.__data_row['account'] == 'no tag':
+                pass
             else:
-                message.setField(quickfix.Account(self.__data_row['account']))
+                message.setField(quickfix.Account(self.__data_row.get('account')))
+        else:
+            if self.__data_row['msgType'] != 'g':
+                if env == 'DEV':
+                    message.setField(quickfix.Account(ACCOUNT_DEV))
+                elif env == 'UAT':
+                    message.setField(quickfix.Account(ACCOUNT_UAT))
 
         if self.__data_row.get('orderQty'):
             message.setField(quickfix.OrderQty(float(self.__data_row['orderQty'])))
 
-        if self.__data_row.get('price'):
-            message.setField(quickfix.Price(float(self.__data_row['price'])))
-
-        if self.__data_row.get('ordType'):
-            if self.__data_row['ordType'] == 'empty':
-                message.setField(quickfix.OrdType(''))
-            else:
-                message.setField(quickfix.OrdType(self.__data_row['ordType']))
-
         if self.__data_row.get('side'):
             if self.__data_row['side'] == 'empty':
                 message.setField(quickfix.Side(''))
             else:
                 message.setField(quickfix.Side(self.__data_row['side']))
 
         if self.__data_row.get('symbol'):
             if self.__data_row['symbol'] == 'empty':
                 message.setField(quickfix.Symbol(''))
             else:
                 message.setField(quickfix.Symbol(self.__data_row['symbol']))
 
-        if self.__data_row.get('tif'):
-            message.setField(quickfix.TimeInForce(self.__data_row['tif']))
-
         if self.__data_row.get('currency'):
             if self.__data_row['currency'] == 'empty':
                 message.setField(quickfix.Currency(''))
             else:
                 message.setField(quickfix.Currency(self.__data_row['currency']))
 
         if self.__data_row.get('settlType'):
             if self.__data_row['settlType'] == 'empty':
                 message.setField(quickfix.SettlType(''))
             else:
                 message.setField(quickfix.SettlType(self.__data_row['settlType']))
 
+        if self.__data_row.get('quoteType'):
+            message.setField(quickfix.QuoteType(int(self.__data_row['quoteType'])))
+
         if self.__data_row.get('noPartyId'):
             if self.__data_row['noPartyId'] == "1":
                 group = quickfix.Group(453, 448)
             else:
                 groupOne = quickfix.Group(453, 448)
                 groupTwo = quickfix.Group(453, 448)
 
         if self.__data_row.get('partyId'):
             if self.__data_row['partyId'] == 'empty':
                 group.setField(quickfix.PartyID(''))
+            elif self.__data_row['partyId'] == 'no tag':
+                pass
             else:
                 if self.__data_row['noPartyId'] == "1":
                     group.setField(quickfix.PartyID(self.__data_row['partyId']))
+        else:
+            if self.__data_row['msgType'] != 'g':
+                if self.__data_row['noPartyId'] == "1":
+                    if env == 'DEV':
+                        group.setField(quickfix.PartyID(PARTY_ID_DEV))
+                    elif env == 'UAT':
+                        group.setField(quickfix.PartyID(PARTY_ID_UAT))
                 else:
-                    groupOne.setField(quickfix.PartyID(self.__data_row['partyId']))
-                    groupTwo.setField(quickfix.PartyID(self.__data_row['partyId']))
+                    if env == 'DEV':
+                        groupOne.setField(quickfix.PartyID(PARTY_ID_DEV))
+                        groupTwo.setField(quickfix.PartyID(PARTY_ID_DEV))
+                    else:
+                        groupOne.setField(quickfix.PartyID(PARTY_ID_UAT))
+                        groupTwo.setField(quickfix.PartyID(PARTY_ID_UAT))
 
         if self.__data_row.get('partyIdSource'):
             if self.__data_row['partyIdSource'] == 'empty':
                 group.setField(quickfix.PartyIDSource(''))
             else:
                 if self.__data_row['noPartyId'] == "1":
                     group.setField(quickfix.PartyIDSource(self.__data_row['partyIdSource']))
@@ -123,54 +142,64 @@
                     message.addGroup(group)
                 else:
                     groupOne.setField(quickfix.PartyRole(int(self.__data_row['partyRole'])))
                     groupTwo.setField(quickfix.PartyRole(int(self.__data_row['partyRole'])))
                     message.addGroup(groupOne)
                     message.addGroup(groupTwo)
 
+        if self.__data_row.get('quoteReqId'):
+            message.setField(quickfix.QuoteReqID(self.__quote_request_id))
+
+        if self.__data_row.get('ordType'):
+            if self.__data_row['ordType'] == 'empty':
+                message.setField(quickfix.OrdType(''))
+            else:
+                message.setField(quickfix.OrdType(self.__data_row['ordType']))
+
+        if self.__data_row.get('tif'):
+            if self.__data_row['tif'] == 'empty':
+                message.setField(quickfix.TimeInForce(''))
+            else:
+                message.setField(quickfix.TimeInForce(self.__data_row['tif']))
+
+        if self.__data_row.get('clOrdId'):
+            message.setField(quickfix.ClOrdID(self.__client_order_id))
+
         if self.__data_row.get('tradSesReqId'):
             if self.__data_row['tradSesReqId'] == 'empty':
                 message.setField(quickfix.TradSesReqID(''))
             elif self.__data_row['tradSesReqId'] == 'no tag':
                 pass
             elif self.__data_row['tradSesReqId'] == 'yes':
                 tradeReqId = str(randint(0, 100000)) + str(datetime.now().strftime('%M:%S.%f')[:-4])
                 message.setField(quickfix.TradSesReqID(tradeReqId))
             else:
                 message.setField(quickfix.TradSesReqID("12"))
 
-        if self.__data_row.get('clOrdId') and self.__client_order_id is not None:
-            message.setField(quickfix.ClOrdID(self.__client_order_id))
-
         if self.__data_row.get('trxTime'):
             self.setTransactionTime(message)
 
         return message
 
     def setTransactionTime(self, message):
         if self.__data_row['trxTime'] == 'yes':
             transactTime = quickfix.TransactTime()
             transactTime.setString(datetime.utcnow().strftime("%Y%m%d-%H:%M:%S.%f")[:-3])
             message.setField(transactTime)
         elif self.__data_row['trxTime'] == 'invalid':
             message.setField(quickfix.TransactTime(10))
 
     @staticmethod
-    def __get_client_order_id(row, last_order) -> str:
-        if row['clOrdId'] == 'yes':
+    def generateUniqueId(row, requestString) -> str:
+        if row[requestString] == 'yes':
             return str(randint(0, 100000)) + str(datetime.now().strftime('%M:%S.%f')[:-4])
-        elif row['clOrdId'] == 'no tag':
+        elif row[requestString] == 'no tag':
             return None
-        elif row['clOrdId'] == 'empty':
+        elif row[requestString] == 'empty':
             return ''
-        elif row['clOrdId'] == 'duplicate':
-            if not last_order:
-                raise Exception("Invalid usage. Cannot use 'duplicate' for client order id, when not previous orders "
-                                "have been sent via this connection.")
-            return last_order.get_client_order_id()
-        else:
-            return row['clOrdId']
+        elif row[requestString] == 'duplicate':
+            return '12345'
 
     @staticmethod
-    def from_table_row(row: dict, last_order) -> 'ClientOrder':
-        client_order_id = ClientOrder.__get_client_order_id(row, last_order)
-        return ClientOrder(client_order_id, row)
+    def from_table_row(row: dict, requestString) -> 'ClientOrder':
+        unique_id = ClientOrder.generateUniqueId(row, requestString)
+        return ClientOrder(unique_id, row)
```

