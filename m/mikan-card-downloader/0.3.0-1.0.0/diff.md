# Comparing `tmp/mikan_card_downloader-0.3.0.tar.gz` & `tmp/mikan_card_downloader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-0.3.0.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.0.0.tar", max compression
```

## Comparing `mikan_card_downloader-0.3.0.tar` & `mikan_card_downloader-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.3.0/LICENSE
--rw-r--r--   0        0        0     1041 2023-04-23 22:20:01.579058 mikan_card_downloader-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.3.0/src/mikan/__init__.py
--rw-r--r--   0        0        0     1253 2023-04-23 14:42:49.133150 mikan_card_downloader-0.3.0/src/mikan/classes.py
--rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-0.3.0/src/mikan/config.py
--rw-r--r--   0        0        0     4518 2023-04-23 20:47:08.508195 mikan_card_downloader-0.3.0/src/mikan/downloader.py
--rw-r--r--   0        0        0     5802 2023-04-23 15:20:19.047035 mikan_card_downloader-0.3.0/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-0.3.0/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2149 2023-04-23 20:44:25.688821 mikan_card_downloader-0.3.0/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.3.0/src/mikan/py.typed
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.3.0/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1041 2023-04-26 22:38:39.384353 mikan_card_downloader-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.0.0/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1317 2023-04-26 16:41:23.873925 mikan_card_downloader-1.0.0/src/mikan/classes.py
+-rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-1.0.0/src/mikan/config.py
+-rw-r--r--   0        0        0     3209 2023-04-26 16:41:23.873925 mikan_card_downloader-1.0.0/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5958 2023-04-26 22:37:48.260144 mikan_card_downloader-1.0.0/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.0.0/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2217 2023-04-26 22:37:48.260144 mikan_card_downloader-1.0.0/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.0.0/src/mikan/py.typed
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-1.0.0/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.0.0/PKG-INFO
```

### Comparing `mikan_card_downloader-0.3.0/LICENSE` & `mikan_card_downloader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.3.0/pyproject.toml` & `mikan_card_downloader-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "0.3.0"
+version = "1.0.0"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-0.3.0/src/mikan/classes.py` & `mikan_card_downloader-1.0.0/src/mikan/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,12 +29,12 @@
     list_url_template: ClassVar = "https://idol.st/ajax/allstars/stills/?page="
     url_template: ClassVar = "https://idol.st/ajax/allstars/still/"
 
 
 @dataclass
 class SIFCard:
     results_dir: ClassVar = "SIF_Cards"
-    list_url_template: ClassVar = ""
-    url_template: ClassVar = ""
+    list_url_template: ClassVar = "https://schoolido.lu/api/cardids/"
+    url_template: ClassVar = "https://schoolido.lu/api/cards/"
 
 
 Item: TypeAlias = Card | Still | SIFCard
```

### Comparing `mikan_card_downloader-0.3.0/src/mikan/config.py` & `mikan_card_downloader-1.0.0/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.3.0/src/mikan/downloader.py` & `mikan_card_downloader-1.0.0/src/mikan/downloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 
 from __future__ import annotations
 
-import asyncio
 from pathlib import Path
 from typing import Any, Coroutine
 
 import aiohttp
 from tqdm.asyncio import tqdm
 
 import mikan.html_parser as parser
 from mikan import json_utils
-from mikan.classes import Item, SIFCard
+from mikan.classes import Item
 
 
 class Downloader:
     def __init__(self, data_path: Path, config_path: Path, img_type: type[Item]):
         self.base_path = data_path.expanduser()
         self.path = self.base_path / img_type.results_dir
         self.objs: dict[str, dict[str, list[str]]] = {}
@@ -37,25 +36,17 @@
         self.img_type = img_type
         self.objs[self.img_type.results_dir] = {}
 
         self.session = aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None))
 
         json_utils.load_cards(self.objs, self.config_path)
 
-        self.list_parser: parser.ListParser | parser.SIFListParser = (
-            parser.ListParser(self.img_type)
-            if self.img_type != SIFCard
-            else parser.SIFListParser()
-        )
-        self.item_parser = getattr(parser, f"{img_type.__name__}Parser")()
+        self.parser = parser.Parser(self.objs, self.img_type, self.session)
 
     async def __aenter__(self) -> Downloader:
