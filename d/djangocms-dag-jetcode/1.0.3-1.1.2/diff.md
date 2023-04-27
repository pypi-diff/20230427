# Comparing `tmp/djangocms_dag_jetcode-1.0.3.tar.gz` & `tmp/djangocms_dag_jetcode-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_dag_jetcode-1.0.3.tar", max compression
+gzip compressed data, was "djangocms_dag_jetcode-1.1.2.tar", max compression
```

## Comparing `djangocms_dag_jetcode-1.0.3.tar` & `djangocms_dag_jetcode-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1491 2022-02-22 13:50:53.885088 djangocms_dag_jetcode-1.0.3/LICENSE
--rw-r--r--   0        0        0     2101 2022-02-22 14:22:06.091912 djangocms_dag_jetcode-1.0.3/README.md
--rw-r--r--   0        0        0       89 2022-02-22 14:22:43.260924 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/__init__.py
--rw-r--r--   0        0        0      448 2022-02-15 08:03:06.393068 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/admin.py
--rw-r--r--   0        0        0      150 2022-02-21 15:32:48.925912 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/apps.py
--rw-r--r--   0        0        0     1302 2022-02-22 11:08:14.747979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/cms_plugins.py
--rw-r--r--   0        0        0        0 2022-02-14 17:30:31.284449 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/conf/__init__.py
--rw-r--r--   0        0        0      219 2022-02-22 11:08:14.744979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/conf/settings.py
--rw-r--r--   0        0        0      867 2022-02-22 09:38:42.675430 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1059 2022-02-22 09:38:29.463900 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3233 2022-02-22 11:08:14.440979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-02-15 08:03:06.399068 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/migrations/__init__.py
--rw-r--r--   0        0        0     1712 2022-02-22 11:08:14.738979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/models.py
--rw-r--r--   0        0        0       39 2022-02-21 17:33:56.173622 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/base.css
--rw-r--r--   0        0        0        0 2022-02-22 10:25:03.879619 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/package.css
--rw-r--r--   0        0        0        0 2022-02-22 10:25:08.247619 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/product.css
--rw-r--r--   0        0        0        0 2022-02-22 10:25:13.069619 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/productselector.css
--rw-r--r--   0        0        0     7187 2022-02-21 16:52:49.025453 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/img/calendar-icon.png
--rw-r--r--   0        0        0      383 2022-02-21 15:48:28.574255 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/templates/djangocms_dag_jetcode/default.html
--rw-r--r--   0        0        0      178 2022-02-22 11:08:14.748979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/urls.py
--rw-r--r--   0        0        0     1689 2022-02-22 11:08:14.742979 djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/views.py
--rw-r--r--   0        0        0     1035 2022-02-22 14:22:43.261924 djangocms_dag_jetcode-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3367 2022-02-22 14:23:56.213305 djangocms_dag_jetcode-1.0.3/setup.py
--rw-r--r--   0        0        0     3022 2022-02-22 14:23:56.213794 djangocms_dag_jetcode-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2022-02-22 13:50:53.885088 djangocms_dag_jetcode-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3083 2023-04-26 16:12:16.931120 djangocms_dag_jetcode-1.1.2/README.md
+-rw-r--r--   0        0        0       89 2023-04-27 07:26:24.060562 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/__init__.py
+-rw-r--r--   0        0        0      448 2022-02-15 08:03:06.393068 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/admin.py
+-rw-r--r--   0        0        0      150 2022-02-21 15:32:48.925912 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/apps.py
+-rw-r--r--   0        0        0     1302 2022-02-22 11:08:14.747979 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/cms_plugins.py
+-rw-r--r--   0        0        0        0 2022-02-14 17:30:31.284449 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/conf/__init__.py
+-rw-r--r--   0        0        0      219 2022-02-22 11:08:14.744979 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/conf/settings.py
+-rw-r--r--   0        0        0      922 2022-06-10 10:11:31.918438 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1108 2022-06-10 10:09:23.424309 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3233 2022-02-22 11:08:14.440979 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1002 2022-10-12 07:54:58.650156 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/migrations/0002_auto_20220610_1207.py
+-rw-r--r--   0        0        0        0 2022-02-15 08:03:06.399068 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/migrations/__init__.py
+-rw-r--r--   0        0        0     1750 2022-06-10 10:03:11.870658 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/models.py
+-rw-r--r--   0        0        0       39 2022-02-21 17:33:56.173622 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/base.css
+-rw-r--r--   0        0        0        0 2022-10-12 07:52:47.042673 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/container.css
+-rw-r--r--   0        0        0        0 2022-02-22 10:25:03.879619 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/package.css
+-rw-r--r--   0        0        0        0 2022-02-22 10:25:08.247619 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/product.css
+-rw-r--r--   0        0        0        0 2022-02-22 10:25:13.069619 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/css/productselector.css
+-rw-r--r--   0        0        0     7187 2022-02-21 16:52:49.025453 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/img/calendar-icon.png
+-rw-r--r--   0        0        0      315 2022-06-10 10:01:46.053880 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/templates/djangocms_dag_jetcode/default.html
+-rw-r--r--   0        0        0      178 2022-03-10 11:48:35.309072 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/urls.py
+-rw-r--r--   0        0        0     1689 2022-03-10 11:48:35.309072 djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/views.py
+-rw-r--r--   0        0        0     1035 2023-04-27 07:26:24.061562 djangocms_dag_jetcode-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4368 2023-04-27 07:27:13.635707 djangocms_dag_jetcode-1.1.2/setup.py
+-rw-r--r--   0        0        0     4004 2023-04-27 07:27:13.636038 djangocms_dag_jetcode-1.1.2/PKG-INFO
```

### Comparing `djangocms_dag_jetcode-1.0.3/LICENSE` & `djangocms_dag_jetcode-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_dag_jetcode-1.0.3/README.md` & `djangocms_dag_jetcode-1.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,25 +10,44 @@
 - Django 2.0+
 - Django CMS 3.8.0+
 
 # Installation
 
 - run `pip install djangocms-dag-jetcode`
 - add `djangocms_dag_jetcode` to your `INSTALLED_APPS`
