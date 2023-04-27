# Comparing `tmp/gallagher_restapi-0.1.0b5.tar.gz` & `tmp/gallagher_restapi-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallagher_restapi-0.1.0b5.tar", max compression
+gzip compressed data, was "gallagher_restapi-0.1.0b6.tar", max compression
```

## Comparing `gallagher_restapi-0.1.0b5.tar` & `gallagher_restapi-0.1.0b6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      478 2023-02-11 14:01:55.793713 gallagher_restapi-0.1.0b5/gallagher_restapi/__init__.py
--rw-r--r--   0        0        0     2407 2023-02-11 14:01:55.793713 gallagher_restapi-0.1.0b5/gallagher_restapi/__main__.py
--rw-r--r--   0        0        0     7686 2023-02-11 14:01:55.793713 gallagher_restapi-0.1.0b5/gallagher_restapi/client.py
--rw-r--r--   0        0        0      408 2023-02-11 14:01:55.793713 gallagher_restapi-0.1.0b5/gallagher_restapi/exceptions.py
--rw-r--r--   0        0        0    18000 2023-02-14 10:58:50.702265 gallagher_restapi-0.1.0b5/gallagher_restapi/models.py
--rw-r--r--   0        0        0      364 2023-02-14 10:59:02.710428 gallagher_restapi-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b5/setup.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0      478 2023-02-28 13:10:35.763716 gallagher_restapi-0.1.0b6/gallagher_restapi/__init__.py
+-rw-r--r--   0        0        0     3871 2023-04-27 13:33:38.065231 gallagher_restapi-0.1.0b6/gallagher_restapi/__main__.py
+-rw-r--r--   0        0        0     9578 2023-04-27 13:29:58.793058 gallagher_restapi-0.1.0b6/gallagher_restapi/client.py
+-rw-r--r--   0        0        0      408 2023-02-17 07:35:07.879731 gallagher_restapi-0.1.0b6/gallagher_restapi/exceptions.py
+-rw-r--r--   0        0        0    22956 2023-04-27 13:27:39.116922 gallagher_restapi-0.1.0b6/gallagher_restapi/models.py
+-rw-r--r--   0        0        0      382 2023-04-27 13:34:54.533282 gallagher_restapi-0.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b6/setup.py
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b6/PKG-INFO
```

### Comparing `gallagher_restapi-0.1.0b5/gallagher_restapi/client.py` & `gallagher_restapi-0.1.0b6/gallagher_restapi/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Gallagher REST api python library."""
 import asyncio
 import logging
+from enum import Enum
 from ssl import SSLError
 from typing import Any, AsyncIterator
 
 import httpx
 
 from .exceptions import (
     ConnectError,
@@ -15,26 +16,28 @@
 )
 from .models import (
     EventFilter,
     FTApiFeatures,
     FTCardholder,
     FTEvent,
     FTEventGroup,
-    FTEventType,
     FTItem,
+    FTItemReference,
+    FTITemTypes,
+    FTPersonalDataFieldDefinition,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BaseClient:
     """Gallagher REST api base client."""
 
     api_features: FTApiFeatures
-    item_types: dict
+    item_types: FTITemTypes
 
     def __init__(
         self,
         api_key: str,
         *,
         host: str = "localhost",
         port: int = 8904,
@@ -42,72 +45,118 @@
     ) -> None:
         """Initialize REST api client."""
         self.server_url = f"https://{host}:{port}"
         self.httpx_client: httpx.AsyncClient = httpx_client or httpx.AsyncClient(
             verify=False
         )
         self.httpx_client.headers = httpx.Headers(
-            {"Authorization": f"GGL-API-KEY {api_key}"}
+            {
+                "Authorization": f"GGL-API-KEY {api_key}",
+                "Content-Type": "application/json",
+            }
         )
         self.httpx_client.timeout.read = 60
 
     async def _async_request(
-        self, method: str, endpoint: str, params: dict[str, str] | None = None
+        self,
+        method: str,
+        endpoint: str,
+        *,
+        data: dict[str, Any] | None = None,
+        params: dict[str, str] | str | None = None,
     ) -> Any:
         """Send a http request and return the response."""
-        _LOGGER.info("Sending request to endpoint: %s, params: %s", endpoint, params)
+        _LOGGER.info(
+            "Sending %s request to endpoint: %s, data: %s, params: %s",
+            method,
+            endpoint,
+            data,
+            params,
+        )
         try:
-            response = await self.httpx_client.request(method, endpoint, params=params)
+            response = await self.httpx_client.request(
+                method, endpoint, params=params, json=data
+            )
         except (httpx.ConnectError, httpx.ReadTimeout, SSLError) as err:
             raise ConnectError(
                 f"Connection failed while sending request: {err}"
             ) from err
+        _LOGGER.debug(
+            "status_code: %s, response: %s", response.status_code, response.text
+        )
         if response.status_code == httpx.codes.UNAUTHORIZED:
             raise Unauthorized("Unauthorized request. Ensure api key is correct")
         if response.status_code == httpx.codes.FORBIDDEN:
             raise LicenseError("Site is not licensed for this operation")
         if response.status_code == httpx.codes.NOT_FOUND:
             raise RequestError(
                 "Requested item does not exist or "
                 "your operator does not have the privilege to view it"
             )
         if response.status_code == httpx.codes.BAD_REQUEST:
             raise RequestError(response.json()["message"])
-        if response.status_code != httpx.codes.OK:
-            raise GllApiError(response.text)
-        _LOGGER.debug("Response: %s", response.text)
+        if response.status_code == httpx.codes.CREATED:
+            return True
         return response.json()
 
-    async def authenticate(self):
+    async def authenticate(self) -> None:
         """Connect to Server to authenticate."""
         response = await self._async_request("GET", f"{self.server_url}/api/")
-        self.api_features = FTApiFeatures(response["features"])
+        self.api_features = FTApiFeatures(**response["features"])
 
-    async def get_item_types(self):
+    async def get_item_types(self) -> None:
         """Get FTItem types."""
-        item_types = await self._async_request("GET", self.api_features.item_types.href)
-        if item_types.get("itemTypes"):
-            for item_type in item_types["itemTypes"]:
-                self.item_types.update({item_type["name"]: item_type["id"]})
+        item_types: list[str] = []
+        response = await self._async_request(
+            "GET", self.api_features.href("items/item_types")
+        )
+        if response.get("itemTypes"):
+            item_types = [
+                item_type["name"]
+                for item_type in response["itemTypes"]
+                if item_type["name"]
+            ]
+        self.item_types = Enum("FTITemTypes", item_types)  # type: ignore
+
+    async def get_item(
+        self, item_type: FTITemTypes, name: str | None = None
+    ) -> list[FTItem]:
+        """Get FTItems filtered by type and name."""
+        # We will force selecting type for now
+        params = {"type": item_type.value}
+        if name:
+            params["name"] = name
+        items: list[FTItem] = []
+        if response := await self._async_request(
+            "GET", self.api_features.href("items"), params=params
+        ):
+            items = [FTItem(**item) for item in response["results"]]
+        return items
 
 
 class CardholderClient(BaseClient):
     """REST api cardholder client for Gallagher Command Center."""
 
-    async def get_personal_data_field(self, name: str | None = None) -> list[FTItem]:
+    async def get_personal_data_field(
+        self, name: str | None = None, extra_fields: list[str] = []
+    ) -> list[FTItem]:
         """Return List of available personal data fields."""
         pdfs: list[FTItem] = []
-        params = {}
+        extra_fields.append("defaults")
+        params = {"fields": ",".join(extra_fields)}
         if name:
             params = {"name": name}
 
         if response := await self._async_request(
-            "GET", self.api_features.personal_data_fields.href, params=params
+            "GET", self.api_features.href("personalDataFields"), params=params
         ):
-            pdfs = [FTItem(pdf) for pdf in response]
+            pdfs = [
+                FTPersonalDataFieldDefinition.from_dict(pdf)
+                for pdf in response["results"]
+            ]
 
         return pdfs
 
     async def get_cardholder(
         self,
         *,
         ftitem_id: int | None = None,
@@ -115,97 +164,110 @@
         pdfs: dict[str, str] | None = None,
         detailed: bool = False,
     ) -> list[FTCardholder]:
         """Return list of cardholders."""
         cardholders: list[FTCardholder] = []
         if ftitem_id:
             response: dict[str, Any] = await self._async_request(
-                "GET", f"{self.api_features.cardholders.href}/{ftitem_id}"
+                "GET", f"{self.api_features.href('cardholders')}/{ftitem_id}"
             )
             if response:
-                return [FTCardholder(response)]
+                return [FTCardholder.from_dict(response)]
 
         else:
             if name and not isinstance(name, str):
                 raise ValueError("name field must be a string value.")
             if pdfs and not isinstance(pdfs, dict):
                 raise ValueError("pdfs field must be a dict.")
             params = {}
             if name:
                 params = {"name": name}
 
             if pdfs:
-                for name, value in pdfs.items():
-                    if not (name.startswith('"') and name.endswith('"')):
-                        name = f'"{name}"'
+                for pdf_name, value in pdfs.items():
+                    if not (pdf_name.startswith('"') and pdf_name.endswith('"')):
+                        pdf_name = f'"{pdf_name}"'
                     # if pdf name is correct we expect the result to include one item only
-                    if not (pdf_field := await self.get_personal_data_field(name=name)):
-                        raise GllApiError(f"pdf field: {name} not found")
-                    params.update({f"pdf_{pdf_field[0].ftitem_id}": value})
+                    if not (
+                        pdf_field := await self.get_personal_data_field(name=pdf_name)
+                    ):
+                        raise GllApiError(f"pdf field: {pdf_name} not found")
+                    params.update({f"pdf_{pdf_field[0].id}": value})
 
             response = await self._async_request(
-                "GET", self.api_features.cardholders.href, params=params
+                "GET", self.api_features.href("cardholders"), params=params
             )
             if response["results"]:
                 if detailed:
                     for cardholder in response["results"]:
                         cardholder_details = await self._async_request(
                             "GET", cardholder["href"]
                         )
-                        cardholders.append(FTCardholder(cardholder_details))
+                        cardholders.append(FTCardholder.from_dict(cardholder_details))
                 else:
                     cardholders = [
-                        FTCardholder(cardholder) for cardholder in response["results"]
+                        FTCardholder.from_dict(cardholder)
+                        for cardholder in response["results"]
                     ]
         return cardholders
 
+    async def create_cardholder(self, cardholder: FTCardholder) -> FTItemReference:
+        """Create a new cardholder in Gallagher."""
+        return await self._async_request(
+            "POST", self.api_features.href("cardholders"), data=cardholder.as_dict
+        )
+
 
 class EventClient(BaseClient):
     """REST api event client for Gallagher Command Center."""
 
     event_groups: dict[str, FTEventGroup]
-    event_types: dict[str, FTEventType]
+    event_types: dict[str, FTItem]
 
     async def get_event_types(self) -> None:
         """Return list of event types."""
         response = await self._async_request(
-            "GET", self.api_features.events_features.event_groups.href
+            "GET", self.api_features.href("events/eventGroups")
         )
         self.event_groups = {
-            FTEventGroup(event_group).name: FTEventGroup(event_group)
+            FTEventGroup.from_dict(event_group).name: FTEventGroup.from_dict(
+                event_group
+            )
             for event_group in response["eventGroups"]
         }
         self.event_types = {}
         for event_group in self.event_groups.values():
             self.event_types.update(
                 {event_type.name: event_type for event_type in event_group.event_types}
             )
 
-    async def get_events(self, filter: EventFilter | None = None) -> list[FTEvent]:
+    async def get_events(
+        self, event_filter: EventFilter | None = None
+    ) -> list[FTEvent]:
         """Return list of events filtered by params."""
         events: list[FTEvent] = []
         if response := await self._async_request(
             "GET",
-            self.api_features.events_features.events.href,
-            params=filter.params if filter else None,
+            self.api_features.href("events"),
+            params=event_filter.as_dict if event_filter else None,
         ):
-            events = [FTEvent(event) for event in response["events"]]
+            events = [FTEvent.from_dict(event) for event in response["events"]]
         return events
 
     async def get_new_events(
-        self, filter: EventFilter | None = None
+        self, event_filter: EventFilter | None = None
     ) -> AsyncIterator[list[FTEvent]]:
         """Yield a list of new events filtered by params."""
         response = await self._async_request(
             "GET",
-            self.api_features.events_features.updates.href,
-            params=filter.params if filter else None,
+            self.api_features.href("events/updates"),
+            params=event_filter.as_dict if event_filter else None,
         )
         while True:
             _LOGGER.debug(response)
-            yield [FTEvent(event) for event in response["events"]]
+            yield [FTEvent.from_dict(event) for event in response["events"]]
             await asyncio.sleep(1)
             response = await self._async_request(
                 "GET",
                 response["updates"]["href"],
-                params=filter.params if filter else None,
+                params=event_filter.as_dict if event_filter else None,
             )
```

### Comparing `gallagher_restapi-0.1.0b5/gallagher_restapi/models.py` & `gallagher_restapi-0.1.0b6/gallagher_restapi/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,216 +1,361 @@
 """Gallagher item models."""
+from __future__ import annotations
+
+import json
 from collections.abc import Callable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
+from enum import Enum
 from typing import Any
+
 import pytz
 
-class FTItemReference:
-    """FTItem reference class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTItemReference."""
+class FTITemTypes(Enum):
+    """Enumrate FTItem types."""
+
+
+@dataclass
+class FTApiFeatures:
+    """FTApiFeatures class."""
+
+    accessGroups: dict[str, Any]
+    accessZones: dict[str, Any]
+    alarms: dict[str, Any]
+    alarmZones: dict[str, Any]
+    cardholders: dict[str, Any]
+    cardTypes: dict[str, Any]
+    competencies: dict[str, Any]
+    dayCategories: dict[str, Any]
+    doors: dict[str, Any]
+    elevators: dict[str, Any]
+    events: dict[str, Any]
+    fenceZones: dict[str, Any]
+    inputs: dict[str, Any]
+    interlockGroups: dict[str, Any]
+    items: dict[str, Any]
+    lockerBanks: dict[str, Any]
+    macros: dict[str, Any]
+    operatorGroups: dict[str, Any]
+    outputs: dict[str, Any]
+    personalDataFields: dict[str, Any]
+    receptions: dict[str, Any]
+    roles: dict[str, Any]
+    schedules: dict[str, Any]
+    visits: dict[str, Any]
+
+    def href(self, feature: str) -> str:
+        """
+        Return href link for feature.
+        For subfeteatures use format feature/subfeature
+        """
+        main_feature = sub_feature = ""
+        try:
+            if "/" in feature:
+                main_feature, sub_feature = feature.split("/")
+            else:
+                main_feature = feature
+        except ValueError:
+            raise ValueError("Incorrect syntax of feature.")
+
+        if not (attr := getattr(self, main_feature)):
+            raise ValueError(f"{main_feature} is not a valid feature")
+        if sub_feature and sub_feature not in attr:
+            raise ValueError(f"{sub_feature} is not found in {main_feature}")
+        return attr[main_feature or sub_feature]["href"]
 
-        self.href: str = kwargs.get("href", "")
 
+@dataclass
+class FTItemReference:
+    """FTItem reference class."""
 
-class FTNavigation(FTItemReference):
-    """FTNavigation Class."""
+    href: str = field(default_factory=str)
 
 
+@dataclass
 class FTStatus:
     """FTStatus class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTStatus item."""
-        self.value = kwargs["value"]
-        self.type = kwargs["type"]
+    value: str
+    type: str
 
 
+@dataclass
 class FTItemType:
     """FTItemType class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTItem type."""
-        self.ftitem_id: str = kwargs["id"]
-        self.name: str = kwargs["name"]
+    id: str
+    name: str
 
 
-class FTItem(FTItemReference):
+@dataclass
+class FTItem:
     """FTItem class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTItem."""
-        super().__init__(kwargs)
-        self.ftitem_id: str = kwargs["id"]
-        self.name: str = kwargs["name"]
+    id: str
+    name: str
+    href: str = field(default_factory=str)
+    type: dict = field(default_factory=dict)
 
 
-class FTLinkItem(FTItemReference):
+@dataclass
+class FTLinkItem:
     """FTLinkItem class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTItem link."""
-        super().__init__(kwargs)
-        self.name: str = kwargs["name"]
-
-
-class FTApiFeaturesEvents:
-    """FTApiFeature events class."""
-
-    def __init__(self, features: dict[str, Any]) -> None:
-        """Initialize FTApiFeature events."""
-        self.events = FTNavigation(features["events"])
-        self.updates = FTNavigation(features["updates"])
-        self.event_groups = FTNavigation(features["eventGroups"])
-        self.divisions = FTNavigation(features["divisions"])
-
-
-class FTApiFeaturesAlarms:
-    """FTApiFeature alarms class."""
-
-    def __init__(self, features: dict[str, Any]) -> None:
-        """Initialize FTApiFeature alarms."""
-        self.alarms = FTNavigation(features["alarms"])
-        self.updates = FTNavigation(features["updates"])
-        self.divisions = FTNavigation(features["divisions"])
-
-
-class FTApiFeatures:
-    """FTApiFeatures class."""
-
-    def __init__(self, features: dict[str, Any]) -> None:
-        """Initialize FTApi features."""
-        self.items = FTNavigation(features["items"]["items"])
-        self.item_types = FTNavigation(features["items"]["itemTypes"])
-        self.alarms_features = FTApiFeaturesAlarms(features["alarms"])
-        self.events_features = FTApiFeaturesEvents(features["events"])
-        self.cardholders = FTNavigation(features["cardholders"]["cardholders"])
-        self.personal_data_fields = FTNavigation(
-            features["personalDataFields"]["personalDataFields"]
-        )
+    name: str
+    href: str = field(default_factory=str)
 
 
-class FTAccessGroupMembership(FTItemReference):
+@dataclass
+class FTAccessGroupMembership:
     """FTAccessGroupMembership base class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTAccessGroupMembership item."""
-        super().__init__(kwargs)
-        self.status = FTStatus(kwargs["status"])
-        self.access_group = FTLinkItem(kwargs["accessGroup"])
+    status: FTStatus = field(init=False)
+    access_group: FTLinkItem = field(init=False)
+    active_from: datetime = field(init=False)
+    active_until: datetime = field(init=False)
+    href: str = field(default_factory=str)
+
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        """Return json string for post and update."""
+        _dict: dict[str, Any] = {"accessgroup": {"href": self.href}}
+        if self.active_from:
+            _dict["from"] = f"{self.active_from.isoformat()}Z"
+        if self.active_until:
+            _dict["until"] = f"{self.active_until.isoformat()}Z"
+        return _dict
+
+    @classmethod
+    def assign_membership(
+        cls,
+        access_group: FTItem,
+        active_from: datetime | None = None,
+        active_until: datetime | None = None,
+    ) -> FTAccessGroupMembership:
+        """Create an FTAccessGroup item to assign."""
+        _cls = FTAccessGroupMembership(href=access_group.href)
+        if active_from:
+            _cls.active_from = active_from
+        if active_until:
+            _cls.active_until = active_until
+        return _cls
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTAccessGroupMembership:
+        """Return FTAccessGroupMembership object from dict."""
+        _cls = FTAccessGroupMembership()
+
+        if status := kwargs.get("status"):
+            _cls.status = FTStatus(**status)
+        if access_group := kwargs.get("accessGroup"):
+            _cls.access_group = FTLinkItem(**access_group)
         if active_from := kwargs.get("from"):
-            self.active_from = datetime.fromisoformat(active_from[:-1]).replace(tzinfo=pytz.UTC)
+            _cls.active_from = datetime.fromisoformat(active_from[:-1]).replace(
+                tzinfo=pytz.utc
+            )
         if active_until := kwargs.get("until"):
-            self.active_until = datetime.fromisoformat(active_until[:-1]).replace(tzinfo=pytz.UTC)
+            _cls.active_until = datetime.fromisoformat(active_until[:-1]).replace(
+                tzinfo=pytz.utc
+            )
+        return _cls
 
 
-class FTCardholderCard(FTItemReference):
+@dataclass
+class FTCardholderCard:
     """FTCardholder card base class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTCardholder card item."""
-        super().__init__(kwargs)
-        self.number: str = kwargs["number"]
-        self.card_serial_number: str | None = kwargs.get("cardSerialNumber")
-        self.issue_level: int | None = kwargs.get("issueLevel")
-        self.status = FTStatus(kwargs["status"])
-        self.type = FTLinkItem(kwargs["type"])
-        if access_group := kwargs.get("accessGroups"):
-            self.access_group = FTLinkItem(access_group)
+    type: FTLinkItem | FTItem
+    number: str = field(init=False)
+    card_serial_number: str = field(init=False)
+    issue_level: int = field(init=False)
+    status: FTStatus = field(init=False)
+    active_from: datetime = field(init=False)
+    active_until: datetime = field(init=False)
+
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        """Return json string for post and update."""
+        _dict: dict[str, Any] = {"type": {"href": self.type.href}}
+        if self.number:
+            _dict["number"] = self.number
+        if self.issue_level:
+            _dict["issueLevel"] = self.issue_level
+        if self.active_from:
+            _dict["from"] = f"{self.active_from.isoformat()}Z"
+        if self.active_until:
+            _dict["until"] = f"{self.active_until.isoformat()}Z"
+        return _dict
+
+    @classmethod
+    def create_card(
+        cls,
+        card_type: FTItem,
+        number: str = "",
+        issue_level: int | None = None,
+        active_from: datetime | None = None,
+        active_until: datetime | None = None,
+    ) -> FTCardholderCard:
+        """Create an FTCardholder card object."""
+        _cls = FTCardholderCard(type=card_type)
+        if number:
+            _cls.number = number
+        if issue_level:
+            _cls.issue_level = issue_level
+        if active_from:
+            _cls.active_from = active_from
+        if active_until:
+            _cls.active_until = active_until
+        return _cls
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTCardholderCard:
+        """Return FTCardholderCard object from dict."""
+        _cls = FTCardholderCard(type=FTLinkItem(**kwargs["type"]))
+        if number := kwargs.get("number"):
+            _cls.number = number
+        if issue_level := kwargs.get("issueLevel"):
+            _cls.issue_level = issue_level
+        if status := kwargs.get("status"):
+            _cls.status = FTStatus(**status)
         if active_from := kwargs.get("from"):
-            self.active_from = datetime.fromisoformat(active_from[:-1]).replace(tzinfo=pytz.UTC)
+            _cls.active_from = datetime.fromisoformat(active_from[:-1]).replace(
+                tzinfo=pytz.utc
+            )
         if active_until := kwargs.get("until"):
-            self.active_until = datetime.fromisoformat(active_until[:-1]).replace(tzinfo=pytz.UTC)
+            _cls.active_until = datetime.fromisoformat(active_until[:-1]).replace(
+                tzinfo=pytz.utc
+            )
+        return _cls
 
 
-class FTPersonalDataDefinition(FTItem):
-    """FTPersonalDataDefinition class."""
+@dataclass(init=False)
+class FTPersonalDataFieldDefinition:
+    """FTPersonalDataFieldDefinition class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTPersonalDataDefinition item."""
-        super().__init__(kwargs)
-        self.type = kwargs["type"]
+    id: str
+    name: str
+    description: str
+    type: str
+    division: FTItemReference | None = None
+    default: str = field(default_factory=str)
+    href: str = field(default_factory=str)
+    required: bool = False
+    unique: bool = False
+    accessGroups: list[FTLinkItem] = field(default_factory=list)
+    regex: str = ""
+    regexDescription: str = ""
+    contentType: str = ""
+    isProfileImage: bool = False
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTPersonalDataFieldDefinition:
+        """Return FTPersonalDataFieldDefinition object from dict."""
+        _cls = FTPersonalDataFieldDefinition()
+        for key, value in kwargs.items():
+            setattr(_cls, key, value)
+        return _cls
 
 
-class FTCardholderPdfValue(FTItemReference):
+@dataclass
+class FTCardholderPdfValue:
     """FTCardholderPdfValue class."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTCardholderPdfValue item."""
