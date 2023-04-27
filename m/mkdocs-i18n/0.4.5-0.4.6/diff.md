# Comparing `tmp/mkdocs-i18n-0.4.5.tar.gz` & `tmp/mkdocs-i18n-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-i18n-0.4.5.tar", last modified: Tue Apr 25 11:19:18 2023, max compression
+gzip compressed data, was "mkdocs-i18n-0.4.6.tar", last modified: Thu Apr 27 11:47:58 2023, max compression
```

## Comparing `mkdocs-i18n-0.4.5.tar` & `mkdocs-i18n-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/COPYING
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.519130 mkdocs-i18n-0.4.5/mkdocs_i18n/
--rwxrwxrwx   0 root         (0) root         (0)    10722 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/mkdocs_i18n/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:19:18.521130 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-25 11:19:18.000000 mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:19:18.522131 mkdocs-i18n-0.4.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2517 2023-04-25 11:19:07.000000 mkdocs-i18n-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.048363 mkdocs-i18n-0.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/.gitlint
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/COPYING
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-04-27 11:47:58.047447 mkdocs-i18n-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.042867 mkdocs-i18n-0.4.6/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.043783 mkdocs-i18n-0.4.6/docs/dir/
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/dir/index.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/dir/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/dir/no-en.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/dir/no-en.es.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/index.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/index.es.md
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/nav-title.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/nav-title.en.md
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/nav-title.es.md
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/no-nav-title.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/no-nav-title.es.md
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/no-nav-title.md
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/only-es.es.md
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/translated-title.ca.md
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/translated-title.en.md
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/docs/translated-title.es.md
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 11:47:58.048363 mkdocs-i18n-0.4.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.044699 mkdocs-i18n-0.4.6/spec/
+-rwxrwxrwx   0 root         (0) root         (0)    11267 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/spec/integration_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/spec/localize_src_path_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.032790 mkdocs-i18n-0.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.045615 mkdocs-i18n-0.4.6/src/mkdocs_i18n/
+-rwxrwxrwx   0 root         (0) root         (0)    10882 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:47:58.047447 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-04-27 11:47:57.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-27 11:47:58.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:47:57.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-27 11:47:58.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-27 11:47:58.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-27 11:47:58.000000 mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      291 2023-04-27 11:47:35.000000 mkdocs-i18n-0.4.6/test.sh
```

### Comparing `mkdocs-i18n-0.4.5/COPYING` & `mkdocs-i18n-0.4.6/COPYING`

 * *Files identical despite different names*

### Comparing `mkdocs-i18n-0.4.5/PKG-INFO` & `mkdocs-i18n-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: mkdocs-i18n
-Version: 0.4.5
+Version: 0.4.6
 Summary: MkDocs i18n plugin
-Home-page: https://gitlab.com/mkdocs-i18n/mkdocs-i18n
-Author: Simó Albert i Beltran
-Author-email: sim6@bona.gent
+Author-email: Simó Albert i Beltran <sim6@bona.gent>
 License: AGPL-3.0-or-later
+Project-URL: Homepage, https://gitlab.com/mkdocs-i18n/mkdocs-i18n
 Project-URL: Bug Reports, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues
 Project-URL: Funding, https://liberapay.com/mkdocs-i18n/donate
 Project-URL: Source, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/tree/main
 Keywords: mkdocs,plugin,i18n
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7, <4
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: COPYING
 
 # MkDocs i18n plugin
 
 A plugin to internationalize MkDocs. It adds links to translated pages for each page. It also hides other languages page links of navigation menu if there is a translation for current page language.
 
 Example of mkdocs-i18n usage: <https://mkdocs-i18n.gitlab.io/mkdocs-i18n>
 
 Feel free to write your comments or request adaptations to your requirements at <https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues>.
 
 mkdocs-i18n updates [Site Language of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language) if [it is enabled](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L7).
 
-mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L59).
+mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L57).
 
 ## Case Studies
 
 <http://isardvdi.com> (<https://isard.gitlab.io/isardvdi-docs>) is a multilingual community, most members know 2 languages but not the same ones, some understand 3... Each one has its favorite language and has different levels of knowledge about other languages. In addition, community documentation doesn't have a source language and not all documents need to be translated into all languages. Therefore, this plugin shows all available translations for the page shown at the top of the document and also for pages not translated into the language selected in the navigation menu.
 
 ## Setup
 
