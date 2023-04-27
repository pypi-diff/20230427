# Comparing `tmp/html2notion-0.1.4.tar.gz` & `tmp/html2notion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.4.tar", last modified: Mon Apr 24 05:22:51 2023, max compression
+gzip compressed data, was "html2notion-0.1.5.tar", last modified: Thu Apr 27 02:04:10 2023, max compression
```

## Comparing `html2notion-0.1.4.tar` & `html2notion-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.113231 html2notion-0.1.4/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.4/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-24 05:22:51.113409 html2notion-0.1.4/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.4/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.097775 html2notion-0.1.4/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.4/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.4/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.106635 html2notion-0.1.4/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.4/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.4/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.4/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2689 2023-04-23 06:05:09.000000 html2notion-0.1.4/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7936 2023-04-24 05:22:27.000000 html2notion-0.1.4/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.4/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    10540 2023-04-24 05:22:27.000000 html2notion-0.1.4/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.4/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2389 2023-04-23 05:23:44.000000 html2notion-0.1.4/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.109650 html2notion-0.1.4/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.4/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.4/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.4/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.4/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.100459 html2notion-0.1.4/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      875 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.4/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-24 05:22:51.114083 html2notion-0.1.4/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.4/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.112729 html2notion-0.1.4/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.4/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.4/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.4/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    17438 2023-04-24 05:22:27.000000 html2notion-0.1.4/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.991210 html2notion-0.1.5/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.5/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-27 02:04:10.991558 html2notion-0.1.5/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.5/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.965782 html2notion-0.1.5/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.5/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.5/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.982001 html2notion-0.1.5/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.5/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.5/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.5/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3662 2023-04-24 06:00:38.000000 html2notion-0.1.5/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    10927 2023-04-27 01:54:11.000000 html2notion-0.1.5/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1452 2023-04-24 05:58:55.000000 html2notion-0.1.5/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.5/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    12779 2023-04-27 01:55:39.000000 html2notion-0.1.5/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.5/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2389 2023-04-27 01:51:59.000000 html2notion-0.1.5/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.986174 html2notion-0.1.5/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.5/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.5/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.5/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.5/html2notion/utils/timeutil.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.969416 html2notion-0.1.5/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      918 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-27 02:04:10.000000 html2notion-0.1.5/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.5/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-27 02:04:10.992579 html2notion-0.1.5/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.5/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-27 02:04:10.990591 html2notion-0.1.5/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.5/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.5/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.5/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    31656 2023-04-27 02:03:06.000000 html2notion-0.1.5/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.4/LICENSE` & `html2notion-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/PKG-INFO` & `html2notion-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.4/README.md` & `html2notion-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/main.py` & `html2notion-0.1.5/html2notion/main.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/translate/batch_import.py` & `html2notion-0.1.5/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/translate/cos_uploader.py` & `html2notion-0.1.5/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/translate/html2json.py` & `html2notion-0.1.5/html2notion/translate/html2json.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import singledispatch
 from pathlib import Path
 from bs4 import BeautifulSoup, Tag
 from ..utils import logger, test_prepare_conf
 from ..translate.html2json_base import Html2JsonBase
 from ..translate.html2json_default import Default_Type
 from ..translate.html2json_yinxiang import YinXiang_Type
+from ..translate.html2json_clipper import YinXiangClipper_Type
 
 
 """
 <meta name="source" content="yinxiang.superNote"/>
 <meta name="source" content="desktop.mac"/>
 """
 def _is_yinxiang_export_html(html_soup):
@@ -18,26 +19,45 @@
     meta_source = html_soup.select_one('html > head > meta[name="source"]')
     exporter_version_content = exporter_version_meta.get( 'content', "") if isinstance(exporter_version_meta, Tag) else ""
 
     meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
     if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
         return False
 
-    yinxiang_source_content = ["yinxiang", "desktop"]
+    yinxiang_source_content = ["yinxiang", "desktop", "web"]
     for prefix in yinxiang_source_content:
         if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
             return True
     return False
 
 
