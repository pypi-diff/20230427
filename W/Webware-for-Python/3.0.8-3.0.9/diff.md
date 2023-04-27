# Comparing `tmp/Webware-for-Python-3.0.8.tar.gz` & `tmp/Webware-for-Python-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Webware-for-Python-3.0.8.tar", last modified: Thu Mar 16 11:43:58 2023, max compression
+gzip compressed data, was "Webware-for-Python-3.0.9.tar", last modified: Thu Apr 27 19:07:31 2023, max compression
```

## Comparing `Webware-for-Python-3.0.8.tar` & `Webware-for-Python-3.0.9.tar`

### file list

```diff
@@ -1,443 +1,443 @@
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/
--rw-r--r--   0 cito      (1000) cito      (1000)      143 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/.flake8
--rw-r--r--   0 cito      (1000) cito      (1000)     1564 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/.pylintrc
--rw-r--r--   0 cito      (1000) cito      (1000)     1164 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/LICENSE
--rw-r--r--   0 cito      (1000) cito      (1000)      417 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/MANIFEST.in
--rw-r--r--   0 cito      (1000) cito      (1000)     2635 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/PKG-INFO
--rw-r--r--   0 cito      (1000) cito      (1000)      957 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/README.md
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.790447 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/
--rw-r--r--   0 cito      (1000) cito      (1000)     2635 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/PKG-INFO
--rw-r--r--   0 cito      (1000) cito      (1000)    12307 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/SOURCES.txt
--rw-r--r--   0 cito      (1000) cito      (1000)        1 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/dependency_links.txt
--rw-r--r--   0 cito      (1000) cito      (1000)      208 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/entry_points.txt
--rw-r--r--   0 cito      (1000) cito      (1000)      500 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/requires.txt
--rw-r--r--   0 cito      (1000) cito      (1000)        8 2023-03-16 11:43:58.000000 Webware-for-Python-3.0.8/Webware_for_Python.egg-info/top_level.txt
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.790447 Webware-for-Python-3.0.8/bin/
--rw-r--r--   0 cito      (1000) cito      (1000)      120 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/bin/editfile.bat
--rw-r--r--   0 cito      (1000) cito      (1000)     2586 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/bin/editfile.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.790447 Webware-for-Python-3.0.8/docs/
--rw-r--r--   0 cito      (1000) cito      (1000)      634 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/Makefile
--rw-r--r--   0 cito      (1000) cito      (1000)    28921 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/appdev.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     4006 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/changes.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     2720 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/conf.py
--rw-r--r--   0 cito      (1000) cito      (1000)    25106 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/config.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     1669 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/copyright.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.790447 Webware-for-Python-3.0.8/docs/css/
--rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/css/custom.css
--rw-r--r--   0 cito      (1000) cito      (1000)     3392 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/css/logo.png
--rw-r--r--   0 cito      (1000) cito      (1000)    43297 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/deploy.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      401 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     2770 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/install.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      795 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/make.bat
--rw-r--r--   0 cito      (1000) cito      (1000)     6123 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/migrate.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      367 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/miscutils.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     9109 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/overview.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     2643 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/plugins.rst
--rw-r--r--   0 cito      (1000) cito      (1000)    20607 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/psp.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     7621 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/quickstart.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.790447 Webware-for-Python-3.0.8/docs/ref/
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.800447 Webware-for-Python-3.0.8/docs/ref/core/
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/application.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      107 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/configurableforserversidepath.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/cookie.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/exceptionhandler.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/httpcontent.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/httpexceptions.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/httprequest.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       56 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/httpresponse.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/httpservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/importmanager.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      704 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/jsonrpcservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       32 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/page.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/picklerpcservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/plugin.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/properties.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/request.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       44 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/response.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/rpcservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/servlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/servletfactory.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/session.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       77 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessiondynamicstore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionfilestore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       83 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionmemcachedstore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionmemorystore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       71 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionredisstore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionshelvestore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       56 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sessionstore.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/sidebarpage.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/transaction.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       86 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/unknownfiletypeservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       47 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/urlparser.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/wsgistreamout.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/core/xmlrpcservlet.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      226 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/index.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.800447 Webware-for-Python-3.0.8/docs/ref/miscutils/
--rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/configurable.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/csvjoiner.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/csvparser.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/datatable.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/dateinterval.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       60 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/dateparser.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       48 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/dbpool.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/dictforargs.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       71 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/error.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/funcs.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      317 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/mixin.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       78 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/namedvalueaccess.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/paramfactory.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/picklecache.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/miscutils/picklerpc.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.800447 Webware-for-Python-3.0.8/docs/ref/psp/
--rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/braceconverter.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/context.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       54 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/generators.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      292 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       75 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/parseeventhandler.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/pspcompiler.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/psppage.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       51 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/pspparser.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       75 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/pspservletfactory.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       48 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/psputils.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/servletwriter.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       60 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/psp/streamreader.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.800447 Webware-for-Python-3.0.8/docs/ref/taskkit/
--rw-r--r--   0 cito      (1000) cito      (1000)      166 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/taskkit/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       55 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/taskkit/scheduler.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/taskkit/task.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       61 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/taskkit/taskhandler.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.810447 Webware-for-Python-3.0.8/docs/ref/userkit/
--rw-r--r--   0 cito      (1000) cito      (1000)       52 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/hierrole.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      274 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/role.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       52 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/roleuser.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       73 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/roleusermanager.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       88 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/roleusermanagermixin.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       91 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/roleusermanagertofile.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/user.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       61 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/usermanager.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       79 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/userkit/usermanagertofile.rst
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.810447 Webware-for-Python-3.0.8/docs/ref/webutils/
--rw-r--r--   0 cito      (1000) cito      (1000)      104 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/expansivehtmlforexception.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       65 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/fieldstorage.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       44 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/funcs.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       77 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/htmlforexception.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/htmltag.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/httpstatuscodes.rst
--rw-r--r--   0 cito      (1000) cito      (1000)      216 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/ref/webutils/index.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       33 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/requirements.txt
--rw-r--r--   0 cito      (1000) cito      (1000)    11683 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/style.rst
--rw-r--r--   0 cito      (1000) cito      (1000)    17413 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/taskkit.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     3061 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/testing.rst
--rw-r--r--   0 cito      (1000) cito      (1000)    14689 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/tutorial.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     2930 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/userkit.rst
--rw-r--r--   0 cito      (1000) cito      (1000)     3262 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/docs/webutils.rst
--rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/setup.cfg
--rw-r--r--   0 cito      (1000) cito      (1000)     2991 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/setup.py
--rw-r--r--   0 cito      (1000) cito      (1000)      636 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/tox.ini
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.810447 Webware-for-Python-3.0.8/webware/
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.820447 Webware-for-Python-3.0.8/webware/Admin/
--rw-r--r--   0 cito      (1000) cito      (1000)      144 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/Access.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1739 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/AdminPage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2443 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/AdminSecurity.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2834 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/AppControl.py
--rw-r--r--   0 cito      (1000) cito      (1000)      289 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/Config.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1882 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/DumpCSV.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1162 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/EditFile.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1119 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/Errors.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2236 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/LoginPage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1379 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1018 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/PlugIns.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4322 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/ServletCache.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1630 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/View.py
--rw-r--r--   0 cito      (1000) cito      (1000)       20 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Admin/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)    46097 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Application.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.820447 Webware-for-Python-3.0.8/webware/Configs/
--rw-r--r--   0 cito      (1000) cito      (1000)     4919 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Configs/Application.config
--rw-r--r--   0 cito      (1000) cito      (1000)     1577 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/ConfigurableForServerSidePath.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4620 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Cookie.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.820447 Webware-for-Python-3.0.8/webware/Examples/
--rw-r--r--   0 cito      (1000) cito      (1000)     7861 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/AjaxPage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2580 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/AjaxSuggest.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1949 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Colorize.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3097 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Colors.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1150 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/CountVisits.py
--rw-r--r--   0 cito      (1000) cito      (1000)    18214 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/DBUtilsDemo.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1378 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/DominateDemo.py
--rw-r--r--   0 cito      (1000) cito      (1000)      995 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Error.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3676 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ExamplePage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2473 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/FileUpload.py
--rw-r--r--   0 cito      (1000) cito      (1000)      463 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Forward.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3505 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ImageDemo.py
--rw-r--r--   0 cito      (1000) cito      (1000)      201 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/IncludeMe.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1323 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Introspect.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2511 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/JSONRPCClient.py
--rw-r--r--   0 cito      (1000) cito      (1000)      662 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/JSONRPCExample.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4374 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ListBox.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2736 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/LoginPage.py
--rw-r--r--   0 cito      (1000) cito      (1000)      333 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/OtherFileTypes.py
--rw-r--r--   0 cito      (1000) cito      (1000)      783 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/PickleRPCExample.py
--rw-r--r--   0 cito      (1000) cito      (1000)      627 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/PlugInInspector.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2891 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/PushServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2052 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/RequestInformation.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1537 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/SecureCountVisits.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5818 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/SecurePage.py
--rw-r--r--   0 cito      (1000) cito      (1000)      263 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ShowTime.py
--rw-r--r--   0 cito      (1000) cito      (1000)      183 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Simple.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1393 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/View.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1625 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/Welcome.py
--rw-r--r--   0 cito      (1000) cito      (1000)      785 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/XMLRPCExample.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3478 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/YattagDemo.py
--rw-r--r--   0 cito      (1000) cito      (1000)       28 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3145 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ajaxcall.js
--rw-r--r--   0 cito      (1000) cito      (1000)     1584 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ajaxpoll.js
--rw-r--r--   0 cito      (1000) cito      (1000)      758 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ajaxsuggest.css
--rw-r--r--   0 cito      (1000) cito      (1000)     1691 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/ajaxsuggest.js
--rw-r--r--   0 cito      (1000) cito      (1000)     3758 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/favicon.ico
--rw-r--r--   0 cito      (1000) cito      (1000)      606 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/index.py
--rw-r--r--   0 cito      (1000) cito      (1000)    13422 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Examples/jsonrpc.js
--rw-r--r--   0 cito      (1000) cito      (1000)    24484 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/ExceptionHandler.py
--rw-r--r--   0 cito      (1000) cito      (1000)    12945 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/HTTPContent.py
--rw-r--r--   0 cito      (1000) cito      (1000)    11634 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/HTTPExceptions.py
--rw-r--r--   0 cito      (1000) cito      (1000)    29883 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/HTTPRequest.py
--rw-r--r--   0 cito      (1000) cito      (1000)    17581 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/HTTPResponse.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3017 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/HTTPServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     9681 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/ImportManager.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3780 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/JSONRPCServlet.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/MiscUtils/
--rw-r--r--   0 cito      (1000) cito      (1000)      838 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/CSVJoiner.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7946 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/CSVParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7516 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Configurable.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6956 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/DBPool.py
--rw-r--r--   0 cito      (1000) cito      (1000)    26216 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/DataTable.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1469 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/DateInterval.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1420 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/DateParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5714 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/DictForArgs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2047 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Error.py
--rw-r--r--   0 cito      (1000) cito      (1000)    10659 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Funcs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1593 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/M2PickleRPC.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4133 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/MixIn.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3632 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/NamedValueAccess.py
--rw-r--r--   0 cito      (1000) cito      (1000)      677 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/ParamFactory.py
--rw-r--r--   0 cito      (1000) cito      (1000)     9354 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/PickleCache.py
--rw-r--r--   0 cito      (1000) cito      (1000)    12761 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/PickleRPC.py
--rw-r--r--   0 cito      (1000) cito      (1000)      266 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Properties.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6197 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/PropertiesObject.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/
--rw-r--r--   0 cito      (1000) cito      (1000)     2212 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/BenchCSVParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2152 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/BenchDataTable.py
--rw-r--r--   0 cito      (1000) cito      (1000)      530 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/Sample.csv
--rw-r--r--   0 cito      (1000) cito      (1000)    13824 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/Sample.xls
--rw-r--r--   0 cito      (1000) cito      (1000)     2939 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestCSVParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)      489 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDBPool.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7699 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDataTable.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1108 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDateInterval.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3181 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDateParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2781 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDictForArgs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1753 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestError.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7576 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestFuncs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     8788 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestMixIn.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3602 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestNamedValueAccess.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2733 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestPickleCache.py
--rw-r--r--   0 cito      (1000) cito      (1000)       22 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1831 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MiscUtils/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2287 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/MockApplication.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/PSP/
--rw-r--r--   0 cito      (1000) cito      (1000)     4962 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/BraceConverter.py
--rw-r--r--   0 cito      (1000) cito      (1000)      710 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/CompilePSP.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5475 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Context.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/PSP/Examples/
--rw-r--r--   0 cito      (1000) cito      (1000)     2260 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/Braces.psp
--rw-r--r--   0 cito      (1000) cito      (1000)     1588 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/Hello.psp
--rw-r--r--   0 cito      (1000) cito      (1000)      429 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/PSPExamplePage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5021 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/PSPTests-Braces.psp
--rw-r--r--   0 cito      (1000) cito      (1000)     5745 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/PSPTests.psp
--rw-r--r--   0 cito      (1000) cito      (1000)      102 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/PSPinclude.psp
--rw-r--r--   0 cito      (1000) cito      (1000)     1488 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/View.py
--rw-r--r--   0 cito      (1000) cito      (1000)       28 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/index.psp
--rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/my_include.html
--rw-r--r--   0 cito      (1000) cito      (1000)       86 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/my_include.psp
--rw-r--r--   0 cito      (1000) cito      (1000)    18092 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Examples/psplogo.png
--rw-r--r--   0 cito      (1000) cito      (1000)    10688 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Generators.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1489 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/PSPCompiler.py
--rw-r--r--   0 cito      (1000) cito      (1000)      555 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/PSPPage.py
--rw-r--r--   0 cito      (1000) cito      (1000)    12760 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/PSPParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4411 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/PSPServletFactory.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2817 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/PSPUtils.py
--rw-r--r--   0 cito      (1000) cito      (1000)    17800 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/ParseEventHandler.py
--rw-r--r--   0 cito      (1000) cito      (1000)      527 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Properties.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3853 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/ServletWriter.py
--rw-r--r--   0 cito      (1000) cito      (1000)     9513 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/StreamReader.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/PSP/Tests/
--rw-r--r--   0 cito      (1000) cito      (1000)     2544 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Tests/TestBraceConverter.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5438 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Tests/TestCompiler.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1415 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Tests/TestContext.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3876 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Tests/TestUtils.py
--rw-r--r--   0 cito      (1000) cito      (1000)       26 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      194 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PSP/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     8303 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Page.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7464 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PickleRPCServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6844 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PlugIn.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2288 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/PlugInLoader.py
--rw-r--r--   0 cito      (1000) cito      (1000)      641 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Properties.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3116 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/RPCServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3620 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Request.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1736 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Response.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.830447 Webware-for-Python-3.0.8/webware/Scripts/
--rw-r--r--   0 cito      (1000) cito      (1000)    15461 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Scripts/MakeAppWorkDir.py
--rw-r--r--   0 cito      (1000) cito      (1000)      610 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Scripts/WSGIScript.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5457 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Scripts/WaitressServer.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1283 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Scripts/WebwareCLI.py
--rw-r--r--   0 cito      (1000) cito      (1000)       46 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Scripts/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5412 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Servlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)    15132 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/ServletFactory.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6984 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Session.py
--rw-r--r--   0 cito      (1000) cito      (1000)    10824 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionDynamicStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5782 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionFileStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     8844 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionMemcachedStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3379 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionMemoryStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7735 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionRedisStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3861 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionShelveStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     8523 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SessionStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5658 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/SidebarPage.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/TaskKit/
--rw-r--r--   0 cito      (1000) cito      (1000)      194 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Properties.py
--rw-r--r--   0 cito      (1000) cito      (1000)    16126 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Scheduler.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1956 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Task.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3999 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/TaskHandler.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/TaskKit/Tests/
--rw-r--r--   0 cito      (1000) cito      (1000)     1816 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Tests/SchedulerTest.py
--rw-r--r--   0 cito      (1000) cito      (1000)      342 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Tests/TestScheduler.py
--rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/TaskKit/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Tasks/
--rw-r--r--   0 cito      (1000) cito      (1000)      297 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tasks/SessionTask.py
--rw-r--r--   0 cito      (1000) cito      (1000)        2 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tasks/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/
--rw-r--r--   0 cito      (1000) cito      (1000)      846 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/DebugPage.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/Dir/
--rw-r--r--   0 cito      (1000) cito      (1000)      262 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/File.html
--rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/Forward2Target.py
--rw-r--r--   0 cito      (1000) cito      (1000)      244 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/Forward3.py
--rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/Forward3Target.py
--rw-r--r--   0 cito      (1000) cito      (1000)      911 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/IncludeURLTest2.py
--rw-r--r--   0 cito      (1000) cito      (1000)       14 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      254 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Dir/index.html
--rw-r--r--   0 cito      (1000) cito      (1000)      781 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/EmbeddedServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5596 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/FieldStorage.py
--rw-r--r--   0 cito      (1000) cito      (1000)      241 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Forward1.py
--rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Forward1Target.py
--rw-r--r--   0 cito      (1000) cito      (1000)      245 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Forward2.py
--rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Forward3Target.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4772 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/IncludeURLTest.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3292 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)      483 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/Servlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1287 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/ServletImport.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1542 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/SetCookie.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1725 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/TestCases.data
--rw-r--r--   0 cito      (1000) cito      (1000)     3874 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/TestIMS.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/
--rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      799 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/index.html
--rw-r--r--   0 cito      (1000) cito      (1000)      302 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/simple.html
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test1/
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test1/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)       12 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test1/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test2/
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test2/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)       81 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test2/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test3/
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test3/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test3/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test4/
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test4/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)      148 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test4/__init__.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test5/
--rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5/url3.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test5join1/
--rw-r--r--   0 cito      (1000) cito      (1000)       17 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5join1/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5join1/url1.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/test5join2/
--rw-r--r--   0 cito      (1000) cito      (1000)       17 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5join2/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5join2/url1.py
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/test5join2/url2.py
--rw-r--r--   0 cito      (1000) cito      (1000)      698 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/util.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Testing/URL/vhosts/
--rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/vhosts/Main.py
--rw-r--r--   0 cito      (1000) cito      (1000)      263 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/URL/vhosts/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       22 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)       64 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/test.html
--rw-r--r--   0 cito      (1000) cito      (1000)       11 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Testing/test.text
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.840447 Webware-for-Python-3.0.8/webware/Tests/
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/
--rw-r--r--   0 cito      (1000) cito      (1000)     2949 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/AppTest.py
--rw-r--r--   0 cito      (1000) cito      (1000)    11148 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestAdmin.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2812 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestContextMap.py
--rw-r--r--   0 cito      (1000) cito      (1000)    27039 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestExamples.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3086 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestMakeApp.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5268 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestPSPExamples.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7958 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestServer.py
--rw-r--r--   0 cito      (1000) cito      (1000)    11391 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestTesting.py
--rw-r--r--   0 cito      (1000) cito      (1000)       31 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1314 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestMocking.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/Tests/TestSessions/
--rw-r--r--   0 cito      (1000) cito      (1000)     1035 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/Application.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1129 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/Session.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5145 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSession.py
--rw-r--r--   0 cito      (1000) cito      (1000)      797 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionDynamicStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1016 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionFileStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2480 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionMemcachedStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6134 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionMemoryStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)      528 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionRedisStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)      944 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionShelveStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1240 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionStore.py
--rw-r--r--   0 cito      (1000) cito      (1000)      226 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/Transaction.py
--rw-r--r--   0 cito      (1000) cito      (1000)       33 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      823 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/memcache.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1374 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/TestSessions/redis.py
--rw-r--r--   0 cito      (1000) cito      (1000)       20 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6459 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/Transaction.py
--rw-r--r--   0 cito      (1000) cito      (1000)    32708 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/URLParser.py
--rw-r--r--   0 cito      (1000) cito      (1000)     8679 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UnknownFileTypeServlet.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/UserKit/
--rw-r--r--   0 cito      (1000) cito      (1000)      856 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/HierRole.py
--rw-r--r--   0 cito      (1000) cito      (1000)      157 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Properties.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1655 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Role.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2310 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/RoleUser.py
--rw-r--r--   0 cito      (1000) cito      (1000)      370 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/RoleUserManager.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1370 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/RoleUserManagerMixIn.py
--rw-r--r--   0 cito      (1000) cito      (1000)      406 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/RoleUserManagerToFile.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/UserKit/Tests/
--rw-r--r--   0 cito      (1000) cito      (1000)     3692 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Tests/TestExample.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2875 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Tests/TestRole.py
--rw-r--r--   0 cito      (1000) cito      (1000)     5757 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Tests/TestUserManager.py
--rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3336 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/User.py
--rw-r--r--   0 cito      (1000) cito      (1000)     9472 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/UserManager.py
--rw-r--r--   0 cito      (1000) cito      (1000)     6264 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/UserManagerToFile.py
--rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/UserKit/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     7425 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WSGIStreamOut.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/WebUtils/
--rw-r--r--   0 cito      (1000) cito      (1000)     9464 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/CGITraceback.py
--rw-r--r--   0 cito      (1000) cito      (1000)      725 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/ExpansiveHTMLForException.py
--rw-r--r--   0 cito      (1000) cito      (1000)    23967 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/FieldStorage.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4185 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Funcs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3044 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/HTMLForException.py
--rw-r--r--   0 cito      (1000) cito      (1000)    21991 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/HTMLTag.py
--rw-r--r--   0 cito      (1000) cito      (1000)     2345 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/HTTPStatusCodes.py
--rw-r--r--   0 cito      (1000) cito      (1000)      152 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Properties.py
-drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-03-16 11:43:58.850447 Webware-for-Python-3.0.8/webware/WebUtils/Tests/
--rw-r--r--   0 cito      (1000) cito      (1000)    13077 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFieldStorageModified.py
--rw-r--r--   0 cito      (1000) cito      (1000)    15484 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFieldStorageStandard.py
--rw-r--r--   0 cito      (1000) cito      (1000)     4641 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFuncs.py
--rw-r--r--   0 cito      (1000) cito      (1000)     1242 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestHTMLStatusCodes.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3057 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestHTMLTag.py
--rw-r--r--   0 cito      (1000) cito      (1000)       21 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/Tests/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      156 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/WebUtils/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)     3272 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/XMLRPCServlet.py
--rw-r--r--   0 cito      (1000) cito      (1000)      593 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/__init__.py
--rw-r--r--   0 cito      (1000) cito      (1000)      430 2023-03-16 11:43:25.000000 Webware-for-Python-3.0.8/webware/error404.html
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/
+-rw-r--r--   0 cito      (1000) cito      (1000)      143 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/.flake8
+-rw-r--r--   0 cito      (1000) cito      (1000)     1564 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/.pylintrc
+-rw-r--r--   0 cito      (1000) cito      (1000)     1164 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/LICENSE
+-rw-r--r--   0 cito      (1000) cito      (1000)      417 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/MANIFEST.in
+-rw-r--r--   0 cito      (1000) cito      (1000)     2635 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/PKG-INFO
+-rw-r--r--   0 cito      (1000) cito      (1000)      957 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/README.md
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.690077 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/
+-rw-r--r--   0 cito      (1000) cito      (1000)     2635 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/PKG-INFO
+-rw-r--r--   0 cito      (1000) cito      (1000)    12307 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 cito      (1000) cito      (1000)        1 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 cito      (1000) cito      (1000)      208 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/entry_points.txt
+-rw-r--r--   0 cito      (1000) cito      (1000)      500 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/requires.txt
+-rw-r--r--   0 cito      (1000) cito      (1000)        8 2023-04-27 19:07:31.000000 Webware-for-Python-3.0.9/Webware_for_Python.egg-info/top_level.txt
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.690077 Webware-for-Python-3.0.9/bin/
+-rw-r--r--   0 cito      (1000) cito      (1000)      120 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/bin/editfile.bat
+-rw-r--r--   0 cito      (1000) cito      (1000)     2586 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/bin/editfile.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.700077 Webware-for-Python-3.0.9/docs/
+-rw-r--r--   0 cito      (1000) cito      (1000)      634 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/Makefile
+-rw-r--r--   0 cito      (1000) cito      (1000)    28921 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/appdev.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     4006 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/changes.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     2720 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/conf.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    25106 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/config.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     1669 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/copyright.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.700077 Webware-for-Python-3.0.9/docs/css/
+-rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/css/custom.css
+-rw-r--r--   0 cito      (1000) cito      (1000)     3392 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/css/logo.png
+-rw-r--r--   0 cito      (1000) cito      (1000)    43297 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/deploy.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      401 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     2770 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/install.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      795 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/make.bat
+-rw-r--r--   0 cito      (1000) cito      (1000)     6123 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/migrate.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      367 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/miscutils.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     9109 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/overview.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     2643 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/plugins.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)    20607 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/psp.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     7621 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/quickstart.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.700077 Webware-for-Python-3.0.9/docs/ref/
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.700077 Webware-for-Python-3.0.9/docs/ref/core/
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/application.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      107 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/configurableforserversidepath.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/cookie.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/exceptionhandler.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/httpcontent.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/httpexceptions.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/httprequest.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       56 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/httpresponse.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/httpservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/importmanager.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      704 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/jsonrpcservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       32 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/page.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/picklerpcservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/plugin.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/properties.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/request.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       44 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/response.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/rpcservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/servlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       62 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/servletfactory.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       41 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/session.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       77 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessiondynamicstore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       68 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionfilestore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       83 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionmemcachedstore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionmemorystore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       71 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionredisstore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionshelvestore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       56 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sessionstore.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/sidebarpage.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       53 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/transaction.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       86 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/unknownfiletypeservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       47 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/urlparser.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/wsgistreamout.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/core/xmlrpcservlet.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      226 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/index.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.700077 Webware-for-Python-3.0.9/docs/ref/miscutils/
+-rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/configurable.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/csvjoiner.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/csvparser.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/datatable.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/dateinterval.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       60 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/dateparser.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       48 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/dbpool.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/dictforargs.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       71 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/error.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/funcs.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      317 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/mixin.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       78 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/namedvalueaccess.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/paramfactory.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/picklecache.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/miscutils/picklerpc.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.710077 Webware-for-Python-3.0.9/docs/ref/psp/
+-rw-r--r--   0 cito      (1000) cito      (1000)       66 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/braceconverter.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/context.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       54 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/generators.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      292 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       75 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/parseeventhandler.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       57 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/pspcompiler.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       45 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/psppage.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       51 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/pspparser.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       75 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/pspservletfactory.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       48 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/psputils.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       63 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/servletwriter.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       60 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/psp/streamreader.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.710077 Webware-for-Python-3.0.9/docs/ref/taskkit/
+-rw-r--r--   0 cito      (1000) cito      (1000)      166 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/taskkit/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       55 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/taskkit/scheduler.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/taskkit/task.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       61 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/taskkit/taskhandler.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.710077 Webware-for-Python-3.0.9/docs/ref/userkit/
+-rw-r--r--   0 cito      (1000) cito      (1000)       52 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/hierrole.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      274 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/role.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       52 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/roleuser.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       73 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/roleusermanager.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       88 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/roleusermanagermixin.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       91 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/roleusermanagertofile.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       40 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/user.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       61 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/usermanager.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       79 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/userkit/usermanagertofile.rst
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.710077 Webware-for-Python-3.0.9/docs/ref/webutils/
+-rw-r--r--   0 cito      (1000) cito      (1000)      104 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/expansivehtmlforexception.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       65 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/fieldstorage.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       44 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/funcs.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       77 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/htmlforexception.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       50 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/htmltag.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       74 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/httpstatuscodes.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)      216 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/ref/webutils/index.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       33 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/requirements.txt
+-rw-r--r--   0 cito      (1000) cito      (1000)    11683 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/style.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)    17413 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/taskkit.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     3061 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/testing.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)    14689 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/tutorial.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     2930 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/userkit.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)     3262 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/docs/webutils.rst
+-rw-r--r--   0 cito      (1000) cito      (1000)       38 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/setup.cfg
+-rw-r--r--   0 cito      (1000) cito      (1000)     2991 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/setup.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      636 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/tox.ini
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.710077 Webware-for-Python-3.0.9/webware/
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.720077 Webware-for-Python-3.0.9/webware/Admin/
+-rw-r--r--   0 cito      (1000) cito      (1000)      144 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/Access.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1739 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/AdminPage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2443 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/AdminSecurity.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2834 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/AppControl.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      289 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/Config.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1882 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/DumpCSV.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1162 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/EditFile.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1119 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/Errors.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2236 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/LoginPage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1379 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1018 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/PlugIns.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4322 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/ServletCache.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1630 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/View.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       20 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Admin/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    46097 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Application.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.720077 Webware-for-Python-3.0.9/webware/Configs/
+-rw-r--r--   0 cito      (1000) cito      (1000)     4919 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Configs/Application.config
+-rw-r--r--   0 cito      (1000) cito      (1000)     1577 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/ConfigurableForServerSidePath.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4620 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Cookie.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.720077 Webware-for-Python-3.0.9/webware/Examples/
+-rw-r--r--   0 cito      (1000) cito      (1000)     7861 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/AjaxPage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2580 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/AjaxSuggest.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1949 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Colorize.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3097 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Colors.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1150 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/CountVisits.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    18214 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/DBUtilsDemo.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1378 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/DominateDemo.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      995 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Error.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3676 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ExamplePage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2473 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/FileUpload.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      463 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Forward.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3505 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ImageDemo.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      201 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/IncludeMe.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1323 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Introspect.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2511 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/JSONRPCClient.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      662 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/JSONRPCExample.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4374 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ListBox.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2736 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/LoginPage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      333 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/OtherFileTypes.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      783 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/PickleRPCExample.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      627 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/PlugInInspector.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2891 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/PushServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2052 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/RequestInformation.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1537 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/SecureCountVisits.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5818 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/SecurePage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      263 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ShowTime.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      183 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Simple.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1393 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/View.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1625 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/Welcome.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      785 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/XMLRPCExample.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3478 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/YattagDemo.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       28 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3145 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ajaxcall.js
+-rw-r--r--   0 cito      (1000) cito      (1000)     1584 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ajaxpoll.js
+-rw-r--r--   0 cito      (1000) cito      (1000)      758 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ajaxsuggest.css
+-rw-r--r--   0 cito      (1000) cito      (1000)     1691 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/ajaxsuggest.js
+-rw-r--r--   0 cito      (1000) cito      (1000)     3758 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/favicon.ico
+-rw-r--r--   0 cito      (1000) cito      (1000)      606 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/index.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    13422 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Examples/jsonrpc.js
+-rw-r--r--   0 cito      (1000) cito      (1000)    24484 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/ExceptionHandler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    12945 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/HTTPContent.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    11634 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/HTTPExceptions.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    29883 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/HTTPRequest.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    17581 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/HTTPResponse.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3017 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/HTTPServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     9681 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/ImportManager.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3780 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/JSONRPCServlet.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.720077 Webware-for-Python-3.0.9/webware/MiscUtils/
+-rw-r--r--   0 cito      (1000) cito      (1000)      838 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/CSVJoiner.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7946 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/CSVParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7516 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Configurable.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6956 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/DBPool.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    26216 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/DataTable.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1469 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/DateInterval.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1420 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/DateParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5714 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/DictForArgs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2047 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Error.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    10659 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Funcs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1593 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/M2PickleRPC.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4133 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/MixIn.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3632 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/NamedValueAccess.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      677 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/ParamFactory.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     9354 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/PickleCache.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    12761 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/PickleRPC.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      266 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Properties.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6197 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/PropertiesObject.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/
+-rw-r--r--   0 cito      (1000) cito      (1000)     2212 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/BenchCSVParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2152 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/BenchDataTable.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      530 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/Sample.csv
+-rw-r--r--   0 cito      (1000) cito      (1000)    13824 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/Sample.xls
+-rw-r--r--   0 cito      (1000) cito      (1000)     2939 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestCSVParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      489 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDBPool.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7699 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDataTable.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1108 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDateInterval.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3181 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDateParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2781 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDictForArgs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1753 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestError.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7576 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestFuncs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     8788 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestMixIn.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3602 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestNamedValueAccess.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2733 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestPickleCache.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       22 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1831 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MiscUtils/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2287 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/MockApplication.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/PSP/
+-rw-r--r--   0 cito      (1000) cito      (1000)     4962 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/BraceConverter.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      710 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/CompilePSP.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5475 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Context.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/PSP/Examples/
+-rw-r--r--   0 cito      (1000) cito      (1000)     2260 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/Braces.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)     1588 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/Hello.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)      429 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/PSPExamplePage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5021 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/PSPTests-Braces.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)     5745 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/PSPTests.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)      102 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/PSPinclude.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)     1488 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/View.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       28 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/index.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/my_include.html
+-rw-r--r--   0 cito      (1000) cito      (1000)       86 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/my_include.psp
+-rw-r--r--   0 cito      (1000) cito      (1000)    18092 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Examples/psplogo.png
+-rw-r--r--   0 cito      (1000) cito      (1000)    10688 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Generators.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1489 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/PSPCompiler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      555 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/PSPPage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    12760 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/PSPParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4411 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/PSPServletFactory.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2817 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/PSPUtils.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    17800 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/ParseEventHandler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      527 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Properties.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3853 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/ServletWriter.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     9513 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/StreamReader.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/PSP/Tests/
+-rw-r--r--   0 cito      (1000) cito      (1000)     2544 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Tests/TestBraceConverter.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5438 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Tests/TestCompiler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1415 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Tests/TestContext.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3876 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Tests/TestUtils.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       26 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      194 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PSP/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     8303 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Page.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7464 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PickleRPCServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6844 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PlugIn.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2288 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/PlugInLoader.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      641 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Properties.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3116 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/RPCServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3620 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Request.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1736 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Response.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/Scripts/
+-rw-r--r--   0 cito      (1000) cito      (1000)    15461 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Scripts/MakeAppWorkDir.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      610 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Scripts/WSGIScript.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5457 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Scripts/WaitressServer.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1283 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Scripts/WebwareCLI.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       46 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Scripts/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5412 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Servlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    15132 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/ServletFactory.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6984 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Session.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    10824 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionDynamicStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5782 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionFileStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     8844 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionMemcachedStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3379 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionMemoryStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7735 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionRedisStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3861 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionShelveStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     8523 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SessionStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5658 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/SidebarPage.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/TaskKit/
+-rw-r--r--   0 cito      (1000) cito      (1000)      194 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Properties.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    16126 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Scheduler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1956 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Task.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3999 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/TaskHandler.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/TaskKit/Tests/
+-rw-r--r--   0 cito      (1000) cito      (1000)     1816 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Tests/SchedulerTest.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      342 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Tests/TestScheduler.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/TaskKit/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.730077 Webware-for-Python-3.0.9/webware/Tasks/
+-rw-r--r--   0 cito      (1000) cito      (1000)      297 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tasks/SessionTask.py
+-rw-r--r--   0 cito      (1000) cito      (1000)        2 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tasks/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/
+-rw-r--r--   0 cito      (1000) cito      (1000)      846 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/DebugPage.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/Dir/
+-rw-r--r--   0 cito      (1000) cito      (1000)      262 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/File.html
+-rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/Forward2Target.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      244 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/Forward3.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/Forward3Target.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      911 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/IncludeURLTest2.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       14 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      254 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Dir/index.html
+-rw-r--r--   0 cito      (1000) cito      (1000)      781 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/EmbeddedServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5596 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/FieldStorage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      241 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Forward1.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Forward1Target.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      245 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Forward2.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       84 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Forward3Target.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4772 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/IncludeURLTest.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3292 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      483 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/Servlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1287 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/ServletImport.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1542 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/SetCookie.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1725 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/TestCases.data
+-rw-r--r--   0 cito      (1000) cito      (1000)     3874 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/TestIMS.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/
+-rw-r--r--   0 cito      (1000) cito      (1000)       89 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      799 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/index.html
+-rw-r--r--   0 cito      (1000) cito      (1000)      302 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/simple.html
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test1/
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test1/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       12 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test1/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test2/
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test2/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       81 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test2/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test3/
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test3/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test3/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test4/
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test4/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      148 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test4/__init__.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test5/
+-rw-r--r--   0 cito      (1000) cito      (1000)       59 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5/url3.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test5join1/
+-rw-r--r--   0 cito      (1000) cito      (1000)       17 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5join1/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5join1/url1.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/test5join2/
+-rw-r--r--   0 cito      (1000) cito      (1000)       17 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5join2/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5join2/url1.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/test5join2/url2.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      698 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/util.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Testing/URL/vhosts/
+-rw-r--r--   0 cito      (1000) cito      (1000)       93 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/vhosts/Main.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      263 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/URL/vhosts/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       22 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       64 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/test.html
+-rw-r--r--   0 cito      (1000) cito      (1000)       11 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Testing/test.text
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Tests/
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/
+-rw-r--r--   0 cito      (1000) cito      (1000)     2949 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/AppTest.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    11148 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestAdmin.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2812 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestContextMap.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    27039 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestExamples.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3086 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestMakeApp.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5268 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestPSPExamples.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7958 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestServer.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    11391 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestTesting.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       31 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1314 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestMocking.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.740077 Webware-for-Python-3.0.9/webware/Tests/TestSessions/
+-rw-r--r--   0 cito      (1000) cito      (1000)     1035 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/Application.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1129 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/Session.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5145 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSession.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      797 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionDynamicStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1016 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionFileStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2480 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionMemcachedStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6134 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionMemoryStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      528 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionRedisStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      944 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionShelveStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1240 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionStore.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      226 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/Transaction.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       33 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      823 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/memcache.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1374 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/TestSessions/redis.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       20 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6459 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/Transaction.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    32708 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/URLParser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     8679 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UnknownFileTypeServlet.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/webware/UserKit/
+-rw-r--r--   0 cito      (1000) cito      (1000)      856 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/HierRole.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      157 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Properties.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1655 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Role.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2310 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/RoleUser.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      370 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/RoleUserManager.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1370 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/RoleUserManagerMixIn.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      406 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/RoleUserManagerToFile.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/webware/UserKit/Tests/
+-rw-r--r--   0 cito      (1000) cito      (1000)     3692 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Tests/TestExample.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2875 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Tests/TestRole.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     5757 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Tests/TestUserManager.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       30 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3336 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/User.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     9472 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/UserManager.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     6264 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/UserManagerToFile.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       92 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/UserKit/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     7425 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WSGIStreamOut.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/webware/WebUtils/
+-rw-r--r--   0 cito      (1000) cito      (1000)     9464 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/CGITraceback.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      725 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/ExpansiveHTMLForException.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    24005 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/FieldStorage.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4185 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Funcs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3044 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/HTMLForException.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    21991 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/HTMLTag.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     2345 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/HTTPStatusCodes.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      152 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Properties.py
+drwxr-xr-x   0 cito      (1000) cito      (1000)        0 2023-04-27 19:07:31.750077 Webware-for-Python-3.0.9/webware/WebUtils/Tests/
+-rw-r--r--   0 cito      (1000) cito      (1000)    16540 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFieldStorageModified.py
+-rw-r--r--   0 cito      (1000) cito      (1000)    15484 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFieldStorageStandard.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     4641 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFuncs.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     1242 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestHTMLStatusCodes.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3057 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestHTMLTag.py
+-rw-r--r--   0 cito      (1000) cito      (1000)       21 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/Tests/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      156 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/WebUtils/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)     3272 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/XMLRPCServlet.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      593 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/__init__.py
+-rw-r--r--   0 cito      (1000) cito      (1000)      430 2023-04-27 19:05:03.000000 Webware-for-Python-3.0.9/webware/error404.html
```

### Comparing `Webware-for-Python-3.0.8/.pylintrc` & `Webware-for-Python-3.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/LICENSE` & `Webware-for-Python-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/PKG-INFO` & `Webware-for-Python-3.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Webware-for-Python
-Version: 3.0.8
+Version: 3.0.9
 Summary: Webware for Python is a time-tested modular, object-oriented web framework.
 Home-page: https://webwareforpython.github.io/w4py3/
 Author: Christoph Zwerschke et al.
 Author-email: cito@online.de
 License: UNKNOWN
 Project-URL: Source, https://github.com/WebwareForPython/w4py3
 Project-URL: Issues, https://github.com/WebwareForPython/w4py3/issues
