# Comparing `tmp/rpa_cooperativa-1.0.45.tar.gz` & `tmp/rpa_cooperativa-1.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.45.tar", last modified: Mon Apr 24 14:20:46 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.46.tar", last modified: Thu Apr 27 12:44:56 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.45.tar` & `rpa_cooperativa-1.0.46.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:46.088781 rpa_cooperativa-1.0.45/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.45/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-04-24 14:20:46.077597 rpa_cooperativa-1.0.45/PKG-INFO
--rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.45/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:45.445193 rpa_cooperativa-1.0.45/rpa_coop/
--rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.45/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:45.846178 rpa_cooperativa-1.0.45/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.45/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.45/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.45/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.45/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.45/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    71299 2023-04-24 14:17:17.000000 rpa_cooperativa-1.0.45/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:46.054700 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-04-24 14:20:44.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 14:20:46.092352 rpa_cooperativa-1.0.45/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-04-24 14:20:34.000000 rpa_cooperativa-1.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.191722 rpa_cooperativa-1.0.46/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.46/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-04-27 12:44:56.189723 rpa_cooperativa-1.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.46/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:44:55.957647 rpa_cooperativa-1.0.46/rpa_coop/
+-rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.46/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.121074 rpa_cooperativa-1.0.46/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.46/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.46/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.46/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.46/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.46/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    71299 2023-04-24 14:17:17.000000 rpa_cooperativa-1.0.46/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.184727 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-04-27 12:44:55.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 12:44:56.193735 rpa_cooperativa-1.0.46/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-04-27 12:44:30.000000 rpa_cooperativa-1.0.46/setup.py
```

### Comparing `rpa_cooperativa-1.0.45/LICENSE` & `rpa_cooperativa-1.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/PKG-INFO` & `rpa_cooperativa-1.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.45
+Version: 1.0.46
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.45/README.md` & `rpa_cooperativa-1.0.46/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.46/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.46/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.46/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.46/rpa_coop/rpa_coop.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.45
+Version: 1.0.46
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 pymysql
 pyodbc
 sqlalchemy==1.4.37
 psycopg2
 psycopg2-binary
 denodo-sqlalchemy
 pillow
-requests==2.28.1
-urllib3==1.26.9
-certifi==2022.5.18.1
-pyopenssl==22.0.0
-idna==3.3
-charset-normalizer==2.0.12
+requests>=2.28.1
+urllib3>=1.26.9
+certifi>=2022.5.18.1
+pyopenssl>=22.0.0
+idna>=3.3
+charset-normalizer>=2.0.12
 pyautogui
 pyrect
 pyscreeze
 pytz
 graypy
 reportlab
 psutil
@@ -39,9 +39,9 @@
 pywinauto
 beautifulsoup4
 mechanize
 matplotlib
 Unidecode
 WMI
 tabulate
-python-dateutil==2.8.2
+python-dateutil>=2.8.2
 secure-smtplib
```

### Comparing `rpa_cooperativa-1.0.45/setup.py` & `rpa_cooperativa-1.0.46/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.45",
+    version="1.0.46",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
@@ -33,13 +33,13 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.8',
     install_requires=['wheel', 'pandas', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python==8.0.28',
-                      'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pillow', 'requests==2.28.1', 'urllib3==1.26.9', 
-                      'certifi==2022.5.18.1', 'pyopenssl==22.0.0', 'idna==3.3', 'charset-normalizer==2.0.12', 'pyautogui',
+                      'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pillow', 'requests>=2.28.1', 'urllib3>=1.26.9', 
+                      'certifi>=2022.5.18.1', 'pyopenssl>=22.0.0', 'idna>=3.3', 'charset-normalizer>=2.0.12', 'pyautogui',
                       'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'paramiko','opencv-python',
                       'pytesseract', 'xmltodict', 'pywin32', 'pywinauto', 'beautifulsoup4', 'mechanize', 'matplotlib', 
-                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil==2.8.2', 'secure-smtplib']
+                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil>=2.8.2', 'secure-smtplib']
 )
```

