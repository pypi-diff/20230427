# Comparing `tmp/rapidocr_pdf-0.0.1-py3-none-any.whl.zip` & `tmp/rapidocr_pdf-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 6443 bytes, number of entries: 6
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2091 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-Apr-17 01:24 rapidocr_pdf-0.0.1.dist-info/RECORD
-6 files, 14117 bytes uncompressed, 5507 bytes compressed:  61.0%
+Zip file size: 8486 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      124 b- defN 23-Apr-27 02:38 rapidocr_pdf/__init__.py
+-rw-r--r--  2.0 unx     4090 b- defN 23-Apr-27 02:38 rapidocr_pdf/main.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2714 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      669 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/RECORD
+8 files, 19116 bytes uncompressed, 7310 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
-Filename: rapidocr_pdf-0.0.1.dist-info/LICENSE
+Filename: rapidocr_pdf/__init__.py
 Comment: 
 
-Filename: rapidocr_pdf-0.0.1.dist-info/METADATA
+Filename: rapidocr_pdf/main.py
 Comment: 
 
-Filename: rapidocr_pdf-0.0.1.dist-info/WHEEL
+Filename: rapidocr_pdf-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: rapidocr_pdf-0.0.1.dist-info/entry_points.txt
+Filename: rapidocr_pdf-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_pdf-0.0.1.dist-info/top_level.txt
+Filename: rapidocr_pdf-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_pdf-0.0.1.dist-info/RECORD
+Filename: rapidocr_pdf-0.0.2.dist-info/entry_points.txt
+Comment: 
+
+Filename: rapidocr_pdf-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: rapidocr_pdf-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapidocr_pdf-0.0.1.dist-info/LICENSE` & `rapidocr_pdf-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapidocr_pdf-0.0.1.dist-info/METADATA` & `rapidocr_pdf-0.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 Metadata-Version: 2.1
 Name: rapidocr-pdf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools of extracting PDF content based on RapidOCR
 Home-page: https://github.com/RapidAI/RapidOCRPDF
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino
 Platform: Any
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6,<=3.10
+Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: filetype
 Requires-Dist: pymupdf
 Provides-Extra: onnxruntime
 Requires-Dist: rapidocr-onnxruntime ; extra == 'onnxruntime'
 Provides-Extra: openvino
 Requires-Dist: rapidocr-openvino ; extra == 'openvino'
 
 ## RapidOCRPDF
 <p>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