+- include in your `urls.py`
+  ```py
+  path(
+      "djangocms-dag-jetcode/",
+      include("djangocms_dag_jetcode.urls", namespace="djangocms-dag-jetcode"),
+  ),
+  ```
 - run `python manage.py migrate djangocms_dag_jetcode`
 - import DAG's scripts before the closing `</body>` tag
   ```html
   <script src="https://jetcode.dag-system.com/jetcodes/fr?customerID=<your customer id>" defer></script>
   ```
+- add required `<div>` for the basket
+  ```html
+  <div class="basket-jetcode" data-basket-id="0" css-jetcode-href="https://absolute.path/to/custom.css"></div>
+  ```
+- add required `<div>` for the popups
+  ```html
+  <div class="rate-jetcode-def" css-jetcode-href="https://absolute.path/to/custom.css" data-content="jet-code-div"></div>
+  <div class="cart-jetcode-def" css-jetcode-href="https://absolute.path/to/custom.css" data-content="jet-code-div"></div>
+  <div class="checkout-jetcode-def" css-jetcode-href="https://absolute.path/to/custom.css" data-content="jet-code-div" jetcode-options="zipCode"></div>
+  <div class="payinresult-jetcode-def" css-jetcode-href="https://absolute.path/to/custom.css" data-content="jet-code-div"></div>
+  ```
 
 You can override some files to customize the style:
 - `static/djangocms_dag_jetcode/css/base.css` base style for all Jetcodes
 - `static/djangocms_dag_jetcode/css/product.css` product Jetcodes
 - `static/djangocms_dag_jetcode/css/productselector.css` product selector Jetcodes
 - `static/djangocms_dag_jetcode/css/package.css` package Jetcodes
+- `static/djangocms_dag_jetcode/css/container.css` container Jetcodes
 - `static/djangocms_dag_jetcode/img/calendar-icon.png` the calendar icon
 - `templates/djangocms_dag_jetcode/default.html` the template used to render the Jetcodes
 
 # Settings
 
 ## Styles choices
 