-        super().__init__(kwargs)
-        self.definition = FTPersonalDataDefinition(kwargs["definition"])
-        if value := kwargs.get("value"):
-            if isinstance(value, dict):
-                self.value = FTNavigation(value)
-            else:
-                self.value = value
+    name: str
+    value: str | FTItemReference = field(init=False)
+    notifications: bool = field(init=False)
+    definition: FTItem = field(init=False)
+    href: str = field(init=False)
+
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        """Return json string for post and update."""
+        return {f"@{self.name}": {"notifications": self.notifications}}
+
+    @classmethod
+    def create_pdf(
+        cls, pdf_definition: FTItem, value: str, enable_notification: bool = False
+    ) -> FTCardholderPdfValue:
+        """Create FTCardholderPdfValue object for POST."""
+        _cls = FTCardholderPdfValue(name=pdf_definition.name)
+        _cls.value = value
+        _cls.notifications = enable_notification
+        return _cls
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, dict[str, Any]]) -> FTCardholderPdfValue:
+        """Return FTCardholderPdfValue object from dict."""
+        for name, info in kwargs.items():
+            _cls = FTCardholderPdfValue(name=name[1:])
+            if value := info.get("value"):
+                _cls.value = (
+                    FTItemReference(**value) if isinstance(value, dict) else value
+                )
+            if definition := info.get("definition"):
+                _cls.definition = FTPersonalDataDefinition(**definition)
+            if href := info.get("href"):
+                _cls.href = href
+        return _cls
 
 
 @dataclass
 class FTCardholderField:
     """Class to represent FTCardholder field."""
 