-        self.list_parser.set_session(self.session)
-        self.item_parser.set_session(self.session)
-
         return self
 
     async def __aexit__(self, ext_type: None, value: None, trace: None) -> None:
         await self.session.close()
 
     async def download_file(self, item: str) -> None:
         try:
@@ -70,41 +61,14 @@
                 message = f"Downloaded item {self.get_card_image_name(item)}."
 
         except aiohttp.ClientError as e:
             message = f"Couldn't download item {item}: {e}"
 
         tqdm.write(message)
 
-    async def add_item_to_object_list(self, item: int) -> None:
-        i, obj = await self.item_parser.get_item(item)
-        self.objs[self.img_type.results_dir][i] = obj
-        print(f"Getting item {i}.")
-
-    async def get_page(self, idx: int) -> list[None]:
-        tasks: list[Coroutine[Any, Any, None]] = []
-        page = await self.list_parser.get_page(idx)
-
-        for item in page:
-            if str(item) not in self.objs[self.img_type.results_dir]:
-                tasks.append(self.add_item_to_object_list(item))
-
-        res: list[None] = await asyncio.gather(*tasks, return_exceptions=False)
-
-        return res
-
-    async def get_cards_from_parser(self) -> None:
-        num_pages = await self.list_parser.get_num_pages() + 1
-        current_num = 1
-        for _ in range(1, num_pages):
-            current_page = await self.get_page(current_num)
-            if not current_page and self.img_type != SIFCard:
-                break
-
-            current_num += 1
-
     def get_card_image_name(self, url: str) -> str:
         return url.split("/")[-1]
 
     async def get(self) -> None:
         tasks: list[Coroutine[Any, Any, None]] = []
 
         for _, item in self.objs[self.img_type.results_dir].items():
@@ -116,15 +80,15 @@
                 ]
             )
 
         await tqdm.gather(*tasks, disable=len(tasks) == 0)
 
     async def update(self) -> None:
         print("Searching for new or missing items...")
