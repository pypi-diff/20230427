# Comparing `tmp/ims-bootstrap-5.0.1.tar.gz` & `tmp/ims-bootstrap-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ims-bootstrap-5.0.1.tar", last modified: Wed Feb 22 15:10:26 2023, max compression
+gzip compressed data, was "ims-bootstrap-5.0.2.tar", last modified: Thu Apr 27 13:35:18 2023, max compression
```

## Comparing `ims-bootstrap-5.0.1.tar` & `ims-bootstrap-5.0.2.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.609447 ims-bootstrap-5.0.1/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/LICENSE
--rw-rw----   0 ruttenb   (1328) ims        (100)       79 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/MANIFEST.in
--rw-r--r--   0 ruttenb   (1328) ims        (100)      582 2023-02-22 15:10:26.610439 ims-bootstrap-5.0.1/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)      190 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/README.md
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.616431 ims-bootstrap-5.0.1/bootstrap/
--rw-r--r--   0 ruttenb   (1328) ims        (100)      141 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      217 2021-08-11 13:49:47.000000 ims-bootstrap-5.0.1/bootstrap/apps.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.508456 ims-bootstrap-5.0.1/bootstrap/static/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.494429 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.868455 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/
--rw-r--r--   0 ruttenb   (1328) ims        (100)    71861 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   210357 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    53265 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   131395 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    71935 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   210361 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    53340 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   131472 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7965 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   110875 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)     6490 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)    40331 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7958 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   110888 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)     6562 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)    48693 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    76347 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   212450 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    58266 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   131956 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    76214 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   212393 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    58194 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   131791 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rwxr-xr-x   0 ruttenb   (1328) ims        (100)   237950 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   608300 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.css.map
--rwxr-xr-x   0 ruttenb   (1328) ims        (100)   194901 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   522639 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)   237528 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   608144 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)   195007 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   767483 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:25.018441 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/
--rw-rw----   0 ruttenb   (1328) ims        (100)    20127 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw----   0 ruttenb   (1328) ims        (100)   108738 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw----   0 ruttenb   (1328) ims        (100)    45404 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw----   0 ruttenb   (1328) ims        (100)    23424 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw----   0 ruttenb   (1328) ims        (100)    18028 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:25.132448 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/
--rw-r--r--   0 ruttenb   (1328) ims        (100)   207989 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   451770 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    80420 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   333078 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)   136215 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   308207 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0 ruttenb   (1328) ims        (100)    73978 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   221179 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.min.js.map
--rwxr-xr-x   0 ruttenb   (1328) ims        (100)   145543 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   309348 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.js.map
--rwxr-xr-x   0 ruttenb   (1328) ims        (100)    60404 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)   216913 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.min.js.map
--rw-rw----   0 ruttenb   (1328) ims        (100)     4591 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/respond.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     9004 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/respond.src.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.499436 ims-bootstrap-5.0.1/bootstrap/static/datepicker/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:25.378436 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/
--rw-rw----   0 ruttenb   (1328) ims        (100)    17190 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    18548 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.css.map
--rw-rw----   0 ruttenb   (1328) ims        (100)    15731 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.min.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    18056 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    20785 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css.map
--rw-rw----   0 ruttenb   (1328) ims        (100)    16452 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.min.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    22835 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    23849 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.css.map
--rw-rw----   0 ruttenb   (1328) ims        (100)    21100 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.min.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    23600 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    25703 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css.map
--rw-rw----   0 ruttenb   (1328) ims        (100)    21734 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.min.css
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:25.412429 ims-bootstrap-5.0.1/bootstrap/static/datepicker/js/
--rw-rw----   0 ruttenb   (1328) ims        (100)    77510 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/js/bootstrap-datepicker.js
--rw-rw----   0 ruttenb   (1328) ims        (100)    33693 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/js/bootstrap-datepicker.min.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:25.956433 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/
--rw-rw----   0 ruttenb   (1328) ims        (100)      636 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker-en-CA.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      704 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar-tn.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      531 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.az.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      615 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bg.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      562 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bm.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1210 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bn.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      510 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.br.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      475 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bs.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ca.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      536 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.cs.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      433 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.cy.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      514 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.da.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.de.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      764 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.el.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-AU.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-CA.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-GB.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-IE.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-NZ.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-ZA.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.eo.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.es.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      537 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.et.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.eu.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      670 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fa.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fi.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      488 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fo.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      512 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr-CH.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      536 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      489 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.gl.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      563 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.he.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      944 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hi.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      462 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hr.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      541 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hu.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      757 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hy.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      453 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.id.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      496 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.is.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      506 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.it-CH.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      525 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.it.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      502 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ja.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      970 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ka.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1076 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kh.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      649 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kk.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      945 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.km.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      532 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ko.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      575 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kr.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      565 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.lt.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      526 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.lv.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      493 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.me.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      657 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.mk.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      638 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.mn.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      448 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ms.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      462 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.nb.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      522 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl-BE.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.no.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.oc.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      552 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.pl.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      504 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.pt-BR.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      498 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.pt.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      505 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ro.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      662 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs-latin.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      817 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      731 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ru.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      988 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.si.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      497 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sk.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      455 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sl.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sq.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      478 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr-latin.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      651 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      492 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sv.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      431 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sw.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      934 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ta.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      700 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.tg.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      833 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.th.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      530 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.tk.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      495 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.tr.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      722 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uk.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      703 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      516 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-latn.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      551 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.vi.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      613 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-CN.min.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      566 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.505441 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.005507 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/css/
--rw-rw----   0 ruttenb   (1328) ims        (100)    37414 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/css/font-awesome.css
--rw-rw----   0 ruttenb   (1328) ims        (100)    31000 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/css/font-awesome.min.css
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.158433 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/
--rw-rw----   0 ruttenb   (1328) ims        (100)   134808 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/FontAwesome.otf
--rw-rw----   0 ruttenb   (1328) ims        (100)   165742 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.eot
--rw-rw----   0 ruttenb   (1328) ims        (100)   444379 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.svg
--rw-rw----   0 ruttenb   (1328) ims        (100)   165548 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.ttf
--rw-rw----   0 ruttenb   (1328) ims        (100)    98024 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff
--rw-rw----   0 ruttenb   (1328) ims        (100)    77160 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff2
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.223431 ims-bootstrap-5.0.1/bootstrap/static/jquery/
--rw-rw----   0 ruttenb   (1328) ims        (100)   268039 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/jquery/jquery.js
--rw-rw----   0 ruttenb   (1328) ims        (100)    86659 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/jquery/jquery.min.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.510470 ims-bootstrap-5.0.1/bootstrap/static/selectize/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.313436 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/
--rwxrwx---   0 ruttenb   (1328) ims        (100)    15477 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.bootstrap2.css
--rwxrwx---   0 ruttenb   (1328) ims        (100)    10602 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.bootstrap3.css
--rwxrwx---   0 ruttenb   (1328) ims        (100)     8425 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.css
--rwxrwx---   0 ruttenb   (1328) ims        (100)    11528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.default.css
--rwxrwx---   0 ruttenb   (1328) ims        (100)    10930 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.legacy.css
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.371434 ims-bootstrap-5.0.1/bootstrap/static/selectize/js/
--rwxrwx---   0 ruttenb   (1328) ims        (100)    98386 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/js/selectize.js
--rwxrwx---   0 ruttenb   (1328) ims        (100)    42321 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.1/bootstrap/static/selectize/js/selectize.min.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.529455 ims-bootstrap-5.0.1/bootstrap/templates/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.551433 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2709 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/field.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      725 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/field_readonly.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      627 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/form.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      942 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/pager.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      194 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/value.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.531433 ims-bootstrap-5.0.1/bootstrap/templates/django/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:24.533429 ims-bootstrap-5.0.1/bootstrap/templates/django/forms/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.556443 ims-bootstrap-5.0.1/bootstrap/templates/django/forms/widgets/
--rw-rw----   0 ruttenb   (1328) ims        (100)      417 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.1/bootstrap/templates/django/forms/widgets/attrs.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.587443 ims-bootstrap-5.0.1/bootstrap/templatetags/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.1/bootstrap/templatetags/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    10777 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/templatetags/bootstrap.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     8264 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.1/bootstrap/widgets.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-22 15:10:26.605435 ims-bootstrap-5.0.1/ims_bootstrap.egg-info/
--rw-rw----   0 ruttenb   (1328) ims        (100)      582 2023-02-22 15:10:11.000000 ims-bootstrap-5.0.1/ims_bootstrap.egg-info/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)    10903 2023-02-22 15:10:12.000000 ims-bootstrap-5.0.1/ims_bootstrap.egg-info/SOURCES.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-02-22 15:10:11.000000 ims-bootstrap-5.0.1/ims_bootstrap.egg-info/dependency_links.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)       10 2023-02-22 15:10:11.000000 ims-bootstrap-5.0.1/ims_bootstrap.egg-info/top_level.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)      385 2023-02-22 15:10:26.613430 ims-bootstrap-5.0.1/setup.cfg
--rw-rw----   0 ruttenb   (1328) ims        (100)      736 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.1/setup.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.106717 ims-bootstrap-5.0.2/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/LICENSE
+-rw-rw----   0 ruttenb   (1328) ims        (100)       79 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/MANIFEST.in
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      582 2023-04-27 13:35:18.107719 ims-bootstrap-5.0.2/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)      190 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/README.md
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.259720 ims-bootstrap-5.0.2/bootstrap/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      141 2023-04-27 13:34:54.000000 ims-bootstrap-5.0.2/bootstrap/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      217 2021-08-11 13:49:47.000000 ims-bootstrap-5.0.2/bootstrap/apps.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.215716 ims-bootstrap-5.0.2/bootstrap/static/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.202723 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.418713 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    71861 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   210357 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    53265 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   131395 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    71935 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   210361 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    53340 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   131472 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7965 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   110875 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     6490 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    40331 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7958 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   110888 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     6562 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    48693 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    76347 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   212450 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    58266 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   131956 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    76214 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   212393 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    58194 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   131791 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rwxr-xr-x   0 ruttenb   (1328) ims        (100)   237950 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   608300 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.css.map
+-rwxr-xr-x   0 ruttenb   (1328) ims        (100)   194901 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   522639 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   237528 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   608144 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   195007 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   767483 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.447714 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/
+-rw-rw----   0 ruttenb   (1328) ims        (100)    20127 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw----   0 ruttenb   (1328) ims        (100)   108738 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw----   0 ruttenb   (1328) ims        (100)    45404 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw----   0 ruttenb   (1328) ims        (100)    23424 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw----   0 ruttenb   (1328) ims        (100)    18028 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.518711 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   207989 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   451770 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    80420 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   333078 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   136215 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   308207 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    73978 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   221179 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.min.js.map
+-rwxr-xr-x   0 ruttenb   (1328) ims        (100)   145543 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   309348 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.js.map
+-rwxr-xr-x   0 ruttenb   (1328) ims        (100)    60404 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   216913 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw----   0 ruttenb   (1328) ims        (100)     4591 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/respond.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     9004 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/respond.src.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.208715 ims-bootstrap-5.0.2/bootstrap/static/datepicker/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.570720 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/
+-rw-rw----   0 ruttenb   (1328) ims        (100)    17190 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    18548 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.css.map
+-rw-rw----   0 ruttenb   (1328) ims        (100)    15731 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.min.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    18056 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    20785 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css.map
+-rw-rw----   0 ruttenb   (1328) ims        (100)    16452 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.min.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    22835 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    23849 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.css.map
+-rw-rw----   0 ruttenb   (1328) ims        (100)    21100 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.min.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    23600 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    25703 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css.map
+-rw-rw----   0 ruttenb   (1328) ims        (100)    21734 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.min.css
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.579713 ims-bootstrap-5.0.2/bootstrap/static/datepicker/js/
+-rw-rw----   0 ruttenb   (1328) ims        (100)    77510 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/js/bootstrap-datepicker.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)    33693 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/js/bootstrap-datepicker.min.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.946715 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      636 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker-en-CA.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      704 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      531 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.az.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      615 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bg.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      562 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bm.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1210 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bn.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      510 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.br.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      475 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bs.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ca.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      536 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.cs.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      433 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.cy.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      514 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.da.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.de.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      764 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.el.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-AU.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-CA.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-GB.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-IE.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      517 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.eo.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.es.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      537 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.et.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.eu.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      670 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fa.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fi.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      488 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fo.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      512 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      536 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      489 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.gl.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      563 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.he.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      944 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hi.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      462 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hr.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      541 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hu.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      757 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hy.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      453 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.id.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      496 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.is.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      506 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.it-CH.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      525 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.it.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      502 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ja.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      970 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ka.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1076 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kh.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      649 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kk.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      945 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.km.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      532 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ko.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      575 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kr.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      565 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.lt.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      526 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.lv.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      493 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.me.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      657 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.mk.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      638 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.mn.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      448 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ms.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      462 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.nb.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      522 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      513 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.no.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      515 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.oc.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      552 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.pl.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      504 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      498 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.pt.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      505 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ro.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      662 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      817 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      731 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ru.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      988 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.si.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      497 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sk.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      455 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sl.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      518 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sq.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      478 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      651 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      492 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sv.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      431 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sw.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      934 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ta.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      700 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.tg.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      833 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.th.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      530 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.tk.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      495 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.tr.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      722 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uk.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      703 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      516 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      551 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.vi.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      613 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      566 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.212726 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.955714 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/css/
+-rw-rw----   0 ruttenb   (1328) ims        (100)    37414 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/css/font-awesome.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)    31000 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/css/font-awesome.min.css
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.987717 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/
+-rw-rw----   0 ruttenb   (1328) ims        (100)   134808 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/FontAwesome.otf
+-rw-rw----   0 ruttenb   (1328) ims        (100)   165742 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.eot
+-rw-rw----   0 ruttenb   (1328) ims        (100)   444379 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.svg
+-rw-rw----   0 ruttenb   (1328) ims        (100)   165548 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.ttf
+-rw-rw----   0 ruttenb   (1328) ims        (100)    98024 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff
+-rw-rw----   0 ruttenb   (1328) ims        (100)    77160 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff2
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.998710 ims-bootstrap-5.0.2/bootstrap/static/jquery/
+-rw-rw----   0 ruttenb   (1328) ims        (100)   268039 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/jquery/jquery.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)    86659 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/jquery/jquery.min.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.218715 ims-bootstrap-5.0.2/bootstrap/static/selectize/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.024729 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    15477 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.bootstrap2.css
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    10602 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.bootstrap3.css
+-rwxrwx---   0 ruttenb   (1328) ims        (100)     8425 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.css
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    11528 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.default.css
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    10930 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.legacy.css
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.033731 ims-bootstrap-5.0.2/bootstrap/static/selectize/js/
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    98386 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/js/selectize.js
+-rwxrwx---   0 ruttenb   (1328) ims        (100)    42321 2019-12-09 20:42:30.000000 ims-bootstrap-5.0.2/bootstrap/static/selectize/js/selectize.min.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.222730 ims-bootstrap-5.0.2/bootstrap/templates/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.071716 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2709 2023-02-22 15:09:30.000000 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/field.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      725 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/field_readonly.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      627 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/form.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      942 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/pager.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      194 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/value.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.223720 ims-bootstrap-5.0.2/bootstrap/templates/django/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:17.224730 ims-bootstrap-5.0.2/bootstrap/templates/django/forms/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.076719 ims-bootstrap-5.0.2/bootstrap/templates/django/forms/widgets/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      417 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.2/bootstrap/templates/django/forms/widgets/attrs.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.084724 ims-bootstrap-5.0.2/bootstrap/templatetags/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.2/bootstrap/templatetags/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    10777 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/templatetags/bootstrap.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     8264 2022-12-02 18:39:43.000000 ims-bootstrap-5.0.2/bootstrap/widgets.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 13:35:18.102735 ims-bootstrap-5.0.2/ims_bootstrap.egg-info/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      582 2023-04-27 13:35:14.000000 ims-bootstrap-5.0.2/ims_bootstrap.egg-info/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)    10903 2023-04-27 13:35:14.000000 ims-bootstrap-5.0.2/ims_bootstrap.egg-info/SOURCES.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-04-27 13:35:14.000000 ims-bootstrap-5.0.2/ims_bootstrap.egg-info/dependency_links.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)       10 2023-04-27 13:35:14.000000 ims-bootstrap-5.0.2/ims_bootstrap.egg-info/top_level.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)      385 2023-04-27 13:35:18.109725 ims-bootstrap-5.0.2/setup.cfg
+-rw-rw----   0 ruttenb   (1328) ims        (100)      736 2019-12-09 20:42:31.000000 ims-bootstrap-5.0.2/setup.py
```

### Comparing `ims-bootstrap-5.0.1/LICENSE` & `ims-bootstrap-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/PKG-INFO` & `ims-bootstrap-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ims-bootstrap
-Version: 5.0.1
+Version: 5.0.2
 Summary: A collection of Django widgets and templatetags for Bootstrap integration.
 Home-page: https://github.com/imsweb/django-bootstrap
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.esm.min.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/bootstrap.min.js.map` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/respond.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/bootstrap/js/respond.src.js` & `ims-bootstrap-5.0.2/bootstrap/static/bootstrap/js/respond.src.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker.standalone.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css.map` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.css.map`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/css/bootstrap-datepicker3.standalone.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/js/bootstrap-datepicker.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/js/bootstrap-datepicker.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker-en-CA.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar-tn.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.az.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bg.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bm.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.bn.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ca.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.cs.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.da.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.de.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.el.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-AU.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-CA.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-GB.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-IE.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-NZ.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-ZA.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.eo.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.es.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.et.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.eu.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fa.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fi.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr-CH.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.he.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hi.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hu.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.hy.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.it.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ka.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kh.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kk.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.km.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ko.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.kr.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.lt.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.lv.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.mk.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.mn.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl-BE.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.no.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.oc.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.pl.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs-latin.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ru.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.si.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sq.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.ta.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.tg.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.th.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.tk.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uk.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-latn.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.vi.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-CN.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-TW.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/datepicker/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/css/font-awesome.css` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/css/font-awesome.min.css` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/FontAwesome.otf` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.eot` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.svg` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.ttf` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff2` & `ims-bootstrap-5.0.2/bootstrap/static/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/jquery/jquery.js` & `ims-bootstrap-5.0.2/bootstrap/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/jquery/jquery.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.bootstrap2.css` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.bootstrap3.css` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.css` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.default.css` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/css/selectize.legacy.css` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/js/selectize.js` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/js/selectize.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/static/selectize/js/selectize.min.js` & `ims-bootstrap-5.0.2/bootstrap/static/selectize/js/selectize.min.js`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/field.html` & `ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/field.html`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/field_readonly.html` & `ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/field_readonly.html`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/form.html` & `ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/form.html`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/templates/bootstrap/pager.html` & `ims-bootstrap-5.0.2/bootstrap/templates/bootstrap/pager.html`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/templatetags/bootstrap.py` & `ims-bootstrap-5.0.2/bootstrap/templatetags/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/bootstrap/widgets.py` & `ims-bootstrap-5.0.2/bootstrap/widgets.py`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/ims_bootstrap.egg-info/PKG-INFO` & `ims-bootstrap-5.0.2/ims_bootstrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ims-bootstrap
-Version: 5.0.1
+Version: 5.0.2
 Summary: A collection of Django widgets and templatetags for Bootstrap integration.
 Home-page: https://github.com/imsweb/django-bootstrap
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ims-bootstrap-5.0.1/ims_bootstrap.egg-info/SOURCES.txt` & `ims-bootstrap-5.0.2/ims_bootstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ims-bootstrap-5.0.1/setup.py` & `ims-bootstrap-5.0.2/setup.py`

 * *Files identical despite different names*