-    key: str
     name: str
-    value: Callable[[Any], Any] = lambda val: val
+    from_dict: Callable[[Any], Any] = lambda val: val
+    to_dict: Callable[[Any], Any] = lambda val: val
 
 
 FTCARDHOLDER_FIELDS: tuple[FTCardholderField, ...] = (
-    FTCardholderField(key="href", name="href"),
-    FTCardholderField(key="ftitem_id", name="id"),
-    FTCardholderField(key="name", name="name"),
-    FTCardholderField(key="first_name", name="firstName"),
-    FTCardholderField(key="last_name", name="lastName"),
-    FTCardholderField(key="short_name", name="shortName"),
-    FTCardholderField(key="description", name="description"),
-    FTCardholderField(key="authorised", name="authorised"),
+    FTCardholderField(name="href"),
+    FTCardholderField(name="id"),
+    FTCardholderField(name="name"),
+    FTCardholderField(name="firstName"),
+    FTCardholderField(name="lastName"),
+    FTCardholderField(name="shortName"),
+    FTCardholderField(name="description"),
+    FTCardholderField(name="authorised"),
     FTCardholderField(
-        key="last_successful_access_time",
         name="lastSuccessfulAccessTime",
-        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.UTC),
+        from_dict=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
     ),
     FTCardholderField(
-        key="last_successful_access_zone",
         name="lastSuccessfulAccessZone",
-        value=lambda val: FTLinkItem(val),
+        from_dict=lambda val: FTLinkItem(**val),
     ),
