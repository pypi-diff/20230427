# Comparing `tmp/tabdoc-1.0.0b9-py3-none-any.whl.zip` & `tmp/tabdoc-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,12 @@
-Zip file size: 5307757 bytes, number of entries: 12
--rw-r--r--  2.0 unx      207 b- defN 19-Oct-09 08:51 tabdoc/__init__.py
--rw-r--r--  2.0 unx     8098 b- defN 19-Nov-18 15:49 tabdoc/tabexcel.py
+Zip file size: 11691 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      205 b- defN 23-Apr-27 16:34 tabdoc/__init__.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Apr-27 17:15 tabdoc/tabexcel.py
 -rw-r--r--  2.0 unx    10330 b- defN 19-Oct-15 10:31 tabdoc/tabpdf.py
--rw-r--r--  2.0 unx     8020 b- defN 19-Mar-20 16:14 tabdoc/tabword.py
--rw-r--r--  2.0 unx 10063973 b- defN 19-Feb-13 10:22 tabdoc/templates/SimHei.ttf
+-rw-r--r--  2.0 unx     8081 b- defN 23-Apr-27 17:14 tabdoc/tabword.py
 -rw-r--r--  2.0 unx      112 b- defN 19-Jul-25 12:59 tabdoc/templates/__init__.py
--rw-r--r--  2.0 unx    20235 b- defN 19-Feb-13 05:45 tabdoc/templates/template.docx
--rw-r--r--  2.0 unx     1066 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/LICENSE
--rw-r--r--  2.0 unx     1274 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      947 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/RECORD
-12 files, 10114361 bytes uncompressed, 5306187 bytes compressed:  47.5%
+-rw-r--r--  2.0 unx     1066 b- defN 23-Apr-27 17:31 tabdoc-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1272 b- defN 23-Apr-27 17:31 tabdoc-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 17:31 tabdoc-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-27 17:31 tabdoc-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      761 b- defN 23-Apr-27 17:31 tabdoc-1.0.1.dist-info/RECORD
+10 files, 29607 bytes uncompressed, 10407 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -6,32 +6,26 @@
 
 Filename: tabdoc/tabpdf.py
 Comment: 
 
 Filename: tabdoc/tabword.py
 Comment: 
 
-Filename: tabdoc/templates/SimHei.ttf
-Comment: 
-
 Filename: tabdoc/templates/__init__.py
 Comment: 
 
-Filename: tabdoc/templates/template.docx
-Comment: 
-
-Filename: tabdoc-1.0.0b9.dist-info/LICENSE
+Filename: tabdoc-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: tabdoc-1.0.0b9.dist-info/METADATA
+Filename: tabdoc-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tabdoc-1.0.0b9.dist-info/WHEEL
+Filename: tabdoc-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tabdoc-1.0.0b9.dist-info/top_level.txt
+Filename: tabdoc-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tabdoc-1.0.0b9.dist-info/RECORD
+Filename: tabdoc-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tabdoc/__init__.py

```diff
@@ -3,12 +3,12 @@
 
 """
 @author: guoyanfeng
 @software: PyCharm
 @time: 19-3-20 下午6:29
 """
 
-__version__ = "1.0.0b9"
+__version__ = "1.0.1"
 
 from .tabexcel import *
 from .tabpdf import *
 from .tabword import *
```

## tabdoc/tabexcel.py

```diff
@@ -10,15 +10,14 @@
 from io import BytesIO
 
 import tablib
 from openpyxl import Workbook
 from openpyxl.styles import Alignment, Border, Font, PatternFill, Side
 from openpyxl.utils import get_column_letter
 from path import Path
-from tablib.compat import unicode
 
 __all__ = ("ExcelWriter",)
 
 
 class ExcelWriter(object):
     """
     excel book writer
@@ -53,14 +52,15 @@
         Args:
 
         Returns:
 
         """
         self.save()
 
+    # noinspection DuplicatedCode
     @staticmethod
     def _reduce_datetimes(row):
         """Receives a row, converts datetimes to strings."""
 
         row = list(row)
 
         for i, val in enumerate(row):
@@ -177,38 +177,28 @@
                     cell_value: str = cell_value.get("value", '')
                     if cell_color:
                         cell.fill = PatternFill("solid", fgColor=cell_color.lstrip("# "))
                 cell.alignment = Alignment(wrap_text=True, horizontal=cell_horizontal, vertical=cell_vertical)
                 # 增加边框单线，这里是固定的
                 thin = Side(border_style="thin", color="000000")
                 cell.border = Border(top=thin, left=thin, right=thin, bottom=thin)
-
                 # bold headers
                 if (row_number == 1) and dataset.headers:
-                    # cell.value = unicode('%s' % col, errors='ignore')
-                    cell.value = unicode(cell_value)
+                    cell.value = str(cell_value)
                     cell.font = bold
                     if freeze_panes:
                         #  Export Freeze only after first Line
                         ws.freeze_panes = 'A2'
-
                 # bold separators
                 elif len(row) < dataset.width:
-                    cell.value = unicode('%s' % cell_value, errors='ignore')
+                    cell.value = str(cell_value)
                     cell.font = bold
-
                 # wrap the rest
                 else:
-                    try:
-                        if '\n' in cell_value:
-                            cell.value = unicode('%s' % cell_value, errors='ignore')
-                        else:
-                            cell.value = unicode('%s' % cell_value, errors='ignore')
-                    except TypeError:
-                        cell.value = unicode(cell_value)
+                    cell.value = str(cell_value.strip())
 
     def save(self, ):
         """
         保存工作簿
         Args:
         Returns:
```

## tabdoc/tabword.py

```diff
@@ -52,14 +52,15 @@
         Args:
 
         Returns:
 
         """
         self.save()
 
+    # noinspection DuplicatedCode
     @staticmethod
     def _reduce_datetimes(row):
         """Receives a row, converts datetimes to strings."""
 
         row = list(row)
 
         for i, val in enumerate(row):
@@ -199,15 +200,16 @@
             image_text: 针对图片的说明文字
         Returns:
 
         """
         p = self.document.add_paragraph(style="p-first-line-not-indent-center")
         p.alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
         run = p.add_run()
-        run.add_picture(image_path, width=Inches(5.8))
+        if image_path:
+            run.add_picture(image_path, width=Inches(5.8))
         bold_run = p.add_run(f"\n{image_text}")
         bold_run.font.size = Pt(12)
         bold_run.font.bold = True
 
     def save(self, ):
         """
         保存工作簿
```

## Comparing `tabdoc-1.0.0b9.dist-info/LICENSE` & `tabdoc-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tabdoc-1.0.0b9.dist-info/METADATA` & `tabdoc-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabdoc
-Version: 1.0.0b9
+Version: 1.0.1
 Summary: tabular datasets to excel,word,pdf
 Home-page: https://github.com/tinybees/tabdoc
 Author: TinyBees
 Author-email: a598824322@qq.com
 License: MIT
 Keywords: tabular,datasets,excel,word,pdf
 Platform: UNKNOWN
```

