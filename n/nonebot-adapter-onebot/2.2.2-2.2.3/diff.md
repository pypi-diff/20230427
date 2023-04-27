# Comparing `tmp/nonebot_adapter_onebot-2.2.2.tar.gz` & `tmp/nonebot_adapter_onebot-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_onebot-2.2.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_onebot-2.2.3.tar", max compression
```

## Comparing `nonebot_adapter_onebot-2.2.2.tar` & `nonebot_adapter_onebot-2.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1064 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/LICENSE
--rw-r--r--   0        0        0     3931 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/README.md
--rw-r--r--   0        0        0      657 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/__init__.py
--rw-r--r--   0        0        0     3676 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/collator.py
--rw-r--r--   0        0        0     1040 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/store.py
--rw-r--r--   0        0        0     1447 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/utils.py
--rw-r--r--   0        0        0      721 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/__init__.py
--rw-r--r--   0        0        0    16027 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/adapter.py
--rw-r--r--   0        0        0     7347 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/bot.py
--rw-r--r--   0        0        0    12564 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/bot.pyi
--rw-r--r--   0        0        0      822 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/config.py
--rw-r--r--   0        0        0    13865 2023-03-17 08:07:49.331112 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/event.py
--rw-r--r--   0        0        0     1541 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/exception.py
--rw-r--r--   0        0        0     8664 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/helpers.py
--rw-r--r--   0        0        0    10253 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/message.py
--rw-r--r--   0        0        0     2036 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/permission.py
--rw-r--r--   0        0        0     1302 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/utils.py
--rw-r--r--   0        0        0      428 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/__init__.py
--rw-r--r--   0        0        0    24430 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/adapter.py
--rw-r--r--   0        0        0     7506 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/bot.py
--rw-r--r--   0        0        0    15093 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/bot.pyi
--rw-r--r--   0        0        0     1007 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/config.py
--rw-r--r--   0        0        0     8798 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/event.py
--rw-r--r--   0        0        0     6704 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/exception.py
--rw-r--r--   0        0        0     3956 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/message.py
--rw-r--r--   0        0        0      569 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/permission.py
--rw-r--r--   0        0        0     1674 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/utils.py
--rw-r--r--   0        0        0     1596 2023-03-17 08:07:49.335113 nonebot_adapter_onebot-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 nonebot_adapter_onebot-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/LICENSE
+-rw-r--r--   0        0        0     3931 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/README.md
+-rw-r--r--   0        0        0      657 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/__init__.py
+-rw-r--r--   0        0        0     3676 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/collator.py
+-rw-r--r--   0        0        0     1040 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/store.py
+-rw-r--r--   0        0        0     3087 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/utils.py
+-rw-r--r--   0        0        0      721 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/__init__.py
+-rw-r--r--   0        0        0    16027 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/adapter.py
+-rw-r--r--   0        0        0     7347 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.py
+-rw-r--r--   0        0        0    12564 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.pyi
+-rw-r--r--   0        0        0      822 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/config.py
+-rw-r--r--   0        0        0    13247 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/event.py
+-rw-r--r--   0        0        0     1541 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/exception.py
+-rw-r--r--   0        0        0     8664 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/helpers.py
+-rw-r--r--   0        0        0    10577 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/message.py
+-rw-r--r--   0        0        0     2036 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/permission.py
+-rw-r--r--   0        0        0     1302 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/utils.py
+-rw-r--r--   0        0        0      428 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/__init__.py
+-rw-r--r--   0        0        0    24430 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/adapter.py
+-rw-r--r--   0        0        0     7506 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.py
+-rw-r--r--   0        0        0    15093 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.pyi
+-rw-r--r--   0        0        0     1007 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/config.py
+-rw-r--r--   0        0        0     8217 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/event.py
+-rw-r--r--   0        0        0     6704 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/exception.py
+-rw-r--r--   0        0        0     4136 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/message.py
+-rw-r--r--   0        0        0      569 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/permission.py
+-rw-r--r--   0        0        0     1674 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/utils.py
+-rw-r--r--   0        0        0     1649 2023-04-27 10:11:01.265124 nonebot_adapter_onebot-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 nonebot_adapter_onebot-2.2.3/PKG-INFO
```

### Comparing `nonebot_adapter_onebot-2.2.2/LICENSE` & `nonebot_adapter_onebot-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/README.md` & `nonebot_adapter_onebot-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/__init__.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/collator.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/store.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/__init__.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/adapter.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/bot.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/bot.pyi` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/config.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/event.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 FrontMatter:
     sidebar_position: 4
     description: onebot.v11.event 模块
 """
 
 from copy import deepcopy
-from functools import reduce
-from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
+from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
 
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from pydantic import BaseModel, root_validator
 
 from nonebot.adapters import Event as BaseEvent
+from nonebot.adapters.onebot.utils import highlight_rich_message
 
 from .message import Message
 from .exception import NoLogException
 
 if TYPE_CHECKING:
     from .bot import Bot
 
@@ -176,49 +176,33 @@
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     message_type: Literal["private"]
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        texts: List[str] = []
-        msg_string: List[str] = []
-        for seg in self.original_message:
-            if seg.is_text():
-                texts.append(repr(seg))
-            else:
-                msg_string.extend(
-                    (escape_tag("".join(texts)), f"<le>{escape_tag(repr(seg))}</le>")
-                )
-                texts.clear()
-        msg_string.append(escape_tag("".join(texts)))
-        return f"Message {self.message_id} from {self.user_id} {''.join(msg_string)!r}"
+        return (
+            f"Message {self.message_id} from {self.user_id} "
+            f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
+        )
 
 
 class GroupMessageEvent(MessageEvent):
     """群消息"""
 
     message_type: Literal["group"]
     group_id: int
     anonymous: Optional[Anonymous] = None
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        texts: List[str] = []
-        msg_string: List[str] = []
-        for seg in self.original_message:
-            if seg.is_text():
-                texts.append(repr(seg))
-            else:
-                msg_string.extend(
-                    (escape_tag("".join(texts)), f"<le>{escape_tag(repr(seg))}</le>")
-                )
-                texts.clear()
-        msg_string.append(escape_tag("".join(texts)))
-        return f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] {''.join(msg_string)!r}"
+        return (
+            f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] "
+            f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
+        )
 
     @overrides(MessageEvent)
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 # Notice Events
```

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/exception.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/helpers.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/helpers.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/message.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,23 @@
     sidebar_position: 5
     description: onebot.v11.message 模块
 """
 
 import re
 from io import BytesIO
 from pathlib import Path
+from functools import partial
 from typing import Type, Tuple, Union, Iterable, Optional
 
 from nonebot.typing import overrides
 
+from nonebot.adapters.onebot.utils import b2s, f2s
 from nonebot.adapters import Message as BaseMessage
-from nonebot.adapters.onebot.utils import b2s, f2s, truncate
+from nonebot.adapters.onebot.utils import rich_escape
+from nonebot.adapters.onebot.utils import truncate as trunc
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 from .utils import log, escape, unescape
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
     """OneBot v11 协议 MessageSegment 适配。具体方法参考协议消息段类型或源码。"""
@@ -25,29 +28,32 @@
     @classmethod
     @overrides(BaseMessageSegment)
     def get_message_class(cls) -> Type["Message"]:
         return Message
 
     @overrides(BaseMessageSegment)
     def __str__(self) -> str:
-        # process special types
         if self.is_text():
             return escape(self.data.get("text", ""), escape_comma=False)
 
         params = ",".join(
-            [f"{k}={escape(str(v))}" for k, v in self.data.items() if v is not None]
+            f"{k}={escape(str(v))}" for k, v in self.data.items() if v is not None
         )
         return f"[CQ:{self.type}{',' if params else ''}{params}]"
 
-    def __repr__(self) -> str:
+    def to_rich_text(self, truncate: Optional[int] = 70) -> str:
         if self.is_text():
-            return escape(self.data.get("text", ""), escape_comma=False)
+            return rich_escape(self.data.get("text", ""), escape_comma=False)
+
+        truncate_func = partial(trunc, length=truncate) if truncate else lambda x: x
 
-        params = ", ".join(
-            [f"{k}={truncate(str(v))}" for k, v in self.data.items() if v is not None]
+        params = ",".join(
+            f"{k}={rich_escape(truncate_func(str(v)))}"
+            for k, v in self.data.items()
+            if v is not None
         )
         return f"[{self.type}{':' if params else ''}{params}]"
 
     @overrides(BaseMessageSegment)
     def __add__(
         self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
     ) -> "Message":
@@ -260,16 +266,16 @@
     def __add__(
         self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
     ) -> "Message":
         return super(Message, self).__add__(
             MessageSegment.text(other) if isinstance(other, str) else other
         )
 
-    def __repr__(self) -> str:
-        return "".join(repr(seg) for seg in self)
+    def to_rich_text(self, truncate: Optional[int] = 70) -> str:
+        return "".join(seg.to_rich_text(truncate=truncate) for seg in self)
 
     @overrides(BaseMessage)
     def __radd__(
         self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
     ) -> "Message":
         return super(Message, self).__radd__(
             MessageSegment.text(other) if isinstance(other, str) else other
```

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/permission.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v11/utils.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/adapter.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,11 +650,11 @@
         if impl is not None and platform is None:
             raise ValueError("platform must be specified")
         key = f"/{impl}/{platform}" if impl and platform else ""
         cls.send_handlers[key] = send_func
 
     @classmethod
     def get_send(
-        cls, platform: Optional[str] = None, impl: Optional[str] = None
+        cls, impl: Optional[str] = None, platform: Optional[str] = None
     ) -> Callable[[Bot, Event, Union[str, Message, MessageSegment]], Any]:
         key = f"/{impl}/{platform}" if impl and platform else ""
         return cls.send_handlers.get(key, cls.send_handlers.get("", send))
```

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/bot.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/bot.pyi` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/config.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/event.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, Dict, List, Literal, Optional
 
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from pydantic import Extra, BaseModel, root_validator
 
 from nonebot.adapters import Event as BaseEvent
+from nonebot.adapters.onebot.utils import highlight_rich_message
 
 from .message import Message
 from .exception import NoLogException
 
 
 class Event(BaseEvent, extra=Extra.allow):
     """OneBot V12 协议事件，字段与 OneBot 一致
