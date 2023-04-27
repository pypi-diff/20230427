# Comparing `tmp/tabdoc-1.0.0b8-py3-none-any.whl.zip` & `tmp/tabdoc-1.0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5305927 bytes, number of entries: 12
--rw-r--r--  2.0 unx      207 b- defN 19-Jul-31 08:56 tabdoc/__init__.py
--rw-r--r--  2.0 unx     3498 b- defN 19-Jul-31 08:49 tabdoc/tabexcel.py
--rw-r--r--  2.0 unx     8528 b- defN 19-Jul-31 07:21 tabdoc/tabpdf.py
+Zip file size: 5307757 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      207 b- defN 19-Oct-09 08:51 tabdoc/__init__.py
+-rw-r--r--  2.0 unx     8098 b- defN 19-Nov-18 15:49 tabdoc/tabexcel.py
+-rw-r--r--  2.0 unx    10330 b- defN 19-Oct-15 10:31 tabdoc/tabpdf.py
 -rw-r--r--  2.0 unx     8020 b- defN 19-Mar-20 16:14 tabdoc/tabword.py
 -rw-r--r--  2.0 unx 10063973 b- defN 19-Feb-13 10:22 tabdoc/templates/SimHei.ttf
 -rw-r--r--  2.0 unx      112 b- defN 19-Jul-25 12:59 tabdoc/templates/__init__.py
 -rw-r--r--  2.0 unx    20235 b- defN 19-Feb-13 05:45 tabdoc/templates/template.docx
--rw-r--r--  2.0 unx     1066 b- defN 19-Jul-31 09:06 tabdoc-1.0.0b8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1274 b- defN 19-Jul-31 09:06 tabdoc-1.0.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Jul-31 09:06 tabdoc-1.0.0b8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 19-Jul-31 09:06 tabdoc-1.0.0b8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      946 b- defN 19-Jul-31 09:06 tabdoc-1.0.0b8.dist-info/RECORD
-12 files, 10107958 bytes uncompressed, 5304357 bytes compressed:  47.5%
+-rw-r--r--  2.0 unx     1066 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1274 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      947 b- defN 19-Nov-18 15:49 tabdoc-1.0.0b9.dist-info/RECORD
+12 files, 10114361 bytes uncompressed, 5306187 bytes compressed:  47.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tabdoc/templates/__init__.py
 Comment: 
 
 Filename: tabdoc/templates/template.docx
 Comment: 
 
-Filename: tabdoc-1.0.0b8.dist-info/LICENSE
+Filename: tabdoc-1.0.0b9.dist-info/LICENSE
 Comment: 
 
-Filename: tabdoc-1.0.0b8.dist-info/METADATA
+Filename: tabdoc-1.0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: tabdoc-1.0.0b8.dist-info/WHEEL
+Filename: tabdoc-1.0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: tabdoc-1.0.0b8.dist-info/top_level.txt
+Filename: tabdoc-1.0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: tabdoc-1.0.0b8.dist-info/RECORD
+Filename: tabdoc-1.0.0b9.dist-info/RECORD
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
 
-__version__ = "1.0.0b8"
+__version__ = "1.0.0b9"
 
 from .tabexcel import *
 from .tabpdf import *
 from .tabword import *
```

## tabdoc/tabexcel.py

```diff
@@ -3,17 +3,22 @@
 
 """
 @author: guoyanfeng
 @software: PyCharm
 @time: 19-2-11 下午6:14
 """
 from collections import Counter, MutableMapping, Sequence
+from io import BytesIO
 
 import tablib
+from openpyxl import Workbook
+from openpyxl.styles import Alignment, Border, Font, PatternFill, Side
+from openpyxl.utils import get_column_letter
 from path import Path
+from tablib.compat import unicode
 
 __all__ = ("ExcelWriter",)
 
 
 class ExcelWriter(object):
     """
     excel book writer
@@ -23,16 +28,17 @@
         """
             excel book writer
         Args:
             excel_path: excel path
             excel_name: excel 名称
         """
         self.excel_path = excel_path
-        self.excel_name = f"{excel_name}.xls"
+        self.excel_name = f"{excel_name}.xlsx"
         self.excel_book = tablib.Databook()
+        self.merge_cells_index = {}
         self.sheet_names = Counter()  # 多个sheet name的映射，防止名称重复造成错误
 
     def __enter__(self):
         """
 
         Args:
 
@@ -60,20 +66,21 @@
         for i, val in enumerate(row):
             if hasattr(val, "strftime"):
                 row[i] = val.strftime("%Y-%m-%d %H:%M:%S")
             elif hasattr(val, 'isoformat'):
                 row[i] = val.isoformat()
         return tuple(row)
 
