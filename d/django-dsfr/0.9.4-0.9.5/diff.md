# Comparing `tmp/django_dsfr-0.9.4.tar.gz` & `tmp/django_dsfr-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dsfr-0.9.4.tar", max compression
+gzip compressed data, was "django_dsfr-0.9.5.tar", max compression
```

## Comparing `django_dsfr-0.9.4.tar` & `django_dsfr-0.9.5.tar`

### file list

```diff
@@ -1,1657 +1,1657 @@
--rw-r--r--   0        0        0     1190 2022-10-17 16:38:19.493122 django_dsfr-0.9.4/LICENSE
--rw-r--r--   0        0        0     2781 2022-10-17 16:38:19.493122 django_dsfr-0.9.4/README.rst
--rw-r--r--   0        0        0        0 2022-10-17 16:38:19.493122 django_dsfr-0.9.4/dsfr/__init__.py
--rw-r--r--   0        0        0      666 2022-10-17 16:38:19.493122 django_dsfr-0.9.4/dsfr/admin.py
--rw-r--r--   0        0        0      193 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/apps.py
--rw-r--r--   0        0        0      152 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/context_processors.py
--rw-r--r--   0        0        0      454 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/fixtures/init.json
--rw-r--r--   0        0        0     1540 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/forms.py
--rw-r--r--   0        0        0     1798 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/migrations/0001_initial.py
--rw-r--r--   0        0        0     2254 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/migrations/0002_auto_20211209_1557.py
--rw-r--r--   0        0        0      553 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py
--rw-r--r--   0        0        0        0 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/migrations/__init__.py
--rw-r--r--   0        0        0     1855 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/models.py
--rw-r--r--   0        0        0      469 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/README.md
--rw-r--r--   0        0        0    16409 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/background/ovoid.svg
--rw-r--r--   0        0        0     4127 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/dark.svg
--rw-r--r--   0        0        0     4958 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/light.svg
--rw-r--r--   0        0        0    15223 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/system.svg
--rw-r--r--   0        0        0     2317 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/technical-error.svg
--rw-r--r--   0        0        0     4967 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/test.svg
--rw-r--r--   0        0        0      964 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/README.md
--rw-r--r--   0        0        0     1145 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/README.md
--rw-r--r--   0        0        0     4006 2022-10-17 16:38:19.497122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.css
--rw-r--r--   0        0        0    46932 2022-10-17 16:38:19.501122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.css.map
--rw-r--r--   0        0        0     1422 2022-10-17 16:38:19.501122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css
--rw-r--r--   0        0        0    23139 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css.map
--rw-r--r--   0        0        0     1090 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css
--rw-r--r--   0        0        0    22480 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css.map
--rw-r--r--   0        0        0     2843 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.css
--rw-r--r--   0        0        0    41772 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.css.map
--rw-r--r--   0        0        0     2271 2022-10-17 16:38:19.505122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css
--rw-r--r--   0        0        0    41227 2022-10-17 16:38:19.509122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css.map
--rw-r--r--   0        0        0     3133 2022-10-17 16:38:19.509122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.min.css
--rw-r--r--   0        0        0    45730 2022-10-17 16:38:19.509122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.min.css.map
--rw-r--r--   0        0        0      913 2022-10-17 16:38:19.509122 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.js
--rw-r--r--   0        0        0     2596 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.js.map
--rw-r--r--   0        0        0      619 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js
--rw-r--r--   0        0        0     2258 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js.map
--rw-r--r--   0        0        0     1561 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js
--rw-r--r--   0        0        0     2552 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js.map
--rw-r--r--   0        0        0      875 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js
--rw-r--r--   0        0        0     2288 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js.map
--rw-r--r--   0        0        0      732 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/README.md
--rw-r--r--   0        0        0     6219 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.css
--rw-r--r--   0        0        0    44082 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.css.map
--rw-r--r--   0        0        0     2205 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.css
--rw-r--r--   0        0        0    24264 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.css.map
--rw-r--r--   0        0        0     1591 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css
--rw-r--r--   0        0        0    23737 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css.map
--rw-r--r--   0        0        0     4255 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.css
--rw-r--r--   0        0        0    37199 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.css.map
--rw-r--r--   0        0        0     3510 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.min.css
--rw-r--r--   0        0        0    36557 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.min.css.map
--rw-r--r--   0        0        0     4873 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.min.css
--rw-r--r--   0        0        0    42896 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.min.css.map
--rw-r--r--   0        0        0      670 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/README.md
--rw-r--r--   0        0        0    15641 2022-10-17 16:38:19.513121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.css
--rw-r--r--   0        0        0    71605 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.css.map
--rw-r--r--   0        0        0     3928 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.css
--rw-r--r--   0        0        0    31260 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.css.map
--rw-r--r--   0        0        0     3116 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css
--rw-r--r--   0        0        0    31066 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css.map
--rw-r--r--   0        0        0    11954 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.css
--rw-r--r--   0        0        0    60075 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.css.map
--rw-r--r--   0        0        0    10542 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.min.css
--rw-r--r--   0        0        0    59256 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.min.css.map
--rw-r--r--   0        0        0    13430 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.min.css
--rw-r--r--   0        0        0    70608 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.min.css.map
--rw-r--r--   0        0        0     1179 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/README.md
--rw-r--r--   0        0        0     3808 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css
--rw-r--r--   0        0        0    38146 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css.map
--rw-r--r--   0        0        0     1026 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css
--rw-r--r--   0        0        0    22443 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css.map
--rw-r--r--   0        0        0      784 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css
--rw-r--r--   0        0        0    21919 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css.map
--rw-r--r--   0        0        0     3041 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css
--rw-r--r--   0        0        0    34129 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css.map
--rw-r--r--   0        0        0     2283 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css
--rw-r--r--   0        0        0    33545 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css.map
--rw-r--r--   0        0        0     2839 2022-10-17 16:38:19.517121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css
--rw-r--r--   0        0        0    37041 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css.map
--rw-r--r--   0        0        0     2225 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js
--rw-r--r--   0        0        0     6007 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js.map
--rw-r--r--   0        0        0     1462 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js
--rw-r--r--   0        0        0     4793 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js.map
--rw-r--r--   0        0        0     3421 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js
--rw-r--r--   0        0        0     5944 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js.map
--rw-r--r--   0        0        0     1957 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js
--rw-r--r--   0        0        0     4880 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js.map
--rw-r--r--   0        0        0     1115 2022-10-17 16:38:19.521121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/README.md
--rw-r--r--   0        0        0    39219 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.css
--rw-r--r--   0        0        0   106440 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.css.map
--rw-r--r--   0        0        0     9674 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.css
--rw-r--r--   0        0        0    40803 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.css.map
--rw-r--r--   0        0        0     8440 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.min.css
--rw-r--r--   0        0        0    40562 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.min.css.map
--rw-r--r--   0        0        0    29786 2022-10-17 16:38:19.525121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.css
--rw-r--r--   0        0        0    85565 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.css.map
--rw-r--r--   0        0        0    26098 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.min.css
--rw-r--r--   0        0        0    84202 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.min.css.map
--rw-r--r--   0        0        0    34310 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.min.css
--rw-r--r--   0        0        0   104814 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.min.css.map
--rw-r--r--   0        0        0      761 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.js
--rw-r--r--   0        0        0     1961 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.js.map
--rw-r--r--   0        0        0      559 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.min.js
--rw-r--r--   0        0        0     1692 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.min.js.map
--rw-r--r--   0        0        0      834 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.js
--rw-r--r--   0        0        0     1943 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.js.map
--rw-r--r--   0        0        0      583 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js
--rw-r--r--   0        0        0     1699 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js.map
--rw-r--r--   0        0        0      791 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/README.md
--rw-r--r--   0        0        0     9442 2022-10-17 16:38:19.529121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.css
--rw-r--r--   0        0        0    39264 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.css.map
--rw-r--r--   0        0        0     2612 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.css
--rw-r--r--   0        0        0    23866 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.css.map
--rw-r--r--   0        0        0     2091 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css
--rw-r--r--   0        0        0    23758 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css.map
--rw-r--r--   0        0        0     7070 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.css
--rw-r--r--   0        0        0    30331 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.css.map
--rw-r--r--   0        0        0     6203 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.min.css
--rw-r--r--   0        0        0    29713 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.min.css.map
--rw-r--r--   0        0        0     8066 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.min.css
--rw-r--r--   0        0        0    38530 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.min.css.map
--rw-r--r--   0        0        0     1070 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/README.md
--rw-r--r--   0        0        0    10928 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.css
--rw-r--r--   0        0        0    62169 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.css.map
--rw-r--r--   0        0        0     1686 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.css
--rw-r--r--   0        0        0    21335 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.css.map
--rw-r--r--   0        0        0     1328 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.min.css
--rw-r--r--   0        0        0    21256 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.min.css.map
--rw-r--r--   0        0        0     9483 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.css
--rw-r--r--   0        0        0    55982 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.css.map
--rw-r--r--   0        0        0     7972 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.min.css
--rw-r--r--   0        0        0    54994 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.min.css.map
--rw-r--r--   0        0        0     9072 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.min.css
--rw-r--r--   0        0        0    61094 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.min.css.map
--rw-r--r--   0        0        0      970 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/README.md
--rw-r--r--   0        0        0     7827 2022-10-17 16:38:19.533121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.css
--rw-r--r--   0        0        0    38280 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.css.map
--rw-r--r--   0        0        0     2384 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css
--rw-r--r--   0        0        0    20619 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css.map
--rw-r--r--   0        0        0     1518 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css
--rw-r--r--   0        0        0    20480 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css.map
--rw-r--r--   0        0        0     5770 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css
--rw-r--r--   0        0        0    33762 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css.map
--rw-r--r--   0        0        0     3809 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css
--rw-r--r--   0        0        0    32947 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css.map
--rw-r--r--   0        0        0     5099 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css
--rw-r--r--   0        0        0    37353 2022-10-17 16:38:19.537121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css.map
--rw-r--r--   0        0        0   410184 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.css
--rw-r--r--   0        0        0   920455 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.css.map
--rw-r--r--   0        0        0   108837 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.css
--rw-r--r--   0        0        0   317932 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.css.map
--rw-r--r--   0        0        0    85909 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.min.css
--rw-r--r--   0        0        0   305852 2022-10-17 16:38:19.541121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.min.css.map
--rw-r--r--   0        0        0   303311 2022-10-17 16:38:19.545121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.css
--rw-r--r--   0        0        0   675083 2022-10-17 16:38:19.545121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.css.map
--rw-r--r--   0        0        0   248216 2022-10-17 16:38:19.545121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.min.css
--rw-r--r--   0        0        0   640056 2022-10-17 16:38:19.545121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.min.css.map
--rw-r--r--   0        0        0   333239 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.min.css
--rw-r--r--   0        0        0   877679 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.min.css.map
--rw-r--r--   0        0        0    39818 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.js
--rw-r--r--   0        0        0   102818 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.js.map
--rw-r--r--   0        0        0    25225 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.min.js
--rw-r--r--   0        0        0    79906 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.min.js.map
--rw-r--r--   0        0        0    59695 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.js
--rw-r--r--   0        0        0   100791 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.js.map
--rw-r--r--   0        0        0    33147 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.min.js
--rw-r--r--   0        0        0    80290 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.min.js.map
--rw-r--r--   0        0        0      702 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/README.md
--rw-r--r--   0        0        0     8502 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.css
--rw-r--r--   0        0        0    38832 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.css.map
--rw-r--r--   0        0        0      990 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.css
--rw-r--r--   0        0        0    16990 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.css.map
--rw-r--r--   0        0        0      837 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css
--rw-r--r--   0        0        0    16973 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css.map
--rw-r--r--   0        0        0     7753 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.css
--rw-r--r--   0        0        0    34706 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.css.map
--rw-r--r--   0        0        0     7308 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.min.css
--rw-r--r--   0        0        0    34180 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.min.css.map
--rw-r--r--   0        0        0     7917 2022-10-17 16:38:19.549121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.min.css
--rw-r--r--   0        0        0    38280 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.min.css.map
--rw-r--r--   0        0        0     1494 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/README.md
--rw-r--r--   0        0        0     9546 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.css
--rw-r--r--   0        0        0    63891 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.css.map
--rw-r--r--   0        0        0     1832 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.css
--rw-r--r--   0        0        0    21340 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.css.map
--rw-r--r--   0        0        0     1575 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css
--rw-r--r--   0        0        0    21317 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css.map
--rw-r--r--   0        0        0     7954 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.css
--rw-r--r--   0        0        0    57724 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.css.map
--rw-r--r--   0        0        0     6348 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.min.css
--rw-r--r--   0        0        0    56970 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.min.css.map
--rw-r--r--   0        0        0     7695 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.min.css
--rw-r--r--   0        0        0    63102 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.min.css.map
--rw-r--r--   0        0        0      868 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/README.md
--rw-r--r--   0        0        0     6585 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.css
--rw-r--r--   0        0        0    49482 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.css.map
--rw-r--r--   0        0        0     2287 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.css
--rw-r--r--   0        0        0    21297 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.css.map
--rw-r--r--   0        0        0     1955 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.min.css
--rw-r--r--   0        0        0    21246 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.min.css.map
--rw-r--r--   0        0        0     4539 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.css
--rw-r--r--   0        0        0    42935 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.css.map
--rw-r--r--   0        0        0     3834 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.min.css
--rw-r--r--   0        0        0    42175 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.min.css.map
--rw-r--r--   0        0        0     5561 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.min.css
--rw-r--r--   0        0        0    48661 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.min.css.map
--rw-r--r--   0        0        0     1462 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/README.md
--rw-r--r--   0        0        0     2053 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.js
--rw-r--r--   0        0        0     5375 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.js.map
--rw-r--r--   0        0        0     1378 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.min.js
--rw-r--r--   0        0        0     4408 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.min.js.map
--rw-r--r--   0        0        0     3304 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.js
--rw-r--r--   0        0        0     5308 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.js.map
--rw-r--r--   0        0        0     1891 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js
--rw-r--r--   0        0        0     4467 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js.map
--rw-r--r--   0        0        0     1098 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/README.md
--rw-r--r--   0        0        0     5134 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.css
--rw-r--r--   0        0        0    45037 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.css.map
--rw-r--r--   0        0        0     4331 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.min.css
--rw-r--r--   0        0        0    44381 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.min.css.map
--rw-r--r--   0        0        0     3351 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.js
--rw-r--r--   0        0        0     8599 2022-10-17 16:38:19.553121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.js.map
--rw-r--r--   0        0        0     2150 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.min.js
--rw-r--r--   0        0        0     6818 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.min.js.map
--rw-r--r--   0        0        0     4446 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.js
--rw-r--r--   0        0        0     8460 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.js.map
--rw-r--r--   0        0        0     2531 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js
--rw-r--r--   0        0        0     6863 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js.map
--rw-r--r--   0        0        0     1061 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/README.md
--rw-r--r--   0        0        0    19629 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.css
--rw-r--r--   0        0        0    81515 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.css.map
--rw-r--r--   0        0        0     7301 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.css
--rw-r--r--   0        0        0    32183 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.css.map
--rw-r--r--   0        0        0     6007 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css
--rw-r--r--   0        0        0    31290 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css.map
--rw-r--r--   0        0        0    12587 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.css
--rw-r--r--   0        0        0    65641 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.css.map
--rw-r--r--   0        0        0    10004 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.min.css
--rw-r--r--   0        0        0    63612 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.min.css.map
--rw-r--r--   0        0        0    15783 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.min.css
--rw-r--r--   0        0        0    79221 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.min.css.map
--rw-r--r--   0        0        0      933 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/README.md
--rw-r--r--   0        0        0    11645 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.css
--rw-r--r--   0        0        0    61397 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.css.map
--rw-r--r--   0        0        0     1296 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.css
--rw-r--r--   0        0        0    22953 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.css.map
--rw-r--r--   0        0        0      966 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css
--rw-r--r--   0        0        0    22439 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css.map
--rw-r--r--   0        0        0    10608 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.css
--rw-r--r--   0        0        0    57898 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.css.map
--rw-r--r--   0        0        0     7180 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.min.css
--rw-r--r--   0        0        0    56275 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.min.css.map
--rw-r--r--   0        0        0     7918 2022-10-17 16:38:19.557121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.min.css
--rw-r--r--   0        0        0    59261 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.min.css.map
--rw-r--r--   0        0        0      563 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/README.md
--rw-r--r--   0        0        0     8815 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.css
--rw-r--r--   0        0        0    49398 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.css.map
--rw-r--r--   0        0        0     2826 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.css
--rw-r--r--   0        0        0    23948 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.css.map
--rw-r--r--   0        0        0     1491 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.min.css
--rw-r--r--   0        0        0    23610 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.min.css.map
--rw-r--r--   0        0        0     6319 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.css
--rw-r--r--   0        0        0    41901 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.css.map
--rw-r--r--   0        0        0     4309 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.min.css
--rw-r--r--   0        0        0    40971 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.min.css.map
--rw-r--r--   0        0        0     5572 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.min.css
--rw-r--r--   0        0        0    48171 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.min.css.map
--rw-r--r--   0        0        0     2239 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/README.md
--rw-r--r--   0        0        0    23738 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.css
--rw-r--r--   0        0        0    93426 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.css.map
--rw-r--r--   0        0        0     6650 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.css
--rw-r--r--   0        0        0    39667 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.css.map
--rw-r--r--   0        0        0     5511 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.min.css
--rw-r--r--   0        0        0    39340 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.min.css.map
--rw-r--r--   0        0        0    17329 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.css
--rw-r--r--   0        0        0    78442 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.css.map
--rw-r--r--   0        0        0    14644 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.min.css
--rw-r--r--   0        0        0    77171 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.min.css.map
--rw-r--r--   0        0        0    19927 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.min.css
--rw-r--r--   0        0        0    91812 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.min.css.map
--rw-r--r--   0        0        0     3409 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.js
--rw-r--r--   0        0        0     8125 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.js.map
--rw-r--r--   0        0        0     2352 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.min.js
--rw-r--r--   0        0        0     6627 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.min.js.map
--rw-r--r--   0        0        0     4882 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.js
--rw-r--r--   0        0        0     7940 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.js.map
--rw-r--r--   0        0        0     2896 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js
--rw-r--r--   0        0        0     6632 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js.map
--rw-r--r--   0        0        0      704 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/README.md
--rw-r--r--   0        0        0     4095 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.css
--rw-r--r--   0        0        0    25802 2022-10-17 16:38:19.561121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.css.map
--rw-r--r--   0        0        0     1888 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css
--rw-r--r--   0        0        0    15944 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css.map
--rw-r--r--   0        0        0     1570 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css
--rw-r--r--   0        0        0    15859 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css.map
--rw-r--r--   0        0        0     2447 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.css
--rw-r--r--   0        0        0    20905 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.css.map
--rw-r--r--   0        0        0     2134 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css
--rw-r--r--   0        0        0    20344 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css.map
--rw-r--r--   0        0        0     3476 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.min.css
--rw-r--r--   0        0        0    25147 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.min.css.map
--rw-r--r--   0        0        0      804 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/README.md
--rw-r--r--   0        0        0     7031 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.css
--rw-r--r--   0        0        0    44445 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.css.map
--rw-r--r--   0        0        0     2529 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.css
--rw-r--r--   0        0        0    21651 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.css.map
--rw-r--r--   0        0        0     1809 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.min.css
--rw-r--r--   0        0        0    21482 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.min.css.map
--rw-r--r--   0        0        0     5031 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.css
--rw-r--r--   0        0        0    39484 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.css.map
--rw-r--r--   0        0        0     3993 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.min.css
--rw-r--r--   0        0        0    38818 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.min.css.map
--rw-r--r--   0        0        0     5437 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.min.css
--rw-r--r--   0        0        0    43676 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.min.css.map
--rw-r--r--   0        0        0      785 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/README.md
--rw-r--r--   0        0        0     9985 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.css
--rw-r--r--   0        0        0    56085 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.css.map
--rw-r--r--   0        0        0     1781 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.css
--rw-r--r--   0        0        0    24978 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.css.map
--rw-r--r--   0        0        0     1273 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.min.css
--rw-r--r--   0        0        0    24813 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.min.css.map
--rw-r--r--   0        0        0     8445 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.css
--rw-r--r--   0        0        0    50271 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.css.map
--rw-r--r--   0        0        0     7364 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.min.css
--rw-r--r--   0        0        0    49346 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.min.css.map
--rw-r--r--   0        0        0     8409 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.min.css
--rw-r--r--   0        0        0    54985 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.min.css.map
--rw-r--r--   0        0        0      435 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/README.md
--rw-r--r--   0        0        0    12189 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.css
--rw-r--r--   0        0        0    40172 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.css.map
--rw-r--r--   0        0        0      428 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.css
--rw-r--r--   0        0        0    12090 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.css.map
--rw-r--r--   0        0        0      383 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css
--rw-r--r--   0        0        0    12090 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css.map
--rw-r--r--   0        0        0    12001 2022-10-17 16:38:19.565121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.css
--rw-r--r--   0        0        0    38695 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.css.map
--rw-r--r--   0        0        0    11538 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.min.css
--rw-r--r--   0        0        0    38182 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.min.css.map
--rw-r--r--   0        0        0    11693 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.min.css
--rw-r--r--   0        0        0    39650 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.min.css.map
--rw-r--r--   0        0        0     1389 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/README.md
--rw-r--r--   0        0        0     3843 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.css
--rw-r--r--   0        0        0    38267 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.css.map
--rw-r--r--   0        0        0      617 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.css
--rw-r--r--   0        0        0    14164 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.css.map
--rw-r--r--   0        0        0      528 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css
--rw-r--r--   0        0        0    14151 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css.map
--rw-r--r--   0        0        0     3487 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.css
--rw-r--r--   0        0        0    35627 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.css.map
--rw-r--r--   0        0        0     2669 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.min.css
--rw-r--r--   0        0        0    34970 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.min.css.map
--rw-r--r--   0        0        0     2953 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.min.css
--rw-r--r--   0        0        0    37591 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.min.css.map
--rw-r--r--   0        0        0     9842 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.js
--rw-r--r--   0        0        0    24837 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.js.map
--rw-r--r--   0        0        0     6081 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.min.js
--rw-r--r--   0        0        0    19410 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.min.js.map
--rw-r--r--   0        0        0    13564 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js
--rw-r--r--   0        0        0    24406 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js.map
--rw-r--r--   0        0        0     7638 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js
--rw-r--r--   0        0        0    19511 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js.map
--rw-r--r--   0        0        0     1420 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/README.md
--rw-r--r--   0        0        0    10943 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.css
--rw-r--r--   0        0        0    64082 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.css.map
--rw-r--r--   0        0        0     3254 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css
--rw-r--r--   0        0        0    33315 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css.map
--rw-r--r--   0        0        0     2439 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css
--rw-r--r--   0        0        0    33110 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css.map
--rw-r--r--   0        0        0     7948 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.css
--rw-r--r--   0        0        0    54402 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.css.map
--rw-r--r--   0        0        0     6386 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css
--rw-r--r--   0        0        0    53605 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css.map
--rw-r--r--   0        0        0     8597 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.min.css
--rw-r--r--   0        0        0    63083 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.min.css.map
--rw-r--r--   0        0        0     4296 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.js
--rw-r--r--   0        0        0    11212 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.js.map
--rw-r--r--   0        0        0     2911 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js
--rw-r--r--   0        0        0     9075 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js.map
--rw-r--r--   0        0        0     6425 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js
--rw-r--r--   0        0        0    11074 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js.map
--rw-r--r--   0        0        0     3750 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js
--rw-r--r--   0        0        0     9158 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js.map
--rw-r--r--   0        0        0      774 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/README.md
--rw-r--r--   0        0        0     3193 2022-10-17 16:38:19.569121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.css
--rw-r--r--   0        0        0    38972 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.css.map
--rw-r--r--   0        0        0     1096 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.css
--rw-r--r--   0        0        0    21520 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.css.map
--rw-r--r--   0        0        0      870 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css
--rw-r--r--   0        0        0    21507 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css.map
--rw-r--r--   0        0        0     2338 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.css
--rw-r--r--   0        0        0    34384 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.css.map
--rw-r--r--   0        0        0     1892 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.min.css
--rw-r--r--   0        0        0    33880 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.min.css.map
--rw-r--r--   0        0        0     2534 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.min.css
--rw-r--r--   0        0        0    38444 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.min.css.map
--rw-r--r--   0        0        0      709 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/README.md
--rw-r--r--   0        0        0    14519 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.css
--rw-r--r--   0        0        0    70844 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.css.map
--rw-r--r--   0        0        0     2837 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css
--rw-r--r--   0        0        0    29987 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css.map
--rw-r--r--   0        0        0     2259 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css
--rw-r--r--   0        0        0    29890 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css.map
--rw-r--r--   0        0        0    11941 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.css
--rw-r--r--   0        0        0    62771 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.css.map
--rw-r--r--   0        0        0     9783 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css
--rw-r--r--   0        0        0    62033 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css.map
--rw-r--r--   0        0        0    11814 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.min.css
--rw-r--r--   0        0        0    70005 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.min.css.map
--rw-r--r--   0        0        0      731 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/README.md
--rw-r--r--   0        0        0     6491 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.css
--rw-r--r--   0        0        0    44939 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.css.map
--rw-r--r--   0        0        0     1930 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.css
--rw-r--r--   0        0        0    20637 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.css.map
--rw-r--r--   0        0        0     1481 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css
--rw-r--r--   0        0        0    20530 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css.map
--rw-r--r--   0        0        0     4801 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.css
--rw-r--r--   0        0        0    37836 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.css.map
--rw-r--r--   0        0        0     3971 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.min.css
--rw-r--r--   0        0        0    37165 2022-10-17 16:38:19.573121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.min.css.map
--rw-r--r--   0        0        0     5224 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.min.css
--rw-r--r--   0        0        0    44153 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.min.css.map
--rw-r--r--   0        0        0      914 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/README.md
--rw-r--r--   0        0        0    11535 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.css
--rw-r--r--   0        0        0    51985 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.css.map
--rw-r--r--   0        0        0     3317 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.css
--rw-r--r--   0        0        0    27939 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.css.map
--rw-r--r--   0        0        0     2483 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css
--rw-r--r--   0        0        0    24727 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css.map
--rw-r--r--   0        0        0     8536 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.css
--rw-r--r--   0        0        0    45337 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.css.map
--rw-r--r--   0        0        0     6356 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.min.css
--rw-r--r--   0        0        0    41003 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.min.css.map
--rw-r--r--   0        0        0     8611 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.min.css
--rw-r--r--   0        0        0    47500 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.min.css.map
--rw-r--r--   0        0        0      979 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/README.md
--rw-r--r--   0        0        0     3247 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.css
--rw-r--r--   0        0        0    35926 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.css.map
--rw-r--r--   0        0        0     1071 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.css
--rw-r--r--   0        0        0    17968 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.css.map
--rw-r--r--   0        0        0      778 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.min.css
--rw-r--r--   0        0        0    17911 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.min.css.map
--rw-r--r--   0        0        0     2465 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.css
--rw-r--r--   0        0        0    32282 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.css.map
--rw-r--r--   0        0        0     1726 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.min.css
--rw-r--r--   0        0        0    31706 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.min.css.map
--rw-r--r--   0        0        0     2276 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.min.css
--rw-r--r--   0        0        0    35306 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.min.css.map
--rw-r--r--   0        0        0      752 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/README.md
--rw-r--r--   0        0        0     4577 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.css
--rw-r--r--   0        0        0    32295 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.css.map
--rw-r--r--   0        0        0     1876 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.css
--rw-r--r--   0        0        0    19721 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.css.map
--rw-r--r--   0        0        0     1276 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.min.css
--rw-r--r--   0        0        0    19610 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.min.css.map
--rw-r--r--   0        0        0     2980 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.css
--rw-r--r--   0        0        0    27997 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.css.map
--rw-r--r--   0        0        0     2363 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.min.css
--rw-r--r--   0        0        0    27461 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.min.css.map
--rw-r--r--   0        0        0     3411 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.min.css
--rw-r--r--   0        0        0    31667 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.min.css.map
--rw-r--r--   0        0        0      879 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/README.md
--rw-r--r--   0        0        0    11034 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.css
--rw-r--r--   0        0        0    61215 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.css.map
--rw-r--r--   0        0        0     3247 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.css
--rw-r--r--   0        0        0    24012 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.css.map
--rw-r--r--   0        0        0     2667 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.min.css
--rw-r--r--   0        0        0    23879 2022-10-17 16:38:19.577121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.min.css.map
--rw-r--r--   0        0        0     8028 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.css
--rw-r--r--   0        0        0    52205 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.css.map
--rw-r--r--   0        0        0     6353 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.min.css
--rw-r--r--   0        0        0    51225 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.min.css.map
--rw-r--r--   0        0        0     8792 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.min.css
--rw-r--r--   0        0        0    60075 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.min.css.map
--rw-r--r--   0        0        0     1152 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/README.md
--rw-r--r--   0        0        0    10416 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css
--rw-r--r--   0        0        0    60219 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css.map
--rw-r--r--   0        0        0     2347 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css
--rw-r--r--   0        0        0    29464 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css.map
--rw-r--r--   0        0        0     1677 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css
--rw-r--r--   0        0        0    29290 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css.map
--rw-r--r--   0        0        0     8346 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css
--rw-r--r--   0        0        0    53409 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css.map
--rw-r--r--   0        0        0     5801 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css
--rw-r--r--   0        0        0    52533 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css.map
--rw-r--r--   0        0        0     7250 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css
--rw-r--r--   0        0        0    59189 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css.map
--rw-r--r--   0        0        0      890 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js
--rw-r--r--   0        0        0     2547 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js.map
--rw-r--r--   0        0        0      605 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js
--rw-r--r--   0        0        0     2200 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js.map
--rw-r--r--   0        0        0     1514 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js
--rw-r--r--   0        0        0     2503 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js.map
--rw-r--r--   0        0        0      861 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js
--rw-r--r--   0        0        0     2231 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js.map
--rw-r--r--   0        0        0      846 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/README.md
--rw-r--r--   0        0        0     1857 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.css
--rw-r--r--   0        0        0    29655 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.css.map
--rw-r--r--   0        0        0      556 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css
--rw-r--r--   0        0        0    12744 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css.map
--rw-r--r--   0        0        0      465 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css
--rw-r--r--   0        0        0    12728 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css.map
--rw-r--r--   0        0        0     1541 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css
--rw-r--r--   0        0        0    27524 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css.map
--rw-r--r--   0        0        0     1229 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css
--rw-r--r--   0        0        0    27007 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css.map
--rw-r--r--   0        0        0     1466 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css
--rw-r--r--   0        0        0    29111 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css.map
--rw-r--r--   0        0        0      694 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/README.md
--rw-r--r--   0        0        0     4657 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.css
--rw-r--r--   0        0        0    33046 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.css.map
--rw-r--r--   0        0        0      910 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css
--rw-r--r--   0        0        0    17346 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css.map
--rw-r--r--   0        0        0      787 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css
--rw-r--r--   0        0        0    17313 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css.map
--rw-r--r--   0        0        0     3988 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.css
--rw-r--r--   0        0        0    29547 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.css.map
--rw-r--r--   0        0        0     3428 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css
--rw-r--r--   0        0        0    28969 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css.map
--rw-r--r--   0        0        0     3987 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.min.css
--rw-r--r--   0        0        0    32425 2022-10-17 16:38:19.581121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.min.css.map
--rw-r--r--   0        0        0      707 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/README.md
--rw-r--r--   0        0        0     1735 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.css
--rw-r--r--   0        0        0    27099 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.css.map
--rw-r--r--   0        0        0      535 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.css
--rw-r--r--   0        0        0    13066 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.css.map
--rw-r--r--   0        0        0      444 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css
--rw-r--r--   0        0        0    12642 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css.map
--rw-r--r--   0        0        0     1441 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.css
--rw-r--r--   0        0        0    25608 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.css.map
--rw-r--r--   0        0        0     1166 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.min.css
--rw-r--r--   0        0        0    25100 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.min.css.map
--rw-r--r--   0        0        0     1382 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.min.css
--rw-r--r--   0        0        0    26554 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.min.css.map
--rw-r--r--   0        0        0     1090 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/README.md
--rw-r--r--   0        0        0     9125 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.css
--rw-r--r--   0        0        0    60013 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.css.map
--rw-r--r--   0        0        0     1578 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.css
--rw-r--r--   0        0        0    24683 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.css.map
--rw-r--r--   0        0        0     1169 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css
--rw-r--r--   0        0        0    24150 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css.map
--rw-r--r--   0        0        0     7820 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.css
--rw-r--r--   0        0        0    55906 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.css.map
--rw-r--r--   0        0        0     5810 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.min.css
--rw-r--r--   0        0        0    55193 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.min.css.map
--rw-r--r--   0        0        0     6751 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.min.css
--rw-r--r--   0        0        0    58782 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.min.css.map
--rw-r--r--   0        0        0     9505 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.js
--rw-r--r--   0        0        0    22379 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.js.map
--rw-r--r--   0        0        0     5322 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.min.js
--rw-r--r--   0        0        0    17344 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.min.js.map
--rw-r--r--   0        0        0    13744 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js
--rw-r--r--   0        0        0    22056 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js.map
--rw-r--r--   0        0        0     7067 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js
--rw-r--r--   0        0        0    17502 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js.map
--rw-r--r--   0        0        0     1082 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/README.md
--rw-r--r--   0        0        0    34105 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.css
--rw-r--r--   0        0        0    84775 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.css.map
--rw-r--r--   0        0        0    10190 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.css
--rw-r--r--   0        0        0    36407 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.css.map
--rw-r--r--   0        0        0     6960 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.min.css
--rw-r--r--   0        0        0    35107 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.min.css.map
--rw-r--r--   0        0        0    24733 2022-10-17 16:38:19.585121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.css
--rw-r--r--   0        0        0    62959 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.css.map
--rw-r--r--   0        0        0    20075 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.min.css
--rw-r--r--   0        0        0    60880 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.min.css.map
--rw-r--r--   0        0        0    26807 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.min.css
--rw-r--r--   0        0        0    82085 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.min.css.map
--rw-r--r--   0        0        0     3810 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.js
--rw-r--r--   0        0        0     9653 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.js.map
--rw-r--r--   0        0        0     2347 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.min.js
--rw-r--r--   0        0        0     7759 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.min.js.map
--rw-r--r--   0        0        0     6032 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.js
--rw-r--r--   0        0        0     9449 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.js.map
--rw-r--r--   0        0        0     3266 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js
--rw-r--r--   0        0        0     7834 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js.map
--rw-r--r--   0        0        0     1112 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/README.md
--rw-r--r--   0        0        0    49631 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.css
--rw-r--r--   0        0        0   128464 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.css.map
--rw-r--r--   0        0        0    26914 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.css
--rw-r--r--   0        0        0    70083 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.css.map
--rw-r--r--   0        0        0    23963 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css
--rw-r--r--   0        0        0    69281 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css.map
--rw-r--r--   0        0        0    23286 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.css
--rw-r--r--   0        0        0    81303 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.css.map
--rw-r--r--   0        0        0    21415 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.min.css
--rw-r--r--   0        0        0    80360 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.min.css.map
--rw-r--r--   0        0        0    44835 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.min.css
--rw-r--r--   0        0        0   126711 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.min.css.map
--rw-r--r--   0        0        0      527 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.js
--rw-r--r--   0        0        0     1451 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.js.map
--rw-r--r--   0        0        0      347 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.min.js
--rw-r--r--   0        0        0     1245 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.min.js.map
--rw-r--r--   0        0        0      594 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js
--rw-r--r--   0        0        0     1445 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js.map
--rw-r--r--   0        0        0      373 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js
--rw-r--r--   0        0        0     1253 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js.map
--rw-r--r--   0        0        0      795 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/README.md
--rw-r--r--   0        0        0     5405 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.css
--rw-r--r--   0        0        0    40961 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.css.map
--rw-r--r--   0        0        0      773 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.css
--rw-r--r--   0        0        0    16327 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.css.map
--rw-r--r--   0        0        0      592 2022-10-17 16:38:19.589121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css
--rw-r--r--   0        0        0    16293 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css.map
--rw-r--r--   0        0        0     4873 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.css
--rw-r--r--   0        0        0    38586 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.css.map
--rw-r--r--   0        0        0     3121 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.min.css
--rw-r--r--   0        0        0    37848 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.min.css.map
--rw-r--r--   0        0        0     3485 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.min.css
--rw-r--r--   0        0        0    40175 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.min.css.map
--rw-r--r--   0        0        0     1211 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/README.md
--rw-r--r--   0        0        0     8764 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.css
--rw-r--r--   0        0        0    49136 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.css.map
--rw-r--r--   0        0        0     2374 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css
--rw-r--r--   0        0        0    25598 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css.map
--rw-r--r--   0        0        0     1967 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css
--rw-r--r--   0        0        0    25484 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css.map
--rw-r--r--   0        0        0     6665 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.css
--rw-r--r--   0        0        0    42288 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.css.map
--rw-r--r--   0        0        0     4992 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css
--rw-r--r--   0        0        0    41598 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css.map
--rw-r--r--   0        0        0     6731 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.min.css
--rw-r--r--   0        0        0    48345 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.min.css.map
--rw-r--r--   0        0        0     2013 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.js
--rw-r--r--   0        0        0     5322 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.js.map
--rw-r--r--   0        0        0     1347 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js
--rw-r--r--   0        0        0     4353 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js.map
--rw-r--r--   0        0        0     3763 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js
--rw-r--r--   0        0        0     5211 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js.map
--rw-r--r--   0        0        0     2056 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js
--rw-r--r--   0        0        0     4432 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js.map
--rw-r--r--   0        0        0     1412 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/README.md
--rw-r--r--   0        0        0     4336 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.css
--rw-r--r--   0        0        0    43755 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.css.map
--rw-r--r--   0        0        0     1403 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.css
--rw-r--r--   0        0        0    20488 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.css.map
--rw-r--r--   0        0        0     1183 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css
--rw-r--r--   0        0        0    20417 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css.map
--rw-r--r--   0        0        0     3393 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.css
--rw-r--r--   0        0        0    39559 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.css.map
--rw-r--r--   0        0        0     2630 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.min.css
--rw-r--r--   0        0        0    38882 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.min.css.map
--rw-r--r--   0        0        0     3395 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.min.css
--rw-r--r--   0        0        0    43023 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.min.css.map
--rw-r--r--   0        0        0      548 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/README.md
--rw-r--r--   0        0        0      875 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.css
--rw-r--r--   0        0        0    11173 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.css.map
--rw-r--r--   0        0        0      699 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.min.css
--rw-r--r--   0        0        0    10753 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.min.css.map
--rw-r--r--   0        0        0     2470 2022-10-17 16:38:19.593121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/README.md
--rw-r--r--   0        0        0   195690 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.css
--rw-r--r--   0        0        0   349835 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.css.map
--rw-r--r--   0        0        0     4342 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.css
--rw-r--r--   0        0        0    38238 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.css.map
--rw-r--r--   0        0        0     3325 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.min.css
--rw-r--r--   0        0        0    35852 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.min.css.map
--rw-r--r--   0        0        0   191587 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.css
--rw-r--r--   0        0        0   337455 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.css.map
--rw-r--r--   0        0        0   158070 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.min.css
--rw-r--r--   0        0        0   324803 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.min.css.map
--rw-r--r--   0        0        0   161167 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.min.css
--rw-r--r--   0        0        0   336524 2022-10-17 16:38:19.597121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.min.css.map
--rw-r--r--   0        0        0    58163 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.js
--rw-r--r--   0        0        0   152953 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.js.map
--rw-r--r--   0        0        0    33997 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.min.js
--rw-r--r--   0        0        0   114120 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.min.js.map
--rw-r--r--   0        0        0    85987 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.js
--rw-r--r--   0        0        0   149067 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.js.map
--rw-r--r--   0        0        0    46071 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.min.js
--rw-r--r--   0        0        0   114880 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.min.js.map
--rw-r--r--   0        0        0      557 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/README.md
--rw-r--r--   0        0        0   618733 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.css
--rw-r--r--   0        0        0  1255933 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.css.map
--rw-r--r--   0        0        0   112590 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css
--rw-r--r--   0        0        0   334683 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css.map
--rw-r--r--   0        0        0    88746 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css
--rw-r--r--   0        0        0   320323 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css.map
--rw-r--r--   0        0        0   508107 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.css
--rw-r--r--   0        0        0   997920 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.css.map
--rw-r--r--   0        0        0   418116 2022-10-17 16:38:19.617120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css
--rw-r--r--   0        0        0   950122 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css.map
--rw-r--r--   0        0        0   505976 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.min.css
--rw-r--r--   0        0        0  1199654 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.min.css.map
--rw-r--r--   0        0        0   102336 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.js
--rw-r--r--   0        0        0   267371 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.js.map
--rw-r--r--   0        0        0    62300 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js
--rw-r--r--   0        0        0   201867 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js.map
--rw-r--r--   0        0        0   165837 2022-10-17 16:38:19.621121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js
--rw-r--r--   0        0        0   299474 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js.map
--rw-r--r--   0        0        0    95534 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js
--rw-r--r--   0        0        0   233645 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js.map
--rw-r--r--   0        0        0   617855 2022-10-17 16:38:19.601121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.css
--rw-r--r--   0        0        0  1254712 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.css.map
--rw-r--r--   0        0        0   112328 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.css
--rw-r--r--   0        0        0   334251 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.css.map
--rw-r--r--   0        0        0    88491 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.min.css
--rw-r--r--   0        0        0   319895 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.min.css.map
--rw-r--r--   0        0        0   507491 2022-10-17 16:38:19.605121 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.css
--rw-r--r--   0        0        0   997129 2022-10-17 16:38:19.609120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.css.map
--rw-r--r--   0        0        0   417510 2022-10-17 16:38:19.609120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.min.css
--rw-r--r--   0        0        0   949337 2022-10-17 16:38:19.609120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.min.css.map
--rw-r--r--   0        0        0   505115 2022-10-17 16:38:19.609120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.min.css
--rw-r--r--   0        0        0  1198443 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.min.css.map
--rw-r--r--   0        0        0   102336 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.js
--rw-r--r--   0        0        0   266969 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.js.map
--rw-r--r--   0        0        0    62300 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.min.js
--rw-r--r--   0        0        0   201465 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.min.js.map
--rw-r--r--   0        0        0   165837 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.js
--rw-r--r--   0        0        0   299054 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.js.map
--rw-r--r--   0        0        0    95534 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.min.js
--rw-r--r--   0        0        0   233225 2022-10-17 16:38:19.613120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.min.js.map
--rw-r--r--   0        0        0     3631 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0     9190 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     3448 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0     7406 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/favicon.ico
--rw-r--r--   0        0        0     6360 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/favicon.svg
--rw-r--r--   0        0        0      292 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/manifest.webmanifest
--rwxr-xr-x   0        0        0    52216 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff
--rwxr-xr-x   0        0        0    42092 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2
--rwxr-xr-x   0        0        0    56436 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff
--rwxr-xr-x   0        0        0    45300 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2
--rwxr-xr-x   0        0        0    50440 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff
--rwxr-xr-x   0        0        0    41368 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2
--rwxr-xr-x   0        0        0    54492 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff
--rwxr-xr-x   0        0        0    43916 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2
--rwxr-xr-x   0        0        0    51292 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff
--rwxr-xr-x   0        0        0    41940 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2
--rwxr-xr-x   0        0        0    54680 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff
--rwxr-xr-x   0        0        0    44572 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2
--rwxr-xr-x   0        0        0    51140 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff
--rwxr-xr-x   0        0        0    41328 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2
--rwxr-xr-x   0        0        0    54328 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff
--rwxr-xr-x   0        0        0    44284 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2
--rw-r--r--   0        0        0   114508 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff
--rw-r--r--   0        0        0    80368 2022-10-17 16:38:19.625120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2
--rw-r--r--   0        0        0   114016 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff
--rw-r--r--   0        0        0    79472 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2
--rw-r--r--   0        0        0      397 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-fill.svg
--rw-r--r--   0        0        0      789 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg
--rw-r--r--   0        0        0      280 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-fill.svg
--rw-r--r--   0        0        0      416 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-line.svg
--rw-r--r--   0        0        0      232 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/bank-fill.svg
--rw-r--r--   0        0        0      262 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/bank-line.svg
--rw-r--r--   0        0        0      204 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/building-fill.svg
--rw-r--r--   0        0        0      225 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/building-line.svg
--rw-r--r--   0        0        0      316 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/community-fill.svg
--rw-r--r--   0        0        0      388 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/community-line.svg
--rw-r--r--   0        0        0      232 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/government-fill.svg
--rw-r--r--   0        0        0      227 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/government-line.svg
--rw-r--r--   0        0        0      209 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/home-4-fill.svg
--rw-r--r--   0        0        0      239 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/home-4-line.svg
--rw-r--r--   0        0        0      212 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/hospital-fill.svg
--rw-r--r--   0        0        0      228 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/hospital-line.svg
--rw-r--r--   0        0        0      224 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/hotel-fill.svg
--rw-r--r--   0        0        0      243 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/hotel-line.svg
--rw-r--r--   0        0        0      437 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/store-fill.svg
--rw-r--r--   0        0        0      546 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/store-line.svg
--rw-r--r--   0        0        0      254 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/archive-fill.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/archive-line.svg
--rw-r--r--   0        0        0      330 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/attachment-fill.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/attachment-line.svg
--rw-r--r--   0        0        0      289 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/award-fill.svg
--rw-r--r--   0        0        0      338 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/award-line.svg
--rw-r--r--   0        0        0      218 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/bar-chart-box-fill.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/bar-chart-box-line.svg
--rw-r--r--   0        0        0      208 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/bookmark-fill.svg
--rw-r--r--   0        0        0      242 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/bookmark-line.svg
--rw-r--r--   0        0        0      253 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/briefcase-fill.svg
--rw-r--r--   0        0        0      267 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/briefcase-line.svg
--rw-r--r--   0        0        0      248 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-2-fill.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-2-line.svg
--rw-r--r--   0        0        0      218 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-event-fill.svg
--rw-r--r--   0        0        0      251 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-event-line.svg
--rw-r--r--   0        0        0      203 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-fill.svg
--rw-r--r--   0        0        0      244 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/calendar-line.svg
--rw-r--r--   0        0        0      254 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/cloud-fill.svg
--rw-r--r--   0        0        0      356 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/cloud-line.svg
--rw-r--r--   0        0        0      290 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/copyright-fill.svg
--rw-r--r--   0        0        0      346 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/copyright-line.svg
--rw-r--r--   0        0        0      341 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/customer-service-fill.svg
--rw-r--r--   0        0        0      375 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/customer-service-line.svg
--rw-r--r--   0        0        0      210 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/flag-fill.svg
--rw-r--r--   0        0        0      255 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/flag-line.svg
--rw-r--r--   0        0        0      540 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/global-fill.svg
--rw-r--r--   0        0        0      607 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/global-line.svg
--rw-r--r--   0        0        0      200 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/line-chart-fill.svg
--rw-r--r--   0        0        0      218 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/line-chart-line.svg
--rw-r--r--   0        0        0      409 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/links-fill.svg
--rw-r--r--   0        0        0      418 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/links-line.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/mail-fill.svg
--rw-r--r--   0        0        0      247 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/mail-line.svg
--rw-r--r--   0        0        0      318 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/mail-open-fill.svg
--rw-r--r--   0        0        0      359 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/mail-open-line.svg
--rw-r--r--   0        0        0      355 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/medal-fill.svg
--rw-r--r--   0        0        0      389 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/medal-line.svg
--rw-r--r--   0        0        0      248 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/pie-chart-2-fill.svg
--rw-r--r--   0        0        0      378 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/pie-chart-2-line.svg
--rw-r--r--   0        0        0      273 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/pie-chart-box-fill.svg
--rw-r--r--   0        0        0      289 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/pie-chart-box-line.svg
--rw-r--r--   0        0        0      256 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/printer-fill.svg
--rw-r--r--   0        0        0      341 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/printer-line.svg
--rw-r--r--   0        0        0      296 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/profil-fill.svg
--rw-r--r--   0        0        0      312 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/profil-line.svg
--rw-r--r--   0        0        0      356 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/projector-2-fill.svg
--rw-r--r--   0        0        0      350 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/projector-2-line.svg
--rw-r--r--   0        0        0      248 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/send-plane-fill.svg
--rw-r--r--   0        0        0      301 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/send-plane-line.svg
--rw-r--r--   0        0        0      226 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/slideshow-fill.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/slideshow-line.svg
--rw-r--r--   0        0        0      215 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/window-fill.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/window-line.svg
--rw-r--r--   0        0        0      199 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-2-fill.svg
--rw-r--r--   0        0        0      237 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-2-line.svg
--rw-r--r--   0        0        0      236 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-3-fill.svg
--rw-r--r--   0        0        0      360 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-3-line.svg
--rw-r--r--   0        0        0      256 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-check-fill.svg
--rw-r--r--   0        0        0      283 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-check-line.svg
--rw-r--r--   0        0        0      321 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-delete-fill.svg
--rw-r--r--   0        0        0      348 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-delete-line.svg
--rw-r--r--   0        0        0      243 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-poll-fill.svg
--rw-r--r--   0        0        0      214 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/chat-poll-line.svg
--rw-r--r--   0        0        0      236 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/discuss-fill.svg
--rw-r--r--   0        0        0      282 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/discuss-line.svg
--rw-r--r--   0        0        0      201 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/feedback-fill.svg
--rw-r--r--   0        0        0      229 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/feedback-line.svg
--rw-r--r--   0        0        0      215 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/message-2-fill.svg
--rw-r--r--   0        0        0      245 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/message-2-line.svg
--rw-r--r--   0        0        0      231 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/question-answer-fill.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/question-answer-line.svg
--rw-r--r--   0        0        0      263 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/questionnaire-fill.svg
--rw-r--r--   0        0        0      327 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/questionnaire-line.svg
--rw-r--r--   0        0        0      206 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/video-chat-fill.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/communication/video-chat-line.svg
--rw-r--r--   0        0        0      318 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/ball-pen-fill.svg
--rw-r--r--   0        0        0      372 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/ball-pen-line.svg
--rw-r--r--   0        0        0      252 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/brush-3-fill.svg
--rw-r--r--   0        0        0      266 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/brush-3-line.svg
--rw-r--r--   0        0        0      449 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/brush-fill.svg
--rw-r--r--   0        0        0      689 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/brush-line.svg
--rw-r--r--   0        0        0      195 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/contrast-fill.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/contrast-line.svg
--rw-r--r--   0        0        0      173 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/crop-fill.svg
--rw-r--r--   0        0        0      184 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/crop-line.svg
--rw-r--r--   0        0        0      399 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/drag-move-2-fill.svg
--rw-r--r--   0        0        0      178 2022-10-17 16:38:19.629120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/drag-move-2-line.svg
--rw-r--r--   0        0        0      153 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/drop-fill.svg
--rw-r--r--   0        0        0      190 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/drop-line.svg
--rw-r--r--   0        0        0      275 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/edit-box-fill.svg
--rw-r--r--   0        0        0      255 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/edit-box-line.svg
--rw-r--r--   0        0        0      206 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/edit-fill.svg
--rw-r--r--   0        0        0      258 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/edit-line.svg
--rw-r--r--   0        0        0      266 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/ink-bottle-fill.svg
--rw-r--r--   0        0        0      323 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/ink-bottle-line.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/layout-grid-fill.svg
--rw-r--r--   0        0        0      232 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/layout-grid-line.svg
--rw-r--r--   0        0        0      401 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/mark-pen-fill.svg
--rw-r--r--   0        0        0      503 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/mark-pen-line.svg
--rw-r--r--   0        0        0      292 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/paint-brush-fill.svg
--rw-r--r--   0        0        0      305 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/paint-brush-line.svg
--rw-r--r--   0        0        0      339 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/paint-fill.svg
--rw-r--r--   0        0        0      362 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/paint-line.svg
--rw-r--r--   0        0        0      437 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/palette-fill.svg
--rw-r--r--   0        0        0      584 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/palette-line.svg
--rw-r--r--   0        0        0      386 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pantone-fill.svg
--rw-r--r--   0        0        0      505 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pantone-line.svg
--rw-r--r--   0        0        0      389 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pen-nib-fill.svg
--rw-r--r--   0        0        0      510 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pen-nib-line.svg
--rw-r--r--   0        0        0      254 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pencil-fill.svg
--rw-r--r--   0        0        0      310 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pencil-line.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pencil-ruler-fill.svg
--rw-r--r--   0        0        0      255 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/pencil-ruler-line.svg
--rw-r--r--   0        0        0      302 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/sip-fill.svg
--rw-r--r--   0        0        0      352 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/sip-line.svg
--rw-r--r--   0        0        0      221 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/table-fill.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/table-line.svg
--rw-r--r--   0        0        0      500 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/bug-fill.svg
--rw-r--r--   0        0        0      632 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/bug-line.svg
--rw-r--r--   0        0        0      360 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/code-box-fill.svg
--rw-r--r--   0        0        0      374 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/code-box-line.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/code-s-slash-line.svg
--rw-r--r--   0        0        0      197 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/cursor-fill.svg
--rw-r--r--   0        0        0      283 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/cursor-line.svg
--rw-r--r--   0        0        0      307 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-branch-fill.svg
--rw-r--r--   0        0        0      425 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-branch-line.svg
--rw-r--r--   0        0        0      187 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-commit-fill.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-commit-line.svg
--rw-r--r--   0        0        0      330 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-merge-fill.svg
--rw-r--r--   0        0        0      455 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-merge-line.svg
--rw-r--r--   0        0        0      233 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-pull-request-fill.svg
--rw-r--r--   0        0        0      356 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-pull-request-line.svg
--rw-r--r--   0        0        0      294 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-commits-fill.svg
--rw-r--r--   0        0        0      320 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-commits-line.svg
--rw-r--r--   0        0        0      285 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-fill.svg
--rw-r--r--   0        0        0      328 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-line.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-private-fill.svg
--rw-r--r--   0        0        0      304 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/git-repository-private-line.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/terminal-box-fill.svg
--rw-r--r--   0        0        0      287 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/terminal-box-line.svg
--rw-r--r--   0        0        0      186 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/terminal-line.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/terminal-window-fill.svg
--rw-r--r--   0        0        0      245 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/terminal-window-line.svg
--rw-r--r--   0        0        0      343 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/bluetooth-fill.svg
--rw-r--r--   0        0        0      343 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/bluetooth-line.svg
--rw-r--r--   0        0        0      256 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/computer-fill.svg
--rw-r--r--   0        0        0      275 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/computer-line.svg
--rw-r--r--   0        0        0      514 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg
--rw-r--r--   0        0        0      552 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg
--rw-r--r--   0        0        0      266 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/database-fill.svg
--rw-r--r--   0        0        0      296 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/database-line.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/device-fill.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/device-line.svg
--rw-r--r--   0        0        0      206 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/hard-drive-2-fill.svg
--rw-r--r--   0        0        0      222 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/hard-drive-2-line.svg
--rw-r--r--   0        0        0      290 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/mac-fill.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/mac-line.svg
--rw-r--r--   0        0        0      485 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/phone-fill.svg
--rw-r--r--   0        0        0      719 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/phone-line.svg
--rw-r--r--   0        0        0      272 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/qr-code-fill.svg
--rw-r--r--   0        0        0      315 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/qr-code-line.svg
--rw-r--r--   0        0        0      229 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/rss-fill.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/rss-line.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/save-3-fill.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/save-3-line.svg
--rw-r--r--   0        0        0      195 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/save-fill.svg
--rw-r--r--   0        0        0      219 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/save-line.svg
--rw-r--r--   0        0        0      219 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/server-fill.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/server-line.svg
--rw-r--r--   0        0        0      208 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/smartphone-fill.svg
--rw-r--r--   0        0        0      224 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/smartphone-line.svg
--rw-r--r--   0        0        0      208 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/tablet-fill.svg
--rw-r--r--   0        0        0      224 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/tablet-line.svg
--rw-r--r--   0        0        0      285 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/tv-fill.svg
--rw-r--r--   0        0        0      304 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/tv-line.svg
--rw-r--r--   0        0        0      618 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg
--rw-r--r--   0        0        0      630 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/wifi-line.svg
--rw-r--r--   0        0        0      233 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/article-fill.svg
--rw-r--r--   0        0        0      249 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/article-line.svg
--rw-r--r--   0        0        0      181 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/book-2-fill.svg
--rw-r--r--   0        0        0      227 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/book-2-line.svg
--rw-r--r--   0        0        0      226 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/booklet-fill.svg
--rw-r--r--   0        0        0      242 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/booklet-line.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/clipboard-fill.svg
--rw-r--r--   0        0        0      274 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/clipboard-line.svg
--rw-r--r--   0        0        0      317 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/draft-fill.svg
--rw-r--r--   0        0        0      303 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/draft-line.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-add-fill.svg
--rw-r--r--   0        0        0      251 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-add-line.svg
--rw-r--r--   0        0        0      227 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-download-fill.svg
--rw-r--r--   0        0        0      245 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-download-line.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-fill.svg
--rw-r--r--   0        0        0      225 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-line.svg
--rw-r--r--   0        0        0      255 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-pdf-fill.svg
--rw-r--r--   0        0        0      273 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-pdf-line.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-text-fill.svg
--rw-r--r--   0        0        0      272 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/file-text-line.svg
--rw-r--r--   0        0        0      198 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/folder-2-fill.svg
--rw-r--r--   0        0        0      234 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/folder-2-line.svg
--rw-r--r--   0        0        0      262 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/newspaper-fill.svg
--rw-r--r--   0        0        0      290 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/newspaper-line.svg
--rw-r--r--   0        0        0      292 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/survey-fill.svg
--rw-r--r--   0        0        0      317 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/survey-line.svg
--rw-r--r--   0        0        0      217 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/todo-fill.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/document/todo-line.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/code-view.svg
--rw-r--r--   0        0        0      250 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/font-size.svg
--rw-r--r--   0        0        0      314 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/fr--bold.svg
--rw-r--r--   0        0        0      160 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/fr--highlight.svg
--rw-r--r--   0        0        0      278 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/fr--quote-fill.svg
--rw-r--r--   0        0        0      344 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/fr--quote-line.svg
--rw-r--r--   0        0        0      223 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-1.svg
--rw-r--r--   0        0        0      387 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-2.svg
--rw-r--r--   0        0        0      542 2022-10-17 16:38:19.633120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-3.svg
--rw-r--r--   0        0        0      268 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-4.svg
--rw-r--r--   0        0        0      393 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-5.svg
--rw-r--r--   0        0        0      538 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-6.svg
--rw-r--r--   0        0        0      298 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/hashtag.svg
--rw-r--r--   0        0        0      158 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/italic.svg
--rw-r--r--   0        0        0      468 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/link-unlink.svg
--rw-r--r--   0        0        0      408 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/link.svg
--rw-r--r--   0        0        0      246 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/list-ordered.svg
--rw-r--r--   0        0        0      275 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/list-unordered.svg
--rw-r--r--   0        0        0      341 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/question-mark.svg
--rw-r--r--   0        0        0      147 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/separator.svg
--rw-r--r--   0        0        0      151 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/space.svg
--rw-r--r--   0        0        0      317 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/subscript.svg
--rw-r--r--   0        0        0      315 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/superscript.svg
--rw-r--r--   0        0        0      263 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/table-2.svg
--rw-r--r--   0        0        0      505 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/translate-2.svg
--rw-r--r--   0        0        0      206 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/bank-card-fill.svg
--rw-r--r--   0        0        0      220 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/bank-card-line.svg
--rw-r--r--   0        0        0      277 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/coin-fill.svg
--rw-r--r--   0        0        0      393 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/gift-fill.svg
--rw-r--r--   0        0        0      406 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/gift-line.svg
--rw-r--r--   0        0        0      366 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/money-euro-box-fill.svg
--rw-r--r--   0        0        0      344 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/money-euro-box-line.svg
--rw-r--r--   0        0        0      365 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-fill.svg
--rw-r--r--   0        0        0      362 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-line.svg
--rw-r--r--   0        0        0      397 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/secure-payment-fill.svg
--rw-r--r--   0        0        0      427 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/secure-payment-line.svg
--rw-r--r--   0        0        0      348 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/shopping-bag-fill.svg
--rw-r--r--   0        0        0      282 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/shopping-bag-line.svg
--rw-r--r--   0        0        0      311 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-fill.svg
--rw-r--r--   0        0        0      343 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-line.svg
--rw-r--r--   0        0        0      200 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/trophy-fill.svg
--rw-r--r--   0        0        0      222 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/finance/trophy-line.svg
--rw-r--r--   0        0        0      289 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/capsule-fill.svg
--rw-r--r--   0        0        0      379 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/capsule-line.svg
--rw-r--r--   0        0        0      336 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/dislike-fill.svg
--rw-r--r--   0        0        0      543 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/dislike-line.svg
--rw-r--r--   0        0        0      243 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/dossier-fill.svg
--rw-r--r--   0        0        0      265 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/dossier-line.svg
--rw-r--r--   0        0        0      269 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/first-aid-kit-fill.svg
--rw-r--r--   0        0        0      283 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/first-aid-kit-line.svg
--rw-r--r--   0        0        0      317 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-fill.svg
--rw-r--r--   0        0        0      359 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-line.svg
--rw-r--r--   0        0        0      258 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/health-book-fill.svg
--rw-r--r--   0        0        0      273 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/health-book-line.svg
--rw-r--r--   0        0        0      209 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/heart-fill.svg
--rw-r--r--   0        0        0      365 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/heart-line.svg
--rw-r--r--   0        0        0      331 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/heart-pulse-fill.svg
--rw-r--r--   0        0        0      661 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg
--rw-r--r--   0        0        0      476 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/lungs-fill.svg
--rw-r--r--   0        0        0      909 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/lungs-line.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/medicine-bottle-fill.svg
--rw-r--r--   0        0        0      293 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/medicine-bottle-line.svg
--rw-r--r--   0        0        0      395 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/mental-health-fill.svg
--rw-r--r--   0        0        0      503 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/mental-health-line.svg
--rw-r--r--   0        0        0      519 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg
--rw-r--r--   0        0        0      618 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/microscope-line.svg
--rw-r--r--   0        0        0      370 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/psychotherapy-fill.svg
--rw-r--r--   0        0        0      504 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/psychotherapy-line.svg
--rw-r--r--   0        0        0      181 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/pulse-line.svg
--rw-r--r--   0        0        0      311 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/stethoscope-fill.svg
--rw-r--r--   0        0        0      346 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/stethoscope-line.svg
--rw-r--r--   0        0        0      446 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/surgical-mask-fill.svg
--rw-r--r--   0        0        0      567 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg
--rw-r--r--   0        0        0      466 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/syringe-fill.svg
--rw-r--r--   0        0        0      486 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/syringe-line.svg
--rw-r--r--   0        0        0      237 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/test-tube-fill.svg
--rw-r--r--   0        0        0      264 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/test-tube-line.svg
--rw-r--r--   0        0        0      484 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/thermometer-fill.svg
--rw-r--r--   0        0        0      576 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg
--rw-r--r--   0        0        0     1055 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/virus-fill.svg
--rw-r--r--   0        0        0     1112 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/virus-line.svg
--rw-r--r--   0        0        0      552 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg
--rw-r--r--   0        0        0      594 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg
--rw-r--r--   0        0        0      591 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg
--rw-r--r--   0        0        0      411 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/edge-line.svg
--rw-r--r--   0        0        0      368 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/facebook-circle-fill.svg
--rw-r--r--   0        0        0      458 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/facebook-circle-line.svg
--rw-r--r--   0        0        0      708 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg
--rw-r--r--   0        0        0     1003 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg
--rw-r--r--   0        0        0      685 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg
--rw-r--r--   0        0        0      806 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg
--rw-r--r--   0        0        0      561 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg
--rw-r--r--   0        0        0      428 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-line.svg
--rw-r--r--   0        0        0      790 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/github-fill.svg
--rw-r--r--   0        0        0     1485 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/github-line.svg
--rw-r--r--   0        0        0      530 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/google-fill.svg
--rw-r--r--   0        0        0      371 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/google-line.svg
--rw-r--r--   0        0        0      965 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg
--rw-r--r--   0        0        0      796 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/ie-line.svg
--rw-r--r--   0        0        0      917 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg
--rw-r--r--   0        0        0     2014 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg
--rw-r--r--   0        0        0      552 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg
--rw-r--r--   0        0        0      366 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/linkedin-box-line.svg
--rw-r--r--   0        0        0      948 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg
--rw-r--r--   0        0        0     1259 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg
--rw-r--r--   0        0        0      202 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/npmjs-fill.svg
--rw-r--r--   0        0        0      220 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/npmjs-line.svg
--rw-r--r--   0        0        0      331 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/remixicon-fill.svg
--rw-r--r--   0        0        0      391 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/remixicon-line.svg
--rw-r--r--   0        0        0      972 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg
--rw-r--r--   0        0        0      574 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/safari-line.svg
--rw-r--r--   0        0        0     1133 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg
--rw-r--r--   0        0        0      514 2022-10-17 16:38:19.637120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/slack-line.svg
--rw-r--r--   0        0        0     1494 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg
--rw-r--r--   0        0        0     1848 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg
--rw-r--r--   0        0        0      398 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/telegram-fill.svg
--rw-r--r--   0        0        0      440 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/telegram-line.svg
--rw-r--r--   0        0        0      332 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitch-fill.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitch-line.svg
--rw-r--r--   0        0        0      586 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg
--rw-r--r--   0        0        0      690 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg
--rw-r--r--   0        0        0      726 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg
--rw-r--r--   0        0        0     1001 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg
--rw-r--r--   0        0        0      178 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vuejs-fill.svg
--rw-r--r--   0        0        0      198 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vuejs-line.svg
--rw-r--r--   0        0        0      418 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/youtube-fill.svg
--rw-r--r--   0        0        0      899 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg
--rw-r--r--   0        0        0      385 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/anchor-fill.svg
--rw-r--r--   0        0        0      350 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/anchor-line.svg
--rw-r--r--   0        0        0      359 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/bike-fill.svg
--rw-r--r--   0        0        0      359 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/bike-line.svg
--rw-r--r--   0        0        0      284 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/bus-fill.svg
--rw-r--r--   0        0        0      299 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/bus-line.svg
--rw-r--r--   0        0        0      372 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/car-fill.svg
--rw-r--r--   0        0        0      387 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/car-line.svg
--rw-r--r--   0        0        0      317 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/caravan-fill.svg
--rw-r--r--   0        0        0      383 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/caravan-line.svg
--rw-r--r--   0        0        0      253 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/charging-pile-2-fill.svg
--rw-r--r--   0        0        0      265 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/charging-pile-2-line.svg
--rw-r--r--   0        0        0      246 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/compass-3-fill.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/compass-3-line.svg
--rw-r--r--   0        0        0      222 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/cup-fill.svg
--rw-r--r--   0        0        0      264 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/cup-line.svg
--rw-r--r--   0        0        0      945 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/earth-fill.svg
--rw-r--r--   0        0        0      905 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/earth-line.svg
--rw-r--r--   0        0        0     2305 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/france-fill.svg
--rw-r--r--   0        0        0     4459 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/france-line.svg
--rw-r--r--   0        0        0      303 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/gas-station-fill.svg
--rw-r--r--   0        0        0      318 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/gas-station-line.svg
--rw-r--r--   0        0        0      179 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/goblet-fill.svg
--rw-r--r--   0        0        0      208 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/goblet-line.svg
--rw-r--r--   0        0        0      214 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/map-pin-2-fill.svg
--rw-r--r--   0        0        0      280 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/map-pin-2-line.svg
--rw-r--r--   0        0        0      277 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/map-pin-user-fill.svg
--rw-r--r--   0        0        0      363 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/map-pin-user-line.svg
--rw-r--r--   0        0        0      378 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/motorbike-fill.svg
--rw-r--r--   0        0        0      447 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/motorbike-line.svg
--rw-r--r--   0        0        0      256 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/passport-fill.svg
--rw-r--r--   0        0        0      272 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/passport-line.svg
--rw-r--r--   0        0        0      221 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/restaurant-fill.svg
--rw-r--r--   0        0        0      257 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/restaurant-line.svg
--rw-r--r--   0        0        0      381 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/road-map-fill.svg
--rw-r--r--   0        0        0      405 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/road-map-line.svg
--rw-r--r--   0        0        0      278 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/sailboat-fill.svg
--rw-r--r--   0        0        0      333 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/sailboat-line.svg
--rw-r--r--   0        0        0      580 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg
--rw-r--r--   0        0        0      562 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg
--rw-r--r--   0        0        0      351 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/signal-tower-fill.svg
--rw-r--r--   0        0        0      348 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/signal-tower-line.svg
--rw-r--r--   0        0        0      271 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/suitcase-2-fill.svg
--rw-r--r--   0        0        0      286 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/suitcase-2-line.svg
--rw-r--r--   0        0        0      374 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/taxi-fill.svg
--rw-r--r--   0        0        0      386 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/taxi-line.svg
--rw-r--r--   0        0        0      251 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/train-fill.svg
--rw-r--r--   0        0        0      293 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/train-line.svg
--rw-r--r--   0        0        0      253 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/camera-fill.svg
--rw-r--r--   0        0        0      311 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/camera-line.svg
--rw-r--r--   0        0        0      294 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/clapperboard-fill.svg
--rw-r--r--   0        0        0      312 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/clapperboard-line.svg
--rw-r--r--   0        0        0      334 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/equalizer-fill.svg
--rw-r--r--   0        0        0      505 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/equalizer-line.svg
--rw-r--r--   0        0        0      340 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/film-fill.svg
--rw-r--r--   0        0        0      355 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/film-line.svg
--rw-r--r--   0        0        0      388 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/gallery-fill.svg
--rw-r--r--   0        0        0      466 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/gallery-line.svg
--rw-r--r--   0        0        0      261 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/headphone-fill.svg
--rw-r--r--   0        0        0      300 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/headphone-line.svg
--rw-r--r--   0        0        0      394 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-add-fill.svg
--rw-r--r--   0        0        0      316 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-add-line.svg
--rw-r--r--   0        0        0      398 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-edit-fill.svg
--rw-r--r--   0        0        0      415 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-edit-line.svg
--rw-r--r--   0        0        0      307 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-fill.svg
--rw-r--r--   0        0        0      334 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/image-line.svg
--rw-r--r--   0        0        0      394 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/live-fill.svg
--rw-r--r--   0        0        0      408 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/live-line.svg
--rw-r--r--   0        0        0      269 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/mic-fill.svg
--rw-r--r--   0        0        0      320 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/mic-line.svg
--rw-r--r--   0        0        0      158 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/music-2-fill.svg
--rw-r--r--   0        0        0      226 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/music-2-line.svg
--rw-r--r--   0        0        0      154 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/notification-3-fill.svg
--rw-r--r--   0        0        0      208 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/notification-3-line.svg
--rw-r--r--   0        0        0      201 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/pause-circle-fill.svg
--rw-r--r--   0        0        0      236 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/pause-circle-line.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/play-circle-fill.svg
--rw-r--r--   0        0        0      313 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/play-circle-line.svg
--rw-r--r--   0        0        0      186 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/stop-circle-fill.svg
--rw-r--r--   0        0        0      221 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/stop-circle-line.svg
--rw-r--r--   0        0        0      160 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/transcription.svg
--rw-r--r--   0        0        0      403 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-down-fill.svg
--rw-r--r--   0        0        0      489 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-down-line.svg
--rw-r--r--   0        0        0      407 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-mute-fill.svg
--rw-r--r--   0        0        0      490 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-mute-line.svg
--rw-r--r--   0        0        0      551 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg
--rw-r--r--   0        0        0      630 2022-10-17 16:38:19.641120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg
--rw-r--r--   0        0        0      334 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/leaf-fill.svg
--rw-r--r--   0        0        0      467 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/leaf-line.svg
--rw-r--r--   0        0        0      253 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/lightbulb-fill.svg
--rw-r--r--   0        0        0      406 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/lightbulb-line.svg
--rw-r--r--   0        0        0      277 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/plant-fill.svg
--rw-r--r--   0        0        0      362 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/plant-line.svg
--rw-r--r--   0        0        0      573 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg
--rw-r--r--   0        0        0      558 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/recycle-line.svg
--rw-r--r--   0        0        0      454 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/scales-3-fill.svg
--rw-r--r--   0        0        0      552 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg
--rw-r--r--   0        0        0      258 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/seedling-fill.svg
--rw-r--r--   0        0        0      326 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/seedling-line.svg
--rw-r--r--   0        0        0      232 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/umbrella-fill.svg
--rw-r--r--   0        0        0      315 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/umbrella-line.svg
--rw-r--r--   0        0        0      209 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/add-circle-fill.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/add-circle-line.svg
--rw-r--r--   0        0        0      136 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/add-line.svg
--rw-r--r--   0        0        0      319 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/alarm-warning-fill.svg
--rw-r--r--   0        0        0      360 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/alarm-warning-line.svg
--rw-r--r--   0        0        0      224 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/alert-fill.svg
--rw-r--r--   0        0        0      257 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/alert-line.svg
--rw-r--r--   0        0        0      127 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-down-fill.svg
--rw-r--r--   0        0        0      188 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-down-line.svg
--rw-r--r--   0        0        0      120 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-down-s-fill.svg
--rw-r--r--   0        0        0      173 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-down-s-line.svg
--rw-r--r--   0        0        0      159 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-go-back-fill.svg
--rw-r--r--   0        0        0      213 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-go-back-line.svg
--rw-r--r--   0        0        0      161 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-fill.svg
--rw-r--r--   0        0        0      218 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-line.svg
--rw-r--r--   0        0        0      128 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-left-fill.svg
--rw-r--r--   0        0        0      184 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-left-line.svg
--rw-r--r--   0        0        0      119 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-left-s-fill.svg
--rw-r--r--   0        0        0      173 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-left-s-line.svg
--rw-r--r--   0        0        0      128 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-right-fill.svg
--rw-r--r--   0        0        0      189 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-right-line.svg
--rw-r--r--   0        0        0      118 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-right-s-fill.svg
--rw-r--r--   0        0        0      175 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-right-s-line.svg
--rw-r--r--   0        0        0      197 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-right-up-line.svg
--rw-r--r--   0        0        0      129 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-up-fill.svg
--rw-r--r--   0        0        0      186 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-up-line.svg
--rw-r--r--   0        0        0      117 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-up-s-fill.svg
--rw-r--r--   0        0        0      173 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/arrow-up-s-line.svg
--rw-r--r--   0        0        0      177 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/check-line.svg
--rw-r--r--   0        0        0      252 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/checkbox-circle-fill.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/checkbox-circle-line.svg
--rw-r--r--   0        0        0      252 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/checkbox-fill.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/checkbox-line.svg
--rw-r--r--   0        0        0      321 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/close-circle-fill.svg
--rw-r--r--   0        0        0      342 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/close-circle-line.svg
--rw-r--r--   0        0        0      210 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/close-line.svg
--rw-r--r--   0        0        0      189 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/delete-bin-fill.svg
--rw-r--r--   0        0        0      203 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/delete-bin-line.svg
--rw-r--r--   0        0        0      142 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/download-fill.svg
--rw-r--r--   0        0        0      198 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/download-line.svg
--rw-r--r--   0        0        0      203 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/error-warning-fill.svg
--rw-r--r--   0        0        0      238 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/error-warning-line.svg
--rw-r--r--   0        0        0      228 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/external-link-fill.svg
--rw-r--r--   0        0        0      230 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/external-link-line.svg
--rw-r--r--   0        0        0      281 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/eye-fill.svg
--rw-r--r--   0        0        0      380 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/eye-line.svg
--rw-r--r--   0        0        0      481 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/eye-off-fill.svg
--rw-r--r--   0        0        0      678 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg
--rw-r--r--   0        0        0      136 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/filter-fill.svg
--rw-r--r--   0        0        0      187 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/filter-line.svg
--rw-r--r--   0        0        0      196 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-first-line.svg
--rw-r--r--   0        0        0      197 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-line-double.svg
--rw-r--r--   0        0        0      201 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-last-line.svg
--rw-r--r--   0        0        0      201 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-line-double.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--error-fill.svg
--rw-r--r--   0        0        0      309 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--error-line.svg
--rw-r--r--   0        0        0      237 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--info-fill.svg
--rw-r--r--   0        0        0      328 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--info-line.svg
--rw-r--r--   0        0        0      253 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--success-fill.svg
--rw-r--r--   0        0        0      289 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--success-line.svg
--rw-r--r--   0        0        0      482 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--theme-fill.svg
--rw-r--r--   0        0        0      225 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--warning-fill.svg
--rw-r--r--   0        0        0      258 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/fr--warning-line.svg
--rw-r--r--   0        0        0      205 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/information-fill.svg
--rw-r--r--   0        0        0      239 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/information-line.svg
--rw-r--r--   0        0        0      238 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/lock-fill.svg
--rw-r--r--   0        0        0      252 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/lock-line.svg
--rw-r--r--   0        0        0      252 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/lock-unlock-fill.svg
--rw-r--r--   0        0        0      268 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/lock-unlock-line.svg
--rw-r--r--   0        0        0      197 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/logout-box-r-fill.svg
--rw-r--r--   0        0        0      219 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/logout-box-r-line.svg
--rw-r--r--   0        0        0      145 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/menu-2-fill.svg
--rw-r--r--   0        0        0      145 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/menu-fill.svg
--rw-r--r--   0        0        0      248 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/more-fill.svg
--rw-r--r--   0        0        0      348 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/more-line.svg
--rw-r--r--   0        0        0      220 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/notification-badge-fill.svg
--rw-r--r--   0        0        0      288 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/notification-badge-line.svg
--rw-r--r--   0        0        0      311 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/question-fill.svg
--rw-r--r--   0        0        0      325 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/question-line.svg
--rw-r--r--   0        0        0      280 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/refresh-fill.svg
--rw-r--r--   0        0        0      244 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/refresh-line.svg
--rw-r--r--   0        0        0      247 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/search-fill.svg
--rw-r--r--   0        0        0      382 2022-10-17 16:38:19.645120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/search-line.svg
--rw-r--r--   0        0        0      864 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg
--rw-r--r--   0        0        0     1599 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg
--rw-r--r--   0        0        0      241 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/shield-fill.svg
--rw-r--r--   0        0        0      332 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/shield-line.svg
--rw-r--r--   0        0        0      217 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/star-fill.svg
--rw-r--r--   0        0        0      333 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/star-line.svg
--rw-r--r--   0        0        0      203 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/star-s-fill.svg
--rw-r--r--   0        0        0      325 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/star-s-line.svg
--rw-r--r--   0        0        0      117 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/subtract-line.svg
--rw-r--r--   0        0        0      341 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/thumb-down-fill.svg
--rw-r--r--   0        0        0      442 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/thumb-down-line.svg
--rw-r--r--   0        0        0      340 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/thumb-up-fill.svg
--rw-r--r--   0        0        0      459 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/thumb-up-line.svg
--rw-r--r--   0        0        0      193 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/time-fill.svg
--rw-r--r--   0        0        0      226 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/time-line.svg
--rw-r--r--   0        0        0      201 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/timer-fill.svg
--rw-r--r--   0        0        0      236 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/timer-line.svg
--rw-r--r--   0        0        0      180 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/upload-2-fill.svg
--rw-r--r--   0        0        0      180 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/upload-2-line.svg
--rw-r--r--   0        0        0      144 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/upload-fill.svg
--rw-r--r--   0        0        0      206 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/upload-line.svg
--rw-r--r--   0        0        0      279 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/zoom-in-fill.svg
--rw-r--r--   0        0        0      407 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/zoom-in-line.svg
--rw-r--r--   0        0        0      260 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/zoom-out-fill.svg
--rw-r--r--   0        0        0      388 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/zoom-out-line.svg
--rw-r--r--   0        0        0      337 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/account-circle-fill.svg
--rw-r--r--   0        0        0      462 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/account-circle-line.svg
--rw-r--r--   0        0        0      383 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/account-pin-circle-fill.svg
--rw-r--r--   0        0        0      575 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg
--rw-r--r--   0        0        0      279 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/admin-fill.svg
--rw-r--r--   0        0        0      349 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/admin-line.svg
--rw-r--r--   0        0        0      357 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/group-fill.svg
--rw-r--r--   0        0        0      462 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/group-line.svg
--rw-r--r--   0        0        0      279 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/parent-fill.svg
--rw-r--r--   0        0        0      413 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/parent-line.svg
--rw-r--r--   0        0        0      424 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/team-fill.svg
--rw-r--r--   0        0        0      750 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/team-line.svg
--rw-r--r--   0        0        0      235 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-add-fill.svg
--rw-r--r--   0        0        0      316 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-add-line.svg
--rw-r--r--   0        0        0      186 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-fill.svg
--rw-r--r--   0        0        0      314 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-heart-fill.svg
--rw-r--r--   0        0        0      439 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-heart-line.svg
--rw-r--r--   0        0        0      275 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-line.svg
--rw-r--r--   0        0        0      314 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-search-fill.svg
--rw-r--r--   0        0        0      384 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-search-line.svg
--rw-r--r--   0        0        0      529 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg
--rw-r--r--   0        0        0      462 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg
--rw-r--r--   0        0        0      298 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-star-fill.svg
--rw-r--r--   0        0        0      367 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-star-line.svg
--rw-r--r--   0        0        0      167 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/cloudy-2-fill.svg
--rw-r--r--   0        0        0      291 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/cloudy-2-line.svg
--rw-r--r--   0        0        0      128 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/flashlight-fill.svg
--rw-r--r--   0        0        0      172 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/flashlight-line.svg
--rw-r--r--   0        0        0      226 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/moon-fill.svg
--rw-r--r--   0        0        0      286 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/moon-line.svg
--rw-r--r--   0        0        0      449 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/sun-fill.svg
--rw-r--r--   0        0        0      482 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/weather/sun-line.svg
--rw-r--r--   0        0        0      466 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/README.md
--rw-r--r--   0        0        0    14496 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js
--rw-r--r--   0        0        0    38322 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js.map
--rw-r--r--   0        0        0    12899 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js
--rw-r--r--   0        0        0    30524 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js.map
--rw-r--r--   0        0        0      686 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/README.md
--rw-r--r--   0        0        0      760 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/response/README.md
--rw-r--r--   0        0        0      701 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/response/not-found/README.md
--rw-r--r--   0        0        0       13 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/response/unavailable/README.md
--rw-r--r--   0        0        0        9 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/pattern/README.md
--rw-r--r--   0        0        0      855 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/README.md
--rw-r--r--   0        0        0    13710 2022-10-17 16:38:19.649120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.css
--rw-r--r--   0        0        0    24571 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.css.map
--rw-r--r--   0        0        0    12276 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.min.css
--rw-r--r--   0        0        0    24181 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.min.css.map
--rw-r--r--   0        0        0     4982 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.js
--rw-r--r--   0        0        0    12753 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.js.map
--rw-r--r--   0        0        0     3040 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.min.js
--rw-r--r--   0        0        0    10020 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.min.js.map
--rw-r--r--   0        0        0      836 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/README.md
--rw-r--r--   0        0        0      421 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/README.md
--rw-r--r--   0        0        0    66279 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.css
--rw-r--r--   0        0        0   119166 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.css.map
--rw-r--r--   0        0        0    32212 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css
--rw-r--r--   0        0        0    76114 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css.map
--rw-r--r--   0        0        0    26350 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css
--rw-r--r--   0        0        0    74279 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css.map
--rw-r--r--   0        0        0    34195 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.css
--rw-r--r--   0        0        0    54325 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.css.map
--rw-r--r--   0        0        0    30990 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css
--rw-r--r--   0        0        0    53474 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css.map
--rw-r--r--   0        0        0    57212 2022-10-17 16:38:19.653120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.min.css
--rw-r--r--   0        0        0   116475 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.min.css.map
--rw-r--r--   0        0        0      733 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/README.md
--rw-r--r--   0        0        0      788 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md
--rw-r--r--   0        0        0     8218 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css
--rw-r--r--   0        0        0    18263 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css.map
--rw-r--r--   0        0        0     3542 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css
--rw-r--r--   0        0        0     8459 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css.map
--rw-r--r--   0        0        0     3036 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css
--rw-r--r--   0        0        0     8334 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
--rw-r--r--   0        0        0     4916 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css
--rw-r--r--   0        0        0    11989 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css.map
--rw-r--r--   0        0        0     4370 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css
--rw-r--r--   0        0        0    11318 2022-10-17 16:38:19.657120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css.map
--rw-r--r--   0        0        0     7178 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css
--rw-r--r--   0        0        0    17459 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css.map
--rw-r--r--   0        0        0      782 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md
--rw-r--r--   0        0        0    22912 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css
--rw-r--r--   0        0        0    36317 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css.map
--rw-r--r--   0        0        0     9504 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css
--rw-r--r--   0        0        0    15677 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css.map
--rw-r--r--   0        0        0     8088 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css
--rw-r--r--   0        0        0    15303 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css.map
--rw-r--r--   0        0        0    13648 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css
--rw-r--r--   0        0        0    22781 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css.map
--rw-r--r--   0        0        0    12243 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css
--rw-r--r--   0        0        0    21812 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css.map
--rw-r--r--   0        0        0    20103 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css
--rw-r--r--   0        0        0    34966 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css.map
--rw-r--r--   0        0        0      817 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md
--rw-r--r--   0        0        0     8770 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css
--rw-r--r--   0        0        0    18760 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css.map
--rw-r--r--   0        0        0     3786 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css
--rw-r--r--   0        0        0     8631 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css.map
--rw-r--r--   0        0        0     3272 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css
--rw-r--r--   0        0        0     8504 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css.map
--rw-r--r--   0        0        0     5224 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css
--rw-r--r--   0        0        0    12318 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css.map
--rw-r--r--   0        0        0     4674 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css
--rw-r--r--   0        0        0    11630 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css.map
--rw-r--r--   0        0        0     7718 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css
--rw-r--r--   0        0        0    17937 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css.map
--rw-r--r--   0        0        0      768 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md
--rw-r--r--   0        0        0    15237 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css
--rw-r--r--   0        0        0    26962 2022-10-17 16:38:19.661120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css.map
--rw-r--r--   0        0        0     6494 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css
--rw-r--r--   0        0        0    12046 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css.map
--rw-r--r--   0        0        0     5504 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css
--rw-r--r--   0        0        0    11789 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css.map
--rw-r--r--   0        0        0     8983 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css
--rw-r--r--   0        0        0    17098 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css.map
--rw-r--r--   0        0        0     8000 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css
--rw-r--r--   0        0        0    16284 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css.map
--rw-r--r--   0        0        0    13276 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css
--rw-r--r--   0        0        0    25883 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css.map
--rw-r--r--   0        0        0      803 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md
--rw-r--r--   0        0        0    10584 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css
--rw-r--r--   0        0        0    20874 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css.map
--rw-r--r--   0        0        0     4556 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css
--rw-r--r--   0        0        0     9515 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css.map
--rw-r--r--   0        0        0     3954 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css
--rw-r--r--   0        0        0     9364 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css.map
--rw-r--r--   0        0        0     6268 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css
--rw-r--r--   0        0        0    13546 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css.map
--rw-r--r--   0        0        0     5638 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css
--rw-r--r--   0        0        0    12836 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css.map
--rw-r--r--   0        0        0     9364 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css
--rw-r--r--   0        0        0    20005 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css.map
--rw-r--r--   0        0        0      768 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md
--rw-r--r--   0        0        0    13498 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css
--rw-r--r--   0        0        0    24927 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css.map
--rw-r--r--   0        0        0     5696 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css
--rw-r--r--   0        0        0    11137 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css.map
--rw-r--r--   0        0        0     4810 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css
--rw-r--r--   0        0        0    10908 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css.map
--rw-r--r--   0        0        0     8042 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css
--rw-r--r--   0        0        0    15972 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css.map
--rw-r--r--   0        0        0     7132 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css
--rw-r--r--   0        0        0    15179 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css.map
--rw-r--r--   0        0        0    11714 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css
--rw-r--r--   0        0        0    23897 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css.map
--rw-r--r--   0        0        0      782 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md
--rw-r--r--   0        0        0    12044 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css
--rw-r--r--   0        0        0    23019 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css.map
--rw-r--r--   0        0        0     5060 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css
--rw-r--r--   0        0        0    10329 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css.map
--rw-r--r--   0        0        0     4306 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css
--rw-r--r--   0        0        0    10136 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css.map
--rw-r--r--   0        0        0     7224 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css
--rw-r--r--   0        0        0    14874 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css.map
--rw-r--r--   0        0        0     6434 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css
--rw-r--r--   0        0        0    14117 2022-10-17 16:38:19.665120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css.map
--rw-r--r--   0        0        0    10512 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css
--rw-r--r--   0        0        0    22061 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css.map
--rw-r--r--   0        0        0      768 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md
--rw-r--r--   0        0        0    10188 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css
--rw-r--r--   0        0        0    21002 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css.map
--rw-r--r--   0        0        0     4282 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css
--rw-r--r--   0        0        0     9492 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css.map
--rw-r--r--   0        0        0     3576 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css
--rw-r--r--   0        0        0     9312 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css.map
--rw-r--r--   0        0        0     6146 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css
--rw-r--r--   0        0        0    13692 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css.map
--rw-r--r--   0        0        0     5396 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css
--rw-r--r--   0        0        0    12955 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css.map
--rw-r--r--   0        0        0     8744 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css
--rw-r--r--   0        0        0    20077 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css.map
--rw-r--r--   0        0        0      775 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md
--rw-r--r--   0        0        0     6775 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css
--rw-r--r--   0        0        0    16356 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css.map
--rw-r--r--   0        0        0     2988 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css
--rw-r--r--   0        0        0     7682 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css.map
--rw-r--r--   0        0        0     2584 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css
--rw-r--r--   0        0        0     7585 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css.map
--rw-r--r--   0        0        0     4027 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css
--rw-r--r--   0        0        0    10857 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css.map
--rw-r--r--   0        0        0     3577 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css
--rw-r--r--   0        0        0    10222 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css.map
--rw-r--r--   0        0        0     5933 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css
--rw-r--r--   0        0        0    15616 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css.map
--rw-r--r--   0        0        0      768 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md
--rw-r--r--   0        0        0    14367 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css
--rw-r--r--   0        0        0    25638 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css.map
--rw-r--r--   0        0        0     6168 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css
--rw-r--r--   0        0        0    11499 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css.map
--rw-r--r--   0        0        0     5280 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css
--rw-r--r--   0        0        0    11270 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css.map
--rw-r--r--   0        0        0     8439 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css
--rw-r--r--   0        0        0    16321 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css.map
--rw-r--r--   0        0        0     7549 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css
--rw-r--r--   0        0        0    15535 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css.map
--rw-r--r--   0        0        0    12601 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css
--rw-r--r--   0        0        0    24615 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css.map
--rw-r--r--   0        0        0      754 2022-10-17 16:38:19.669120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md
--rw-r--r--   0        0        0    24122 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css
--rw-r--r--   0        0        0    38266 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css.map
--rw-r--r--   0        0        0     9746 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css
--rw-r--r--   0        0        0    16193 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css.map
--rw-r--r--   0        0        0     8200 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css
--rw-r--r--   0        0        0    15782 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css.map
--rw-r--r--   0        0        0    14616 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css
--rw-r--r--   0        0        0    24170 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css.map
--rw-r--r--   0        0        0    13026 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css
--rw-r--r--   0        0        0    23145 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css.map
--rw-r--r--   0        0        0    20998 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css
--rw-r--r--   0        0        0    36822 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css.map
--rw-r--r--   0        0        0      747 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md
--rw-r--r--   0        0        0    17550 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css
--rw-r--r--   0        0        0    29889 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css.map
--rw-r--r--   0        0        0     7456 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css
--rw-r--r--   0        0        0    13240 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css.map
--rw-r--r--   0        0        0     6298 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css
--rw-r--r--   0        0        0    12937 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css.map
--rw-r--r--   0        0        0    10334 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css
--rw-r--r--   0        0        0    18828 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css.map
--rw-r--r--   0        0        0     9184 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css
--rw-r--r--   0        0        0    17960 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css.map
--rw-r--r--   0        0        0    15254 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css
--rw-r--r--   0        0        0    28710 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css.map
--rw-r--r--   0        0        0      761 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md
--rw-r--r--   0        0        0    18969 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css
--rw-r--r--   0        0        0    31555 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css.map
--rw-r--r--   0        0        0     7860 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css
--rw-r--r--   0        0        0    13741 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css.map
--rw-r--r--   0        0        0     6668 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css
--rw-r--r--   0        0        0    13428 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css.map
--rw-r--r--   0        0        0    11349 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css
--rw-r--r--   0        0        0    19995 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css.map
--rw-r--r--   0        0        0    10139 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css
--rw-r--r--   0        0        0    19100 2022-10-17 16:38:19.673120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css.map
--rw-r--r--   0        0        0    16579 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css
--rw-r--r--   0        0        0    30339 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css.map
--rw-r--r--   0        0        0      767 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md
--rw-r--r--   0        0        0     5250 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css
--rw-r--r--   0        0        0    14596 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css.map
--rw-r--r--   0        0        0     2350 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css
--rw-r--r--   0        0        0     6956 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css.map
--rw-r--r--   0        0        0     2012 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css
--rw-r--r--   0        0        0     6877 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css.map
--rw-r--r--   0        0        0     3140 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css
--rw-r--r--   0        0        0     9822 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css.map
--rw-r--r--   0        0        0     2750 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css
--rw-r--r--   0        0        0     9211 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css.map
--rw-r--r--   0        0        0     4534 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css
--rw-r--r--   0        0        0    13898 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css.map
--rw-r--r--   0        0        0      768 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md
--rw-r--r--   0        0        0    59570 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css
--rw-r--r--   0        0        0    82014 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css.map
--rw-r--r--   0        0        0    23823 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css
--rw-r--r--   0        0        0    33361 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css.map
--rw-r--r--   0        0        0    20177 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css
--rw-r--r--   0        0        0    32374 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css.map
--rw-r--r--   0        0        0    35987 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css
--rw-r--r--   0        0        0    50579 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css.map
--rw-r--r--   0        0        0    32364 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css
--rw-r--r--   0        0        0    48850 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css.map
--rw-r--r--   0        0        0    52313 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css
--rw-r--r--   0        0        0    79290 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css.map
--rw-r--r--   0        0        0      754 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md
--rw-r--r--   0        0        0    10694 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css
--rw-r--r--   0        0        0    21341 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css.map
--rw-r--r--   0        0        0     4602 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css
--rw-r--r--   0        0        0     9747 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css.map
--rw-r--r--   0        0        0     3920 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css
--rw-r--r--   0        0        0     9574 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css.map
--rw-r--r--   0        0        0     6332 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css
--rw-r--r--   0        0        0    13774 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css.map
--rw-r--r--   0        0        0     5622 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css
--rw-r--r--   0        0        0    13057 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css.map
--rw-r--r--   0        0        0     9314 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css
--rw-r--r--   0        0        0    20443 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css.map
--rw-r--r--   0        0        0      775 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md
--rw-r--r--   0        0        0     3858 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css
--rw-r--r--   0        0        0    12976 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css.map
--rw-r--r--   0        0        0     1726 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css
--rw-r--r--   0        0        0     6293 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css.map
--rw-r--r--   0        0        0     1484 2022-10-17 16:38:19.677120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css
--rw-r--r--   0        0        0     6240 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css.map
--rw-r--r--   0        0        0     2372 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css
--rw-r--r--   0        0        0     8866 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css.map
--rw-r--r--   0        0        0     2062 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css
--rw-r--r--   0        0        0     8280 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css.map
--rw-r--r--   0        0        0     3318 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css
--rw-r--r--   0        0        0    12329 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css.map
--rw-r--r--   0        0        0   250598 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.css
--rw-r--r--   0        0        0   337223 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.css.map
--rw-r--r--   0        0        0   102435 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css
--rw-r--r--   0        0        0   134791 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css.map
--rw-r--r--   0        0        0    86377 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css
--rw-r--r--   0        0        0   130362 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css.map
--rw-r--r--   0        0        0   148403 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.css
--rw-r--r--   0        0        0   202877 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.css.map
--rw-r--r--   0        0        0   132072 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css
--rw-r--r--   0        0        0   188914 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css.map
--rw-r--r--   0        0        0   218221 2022-10-17 16:38:19.681120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.min.css
--rw-r--r--   0        0        0   317317 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.min.css.map
--rw-r--r--   0        0        0   310059 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.css
--rw-r--r--   0        0        0   449720 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.css.map
--rw-r--r--   0        0        0   132265 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.css
--rw-r--r--   0        0        0   208183 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.css.map
--rw-r--r--   0        0        0   110355 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.min.css
--rw-r--r--   0        0        0   201910 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.min.css.map
--rw-r--r--   0        0        0   178034 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.css
--rw-r--r--   0        0        0   252994 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.css.map
--rw-r--r--   0        0        0   158494 2022-10-17 16:38:19.685120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.min.css
--rw-r--r--   0        0        0   238156 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.min.css.map
--rw-r--r--   0        0        0   268621 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.min.css
--rw-r--r--   0        0        0   426746 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.min.css.map
--rw-r--r--   0        0        0      527 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/django/forms/widgets/checkbox_option.html
--rw-r--r--   0        0        0      394 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/django/forms/widgets/input_option.html
--rw-r--r--   0        0        0      212 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/django/forms/widgets/multiple_input.html
--rw-r--r--   0        0        0      386 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/accordion.html
--rw-r--r--   0        0        0      138 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/accordion_group.html
--rw-r--r--   0        0        0      699 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/alert.html
--rw-r--r--   0        0        0      103 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/badge.html
--rw-r--r--   0        0        0      147 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/badge_group.html
--rw-r--r--   0        0        0      786 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/breadcrumb.html
--rw-r--r--   0        0        0      240 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/button.html
--rw-r--r--   0        0        0      575 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/callout.html
--rw-r--r--   0        0        0     3745 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/card.html
--rw-r--r--   0        0        0      451 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/favicon.html
--rw-r--r--   0        0        0     2791 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/footer.html
--rw-r--r--   0        0        0      364 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html
--rw-r--r--   0        0        0      708 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html
--rw-r--r--   0        0        0      357 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/field_snippet.html
--rw-r--r--   0        0        0      835 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/input_snippet.html
--rw-r--r--   0        0        0      100 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/form_snippet.html
--rw-r--r--   0        0        0      285 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/global_css.html
--rw-r--r--   0        0        0      188 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/global_js.html
--rw-r--r--   0        0        0     3356 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/header.html
--rw-r--r--   0        0        0      141 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/highlight.html
--rw-r--r--   0        0        0      578 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/input.html
--rw-r--r--   0        0        0      394 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/link.html
--rw-r--r--   0        0        0     2564 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/pagination.html
--rw-r--r--   0        0        0     1008 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/quote.html
--rw-r--r--   0        0        0      968 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/select.html
--rw-r--r--   0        0        0     3526 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/sidemenu.html
--rw-r--r--   0        0        0      344 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/skiplinks.html
--rw-r--r--   0        0        0      369 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/summary.html
--rw-r--r--   0        0        0      683 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/table.html
--rw-r--r--   0        0        0      681 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/tag.html
--rw-r--r--   0        0        0     3422 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/theme_modale.html
--rw-r--r--   0        0        0      407 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templates/dsfr/tile.html
--rw-r--r--   0        0        0        0 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templatetags/__init__.py
--rw-r--r--   0        0        0    23659 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/templatetags/dsfr_tags.py
--rw-r--r--   0        0        0        0 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/test/__init__.py
--rw-r--r--   0        0        0      909 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/test/test_config.py
--rw-r--r--   0        0        0    26318 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/test/test_templatetags.py
--rw-r--r--   0        0        0     1116 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/test/test_utils.py
--rw-r--r--   0        0        0     3141 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/utils.py
--rw-r--r--   0        0        0       63 2022-10-17 16:38:19.689120 django_dsfr-0.9.4/dsfr/views.py
--rw-r--r--   0        0        0     1470 2022-10-17 16:38:19.693120 django_dsfr-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     8422 1970-01-01 00:00:00.000000 django_dsfr-0.9.4/setup.py
--rw-r--r--   0        0        0     4235 1970-01-01 00:00:00.000000 django_dsfr-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1190 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2790 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/README.rst
+-rw-r--r--   0        0        0        0 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/__init__.py
+-rw-r--r--   0        0        0      666 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/admin.py
+-rw-r--r--   0        0        0      193 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/apps.py
+-rw-r--r--   0        0        0      152 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/context_processors.py
+-rw-r--r--   0        0        0      454 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/fixtures/init.json
+-rw-r--r--   0        0        0     1932 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/forms.py
+-rw-r--r--   0        0        0     1798 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2254 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/migrations/0002_auto_20211209_1557.py
+-rw-r--r--   0        0        0      553 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py
+-rw-r--r--   0        0        0        0 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/migrations/__init__.py
+-rw-r--r--   0        0        0     1855 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/models.py
+-rw-r--r--   0        0        0      469 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/README.md
+-rw-r--r--   0        0        0    16409 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/background/ovoid.svg
+-rw-r--r--   0        0        0     4127 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/dark.svg
+-rw-r--r--   0        0        0     4958 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/light.svg
+-rw-r--r--   0        0        0    15223 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/system.svg
+-rw-r--r--   0        0        0     2317 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/technical-error.svg
+-rw-r--r--   0        0        0     4967 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/test.svg
+-rw-r--r--   0        0        0      964 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/README.md
+-rw-r--r--   0        0        0     1145 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/README.md
+-rw-r--r--   0        0        0     4006 2022-10-19 09:15:30.270830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.css
+-rw-r--r--   0        0        0    46932 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.css.map
+-rw-r--r--   0        0        0     1422 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css
+-rw-r--r--   0        0        0    23139 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css.map
+-rw-r--r--   0        0        0     1090 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css
+-rw-r--r--   0        0        0    22480 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css.map
+-rw-r--r--   0        0        0     2843 2022-10-19 09:15:30.278830 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.css
+-rw-r--r--   0        0        0    41772 2022-10-19 09:15:30.282831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.css.map
+-rw-r--r--   0        0        0     2271 2022-10-19 09:15:30.282831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css
+-rw-r--r--   0        0        0    41227 2022-10-19 09:15:30.282831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css.map
+-rw-r--r--   0        0        0     3133 2022-10-19 09:15:30.282831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.min.css
+-rw-r--r--   0        0        0    45730 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.min.css.map
+-rw-r--r--   0        0        0      913 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.js
+-rw-r--r--   0        0        0     2596 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.js.map
+-rw-r--r--   0        0        0      619 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js
+-rw-r--r--   0        0        0     2258 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js.map
+-rw-r--r--   0        0        0     1561 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js
+-rw-r--r--   0        0        0     2552 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js.map
+-rw-r--r--   0        0        0      875 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js
+-rw-r--r--   0        0        0     2288 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js.map
+-rw-r--r--   0        0        0      732 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/README.md
+-rw-r--r--   0        0        0     6219 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.css
+-rw-r--r--   0        0        0    44082 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.css.map
+-rw-r--r--   0        0        0     2205 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.css
+-rw-r--r--   0        0        0    24264 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.css.map
+-rw-r--r--   0        0        0     1591 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css
+-rw-r--r--   0        0        0    23737 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css.map
+-rw-r--r--   0        0        0     4255 2022-10-19 09:15:30.286831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.css
+-rw-r--r--   0        0        0    37199 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.css.map
+-rw-r--r--   0        0        0     3510 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.min.css
+-rw-r--r--   0        0        0    36557 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.min.css.map
+-rw-r--r--   0        0        0     4873 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.min.css
+-rw-r--r--   0        0        0    42896 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.min.css.map
+-rw-r--r--   0        0        0      670 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/README.md
+-rw-r--r--   0        0        0    15641 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.css
+-rw-r--r--   0        0        0    71605 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.css.map
+-rw-r--r--   0        0        0     3928 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.css
+-rw-r--r--   0        0        0    31260 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.css.map
+-rw-r--r--   0        0        0     3116 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css
+-rw-r--r--   0        0        0    31066 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css.map
+-rw-r--r--   0        0        0    11954 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.css
+-rw-r--r--   0        0        0    60075 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.css.map
+-rw-r--r--   0        0        0    10542 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.min.css
+-rw-r--r--   0        0        0    59256 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.min.css.map
+-rw-r--r--   0        0        0    13430 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.min.css
+-rw-r--r--   0        0        0    70608 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.min.css.map
+-rw-r--r--   0        0        0     1179 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/README.md
+-rw-r--r--   0        0        0     3808 2022-10-19 09:15:30.290831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css
+-rw-r--r--   0        0        0    38146 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css.map
+-rw-r--r--   0        0        0     1026 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css
+-rw-r--r--   0        0        0    22443 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css.map
+-rw-r--r--   0        0        0      784 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css
+-rw-r--r--   0        0        0    21919 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css.map
+-rw-r--r--   0        0        0     3041 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css
+-rw-r--r--   0        0        0    34129 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css.map
+-rw-r--r--   0        0        0     2283 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css
+-rw-r--r--   0        0        0    33545 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css.map
+-rw-r--r--   0        0        0     2839 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css
+-rw-r--r--   0        0        0    37041 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css.map
+-rw-r--r--   0        0        0     2225 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js
+-rw-r--r--   0        0        0     6007 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js.map
+-rw-r--r--   0        0        0     1462 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js
+-rw-r--r--   0        0        0     4793 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js.map
+-rw-r--r--   0        0        0     3421 2022-10-19 09:15:30.294831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js
+-rw-r--r--   0        0        0     5944 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js.map
+-rw-r--r--   0        0        0     1957 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js
+-rw-r--r--   0        0        0     4880 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js.map
+-rw-r--r--   0        0        0     1115 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/README.md
+-rw-r--r--   0        0        0    39219 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.css
+-rw-r--r--   0        0        0   106440 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.css.map
+-rw-r--r--   0        0        0     9674 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.css
+-rw-r--r--   0        0        0    40803 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.css.map
+-rw-r--r--   0        0        0     8440 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.min.css
+-rw-r--r--   0        0        0    40562 2022-10-19 09:15:30.298831 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.min.css.map
+-rw-r--r--   0        0        0    29786 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.css
+-rw-r--r--   0        0        0    85565 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.css.map
+-rw-r--r--   0        0        0    26098 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.min.css
+-rw-r--r--   0        0        0    84202 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.min.css.map
+-rw-r--r--   0        0        0    34310 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.min.css
+-rw-r--r--   0        0        0   104814 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.min.css.map
+-rw-r--r--   0        0        0      761 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.js
+-rw-r--r--   0        0        0     1961 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.js.map
+-rw-r--r--   0        0        0      559 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.min.js
+-rw-r--r--   0        0        0     1692 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.min.js.map
+-rw-r--r--   0        0        0      834 2022-10-19 09:15:30.302832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.js
+-rw-r--r--   0        0        0     1943 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.js.map
+-rw-r--r--   0        0        0      583 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js
+-rw-r--r--   0        0        0     1699 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js.map
+-rw-r--r--   0        0        0      791 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/README.md
+-rw-r--r--   0        0        0     9442 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.css
+-rw-r--r--   0        0        0    39264 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.css.map
+-rw-r--r--   0        0        0     2612 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.css
+-rw-r--r--   0        0        0    23866 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.css.map
+-rw-r--r--   0        0        0     2091 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css
+-rw-r--r--   0        0        0    23758 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css.map
+-rw-r--r--   0        0        0     7070 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.css
+-rw-r--r--   0        0        0    30331 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.css.map
+-rw-r--r--   0        0        0     6203 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.min.css
+-rw-r--r--   0        0        0    29713 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.min.css.map
+-rw-r--r--   0        0        0     8066 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.min.css
+-rw-r--r--   0        0        0    38530 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.min.css.map
+-rw-r--r--   0        0        0     1070 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/README.md
+-rw-r--r--   0        0        0    10928 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.css
+-rw-r--r--   0        0        0    62169 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.css.map
+-rw-r--r--   0        0        0     1686 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.css
+-rw-r--r--   0        0        0    21335 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.css.map
+-rw-r--r--   0        0        0     1328 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.min.css
+-rw-r--r--   0        0        0    21256 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.min.css.map
+-rw-r--r--   0        0        0     9483 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.css
+-rw-r--r--   0        0        0    55982 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.css.map
+-rw-r--r--   0        0        0     7972 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.min.css
+-rw-r--r--   0        0        0    54994 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.min.css.map
+-rw-r--r--   0        0        0     9072 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.min.css
+-rw-r--r--   0        0        0    61094 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.min.css.map
+-rw-r--r--   0        0        0      970 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/README.md
+-rw-r--r--   0        0        0     7827 2022-10-19 09:15:30.306832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.css
+-rw-r--r--   0        0        0    38280 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.css.map
+-rw-r--r--   0        0        0     2384 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css
+-rw-r--r--   0        0        0    20619 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css.map
+-rw-r--r--   0        0        0     1518 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css
+-rw-r--r--   0        0        0    20480 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css.map
+-rw-r--r--   0        0        0     5770 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css
+-rw-r--r--   0        0        0    33762 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css.map
+-rw-r--r--   0        0        0     3809 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css
+-rw-r--r--   0        0        0    32947 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css.map
+-rw-r--r--   0        0        0     5099 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css
+-rw-r--r--   0        0        0    37353 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css.map
+-rw-r--r--   0        0        0   410184 2022-10-19 09:15:30.310832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.css
+-rw-r--r--   0        0        0   920455 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.css.map
+-rw-r--r--   0        0        0   108837 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.css
+-rw-r--r--   0        0        0   317932 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.css.map
+-rw-r--r--   0        0        0    85909 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.min.css
+-rw-r--r--   0        0        0   305852 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.min.css.map
+-rw-r--r--   0        0        0   303311 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.css
+-rw-r--r--   0        0        0   675083 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.css.map
+-rw-r--r--   0        0        0   248216 2022-10-19 09:15:30.314832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.min.css
+-rw-r--r--   0        0        0   640056 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.min.css.map
+-rw-r--r--   0        0        0   333239 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.min.css
+-rw-r--r--   0        0        0   877679 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.min.css.map
+-rw-r--r--   0        0        0    39818 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.js
+-rw-r--r--   0        0        0   102818 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.js.map
+-rw-r--r--   0        0        0    25225 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.min.js
+-rw-r--r--   0        0        0    79906 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.min.js.map
+-rw-r--r--   0        0        0    59695 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.js
+-rw-r--r--   0        0        0   100791 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.js.map
+-rw-r--r--   0        0        0    33147 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.min.js
+-rw-r--r--   0        0        0    80290 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.min.js.map
+-rw-r--r--   0        0        0      702 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/README.md
+-rw-r--r--   0        0        0     8502 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.css
+-rw-r--r--   0        0        0    38832 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.css.map
+-rw-r--r--   0        0        0      990 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.css
+-rw-r--r--   0        0        0    16990 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.css.map
+-rw-r--r--   0        0        0      837 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css
+-rw-r--r--   0        0        0    16973 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css.map
+-rw-r--r--   0        0        0     7753 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.css
+-rw-r--r--   0        0        0    34706 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.css.map
+-rw-r--r--   0        0        0     7308 2022-10-19 09:15:30.318832 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.min.css
+-rw-r--r--   0        0        0    34180 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.min.css.map
+-rw-r--r--   0        0        0     7917 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.min.css
+-rw-r--r--   0        0        0    38280 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.min.css.map
+-rw-r--r--   0        0        0     1494 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/README.md
+-rw-r--r--   0        0        0     9546 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.css
+-rw-r--r--   0        0        0    63891 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.css.map
+-rw-r--r--   0        0        0     1832 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.css
+-rw-r--r--   0        0        0    21340 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.css.map
+-rw-r--r--   0        0        0     1575 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css
+-rw-r--r--   0        0        0    21317 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css.map
+-rw-r--r--   0        0        0     7954 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.css
+-rw-r--r--   0        0        0    57724 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.css.map
+-rw-r--r--   0        0        0     6348 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.min.css
+-rw-r--r--   0        0        0    56970 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.min.css.map
+-rw-r--r--   0        0        0     7695 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.min.css
+-rw-r--r--   0        0        0    63102 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.min.css.map
+-rw-r--r--   0        0        0      868 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/README.md
+-rw-r--r--   0        0        0     6585 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.css
+-rw-r--r--   0        0        0    49482 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.css.map
+-rw-r--r--   0        0        0     2287 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.css
+-rw-r--r--   0        0        0    21297 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.css.map
+-rw-r--r--   0        0        0     1955 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.min.css
+-rw-r--r--   0        0        0    21246 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.min.css.map
+-rw-r--r--   0        0        0     4539 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.css
+-rw-r--r--   0        0        0    42935 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.css.map
+-rw-r--r--   0        0        0     3834 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.min.css
+-rw-r--r--   0        0        0    42175 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.min.css.map
+-rw-r--r--   0        0        0     5561 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.min.css
+-rw-r--r--   0        0        0    48661 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.min.css.map
+-rw-r--r--   0        0        0     1462 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/README.md
+-rw-r--r--   0        0        0     2053 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.js
+-rw-r--r--   0        0        0     5375 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.js.map
+-rw-r--r--   0        0        0     1378 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.min.js
+-rw-r--r--   0        0        0     4408 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.min.js.map
+-rw-r--r--   0        0        0     3304 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.js
+-rw-r--r--   0        0        0     5308 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.js.map
+-rw-r--r--   0        0        0     1891 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js
+-rw-r--r--   0        0        0     4467 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js.map
+-rw-r--r--   0        0        0     1098 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/README.md
+-rw-r--r--   0        0        0     5134 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.css
+-rw-r--r--   0        0        0    45037 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.css.map
+-rw-r--r--   0        0        0     4331 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.min.css
+-rw-r--r--   0        0        0    44381 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.min.css.map
+-rw-r--r--   0        0        0     3351 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.js
+-rw-r--r--   0        0        0     8599 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.js.map
+-rw-r--r--   0        0        0     2150 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.min.js
+-rw-r--r--   0        0        0     6818 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.min.js.map
+-rw-r--r--   0        0        0     4446 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.js
+-rw-r--r--   0        0        0     8460 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.js.map
+-rw-r--r--   0        0        0     2531 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js
+-rw-r--r--   0        0        0     6863 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js.map
+-rw-r--r--   0        0        0     1061 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/README.md
+-rw-r--r--   0        0        0    19629 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.css
+-rw-r--r--   0        0        0    81515 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.css.map
+-rw-r--r--   0        0        0     7301 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.css
+-rw-r--r--   0        0        0    32183 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.css.map
+-rw-r--r--   0        0        0     6007 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css
+-rw-r--r--   0        0        0    31290 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css.map
+-rw-r--r--   0        0        0    12587 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.css
+-rw-r--r--   0        0        0    65641 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.css.map
+-rw-r--r--   0        0        0    10004 2022-10-19 09:15:30.322833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.min.css
+-rw-r--r--   0        0        0    63612 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.min.css.map
+-rw-r--r--   0        0        0    15783 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.min.css
+-rw-r--r--   0        0        0    79221 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.min.css.map
+-rw-r--r--   0        0        0      933 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/README.md
+-rw-r--r--   0        0        0    11645 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.css
+-rw-r--r--   0        0        0    61397 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.css.map
+-rw-r--r--   0        0        0     1296 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.css
+-rw-r--r--   0        0        0    22953 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.css.map
+-rw-r--r--   0        0        0      966 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css
+-rw-r--r--   0        0        0    22439 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css.map
+-rw-r--r--   0        0        0    10608 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.css
+-rw-r--r--   0        0        0    57898 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.css.map
+-rw-r--r--   0        0        0     7180 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.min.css
+-rw-r--r--   0        0        0    56275 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.min.css.map
+-rw-r--r--   0        0        0     7918 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.min.css
+-rw-r--r--   0        0        0    59261 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.min.css.map
+-rw-r--r--   0        0        0      563 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/README.md
+-rw-r--r--   0        0        0     8815 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.css
+-rw-r--r--   0        0        0    49398 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.css.map
+-rw-r--r--   0        0        0     2826 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.css
+-rw-r--r--   0        0        0    23948 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.css.map
+-rw-r--r--   0        0        0     1491 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.min.css
+-rw-r--r--   0        0        0    23610 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.min.css.map
+-rw-r--r--   0        0        0     6319 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.css
+-rw-r--r--   0        0        0    41901 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.css.map
+-rw-r--r--   0        0        0     4309 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.min.css
+-rw-r--r--   0        0        0    40971 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.min.css.map
+-rw-r--r--   0        0        0     5572 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.min.css
+-rw-r--r--   0        0        0    48171 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.min.css.map
+-rw-r--r--   0        0        0     2239 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/README.md
+-rw-r--r--   0        0        0    23738 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.css
+-rw-r--r--   0        0        0    93426 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.css.map
+-rw-r--r--   0        0        0     6650 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.css
+-rw-r--r--   0        0        0    39667 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.css.map
+-rw-r--r--   0        0        0     5511 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.min.css
+-rw-r--r--   0        0        0    39340 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.min.css.map
+-rw-r--r--   0        0        0    17329 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.css
+-rw-r--r--   0        0        0    78442 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.css.map
+-rw-r--r--   0        0        0    14644 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.min.css
+-rw-r--r--   0        0        0    77171 2022-10-19 09:15:30.326833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.min.css.map
+-rw-r--r--   0        0        0    19927 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.min.css
+-rw-r--r--   0        0        0    91812 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.min.css.map
+-rw-r--r--   0        0        0     3409 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.js
+-rw-r--r--   0        0        0     8125 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.js.map
+-rw-r--r--   0        0        0     2352 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.min.js
+-rw-r--r--   0        0        0     6627 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.min.js.map
+-rw-r--r--   0        0        0     4882 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.js
+-rw-r--r--   0        0        0     7940 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.js.map
+-rw-r--r--   0        0        0     2896 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js
+-rw-r--r--   0        0        0     6632 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js.map
+-rw-r--r--   0        0        0      704 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/README.md
+-rw-r--r--   0        0        0     4095 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.css
+-rw-r--r--   0        0        0    25802 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.css.map
+-rw-r--r--   0        0        0     1888 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css
+-rw-r--r--   0        0        0    15944 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css.map
+-rw-r--r--   0        0        0     1570 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css
+-rw-r--r--   0        0        0    15859 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css.map
+-rw-r--r--   0        0        0     2447 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.css
+-rw-r--r--   0        0        0    20905 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.css.map
+-rw-r--r--   0        0        0     2134 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css
+-rw-r--r--   0        0        0    20344 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css.map
+-rw-r--r--   0        0        0     3476 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.min.css
+-rw-r--r--   0        0        0    25147 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.min.css.map
+-rw-r--r--   0        0        0      804 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/README.md
+-rw-r--r--   0        0        0     7031 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.css
+-rw-r--r--   0        0        0    44445 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.css.map
+-rw-r--r--   0        0        0     2529 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.css
+-rw-r--r--   0        0        0    21651 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.css.map
+-rw-r--r--   0        0        0     1809 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.min.css
+-rw-r--r--   0        0        0    21482 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.min.css.map
+-rw-r--r--   0        0        0     5031 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.css
+-rw-r--r--   0        0        0    39484 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.css.map
+-rw-r--r--   0        0        0     3993 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.min.css
+-rw-r--r--   0        0        0    38818 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.min.css.map
+-rw-r--r--   0        0        0     5437 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.min.css
+-rw-r--r--   0        0        0    43676 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.min.css.map
+-rw-r--r--   0        0        0      785 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/README.md
+-rw-r--r--   0        0        0     9985 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.css
+-rw-r--r--   0        0        0    56085 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.css.map
+-rw-r--r--   0        0        0     1781 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.css
+-rw-r--r--   0        0        0    24978 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.css.map
+-rw-r--r--   0        0        0     1273 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.min.css
+-rw-r--r--   0        0        0    24813 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.min.css.map
+-rw-r--r--   0        0        0     8445 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.css
+-rw-r--r--   0        0        0    50271 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.css.map
+-rw-r--r--   0        0        0     7364 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.min.css
+-rw-r--r--   0        0        0    49346 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.min.css.map
+-rw-r--r--   0        0        0     8409 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.min.css
+-rw-r--r--   0        0        0    54985 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.min.css.map
+-rw-r--r--   0        0        0      435 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/README.md
+-rw-r--r--   0        0        0    12189 2022-10-19 09:15:30.330833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.css
+-rw-r--r--   0        0        0    40172 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.css.map
+-rw-r--r--   0        0        0      428 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.css
+-rw-r--r--   0        0        0    12090 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.css.map
+-rw-r--r--   0        0        0      383 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css
+-rw-r--r--   0        0        0    12090 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css.map
+-rw-r--r--   0        0        0    12001 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.css
+-rw-r--r--   0        0        0    38695 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.css.map
+-rw-r--r--   0        0        0    11538 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.min.css
+-rw-r--r--   0        0        0    38182 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.min.css.map
+-rw-r--r--   0        0        0    11693 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.min.css
+-rw-r--r--   0        0        0    39650 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.min.css.map
+-rw-r--r--   0        0        0     1389 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/README.md
+-rw-r--r--   0        0        0     3843 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.css
+-rw-r--r--   0        0        0    38267 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.css.map
+-rw-r--r--   0        0        0      617 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.css
+-rw-r--r--   0        0        0    14164 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.css.map
+-rw-r--r--   0        0        0      528 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css
+-rw-r--r--   0        0        0    14151 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css.map
+-rw-r--r--   0        0        0     3487 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.css
+-rw-r--r--   0        0        0    35627 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.css.map
+-rw-r--r--   0        0        0     2669 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.min.css
+-rw-r--r--   0        0        0    34970 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.min.css.map
+-rw-r--r--   0        0        0     2953 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.min.css
+-rw-r--r--   0        0        0    37591 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.min.css.map
+-rw-r--r--   0        0        0     9842 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.js
+-rw-r--r--   0        0        0    24837 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.js.map
+-rw-r--r--   0        0        0     6081 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.min.js
+-rw-r--r--   0        0        0    19410 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.min.js.map
+-rw-r--r--   0        0        0    13564 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js
+-rw-r--r--   0        0        0    24406 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js.map
+-rw-r--r--   0        0        0     7638 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js
+-rw-r--r--   0        0        0    19511 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js.map
+-rw-r--r--   0        0        0     1420 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/README.md
+-rw-r--r--   0        0        0    10943 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.css
+-rw-r--r--   0        0        0    64082 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.css.map
+-rw-r--r--   0        0        0     3254 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css
+-rw-r--r--   0        0        0    33315 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css.map
+-rw-r--r--   0        0        0     2439 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css
+-rw-r--r--   0        0        0    33110 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css.map
+-rw-r--r--   0        0        0     7948 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.css
+-rw-r--r--   0        0        0    54402 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.css.map
+-rw-r--r--   0        0        0     6386 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css
+-rw-r--r--   0        0        0    53605 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css.map
+-rw-r--r--   0        0        0     8597 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.min.css
+-rw-r--r--   0        0        0    63083 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.min.css.map
+-rw-r--r--   0        0        0     4296 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.js
+-rw-r--r--   0        0        0    11212 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.js.map
+-rw-r--r--   0        0        0     2911 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js
+-rw-r--r--   0        0        0     9075 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js.map
+-rw-r--r--   0        0        0     6425 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js
+-rw-r--r--   0        0        0    11074 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js.map
+-rw-r--r--   0        0        0     3750 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js
+-rw-r--r--   0        0        0     9158 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js.map
+-rw-r--r--   0        0        0      774 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/README.md
+-rw-r--r--   0        0        0     3193 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.css
+-rw-r--r--   0        0        0    38972 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.css.map
+-rw-r--r--   0        0        0     1096 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.css
+-rw-r--r--   0        0        0    21520 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.css.map
+-rw-r--r--   0        0        0      870 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css
+-rw-r--r--   0        0        0    21507 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css.map
+-rw-r--r--   0        0        0     2338 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.css
+-rw-r--r--   0        0        0    34384 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.css.map
+-rw-r--r--   0        0        0     1892 2022-10-19 09:15:30.334833 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.min.css
+-rw-r--r--   0        0        0    33880 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.min.css.map
+-rw-r--r--   0        0        0     2534 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.min.css
+-rw-r--r--   0        0        0    38444 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.min.css.map
+-rw-r--r--   0        0        0      709 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/README.md
+-rw-r--r--   0        0        0    14519 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.css
+-rw-r--r--   0        0        0    70844 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.css.map
+-rw-r--r--   0        0        0     2837 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css
+-rw-r--r--   0        0        0    29987 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css.map
+-rw-r--r--   0        0        0     2259 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css
+-rw-r--r--   0        0        0    29890 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css.map
+-rw-r--r--   0        0        0    11941 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.css
+-rw-r--r--   0        0        0    62771 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.css.map
+-rw-r--r--   0        0        0     9783 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css
+-rw-r--r--   0        0        0    62033 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css.map
+-rw-r--r--   0        0        0    11814 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.min.css
+-rw-r--r--   0        0        0    70005 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.min.css.map
+-rw-r--r--   0        0        0      731 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/README.md
+-rw-r--r--   0        0        0     6491 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.css
+-rw-r--r--   0        0        0    44939 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.css.map
+-rw-r--r--   0        0        0     1930 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.css
+-rw-r--r--   0        0        0    20637 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.css.map
+-rw-r--r--   0        0        0     1481 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css
+-rw-r--r--   0        0        0    20530 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css.map
+-rw-r--r--   0        0        0     4801 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.css
+-rw-r--r--   0        0        0    37836 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.css.map
+-rw-r--r--   0        0        0     3971 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.min.css
+-rw-r--r--   0        0        0    37165 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.min.css.map
+-rw-r--r--   0        0        0     5224 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.min.css
+-rw-r--r--   0        0        0    44153 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.min.css.map
+-rw-r--r--   0        0        0      914 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/README.md
+-rw-r--r--   0        0        0    11535 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.css
+-rw-r--r--   0        0        0    51985 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.css.map
+-rw-r--r--   0        0        0     3317 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.css
+-rw-r--r--   0        0        0    27939 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.css.map
+-rw-r--r--   0        0        0     2483 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css
+-rw-r--r--   0        0        0    24727 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css.map
+-rw-r--r--   0        0        0     8536 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.css
+-rw-r--r--   0        0        0    45337 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.css.map
+-rw-r--r--   0        0        0     6356 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.min.css
+-rw-r--r--   0        0        0    41003 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.min.css.map
+-rw-r--r--   0        0        0     8611 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.min.css
+-rw-r--r--   0        0        0    47500 2022-10-19 09:15:30.338834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.min.css.map
+-rw-r--r--   0        0        0      979 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/README.md
+-rw-r--r--   0        0        0     3247 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.css
+-rw-r--r--   0        0        0    35926 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.css.map
+-rw-r--r--   0        0        0     1071 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.css
+-rw-r--r--   0        0        0    17968 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.css.map
+-rw-r--r--   0        0        0      778 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.min.css
+-rw-r--r--   0        0        0    17911 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.min.css.map
+-rw-r--r--   0        0        0     2465 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.css
+-rw-r--r--   0        0        0    32282 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.css.map
+-rw-r--r--   0        0        0     1726 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.min.css
+-rw-r--r--   0        0        0    31706 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.min.css.map
+-rw-r--r--   0        0        0     2276 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.min.css
+-rw-r--r--   0        0        0    35306 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.min.css.map
+-rw-r--r--   0        0        0      752 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/README.md
+-rw-r--r--   0        0        0     4577 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.css
+-rw-r--r--   0        0        0    32295 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.css.map
+-rw-r--r--   0        0        0     1876 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.css
+-rw-r--r--   0        0        0    19721 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.css.map
+-rw-r--r--   0        0        0     1276 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.min.css
+-rw-r--r--   0        0        0    19610 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.min.css.map
+-rw-r--r--   0        0        0     2980 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.css
+-rw-r--r--   0        0        0    27997 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.css.map
+-rw-r--r--   0        0        0     2363 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.min.css
+-rw-r--r--   0        0        0    27461 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.min.css.map
+-rw-r--r--   0        0        0     3411 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.min.css
+-rw-r--r--   0        0        0    31667 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.min.css.map
+-rw-r--r--   0        0        0      879 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/README.md
+-rw-r--r--   0        0        0    11034 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.css
+-rw-r--r--   0        0        0    61215 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.css.map
+-rw-r--r--   0        0        0     3247 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.css
+-rw-r--r--   0        0        0    24012 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.css.map
+-rw-r--r--   0        0        0     2667 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.min.css
+-rw-r--r--   0        0        0    23879 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.min.css.map
+-rw-r--r--   0        0        0     8028 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.css
+-rw-r--r--   0        0        0    52205 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.css.map
+-rw-r--r--   0        0        0     6353 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.min.css
+-rw-r--r--   0        0        0    51225 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.min.css.map
+-rw-r--r--   0        0        0     8792 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.min.css
+-rw-r--r--   0        0        0    60075 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.min.css.map
+-rw-r--r--   0        0        0     1152 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/README.md
+-rw-r--r--   0        0        0    10416 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css
+-rw-r--r--   0        0        0    60219 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css.map
+-rw-r--r--   0        0        0     2347 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css
+-rw-r--r--   0        0        0    29464 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css.map
+-rw-r--r--   0        0        0     1677 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css
+-rw-r--r--   0        0        0    29290 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css.map
+-rw-r--r--   0        0        0     8346 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css
+-rw-r--r--   0        0        0    53409 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css.map
+-rw-r--r--   0        0        0     5801 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css
+-rw-r--r--   0        0        0    52533 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css.map
+-rw-r--r--   0        0        0     7250 2022-10-19 09:15:30.342834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css
+-rw-r--r--   0        0        0    59189 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css.map
+-rw-r--r--   0        0        0      890 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js
+-rw-r--r--   0        0        0     2547 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js.map
+-rw-r--r--   0        0        0      605 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js
+-rw-r--r--   0        0        0     2200 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js.map
+-rw-r--r--   0        0        0     1514 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js
+-rw-r--r--   0        0        0     2503 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js.map
+-rw-r--r--   0        0        0      861 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js
+-rw-r--r--   0        0        0     2231 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js.map
+-rw-r--r--   0        0        0      846 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/README.md
+-rw-r--r--   0        0        0     1857 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.css
+-rw-r--r--   0        0        0    29655 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.css.map
+-rw-r--r--   0        0        0      556 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css
+-rw-r--r--   0        0        0    12744 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css.map
+-rw-r--r--   0        0        0      465 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css
+-rw-r--r--   0        0        0    12728 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css.map
+-rw-r--r--   0        0        0     1541 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css
+-rw-r--r--   0        0        0    27524 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css.map
+-rw-r--r--   0        0        0     1229 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css
+-rw-r--r--   0        0        0    27007 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css.map
+-rw-r--r--   0        0        0     1466 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css
+-rw-r--r--   0        0        0    29111 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css.map
+-rw-r--r--   0        0        0      694 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/README.md
+-rw-r--r--   0        0        0     4657 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.css
+-rw-r--r--   0        0        0    33046 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.css.map
+-rw-r--r--   0        0        0      910 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css
+-rw-r--r--   0        0        0    17346 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css.map
+-rw-r--r--   0        0        0      787 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css
+-rw-r--r--   0        0        0    17313 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css.map
+-rw-r--r--   0        0        0     3988 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.css
+-rw-r--r--   0        0        0    29547 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.css.map
+-rw-r--r--   0        0        0     3428 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css
+-rw-r--r--   0        0        0    28969 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css.map
+-rw-r--r--   0        0        0     3987 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.min.css
+-rw-r--r--   0        0        0    32425 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.min.css.map
+-rw-r--r--   0        0        0      707 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/README.md
+-rw-r--r--   0        0        0     1735 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.css
+-rw-r--r--   0        0        0    27099 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.css.map
+-rw-r--r--   0        0        0      535 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.css
+-rw-r--r--   0        0        0    13066 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.css.map
+-rw-r--r--   0        0        0      444 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css
+-rw-r--r--   0        0        0    12642 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css.map
+-rw-r--r--   0        0        0     1441 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.css
+-rw-r--r--   0        0        0    25608 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.css.map
+-rw-r--r--   0        0        0     1166 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.min.css
+-rw-r--r--   0        0        0    25100 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.min.css.map
+-rw-r--r--   0        0        0     1382 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.min.css
+-rw-r--r--   0        0        0    26554 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.min.css.map
+-rw-r--r--   0        0        0     1090 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/README.md
+-rw-r--r--   0        0        0     9125 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.css
+-rw-r--r--   0        0        0    60013 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.css.map
+-rw-r--r--   0        0        0     1578 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.css
+-rw-r--r--   0        0        0    24683 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.css.map
+-rw-r--r--   0        0        0     1169 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css
+-rw-r--r--   0        0        0    24150 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css.map
+-rw-r--r--   0        0        0     7820 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.css
+-rw-r--r--   0        0        0    55906 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.css.map
+-rw-r--r--   0        0        0     5810 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.min.css
+-rw-r--r--   0        0        0    55193 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.min.css.map
+-rw-r--r--   0        0        0     6751 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.min.css
+-rw-r--r--   0        0        0    58782 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.min.css.map
+-rw-r--r--   0        0        0     9505 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.js
+-rw-r--r--   0        0        0    22379 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.js.map
+-rw-r--r--   0        0        0     5322 2022-10-19 09:15:30.346834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.min.js
+-rw-r--r--   0        0        0    17344 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.min.js.map
+-rw-r--r--   0        0        0    13744 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js
+-rw-r--r--   0        0        0    22056 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js.map
+-rw-r--r--   0        0        0     7067 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js
+-rw-r--r--   0        0        0    17502 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js.map
+-rw-r--r--   0        0        0     1082 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/README.md
+-rw-r--r--   0        0        0    34105 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.css
+-rw-r--r--   0        0        0    84775 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.css.map
+-rw-r--r--   0        0        0    10190 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.css
+-rw-r--r--   0        0        0    36407 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.css.map
+-rw-r--r--   0        0        0     6960 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.min.css
+-rw-r--r--   0        0        0    35107 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.min.css.map
+-rw-r--r--   0        0        0    24733 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.css
+-rw-r--r--   0        0        0    62959 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.css.map
+-rw-r--r--   0        0        0    20075 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.min.css
+-rw-r--r--   0        0        0    60880 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.min.css.map
+-rw-r--r--   0        0        0    26807 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.min.css
+-rw-r--r--   0        0        0    82085 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.min.css.map
+-rw-r--r--   0        0        0     3810 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.js
+-rw-r--r--   0        0        0     9653 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.js.map
+-rw-r--r--   0        0        0     2347 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.min.js
+-rw-r--r--   0        0        0     7759 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.min.js.map
+-rw-r--r--   0        0        0     6032 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.js
+-rw-r--r--   0        0        0     9449 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.js.map
+-rw-r--r--   0        0        0     3266 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js
+-rw-r--r--   0        0        0     7834 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js.map
+-rw-r--r--   0        0        0     1112 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/README.md
+-rw-r--r--   0        0        0    49631 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.css
+-rw-r--r--   0        0        0   128464 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.css.map
+-rw-r--r--   0        0        0    26914 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.css
+-rw-r--r--   0        0        0    70083 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.css.map
+-rw-r--r--   0        0        0    23963 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css
+-rw-r--r--   0        0        0    69281 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css.map
+-rw-r--r--   0        0        0    23286 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.css
+-rw-r--r--   0        0        0    81303 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.css.map
+-rw-r--r--   0        0        0    21415 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.min.css
+-rw-r--r--   0        0        0    80360 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.min.css.map
+-rw-r--r--   0        0        0    44835 2022-10-19 09:15:30.350834 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.min.css
+-rw-r--r--   0        0        0   126711 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.min.css.map
+-rw-r--r--   0        0        0      527 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.js
+-rw-r--r--   0        0        0     1451 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.js.map
+-rw-r--r--   0        0        0      347 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.min.js
+-rw-r--r--   0        0        0     1245 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.min.js.map
+-rw-r--r--   0        0        0      594 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js
+-rw-r--r--   0        0        0     1445 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js.map
+-rw-r--r--   0        0        0      373 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js
+-rw-r--r--   0        0        0     1253 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js.map
+-rw-r--r--   0        0        0      795 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/README.md
+-rw-r--r--   0        0        0     5405 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.css
+-rw-r--r--   0        0        0    40961 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.css.map
+-rw-r--r--   0        0        0      773 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.css
+-rw-r--r--   0        0        0    16327 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.css.map
+-rw-r--r--   0        0        0      592 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css
+-rw-r--r--   0        0        0    16293 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css.map
+-rw-r--r--   0        0        0     4873 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.css
+-rw-r--r--   0        0        0    38586 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.css.map
+-rw-r--r--   0        0        0     3121 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.min.css
+-rw-r--r--   0        0        0    37848 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.min.css.map
+-rw-r--r--   0        0        0     3485 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.min.css
+-rw-r--r--   0        0        0    40175 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.min.css.map
+-rw-r--r--   0        0        0     1211 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/README.md
+-rw-r--r--   0        0        0     8764 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.css
+-rw-r--r--   0        0        0    49136 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.css.map
+-rw-r--r--   0        0        0     2374 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css
+-rw-r--r--   0        0        0    25598 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css.map
+-rw-r--r--   0        0        0     1967 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css
+-rw-r--r--   0        0        0    25484 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css.map
+-rw-r--r--   0        0        0     6665 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.css
+-rw-r--r--   0        0        0    42288 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.css.map
+-rw-r--r--   0        0        0     4992 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css
+-rw-r--r--   0        0        0    41598 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css.map
+-rw-r--r--   0        0        0     6731 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.min.css
+-rw-r--r--   0        0        0    48345 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.min.css.map
+-rw-r--r--   0        0        0     2013 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.js
+-rw-r--r--   0        0        0     5322 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.js.map
+-rw-r--r--   0        0        0     1347 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js
+-rw-r--r--   0        0        0     4353 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js.map
+-rw-r--r--   0        0        0     3763 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js
+-rw-r--r--   0        0        0     5211 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js.map
+-rw-r--r--   0        0        0     2056 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js
+-rw-r--r--   0        0        0     4432 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js.map
+-rw-r--r--   0        0        0     1412 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/README.md
+-rw-r--r--   0        0        0     4336 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.css
+-rw-r--r--   0        0        0    43755 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.css.map
+-rw-r--r--   0        0        0     1403 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.css
+-rw-r--r--   0        0        0    20488 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.css.map
+-rw-r--r--   0        0        0     1183 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css
+-rw-r--r--   0        0        0    20417 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css.map
+-rw-r--r--   0        0        0     3393 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.css
+-rw-r--r--   0        0        0    39559 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.css.map
+-rw-r--r--   0        0        0     2630 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.min.css
+-rw-r--r--   0        0        0    38882 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.min.css.map
+-rw-r--r--   0        0        0     3395 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.min.css
+-rw-r--r--   0        0        0    43023 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.min.css.map
+-rw-r--r--   0        0        0      548 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/README.md
+-rw-r--r--   0        0        0      875 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.css
+-rw-r--r--   0        0        0    11173 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.css.map
+-rw-r--r--   0        0        0      699 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.min.css
+-rw-r--r--   0        0        0    10753 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.min.css.map
+-rw-r--r--   0        0        0     2470 2022-10-19 09:15:30.354835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/README.md
+-rw-r--r--   0        0        0   195690 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.css
+-rw-r--r--   0        0        0   349835 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.css.map
+-rw-r--r--   0        0        0     4342 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.css
+-rw-r--r--   0        0        0    38238 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.css.map
+-rw-r--r--   0        0        0     3325 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.min.css
+-rw-r--r--   0        0        0    35852 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.min.css.map
+-rw-r--r--   0        0        0   191587 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.css
+-rw-r--r--   0        0        0   337455 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.css.map
+-rw-r--r--   0        0        0   158070 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.min.css
+-rw-r--r--   0        0        0   324803 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.min.css.map
+-rw-r--r--   0        0        0   161167 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.min.css
+-rw-r--r--   0        0        0   336524 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.min.css.map
+-rw-r--r--   0        0        0    58163 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.js
+-rw-r--r--   0        0        0   152953 2022-10-19 09:15:30.358835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.js.map
+-rw-r--r--   0        0        0    33997 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.min.js
+-rw-r--r--   0        0        0   114120 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.min.js.map
+-rw-r--r--   0        0        0    85987 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.js
+-rw-r--r--   0        0        0   149067 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.js.map
+-rw-r--r--   0        0        0    46071 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.min.js
+-rw-r--r--   0        0        0   114880 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.min.js.map
+-rw-r--r--   0        0        0      557 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/README.md
+-rw-r--r--   0        0        0   618733 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.css
+-rw-r--r--   0        0        0  1255933 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.css.map
+-rw-r--r--   0        0        0   112590 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css
+-rw-r--r--   0        0        0   334683 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css.map
+-rw-r--r--   0        0        0    88746 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css
+-rw-r--r--   0        0        0   320323 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css.map
+-rw-r--r--   0        0        0   508107 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.css
+-rw-r--r--   0        0        0   997920 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.css.map
+-rw-r--r--   0        0        0   418116 2022-10-19 09:15:30.378836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css
+-rw-r--r--   0        0        0   950122 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css.map
+-rw-r--r--   0        0        0   505976 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.min.css
+-rw-r--r--   0        0        0  1199654 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.min.css.map
+-rw-r--r--   0        0        0   102336 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.js
+-rw-r--r--   0        0        0   267371 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.js.map
+-rw-r--r--   0        0        0    62300 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js
+-rw-r--r--   0        0        0   201867 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js.map
+-rw-r--r--   0        0        0   165837 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js
+-rw-r--r--   0        0        0   299474 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js.map
+-rw-r--r--   0        0        0    95534 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0   233645 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js.map
+-rw-r--r--   0        0        0   617855 2022-10-19 09:15:30.362835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.css
+-rw-r--r--   0        0        0  1254712 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.css.map
+-rw-r--r--   0        0        0   112328 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.css
+-rw-r--r--   0        0        0   334251 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.css.map
+-rw-r--r--   0        0        0    88491 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.min.css
+-rw-r--r--   0        0        0   319895 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.min.css.map
+-rw-r--r--   0        0        0   507491 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.css
+-rw-r--r--   0        0        0   997129 2022-10-19 09:15:30.366835 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.css.map
+-rw-r--r--   0        0        0   417510 2022-10-19 09:15:30.370836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.min.css
+-rw-r--r--   0        0        0   949337 2022-10-19 09:15:30.370836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.min.css.map
+-rw-r--r--   0        0        0   505115 2022-10-19 09:15:30.370836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.min.css
+-rw-r--r--   0        0        0  1198443 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.min.css.map
+-rw-r--r--   0        0        0   102336 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.js
+-rw-r--r--   0        0        0   266969 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.js.map
+-rw-r--r--   0        0        0    62300 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.min.js
+-rw-r--r--   0        0        0   201465 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.min.js.map
+-rw-r--r--   0        0        0   165837 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.js
+-rw-r--r--   0        0        0   299054 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.js.map
+-rw-r--r--   0        0        0    95534 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0   233225 2022-10-19 09:15:30.374836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.min.js.map
+-rw-r--r--   0        0        0     3631 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     9190 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3448 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0     7406 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/favicon.ico
+-rw-r--r--   0        0        0     6360 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/favicon.svg
+-rw-r--r--   0        0        0      292 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/manifest.webmanifest
+-rwxr-xr-x   0        0        0    52216 2022-10-19 09:15:30.382836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff
+-rwxr-xr-x   0        0        0    42092 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2
+-rwxr-xr-x   0        0        0    56436 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff
+-rwxr-xr-x   0        0        0    45300 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2
+-rwxr-xr-x   0        0        0    50440 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff
+-rwxr-xr-x   0        0        0    41368 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2
+-rwxr-xr-x   0        0        0    54492 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff
+-rwxr-xr-x   0        0        0    43916 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2
+-rwxr-xr-x   0        0        0    51292 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff
+-rwxr-xr-x   0        0        0    41940 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2
+-rwxr-xr-x   0        0        0    54680 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff
+-rwxr-xr-x   0        0        0    44572 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2
+-rwxr-xr-x   0        0        0    51140 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff
+-rwxr-xr-x   0        0        0    41328 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2
+-rwxr-xr-x   0        0        0    54328 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff
+-rwxr-xr-x   0        0        0    44284 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2
+-rw-r--r--   0        0        0   114508 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff
+-rw-r--r--   0        0        0    80368 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2
+-rw-r--r--   0        0        0   114016 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff
+-rw-r--r--   0        0        0    79472 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2
+-rw-r--r--   0        0        0      397 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-fill.svg
+-rw-r--r--   0        0        0      789 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg
+-rw-r--r--   0        0        0      280 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-fill.svg
+-rw-r--r--   0        0        0      416 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/ancient-pavilion-line.svg
+-rw-r--r--   0        0        0      232 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/bank-fill.svg
+-rw-r--r--   0        0        0      262 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/bank-line.svg
+-rw-r--r--   0        0        0      204 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/building-fill.svg
+-rw-r--r--   0        0        0      225 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/building-line.svg
+-rw-r--r--   0        0        0      316 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/community-fill.svg
+-rw-r--r--   0        0        0      388 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/community-line.svg
+-rw-r--r--   0        0        0      232 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/government-fill.svg
+-rw-r--r--   0        0        0      227 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/government-line.svg
+-rw-r--r--   0        0        0      209 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/home-4-fill.svg
+-rw-r--r--   0        0        0      239 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/home-4-line.svg
+-rw-r--r--   0        0        0      212 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/hospital-fill.svg
+-rw-r--r--   0        0        0      228 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/hospital-line.svg
+-rw-r--r--   0        0        0      224 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/hotel-fill.svg
+-rw-r--r--   0        0        0      243 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/hotel-line.svg
+-rw-r--r--   0        0        0      437 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/store-fill.svg
+-rw-r--r--   0        0        0      546 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/store-line.svg
+-rw-r--r--   0        0        0      254 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/archive-fill.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/archive-line.svg
+-rw-r--r--   0        0        0      330 2022-10-19 09:15:30.386836 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/attachment-fill.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/attachment-line.svg
+-rw-r--r--   0        0        0      289 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/award-fill.svg
+-rw-r--r--   0        0        0      338 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/award-line.svg
+-rw-r--r--   0        0        0      218 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/bar-chart-box-fill.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/bar-chart-box-line.svg
+-rw-r--r--   0        0        0      208 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/bookmark-fill.svg
+-rw-r--r--   0        0        0      242 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/bookmark-line.svg
+-rw-r--r--   0        0        0      253 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/briefcase-fill.svg
+-rw-r--r--   0        0        0      267 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/briefcase-line.svg
+-rw-r--r--   0        0        0      248 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-2-fill.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-2-line.svg
+-rw-r--r--   0        0        0      218 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-event-fill.svg
+-rw-r--r--   0        0        0      251 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-event-line.svg
+-rw-r--r--   0        0        0      203 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-fill.svg
+-rw-r--r--   0        0        0      244 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/calendar-line.svg
+-rw-r--r--   0        0        0      254 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/cloud-fill.svg
+-rw-r--r--   0        0        0      356 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/cloud-line.svg
+-rw-r--r--   0        0        0      290 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/copyright-fill.svg
+-rw-r--r--   0        0        0      346 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/copyright-line.svg
+-rw-r--r--   0        0        0      341 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/customer-service-fill.svg
+-rw-r--r--   0        0        0      375 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/customer-service-line.svg
+-rw-r--r--   0        0        0      210 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/flag-fill.svg
+-rw-r--r--   0        0        0      255 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/flag-line.svg
+-rw-r--r--   0        0        0      540 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/global-fill.svg
+-rw-r--r--   0        0        0      607 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/global-line.svg
+-rw-r--r--   0        0        0      200 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/line-chart-fill.svg
+-rw-r--r--   0        0        0      218 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/line-chart-line.svg
+-rw-r--r--   0        0        0      409 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/links-fill.svg
+-rw-r--r--   0        0        0      418 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/links-line.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/mail-fill.svg
+-rw-r--r--   0        0        0      247 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/mail-line.svg
+-rw-r--r--   0        0        0      318 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/mail-open-fill.svg
+-rw-r--r--   0        0        0      359 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/mail-open-line.svg
+-rw-r--r--   0        0        0      355 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/medal-fill.svg
+-rw-r--r--   0        0        0      389 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/medal-line.svg
+-rw-r--r--   0        0        0      248 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/pie-chart-2-fill.svg
+-rw-r--r--   0        0        0      378 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/pie-chart-2-line.svg
+-rw-r--r--   0        0        0      273 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/pie-chart-box-fill.svg
+-rw-r--r--   0        0        0      289 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/pie-chart-box-line.svg
+-rw-r--r--   0        0        0      256 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/printer-fill.svg
+-rw-r--r--   0        0        0      341 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/printer-line.svg
+-rw-r--r--   0        0        0      296 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/profil-fill.svg
+-rw-r--r--   0        0        0      312 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/profil-line.svg
+-rw-r--r--   0        0        0      356 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/projector-2-fill.svg
+-rw-r--r--   0        0        0      350 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/projector-2-line.svg
+-rw-r--r--   0        0        0      248 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/send-plane-fill.svg
+-rw-r--r--   0        0        0      301 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/send-plane-line.svg
+-rw-r--r--   0        0        0      226 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/slideshow-fill.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/slideshow-line.svg
+-rw-r--r--   0        0        0      215 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/window-fill.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/window-line.svg
+-rw-r--r--   0        0        0      199 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-2-fill.svg
+-rw-r--r--   0        0        0      237 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-2-line.svg
+-rw-r--r--   0        0        0      236 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-3-fill.svg
+-rw-r--r--   0        0        0      360 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-3-line.svg
+-rw-r--r--   0        0        0      256 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-check-fill.svg
+-rw-r--r--   0        0        0      283 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-check-line.svg
+-rw-r--r--   0        0        0      321 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-delete-fill.svg
+-rw-r--r--   0        0        0      348 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-delete-line.svg
+-rw-r--r--   0        0        0      243 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-poll-fill.svg
+-rw-r--r--   0        0        0      214 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/chat-poll-line.svg
+-rw-r--r--   0        0        0      236 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/discuss-fill.svg
+-rw-r--r--   0        0        0      282 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/discuss-line.svg
+-rw-r--r--   0        0        0      201 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/feedback-fill.svg
+-rw-r--r--   0        0        0      229 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/feedback-line.svg
+-rw-r--r--   0        0        0      215 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/message-2-fill.svg
+-rw-r--r--   0        0        0      245 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/message-2-line.svg
+-rw-r--r--   0        0        0      231 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/question-answer-fill.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/question-answer-line.svg
+-rw-r--r--   0        0        0      263 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/questionnaire-fill.svg
+-rw-r--r--   0        0        0      327 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/questionnaire-line.svg
+-rw-r--r--   0        0        0      206 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/video-chat-fill.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/communication/video-chat-line.svg
+-rw-r--r--   0        0        0      318 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/ball-pen-fill.svg
+-rw-r--r--   0        0        0      372 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/ball-pen-line.svg
+-rw-r--r--   0        0        0      252 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/brush-3-fill.svg
+-rw-r--r--   0        0        0      266 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/brush-3-line.svg
+-rw-r--r--   0        0        0      449 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/brush-fill.svg
+-rw-r--r--   0        0        0      689 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/brush-line.svg
+-rw-r--r--   0        0        0      195 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/contrast-fill.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/contrast-line.svg
+-rw-r--r--   0        0        0      173 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/crop-fill.svg
+-rw-r--r--   0        0        0      184 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/crop-line.svg
+-rw-r--r--   0        0        0      399 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/drag-move-2-fill.svg
+-rw-r--r--   0        0        0      178 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/drag-move-2-line.svg
+-rw-r--r--   0        0        0      153 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/drop-fill.svg
+-rw-r--r--   0        0        0      190 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/drop-line.svg
+-rw-r--r--   0        0        0      275 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/edit-box-fill.svg
+-rw-r--r--   0        0        0      255 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/edit-box-line.svg
+-rw-r--r--   0        0        0      206 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/edit-fill.svg
+-rw-r--r--   0        0        0      258 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/edit-line.svg
+-rw-r--r--   0        0        0      266 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/ink-bottle-fill.svg
+-rw-r--r--   0        0        0      323 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/ink-bottle-line.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/layout-grid-fill.svg
+-rw-r--r--   0        0        0      232 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/layout-grid-line.svg
+-rw-r--r--   0        0        0      401 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/mark-pen-fill.svg
+-rw-r--r--   0        0        0      503 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/mark-pen-line.svg
+-rw-r--r--   0        0        0      292 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/paint-brush-fill.svg
+-rw-r--r--   0        0        0      305 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/paint-brush-line.svg
+-rw-r--r--   0        0        0      339 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/paint-fill.svg
+-rw-r--r--   0        0        0      362 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/paint-line.svg
+-rw-r--r--   0        0        0      437 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/palette-fill.svg
+-rw-r--r--   0        0        0      584 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/palette-line.svg
+-rw-r--r--   0        0        0      386 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pantone-fill.svg
+-rw-r--r--   0        0        0      505 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pantone-line.svg
+-rw-r--r--   0        0        0      389 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pen-nib-fill.svg
+-rw-r--r--   0        0        0      510 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pen-nib-line.svg
+-rw-r--r--   0        0        0      254 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pencil-fill.svg
+-rw-r--r--   0        0        0      310 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pencil-line.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pencil-ruler-fill.svg
+-rw-r--r--   0        0        0      255 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/pencil-ruler-line.svg
+-rw-r--r--   0        0        0      302 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/sip-fill.svg
+-rw-r--r--   0        0        0      352 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/sip-line.svg
+-rw-r--r--   0        0        0      221 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/table-fill.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/table-line.svg
+-rw-r--r--   0        0        0      500 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/bug-fill.svg
+-rw-r--r--   0        0        0      632 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/bug-line.svg
+-rw-r--r--   0        0        0      360 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/code-box-fill.svg
+-rw-r--r--   0        0        0      374 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/code-box-line.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/code-s-slash-line.svg
+-rw-r--r--   0        0        0      197 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/cursor-fill.svg
+-rw-r--r--   0        0        0      283 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/cursor-line.svg
+-rw-r--r--   0        0        0      307 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-branch-fill.svg
+-rw-r--r--   0        0        0      425 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-branch-line.svg
+-rw-r--r--   0        0        0      187 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-commit-fill.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-commit-line.svg
+-rw-r--r--   0        0        0      330 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-merge-fill.svg
+-rw-r--r--   0        0        0      455 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-merge-line.svg
+-rw-r--r--   0        0        0      233 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-pull-request-fill.svg
+-rw-r--r--   0        0        0      356 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-pull-request-line.svg
+-rw-r--r--   0        0        0      294 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-commits-fill.svg
+-rw-r--r--   0        0        0      320 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-commits-line.svg
+-rw-r--r--   0        0        0      285 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-fill.svg
+-rw-r--r--   0        0        0      328 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-line.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-private-fill.svg
+-rw-r--r--   0        0        0      304 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/git-repository-private-line.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/terminal-box-fill.svg
+-rw-r--r--   0        0        0      287 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/terminal-box-line.svg
+-rw-r--r--   0        0        0      186 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/terminal-line.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/terminal-window-fill.svg
+-rw-r--r--   0        0        0      245 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/terminal-window-line.svg
+-rw-r--r--   0        0        0      343 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/bluetooth-fill.svg
+-rw-r--r--   0        0        0      343 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/bluetooth-line.svg
+-rw-r--r--   0        0        0      256 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/computer-fill.svg
+-rw-r--r--   0        0        0      275 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/computer-line.svg
+-rw-r--r--   0        0        0      514 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg
+-rw-r--r--   0        0        0      552 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg
+-rw-r--r--   0        0        0      266 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/database-fill.svg
+-rw-r--r--   0        0        0      296 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/database-line.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/device-fill.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/device-line.svg
+-rw-r--r--   0        0        0      206 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/hard-drive-2-fill.svg
+-rw-r--r--   0        0        0      222 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/hard-drive-2-line.svg
+-rw-r--r--   0        0        0      290 2022-10-19 09:15:30.390837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/mac-fill.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/mac-line.svg
+-rw-r--r--   0        0        0      485 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/phone-fill.svg
+-rw-r--r--   0        0        0      719 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/phone-line.svg
+-rw-r--r--   0        0        0      272 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/qr-code-fill.svg
+-rw-r--r--   0        0        0      315 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/qr-code-line.svg
+-rw-r--r--   0        0        0      229 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/rss-fill.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/rss-line.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/save-3-fill.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/save-3-line.svg
+-rw-r--r--   0        0        0      195 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/save-fill.svg
+-rw-r--r--   0        0        0      219 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/save-line.svg
+-rw-r--r--   0        0        0      219 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/server-fill.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/server-line.svg
+-rw-r--r--   0        0        0      208 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/smartphone-fill.svg
+-rw-r--r--   0        0        0      224 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/smartphone-line.svg
+-rw-r--r--   0        0        0      208 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/tablet-fill.svg
+-rw-r--r--   0        0        0      224 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/tablet-line.svg
+-rw-r--r--   0        0        0      285 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/tv-fill.svg
+-rw-r--r--   0        0        0      304 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/tv-line.svg
+-rw-r--r--   0        0        0      618 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg
+-rw-r--r--   0        0        0      630 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/wifi-line.svg
+-rw-r--r--   0        0        0      233 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/article-fill.svg
+-rw-r--r--   0        0        0      249 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/article-line.svg
+-rw-r--r--   0        0        0      181 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/book-2-fill.svg
+-rw-r--r--   0        0        0      227 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/book-2-line.svg
+-rw-r--r--   0        0        0      226 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/booklet-fill.svg
+-rw-r--r--   0        0        0      242 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/booklet-line.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/clipboard-fill.svg
+-rw-r--r--   0        0        0      274 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/clipboard-line.svg
+-rw-r--r--   0        0        0      317 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/draft-fill.svg
+-rw-r--r--   0        0        0      303 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/draft-line.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-add-fill.svg
+-rw-r--r--   0        0        0      251 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-add-line.svg
+-rw-r--r--   0        0        0      227 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-download-fill.svg
+-rw-r--r--   0        0        0      245 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-download-line.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-fill.svg
+-rw-r--r--   0        0        0      225 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-line.svg
+-rw-r--r--   0        0        0      255 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-pdf-fill.svg
+-rw-r--r--   0        0        0      273 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-pdf-line.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-text-fill.svg
+-rw-r--r--   0        0        0      272 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/file-text-line.svg
+-rw-r--r--   0        0        0      198 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/folder-2-fill.svg
+-rw-r--r--   0        0        0      234 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/folder-2-line.svg
+-rw-r--r--   0        0        0      262 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/newspaper-fill.svg
+-rw-r--r--   0        0        0      290 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/newspaper-line.svg
+-rw-r--r--   0        0        0      292 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/survey-fill.svg
+-rw-r--r--   0        0        0      317 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/survey-line.svg
+-rw-r--r--   0        0        0      217 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/todo-fill.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/document/todo-line.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/code-view.svg
+-rw-r--r--   0        0        0      250 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/font-size.svg
+-rw-r--r--   0        0        0      314 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/fr--bold.svg
+-rw-r--r--   0        0        0      160 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/fr--highlight.svg
+-rw-r--r--   0        0        0      278 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/fr--quote-fill.svg
+-rw-r--r--   0        0        0      344 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/fr--quote-line.svg
+-rw-r--r--   0        0        0      223 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-1.svg
+-rw-r--r--   0        0        0      387 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-2.svg
+-rw-r--r--   0        0        0      542 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-3.svg
+-rw-r--r--   0        0        0      268 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-4.svg
+-rw-r--r--   0        0        0      393 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-5.svg
+-rw-r--r--   0        0        0      538 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-6.svg
+-rw-r--r--   0        0        0      298 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/hashtag.svg
+-rw-r--r--   0        0        0      158 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/italic.svg
+-rw-r--r--   0        0        0      468 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/link-unlink.svg
+-rw-r--r--   0        0        0      408 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/link.svg
+-rw-r--r--   0        0        0      246 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/list-ordered.svg
+-rw-r--r--   0        0        0      275 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/list-unordered.svg
+-rw-r--r--   0        0        0      341 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/question-mark.svg
+-rw-r--r--   0        0        0      147 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/separator.svg
+-rw-r--r--   0        0        0      151 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/space.svg
+-rw-r--r--   0        0        0      317 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/subscript.svg
+-rw-r--r--   0        0        0      315 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/superscript.svg
+-rw-r--r--   0        0        0      263 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/table-2.svg
+-rw-r--r--   0        0        0      505 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/translate-2.svg
+-rw-r--r--   0        0        0      206 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/bank-card-fill.svg
+-rw-r--r--   0        0        0      220 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/bank-card-line.svg
+-rw-r--r--   0        0        0      277 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/coin-fill.svg
+-rw-r--r--   0        0        0      393 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/gift-fill.svg
+-rw-r--r--   0        0        0      406 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/gift-line.svg
+-rw-r--r--   0        0        0      366 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/money-euro-box-fill.svg
+-rw-r--r--   0        0        0      344 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/money-euro-box-line.svg
+-rw-r--r--   0        0        0      365 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-fill.svg
+-rw-r--r--   0        0        0      362 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/money-euro-circle-line.svg
+-rw-r--r--   0        0        0      397 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/secure-payment-fill.svg
+-rw-r--r--   0        0        0      427 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/secure-payment-line.svg
+-rw-r--r--   0        0        0      348 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/shopping-bag-fill.svg
+-rw-r--r--   0        0        0      282 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/shopping-bag-line.svg
+-rw-r--r--   0        0        0      311 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-fill.svg
+-rw-r--r--   0        0        0      343 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/shopping-cart-2-line.svg
+-rw-r--r--   0        0        0      200 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/trophy-fill.svg
+-rw-r--r--   0        0        0      222 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/finance/trophy-line.svg
+-rw-r--r--   0        0        0      289 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/capsule-fill.svg
+-rw-r--r--   0        0        0      379 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/capsule-line.svg
+-rw-r--r--   0        0        0      336 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/dislike-fill.svg
+-rw-r--r--   0        0        0      543 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/dislike-line.svg
+-rw-r--r--   0        0        0      243 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/dossier-fill.svg
+-rw-r--r--   0        0        0      265 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/dossier-line.svg
+-rw-r--r--   0        0        0      269 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/first-aid-kit-fill.svg
+-rw-r--r--   0        0        0      283 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/first-aid-kit-line.svg
+-rw-r--r--   0        0        0      317 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-fill.svg
+-rw-r--r--   0        0        0      359 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/hand-sanitizer-line.svg
+-rw-r--r--   0        0        0      258 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/health-book-fill.svg
+-rw-r--r--   0        0        0      273 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/health-book-line.svg
+-rw-r--r--   0        0        0      209 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/heart-fill.svg
+-rw-r--r--   0        0        0      365 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/heart-line.svg
+-rw-r--r--   0        0        0      331 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/heart-pulse-fill.svg
+-rw-r--r--   0        0        0      661 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg
+-rw-r--r--   0        0        0      476 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/lungs-fill.svg
+-rw-r--r--   0        0        0      909 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/lungs-line.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/medicine-bottle-fill.svg
+-rw-r--r--   0        0        0      293 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/medicine-bottle-line.svg
+-rw-r--r--   0        0        0      395 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/mental-health-fill.svg
+-rw-r--r--   0        0        0      503 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/mental-health-line.svg
+-rw-r--r--   0        0        0      519 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg
+-rw-r--r--   0        0        0      618 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/microscope-line.svg
+-rw-r--r--   0        0        0      370 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/psychotherapy-fill.svg
+-rw-r--r--   0        0        0      504 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/psychotherapy-line.svg
+-rw-r--r--   0        0        0      181 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/pulse-line.svg
+-rw-r--r--   0        0        0      311 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/stethoscope-fill.svg
+-rw-r--r--   0        0        0      346 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/stethoscope-line.svg
+-rw-r--r--   0        0        0      446 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/surgical-mask-fill.svg
+-rw-r--r--   0        0        0      567 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg
+-rw-r--r--   0        0        0      466 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/syringe-fill.svg
+-rw-r--r--   0        0        0      486 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/syringe-line.svg
+-rw-r--r--   0        0        0      237 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/test-tube-fill.svg
+-rw-r--r--   0        0        0      264 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/test-tube-line.svg
+-rw-r--r--   0        0        0      484 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/thermometer-fill.svg
+-rw-r--r--   0        0        0      576 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg
+-rw-r--r--   0        0        0     1055 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/virus-fill.svg
+-rw-r--r--   0        0        0     1112 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/virus-line.svg
+-rw-r--r--   0        0        0      552 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg
+-rw-r--r--   0        0        0      594 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg
+-rw-r--r--   0        0        0      591 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg
+-rw-r--r--   0        0        0      411 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/edge-line.svg
+-rw-r--r--   0        0        0      368 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/facebook-circle-fill.svg
+-rw-r--r--   0        0        0      458 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/facebook-circle-line.svg
+-rw-r--r--   0        0        0      708 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg
+-rw-r--r--   0        0        0     1003 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg
+-rw-r--r--   0        0        0      685 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg
+-rw-r--r--   0        0        0      806 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg
+-rw-r--r--   0        0        0      561 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg
+-rw-r--r--   0        0        0      428 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-line.svg
+-rw-r--r--   0        0        0      790 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/github-fill.svg
+-rw-r--r--   0        0        0     1485 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/github-line.svg
+-rw-r--r--   0        0        0      530 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/google-fill.svg
+-rw-r--r--   0        0        0      371 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/google-line.svg
+-rw-r--r--   0        0        0      965 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg
+-rw-r--r--   0        0        0      796 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/ie-line.svg
+-rw-r--r--   0        0        0      917 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg
+-rw-r--r--   0        0        0     2014 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg
+-rw-r--r--   0        0        0      552 2022-10-19 09:15:30.394837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg
+-rw-r--r--   0        0        0      366 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/linkedin-box-line.svg
+-rw-r--r--   0        0        0      948 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg
+-rw-r--r--   0        0        0     1259 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg
+-rw-r--r--   0        0        0      202 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/npmjs-fill.svg
+-rw-r--r--   0        0        0      220 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/npmjs-line.svg
+-rw-r--r--   0        0        0      331 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/remixicon-fill.svg
+-rw-r--r--   0        0        0      391 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/remixicon-line.svg
+-rw-r--r--   0        0        0      972 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg
+-rw-r--r--   0        0        0      574 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/safari-line.svg
+-rw-r--r--   0        0        0     1133 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg
+-rw-r--r--   0        0        0      514 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/slack-line.svg
+-rw-r--r--   0        0        0     1494 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg
+-rw-r--r--   0        0        0     1848 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg
+-rw-r--r--   0        0        0      398 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/telegram-fill.svg
+-rw-r--r--   0        0        0      440 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/telegram-line.svg
+-rw-r--r--   0        0        0      332 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitch-fill.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitch-line.svg
+-rw-r--r--   0        0        0      586 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg
+-rw-r--r--   0        0        0      690 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg
+-rw-r--r--   0        0        0      726 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg
+-rw-r--r--   0        0        0     1001 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg
+-rw-r--r--   0        0        0      178 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vuejs-fill.svg
+-rw-r--r--   0        0        0      198 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vuejs-line.svg
+-rw-r--r--   0        0        0      418 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/youtube-fill.svg
+-rw-r--r--   0        0        0      899 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg
+-rw-r--r--   0        0        0      385 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/anchor-fill.svg
+-rw-r--r--   0        0        0      350 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/anchor-line.svg
+-rw-r--r--   0        0        0      359 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/bike-fill.svg
+-rw-r--r--   0        0        0      359 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/bike-line.svg
+-rw-r--r--   0        0        0      284 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/bus-fill.svg
+-rw-r--r--   0        0        0      299 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/bus-line.svg
+-rw-r--r--   0        0        0      372 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/car-fill.svg
+-rw-r--r--   0        0        0      387 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/car-line.svg
+-rw-r--r--   0        0        0      317 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/caravan-fill.svg
+-rw-r--r--   0        0        0      383 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/caravan-line.svg
+-rw-r--r--   0        0        0      253 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/charging-pile-2-fill.svg
+-rw-r--r--   0        0        0      265 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/charging-pile-2-line.svg
+-rw-r--r--   0        0        0      246 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/compass-3-fill.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/compass-3-line.svg
+-rw-r--r--   0        0        0      222 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/cup-fill.svg
+-rw-r--r--   0        0        0      264 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/cup-line.svg
+-rw-r--r--   0        0        0      945 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/earth-fill.svg
+-rw-r--r--   0        0        0      905 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/earth-line.svg
+-rw-r--r--   0        0        0     2305 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/france-fill.svg
+-rw-r--r--   0        0        0     4459 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/france-line.svg
+-rw-r--r--   0        0        0      303 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/gas-station-fill.svg
+-rw-r--r--   0        0        0      318 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/gas-station-line.svg
+-rw-r--r--   0        0        0      179 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/goblet-fill.svg
+-rw-r--r--   0        0        0      208 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/goblet-line.svg
+-rw-r--r--   0        0        0      214 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/map-pin-2-fill.svg
+-rw-r--r--   0        0        0      280 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/map-pin-2-line.svg
+-rw-r--r--   0        0        0      277 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/map-pin-user-fill.svg
+-rw-r--r--   0        0        0      363 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/map-pin-user-line.svg
+-rw-r--r--   0        0        0      378 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/motorbike-fill.svg
+-rw-r--r--   0        0        0      447 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/motorbike-line.svg
+-rw-r--r--   0        0        0      256 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/passport-fill.svg
+-rw-r--r--   0        0        0      272 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/passport-line.svg
+-rw-r--r--   0        0        0      221 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/restaurant-fill.svg
+-rw-r--r--   0        0        0      257 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/restaurant-line.svg
+-rw-r--r--   0        0        0      381 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/road-map-fill.svg
+-rw-r--r--   0        0        0      405 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/road-map-line.svg
+-rw-r--r--   0        0        0      278 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/sailboat-fill.svg
+-rw-r--r--   0        0        0      333 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/sailboat-line.svg
+-rw-r--r--   0        0        0      580 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg
+-rw-r--r--   0        0        0      562 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg
+-rw-r--r--   0        0        0      351 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/signal-tower-fill.svg
+-rw-r--r--   0        0        0      348 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/signal-tower-line.svg
+-rw-r--r--   0        0        0      271 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/suitcase-2-fill.svg
+-rw-r--r--   0        0        0      286 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/suitcase-2-line.svg
+-rw-r--r--   0        0        0      374 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/taxi-fill.svg
+-rw-r--r--   0        0        0      386 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/taxi-line.svg
+-rw-r--r--   0        0        0      251 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/train-fill.svg
+-rw-r--r--   0        0        0      293 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/train-line.svg
+-rw-r--r--   0        0        0      253 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/camera-fill.svg
+-rw-r--r--   0        0        0      311 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/camera-line.svg
+-rw-r--r--   0        0        0      294 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/clapperboard-fill.svg
+-rw-r--r--   0        0        0      312 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/clapperboard-line.svg
+-rw-r--r--   0        0        0      334 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/equalizer-fill.svg
+-rw-r--r--   0        0        0      505 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/equalizer-line.svg
+-rw-r--r--   0        0        0      340 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/film-fill.svg
+-rw-r--r--   0        0        0      355 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/film-line.svg
+-rw-r--r--   0        0        0      388 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/gallery-fill.svg
+-rw-r--r--   0        0        0      466 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/gallery-line.svg
+-rw-r--r--   0        0        0      261 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/headphone-fill.svg
+-rw-r--r--   0        0        0      300 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/headphone-line.svg
+-rw-r--r--   0        0        0      394 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-add-fill.svg
+-rw-r--r--   0        0        0      316 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-add-line.svg
+-rw-r--r--   0        0        0      398 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-edit-fill.svg
+-rw-r--r--   0        0        0      415 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-edit-line.svg
+-rw-r--r--   0        0        0      307 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-fill.svg
+-rw-r--r--   0        0        0      334 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/image-line.svg
+-rw-r--r--   0        0        0      394 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/live-fill.svg
+-rw-r--r--   0        0        0      408 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/live-line.svg
+-rw-r--r--   0        0        0      269 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/mic-fill.svg
+-rw-r--r--   0        0        0      320 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/mic-line.svg
+-rw-r--r--   0        0        0      158 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/music-2-fill.svg
+-rw-r--r--   0        0        0      226 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/music-2-line.svg
+-rw-r--r--   0        0        0      154 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/notification-3-fill.svg
+-rw-r--r--   0        0        0      208 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/notification-3-line.svg
+-rw-r--r--   0        0        0      201 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/pause-circle-fill.svg
+-rw-r--r--   0        0        0      236 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/pause-circle-line.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/play-circle-fill.svg
+-rw-r--r--   0        0        0      313 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/play-circle-line.svg
+-rw-r--r--   0        0        0      186 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/stop-circle-fill.svg
+-rw-r--r--   0        0        0      221 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/stop-circle-line.svg
+-rw-r--r--   0        0        0      160 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/transcription.svg
+-rw-r--r--   0        0        0      403 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-down-fill.svg
+-rw-r--r--   0        0        0      489 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-down-line.svg
+-rw-r--r--   0        0        0      407 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-mute-fill.svg
+-rw-r--r--   0        0        0      490 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-mute-line.svg
+-rw-r--r--   0        0        0      551 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg
+-rw-r--r--   0        0        0      630 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg
+-rw-r--r--   0        0        0      334 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/leaf-fill.svg
+-rw-r--r--   0        0        0      467 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/leaf-line.svg
+-rw-r--r--   0        0        0      253 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/lightbulb-fill.svg
+-rw-r--r--   0        0        0      406 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/lightbulb-line.svg
+-rw-r--r--   0        0        0      277 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/plant-fill.svg
+-rw-r--r--   0        0        0      362 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/plant-line.svg
+-rw-r--r--   0        0        0      573 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg
+-rw-r--r--   0        0        0      558 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/recycle-line.svg
+-rw-r--r--   0        0        0      454 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/scales-3-fill.svg
+-rw-r--r--   0        0        0      552 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg
+-rw-r--r--   0        0        0      258 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/seedling-fill.svg
+-rw-r--r--   0        0        0      326 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/seedling-line.svg
+-rw-r--r--   0        0        0      232 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/umbrella-fill.svg
+-rw-r--r--   0        0        0      315 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/umbrella-line.svg
+-rw-r--r--   0        0        0      209 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/add-circle-fill.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/add-circle-line.svg
+-rw-r--r--   0        0        0      136 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/add-line.svg
+-rw-r--r--   0        0        0      319 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/alarm-warning-fill.svg
+-rw-r--r--   0        0        0      360 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/alarm-warning-line.svg
+-rw-r--r--   0        0        0      224 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/alert-fill.svg
+-rw-r--r--   0        0        0      257 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/alert-line.svg
+-rw-r--r--   0        0        0      127 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-down-fill.svg
+-rw-r--r--   0        0        0      188 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-down-line.svg
+-rw-r--r--   0        0        0      120 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-down-s-fill.svg
+-rw-r--r--   0        0        0      173 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-down-s-line.svg
+-rw-r--r--   0        0        0      159 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-go-back-fill.svg
+-rw-r--r--   0        0        0      213 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-go-back-line.svg
+-rw-r--r--   0        0        0      161 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-fill.svg
+-rw-r--r--   0        0        0      218 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-go-forward-line.svg
+-rw-r--r--   0        0        0      128 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-left-fill.svg
+-rw-r--r--   0        0        0      184 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-left-line.svg
+-rw-r--r--   0        0        0      119 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-left-s-fill.svg
+-rw-r--r--   0        0        0      173 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-left-s-line.svg
+-rw-r--r--   0        0        0      128 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-right-fill.svg
+-rw-r--r--   0        0        0      189 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-right-line.svg
+-rw-r--r--   0        0        0      118 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-right-s-fill.svg
+-rw-r--r--   0        0        0      175 2022-10-19 09:15:30.398837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-right-s-line.svg
+-rw-r--r--   0        0        0      197 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-right-up-line.svg
+-rw-r--r--   0        0        0      129 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-up-fill.svg
+-rw-r--r--   0        0        0      186 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-up-line.svg
+-rw-r--r--   0        0        0      117 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-up-s-fill.svg
+-rw-r--r--   0        0        0      173 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/arrow-up-s-line.svg
+-rw-r--r--   0        0        0      177 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/check-line.svg
+-rw-r--r--   0        0        0      252 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/checkbox-circle-fill.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/checkbox-circle-line.svg
+-rw-r--r--   0        0        0      252 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/checkbox-fill.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/checkbox-line.svg
+-rw-r--r--   0        0        0      321 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/close-circle-fill.svg
+-rw-r--r--   0        0        0      342 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/close-circle-line.svg
+-rw-r--r--   0        0        0      210 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/close-line.svg
+-rw-r--r--   0        0        0      189 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/delete-bin-fill.svg
+-rw-r--r--   0        0        0      203 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/delete-bin-line.svg
+-rw-r--r--   0        0        0      142 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/download-fill.svg
+-rw-r--r--   0        0        0      198 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/download-line.svg
+-rw-r--r--   0        0        0      203 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/error-warning-fill.svg
+-rw-r--r--   0        0        0      238 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/error-warning-line.svg
+-rw-r--r--   0        0        0      228 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/external-link-fill.svg
+-rw-r--r--   0        0        0      230 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/external-link-line.svg
+-rw-r--r--   0        0        0      281 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/eye-fill.svg
+-rw-r--r--   0        0        0      380 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/eye-line.svg
+-rw-r--r--   0        0        0      481 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/eye-off-fill.svg
+-rw-r--r--   0        0        0      678 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg
+-rw-r--r--   0        0        0      136 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/filter-fill.svg
+-rw-r--r--   0        0        0      187 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/filter-line.svg
+-rw-r--r--   0        0        0      196 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-first-line.svg
+-rw-r--r--   0        0        0      197 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--arrow-left-s-line-double.svg
+-rw-r--r--   0        0        0      201 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-last-line.svg
+-rw-r--r--   0        0        0      201 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--arrow-right-s-line-double.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--error-fill.svg
+-rw-r--r--   0        0        0      309 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--error-line.svg
+-rw-r--r--   0        0        0      237 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--info-fill.svg
+-rw-r--r--   0        0        0      328 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--info-line.svg
+-rw-r--r--   0        0        0      253 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--success-fill.svg
+-rw-r--r--   0        0        0      289 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--success-line.svg
+-rw-r--r--   0        0        0      482 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--theme-fill.svg
+-rw-r--r--   0        0        0      225 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--warning-fill.svg
+-rw-r--r--   0        0        0      258 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/fr--warning-line.svg
+-rw-r--r--   0        0        0      205 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/information-fill.svg
+-rw-r--r--   0        0        0      239 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/information-line.svg
+-rw-r--r--   0        0        0      238 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/lock-fill.svg
+-rw-r--r--   0        0        0      252 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/lock-line.svg
+-rw-r--r--   0        0        0      252 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/lock-unlock-fill.svg
+-rw-r--r--   0        0        0      268 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/lock-unlock-line.svg
+-rw-r--r--   0        0        0      197 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/logout-box-r-fill.svg
+-rw-r--r--   0        0        0      219 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/logout-box-r-line.svg
+-rw-r--r--   0        0        0      145 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/menu-2-fill.svg
+-rw-r--r--   0        0        0      145 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/menu-fill.svg
+-rw-r--r--   0        0        0      248 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/more-fill.svg
+-rw-r--r--   0        0        0      348 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/more-line.svg
+-rw-r--r--   0        0        0      220 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/notification-badge-fill.svg
+-rw-r--r--   0        0        0      288 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/notification-badge-line.svg
+-rw-r--r--   0        0        0      311 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/question-fill.svg
+-rw-r--r--   0        0        0      325 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/question-line.svg
+-rw-r--r--   0        0        0      280 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/refresh-fill.svg
+-rw-r--r--   0        0        0      244 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/refresh-line.svg
+-rw-r--r--   0        0        0      247 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/search-fill.svg
+-rw-r--r--   0        0        0      382 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/search-line.svg
+-rw-r--r--   0        0        0      864 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg
+-rw-r--r--   0        0        0     1599 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg
+-rw-r--r--   0        0        0      241 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/shield-fill.svg
+-rw-r--r--   0        0        0      332 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/shield-line.svg
+-rw-r--r--   0        0        0      217 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/star-fill.svg
+-rw-r--r--   0        0        0      333 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/star-line.svg
+-rw-r--r--   0        0        0      203 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/star-s-fill.svg
+-rw-r--r--   0        0        0      325 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/star-s-line.svg
+-rw-r--r--   0        0        0      117 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/subtract-line.svg
+-rw-r--r--   0        0        0      341 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/thumb-down-fill.svg
+-rw-r--r--   0        0        0      442 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/thumb-down-line.svg
+-rw-r--r--   0        0        0      340 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/thumb-up-fill.svg
+-rw-r--r--   0        0        0      459 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/thumb-up-line.svg
+-rw-r--r--   0        0        0      193 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/time-fill.svg
+-rw-r--r--   0        0        0      226 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/time-line.svg
+-rw-r--r--   0        0        0      201 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/timer-fill.svg
+-rw-r--r--   0        0        0      236 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/timer-line.svg
+-rw-r--r--   0        0        0      180 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/upload-2-fill.svg
+-rw-r--r--   0        0        0      180 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/upload-2-line.svg
+-rw-r--r--   0        0        0      144 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/upload-fill.svg
+-rw-r--r--   0        0        0      206 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/upload-line.svg
+-rw-r--r--   0        0        0      279 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/zoom-in-fill.svg
+-rw-r--r--   0        0        0      407 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/zoom-in-line.svg
+-rw-r--r--   0        0        0      260 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/zoom-out-fill.svg
+-rw-r--r--   0        0        0      388 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/zoom-out-line.svg
+-rw-r--r--   0        0        0      337 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/account-circle-fill.svg
+-rw-r--r--   0        0        0      462 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/account-circle-line.svg
+-rw-r--r--   0        0        0      383 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/account-pin-circle-fill.svg
+-rw-r--r--   0        0        0      575 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg
+-rw-r--r--   0        0        0      279 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/admin-fill.svg
+-rw-r--r--   0        0        0      349 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/admin-line.svg
+-rw-r--r--   0        0        0      357 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/group-fill.svg
+-rw-r--r--   0        0        0      462 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/group-line.svg
+-rw-r--r--   0        0        0      279 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/parent-fill.svg
+-rw-r--r--   0        0        0      413 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/parent-line.svg
+-rw-r--r--   0        0        0      424 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/team-fill.svg
+-rw-r--r--   0        0        0      750 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/team-line.svg
+-rw-r--r--   0        0        0      235 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-add-fill.svg
+-rw-r--r--   0        0        0      316 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-add-line.svg
+-rw-r--r--   0        0        0      186 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-fill.svg
+-rw-r--r--   0        0        0      314 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-heart-fill.svg
+-rw-r--r--   0        0        0      439 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-heart-line.svg
+-rw-r--r--   0        0        0      275 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-line.svg
+-rw-r--r--   0        0        0      314 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-search-fill.svg
+-rw-r--r--   0        0        0      384 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-search-line.svg
+-rw-r--r--   0        0        0      529 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg
+-rw-r--r--   0        0        0      462 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-setting-line.svg
+-rw-r--r--   0        0        0      298 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-star-fill.svg
+-rw-r--r--   0        0        0      367 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-star-line.svg
+-rw-r--r--   0        0        0      167 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/cloudy-2-fill.svg
+-rw-r--r--   0        0        0      291 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/cloudy-2-line.svg
+-rw-r--r--   0        0        0      128 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/flashlight-fill.svg
+-rw-r--r--   0        0        0      172 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/flashlight-line.svg
+-rw-r--r--   0        0        0      226 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/moon-fill.svg
+-rw-r--r--   0        0        0      286 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/moon-line.svg
+-rw-r--r--   0        0        0      449 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/sun-fill.svg
+-rw-r--r--   0        0        0      482 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/weather/sun-line.svg
+-rw-r--r--   0        0        0      466 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/README.md
+-rw-r--r--   0        0        0    14496 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js
+-rw-r--r--   0        0        0    38322 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js.map
+-rw-r--r--   0        0        0    12899 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js
+-rw-r--r--   0        0        0    30524 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js.map
+-rw-r--r--   0        0        0      686 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/README.md
+-rw-r--r--   0        0        0      760 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/response/README.md
+-rw-r--r--   0        0        0      701 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/response/not-found/README.md
+-rw-r--r--   0        0        0       13 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/response/unavailable/README.md
+-rw-r--r--   0        0        0        9 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/pattern/README.md
+-rw-r--r--   0        0        0      855 2022-10-19 09:15:30.402837 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/README.md
+-rw-r--r--   0        0        0    13710 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.css
+-rw-r--r--   0        0        0    24571 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.css.map
+-rw-r--r--   0        0        0    12276 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.min.css
+-rw-r--r--   0        0        0    24181 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.min.css.map
+-rw-r--r--   0        0        0     4982 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.js
+-rw-r--r--   0        0        0    12753 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.js.map
+-rw-r--r--   0        0        0     3040 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.min.js
+-rw-r--r--   0        0        0    10020 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.min.js.map
+-rw-r--r--   0        0        0      836 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/README.md
+-rw-r--r--   0        0        0      421 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/README.md
+-rw-r--r--   0        0        0    66279 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.css
+-rw-r--r--   0        0        0   119166 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.css.map
+-rw-r--r--   0        0        0    32212 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css
+-rw-r--r--   0        0        0    76114 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css.map
+-rw-r--r--   0        0        0    26350 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css
+-rw-r--r--   0        0        0    74279 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css.map
+-rw-r--r--   0        0        0    34195 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.css
+-rw-r--r--   0        0        0    54325 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.css.map
+-rw-r--r--   0        0        0    30990 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css
+-rw-r--r--   0        0        0    53474 2022-10-19 09:15:30.406838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css.map
+-rw-r--r--   0        0        0    57212 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.min.css
+-rw-r--r--   0        0        0   116475 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.min.css.map
+-rw-r--r--   0        0        0      733 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/README.md
+-rw-r--r--   0        0        0      788 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md
+-rw-r--r--   0        0        0     8218 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css
+-rw-r--r--   0        0        0    18263 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css.map
+-rw-r--r--   0        0        0     3542 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css
+-rw-r--r--   0        0        0     8459 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css.map
+-rw-r--r--   0        0        0     3036 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css
+-rw-r--r--   0        0        0     8334 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
+-rw-r--r--   0        0        0     4916 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css
+-rw-r--r--   0        0        0    11989 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css.map
+-rw-r--r--   0        0        0     4370 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css
+-rw-r--r--   0        0        0    11318 2022-10-19 09:15:30.410838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css.map
+-rw-r--r--   0        0        0     7178 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css
+-rw-r--r--   0        0        0    17459 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css.map
+-rw-r--r--   0        0        0      782 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md
+-rw-r--r--   0        0        0    22912 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css
+-rw-r--r--   0        0        0    36317 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css.map
+-rw-r--r--   0        0        0     9504 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css
+-rw-r--r--   0        0        0    15677 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css.map
+-rw-r--r--   0        0        0     8088 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css
+-rw-r--r--   0        0        0    15303 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css.map
+-rw-r--r--   0        0        0    13648 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css
+-rw-r--r--   0        0        0    22781 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css.map
+-rw-r--r--   0        0        0    12243 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css
+-rw-r--r--   0        0        0    21812 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css.map
+-rw-r--r--   0        0        0    20103 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css
+-rw-r--r--   0        0        0    34966 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css.map
+-rw-r--r--   0        0        0      817 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md
+-rw-r--r--   0        0        0     8770 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css
+-rw-r--r--   0        0        0    18760 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css.map
+-rw-r--r--   0        0        0     3786 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css
+-rw-r--r--   0        0        0     8631 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css.map
+-rw-r--r--   0        0        0     3272 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css
+-rw-r--r--   0        0        0     8504 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css.map
+-rw-r--r--   0        0        0     5224 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css
+-rw-r--r--   0        0        0    12318 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css.map
+-rw-r--r--   0        0        0     4674 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css
+-rw-r--r--   0        0        0    11630 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css.map
+-rw-r--r--   0        0        0     7718 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css
+-rw-r--r--   0        0        0    17937 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css.map
+-rw-r--r--   0        0        0      768 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md
+-rw-r--r--   0        0        0    15237 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css
+-rw-r--r--   0        0        0    26962 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css.map
+-rw-r--r--   0        0        0     6494 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css
+-rw-r--r--   0        0        0    12046 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css.map
+-rw-r--r--   0        0        0     5504 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css
+-rw-r--r--   0        0        0    11789 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css.map
+-rw-r--r--   0        0        0     8983 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css
+-rw-r--r--   0        0        0    17098 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css.map
+-rw-r--r--   0        0        0     8000 2022-10-19 09:15:30.414838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css
+-rw-r--r--   0        0        0    16284 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css.map
+-rw-r--r--   0        0        0    13276 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css
+-rw-r--r--   0        0        0    25883 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css.map
+-rw-r--r--   0        0        0      803 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md
+-rw-r--r--   0        0        0    10584 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css
+-rw-r--r--   0        0        0    20874 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css.map
+-rw-r--r--   0        0        0     4556 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css
+-rw-r--r--   0        0        0     9515 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css.map
+-rw-r--r--   0        0        0     3954 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css
+-rw-r--r--   0        0        0     9364 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css.map
+-rw-r--r--   0        0        0     6268 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css
+-rw-r--r--   0        0        0    13546 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css.map
+-rw-r--r--   0        0        0     5638 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css
+-rw-r--r--   0        0        0    12836 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css.map
+-rw-r--r--   0        0        0     9364 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css
+-rw-r--r--   0        0        0    20005 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css.map
+-rw-r--r--   0        0        0      768 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md
+-rw-r--r--   0        0        0    13498 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css
+-rw-r--r--   0        0        0    24927 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css.map
+-rw-r--r--   0        0        0     5696 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css
+-rw-r--r--   0        0        0    11137 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css.map
+-rw-r--r--   0        0        0     4810 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css
+-rw-r--r--   0        0        0    10908 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css.map
+-rw-r--r--   0        0        0     8042 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css
+-rw-r--r--   0        0        0    15972 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css.map
+-rw-r--r--   0        0        0     7132 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css
+-rw-r--r--   0        0        0    15179 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css.map
+-rw-r--r--   0        0        0    11714 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css
+-rw-r--r--   0        0        0    23897 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css.map
+-rw-r--r--   0        0        0      782 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md
+-rw-r--r--   0        0        0    12044 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css
+-rw-r--r--   0        0        0    23019 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css.map
+-rw-r--r--   0        0        0     5060 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css
+-rw-r--r--   0        0        0    10329 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css.map
+-rw-r--r--   0        0        0     4306 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css
+-rw-r--r--   0        0        0    10136 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css.map
+-rw-r--r--   0        0        0     7224 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css
+-rw-r--r--   0        0        0    14874 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css.map
+-rw-r--r--   0        0        0     6434 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css
+-rw-r--r--   0        0        0    14117 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css.map
+-rw-r--r--   0        0        0    10512 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css
+-rw-r--r--   0        0        0    22061 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css.map
+-rw-r--r--   0        0        0      768 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md
+-rw-r--r--   0        0        0    10188 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css
+-rw-r--r--   0        0        0    21002 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css.map
+-rw-r--r--   0        0        0     4282 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css
+-rw-r--r--   0        0        0     9492 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css.map
+-rw-r--r--   0        0        0     3576 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css
+-rw-r--r--   0        0        0     9312 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css.map
+-rw-r--r--   0        0        0     6146 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css
+-rw-r--r--   0        0        0    13692 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css.map
+-rw-r--r--   0        0        0     5396 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css
+-rw-r--r--   0        0        0    12955 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css.map
+-rw-r--r--   0        0        0     8744 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css
+-rw-r--r--   0        0        0    20077 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css.map
+-rw-r--r--   0        0        0      775 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md
+-rw-r--r--   0        0        0     6775 2022-10-19 09:15:30.418838 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css
+-rw-r--r--   0        0        0    16356 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css.map
+-rw-r--r--   0        0        0     2988 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css
+-rw-r--r--   0        0        0     7682 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css.map
+-rw-r--r--   0        0        0     2584 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css
+-rw-r--r--   0        0        0     7585 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css.map
+-rw-r--r--   0        0        0     4027 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css
+-rw-r--r--   0        0        0    10857 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css.map
+-rw-r--r--   0        0        0     3577 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css
+-rw-r--r--   0        0        0    10222 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css.map
+-rw-r--r--   0        0        0     5933 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css
+-rw-r--r--   0        0        0    15616 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css.map
+-rw-r--r--   0        0        0      768 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md
+-rw-r--r--   0        0        0    14367 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css
+-rw-r--r--   0        0        0    25638 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css.map
+-rw-r--r--   0        0        0     6168 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css
+-rw-r--r--   0        0        0    11499 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css.map
+-rw-r--r--   0        0        0     5280 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css
+-rw-r--r--   0        0        0    11270 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css.map
+-rw-r--r--   0        0        0     8439 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css
+-rw-r--r--   0        0        0    16321 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css.map
+-rw-r--r--   0        0        0     7549 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css
+-rw-r--r--   0        0        0    15535 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css.map
+-rw-r--r--   0        0        0    12601 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css
+-rw-r--r--   0        0        0    24615 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css.map
+-rw-r--r--   0        0        0      754 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md
+-rw-r--r--   0        0        0    24122 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css
+-rw-r--r--   0        0        0    38266 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css.map
+-rw-r--r--   0        0        0     9746 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css
+-rw-r--r--   0        0        0    16193 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css.map
+-rw-r--r--   0        0        0     8200 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css
+-rw-r--r--   0        0        0    15782 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css.map
+-rw-r--r--   0        0        0    14616 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css
+-rw-r--r--   0        0        0    24170 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css.map
+-rw-r--r--   0        0        0    13026 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css
+-rw-r--r--   0        0        0    23145 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css.map
+-rw-r--r--   0        0        0    20998 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css
+-rw-r--r--   0        0        0    36822 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css.map
+-rw-r--r--   0        0        0      747 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md
+-rw-r--r--   0        0        0    17550 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css
+-rw-r--r--   0        0        0    29889 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css.map
+-rw-r--r--   0        0        0     7456 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css
+-rw-r--r--   0        0        0    13240 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css.map
+-rw-r--r--   0        0        0     6298 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css
+-rw-r--r--   0        0        0    12937 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css.map
+-rw-r--r--   0        0        0    10334 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css
+-rw-r--r--   0        0        0    18828 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css.map
+-rw-r--r--   0        0        0     9184 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css
+-rw-r--r--   0        0        0    17960 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css.map
+-rw-r--r--   0        0        0    15254 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css
+-rw-r--r--   0        0        0    28710 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css.map
+-rw-r--r--   0        0        0      761 2022-10-19 09:15:30.422839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md
+-rw-r--r--   0        0        0    18969 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css
+-rw-r--r--   0        0        0    31555 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css.map
+-rw-r--r--   0        0        0     7860 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css
+-rw-r--r--   0        0        0    13741 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css.map
+-rw-r--r--   0        0        0     6668 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css
+-rw-r--r--   0        0        0    13428 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css.map
+-rw-r--r--   0        0        0    11349 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css
+-rw-r--r--   0        0        0    19995 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css.map
+-rw-r--r--   0        0        0    10139 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css
+-rw-r--r--   0        0        0    19100 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css.map
+-rw-r--r--   0        0        0    16579 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css
+-rw-r--r--   0        0        0    30339 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css.map
+-rw-r--r--   0        0        0      767 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md
+-rw-r--r--   0        0        0     5250 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css
+-rw-r--r--   0        0        0    14596 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css.map
+-rw-r--r--   0        0        0     2350 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css
+-rw-r--r--   0        0        0     6956 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css.map
+-rw-r--r--   0        0        0     2012 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css
+-rw-r--r--   0        0        0     6877 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css.map
+-rw-r--r--   0        0        0     3140 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css
+-rw-r--r--   0        0        0     9822 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css.map
+-rw-r--r--   0        0        0     2750 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css
+-rw-r--r--   0        0        0     9211 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css.map
+-rw-r--r--   0        0        0     4534 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css
+-rw-r--r--   0        0        0    13898 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css.map
+-rw-r--r--   0        0        0      768 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md
+-rw-r--r--   0        0        0    59570 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css
+-rw-r--r--   0        0        0    82014 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css.map
+-rw-r--r--   0        0        0    23823 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css
+-rw-r--r--   0        0        0    33361 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css.map
+-rw-r--r--   0        0        0    20177 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css
+-rw-r--r--   0        0        0    32374 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css.map
+-rw-r--r--   0        0        0    35987 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css
+-rw-r--r--   0        0        0    50579 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css.map
+-rw-r--r--   0        0        0    32364 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css
+-rw-r--r--   0        0        0    48850 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css.map
+-rw-r--r--   0        0        0    52313 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css
+-rw-r--r--   0        0        0    79290 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css.map
+-rw-r--r--   0        0        0      754 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md
+-rw-r--r--   0        0        0    10694 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css
+-rw-r--r--   0        0        0    21341 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css.map
+-rw-r--r--   0        0        0     4602 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css
+-rw-r--r--   0        0        0     9747 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css.map
+-rw-r--r--   0        0        0     3920 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css
+-rw-r--r--   0        0        0     9574 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css.map
+-rw-r--r--   0        0        0     6332 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css
+-rw-r--r--   0        0        0    13774 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css.map
+-rw-r--r--   0        0        0     5622 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css
+-rw-r--r--   0        0        0    13057 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css.map
+-rw-r--r--   0        0        0     9314 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css
+-rw-r--r--   0        0        0    20443 2022-10-19 09:15:30.426839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css.map
+-rw-r--r--   0        0        0      775 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md
+-rw-r--r--   0        0        0     3858 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css
+-rw-r--r--   0        0        0    12976 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css.map
+-rw-r--r--   0        0        0     1726 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css
+-rw-r--r--   0        0        0     6293 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css.map
+-rw-r--r--   0        0        0     1484 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css
+-rw-r--r--   0        0        0     6240 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css.map
+-rw-r--r--   0        0        0     2372 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css
+-rw-r--r--   0        0        0     8866 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css.map
+-rw-r--r--   0        0        0     2062 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css
+-rw-r--r--   0        0        0     8280 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css.map
+-rw-r--r--   0        0        0     3318 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css
+-rw-r--r--   0        0        0    12329 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css.map
+-rw-r--r--   0        0        0   250598 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.css
+-rw-r--r--   0        0        0   337223 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.css.map
+-rw-r--r--   0        0        0   102435 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css
+-rw-r--r--   0        0        0   134791 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css.map
+-rw-r--r--   0        0        0    86377 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css
+-rw-r--r--   0        0        0   130362 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css.map
+-rw-r--r--   0        0        0   148403 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.css
+-rw-r--r--   0        0        0   202877 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.css.map
+-rw-r--r--   0        0        0   132072 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css
+-rw-r--r--   0        0        0   188914 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css.map
+-rw-r--r--   0        0        0   218221 2022-10-19 09:15:30.430839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.min.css
+-rw-r--r--   0        0        0   317317 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.min.css.map
+-rw-r--r--   0        0        0   310059 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.css
+-rw-r--r--   0        0        0   449720 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.css.map
+-rw-r--r--   0        0        0   132265 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.css
+-rw-r--r--   0        0        0   208183 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.css.map
+-rw-r--r--   0        0        0   110355 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.min.css
+-rw-r--r--   0        0        0   201910 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.min.css.map
+-rw-r--r--   0        0        0   178034 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.css
+-rw-r--r--   0        0        0   252994 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.css.map
+-rw-r--r--   0        0        0   158494 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.min.css
+-rw-r--r--   0        0        0   238156 2022-10-19 09:15:30.434839 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.min.css.map
+-rw-r--r--   0        0        0   268621 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.min.css
+-rw-r--r--   0        0        0   426746 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.min.css.map
+-rw-r--r--   0        0        0      527 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/django/forms/widgets/checkbox_option.html
+-rw-r--r--   0        0        0      394 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/django/forms/widgets/input_option.html
+-rw-r--r--   0        0        0      212 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/django/forms/widgets/multiple_input.html
+-rw-r--r--   0        0        0      386 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/accordion.html
+-rw-r--r--   0        0        0      138 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/accordion_group.html
+-rw-r--r--   0        0        0      699 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/alert.html
+-rw-r--r--   0        0        0      103 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/badge.html
+-rw-r--r--   0        0        0      147 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/badge_group.html
+-rw-r--r--   0        0        0      786 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/breadcrumb.html
+-rw-r--r--   0        0        0      240 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/button.html
+-rw-r--r--   0        0        0      575 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/callout.html
+-rw-r--r--   0        0        0     3745 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/card.html
+-rw-r--r--   0        0        0      451 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/favicon.html
+-rw-r--r--   0        0        0     2791 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/footer.html
+-rw-r--r--   0        0        0      364 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/checkbox_snippet.html
+-rw-r--r--   0        0        0      708 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html
+-rw-r--r--   0        0        0      357 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/field_snippet.html
+-rw-r--r--   0        0        0      835 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/input_snippet.html
+-rw-r--r--   0        0        0      100 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/form_snippet.html
+-rw-r--r--   0        0        0      289 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/global_css.html
+-rw-r--r--   0        0        0      188 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/global_js.html
+-rw-r--r--   0        0        0     3356 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/header.html
+-rw-r--r--   0        0        0      141 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/highlight.html
+-rw-r--r--   0        0        0      578 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/input.html
+-rw-r--r--   0        0        0      394 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/link.html
+-rw-r--r--   0        0        0     2564 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/pagination.html
+-rw-r--r--   0        0        0     1008 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/quote.html
+-rw-r--r--   0        0        0      968 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/select.html
+-rw-r--r--   0        0        0     3526 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/sidemenu.html
+-rw-r--r--   0        0        0      344 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/skiplinks.html
+-rw-r--r--   0        0        0      369 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/summary.html
+-rw-r--r--   0        0        0      683 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/table.html
+-rw-r--r--   0        0        0      681 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/tag.html
+-rw-r--r--   0        0        0     3422 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/theme_modale.html
+-rw-r--r--   0        0        0      407 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templates/dsfr/tile.html
+-rw-r--r--   0        0        0        0 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templatetags/__init__.py
+-rw-r--r--   0        0        0    23659 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/templatetags/dsfr_tags.py
+-rw-r--r--   0        0        0        0 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/test/__init__.py
+-rw-r--r--   0        0        0      909 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/test/test_config.py
+-rw-r--r--   0        0        0    26318 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/test/test_templatetags.py
+-rw-r--r--   0        0        0     1116 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/test/test_utils.py
+-rw-r--r--   0        0        0     3141 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/utils.py
+-rw-r--r--   0        0        0       63 2022-10-19 09:15:30.438840 django_dsfr-0.9.5/dsfr/views.py
+-rw-r--r--   0        0        0     1470 2022-10-19 09:15:30.442840 django_dsfr-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     8431 1970-01-01 00:00:00.000000 django_dsfr-0.9.5/setup.py
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 django_dsfr-0.9.5/PKG-INFO
```

### Comparing `django_dsfr-0.9.4/LICENSE` & `django_dsfr-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/README.rst` & `django_dsfr-0.9.5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ===========
 
 Django-DSFR is a Django app to integrate the `French government Design System ("Système de design de l’État français") <https://www.systeme-de-design.gouv.fr/>`_.
 
 
 This app was created as a part of `Open Collectivités <https://github.com/entrepreneur-interet-general/opencollectivites>`_ and is very much a work in progress. See the `documentation (in French) <https://entrepreneur-interet-general.github.io/django-dsfr/>`_ for details.
 