@@ -142,48 +143,32 @@
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     detail_type: Literal["private"]
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        texts: List[str] = []
-        msg_string: List[str] = []
-        for seg in self.original_message:
-            if seg.is_text():
-                texts.append(repr(seg))
-            else:
-                msg_string.extend(
-                    (escape_tag("".join(texts)), f"<le>{escape_tag(repr(seg))}</le>")
-                )
-                texts.clear()
-        msg_string.append(escape_tag("".join(texts)))
-        return f"Message {self.message_id} from {self.user_id} {''.join(msg_string)!r}"
+        return (
+            f"Message {self.message_id} from {self.user_id} "
+            f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
+        )
 
 
 class GroupMessageEvent(MessageEvent):
     """群消息"""
 
     detail_type: Literal["group"]
     group_id: str
 
     @overrides(Event)
     def get_event_description(self) -> str:
-        texts: List[str] = []
-        msg_string: List[str] = []
-        for seg in self.original_message:
-            if seg.is_text():
-                texts.append(str(seg))
-            else:
-                msg_string.extend(
-                    (escape_tag("".join(texts)), f"<le>{escape_tag(str(seg))}</le>")
-                )
-                texts.clear()
-        msg_string.append(escape_tag("".join(texts)))
-        return f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] {''.join(msg_string)!r}"
+        return (
+            f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] "
+            f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
+        )
 
     @overrides(MessageEvent)
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class ChannelMessageEvent(MessageEvent):
```

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/exception.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/message.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """OneBot v12 消息类型。
 
 FrontMatter:
     sidebar_position: 5
     description: onebot.v12.message 模块
 """
 
-from typing import Any, Type, Iterable
+from functools import partial
+from typing import Any, Type, Iterable, Optional
 
 from nonebot.typing import overrides
 
-from nonebot.adapters.onebot.utils import truncate
 from nonebot.adapters import Message as BaseMessage
+from nonebot.adapters.onebot.utils import rich_escape
+from nonebot.adapters.onebot.utils import truncate as trunc
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
     """OneBot v12 协议 MessageSegment 适配。具体方法参考协议消息段类型或源码。"""
 
     @classmethod
     @overrides(BaseMessageSegment)
     def get_message_class(cls) -> Type["Message"]:
         return Message
 
     @overrides(BaseMessageSegment)
     def __str__(self) -> str:
-        if self.is_text():
-            return self.data.get("text", "")
-
-        params = ", ".join([f"{k}={v}" for k, v in self.data.items() if v is not None])
-        return f"[{self.type}{':' if params else ''}{params}]"
+        return self.to_rich_text(truncate=None)
 
-    def __repr__(self) -> str:
+    def to_rich_text(self, truncate: Optional[int] = 70) -> str:
         if self.is_text():
-            return self.data.get("text", "")
+            return rich_escape(self.data.get("text", ""), escape_comma=False)
+
+        truncate_func = partial(trunc, length=truncate) if truncate else lambda x: x
 
         params = ", ".join(
-            [f"{k}={truncate(str(v))}" for k, v in self.data.items() if v is not None]
+            f"{k}={rich_escape(truncate_func(str(v)))}"
+            for k, v in self.data.items()
+            if v is not None
         )
         return f"[{self.type}{':' if params else ''}{params}]"
 
     @overrides(BaseMessageSegment)
     def is_text(self) -> bool:
         return self.type == "text"
 
@@ -101,16 +103,16 @@
 
 class Message(BaseMessage[MessageSegment]):
     @classmethod
     @overrides(BaseMessage)
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
-    def __repr__(self) -> str:
-        return "".join(repr(seg) for seg in self)
+    def to_rich_text(self, truncate: Optional[int] = 70) -> str:
+        return "".join(seg.to_rich_text(truncate=truncate) for seg in self)
 
     @staticmethod
     @overrides(BaseMessage)
     def _construct(msg: str) -> Iterable[MessageSegment]:
         yield MessageSegment.text(msg)
 
     @overrides(BaseMessage)
```

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/permission.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/nonebot/adapters/onebot/v12/utils.py` & `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.2/pyproject.toml` & `nonebot_adapter_onebot-2.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-onebot"
-version = "2.2.2"
+version = "2.2.3"
 description = "OneBot(CQHTTP) adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://adapter-onebot.netlify.app/"
 repository = "https://github.com/nonebot/adapter-onebot"
 documentation = "https://adapter-onebot.netlify.app/"