```

### Comparing `Webware-for-Python-3.0.8/README.md` & `Webware-for-Python-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/Webware_for_Python.egg-info/PKG-INFO` & `Webware-for-Python-3.0.9/Webware_for_Python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Webware-for-Python
-Version: 3.0.8
+Version: 3.0.9
 Summary: Webware for Python is a time-tested modular, object-oriented web framework.
 Home-page: https://webwareforpython.github.io/w4py3/
 Author: Christoph Zwerschke et al.
 Author-email: cito@online.de
 License: UNKNOWN
 Project-URL: Source, https://github.com/WebwareForPython/w4py3
 Project-URL: Issues, https://github.com/WebwareForPython/w4py3/issues
```

### Comparing `Webware-for-Python-3.0.8/Webware_for_Python.egg-info/SOURCES.txt` & `Webware-for-Python-3.0.9/Webware_for_Python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/bin/editfile.py` & `Webware-for-Python-3.0.9/bin/editfile.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/Makefile` & `Webware-for-Python-3.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/appdev.rst` & `Webware-for-Python-3.0.9/docs/appdev.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/changes.rst` & `Webware-for-Python-3.0.9/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/conf.py` & `Webware-for-Python-3.0.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 project = 'Webware for Python 3'
 copyright = '1999-2023, Christoph Zwerschke et al'
 author = 'Christoph Zwerschke et al.'
 
 # The short X.Y version
 version = '3.0'
 # The full version, including alpha/beta/rc tags