-    def add_sheet(self, sheet_name, sheet_data: list):
+    def add_sheet(self, sheet_name, sheet_data: list, merge_cells=None):
         """
         为excel添加工作表
         Args:
             sheet_name: 工作表的名称
             sheet_data: 工作表的数据， 必须是列表中嵌套元祖、列表或者字典（从records查询出来的数据库的数据）
+            merge_cells: 要合并的单元格的索引, [(start_row, start_column, end_row, end_column)],最小值从1开始
         Returns:
 
         """
         sheet_data = sheet_data if sheet_data else [{}]
         #  处理sheet name可能出现重复的情况
         self.sheet_names[sheet_name] += 1
         sheet_name = sheet_name if self.sheet_names[sheet_name] == 1 else f"{sheet_name}{self.sheet_names[sheet_name]}"
@@ -103,22 +110,113 @@
         else:
             excel_sheet.headers = first
             for row in sheet_data[1:]:
                 row = self._reduce_datetimes(row)
                 excel_sheet.append(row)
 
         self.excel_book.add_sheet(excel_sheet)
+        if merge_cells:
+            verify_cells_index = []
+            for val in merge_cells:
+                verify_cells_index.extend(val)
+            if min(verify_cells_index) < 1:
+                raise ValueError("Min value is 1")
+            self.merge_cells_index[sheet_name] = merge_cells
+
+    # noinspection PyProtectedMember
+    def export_book(self, freeze_panes=True):
+        """Returns XLSX representation of DataBook."""
+
+        wb = Workbook()
+        for sheet in wb.worksheets:
+            wb.remove(sheet)
+        for i, dset in enumerate(self.excel_book._datasets):
+            ws = wb.create_sheet()
+            ws.title = dset.title if dset.title else 'Sheet%s' % i
+            self.dset_sheet(dset, ws, freeze_panes=freeze_panes)
+            # 合并单元格
+            if ws.title in self.merge_cells_index:
+                for ws_row_col in self.merge_cells_index[ws.title]:
+                    ws.merge_cells(start_row=ws_row_col[0], start_column=ws_row_col[1], end_row=ws_row_col[2],
+                                   end_column=ws_row_col[3])
+                    ws._get_cell(ws_row_col[0], ws_row_col[1]).alignment = Alignment(
+                        horizontal="center", vertical="center", wrap_text=True)
+        stream = BytesIO()
+        wb.save(stream)
+        return stream.getvalue()
+
+    # noinspection PyProtectedMember
+    @staticmethod
+    def dset_sheet(dataset, ws, freeze_panes=True):
+        """Completes given worksheet from given Dataset."""
+        _package = dataset._package(dicts=False)
+
+        for i, sep in enumerate(dataset._separators):
+            _offset = i
+            _package.insert((sep[0] + _offset), (sep[1],))
+
+        bold = Font(bold=True)
+
+        for i, row in enumerate(_package):
+            row_number = i + 1
+            for j, cell_value in enumerate(row):
+                col_idx = get_column_letter(j + 1)
+                cell = ws['%s%s' % (col_idx, row_number)]
+                cell_horizontal, cell_vertical = None, None
+                if isinstance(cell_value, dict):
+                    cell_color: str = cell_value.get("color", None)
+                    # 处理水平居中
+                    cell_horizontal: str = cell_value.get("horizontal", None)
+                    if cell_horizontal and cell_horizontal not in ("general", "left", "center", "right"):
+                        cell_horizontal = "general"  # 默认对其方式
+
+                    # 处理垂直居中
+                    cell_vertical: str = cell_value.get("vertical", None)
+                    if cell_vertical and cell_vertical not in ("top", "center", "bottom"):
+                        cell_vertical = "center"  # 默认对其方式
+
+                    cell_value: str = cell_value.get("value", '')
+                    if cell_color:
+                        cell.fill = PatternFill("solid", fgColor=cell_color.lstrip("# "))
+                cell.alignment = Alignment(wrap_text=True, horizontal=cell_horizontal, vertical=cell_vertical)
+                # 增加边框单线，这里是固定的
+                thin = Side(border_style="thin", color="000000")
+                cell.border = Border(top=thin, left=thin, right=thin, bottom=thin)
+
+                # bold headers
+                if (row_number == 1) and dataset.headers:
+                    # cell.value = unicode('%s' % col, errors='ignore')
+                    cell.value = unicode(cell_value)
+                    cell.font = bold
+                    if freeze_panes:
+                        #  Export Freeze only after first Line
+                        ws.freeze_panes = 'A2'
+
+                # bold separators
+                elif len(row) < dataset.width:
+                    cell.value = unicode('%s' % cell_value, errors='ignore')
+                    cell.font = bold
+
+                # wrap the rest
+                else:
+                    try:
+                        if '\n' in cell_value:
+                            cell.value = unicode('%s' % cell_value, errors='ignore')
+                        else:
+                            cell.value = unicode('%s' % cell_value, errors='ignore')
+                    except TypeError:
+                        cell.value = unicode(cell_value)
 
     def save(self, ):
         """
         保存工作簿
         Args:
         Returns:
 
         """
         if self.excel_path is None:
             file_path = self.excel_name
         else:
             file_path = Path(self.excel_path).joinpath(self.excel_name).abspath()
 
         with open(file_path, "wb") as f:
-            f.write(self.excel_book.export("xls"))
+            f.write(self.export_book())
```

## tabdoc/tabpdf.py

```diff
@@ -12,26 +12,46 @@
 from reportlab.lib import colors
 from reportlab.lib.fonts import addMapping
 from reportlab.lib.pagesizes import letter
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.lib.units import inch
 from reportlab.pdfbase import pdfmetrics
 from reportlab.pdfbase.ttfonts import TTFont
-from reportlab.platypus import Paragraph, SimpleDocTemplate, Spacer, Table, TableStyle
+from reportlab.platypus import PageBreak, Paragraph, SimpleDocTemplate, Spacer, Table, TableStyle
 
 __all__ = ("PDFWriter",)
 
 pdfmetrics.registerFont(
     TTFont('simhei', Path(__file__).dirname().joinpath("templates/SimHei.ttf").abspath()))
 addMapping('simhei', 0, 0, 'simhei')  # normal
 addMapping('simhei', 0, 1, 'simhei_italic')  # italic
 addMapping('simhei', 1, 0, 'simhei_bold')  # bold
 addMapping('simhei', 1, 1, 'simhei_boldItalic')  # italic and bold
 
 
+class RotateTable(Table):  # Table Rotate
+
+    def draw(self):
+        #  获取当前的基准Y点
+        current_y = vars(self.canv)["_currentMatrix"][-1]
+        #  这里移动x点以左边界为基准向右移动, 文档的宽度-表格的高度-边界距离
+        #  这里移动y点以上边界为基准向上移动,文档的高度-当前y点-边界距离，就是要向上移动的距离
+        self.canv.translate(letter[0] - sum(self._rowHeights) - inch, letter[1] - current_y - inch)
+        self.canv.rotate(-90)
+        super().draw()
+
+
+class RotateParagraph(Paragraph):  # Table Rotate
+
+    def draw(self):
+        self.canv.translate(letter[0] - 2 * inch, 0)
+        self.canv.rotate(-90)
+        super().draw()
+
+
 class PDFWriter(object):
     """
     pdf book writer
     """
 
     def __init__(self, pdf_name, pdf_path=None, water_mark="", title=None):
         """
@@ -143,35 +163,40 @@
         if alignment not in self.alignment_map:
             raise ValueError("alignment必须是left,center,right,justify")
         styles = self.styles.get('Normal')
         styles.alignment = self.alignment_map[alignment]
         self.story.append(Paragraph(paragraph_text, styles))
         self.story.append(Spacer(1, 0.15 * inch))
 
-    def add_table(self, table_data: list, table_name=None, data_align='CENTER', table_halign='CENTER'):
+    def add_table(self, table_data: list, table_name=None, data_align='CENTER', table_halign='CENTER',
+                  cell_styles: list = None, is_landscape=False):
         """
         为pdf添加表格数据
         Args:
             table_name: 表格的名称
             table_data: 表格的数据， 必须是列表中嵌套元祖、列表或者字典（从records查询出来的数据库的数据）
             data_align: The alignment of the data inside the table (eg.
                 'LEFT', 'CENTER', 'RIGHT')
             table_halign: Horizontal alignment of the table on the page
                 (eg. 'LEFT', 'CENTER', 'RIGHT')