@@ -22,21 +22,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 msgpack = "^1.0.3"
 nonebot2 = "^2.0.0-beta.3"
 
 [tool.poetry.group.dev.dependencies]
+pycln = "^2.1.3"
 isort = "^5.10.1"
-black = "^22.1.0"
+black = "^23.1.0"
 nonebug = "^0.3.0"
 nonemoji = "^0.1.2"
 pytest-cov = "^4.0.0"
-pre-commit = "^2.19.0"
-pytest-asyncio = "^0.20.0"
+pre-commit = "^3.2.0"
+pytest-asyncio = "^0.21.0"
 nb-autodoc = "^1.0.0a5"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = ["fastapi"] }
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = "--cov nonebot.adapters.onebot --cov-report term-missing"
 
@@ -51,10 +52,14 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_adapter_onebot-2.2.2/PKG-INFO` & `nonebot_adapter_onebot-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-onebot
-Version: 2.2.2
+Version: 2.2.3
 Summary: OneBot(CQHTTP) adapter for nonebot2
 Home-page: https://adapter-onebot.netlify.app/
 License: MIT
 Keywords: bot,qq,qqbot,coolq,onebot,cqhttp
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-onebot Version: 2.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-onebot Version: 2.2.3 Summary:
 OneBot(CQHTTP) adapter for nonebot2 Home-page: https://adapter-
 onebot.netlify.app/ License: MIT Keywords: bot,qq,qqbot,coolq,onebot,cqhttp
 Author: yanyongyu Author-email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Robot Framework Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