-    FTCardholderField(key="server_display_name", name="serverDisplayName"),
+    FTCardholderField(name="serverDisplayName"),
+    FTCardholderField(name="division", from_dict=lambda val: FTItemReference(**val)),
+    FTCardholderField(name="disableCipherPad"),
+    FTCardholderField(name="usercode"),
+    FTCardholderField(name="operatorLoginEnabled"),
+    FTCardholderField(name="operatorUsername"),
+    FTCardholderField(name="operatorPassword"),
+    FTCardholderField(name="operatorPasswordExpired"),
+    FTCardholderField(name="windowsLoginEnabled"),
+    FTCardholderField(name="windowsUsername"),
     FTCardholderField(
-        key="division", name="division", value=lambda val: FTItemReference(val)
-    ),
-    FTCardholderField(key="disable_cipher_pad", name="disableCipherPad"),
-    FTCardholderField(key="user_code", name="usercode"),
-    FTCardholderField(key="operator_login_enabled", name="operatorLoginEnabled"),
-    FTCardholderField(key="operator_username", name="operatorUsername"),
-    FTCardholderField(key="operator_password", name="operatorPassword"),
-    FTCardholderField(key="operator_password_expired", name="operatorPasswordExpired"),
-    FTCardholderField(key="windows_login_enabled", name="windowsLoginEnabled"),
-    FTCardholderField(key="windows_username", name="windowsUsername"),
-    FTCardholderField(
-        key="personal_data_definitions",
         name="personalDataDefinitions",
-        value=lambda val: {
-            pdf_name[1:]: FTCardholderPdfValue(pdf_value)
-            for pdf in val
-            for pdf_name, pdf_value in pdf.items()
-        },
+        from_dict=lambda val: [
+            FTCardholderPdfValue.from_dict(pdf_value) for pdf_value in val
+        ],
+        to_dict=lambda val: [pdf_value.to_dict for pdf_value in val],
     ),
     FTCardholderField(
-        key="cards",
         name="cards",
-        value=lambda val: [FTCardholderCard(card) for card in val],
+        from_dict=lambda val: [FTCardholderCard.from_dict(card) for card in val],
+        to_dict=lambda val: [card.to_dict for card in val],
     ),
     FTCardholderField(
-        key="access_groups",
         name="accessGroups",
-        value=lambda val: [
-            FTAccessGroupMembership(access_group) for access_group in val
+        from_dict=lambda val: [
+            FTAccessGroupMembership.from_dict(access_group) for access_group in val
         ],
+        to_dict=lambda val: [card.to_dict for card in val],
     ),
     # FTCardholderField(
     #     key="operator_groups",
     #     name="operatorGroups",
     #     value=lambda val: [
     #         FTOperatorGroup(operator_group) for operator_group in val
     #     ],
@@ -218,124 +363,149 @@
     # FTCardholderField(
     #     key="competencies",
     #     name="competencies",
     #     value=lambda val: [
     #         FTCompetency(competency) for competency in val
     #     ],
     # ),
-    FTCardholderField(key="edit", name="edit", value=lambda val: FTItemReference(val)),
+    FTCardholderField(name="edit", from_dict=lambda val: FTItemReference(**val)),
     FTCardholderField(
-        key="update_location",
         name="updateLocation",
-        value=lambda val: FTItemReference(val),
+        from_dict=lambda val: FTItemReference(**val),
     ),
-    FTCardholderField(key="notes", name="notes"),
+    FTCardholderField(name="notes"),
     # FTCardholderField(key="notifications", name="notifications", value=lambda val: FTNotification(val)),
-    FTCardholderField(key="relationships", name="relationships"),
-    FTCardholderField(key="lockers", name="lockers"),
-    FTCardholderField(key="elevatorGroups", name="elevatorGroups"),
+    FTCardholderField(name="relationships"),
+    FTCardholderField(name="lockers"),
+    FTCardholderField(name="elevatorGroups"),
     FTCardholderField(
-        key="last_printed_or_encodedTime",
         name="lastPrintedOrEncodedTime",
-        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.UTC),
-    ),
-    FTCardholderField(
-        key="last_printed_or_encoded_issue_level", name="lastPrintedOrEncodedIssueLevel"
+        from_dict=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
     ),