+"""
+<meta name="source-application" content="webclipper.evernote" />
+"""
+def _is_yinxiang_clipper_html(html_soup):
+    exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
+    exporter_version_content = exporter_version_meta.get(
+        'content', "") if isinstance(
+        exporter_version_meta, Tag) else ""
+
+    if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
+        return False
+    clipper_source_meta = html_soup.select_one('html > head > meta[name="source-application"]')
+    clipper_source_content = clipper_source_meta.get('content', "") if isinstance(clipper_source_meta, Tag) else ""
+    if isinstance(clipper_source_content, str) and clipper_source_content.endswith("evernote"):
+        return True
+    return False
+
+
 def _infer_input_type(html_content):
     soup = BeautifulSoup(html_content, 'html.parser')
     if _is_yinxiang_export_html(soup):
         return YinXiang_Type
-
+    elif _is_yinxiang_clipper_html(soup):
+        return YinXiangClipper_Type
     return Default_Type
 
 
 def _get_converter(html_content):
     html_type = _infer_input_type(html_content)
     logger.info(f"Input type: {html_type}")
     converter = Html2JsonBase.create(html_type, html_content)
@@ -68,15 +88,15 @@
     converter = _get_converter(html_content)
     result = converter.process()
     return converter.get_notion_data(), result
 
 
 if __name__ == "__main__":
     test_prepare_conf()
-    html_file = Path("./demos/Test Case C.html")
+    html_file = Path("./demos/Test Case D.html")
     result, html_type = html2json_process(html_file)
     print(html_type)
     print(json.dumps(result, indent=4, ensure_ascii=False))
     result2, html_type2 = html2json_process(
         "<html><body><div>test</div></body></html>")
     print(html_type2)
     print(json.dumps(result2, indent=4, ensure_ascii=False))
```

### Comparing `html2notion-0.1.4/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.5/html2notion/translate/html2json_yinxiang.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,61 +61,68 @@
             "object": "block",
             "type": "paragraph",
             "paragraph": {
                 "rich_text": []
             }
         }
         rich_text = json_obj["paragraph"]["rich_text"]
-        tag_text = soup.text if soup.text else ""
-        text_obj = self.parse_inline_block(soup)
+        text_obj = self.generate_inline_obj(soup)
         if text_obj:
             rich_text.extend(text_obj)
         return json_obj
 
+    def convert_divider(self, soup):
+        return {
+            "object": "block",
+            "type": "divider",
+            "divider": {}
+        }
+    
     def convert_heading(self, soup):
         heading_map = {"h1": "heading_1", "h2": "heading_2", "h3": "heading_3",
                        "h4": "heading_3", "h5": "heading_3", "h6": "heading_3"}
 
         heading_level = heading_map.get(soup.name, "heading_3")
         json_obj = {
             "object": "block",
             "type": heading_level,
             heading_level: {
                 "rich_text": []
             }
         }
         rich_text = json_obj[heading_level]["rich_text"]
-        text_obj = self.parse_inline_block(soup)
+        text_obj = self.generate_inline_obj(soup)
         if text_obj:
             rich_text.extend(text_obj)
         return json_obj
     
     def convert_code(self, soup):
         json_obj = {
             "object": "block",
             "type": "code",
             "code": {
                 "rich_text": [],
                 "language": "plain text",
             },
         }
         rich_text = json_obj["code"]["rich_text"]
+
         children_list = list(soup.children) if isinstance(soup, Tag) else [soup]
         for index, child in enumerate(children_list):
             is_last_child = index == len(children_list) - 1
-            text_obj = self.parse_inline_block(child)
+            text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
                 rich_text.append(self.generate_text(plain_text='\n'))
         json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
 
-        style = soup.get('style') if soup.name else ""
+        style = soup.get('style', "") if soup.name else ""
         css_dict = {}
-        if style:
+        if isinstance(style, str):
             style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
             language = css_dict.get('--en-codeblockLanguage', 'plain text')
             json_obj["code"]["language"] = language
         
         return json_obj
     
@@ -133,28 +140,98 @@
             "object": "block",
             "type": "quote",
             "quote": {
                 "rich_text": []
             }
         }
         rich_text = json_obj["quote"]["rich_text"]
+
         children_list = list(soup.children)
         for index, child in enumerate(children_list):
             is_last_child = index == len(children_list) - 1
-            text_obj = self.parse_inline_block(child)
+            text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
                 rich_text.append(self.generate_text(plain_text='\n'))
 
         # Merge tags has same anotions
         logger.debug(f'before merge: {rich_text}')
         json_obj["quote"]["rich_text"] = self.merge_rich_text(rich_text)
         return json_obj
 