@@ -55,9 +53,7 @@
 
 ## Other interesting works:
 
 - [MkDocs static i18n plugin](https://github.com/ultrabug/mkdocs-static-i18n): Builds a parallel structure of translated documents with a source language. It does not link to other translations of the current document and does not show pages that have not been translated into the current language or the default language. Therefore, documents translated only into a non-default language are only linked to the navigation menu when visiting a page with the same language.
 - [MkDocs Theme i18n](https://github.com/mkdocs/mkdocs/pull/2299): Work in progress.
 - [Markdown i18n plugin](https://github.com/gisce/markdown-i18n): Provide translation of documents via po files but images cannot be localized.
 - [MkDocs Multilang](https://pypi.org/project/mkdocs-multilang/): Only released for MkDocs < 1.0
-
-
```

### Comparing `mkdocs-i18n-0.4.5/README.md` & `mkdocs-i18n-0.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Example of mkdocs-i18n usage: <https://mkdocs-i18n.gitlab.io/mkdocs-i18n>
 
 Feel free to write your comments or request adaptations to your requirements at <https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues>.
 
 mkdocs-i18n updates [Site Language of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language) if [it is enabled](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L7).
 
-mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L59).
+mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L57).
 
 ## Case Studies
 
 <http://isardvdi.com> (<https://isard.gitlab.io/isardvdi-docs>) is a multilingual community, most members know 2 languages but not the same ones, some understand 3... Each one has its favorite language and has different levels of knowledge about other languages. In addition, community documentation doesn't have a source language and not all documents need to be translated into all languages. Therefore, this plugin shows all available translations for the page shown at the top of the document and also for pages not translated into the language selected in the navigation menu.
 
 ## Setup
```

### Comparing `mkdocs-i18n-0.4.5/mkdocs_i18n/__init__.py` & `mkdocs-i18n-0.4.6/src/mkdocs_i18n/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,17 @@
                 context["config"]["extra"]["alternate"]
             )
         context["config"]["extra"]["alternate"] = deepcopy(
             context["config"]["extra"]["alternate_origin"]
         )
         for alternate_config in context["config"]["extra"]["alternate"]:
             if alternate_config.get("lang") == lang:
+                alternate_config["name"] = self.config.get("languages", {}).get(
+                    lang, alternate_config.get("name", lang)
+                )
                 alternate_config["link"] = context["page"].url
             else:
                 for alternate in self._get_language_alternate(context["page"], pages):
                     if alternate.get("translated_page") and alternate.get(
                         "lang"
                     ) == alternate_config.get("lang"):
                         alternate_config.update(
```

### Comparing `mkdocs-i18n-0.4.5/mkdocs_i18n.egg-info/PKG-INFO` & `mkdocs-i18n-0.4.6/src/mkdocs_i18n.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: mkdocs-i18n
-Version: 0.4.5
+Version: 0.4.6
 Summary: MkDocs i18n plugin
-Home-page: https://gitlab.com/mkdocs-i18n/mkdocs-i18n
-Author: Simó Albert i Beltran
-Author-email: sim6@bona.gent
+Author-email: Simó Albert i Beltran <sim6@bona.gent>
 License: AGPL-3.0-or-later
+Project-URL: Homepage, https://gitlab.com/mkdocs-i18n/mkdocs-i18n
 Project-URL: Bug Reports, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues
 Project-URL: Funding, https://liberapay.com/mkdocs-i18n/donate
 Project-URL: Source, https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/tree/main
 Keywords: mkdocs,plugin,i18n
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7, <4
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: COPYING
 
 # MkDocs i18n plugin
 
 A plugin to internationalize MkDocs. It adds links to translated pages for each page. It also hides other languages page links of navigation menu if there is a translation for current page language.
 
 Example of mkdocs-i18n usage: <https://mkdocs-i18n.gitlab.io/mkdocs-i18n>
 
 Feel free to write your comments or request adaptations to your requirements at <https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/issues>.
 
 mkdocs-i18n updates [Site Language of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language) if [it is enabled](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L7).
 
-mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L59).
+mkdocs-i18n updates [Site Language Selector of Material for MkDocs](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#site-language-selector) linking each translated page if [it is configured](https://gitlab.com/mkdocs-i18n/mkdocs-i18n/-/blob/main/mkdocs.yml#L57).
 
 ## Case Studies
 
 <http://isardvdi.com> (<https://isard.gitlab.io/isardvdi-docs>) is a multilingual community, most members know 2 languages but not the same ones, some understand 3... Each one has its favorite language and has different levels of knowledge about other languages. In addition, community documentation doesn't have a source language and not all documents need to be translated into all languages. Therefore, this plugin shows all available translations for the page shown at the top of the document and also for pages not translated into the language selected in the navigation menu.
 
 ## Setup
 
@@ -55,9 +53,7 @@
 
 ## Other interesting works:
 
 - [MkDocs static i18n plugin](https://github.com/ultrabug/mkdocs-static-i18n): Builds a parallel structure of translated documents with a source language. It does not link to other translations of the current document and does not show pages that have not been translated into the current language or the default language. Therefore, documents translated only into a non-default language are only linked to the navigation menu when visiting a page with the same language.
 - [MkDocs Theme i18n](https://github.com/mkdocs/mkdocs/pull/2299): Work in progress.
 - [Markdown i18n plugin](https://github.com/gisce/markdown-i18n): Provide translation of documents via po files but images cannot be localized.
 - [MkDocs Multilang](https://pypi.org/project/mkdocs-multilang/): Only released for MkDocs < 1.0
-
-
```