-    FTCardholderField(key="redactions", name="redactions"),
+    FTCardholderField(name="lastPrintedOrEncodedIssueLevel"),
+    FTCardholderField(name="redactions"),
 )
 
 
+@dataclass
 class FTCardholder:
     """FTCardholder details class."""
 
-    href: str
-    ftitem_id: str
-    name: str
-    first_name: str
-    last_name: str
-    short_name: str
-    description: str
-    authorised: bool
-    last_successful_access_time: datetime
-    last_successful_access_zone: FTLinkItem
-    server_display_name: str
-    division: FTItemReference
-    disable_cipher_pad: bool
-    user_code: str
-    operator_login_enabled: bool
-    operator_username: str
-    operator_password: str
-    operator_password_expired: bool
-    windows_login_enabled: bool
-    windows_username: str
-    personal_data_definitions: dict[str, FTCardholderPdfValue]
-    cards: list[FTCardholderCard]
-    access_groups: list[FTAccessGroupMembership]
+    href: str = field(init=False)
+    id: str = field(init=False)
+    division: FTItemReference | None = None
+    name: str = field(init=False)
+    firstName: str = field(default="")
+    lastName: str = field(default="")
+    shortName: str = field(default="")
+    description: str = field(default="")
+    authorised: bool = field(default=False)
+    pdfs: dict[str, Any] = field(default_factory=dict)
+    lastSuccessfulAccessTime: datetime = field(init=False)
+    lastSuccessfulAccessZone: FTLinkItem = field(init=False)
+    serverDisplayName: str = field(init=False)
+    disableCipherPad: bool = field(default=False)
+    usercode: str = field(default="")
+    operatorLoginEnabled: bool = field(default=False)
+    operatorUsername: str = field(default="")
+    operatorPassword: str = field(default="")
+    operatorPasswordExpired: bool = field(default=False)
+    windowsLoginEnabled: bool = field(default=False)
+    windowsUsername: str = field(default="")
+    personalDataDefinitions: dict[str, FTCardholderPdfValue] | None = field(
+        default=None
+    )
+    cards: list[FTCardholderCard] | None = None
+    accessGroups: list[FTAccessGroupMembership] | None = None
     # operator_groups: str
     # competencies: str
     # edit: str