-release = '3.0.8'
+release = '3.0.9'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `Webware-for-Python-3.0.8/docs/config.rst` & `Webware-for-Python-3.0.9/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/copyright.rst` & `Webware-for-Python-3.0.9/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/css/logo.png` & `Webware-for-Python-3.0.9/docs/css/logo.png`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/deploy.rst` & `Webware-for-Python-3.0.9/docs/deploy.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/install.rst` & `Webware-for-Python-3.0.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/make.bat` & `Webware-for-Python-3.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/migrate.rst` & `Webware-for-Python-3.0.9/docs/migrate.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/overview.rst` & `Webware-for-Python-3.0.9/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/plugins.rst` & `Webware-for-Python-3.0.9/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/psp.rst` & `Webware-for-Python-3.0.9/docs/psp.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/quickstart.rst` & `Webware-for-Python-3.0.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/ref/core/index.rst` & `Webware-for-Python-3.0.9/docs/ref/core/index.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/style.rst` & `Webware-for-Python-3.0.9/docs/style.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/taskkit.rst` & `Webware-for-Python-3.0.9/docs/taskkit.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/testing.rst` & `Webware-for-Python-3.0.9/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/tutorial.rst` & `Webware-for-Python-3.0.9/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/userkit.rst` & `Webware-for-Python-3.0.9/docs/userkit.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/docs/webutils.rst` & `Webware-for-Python-3.0.9/docs/webutils.rst`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/setup.py` & `Webware-for-Python-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/tox.ini` & `Webware-for-Python-3.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/AdminPage.py` & `Webware-for-Python-3.0.9/webware/Admin/AdminPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/AdminSecurity.py` & `Webware-for-Python-3.0.9/webware/Admin/AdminSecurity.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/AppControl.py` & `Webware-for-Python-3.0.9/webware/Admin/AppControl.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/DumpCSV.py` & `Webware-for-Python-3.0.9/webware/Admin/DumpCSV.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/EditFile.py` & `Webware-for-Python-3.0.9/webware/Admin/EditFile.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/Errors.py` & `Webware-for-Python-3.0.9/webware/Admin/Errors.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/LoginPage.py` & `Webware-for-Python-3.0.9/webware/Admin/LoginPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/Main.py` & `Webware-for-Python-3.0.9/webware/Admin/Main.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/PlugIns.py` & `Webware-for-Python-3.0.9/webware/Admin/PlugIns.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/ServletCache.py` & `Webware-for-Python-3.0.9/webware/Admin/ServletCache.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Admin/View.py` & `Webware-for-Python-3.0.9/webware/Admin/View.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Application.py` & `Webware-for-Python-3.0.9/webware/Application.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Configs/Application.config` & `Webware-for-Python-3.0.9/webware/Configs/Application.config`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/ConfigurableForServerSidePath.py` & `Webware-for-Python-3.0.9/webware/ConfigurableForServerSidePath.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Cookie.py` & `Webware-for-Python-3.0.9/webware/Cookie.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/AjaxPage.py` & `Webware-for-Python-3.0.9/webware/Examples/AjaxPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/AjaxSuggest.py` & `Webware-for-Python-3.0.9/webware/Examples/AjaxSuggest.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/Colorize.py` & `Webware-for-Python-3.0.9/webware/Examples/Colorize.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/Colors.py` & `Webware-for-Python-3.0.9/webware/Examples/Colors.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/CountVisits.py` & `Webware-for-Python-3.0.9/webware/Examples/CountVisits.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/DBUtilsDemo.py` & `Webware-for-Python-3.0.9/webware/Examples/DBUtilsDemo.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/DominateDemo.py` & `Webware-for-Python-3.0.9/webware/Examples/DominateDemo.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/Error.py` & `Webware-for-Python-3.0.9/webware/Examples/Error.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ExamplePage.py` & `Webware-for-Python-3.0.9/webware/Examples/ExamplePage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/FileUpload.py` & `Webware-for-Python-3.0.9/webware/Examples/FileUpload.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ImageDemo.py` & `Webware-for-Python-3.0.9/webware/Examples/ImageDemo.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/Introspect.py` & `Webware-for-Python-3.0.9/webware/Examples/Introspect.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/JSONRPCClient.py` & `Webware-for-Python-3.0.9/webware/Examples/JSONRPCClient.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/JSONRPCExample.py` & `Webware-for-Python-3.0.9/webware/Examples/JSONRPCExample.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ListBox.py` & `Webware-for-Python-3.0.9/webware/Examples/ListBox.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/LoginPage.py` & `Webware-for-Python-3.0.9/webware/Examples/LoginPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/PickleRPCExample.py` & `Webware-for-Python-3.0.9/webware/Examples/PickleRPCExample.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/PlugInInspector.py` & `Webware-for-Python-3.0.9/webware/Examples/PlugInInspector.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/PushServlet.py` & `Webware-for-Python-3.0.9/webware/Examples/PushServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/RequestInformation.py` & `Webware-for-Python-3.0.9/webware/Examples/RequestInformation.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/SecureCountVisits.py` & `Webware-for-Python-3.0.9/webware/Examples/SecureCountVisits.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/SecurePage.py` & `Webware-for-Python-3.0.9/webware/Examples/SecurePage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/View.py` & `Webware-for-Python-3.0.9/webware/Examples/View.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/Welcome.py` & `Webware-for-Python-3.0.9/webware/Examples/Welcome.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/XMLRPCExample.py` & `Webware-for-Python-3.0.9/webware/Examples/XMLRPCExample.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/YattagDemo.py` & `Webware-for-Python-3.0.9/webware/Examples/YattagDemo.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ajaxcall.js` & `Webware-for-Python-3.0.9/webware/Examples/ajaxcall.js`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ajaxpoll.js` & `Webware-for-Python-3.0.9/webware/Examples/ajaxpoll.js`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ajaxsuggest.css` & `Webware-for-Python-3.0.9/webware/Examples/ajaxsuggest.css`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/ajaxsuggest.js` & `Webware-for-Python-3.0.9/webware/Examples/ajaxsuggest.js`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/favicon.ico` & `Webware-for-Python-3.0.9/webware/Examples/favicon.ico`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/index.py` & `Webware-for-Python-3.0.9/webware/Examples/index.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Examples/jsonrpc.js` & `Webware-for-Python-3.0.9/webware/Examples/jsonrpc.js`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/ExceptionHandler.py` & `Webware-for-Python-3.0.9/webware/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/HTTPContent.py` & `Webware-for-Python-3.0.9/webware/HTTPContent.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/HTTPExceptions.py` & `Webware-for-Python-3.0.9/webware/HTTPExceptions.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/HTTPRequest.py` & `Webware-for-Python-3.0.9/webware/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/HTTPResponse.py` & `Webware-for-Python-3.0.9/webware/HTTPResponse.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/HTTPServlet.py` & `Webware-for-Python-3.0.9/webware/HTTPServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/ImportManager.py` & `Webware-for-Python-3.0.9/webware/ImportManager.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/JSONRPCServlet.py` & `Webware-for-Python-3.0.9/webware/JSONRPCServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/CSVJoiner.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/CSVJoiner.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/CSVParser.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/CSVParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Configurable.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Configurable.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/DBPool.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/DBPool.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/DataTable.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/DataTable.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/DateInterval.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/DateInterval.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/DateParser.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/DateParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/DictForArgs.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/DictForArgs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Error.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Error.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Funcs.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Funcs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/M2PickleRPC.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/M2PickleRPC.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/MixIn.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/MixIn.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/NamedValueAccess.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/NamedValueAccess.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/ParamFactory.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/ParamFactory.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/PickleCache.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/PickleCache.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/PickleRPC.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/PickleRPC.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/PropertiesObject.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/PropertiesObject.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/BenchCSVParser.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/BenchCSVParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/BenchDataTable.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/BenchDataTable.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/Sample.csv` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/Sample.csv`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/Sample.xls` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/Sample.xls`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestCSVParser.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestCSVParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDataTable.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDataTable.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDateInterval.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDateInterval.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDateParser.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDateParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestDictForArgs.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestDictForArgs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestError.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestError.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestFuncs.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestFuncs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestMixIn.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestMixIn.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestNamedValueAccess.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestNamedValueAccess.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/Tests/TestPickleCache.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/Tests/TestPickleCache.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MiscUtils/__init__.py` & `Webware-for-Python-3.0.9/webware/MiscUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/MockApplication.py` & `Webware-for-Python-3.0.9/webware/MockApplication.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/BraceConverter.py` & `Webware-for-Python-3.0.9/webware/PSP/BraceConverter.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/CompilePSP.py` & `Webware-for-Python-3.0.9/webware/PSP/CompilePSP.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Context.py` & `Webware-for-Python-3.0.9/webware/PSP/Context.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/Braces.psp` & `Webware-for-Python-3.0.9/webware/PSP/Examples/Braces.psp`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/Hello.psp` & `Webware-for-Python-3.0.9/webware/PSP/Examples/Hello.psp`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/PSPTests-Braces.psp` & `Webware-for-Python-3.0.9/webware/PSP/Examples/PSPTests-Braces.psp`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/PSPTests.psp` & `Webware-for-Python-3.0.9/webware/PSP/Examples/PSPTests.psp`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/View.py` & `Webware-for-Python-3.0.9/webware/PSP/Examples/View.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Examples/psplogo.png` & `Webware-for-Python-3.0.9/webware/PSP/Examples/psplogo.png`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Generators.py` & `Webware-for-Python-3.0.9/webware/PSP/Generators.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/PSPCompiler.py` & `Webware-for-Python-3.0.9/webware/PSP/PSPCompiler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/PSPPage.py` & `Webware-for-Python-3.0.9/webware/PSP/PSPPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/PSPParser.py` & `Webware-for-Python-3.0.9/webware/PSP/PSPParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/PSPServletFactory.py` & `Webware-for-Python-3.0.9/webware/PSP/PSPServletFactory.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/PSPUtils.py` & `Webware-for-Python-3.0.9/webware/PSP/PSPUtils.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/ParseEventHandler.py` & `Webware-for-Python-3.0.9/webware/PSP/ParseEventHandler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Properties.py` & `Webware-for-Python-3.0.9/webware/PSP/Properties.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/ServletWriter.py` & `Webware-for-Python-3.0.9/webware/PSP/ServletWriter.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/StreamReader.py` & `Webware-for-Python-3.0.9/webware/PSP/StreamReader.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Tests/TestBraceConverter.py` & `Webware-for-Python-3.0.9/webware/PSP/Tests/TestBraceConverter.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Tests/TestCompiler.py` & `Webware-for-Python-3.0.9/webware/PSP/Tests/TestCompiler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Tests/TestContext.py` & `Webware-for-Python-3.0.9/webware/PSP/Tests/TestContext.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PSP/Tests/TestUtils.py` & `Webware-for-Python-3.0.9/webware/PSP/Tests/TestUtils.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Page.py` & `Webware-for-Python-3.0.9/webware/Page.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PickleRPCServlet.py` & `Webware-for-Python-3.0.9/webware/PickleRPCServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PlugIn.py` & `Webware-for-Python-3.0.9/webware/PlugIn.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/PlugInLoader.py` & `Webware-for-Python-3.0.9/webware/PlugInLoader.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Properties.py` & `Webware-for-Python-3.0.9/webware/Properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name = 'Webware for Python'
 
-version = (3, 0, 8)
+version = (3, 0, 9)
 
 status = 'stable'
 
 requiredPyVersion = (3, 6)
 
 synopsis = (
     "Webware for Python is a time-tested"
```