-Django-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://gouvfr.atlassian.net/wiki/spaces/DB/pages/978354177/Version+1.4>`_.
+Django-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://www.systeme-de-design.gouv.fr/a-propos/versions-du-dsfr/version-courante>`_.
 
 Requirements
 ------------
 Tested with Python 3.7 to 3.10 and Django 3.2.5 to 3.2.13. Per `vermin <https://github.com/netromdk/vermin>`_, it should work with Python >= 3.0, and it should work with old versions of Django too.
 
 Quick start
 -----------
```

### Comparing `django_dsfr-0.9.4/dsfr/admin.py` & `django_dsfr-0.9.5/dsfr/admin.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/migrations/0001_initial.py` & `django_dsfr-0.9.5/dsfr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/migrations/0002_auto_20211209_1557.py` & `django_dsfr-0.9.5/dsfr/migrations/0002_auto_20211209_1557.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py` & `django_dsfr-0.9.5/dsfr/migrations/0003_alter_dsfrconfig_accessibility_status.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/models.py` & `django_dsfr-0.9.5/dsfr/models.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/background/ovoid.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/background/ovoid.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/dark.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/dark.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/light.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/light.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/system.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/system.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/technical-error.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/technical-error.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/artwork/test.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/artwork/test.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/accordion/accordion.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/alert/alert.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/alert/alert.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/badge/badge.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/badge/badge.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/breadcrumb/breadcrumb.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/button/button.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/callout/callout.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/callout/callout.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/card/card.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/card/card.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/checkbox/checkbox.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/component.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/component.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/connect/connect.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/connect/connect.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/consent/consent.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/consent/consent.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/content/content.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/content/content.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/display/display.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/download/download.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/follow/follow.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/follow/follow.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/footer/footer.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/footer/footer.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/form/form.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/form/form.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/header/header.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/highlight/highlight.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/highlight/highlight.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/input/input.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/input/input.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/link/link.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/link/link.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/logo/logo.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/logo/logo.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/modal/modal.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/navigation/navigation.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/notice/notice.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/notice/notice.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/pagination/pagination.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/pagination/pagination.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/quote/quote.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/quote/quote.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/radio/radio.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/radio/radio.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/search/search.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/search/search.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/select/select.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/select/select.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/share/share.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/share/share.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/sidemenu/sidemenu.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/skiplink/skiplink.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/stepper/stepper.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/stepper/stepper.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/summary/summary.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/summary/summary.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tab/tab.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/table/table.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tag/tag.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/tile/tile.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/tile/tile.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/toggle/toggle.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/translate/translate.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/translate/translate.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/component/upload/upload.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/component/upload/upload.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/core/core.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/core/core.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr/dsfr.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/dsfr.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/dsfr.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/favicon.ico` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/favicon/favicon.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/favicon/favicon.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Bold_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Light_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Medium_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Marianne-Regular_Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/fonts/Spectral-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/ancient-gate-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/buildings/store-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/buildings/store-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/global-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/global-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/business/global-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/business/global-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/brush-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/brush-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/design/palette-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/design/palette-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/development/bug-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/development/bug-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/dashboard-3-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/dashboard-3-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/phone-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/phone-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/wifi-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/device/wifi-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/device/wifi-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-3.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-3.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/editor/h-6.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/editor/h-6.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/dislike-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/dislike-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/heart-pulse-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/lungs-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/lungs-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/microscope-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/microscope-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/microscope-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/surgical-mask-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/thermometer-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/virus-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/virus-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/health/virus-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/health/virus-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/chrome-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/chrome-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/edge-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/firefox-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/firefox-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--dailymotion-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/fr--tiktok-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/github-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/github-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/github-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/github-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/google-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/google-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/ie-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/ie-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/ie-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/instagram-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/instagram-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/linkedin-box-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/mastodon-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/mastodon-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/safari-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/safari-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/safari-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/slack-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/slack-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/slack-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/snapchat-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/snapchat-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitter-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/twitter-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vimeo-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/vimeo-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/logo/youtube-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/earth-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/earth-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/earth-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/earth-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/france-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/france-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/france-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/france-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/ship-2-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/map/ship-2-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-up-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/media/volume-up-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/recycle-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/recycle-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/recycle-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/others/scales-3-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/eye-off-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/settings-5-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/system/settings-5-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/account-pin-circle-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/team-line.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/team-line.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/icons/user/user-setting-fill.svg`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/legacy/legacy.nomodule.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/response/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/response/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/page/response/not-found/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/page/response/not-found/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.min.js` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.min.js`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/scheme/scheme.module.min.js.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/scheme/scheme.module.min.js.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/colors/colors.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/colors/colors.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-buildings/icons-buildings.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-business/icons-business.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-communication/icons-communication.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-design/icons-design.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-development/icons-development.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-device/icons-device.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-document/icons-document.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-editor/icons-editor.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-finance/icons-finance.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-health/icons-health.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-logo/icons-logo.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-map/icons-map.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-media/icons-media.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-others/icons-others.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-system/icons-system.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-user/icons-user.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/README.md`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons-weather/icons-weather.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/icons/icons.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/icons/icons.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.legacy.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.main.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.main.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.min.css` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.min.css`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/static/dsfr/dist/utility/utility.min.css.map` & `django_dsfr-0.9.5/dsfr/static/dsfr/dist/utility/utility.min.css.map`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/django/forms/widgets/checkbox_option.html` & `django_dsfr-0.9.5/dsfr/templates/django/forms/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/alert.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/alert.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/breadcrumb.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/callout.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/callout.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/card.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/card.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/footer.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/footer.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/checkboxselectmultiple_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/form_field_snippets/input_snippet.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/form_field_snippets/input_snippet.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/header.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/header.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/input.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/input.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/pagination.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/pagination.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/quote.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/quote.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/select.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/select.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/sidemenu.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/sidemenu.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/table.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/table.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/tag.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/tag.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templates/dsfr/theme_modale.html` & `django_dsfr-0.9.5/dsfr/templates/dsfr/theme_modale.html`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/templatetags/dsfr_tags.py` & `django_dsfr-0.9.5/dsfr/templatetags/dsfr_tags.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/test/test_config.py` & `django_dsfr-0.9.5/dsfr/test/test_config.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/test/test_templatetags.py` & `django_dsfr-0.9.5/dsfr/test/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/test/test_utils.py` & `django_dsfr-0.9.5/dsfr/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/dsfr/utils.py` & `django_dsfr-0.9.5/dsfr/utils.py`

 * *Files identical despite different names*