+    """
+    <div>
+    <div><br /></div>
+    <table> <tbody> <tr> <td> </td> </tr> </tbody>
+    <div><br /></div>
+    </div>
+    """
+    # ../examples/insert_table.ipynb
+    def convert_table(self, soup):
+        # logger.debug(f'Convert table: {soup}')
+        # Assert: only one table in table div
+        table_rows = []
+        tr_tags = soup.find_all('tr')
+        if not tr_tags:
+            logger.error(f"No tr found in {soup}")
+            return
+        
+        table_width = len(tr_tags[0].find_all('td'))
+        if table_width == 0:
+            logger.error(f"No td found in {soup}")
+            return
+        
+        for tr in tr_tags:
+            td_tags = tr.find_all('td')
+            one_row = {
+                "type": "table_row",
+                "table_row": {
+                    "cells": []
+                }
+            }
+            for td in td_tags:
+                col = Html2JsonBase.generate_inline_obj(td)
+                one_row["table_row"]["cells"].append(col)
+            table_rows.append(one_row)
+
+        table_obj = {
+            "table": {
+                "has_row_header": False,
+                "has_column_header": False,
+                "table_width": table_width,
+                "children": table_rows,
+            }
+        }
+        return table_obj
+
+    def convert_to_do(self, soup: Tag):
+        # Compatible with the situation where input is under li tag(super note).
+        li_tags = soup.find_all('li', recursive=True)
+        childs = li_tags if li_tags else [soup]
+        to_do_blocks = []
+        for child in childs:
+            json_obj = {
+                "object": "block",
+                "type": "to_do",
+                "to_do": {
+                    "rich_text": [],
+                    "checked": False
+                }
+            }
+            text = json_obj["to_do"]["rich_text"]
+            text_obj = self.generate_inline_obj(child)
+            if text_obj:
+                text.extend(text_obj)
+            input_tag = child.find('input')
+            if input_tag and isinstance(input_tag, Tag) and input_tag.get('checked', 'false') == 'true':
+                json_obj["to_do"]["checked"] = True
+            to_do_blocks.append(json_obj)
+        return to_do_blocks
+
     # <ol><li><div>first</div></li><li><div>second</div></li><li><div>third</div></li></ol>
     def convert_numbered_list_item(self, soup):
         return self.convert_list_items(soup, 'numbered_list_item')
 
     # <ul><li><div>itemA</div></li><li><div>itemB</div></li><li><div>itemC</div></li></ul>
     def convert_bulleted_list_item(self, soup):
         return self.convert_list_items(soup, 'bulleted_list_item')
@@ -181,18 +258,17 @@
             "object": "block",
             list_type: {
                 "rich_text": []
             },
             "type": list_type,
         }
         rich_text = json_obj[list_type]["rich_text"]