-    update_location: FTItemReference
-    notes: str
-    relationships: Any
-    lockers: Any
-    elevatorGroups: Any
-    last_printed_or_encodedTime: datetime
-    last_printed_or_encoded_issue_level: int
-    redactions: Any
-
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize FTCardholder item."""
-        self.pdfs: dict[str, Any] = {
-            pdf_name[1:]: pdf_value
-            for pdf_name, pdf_value in kwargs.items()
-            if pdf_name.startswith("@")
-        }
+    updateLocation: FTItemReference | None = None
+    notes: str = field(default="")
+    # relationships: Any | None = None
+    lockers: Any | None = None
+    elevatorGroups: Any | None = None
+    lastPrintedOrEncodedTime: datetime | None = None
+    lastPrintedOrEncodedIssueLevel: int | None = None
+    # redactions: Any | None = None
+
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        """Return serialized str."""
+        _dict: dict[str, Any] = {}
         for cardholder_field in FTCARDHOLDER_FIELDS:
-            if cardholder_field.name in kwargs:
-                setattr(
-                    self,
-                    cardholder_field.key,
-                    cardholder_field.value(kwargs[cardholder_field.name]),
-                )
+            try:
+                if value := getattr(self, cardholder_field.name):
+                    _dict[cardholder_field.name] = cardholder_field.to_dict(value)
+            except AttributeError:
+                continue
+
+        if self.pdfs:
+            _dict.update({f"@{name}": value for name, value in self.pdfs.items()})
+        return json.loads(json.dumps(_dict, default=lambda o: o.__dict__))
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTCardholder:
+        """Return FTCardholder object from dict."""
+
+        _cls = FTCardholder()
+        for cardholder_field in FTCARDHOLDER_FIELDS:
+            if value := kwargs.get(cardholder_field.name):
+                setattr(_cls, cardholder_field.name, cardholder_field.from_dict(value))
+
+        for cardholder_pdf in list(kwargs.keys()):
+            if cardholder_pdf.startswith("@"):
+                _cls.pdfs[cardholder_pdf[1:]] = kwargs[cardholder_pdf]
+
+        return _cls
 
 
 # Gallagher alarm and event models
-class FTAlarm(FTItemReference):
+@dataclass
+class FTAlarm:
     """FTAlarm summary class"""
 
-    def __init__(self, kwargs: dict[str, Any]):
-        """Initialize FTAlarm."""
-        super().__init__(kwargs)
-        self.state: str = kwargs["state"]
+    state: str
+    href: str = field(default_factory=str)
 
 
+@dataclass
 class FTEventCard:
     """Event card details."""
 
-    def __init__(self, kwargs: dict[str, Any]) -> None:
-        """Initialize event card."""
-        self.number: str = kwargs["number"]
-        self.issue_level: int = kwargs["issueLevel"]
-        self.facility_code: str = kwargs["facilityCode"]
-
+    number: str
+    issue_level: int = field(init=False)
+    facility_code: str = field(init=False)
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTEventCard:
+        """Return Event card object from dict."""
+
+        _cls = FTEventCard(number=kwargs["number"])
+        _cls.issue_level = kwargs["issueLevel"]
+        _cls.facility_code = kwargs["facilityCode"]
+        return _cls
 
-class FTEventType(FTItem):
-    """FTEvent type class."""
 
-
-class FTEventGroup(FTItem):
+@dataclass
+class FTEventGroup:
     """FTEvent group class."""
 
-    def __init__(self, kwargs: dict[str, Any]):
-        """Initialize FTEvent group."""
-        super().__init__(kwargs)
-        self.event_types: list[FTEventType] = [
-            FTEventType(event_type) for event_type in kwargs["eventTypes"]
-        ]
+    id: str
+    name: str
+    href: str = field(default_factory=str)
+    event_types: list[FTItem] = field(init=False)
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTEventGroup:
+        """Return Event card object from dict."""
+        event_types = kwargs.pop("eventTypes")
+        _cls = FTEventGroup(**kwargs)
+        _cls.event_types = [FTItem(**event_type) for event_type in event_types]
+        return _cls
 
 
 @dataclass
 class EventField:
     """Class to represent Event field."""
 
     key: str
@@ -343,66 +513,71 @@
     value: Callable[[Any], Any] = lambda val: val
 
 
 EVENT_FIELDS: tuple[EventField, ...] = (
     EventField(key="defaults", name="defaults"),
     EventField(key="details", name="details"),
     EventField(key="href", name="href"),
-    EventField(key="ftitem_id", name="id"),
+    EventField(key="id", name="id"),
     EventField(key="server_display_name", name="serverDisplayName"),
     EventField(key="message", name="message"),
     EventField(
         key="time",
         name="time",
-        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.UTC),
+        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
     ),
     EventField(key="occurrences", name="occurrences"),
     EventField(key="priority", name="priority"),
-    EventField(key="alarm", name="alarm", value=lambda val: FTAlarm(val)),
-    EventField(key="operator", name="operator", value=lambda val: FTLinkItem(val)),
-    EventField(key="source", name="source", value=lambda val: FTItem(val)),
-    EventField(key="event_group", name="group", value=lambda val: FTItemType(val)),
-    EventField(key="event_type", name="type", value=lambda val: FTItemType(val)),
-    EventField(key="event_type2", name="eventType", value=lambda val: FTItemType(val)),
-    EventField(key="division", name="division", value=lambda val: FTItem(val)),
+    EventField(key="alarm", name="alarm", value=lambda val: FTAlarm(**val)),
+    EventField(key="operator", name="operator", value=lambda val: FTLinkItem(**val)),
+    EventField(key="source", name="source", value=lambda val: FTItem(**val)),
+    EventField(key="event_group", name="group", value=lambda val: FTItemType(**val)),
+    EventField(key="event_type", name="type", value=lambda val: FTItemType(**val)),
     EventField(
-        key="cardholder", name="cardholder", value=lambda val: FTCardholder(val)
+        key="event_type2", name="eventType", value=lambda val: FTItemType(**val)
     ),
+    EventField(key="division", name="division", value=lambda val: FTItem(**val)),
     EventField(
-        key="entry_access_zone", name="entryAccessZone", value=lambda val: FTItem(val)
+        key="cardholder",
+        name="cardholder",
+        value=FTCardholder.from_dict,
     ),
     EventField(
-        key="exit_access_zone", name="exitAccessZone", value=lambda val: FTItem(val)
+        key="entry_access_zone", name="entryAccessZone", value=lambda val: FTItem(**val)
     ),
-    EventField(key="door", name="door", value=lambda val: FTLinkItem(val)),
     EventField(
-        key="access_group", name="accessGroup", value=lambda val: FTItemReference(val)
+        key="exit_access_zone", name="exitAccessZone", value=lambda val: FTItem(**val)
     ),
-    EventField(key="card", name="card", value=lambda val: FTEventCard(val)),
+    EventField(key="door", name="door", value=lambda val: FTLinkItem(**val)),
+    EventField(key="access_group", name="accessGroup", value=lambda val: FTItem(**val)),
+    EventField(key="card", name="card", value=FTEventCard.from_dict),
     # EventField(
     #     key="modified_item",
     #     name="modifiedItem",
     #     value=lambda val: FTEventCard(val),
     # ),
     EventField(
         key="last_occurrence_time",
         name="lastOccurrenceTime",
-        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.UTC),
+        value=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
+    ),
+    EventField(
+        key="previous", name="previous", value=lambda val: FTItemReference(**val)
     ),
-    EventField(key="previous", name="previous", value=lambda val: FTItemReference(val)),
-    EventField(key="next", name="next", value=lambda val: FTItemReference(val)),
-    EventField(key="updates", name="updates", value=lambda val: FTItemReference(val)),
+    EventField(key="next", name="next", value=lambda val: FTItemReference(**val)),
+    EventField(key="updates", name="updates", value=lambda val: FTItemReference(**val)),
 )
 
 
+@dataclass(init=False)
 class FTEvent:
     """FTEvent summary class."""
 
     href: str
-    ftitem_id: str
+    id: str
     details: str
     server_display_name: str
     message: str
     time: datetime
     occurrences: int
     priority: int
     alarm: FTAlarm
@@ -420,96 +595,95 @@
     card: FTEventCard
     # modified_item: str
     last_occurrence_time: datetime
     previous: FTItemReference
     next: FTItemReference
     updates: FTItemReference
 
-    def __init__(self, kwargs: dict[str, Any]):
-        """Initialize FTEvent."""
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTEvent:
+        """Return FTEvent object from dict."""
+
+        _cls = FTEvent()
         for event_field in EVENT_FIELDS:
-            if event_field.name in kwargs:
-                setattr(
-                    self,
-                    event_field.key,
-                    event_field.value(kwargs[event_field.name]),
-                )
+            if (value := kwargs.get(event_field.name)) or (
+                value := kwargs.get(event_field.key)
+            ):
+                if isinstance(value, dict):
+                    value = event_field.value(kwargs[event_field.name])
+                setattr(_cls, event_field.key, value)
 
+        return _cls
 
+
+@dataclass
 class EventFilter:
     """Event filter class."""
 
-    def __init__(
-        self,
-        top: int | None = None,
-        after: datetime | None = None,
-        before: datetime | None = None,
-        sources: list[FTItem] | list[str] | None = None,
-        event_types: list[FTEventType] | list[str] | None = None,
-        event_groups: list[FTEventGroup] | list[str] | None = None,
-        cardholders: list[FTCardholder] | list[str] | None = None,
-        divisions: list[FTItem] | list[str] | None = None,
-        related_items: list[FTItem] | list[str] | None = None,
-        fields: list[str] | None = None,
-        previous: bool = False,
-    ) -> None:
-        """Initialize event filter."""
-        self.params: dict[str, Any] = {"previous": previous}
-        if top:
-            self.params["top"] = str(top)
-        if after and (after_value := after.isoformat()):
-            self.params["after"] = after_value
-        if before and (before_value := before.isoformat()):
-            self.params["after"] = before_value
-        if sources:
+    top: int | None = None
+    after: datetime | None = None
+    before: datetime | None = None
+    sources: list[FTItem] | list[str] | None = None
+    event_types: list[FTItem] | list[str] | None = None
+    event_groups: list[FTEventGroup] | list[str] | None = None
+    cardholders: list[FTCardholder] | list[str] | None = None
+    divisions: list[FTItem] | list[str] | None = None
+    related_items: list[FTItem] | list[str] | None = None
+    fields: list[str] | None = None
+    previous: bool = False
+
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        """Return event filter as dict."""
+        params: dict[str, Any] = {"previous": self.previous}
+        if self.top:
+            params["top"] = str(self.top)
+        if self.after and (after_value := self.after.isoformat()):
+            params["after"] = after_value
+        if self.before and (before_value := self.before.isoformat()):
+            params["after"] = before_value
+        if self.sources:
             source_ids = [
-                source.ftitem_id if isinstance(source, FTItem) else source
-                for source in sources
+                source.id if isinstance(source, FTItem) else source
+                for source in self.sources
             ]
-            self.params["source"] = ",".join(source_ids)
-        if event_types:
+            params["source"] = ",".join(source_ids)
+        if self.event_types:
             event_type_ids = [
-                event_type.ftitem_id
-                if isinstance(event_type, FTEventType)
-                else event_type
-                for event_type in event_types
+                event_type.id if isinstance(event_type, FTItem) else event_type
+                for event_type in self.event_types
             ]
-            self.params["type"] = ",".join(event_type_ids)
-        if event_groups:
+            params["type"] = ",".join(event_type_ids)
+        if self.event_groups:
             event_group_ids = [
-                event_group.ftitem_id
-                if isinstance(event_group, FTEventGroup)
-                else event_group
-                for event_group in event_groups
+                event_group.id if isinstance(event_group, FTEventGroup) else event_group
+                for event_group in self.event_groups
             ]
-            self.params["group"] = ",".join(event_group_ids)
-        if cardholders:
+            params["group"] = ",".join(event_group_ids)
+        if self.cardholders:
             cardholder_ids = [
-                cardholder.ftitem_id
-                if isinstance(cardholder, FTCardholder)
-                else cardholder
-                for cardholder in cardholders
+                cardholder.id if isinstance(cardholder, FTCardholder) else cardholder
+                for cardholder in self.cardholders
             ]
-            self.params["cardholder"] = ",".join(cardholder_ids)
-        if divisions:
+            params["cardholder"] = ",".join(cardholder_ids)
+        if self.divisions:
             division_ids = [
-                division.ftitem_id if isinstance(division, FTItem) else division
-                for division in divisions
+                division.id if isinstance(division, FTItem) else division
+                for division in self.divisions
             ]
-            self.params["division"] = ",".join(division_ids)
-        if related_items:
+            params["division"] = ",".join(division_ids)
+        if self.related_items:
             related_item_ids = [
-                related_item.ftitem_id
-                if isinstance(related_item, FTItem)
-                else related_item
-                for related_item in related_items
+                related_item.id if isinstance(related_item, FTItem) else related_item
+                for related_item in self.related_items
             ]
-            self.params["relatedItem"] = ",".join(related_item_ids)
-        if fields:
+            params["relatedItem"] = ",".join(related_item_ids)
+        if self.fields:
             event_fields = [field.name for field in EVENT_FIELDS]
-            for field in fields:
+            for event_field in self.fields:
                 if (
-                    not field.startswith("cardholder.pdf_")
-                    and field not in event_fields
+                    not event_field.startswith("cardholder.pdf_")
+                    and event_field not in event_fields
                 ):
-                    raise ValueError(f"'{field}' is not a valid field")
-            self.params["fields"] = ",".join(fields)
+                    raise ValueError(f"'{event_field}' is not a valid field")
+            params["fields"] = ",".join(self.fields)
+        return params
```

### Comparing `gallagher_restapi-0.1.0b5/setup.py` & `gallagher_restapi-0.1.0b6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['gallagher_restapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.3,<0.24.0', 'pytz>=2022.7.1,<2023.0.0']
+['attrs>=22.2.0,<23.0.0', 'httpx>=0.23.3,<0.24.0', 'pytz>=2022.7.1,<2023.0.0']
 
 setup_kwargs = {
     'name': 'gallagher-restapi',
-    'version': '0.1.0b5',
+    'version': '0.1.0b6',
     'description': '',
     'long_description': 'None',
     'author': 'Rami Mosleh',
     'author_email': 'engrbm87@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