-        await self.get_cards_from_parser()
+        await self.parser.get_cards_from_pages()
 
         self.update_json_file()
         print("Updated items database.")
 
     def update_json_file(self) -> None:
         self.objs[self.img_type.results_dir] = dict(
             sorted(self.objs[self.img_type.results_dir].items(), reverse=True)
```

### Comparing `mikan_card_downloader-0.3.0/src/mikan/html_parser.py` & `mikan_card_downloader-1.0.0/src/mikan/html_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,191 +10,171 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 
 from __future__ import annotations
 
+import asyncio
 import re
-from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Any, Coroutine
 
 import aiohttp
 import bs4
 
-from mikan.classes import Card, Item, Still
+from mikan.classes import Item, SIFCard, Still
 
 
 class ListParsingException(Exception):
     pass
 
 
 class ItemParsingException(Exception):
     pass
 
 
-class NoHTTPSessionException(Exception):
-    pass
-
-
-class Parser(ABC):
-    def __init__(self) -> None:
-        self.session: Optional[aiohttp.ClientSession] = None
-        self.soup: Optional[bs4.BeautifulSoup] = None
-
-    def set_session(self, session: aiohttp.ClientSession) -> None:
-        self.session = session
-
-    async def get_html(self, url: str) -> str:
-        if isinstance(self.session, aiohttp.ClientSession):
-            html = await self.session.get(url)
-            return await html.text()
-
-        raise NoHTTPSessionException()
-
-    async def soup_page(self, num: int) -> bs4.BeautifulSoup:
-        return bs4.BeautifulSoup(
-            await self.get_html(self.get_url(num)), features="lxml"
+class Parser:
+    def __init__(
+        self,
+        objs: dict[str, dict[str, list[str]]],
+        img_type: type[Item],
+        session: aiohttp.ClientSession,
+    ) -> None:
+        self.session: aiohttp.ClientSession = session
+        self.img_type = img_type
+        self.objs = objs
+
+        self.list_parser: ListParser | SIFListParser = ListParser()
+        self.item_parser: CardParser | StillParser | SIFCardParser = CardParser()
+
+        if self.img_type == SIFCard:
+            self.list_parser = SIFListParser()
+            self.item_parser = SIFCardParser()
+        elif self.img_type == Still:
+            self.item_parser = StillParser()
+
+    async def request_url_data(self, url: str) -> aiohttp.ClientResponse:
+        return await self.session.get(url)
+
+    async def get_page(self, idx: int) -> list[None]:
+        tasks: list[Coroutine[Any, Any, None]] = []
+        data = (
+            await self.request_url_data(f"{self.img_type.list_url_template}{idx}")
+            if self.img_type != SIFCard
+            else idx
         )
+        page = await self.list_parser.get_page(data)
 
-    async def get_item(self, num: int) -> tuple[str, list[str]]:
-        self.soup = await self.soup_page(num)
-
-        return await self.create_item(num)
-
-    @abstractmethod
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        pass
-
-    @abstractmethod
-    def get_url(self, num: int) -> str:
-        pass
+        for item in page:
+            if str(item) not in self.objs[self.img_type.results_dir]:
+                tasks.append(self.add_item_to_object_list(item))
+
+        res: list[None] = await asyncio.gather(*tasks, return_exceptions=False)
+
+        return res
+
+    async def get_cards_from_pages(self) -> None:
+        num_pages = (
+            await self.list_parser.get_num_pages(
+                await self.request_url_data(self.img_type.list_url_template)
+            )
+            + 1
+        )
+        current_num = 1
+        for _ in range(1, num_pages):
+            current_page = await self.get_page(current_num)
+            if not current_page and self.img_type != SIFCard:
+                break
+
+            current_num += 1
+
+    async def add_item_to_object_list(self, item: int) -> None:
+        i, obj = await self.item_parser.create_item(
+            await self.request_url_data(f"{self.img_type.url_template}{item}")
+        )
+        self.objs[self.img_type.results_dir][i] = obj
+        print(f"Getting item {i}.")
 
 
-class SIFListParser(Parser):
+class SIFListParser:
     def __init__(self) -> None:
         self.items: list[list[int]] = []
 
-    async def get_items(self) -> None:
-        if isinstance(self.session, aiohttp.ClientSession):
-            html = await self.session.get("https://schoolido.lu/api/cardids/")
-            json = await html.json()
-
-            self.items = [json[i : i + 10] for i in range(0, len(json), 10)]  # noqa
-        else:
-            raise ListParsingException()
-
-    async def get_page(self, num: int) -> list[int]:
+    async def get_page(self, num: Any) -> list[int]:
         return self.items[num - 1]
 
-    async def get_num_pages(self) -> int:
-        await self.get_items()
+    async def get_num_pages(self, data: aiohttp.ClientResponse) -> int:
+        json = await data.json()
+        self.items = [json[i : i + 10] for i in range(0, len(json), 10)]  # noqa
         return len(self.items)
 
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        pass
 
-    def get_url(self, num: int) -> str:
-        pass
+class SIFCardParser:
+    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+        json = await data.json()
+        return str(json["id"]), [
+            card for card in [json["card_image"], json["card_idolized_image"]] if card
+        ]
 
 
-class SIFCardParser(Parser):
-    def get_url(self, num: int) -> str:
-        pass
-
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        if isinstance(self.session, aiohttp.ClientSession):
-            html = await self.session.get(f"https://schoolido.lu/api/cards/{num}/")
-            json = await html.json()
-
-            return str(json["id"]), [
-                card
-                for card in [json["card_image"], json["card_idolized_image"]]
-                if card
-            ]
-        raise ItemParsingException()
-
-    async def get_item(self, num: int) -> tuple[str, list[str]]:
-        return await self.create_item(num)
-
-
-class ListParser(Parser):
-    def __init__(self, img_type: type[Item]):
-        super().__init__()
-        self.url = img_type.list_url_template
-
-    def get_url(self, num: int) -> str:
-        return f"{self.url}{num}"
-
-    async def get_page(self, num: int) -> list[int]:
+class ListParser:
+    async def get_page(self, data: Any) -> list[int]:
         nums: list[int] = []
         pattern = re.compile(r"/(\d+)/")
 
-        page = await self.soup_page(num)
+        page = bs4.BeautifulSoup(await data.text(), features="lxml")
         items = page.find_all(class_="top-item")
 
         for item in items:
             string = item.find("a").get("href")
             match = pattern.search(string)
             if match:
                 nums.append(int(match.group(1)))
 
         if nums:
             return sorted(nums, reverse=True)
 
-        raise ListParsingException()
+        raise ListParsingException("An error occured while getting a page.")
 
-    async def get_num_pages(self) -> int:
+    async def get_num_pages(self, data: aiohttp.ClientResponse) -> int:
         pattern = re.compile(r"=(\d+)")
-        page = await self.soup_page(1)
+        page = bs4.BeautifulSoup(await data.text(), features="lxml")
 
         if isinstance(item := page.find(class_="pagination"), bs4.Tag):
             links = item.find_all("a")
             string = links[-2].get("href")
 
             if match := pattern.search(string):
                 return int(match.group(1))
 
-        raise ListParsingException()
-
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        pass
-
+        raise ListParsingException("An error occured while getting number of pages.")
 
-class CardParser(Parser):
-    def get_url(self, num: int) -> str:
-        return f"{Card.url_template}{num}"
 
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        urls = self.get_item_image_urls()
-        return str(num), [urls[0], urls[1]]
+class CardParser:
+    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+        page = bs4.BeautifulSoup(await data.text(), features="lxml")
+        pattern = re.compile(r"(\d+)")
 
-    def get_item_image_urls(self) -> tuple[str, str]:
-        if self.soup and isinstance(
-            top_item := self.soup.find(class_="top-item"), bs4.Tag
-        ):
+        if isinstance(top_item := page.find(class_="top-item"), bs4.Tag):
             links = top_item.find_all("a")
             first: str = links[0].get("href")
             second: str = links[1].get("href")
 
-            return (first, second)
+            if match := pattern.search(first.split("/")[-1]):
+                return match.group(1), [first, second]
 
-        raise ItemParsingException()
+        raise ItemParsingException("An error occured while getting a card.")
 
 
-class StillParser(Parser):
-    def get_url(self, num: int) -> str:
-        return f"{Still.url_template}{num}"
+class StillParser:
+    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+        page = bs4.BeautifulSoup(await data.text(), features="lxml")
+        pattern = re.compile(r"(\d+)")
 
-    async def create_item(self, num: int) -> tuple[str, list[str]]:
-        url = self.get_item_image_url()
-        return str(num), [url]
-
-    def get_item_image_url(self) -> str:
-        if self.soup and isinstance(
-            top_item := self.soup.find(class_="top-item"), bs4.Tag
-        ):
+        if isinstance(top_item := page.find(class_="top-item"), bs4.Tag):
             links = top_item.find_all("a")
-            if isinstance(link := links[0].get("href"), str):
-                return link
+            url: str = links[0].get("href")
+
+            if match := pattern.search(url.split("/")[-1]):
+                return match.group(1), [url]
 
-        raise ItemParsingException()
+        raise ItemParsingException("An error occured while getting a still.")
```

### Comparing `mikan_card_downloader-0.3.0/src/mikan/json_utils.py` & `mikan_card_downloader-1.0.0/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.3.0/src/mikan/main.py` & `mikan_card_downloader-1.0.0/src/mikan/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,13 +63,15 @@
         await downloader.update()
         await downloader.get()
 
 
 def main() -> None:  # pragma: no cover
     if sys.platform.startswith("win"):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-
-    asyncio.run(run())
+    try:
+        asyncio.run(run())
+    except Exception as e:
+        print(f"Error: {e}")
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `mikan_card_downloader-0.3.0/setup.py` & `mikan_card_downloader-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tqdm>=4.64.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['mikan = mikan.main:main']}
 
 setup_kwargs = {
     'name': 'mikan-card-downloader',
-    'version': '0.3.0',
+    'version': '1.0.0',
     'description': 'Downloads cards and stills from SIFAS and SIF.',
     'long_description': 'None',
     'author': 'DemonicSavage',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