-        for child in soup.children:
-            text_obj = self.parse_inline_block(child)
-            if text_obj:
-                rich_text.extend(text_obj)
+        text_obj = Html2JsonBase.generate_inline_obj(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
 
         return json_obj
 
     def _recursive_parse_style(self, tag_soup, tag_text, text_params):
         tag_name = tag_soup.name.lower() if tag_soup.name else ""
         style = tag_soup.get('style') if tag_name else ""
         styles = {}
@@ -215,74 +291,68 @@
         if color != 'default':
             text_params["color"] = color
 
         if not tag_soup or isinstance(tag_soup, NavigableString):
             return
 
         for child in tag_soup.children:
-            logger.debug(f'Recursive, child: {child}, {child.name}')
             if isinstance(child, Tag):
                 self._recursive_parse_style(child, child.text, text_params)
         return
 
-    # <b><u>unlineline and bold</u></b>
-    # <div><font color="#ff2600">Red color4</font></div>
-    # <div> Code in super note</div>
-    def parse_inline_block(self, tag_soup):
-        block_objs = []
-        all_tags = tag_soup.children if isinstance(tag_soup, Tag) else [tag_soup]
-        for child in all_tags:
-            text_params = {}
-            tag_name = child.name.lower() if child.name else ""
-            child_text = child.text if child.text else ""
- 
-            text_params["plain_text"] = child_text
-            if not isinstance(child, NavigableString):
-                self._recursive_parse_style(child, child_text, text_params)
-
-            text_obj = {}
-            if not isinstance(child, NavigableString) and tag_name == 'a':
-                href = child.get('href', "")
-                if not href:
-                    logger.warning("Link href is empty")
-                text_params["url"] = href
-                text_obj = self.generate_link(**text_params)
-            else:
-                text_obj = self.generate_text(**text_params)
-            logger.debug(f'parse_inline_block: {text_obj}')
-            if text_obj:
-                block_objs.append(text_obj)
-
-        return block_objs
-
     def get_block_type(self, single_tag):
         tag_name = single_tag.name
         style = single_tag.get('style') if tag_name else ""
 
-        if tag_name == 'ol':
+        # There are priorities here. It is possible to hit multiple targets 
+        # at the same time, and the first one takes precedence.
+        if self._check_is_todo(single_tag):
+            return Block.TO_DO.value
+        elif tag_name == 'hr':
+            return Block.DIVIDER.value
+        elif tag_name == 'ol':
             return Block.NUMBERED_LIST.value
         elif tag_name == 'ul':
             return Block.BULLETED_LIST.value
         elif tag_name == 'p':
             return Block.PARAGRAPH.value
         elif tag_name in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
             return Block.HEADING.value
+        elif tag_name == 'table' or self._check_is_table(single_tag):
+            return Block.TABLE.value
         if not style and tag_name == 'div':
             return Block.PARAGRAPH.value
 
         css_dict = {}
         if style:
             # Remove all space such as \t \n in style
             style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(
-                ':')[1].strip() for rule in style.split(';') if rule}
+                ':')[1].strip().lower() for rule in style.split(';') if rule}
         if css_dict.get('--en-blockquote', None) == 'true':
             return Block.QUOTE.value
         if css_dict.get('--en-codeblock', None) == 'true':
             return Block.CODE.value
         if css_dict.get('-en-codeblock', None) == 'true':
             return Block.CODE.value
         
         return Block.FAIL.value
 
+    def _check_is_table(self, tag):
+        if tag.name == "div":
+            children = list(filter(lambda x: x != '\n', tag.contents))
+            table_count = sum(1 for child in children if child.name == "table")
+            div_br_count = sum(1 for child in children if child.name == "div" and len(
+                child.contents) == 1 and child.contents[0].name == "br")
+
+            return table_count == 1 and div_br_count >= 2 and (table_count + div_br_count) == len(children)
+        return False
+
+    def _check_is_todo(self, tag):
+        if not isinstance(tag, Tag):
+            return False
+        input_tag = tag.find('input')
+        if input_tag and isinstance(input_tag, Tag) and input_tag.get('type') == 'checkbox':
+            return True
+        return False
 
 Html2JsonBase.register(YinXiang_Type, Html2JsonYinXiang)
```

### Comparing `html2notion-0.1.4/html2notion/translate/notion_export.py` & `html2notion-0.1.5/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/translate/notion_import.py` & `html2notion-0.1.5/html2notion/translate/notion_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/utils/load_config.py` & `html2notion-0.1.5/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion/utils/log.py` & `html2notion-0.1.5/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.5/html2notion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.4/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.5/html2notion.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 html2notion.egg-info/requires.txt
 html2notion.egg-info/top_level.txt
 html2notion/translate/__init__.py
 html2notion/translate/batch_import.py
 html2notion/translate/cos_uploader.py
 html2notion/translate/html2json.py
 html2notion/translate/html2json_base.py
+html2notion/translate/html2json_clipper.py
 html2notion/translate/html2json_default.py
 html2notion/translate/html2json_yinxiang.py
 html2notion/translate/notion_export.py
 html2notion/translate/notion_import.py
 html2notion/utils/__init__.py
 html2notion/utils/load_config.py
 html2notion/utils/log.py
```

### Comparing `html2notion-0.1.4/setup.cfg` & `html2notion-0.1.5/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.4
+version = 0.1.5
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.4/tests/test_batchimport.py` & `html2notion-0.1.5/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/tests/test_cosupload.py` & `html2notion-0.1.5/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.4/tests/test_notionexport.py` & `html2notion-0.1.5/tests/test_notionexport.py`

 * *Files identical despite different names*