### Comparing `Webware-for-Python-3.0.8/webware/RPCServlet.py` & `Webware-for-Python-3.0.9/webware/RPCServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Request.py` & `Webware-for-Python-3.0.9/webware/Request.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Response.py` & `Webware-for-Python-3.0.9/webware/Response.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Scripts/MakeAppWorkDir.py` & `Webware-for-Python-3.0.9/webware/Scripts/MakeAppWorkDir.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Scripts/WSGIScript.py` & `Webware-for-Python-3.0.9/webware/Scripts/WSGIScript.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Scripts/WaitressServer.py` & `Webware-for-Python-3.0.9/webware/Scripts/WaitressServer.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Scripts/WebwareCLI.py` & `Webware-for-Python-3.0.9/webware/Scripts/WebwareCLI.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Servlet.py` & `Webware-for-Python-3.0.9/webware/Servlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/ServletFactory.py` & `Webware-for-Python-3.0.9/webware/ServletFactory.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Session.py` & `Webware-for-Python-3.0.9/webware/Session.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionDynamicStore.py` & `Webware-for-Python-3.0.9/webware/SessionDynamicStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionFileStore.py` & `Webware-for-Python-3.0.9/webware/SessionFileStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionMemcachedStore.py` & `Webware-for-Python-3.0.9/webware/SessionMemcachedStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionMemoryStore.py` & `Webware-for-Python-3.0.9/webware/SessionMemoryStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionRedisStore.py` & `Webware-for-Python-3.0.9/webware/SessionRedisStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionShelveStore.py` & `Webware-for-Python-3.0.9/webware/SessionShelveStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SessionStore.py` & `Webware-for-Python-3.0.9/webware/SessionStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/SidebarPage.py` & `Webware-for-Python-3.0.9/webware/SidebarPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/TaskKit/Scheduler.py` & `Webware-for-Python-3.0.9/webware/TaskKit/Scheduler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/TaskKit/Task.py` & `Webware-for-Python-3.0.9/webware/TaskKit/Task.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/TaskKit/TaskHandler.py` & `Webware-for-Python-3.0.9/webware/TaskKit/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/TaskKit/Tests/SchedulerTest.py` & `Webware-for-Python-3.0.9/webware/TaskKit/Tests/SchedulerTest.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/DebugPage.py` & `Webware-for-Python-3.0.9/webware/Testing/DebugPage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/Dir/IncludeURLTest2.py` & `Webware-for-Python-3.0.9/webware/Testing/Dir/IncludeURLTest2.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/EmbeddedServlet.py` & `Webware-for-Python-3.0.9/webware/Testing/EmbeddedServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/FieldStorage.py` & `Webware-for-Python-3.0.9/webware/Testing/FieldStorage.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/IncludeURLTest.py` & `Webware-for-Python-3.0.9/webware/Testing/IncludeURLTest.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/Main.py` & `Webware-for-Python-3.0.9/webware/Testing/Main.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/ServletImport.py` & `Webware-for-Python-3.0.9/webware/Testing/ServletImport.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/SetCookie.py` & `Webware-for-Python-3.0.9/webware/Testing/SetCookie.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/TestCases.data` & `Webware-for-Python-3.0.9/webware/Testing/TestCases.data`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/TestIMS.py` & `Webware-for-Python-3.0.9/webware/Testing/TestIMS.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/URL/index.html` & `Webware-for-Python-3.0.9/webware/Testing/URL/index.html`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Testing/URL/util.py` & `Webware-for-Python-3.0.9/webware/Testing/URL/util.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/AppTest.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/AppTest.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestAdmin.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestAdmin.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestContextMap.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestContextMap.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestExamples.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestExamples.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestMakeApp.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestMakeApp.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestPSPExamples.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestPSPExamples.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestServer.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestServer.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestEndToEnd/TestTesting.py` & `Webware-for-Python-3.0.9/webware/Tests/TestEndToEnd/TestTesting.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestMocking.py` & `Webware-for-Python-3.0.9/webware/Tests/TestMocking.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/Application.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/Application.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/Session.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/Session.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSession.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSession.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionDynamicStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionDynamicStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionFileStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionFileStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionMemcachedStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionMemcachedStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionMemoryStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionMemoryStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionRedisStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionRedisStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionShelveStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionShelveStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/TestSessionStore.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/TestSessionStore.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/memcache.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/memcache.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Tests/TestSessions/redis.py` & `Webware-for-Python-3.0.9/webware/Tests/TestSessions/redis.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/Transaction.py` & `Webware-for-Python-3.0.9/webware/Transaction.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/URLParser.py` & `Webware-for-Python-3.0.9/webware/URLParser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UnknownFileTypeServlet.py` & `Webware-for-Python-3.0.9/webware/UnknownFileTypeServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/HierRole.py` & `Webware-for-Python-3.0.9/webware/UserKit/HierRole.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/Role.py` & `Webware-for-Python-3.0.9/webware/UserKit/Role.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/RoleUser.py` & `Webware-for-Python-3.0.9/webware/UserKit/RoleUser.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/RoleUserManagerMixIn.py` & `Webware-for-Python-3.0.9/webware/UserKit/RoleUserManagerMixIn.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/Tests/TestExample.py` & `Webware-for-Python-3.0.9/webware/UserKit/Tests/TestExample.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/Tests/TestRole.py` & `Webware-for-Python-3.0.9/webware/UserKit/Tests/TestRole.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/Tests/TestUserManager.py` & `Webware-for-Python-3.0.9/webware/UserKit/Tests/TestUserManager.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/User.py` & `Webware-for-Python-3.0.9/webware/UserKit/User.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/UserManager.py` & `Webware-for-Python-3.0.9/webware/UserKit/UserManager.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/UserKit/UserManagerToFile.py` & `Webware-for-Python-3.0.9/webware/UserKit/UserManagerToFile.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WSGIStreamOut.py` & `Webware-for-Python-3.0.9/webware/WSGIStreamOut.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/CGITraceback.py` & `Webware-for-Python-3.0.9/webware/WebUtils/CGITraceback.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/ExpansiveHTMLForException.py` & `Webware-for-Python-3.0.9/webware/WebUtils/ExpansiveHTMLForException.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/FieldStorage.py` & `Webware-for-Python-3.0.9/webware/WebUtils/FieldStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,16 @@
                 break
             if not self._binary_file:
                 # fix for https://github.com/python/cpython/issues/71964
                 try:
                     data = data.decode()
                 except UnicodeDecodeError:
                     self._binary_file = True