### Comparing `django_dsfr-0.9.4/pyproject.toml` & `django_dsfr-0.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Sylvain Boissel <sylvain.boissel@beta.gouv.fr>"]
 description = "Integrate the French government Design System into a Django app"
 license = "MIT"
 name = "django-dsfr"
-version = "0.9.4"
+version = "0.9.5"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Operating System :: OS Independent",
   "Intended Audience :: Developers",
```

### Comparing `django_dsfr-0.9.4/setup.py` & `django_dsfr-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
 install_requires = \
 ['Django>=3.2.5,<4.0.0',
  'django-widget-tweaks>=1.4.12,<2.0.0',
  'requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'django-dsfr',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Integrate the French government Design System into a Django app',
-    'long_description': '.. image:: https://badge.fury.io/py/django-dsfr.svg\n    :target: https://pypi.org/project/django-dsfr/\n\n.. image:: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/django.yml/badge.svg\n    :target: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/django.yml\n\n.. image:: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/codeql-analysis.yml/badge.svg\n    :target: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/codeql-analysis.yml\n\n\n===========\nDjango-DSFR\n===========\n\nDjango-DSFR is a Django app to integrate the `French government Design System ("Système de design de l’État français") <https://www.systeme-de-design.gouv.fr/>`_.\n\n\nThis app was created as a part of `Open Collectivités <https://github.com/entrepreneur-interet-general/opencollectivites>`_ and is very much a work in progress. See the `documentation (in French) <https://entrepreneur-interet-general.github.io/django-dsfr/>`_ for details.\n\nDjango-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://gouvfr.atlassian.net/wiki/spaces/DB/pages/978354177/Version+1.4>`_.\n\nRequirements\n------------\nTested with Python 3.7 to 3.10 and Django 3.2.5 to 3.2.13. Per `vermin <https://github.com/netromdk/vermin>`_, it should work with Python >= 3.0, and it should work with old versions of Django too.\n\nQuick start\n-----------\n\n1. Install with :code:`pip install django-dsfr`.\n\n2. Add "widget_tweaks" and "dsfr" to INSTALLED_APPS in your settings.py like this, before the app you want to use it with::\n\n    INSTALLED_APPS = [\n        ...\n        "widget_tweaks"\n        "dsfr",\n        <your_app>\n    ]\n\n3. Add the following info in the TEMPLATES section in your settings.py so that the choice forms work::\n\n    TEMPLATES = [\n        {        \n            [...]\n            "DIRS": [\n                os.path.join(BASE_DIR, "dsfr/templates"),\n                os.path.join(BASE_DIR, "templates"),\n            ],\n        },\n    ]\n\n4. Add the following FORM_RENDERER in settings.py so that the choice forms work::\n\n    FORM_RENDERER = "django.forms.renderers.TemplatesSetting"\n\n5. (Optional) Add the context processor to your settings.py and create an instance of "DsfrConfig" in the admin panel::\n\n    TEMPLATES = [\n        {\n            [...]\n            "OPTIONS": {\n                "context_processors": [\n                    [...]\n                    "dsfr.context_processors.site_config",\n                ],\n            },\n        },\n    ]\n\n6. Include the tags in your base.html file (see example file at https://github.com/entrepreneur-interet-general/django-dsfr/blob/main/example_app/templates/example_app/base.html)\n\n7. Start the development server and visit http://127.0.0.1:8000/',
+    'long_description': '.. image:: https://badge.fury.io/py/django-dsfr.svg\n    :target: https://pypi.org/project/django-dsfr/\n\n.. image:: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/django.yml/badge.svg\n    :target: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/django.yml\n\n.. image:: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/codeql-analysis.yml/badge.svg\n    :target: https://github.com/entrepreneur-interet-general/django-dsfr/actions/workflows/codeql-analysis.yml\n\n\n===========\nDjango-DSFR\n===========\n\nDjango-DSFR is a Django app to integrate the `French government Design System ("Système de design de l’État français") <https://www.systeme-de-design.gouv.fr/>`_.\n\n\nThis app was created as a part of `Open Collectivités <https://github.com/entrepreneur-interet-general/opencollectivites>`_ and is very much a work in progress. See the `documentation (in French) <https://entrepreneur-interet-general.github.io/django-dsfr/>`_ for details.\n\nDjango-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://www.systeme-de-design.gouv.fr/a-propos/versions-du-dsfr/version-courante>`_.\n\nRequirements\n------------\nTested with Python 3.7 to 3.10 and Django 3.2.5 to 3.2.13. Per `vermin <https://github.com/netromdk/vermin>`_, it should work with Python >= 3.0, and it should work with old versions of Django too.\n\nQuick start\n-----------\n\n1. Install with :code:`pip install django-dsfr`.\n\n2. Add "widget_tweaks" and "dsfr" to INSTALLED_APPS in your settings.py like this, before the app you want to use it with::\n\n    INSTALLED_APPS = [\n        ...\n        "widget_tweaks"\n        "dsfr",\n        <your_app>\n    ]\n\n3. Add the following info in the TEMPLATES section in your settings.py so that the choice forms work::\n\n    TEMPLATES = [\n        {        \n            [...]\n            "DIRS": [\n                os.path.join(BASE_DIR, "dsfr/templates"),\n                os.path.join(BASE_DIR, "templates"),\n            ],\n        },\n    ]\n\n4. Add the following FORM_RENDERER in settings.py so that the choice forms work::\n\n    FORM_RENDERER = "django.forms.renderers.TemplatesSetting"\n\n5. (Optional) Add the context processor to your settings.py and create an instance of "DsfrConfig" in the admin panel::\n\n    TEMPLATES = [\n        {\n            [...]\n            "OPTIONS": {\n                "context_processors": [\n                    [...]\n                    "dsfr.context_processors.site_config",\n                ],\n            },\n        },\n    ]\n\n6. Include the tags in your base.html file (see example file at https://github.com/entrepreneur-interet-general/django-dsfr/blob/main/example_app/templates/example_app/base.html)\n\n7. Start the development server and visit http://127.0.0.1:8000/',
     'author': 'Sylvain Boissel',
     'author_email': 'sylvain.boissel@beta.gouv.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/entrepreneur-interet-general/django-dsfr',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django_dsfr-0.9.4/PKG-INFO` & `django_dsfr-0.9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dsfr
-Version: 0.9.4
+Version: 0.9.5
 Summary: Integrate the French government Design System into a Django app
 Home-page: https://github.com/entrepreneur-interet-general/django-dsfr
 License: MIT
 Keywords: django
 Author: Sylvain Boissel
 Author-email: sylvain.boissel@beta.gouv.fr
 Requires-Python: >=3.8,<4.0
@@ -47,15 +47,15 @@
 ===========
 
 Django-DSFR is a Django app to integrate the `French government Design System ("Système de design de l’État français") <https://www.systeme-de-design.gouv.fr/>`_.
 
 
 This app was created as a part of `Open Collectivités <https://github.com/entrepreneur-interet-general/opencollectivites>`_ and is very much a work in progress. See the `documentation (in French) <https://entrepreneur-interet-general.github.io/django-dsfr/>`_ for details.
 
-Django-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://gouvfr.atlassian.net/wiki/spaces/DB/pages/978354177/Version+1.4>`_.
+Django-DSFR (partly) implements the `version 1.7.2 of the DSFR <https://www.systeme-de-design.gouv.fr/a-propos/versions-du-dsfr/version-courante>`_.
 
 Requirements
 ------------
 Tested with Python 3.7 to 3.10 and Django 3.2.5 to 3.2.13. Per `vermin <https://github.com/netromdk/vermin>`_, it should work with Python >= 3.0, and it should work with old versions of Django too.
 
 Quick start
 -----------
```