+    <a href="https://pypi.org/project/rapidocr-pdf/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapidocr-pdf"></a>
+    <a href="https://pepy.tech/project/rapidocr-pdf"><img src="https://static.pepy.tech/personalized-badge/rapidocr-pdf?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
-- 依托于[RapidOCR](https://github.com/RapidAI/RapidOCR)仓库，快速提取PDF中文字，包括扫描版PDF、加密版PDF。
-- 暂不包括版式还原。
+- Relying on [RapidOCR](https://github.com/RapidAI/RapidOCR), quickly extract text from PDF, including scanned PDF and encrypted PDF.
+- Layout restore is not included for now.
 
-### 使用
-1. 安装`rapid_ocr_pdf`库
+
+### 1. Install package by pypi.
    ```bash
-   # 基于rapidocr_onnxruntime
-   pip install rapid_ocr_pdf[onnxruntime]
+   # base rapidocr_onnxruntime
+   pip install rapidocr_pdf[onnxruntime]
 
-   # 基于rapidocr_openvino
+   # base rapidocr_openvino
    pip install rapidocr_pdf[openvino]
    ```
-2. 使用方式
+
+### 2. Use
+- Run by script.
     ```python
     from rapidocr_pdf import PDFExtracter
 
     pdf_extracter = PDFExtracter()
 
     pdf_path = 'tests/test_files/direct_and_image.pdf'
     texts = pdf_extracter(pdf_path)
     print(texts)
     ```
-3. 输入输出说明
-   - **输入**：`Union[str, Path, bytes]`
-   - **输出**：`List` \[**页码**, **文本内容** + **置信度**\]， 具体参见下例：
+- Run by command line.
+    ```bash
+    $ rapidocr_pdf -h
+    usage: rapidocr_pdf [-h] [-path FILE_PATH]
+
+    options:
+    -h, --help            show this help message and exit
+    -path FILE_PATH, --file_path FILE_PATH
+                            File path, PDF or images
+
+    $ rapidocr_pdf -path tests/test_files/direct_and_image.pdf
+    ```
+### 3. Ouput format.
+   - **Input**：`Union[str, Path, bytes]`
+   - **Output**：`List` \[**Page num**, **Page content** + **score**\], ：
        ```python
        [
            ['0', '达大学拉斯维加斯分校）的一次中文评测中获得最', '0.8969868'],
            ['1', 'ABCNet: Real-time Scene Text Spotting with Adaptive Bezier-Curve Network∗\nYuliang Liu‡†', '0.8969868'],
        ]
        ```
```

### html2text {}

```diff
@@ -1,27 +1,32 @@
-Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.0.1 Summary: Tools of
+Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.0.2 Summary: Tools of
 extracting PDF content based on RapidOCR Home-page: https://github.com/RapidAI/
 RapidOCRPDF Author: SWHL Author-email: liekkaskono@163.com License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino Platform:
-Any Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.6,<=3.10 Description-Content-
-Type: text/markdown Requires-Dist: filetype Requires-Dist: pymupdf Provides-
-Extra: onnxruntime Requires-Dist: rapidocr-onnxruntime ; extra == 'onnxruntime'
-Provides-Extra: openvino Requires-Dist: rapidocr-openvino ; extra == 'openvino'
-## RapidOCRPDF
+Any Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Python:
+>=3.7,<=3.10 Description-Content-Type: text/markdown Requires-Dist: filetype
+Requires-Dist: pymupdf Provides-Extra: onnxruntime Requires-Dist: rapidocr-
+onnxruntime ; extra == 'onnxruntime' Provides-Extra: openvino Requires-Dist:
+rapidocr-openvino ; extra == 'openvino' ## RapidOCRPDF
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
-img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg]
-- ä¾æäº[RapidOCR](https://github.com/RapidAI/
-RapidOCR)ä»åºï¼å¿«éæåPDFä¸­æå­ï¼åæ¬æ«æçPDFãå å¯çPDFã
-- æä¸åæ¬çå¼è¿åã ### ä½¿ç¨ 1. å®è£`rapid_ocr_pdf`åº ```bash #
-åºäºrapidocr_onnxruntime pip install rapid_ocr_pdf[onnxruntime] #
-åºäºrapidocr_openvino pip install rapidocr_pdf[openvino] ``` 2. ä½¿ç¨æ¹å¼
-```python from rapidocr_pdf import PDFExtracter pdf_extracter = PDFExtracter()
-pdf_path = 'tests/test_files/direct_and_image.pdf' texts = pdf_extracter
-(pdf_path) print(texts) ``` 3. è¾å¥è¾åºè¯´æ - **è¾å¥**ï¼`Union[str,
-Path, bytes]` - **è¾åº**ï¼`List` \[**é¡µç **, **ææ¬åå®¹** +
-**ç½®ä¿¡åº¦**\]ï¼ å·ä½åè§ä¸ä¾ï¼ ```python [ ['0',
+img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
+static.pepy.tech/personalized-badge/rapidocr-
+pdf?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
+- Relying on [RapidOCR](https://github.com/RapidAI/RapidOCR), quickly extract
+text from PDF, including scanned PDF and encrypted PDF. - Layout restore is not
+included for now. ### 1. Install package by pypi. ```bash # base
+rapidocr_onnxruntime pip install rapidocr_pdf[onnxruntime] # base
+rapidocr_openvino pip install rapidocr_pdf[openvino] ``` ### 2. Use - Run by
+script. ```python from rapidocr_pdf import PDFExtracter pdf_extracter =
+PDFExtracter() pdf_path = 'tests/test_files/direct_and_image.pdf' texts =
+pdf_extracter(pdf_path) print(texts) ``` - Run by command line. ```bash $
+rapidocr_pdf -h usage: rapidocr_pdf [-h] [-path FILE_PATH] options: -h, --help
+show this help message and exit -path FILE_PATH, --file_path FILE_PATH File
+path, PDF or images $ rapidocr_pdf -path tests/test_files/direct_and_image.pdf
+``` ### 3. Ouput format. - **Input**ï¼`Union[str, Path, bytes]` -
+**Output**ï¼`List` \[**Page num**, **Page content** + **score**\], ï¼
+```python [ ['0',
 'è¾¾å¤§å­¦ææ¯ç»´å æ¯åæ ¡ï¼çä¸æ¬¡ä¸­æè¯æµä¸­è·å¾æ',
 '0.8969868'], ['1', 'ABCNet: Real-time Scene Text Spotting with Adaptive
 Bezier-Curve Networkâ\nYuliang Liuâ¡â ', '0.8969868'], ] ```
```