-            self.file = self.make_file()
+            if self.file is None:
+                self.file = self.make_file()
             self.file.write(data)
             todo -= len(data)
 
     def read_lines(self):
         """Internal: read lines until EOF or outerboundary."""
         self.file = self.__file = BytesIO(
             ) if self._binary_file else StringIO()
```

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Funcs.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Funcs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/HTMLForException.py` & `Webware-for-Python-3.0.9/webware/WebUtils/HTMLForException.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/HTMLTag.py` & `Webware-for-Python-3.0.9/webware/WebUtils/HTMLTag.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/HTTPStatusCodes.py` & `Webware-for-Python-3.0.9/webware/WebUtils/HTTPStatusCodes.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFieldStorageModified.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFieldStorageModified.py`

 * *Files 16% similar despite different names*

```diff
@@ -253,14 +253,94 @@
             'content-type': 'text/plain',
             'content-length': length})
         self.assertEqual(fs.type, 'text/plain')
         self.assertEqual(fs.length, length)
         self.assertEqual(fs.bytes_read, length)
         self.assertEqual(fs.file.read(), content)
 
+    def testPostRequestWithSmallPayloadWithContentLength(self):
+        length = 1000  # much smaller than buffer size
+        payload = 'x' * length
+        fs = FieldStorage(
+            fp=BytesIO(payload.encode()),
+            environ={'REQUEST_METHOD': 'POST',
+                     'CONTENT_TYPE': 'text/plain',
+                     'CONTENT_LENGTH': length})
+        self.assertEqual(fs.headers, {
+            'content-type': 'text/plain',
+            'content-length': length})
+        self.assertEqual(fs.type, 'text/plain')
+        self.assertEqual(fs.length, length)
+        self.assertEqual(fs.bytes_read, length)
+        self.assertEqual(fs.file.read(), payload)
+
+    def testPostRequestWithLargeTextPayloadWithContentLength(self):
+        length = 25000  # much larger than buffer size
+        payload = 'x' * length
+        fs = FieldStorage(
+            fp=BytesIO(payload.encode()),
+            environ={'REQUEST_METHOD': 'POST',
+                     'CONTENT_TYPE': 'text/plain',
+                     'CONTENT_LENGTH': length})
+        self.assertEqual(fs.headers, {
+            'content-type': 'text/plain',
+            'content-length': length})
+        self.assertEqual(fs.type, 'text/plain')
+        self.assertEqual(fs.length, length)
+        self.assertEqual(fs.bytes_read, length)
+        self.assertEqual(fs.file.read(), payload)
+
+    def testPostRequestWithLargeJsonPayloadWithContentLength(self):
+        # create JSON payload that is much larger than the buffer size
+        payload = {f'test{i}': str(i) * 5000 for i in range(5)}
+        payload = str(payload).replace("'", '"')
+        length = len(payload)
+        self.assertGreater(length, 25000)
+        fs = FieldStorage(
+            fp=BytesIO(payload.encode()),
+            environ={'REQUEST_METHOD': 'POST',
+                     'CONTENT_TYPE': 'application/json',
+                     'CONTENT_LENGTH': length})
+        self.assertEqual(fs.headers, {
+            'content-type': 'application/json',
+            'content-length': length})
+        self.assertEqual(fs.type, 'application/json')
+        self.assertEqual(fs.length, length)
+        self.assertEqual(fs.bytes_read, length)
+        # make sure that the original payload is preserved
+        self.assertEqual(fs.file.read(), payload)
+
+    def testPostRequestWithSmallPayloadWithoutContentLength(self):
+        length = 1000  # much smaller than buffer size
+        payload = 'x' * length
+        fs = FieldStorage(
+            fp=BytesIO(payload.encode()),
+            environ={'REQUEST_METHOD': 'POST',
+                     'CONTENT_TYPE': 'text/plain'})
+        self.assertEqual(fs.headers, {
+            'content-type': 'text/plain'})
+        self.assertEqual(fs.type, 'text/plain')
+        self.assertEqual(fs.length, -1)
+        self.assertEqual(fs.bytes_read, length)
+        self.assertEqual(fs.file.read(), payload)
+
+    def testPostRequestWithLargePayloadWithoutContentLength(self):
+        length = 25000  # much larger than buffer size
+        payload = 'x' * length
+        fs = FieldStorage(
+            fp=BytesIO(payload.encode()),
+            environ={'REQUEST_METHOD': 'POST',
+                     'CONTENT_TYPE': 'text/plain'})
+        self.assertEqual(fs.headers, {
+            'content-type': 'text/plain'})
+        self.assertEqual(fs.type, 'text/plain')
+        self.assertEqual(fs.length, -1)
+        self.assertEqual(fs.bytes_read, length)
+        self.assertEqual(fs.file.read(), payload)
+
     def testIsBinaryType(self):
         self.assertIs(isBinaryType('application/json'), False)
         self.assertIs(isBinaryType('application/xml'), False)
         self.assertIs(isBinaryType('application/calendar+json'), False)
         self.assertIs(isBinaryType('application/calendar+xml'), False)
         self.assertIs(isBinaryType('model/x3d+xml'), False)
         self.assertIs(isBinaryType('text/csv'), False)
```

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFieldStorageStandard.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFieldStorageStandard.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestFuncs.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestFuncs.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestHTMLStatusCodes.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestHTMLStatusCodes.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/WebUtils/Tests/TestHTMLTag.py` & `Webware-for-Python-3.0.9/webware/WebUtils/Tests/TestHTMLTag.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/XMLRPCServlet.py` & `Webware-for-Python-3.0.9/webware/XMLRPCServlet.py`

 * *Files identical despite different names*

### Comparing `Webware-for-Python-3.0.8/webware/__init__.py` & `Webware-for-Python-3.0.9/webware/__init__.py`

 * *Files identical despite different names*