-
+            cell_styles: 每个单元格样式
+            is_landscape: 是否横向展示，默认false
         Returns:
 
         """
         table_data = table_data if table_data else [[""]]
-        
+        self.story.append(PageBreak())
         if table_name:
             styles = self.styles.get('Heading4')
             styles.alignment = self.alignment_map.get(table_halign.lower(), "center")
-            self.story.append(Paragraph(table_name, styles))
-            self.story.append(Spacer(1, 0.15 * inch))
+            if is_landscape:
+                self.story.append(RotateParagraph(table_name, styles))
+            else:
+                self.story.append(Paragraph(table_name, styles))
+            # self.story.append(Spacer(1, 0.15 * inch)) # 这里是增加间距，测试后发现去掉更美观点
 
         for index, row in enumerate(table_data):
             if not isinstance(row, (MutableMapping, Sequence)):
                 raise ValueError("table_data值数据类型错误,请检查")
             table_data[index] = row[:36]  # 解决超过36列行高大于一页而报错的问题
 
         # 处理list或者tuple个别长度不一致的情况
@@ -196,40 +221,53 @@
                     table_data[index] = self._reduce_datetimes(row.values())
         cell_styles = self.styles["Normal"]
         for row_index, row in enumerate(table_data):
             for column_index, one_value in enumerate(row):
                 table_data[row_index][column_index] = Paragraph(str(one_value) if one_value else "", cell_styles)
 
         # 第一列的宽度是其他列的两倍,第二列的宽度是其他列的1.5倍
-        column_len, column_width_per = len(table_data[-1]), self.document.width / (len(table_data[-1]) + 2)
+        if is_landscape:
+            column_len, column_width_per = len(table_data[-1]), (letter[1] - 2 * inch) / (len(table_data[-1]) + 2)
+        else:
+            column_len, column_width_per = len(table_data[-1]), self.document.width / (len(table_data[-1]) + 2)
+
         column_width = [column_width_per * 2, column_width_per * 1.5,
                         *[column_width_per for _ in range(column_len - 2)]]
-        table = Table(table_data, hAlign=table_halign, colWidths=column_width)
+        if is_landscape:
+            table = RotateTable(table_data, hAlign=table_halign, colWidths=column_width)
+        else:
+            table = Table(table_data, hAlign=table_halign, colWidths=column_width)
         # (列,行) (0, 0)(-1, -1)代表0列0行到所有的单元格
-        table.setStyle(TableStyle([('FONT', (0, 0), (-1, -1), 'simhei'),  # 所有单元格设置雅黑字体
-                                   ('ALIGN', (0, 0), (-1, 0), 'LEFT'),  # 第一列左对齐
-                                   ('ALIGN', (0, 0), (0, 0), data_align),  # 第一个单元格
-                                   ('ALIGN', (1, 0), (-1, -1), data_align),  # 第一列到剩下的所有数据
-                                   ('INNERGRID', (0, 0), (-1, -1), 0.50, colors.black),
-                                   ('BOX', (0, 0), (-1, -1), 0.25, colors.black)]))
+        if not cell_styles:
+            table_style = TableStyle([('FONT', (0, 0), (-1, -1), 'simhei'),  # 所有单元格设置雅黑字体
+                                      ('ALIGN', (0, 0), (-1, 0), 'LEFT'),  # 第一列左对齐
+                                      ('ALIGN', (0, 0), (0, 0), data_align),  # 第一个单元格
+                                      ('ALIGN', (1, 0), (-1, -1), data_align),  # 第一列到剩下的所有数据
+                                      ('INNERGRID', (0, 0), (-1, -1), 0.50, colors.black),
+                                      ('BOX', (0, 0), (-1, -1), 0.25, colors.black)])
+        else:
+            table_style = TableStyle([('FONT', (0, 0), (-1, -1), 'simhei'),  # 所有单元格设置雅黑字体
+                                      ('INNERGRID', (0, 0), (-1, -1), 0.50, colors.black),
+                                      ('BOX', (0, 0), (-1, -1), 0.25, colors.black)])
 
+        table.setStyle(table_style)
         self.story.append(table)
 
     @staticmethod
     def on_pages_setup(canvas, doc):
         """
         为每页增加水印，或者其他的logo等
         Args:
 
         Returns:
 
         """
         canvas.saveState()
 
-        canvas.setFont("simhei", 120)
+        canvas.setFont("simhei", 60)
         canvas.rotate(30)  # 旋转30度
         canvas.setFillAlpha(0.1)  # 设置透明度
         canvas.setFillGray(0.50)  # 设置灰度
         canvas.drawCentredString(6.5 * inch, 3.75 * inch, doc.water_mark)
 
         canvas.restoreState()
```

## Comparing `tabdoc-1.0.0b8.dist-info/LICENSE` & `tabdoc-1.0.0b9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tabdoc-1.0.0b8.dist-info/METADATA` & `tabdoc-1.0.0b9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabdoc
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: tabular datasets to excel,word,pdf
 Home-page: https://github.com/tinybees/tabdoc
 Author: TinyBees
 Author-email: a598824322@qq.com
 License: MIT
 Keywords: tabular,datasets,excel,word,pdf
 Platform: UNKNOWN
```