@@ -54,10 +73,10 @@
 # Reload Jetcode after CMS plugin edit
 
 When you add or edit a plugin, the CMS does not reload the entire page. You should re-instantiate the Jetcodes to display them without a page refresh. Add this code to your pages:
 ```js
 if (window.hasOwnProperty('CMS') === true) {
   CMS.$(window).on('cms-content-refresh', function () {
     initJetcode()
-  }
+  })
 }
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
 # djangocms-dag-jetcode **Django CMS DAG Jetcode** is a plugin for [Django CMS]
 (http://django-cms.org/) that allows you to add [DAG System](https://dag-
 system.com/)'s Jetcodes on your site. ![preview djangocms-dag-jetcode](https://
 gitlab.com/kapt/open-source/djangocms-dag-jetcode/-/raw/main/preview.png) #
 Requirements - Python 3.8+ - Django 2.0+ - Django CMS 3.8.0+ # Installation -
 run `pip install djangocms-dag-jetcode` - add `djangocms_dag_jetcode` to your
-`INSTALLED_APPS` - run `python manage.py migrate djangocms_dag_jetcode` -
+`INSTALLED_APPS` - include in your `urls.py` ```py path( "djangocms-dag-
+jetcode/", include("djangocms_dag_jetcode.urls", namespace="djangocms-dag-
+jetcode"), ), ``` - run `python manage.py migrate djangocms_dag_jetcode` -
 import DAG's scripts before the closing `
 ` tag ```html
- ``` You can override some files to customize the style: - `static/
+ ``` - add required `
+` for the basket ```html
+``` - add required `
+` for the popups ```html
+``` You can override some files to customize the style: - `static/
 djangocms_dag_jetcode/css/base.css` base style for all Jetcodes - `static/
 djangocms_dag_jetcode/css/product.css` product Jetcodes - `static/
 djangocms_dag_jetcode/css/productselector.css` product selector Jetcodes -
 `static/djangocms_dag_jetcode/css/package.css` package Jetcodes - `static/
+djangocms_dag_jetcode/css/container.css` container Jetcodes - `static/
 djangocms_dag_jetcode/img/calendar-icon.png` the calendar icon - `templates/
 djangocms_dag_jetcode/default.html` the template used to render the Jetcodes #
 Settings ## Styles choices ```python DJANGOCMS_DAG_JETCODE_STYLE_CHOICES = [
 ("my-style", "My custom style"), ] ``` defaults to `[]` Each style defined in
 this setting must have a corresponding CSS file in `{STATIC_ROOT}/
 djangocms_dag_jetcode/css/` (for example: `my-style.css`). ## Cache timeout Set
 the cache timeout for the `get_css` view. ```python
 DJANGOCMS_DAG_JETCODE_CACHE_TIMEOUT = 15 * 60 ``` defaults to `15 * 60` (15
 minutes) When `DEBUG=True`, you can set this setting to `0` to disable the
 cache. # Reload Jetcode after CMS plugin edit When you add or edit a plugin,
 the CMS does not reload the entire page. You should re-instantiate the Jetcodes
 to display them without a page refresh. Add this code to your pages: ```js if
 (window.hasOwnProperty('CMS') === true) { CMS.$(window).on('cms-content-
-refresh', function () { initJetcode() } } ```
+refresh', function () { initJetcode() }) } ```
```

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/cms_plugins.py` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.po` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/locale/fr/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Dev Kapt <dev@kapt.mobi>, 2022.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: 1.0.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-22 10:35+0100\n"
+"POT-Creation-Date: 2022-06-10 12:08+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Dev Kapt <dev@kapt.mobi>\n"
 "Language-Team: Dev Kapt <dev@kapt.mobi>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -35,14 +35,17 @@
 
 msgid "Product"
 msgstr "Produit"
 
 msgid "Product selector"
 msgstr "Moteur de recherche de produits"
 
+msgid "Product list"
+msgstr "Liste de produits"
+
 msgid "Package"
 msgstr "Package"
 
 msgid "Type"
 msgstr "Type"
 
 msgid "Identifier"
```

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/migrations/0001_initial.py` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/models.py` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
         return ",".join(options_list)
 
 
 TYPE_CHOICES = (
     ("product", _("Product")),
     ("productselector", _("Product selector")),
+    ("container", _("Product list")),
     ("package", _("Package")),
 )
 
 
 class Jetcode(CMSPlugin):
     jetcode_type = models.CharField(_("Type"), choices=TYPE_CHOICES, max_length=20)
     jetcode_id = models.IntegerField(_("Identifier"))
```

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/static/djangocms_dag_jetcode/img/calendar-icon.png` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/static/djangocms_dag_jetcode/img/calendar-icon.png`

 * *Files identical despite different names*

### Comparing `djangocms_dag_jetcode-1.0.3/djangocms_dag_jetcode/views.py` & `djangocms_dag_jetcode-1.1.2/djangocms_dag_jetcode/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_dag_jetcode-1.0.3/pyproject.toml` & `djangocms_dag_jetcode-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms_dag_jetcode"
-version = "1.0.3"
+version = "1.1.2"
 description = "Django CMS DAG Jetcode is a plugin for Django CMS that allows you to add DAG System's Jetcodes on your site."
 authors = ["Kapt dev team <dev@kapt.mobi>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://gitlab.com/kapt/open-source/djangocms-dag-jetcode"
 
 [tool.poetry.dependencies]
@@ -20,15 +20,15 @@
 black = "~21.9b0"
 flake8 = "~3.9.2"
 isort = "~5.9.3"
 pre-commit = "~2.9"
 djhtml = "~1.4.10"
 
 [build-system]
-requires = ["poetry-core>=2.0.0"]
+requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 include = '\.pyi?$'
 exclude = '''
 (
     \.eggs         # exclude a few common directories in the
```

