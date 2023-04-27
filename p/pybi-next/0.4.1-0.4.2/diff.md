# Comparing `tmp/pybi-next-0.4.1.tar.gz` & `tmp/pybi-next-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybi-next-0.4.1.tar", last modified: Thu Apr 13 15:29:47 2023, max compression
+gzip compressed data, was "pybi-next-0.4.2.tar", last modified: Thu Apr 27 05:08:17 2023, max compression
```

## Comparing `pybi-next-0.4.1.tar` & `pybi-next-0.4.2.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.487250 pybi-next-0.4.1/
--rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      477 2023-04-13 15:29:47.475634 pybi-next-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.086263 pybi-next-0.4.1/pybi/
--rw-rw-rw-   0        0        0     1653 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/__index.py
--rw-rw-rw-   0        0        0       49 2023-04-13 15:29:16.000000 pybi-next-0.4.1/pybi/__init__.py
--rw-rw-rw-   0        0        0    18405 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.134252 pybi-next-0.4.1/pybi/core/
--rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.170912 pybi-next-0.4.1/pybi/core/components/
--rw-rw-rw-   0        0        0      631 2023-03-30 15:24:18.000000 pybi-next-0.4.1/pybi/core/components/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-03-29 14:36:39.000000 pybi-next-0.4.1/pybi/core/components/component.py
--rw-rw-rw-   0        0        0      532 2023-03-30 15:24:18.000000 pybi-next-0.4.1/pybi/core/components/componentTag.py
--rw-rw-rw-   0        0        0     7870 2023-04-11 12:28:53.000000 pybi-next-0.4.1/pybi/core/components/containerComponent.py
--rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.1/pybi/core/components/mermaid.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.213806 pybi-next-0.4.1/pybi/core/components/reactiveComponent/
--rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/base.py
--rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/echarts.py
--rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/input.py
--rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/markdown.py
--rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/numberSlider.py
--rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/slicer.py
--rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/table.py
--rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/textValue.py
--rw-rw-rw-   0        0        0     1008 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/components/staticComponent.py
--rw-rw-rw-   0        0        0     6135 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/dataSource.py
--rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.222782 pybi-next-0.4.1/pybi/core/styles/
--rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/__init__.py
--rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.1/pybi/core/styles/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.233752 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/
--rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/boxShadow.py
--rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textAlign.py
--rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textColor.py
--rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textSize.py
--rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.1/pybi/core/styles/utils.py
--rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/uiResource.py
--rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/webResources.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.248740 pybi-next-0.4.1/pybi/easyEcharts/
--rw-rw-rw-   0        0        0     2090 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/__init__.py
--rw-rw-rw-   0        0        0     3350 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/bar.py
--rw-rw-rw-   0        0        0     3592 2023-04-11 11:04:22.000000 pybi-next-0.4.1/pybi/easyEcharts/base.py
--rw-rw-rw-   0        0        0     3462 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/line.py
--rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/easyEcharts/map.py
--rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.1/pybi/easyEcharts/pie.py
--rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.1/pybi/easyEcharts/scatter.py
--rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.1/pybi/easyEcharts/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.253699 pybi-next-0.4.1/pybi/icons/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/__init__.py
--rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/iconManager.py
--rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/material_icons.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.414827 pybi-next-0.4.1/pybi/static/
--rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.1/pybi/static/echarts.min.js
--rw-rw-rw-   0        0        0      468 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/echartsCps-style.css
--rw-rw-rw-   0        0        0    27467 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/echartsCps.iife.js
--rw-rw-rw-   0        0        0   119709 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/elementCps-style.css
--rw-rw-rw-   0        0        0   349813 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/elementCps.iife.js
--rw-rw-rw-   0        0        0  2778154 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/mermaidCps.iife.js
--rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.1/pybi/static/province_map_full.json
--rw-rw-rw-   0        0        0     2000 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/sysApp-style.css
--rw-rw-rw-   0        0        0  1012054 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/sysApp.iife.js
--rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.1/pybi/static/vue.global.prod.min.js
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.416821 pybi-next-0.4.1/pybi/template/
--rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/template/index.html
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.434802 pybi-next-0.4.1/pybi/utils/
--rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.1/pybi/utils/dataSourceUtils.py
--rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.1/pybi/utils/data_gen.py
--rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.1/pybi/utils/dictUtils.py
--rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.1/pybi/utils/echarts_opts_utils.py
--rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/helper.py
--rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/markdown2.py
--rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/utils/pyecharts_utils.py
--rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/utils/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.473612 pybi-next-0.4.1/pybi_next.egg-info/
--rw-rw-rw-   0        0        0      477 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2201 2023-04-13 15:29:46.000000 pybi-next-0.4.1/pybi_next.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.1/pybi_next.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 15:29:47.488067 pybi-next-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.284434 pybi-next-0.4.2/
+-rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      477 2023-04-27 05:08:17.283460 pybi-next-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.136453 pybi-next-0.4.2/pybi/
+-rw-rw-rw-   0        0        0     1686 2023-04-18 11:27:51.000000 pybi-next-0.4.2/pybi/__index.py
+-rw-rw-rw-   0        0        0       49 2023-04-27 05:06:31.000000 pybi-next-0.4.2/pybi/__init__.py
+-rw-rw-rw-   0        0        0    21545 2023-04-27 04:52:34.000000 pybi-next-0.4.2/pybi/app.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.146426 pybi-next-0.4.2/pybi/core/
+-rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.157398 pybi-next-0.4.2/pybi/core/components/
+-rw-rw-rw-   0        0        0      630 2023-04-18 11:30:38.000000 pybi-next-0.4.2/pybi/core/components/__init__.py
+-rw-rw-rw-   0        0        0     2675 2023-04-16 15:41:13.000000 pybi-next-0.4.2/pybi/core/components/component.py
+-rw-rw-rw-   0        0        0      553 2023-04-16 15:41:13.000000 pybi-next-0.4.2/pybi/core/components/componentTag.py
+-rw-rw-rw-   0        0        0     9911 2023-04-25 06:43:08.000000 pybi-next-0.4.2/pybi/core/components/containerComponent.py
+-rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.2/pybi/core/components/mermaid.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.175350 pybi-next-0.4.2/pybi/core/components/reactiveComponent/
+-rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/base.py
+-rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/echarts.py
+-rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/input.py
+-rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/markdown.py
+-rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/numberSlider.py
+-rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/slicer.py
+-rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/table.py
+-rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/core/components/reactiveComponent/textValue.py
+-rw-rw-rw-   0        0        0     1882 2023-04-16 15:41:13.000000 pybi-next-0.4.2/pybi/core/components/staticComponent.py
+-rw-rw-rw-   0        0        0     6135 2023-04-21 15:56:29.000000 pybi-next-0.4.2/pybi/core/dataSource.py
+-rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/core/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.182554 pybi-next-0.4.2/pybi/core/styles/
+-rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.2/pybi/core/styles/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-17 04:53:14.000000 pybi-next-0.4.2/pybi/core/styles/styleTag.py
+-rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.2/pybi/core/styles/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.191533 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/
+-rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/boxShadow.py
+-rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textAlign.py
+-rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textColor.py
+-rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textSize.py
+-rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.2/pybi/core/styles/utils.py
+-rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/core/uiResource.py
+-rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/core/webResources.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.211480 pybi-next-0.4.2/pybi/easyEcharts/
+-rw-rw-rw-   0        0        0     3756 2023-04-15 13:47:38.000000 pybi-next-0.4.2/pybi/easyEcharts/__init__.py
+-rw-rw-rw-   0        0        0     3350 2023-04-13 15:22:20.000000 pybi-next-0.4.2/pybi/easyEcharts/bar.py
+-rw-rw-rw-   0        0        0     3503 2023-04-15 13:47:38.000000 pybi-next-0.4.2/pybi/easyEcharts/base.py
+-rw-rw-rw-   0        0        0     2686 2023-04-15 13:47:38.000000 pybi-next-0.4.2/pybi/easyEcharts/candlestick.py
+-rw-rw-rw-   0        0        0     3462 2023-04-13 15:22:20.000000 pybi-next-0.4.2/pybi/easyEcharts/line.py
+-rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/easyEcharts/map.py
+-rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.2/pybi/easyEcharts/pie.py
+-rw-rw-rw-   0        0        0     2766 2023-04-15 13:47:38.000000 pybi-next-0.4.2/pybi/easyEcharts/radar.py
+-rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.2/pybi/easyEcharts/scatter.py
+-rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.2/pybi/easyEcharts/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.217464 pybi-next-0.4.2/pybi/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/icons/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/icons/iconManager.py
+-rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/icons/material_icons.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.251373 pybi-next-0.4.2/pybi/static/
+-rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.2/pybi/static/echarts.min.js
+-rw-rw-rw-   0        0        0      479 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/echartsCps-style.css
+-rw-rw-rw-   0        0        0    27649 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/echartsCps.iife.js
+-rw-rw-rw-   0        0        0   119843 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/elementCps-style.css
+-rw-rw-rw-   0        0        0   349858 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/elementCps.iife.js
+-rw-rw-rw-   0        0        0  2778154 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/mermaidCps.iife.js
+-rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.2/pybi/static/province_map_full.json
+-rw-rw-rw-   0        0        0     2141 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/sysApp-style.css
+-rw-rw-rw-   0        0        0  1012891 2023-04-27 04:46:28.000000 pybi-next-0.4.2/pybi/static/sysApp.iife.js
+-rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.2/pybi/static/vue.global.prod.min.js
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.253368 pybi-next-0.4.2/pybi/template/
+-rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.2/pybi/template/index.html
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.270472 pybi-next-0.4.2/pybi/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.2/pybi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.2/pybi/utils/dataSourceUtils.py
+-rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.2/pybi/utils/data_gen.py
+-rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.2/pybi/utils/dictUtils.py
+-rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.2/pybi/utils/echarts_opts_utils.py
+-rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.2/pybi/utils/helper.py
+-rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.2/pybi/utils/markdown2.py
+-rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/utils/pyecharts_utils.py
+-rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.2/pybi/utils/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:08:17.281442 pybi-next-0.4.2/pybi_next.egg-info/
+-rw-rw-rw-   0        0        0      477 2023-04-27 05:08:15.000000 pybi-next-0.4.2/pybi_next.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2288 2023-04-27 05:08:16.000000 pybi-next-0.4.2/pybi_next.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:08:15.000000 pybi-next-0.4.2/pybi_next.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.2/pybi_next.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-27 05:08:15.000000 pybi-next-0.4.2/pybi_next.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 05:08:15.000000 pybi-next-0.4.2/pybi_next.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:08:17.284434 pybi-next-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.2/setup.py
```

### Comparing `pybi-next-0.4.1/LICENSE` & `pybi-next-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/README.md` & `pybi-next-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/__index.py` & `pybi-next-0.4.2/pybi/__index.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "add_icon",
     "affix",
     "add_mermaid",
     "add_input",
     "add_numberSlider",
     # "add_svg_icon",
     "md_icons",
+    "space",
 ]
 
 add_tabs = app.add_tabs
 meta = app.meta
 gridBox = app.gridBox
 set_source = app.set_source
 add_upload = app.add_upload
@@ -71,7 +72,8 @@
 add_markdown = app.add_markdown
 add_icon = app.add_icon
 # add_svg_icon = app.add_svg_icon
 affix = app.affix
 add_mermaid = app.add_mermaid
 add_input = app.add_input
 add_numberSlider = app.add_numberSlider
+space = app.space
```

### Comparing `pybi-next-0.4.1/pybi/app.py` & `pybi-next-0.4.2/pybi/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import pandas as pd
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 import os
 
 from pybi.core.components import (
     ContainerComponent,
-    ColBoxComponent,
     ComponentTag,
     BoxComponent,
     FlowBoxComponent,
     TextComponent,
     UploadComponent,
     GridBoxComponent,
     TabsComponent,
     Markdown,
     IconComponent,
     SvgIconComponent,
     AffixComponent,
     Mermaid,
     Input,
     NumberSlider,
+    SpaceComponent,
 )
 from pybi.core.components.reactiveComponent import EChart, Slicer, Table, TextValue
 from pybi.core.dataSource import (
     DataSourceField,
     DataSourceTable,
     DataView,
     DataViewBase,
@@ -52,14 +52,15 @@
     EChartDatasetInfo,
     EChartJscode,
     OptionsExtractor,
 )
 import pybi.utils.pyecharts_utils as pyecharts_utils
 from pybi.icons.iconManager import get_singleton as get_iconManager
 from pybi.core.webResources import WebResourceManager
+from pybi.core.styles.styleTag import StyleTagInfo
 import pybi as pbi
 
 if TYPE_CHECKING:
     pass
     # from pybi.core.components import ReactiveComponent
 
 
@@ -82,33 +83,40 @@
         self.__app.echartsRenderer = renderer
         return self
 
     def set_doc_title(self, title: str):
         self.__app._doc_title = title
         return self
 
+    def add_style_tag(
+        self, css: str, id: Optional[str] = None, media: Optional[str] = None
+    ):
+        self.__app._style_tags.append(StyleTagInfo(css, id, media))
+        return self
+
 
 class App(ContainerComponent):
     def __init__(self) -> None:
         super().__init__(ComponentTag.App)
         self.dataSources: List[DataSource] = []
         self.dataViews: List[DataViewBase] = []
         self.__dataSetNames = set()
         self._with_temp_host_stack: List[ContainerComponent] = []
         self._clear_data = False
         self.dbLocalStorage = False
         self.echartsRenderer = "canvas"
-        self._doc_title = None
+        self._doc_title: Optional[str] = None
         self.__meta = AppMeta(self)
         self.__json_utils = JsonUtils()
         self.__resourceManager = ResourceManager()
         self._iconManager = get_iconManager()
 
         self.__webResourceManager = WebResourceManager()
         self.webResources = []
+        self._style_tags: List[StyleTagInfo] = []
 
     def __record_and_check_dataset_name(self, name: str):
         if name in self.__dataSetNames:
             raise Exception(f"dataset name '{name}' is duplicate")
         self.__dataSetNames.add(name)
 
     @property
@@ -332,59 +340,137 @@
         host._add_children(cp)
 
         self.__resourceManager.register_echarts()
         return cp
 
     def flowBox(
         self,
+        align: Optional[str] = None,
         *,
         host: Optional[ContainerComponent] = None,
     ):
-        cp = FlowBoxComponent(self)
+        """行容器，里面的组件会横向放置，在超过屏幕宽度时，自动换行
+
+        Args:
+            align (Optional[str], optional): 容器中的元素组件靠向哪个位置。'left' | 'center' | 'right' | 'between' | 'around' |'evenly' |'stretch'. Defaults to None('left').
+
+                - left : 从行首起始位置开始排列
+                - center:居中排列
+                - right:从行尾位置开始排列
+                - between: 均匀排列每个元素,首个元素放置于起点，末尾元素放置于终点
+                - around:  均匀排列每个元素,每个元素周围分配相同的空间
+                - evenly:  均匀排列每个元素, 每个元素之间的间隔相等
+
+        ## 示例
+
+        >>> # 2个文本放置在同一行，并且靠左放置
+        >>> with pbi.flowBox():
+                pbi.add_text('text A')
+                pbi.add_text('text B')
+
+        >>> # 2个文本放置在同一行，并且居中放置
+        >>> with pbi.flowBox('center'):
+                pbi.add_text('text A')
+                pbi.add_text('text B')
+        """
+        cp = FlowBoxComponent(align=align, appHost=self)
 
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
         return cp
 
     def gridBox(
         self,
         areas: Union[List[List[str]], str],
         *,
         host: Optional[ContainerComponent] = None,
     ):
+        """网格布局
+
+        Args:
+            areas (Union[List[List[str]], str]): 网格布局文本
+        ---
+        ### 示例
+        ```python
+        grid='''
+            a b c
+            a e .
+        '''
+
+        with pbi.gridBox(grid):
+            pbi.add_slicer(...).set_gridArea('a')
+            pbi.add_slicer(...).set_gridArea('b')
+        ```
+
+
+        当 `areas` 设置为 '' 时,默认为动态布局，每行放置3格
+        ```python
+        with pbi.gridBox(''):
+            # 3个切片器在第1行
+            pbi.add_slicer(...)
+            pbi.add_slicer(...)
+            pbi.add_slicer(...)
+
+            # 2个切片器在第2行
+            pbi.add_slicer(...)
+            pbi.add_slicer(...)
+        ```
+
+        可以通过 `auto_fill_fixed_num` 修改动态配置
+
+        >>> with pbi.gridBox('').auto_fill_fixed_num(2):
+                ...
+
+        """
         if isinstance(areas, str):
             areas = GridBoxComponent.areas_str2array(areas)
 
         cp = GridBoxComponent(areas, self)
 
+        if len(areas) == 0:
+            cp.auto_fill_fixed_num()
+
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
         return cp
 
     def colBox(
         self,
         spec: List[int] | None = None,
         *,
         host: Optional[ContainerComponent] = None,
     ):
-        cp = ColBoxComponent(spec, self)
-
-        host = host or self._get_temp_host() or self
-        host._add_children(cp)
+        spec = spec or [1, 1]
+        grid_text = " ".join(f"x{n}" for n in range(len(spec)))
+        cp = self.gridBox(grid_text).set_columns_sizes(spec)
 
         return cp
 
     def box(
         self,
+        align: Optional[str] = None,
         *,
         host: Optional[ContainerComponent] = None,
     ):
-        cp = BoxComponent(self)
+        """盒容器，里面的组件会竖向放置
+
+        Args:
+            align (Optional[str], optional): 容器中的元素组件靠向哪个位置。
+                'left' | 'center' | 'right' | 'between' | 'around' |'evenly'|'stretch'. Defaults to None('top').
+
+                - left : 从行首起始位置开始排列
+                - center:居中排列
+                - right:从行尾位置开始排列
+
+        ## 示例
+
+        """
+        cp = BoxComponent(align=align, appHost=self)
         host = host or self._get_temp_host() or self
         host._add_children(cp)
         return cp
 
     def add_tabs(
         self,
         names: List[str],
@@ -416,50 +502,25 @@
                 "input": ds2sqlite_file_base64(
                     self.dataSources, clear_data=self._clear_data
                 ),
                 "actionPipe": [],
             }
         )
 
-        # self.webResources.append(
-        #     {
-        #         "id": "maps1",
-        #         "type": "echarts-map",
-        #         "input": ds2sqlite_file_base64(
-        #             self.dataSources, clear_data=self._clear_data
-        #         ),
-        #         "actionPipe": [],
-        #     }
-        # )
-
-        # self.webResources.append(
-        #     {
-        #         "id": "maps1",
-        #         "type": "echarts-map",
-        #         "input": None,
-        #         "actionPipe": [
-        #             {
-        #                 "name": "fetch",
-        #                 "args": {
-        #                     "url": "https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json",
-        #                     "options": {},
-        #                 },
-        #             }
-        #         ],
-        #     }
-        # )
-
         wrs = self.__webResourceManager.create_webResources()
         self.webResources.extend(wrs)
 
         data = super()._to_json_dict()
 
         if self._doc_title:
             data["docTitle"] = self._doc_title
 
+        if self._style_tags:
+            data["styleTags"] = self._style_tags
+
         data["version"] = pbi.__version__
         return data
 
     def __reset_data(self):
         """support for run on ipython env"""
         self.children = []
         self.dataSources = []
@@ -598,22 +659,26 @@
         host._add_children(cp)
 
         self.__resourceManager.register_mermaid_cps()
         return cp
 
     def add_input(
         self,
-        data: DataSourceTable,
-        field: str,
+        field: Union[DataSourceField, DataSourceTable],
         where_expr="like '%${}%'",
         *,
         host: Optional[ContainerComponent] = None,
     ):
         """ """
-        cp = Input(where_expr).add_updateInfo(data.source_name, field)
+        if isinstance(field, DataSourceTable):
+            field = field[field.columns[0]]
+
+        assert isinstance(field, DataSourceField)
+
+        cp = Input(where_expr).add_updateInfo(field.source_name, field.name)
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
         self.__resourceManager.register_element_cps()
         return cp
 
     def add_numberSlider(
@@ -632,7 +697,30 @@
             .set_props({"range": range})
         )
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
         self.__resourceManager.register_element_cps()
         return cp
+
+    def space(
+        self,
+        space: Optional[str] = None,
+        *,
+        auto_fill_row=False,
+        host: Optional[ContainerComponent] = None,
+    ):
+        """增加组件之间的空间
+
+        Args:
+            space (Optional[str], optional): 间距值(默认为'0.2em'). Defaults to None.
+            auto_fill_row (bool, optional): 放在 flowBox 中,会迫使后续的组件往右靠. Defaults to False.
+        ---
+        >>> pbi.space()
+        >>> pbi.space('100px')
+        >>> pbi.space('0.5em')
+        """
+        cp = SpaceComponent(space, auto_fill_row)
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        return cp
```

### Comparing `pybi-next-0.4.1/pybi/core/components/__init__.py` & `pybi-next-0.4.2/pybi/core/components/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pybi.core.components.componentTag import ComponentTag
 from pybi.core.components.staticComponent import (
     TextComponent,
     UploadComponent,
     IconComponent,
     SvgIconComponent,
+    SpaceComponent,
 )
 from pybi.core.components.reactiveComponent import (
     ReactiveComponent,
     Slicer,
     Table,
     TextValue,
     Markdown,
     Input,
     NumberSlider,
 )
 from pybi.core.components.containerComponent import (
     ContainerComponent,
     BoxComponent,
-    ColBoxComponent,
     FlowBoxComponent,
     GridBoxComponent,
     TabsComponent,
     AffixComponent,
 )
 
 from pybi.core.components.mermaid import Mermaid
```

### Comparing `pybi-next-0.4.1/pybi/core/components/component.py` & `pybi-next-0.4.2/pybi/core/components/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, List, Optional, Union, Dict
 
 
 from pybi.utils.data_gen import Jsonable, get_global_id
 from .componentTag import ComponentTag
+from pybi.core.styles.styles import StyleBuilder
 
 if TYPE_CHECKING:
     from pybi.core.styles.styles import Style
     from pybi.core.sql import SqlWrapper
 
 
 class Component(Jsonable):
@@ -37,14 +38,30 @@
         self.classes.extend(values)
         return self
 
     def set_gridArea(self, area_name: str):
         self.__gridArea = area_name
         return self
 
+    def set_style(self, content: str):
+        """添加样式
+
+        Args:
+            content (str): 样式字符串,多个样式用分号相隔
+
+        ### 示例
+        >>> .set_style('color: #6E93D6; font-size: 200%; font-weight: 300')
+        """
+        styles = content.split(";")
+        styles = (s.split(":") for s in styles if s)
+        styles = {name.strip(): value.strip() for name, value in styles}
+
+        self._styles.append(StyleBuilder(styles))
+        return self
+
     def _to_json_dict(self):
         data = super()._to_json_dict()
         styles_dict = {}
         for style in self._styles:
             styles_dict.update(style._get_styles_dict())
         data["styles"] = styles_dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybi-next-0.4.1/pybi/core/components/componentTag.py` & `pybi-next-0.4.2/pybi/core/components/componentTag.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,7 +18,8 @@
     FlowBox = "FlowBox"
     GridBox = "GridBox"
     Tabs = "elTabs"
     Icon = "Icon"
     SvgIcon = "SvgIcon"
     Affix = "Affix"
     Mermaid = "Mermaid"
+    Space = "Space"
```

### Comparing `pybi-next-0.4.1/pybi/core/components/containerComponent.py` & `pybi-next-0.4.2/pybi/core/components/containerComponent.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,32 +29,80 @@
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         if self._appHost:
             self._appHost._with_temp_host_stack.pop()
 
 
 class BoxComponent(ContainerComponent):
-    def __init__(self, appHost: Optional[App] = None) -> None:
+    m_align_mapping = {
+        "left": "flex-start",
+        "center": "center",
+        "right": "flex-end",
+        "stretch": "stretch",
+    }
+
+    def __init__(
+        self, align: Optional[str] = None, appHost: Optional[App] = None
+    ) -> None:
+        """
+        Args:
+            align (Optional[str], optional): 'top' | 'center' | 'bottom'. Defaults to None.
+        """
         super().__init__(ComponentTag.Box, appHost)
+        self._align = align
+
+    def _to_json_dict(self):
+        data = super()._to_json_dict()
+        if self._align:
+            data["align"] = self.m_align_mapping[self._align]
+
+        return data
 
 
 class FlowBoxComponent(ContainerComponent):
-    def __init__(self, appHost: Optional[App] = None) -> None:
+    m_align_mapping = {
+        "left": "flex-start",
+        "center": "center",
+        "right": "flex-end",
+        "between": "space-between",
+        "around": "space-around",
+        "evenly": "space-evenly",
+        "stretch": "stretch",
+    }
+
+    def __init__(
+        self, align: Optional[str] = None, appHost: Optional[App] = None
+    ) -> None:
+        """
+        Args:
+            align (Optional[str], optional): 'left' | 'center' | 'right'. Defaults to None.
+        """
         super().__init__(ComponentTag.FlowBox, appHost)
+        self._align = align
 
     def __get_item__(self, idx: int):
         return self.children[idx]
 
+    def _to_json_dict(self):
+        data = super()._to_json_dict()
+        if self._align:
+            data["align"] = self.m_align_mapping[self._align]
+
+        return data
+
 
 class GridBoxComponent(ContainerComponent):
-    def __init__(self, areas: List[List[str]], appHost: Optional[App] = None) -> None:
+    def __init__(
+        self, areas: Optional[List[List[str]]] = None, appHost: Optional[App] = None
+    ) -> None:
         super().__init__(ComponentTag.GridBox, appHost)
         self.__areas = areas
         self.__columns_sizes: List[str] = []
         self.__rows_sizes: List[str] = []
+        self.__gridTemplateColumns = None
 
     def set_columns_sizes(self, sizes: List[Union[str, int]]):
         """
         >>> set_columns_sizes([1,2,2])
         >>> set_columns_sizes(['150px','1fr','2fr'])
         >>> set_columns_sizes(['150px','1fr','minmax(100px, 1fr)'])
         """
@@ -69,30 +117,57 @@
         """
         self.__rows_sizes = [f"{s}fr" if isinstance(s, int) else s for s in sizes]
         return self
 
     def __get_item__(self, idx: int):
         return self.children[idx]
 
+    def auto_fill_fixed_width(self, width="15em"):
+        """动态调整每行组件数量，每个组件固定宽度为指定 `width`。
+        当设置有效 grid areas 时，此设置无效
+
+        Args:
+            width (str, optional): 每个组件固定宽度. Defaults to "15em".
+
+        """
+        self.__gridTemplateColumns = f"repeat(auto-fill, {width})"
+        return self
+
+    def auto_fill_fixed_num(self, num=3):
+        """自动调整每行组件宽度，每行组件数量为 `num`。
+        当设置有效 grid areas 时，此设置无效
+
+        Args:
+            num (int, optional): 每行组件数量. Defaults to 3.
+
+        """
+        self.__gridTemplateColumns = f"repeat({3}, 1fr)"
+        return self
+
     def _to_json_dict(self):
         data = super()._to_json_dict()
-        data["areas"] = GridBoxComponent.areas_array2str(self.__areas)
-
-        areas_cols_len = max(map(len, self.__areas))
-        cols_size = GridBoxComponent.padded_grid_template(
-            self.__columns_sizes, areas_cols_len, "1fr"
-        )
 
-        areas_rows_len = len(self.__areas)
-        rows_size = GridBoxComponent.padded_grid_template(
-            self.__rows_sizes, areas_rows_len
-        )
+        if self.__areas:
+            data["areas"] = GridBoxComponent.areas_array2str(self.__areas)
 
-        data["gridTemplateColumns"] = " ".join(cols_size)
-        data["gridTemplateRows"] = " ".join(rows_size)
+            areas_cols_len = max(map(len, self.__areas))
+            cols_size = GridBoxComponent.padded_grid_template(
+                self.__columns_sizes, areas_cols_len, "1fr"
+            )
+
+            areas_rows_len = len(self.__areas)
+            rows_size = GridBoxComponent.padded_grid_template(
+                self.__rows_sizes, areas_rows_len
+            )
+
+            data["gridTemplateColumns"] = " ".join(cols_size)
+            data["gridTemplateRows"] = " ".join(rows_size)
+        else:
+            if self.__gridTemplateColumns:
+                data["gridTemplateColumns"] = self.__gridTemplateColumns
 
         return data
 
     @staticmethod
     def padded_grid_template(sizes: List[str], real_size: int, pad="auto"):
         """
         >>> sizes = ['1fr']
@@ -147,31 +222,14 @@
 
         lines = (line.strip() for line in areas.splitlines())
         remove_empty_rows = (line for line in lines if len(line) > 0)
         splie_space = (line.split() for line in remove_empty_rows)
         return list(splie_space)
 
 
-class ColBoxComponent(ContainerComponent):
-    def __init__(
-        self, spec: Optional[List[int]] = None, appHost: Optional[App] = None
-    ) -> None:
-        super().__init__(ComponentTag.ColBox, appHost)
-
-        if spec is None:
-            spec = [1, 1]
-
-        self.spec = spec
-
-        assert self._appHost is not None, "self._appHost must be app instance"
-
-    def __getitem__(self, idx: int):
-        return self.children[idx]
-
-
 class TabsComponent(ContainerComponent):
     def __init__(self, names: List[str], appHost: Optional[App] = None) -> None:
         """
         mode: 'fullWidth' | 'narrowing'
         """
         super().__init__(ComponentTag.Tabs, appHost)
         if len(names) > len(set(names)):
@@ -182,15 +240,15 @@
         self.panelsProps = {}
         self.tabsClasses: List[str] = []
         self.panelsClasses: List[str] = []
 
         self.__name2idx = {name: idx for idx, name in enumerate(self.names)}
 
         for _ in range(len(self.names)):
-            self._add_children(BoxComponent(appHost))
+            self._add_children(BoxComponent(appHost=appHost))
 
     def __getitem__(self, idx: Union[int, str]):
         if isinstance(idx, str):
             if idx not in self.__name2idx:
                 raise Exception(f"tab name[{idx}] not found")
             idx = self.__name2idx[idx]
 
@@ -245,7 +303,18 @@
 
         return data
 
 
 class AffixComponent(ContainerComponent):
     def __init__(self, appHost: Optional[App] = None) -> None:
         super().__init__(ComponentTag.Affix, appHost)
+
+
+class DynamicBoxComponent:
+    def __init__(self, grid_box: GridBoxComponent) -> None:
+        self.__grid_box = grid_box
+
+    def set_each_row_num(self, num: int):
+        pass
+
+    def set_each_width(self, width: str):
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/base.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/echarts.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/echarts.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/input.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/input.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/markdown.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/markdown.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/numberSlider.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/numberSlider.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/slicer.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/slicer.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/components/reactiveComponent/table.py` & `pybi-next-0.4.2/pybi/core/components/reactiveComponent/table.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/dataSource.py` & `pybi-next-0.4.2/pybi/core/dataSource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/sql.py` & `pybi-next-0.4.2/pybi/core/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/__init__.py` & `pybi-next-0.4.2/pybi/core/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/styles.py` & `pybi-next-0.4.2/pybi/core/styles/styles.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/boxShadow.py` & `pybi-next-0.4.2/pybi/core/styles/tailwindStyles/boxShadow.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textAlign.py` & `pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textAlign.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textColor.py` & `pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textColor.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textSize.py` & `pybi-next-0.4.2/pybi/core/styles/tailwindStyles/textSize.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/uiResource.py` & `pybi-next-0.4.2/pybi/core/uiResource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/core/webResources.py` & `pybi-next-0.4.2/pybi/core/webResources.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/bar.py` & `pybi-next-0.4.2/pybi/easyEcharts/bar.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/base.py` & `pybi-next-0.4.2/pybi/easyEcharts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 import copy
 from .utils import merge_user_options
 
 
 if TYPE_CHECKING:
     pass
 
-m_merge_keys = set(["legend", "title", "grid", "series"])
-
 
 class BaseChart:
     def __init__(self) -> None:
         self.__base_opt = {
-            "tooltip": {},
             "legend": {},
             "series": [],
             "title": {},
             "grid": {"containLabel": True},
         }
         self._merge_opt = {}
         self._updateInfos: List[EChartUpdateInfo] = []
```

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/line.py` & `pybi-next-0.4.2/pybi/easyEcharts/line.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/map.py` & `pybi-next-0.4.2/pybi/easyEcharts/map.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/pie.py` & `pybi-next-0.4.2/pybi/easyEcharts/pie.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/scatter.py` & `pybi-next-0.4.2/pybi/easyEcharts/scatter.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/easyEcharts/utils.py` & `pybi-next-0.4.2/pybi/easyEcharts/utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/icons/iconManager.py` & `pybi-next-0.4.2/pybi/icons/iconManager.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/icons/material_icons.py` & `pybi-next-0.4.2/pybi/icons/material_icons.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/static/echarts.min.js` & `pybi-next-0.4.2/pybi/static/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/static/echartsCps.iife.js` & `pybi-next-0.4.2/pybi/static/echartsCps.iife.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -94,28 +94,28 @@
             stop: p
         }
     }
     var Te;
     (function(e) {
         e.UP = "UP", e.RIGHT = "RIGHT", e.DOWN = "DOWN", e.LEFT = "LEFT", e.NONE = "NONE"
     })(Te || (Te = {}));
-    var At = Object.defineProperty,
-        Ae = Object.getOwnPropertySymbols,
-        mt = Object.prototype.hasOwnProperty,
+    var mt = Object.defineProperty,
+        me = Object.getOwnPropertySymbols,
+        At = Object.prototype.hasOwnProperty,
         $t = Object.prototype.propertyIsEnumerable,
-        me = (e, t, r) => t in e ? At(e, t, {
+        Ae = (e, t, r) => t in e ? mt(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
         Pt = (e, t) => {
-            for (var r in t || (t = {})) mt.call(t, r) && me(e, r, t[r]);
-            if (Ae)
-                for (var r of Ae(t)) $t.call(t, r) && me(e, r, t[r]);
+            for (var r in t || (t = {})) At.call(t, r) && Ae(e, r, t[r]);
+            if (me)
+                for (var r of me(t)) $t.call(t, r) && Ae(e, r, t[r]);
             return e
         };
     Pt({
         linear: gt
     }, {
         easeInSine: [.12, 0, .39, 0],
         easeOutSine: [.61, 1, .88, 1],
@@ -152,38 +152,38 @@
         It = $e || Et || Function("return this")();
     const P = It;
     var St = P.Symbol;
     const S = St;
     var Pe = Object.prototype,
         Ct = Pe.hasOwnProperty,
         Ft = Pe.toString,
-        G = S ? S.toStringTag : void 0;
+        N = S ? S.toStringTag : void 0;
 
     function Rt(e) {
-        var t = Ct.call(e, G),
-            r = e[G];
+        var t = Ct.call(e, N),
+            r = e[N];
         try {
-            e[G] = void 0;
+            e[N] = void 0;
             var n = !0
         } catch {}
         var a = Ft.call(e);
-        return n && (t ? e[G] = r : delete e[G]), a
+        return n && (t ? e[N] = r : delete e[N]), a
     }
     var Dt = Object.prototype,
         jt = Dt.toString;
 
     function Mt(e) {
         return jt.call(e)
     }
-    var Nt = "[object Null]",
-        Gt = "[object Undefined]",
+    var Gt = "[object Null]",
+        Nt = "[object Undefined]",
         xe = S ? S.toStringTag : void 0;
 
     function j(e) {
-        return e == null ? e === void 0 ? Gt : Nt : xe && xe in Object(e) ? Rt(e) : Mt(e)
+        return e == null ? e === void 0 ? Nt : Gt : xe && xe in Object(e) ? Rt(e) : Mt(e)
     }
 
     function M(e) {
         return e != null && typeof e == "object"
     }
     var Lt = "[object Symbol]";
 
@@ -192,22 +192,22 @@
     }
 
     function Bt(e, t) {
         for (var r = -1, n = e == null ? 0 : e.length, a = Array(n); ++r < n;) a[r] = t(e[r], r, e);
         return a
     }
     var Ut = Array.isArray;
-    const m = Ut;
+    const A = Ut;
     var Kt = 1 / 0,
         Ee = S ? S.prototype : void 0,
         Ie = Ee ? Ee.toString : void 0;
 
     function Se(e) {
         if (typeof e == "string") return e;
-        if (m(e)) return Bt(e, Se) + "";
+        if (A(e)) return Bt(e, Se) + "";
         if (Z(e)) return Ie ? Ie.call(e) : "";
         var t = e + "";
         return t == "0" && 1 / e == -Kt ? "-0" : t
     }
 
     function L(e) {
         var t = typeof e;
@@ -349,32 +349,32 @@
 
     function Tr(e) {
         var t = e && e.constructor,
             r = typeof t == "function" && t.prototype || Or;
         return e === r
     }
 
-    function Ar(e, t) {
+    function mr(e, t) {
         for (var r = -1, n = Array(e); ++r < e;) n[r] = t(r);
         return n
     }
-    var mr = "[object Arguments]";
+    var Ar = "[object Arguments]";
 
     function Me(e) {
-        return M(e) && j(e) == mr
+        return M(e) && j(e) == Ar
     }
-    var Ne = Object.prototype,
-        $r = Ne.hasOwnProperty,
-        Pr = Ne.propertyIsEnumerable,
+    var Ge = Object.prototype,
+        $r = Ge.hasOwnProperty,
+        Pr = Ge.propertyIsEnumerable,
         xr = Me(function() {
             return arguments
         }()) ? Me : function(e) {
             return M(e) && $r.call(e, "callee") && !Pr.call(e, "callee")
         };
-    const Ge = xr;
+    const Ne = xr;
 
     function Er() {
         return !1
     }
     var Le = typeof exports == "object" && exports && !exports.nodeType && exports,
         Be = Le && typeof module == "object" && module && !module.nodeType && module,
         Ir = Be && Be.exports === Le,
@@ -383,16 +383,16 @@
         Cr = Sr || Er;
     const ne = Cr;
     var Fr = "[object Arguments]",
         Rr = "[object Array]",
         Dr = "[object Boolean]",
         jr = "[object Date]",
         Mr = "[object Error]",
-        Nr = "[object Function]",
-        Gr = "[object Map]",
+        Gr = "[object Function]",
+        Nr = "[object Map]",
         Lr = "[object Number]",
         Br = "[object Object]",
         Ur = "[object RegExp]",
         Kr = "[object Set]",
         zr = "[object String]",
         Hr = "[object WeakMap]",
         Vr = "[object ArrayBuffer]",
@@ -403,15 +403,15 @@
         Xr = "[object Int16Array]",
         Zr = "[object Int32Array]",
         Jr = "[object Uint8Array]",
         kr = "[object Uint8ClampedArray]",
         en = "[object Uint16Array]",
         tn = "[object Uint32Array]",
         y = {};
-    y[Qr] = y[Wr] = y[Yr] = y[Xr] = y[Zr] = y[Jr] = y[kr] = y[en] = y[tn] = !0, y[Fr] = y[Rr] = y[Vr] = y[Dr] = y[qr] = y[jr] = y[Mr] = y[Nr] = y[Gr] = y[Lr] = y[Br] = y[Ur] = y[Kr] = y[zr] = y[Hr] = !1;
+    y[Qr] = y[Wr] = y[Yr] = y[Xr] = y[Zr] = y[Jr] = y[kr] = y[en] = y[tn] = !0, y[Fr] = y[Rr] = y[Vr] = y[Dr] = y[qr] = y[jr] = y[Mr] = y[Gr] = y[Nr] = y[Lr] = y[Br] = y[Ur] = y[Kr] = y[zr] = y[Hr] = !1;
 
     function rn(e) {
         return M(e) && re(e.length) && !!y[j(e)]
     }
 
     function nn(e) {
         return function(t) {
@@ -432,20 +432,20 @@
     var He = ze && ze.isTypedArray,
         sn = He ? nn(He) : rn;
     const Ve = sn;
     var un = Object.prototype,
         cn = un.hasOwnProperty;
 
     function fn(e, t) {
-        var r = m(e),
-            n = !r && Ge(e),
+        var r = A(e),
+            n = !r && Ne(e),
             a = !r && !n && ne(e),
             i = !r && !n && !a && Ve(e),
             o = r || n || a || i,
-            s = o ? Ar(e.length, String) : [],
+            s = o ? mr(e.length, String) : [],
             u = s.length;
         for (var l in e)(t || cn.call(e, l)) && !(o && (l == "length" || a && (l == "offset" || l == "parent") || i && (l == "buffer" || l == "byteLength" || l == "byteOffset") || ee(l, u))) && s.push(l);
         return s
     }
 
     function ln(e, t) {
         return function(r) {
@@ -467,15 +467,15 @@
     function ie(e) {
         return je(e) ? fn(e) : yn(e)
     }
     var _n = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
         vn = /^\w*$/;
 
     function oe(e, t) {
-        if (m(e)) return !1;
+        if (A(e)) return !1;
         var r = typeof e;
         return r == "number" || r == "symbol" || r == "boolean" || e == null || Z(e) ? !0 : vn.test(e) || !_n.test(e) || t != null && e in Object(t)
     }
     var bn = F(Object, "create");
     const U = bn;
 
     function wn() {
@@ -483,24 +483,24 @@
     }
 
     function On(e) {
         var t = this.has(e) && delete this.__data__[e];
         return this.size -= t ? 1 : 0, t
     }
     var Tn = "__lodash_hash_undefined__",
-        An = Object.prototype,
-        mn = An.hasOwnProperty;
+        mn = Object.prototype,
+        An = mn.hasOwnProperty;
 
     function $n(e) {
         var t = this.__data__;
         if (U) {
             var r = t[e];
             return r === Tn ? void 0 : r
         }
-        return mn.call(t, e) ? t[e] : void 0
+        return An.call(t, e) ? t[e] : void 0
     }
     var Pn = Object.prototype,
         xn = Pn.hasOwnProperty;
 
     function En(e) {
         var t = this.__data__;
         return U ? t[e] !== void 0 : xn.call(t, e)
@@ -548,31 +548,31 @@
         return r < 0 ? void 0 : t[r][1]
     }
 
     function Mn(e) {
         return V(this.__data__, e) > -1
     }
 
-    function Nn(e, t) {
+    function Gn(e, t) {
         var r = this.__data__,
             n = V(r, e);
         return n < 0 ? (++this.size, r.push([e, t])) : r[n][1] = t, this
     }
 
     function x(e) {
         var t = -1,
             r = e == null ? 0 : e.length;
         for (this.clear(); ++t < r;) {
             var n = e[t];
             this.set(n[0], n[1])
         }
     }
-    x.prototype.clear = Cn, x.prototype.delete = Dn, x.prototype.get = jn, x.prototype.has = Mn, x.prototype.set = Nn;
-    var Gn = F(P, "Map");
-    const K = Gn;
+    x.prototype.clear = Cn, x.prototype.delete = Dn, x.prototype.get = jn, x.prototype.has = Mn, x.prototype.set = Gn;
+    var Nn = F(P, "Map");
+    const K = Nn;
 
     function Ln() {
         this.size = 0, this.__data__ = {
             hash: new R,
             map: new(K || x),
             string: new R
         }
@@ -651,15 +651,15 @@
     const Zn = Xn;
 
     function Jn(e) {
         return e == null ? "" : Se(e)
     }
 
     function ue(e, t) {
-        return m(e) ? e : oe(e, t) ? [e] : Zn(Jn(e))
+        return A(e) ? e : oe(e, t) ? [e] : Zn(Jn(e))
     }
     var kn = 1 / 0;
 
     function z(e) {
         if (typeof e == "string" || Z(e)) return e;
         var t = e + "";
         return t == "0" && 1 / e == -kn ? "-0" : t
@@ -735,59 +735,59 @@
                 return la.call(e, t)
             }))
         } : ca;
     const da = pa;
 
     function ha(e, t, r) {
         var n = t(e);
-        return m(e) ? n : ta(n, r(e))
+        return A(e) ? n : ta(n, r(e))
     }
 
     function We(e) {
         return ha(e, ie, da)
     }
     var ga = F(P, "DataView");
     const ce = ga;
     var ya = F(P, "Promise");
     const fe = ya;
     var _a = F(P, "Set");
-    const N = _a;
+    const G = _a;
     var Ye = "[object Map]",
         va = "[object Object]",
         Xe = "[object Promise]",
         Ze = "[object Set]",
         Je = "[object WeakMap]",
         ke = "[object DataView]",
         ba = C(ce),
         wa = C(K),
         Oa = C(fe),
-        Ta = C(N),
-        Aa = C(k),
+        Ta = C(G),
+        ma = C(k),
         D = j;
-    (ce && D(new ce(new ArrayBuffer(1))) != ke || K && D(new K) != Ye || fe && D(fe.resolve()) != Xe || N && D(new N) != Ze || k && D(new k) != Je) && (D = function(e) {
+    (ce && D(new ce(new ArrayBuffer(1))) != ke || K && D(new K) != Ye || fe && D(fe.resolve()) != Xe || G && D(new G) != Ze || k && D(new k) != Je) && (D = function(e) {
         var t = j(e),
             r = t == va ? e.constructor : void 0,
             n = r ? C(r) : "";
         if (n) switch (n) {
             case ba:
                 return ke;
             case wa:
                 return Ye;
             case Oa:
                 return Xe;
             case Ta:
                 return Ze;
-            case Aa:
+            case ma:
                 return Je
         }
         return t
     });
     const et = D;
-    var ma = P.Uint8Array;
-    const tt = ma;
+    var Aa = P.Uint8Array;
+    const tt = Aa;
     var $a = "__lodash_hash_undefined__";
 
     function Pa(e) {
         return this.__data__.set(e, $a), this
     }
 
     function xa(e) {
@@ -864,16 +864,16 @@
         }), r
     }
     var Fa = 1,
         Ra = 2,
         Da = "[object Boolean]",
         ja = "[object Date]",
         Ma = "[object Error]",
-        Na = "[object Map]",
-        Ga = "[object Number]",
+        Ga = "[object Map]",
+        Na = "[object Number]",
         La = "[object RegExp]",
         Ba = "[object Set]",
         Ua = "[object String]",
         Ka = "[object Symbol]",
         za = "[object ArrayBuffer]",
         Ha = "[object DataView]",
         at = S ? S.prototype : void 0,
@@ -884,22 +884,22 @@
             case Ha:
                 if (e.byteLength != t.byteLength || e.byteOffset != t.byteOffset) return !1;
                 e = e.buffer, t = t.buffer;
             case za:
                 return !(e.byteLength != t.byteLength || !i(new tt(e), new tt(t)));
             case Da:
             case ja:
-            case Ga:
+            case Na:
                 return te(+e, +t);
             case Ma:
                 return e.name == t.name && e.message == t.message;
             case La:
             case Ua:
                 return e == t + "";
-            case Na:
+            case Ga:
                 var s = Ca;
             case Ba:
                 var u = n & Fa;
                 if (s || (s = le), e.size != t.size && !u) return !1;
                 var l = o.get(e);
                 if (l) return l == t;
                 n |= Ra, o.set(e, t);
@@ -952,16 +952,16 @@
         it = "[object Arguments]",
         ot = "[object Array]",
         Q = "[object Object]",
         Za = Object.prototype,
         st = Za.hasOwnProperty;
 
     function Ja(e, t, r, n, a, i) {
-        var o = m(e),
-            s = m(t),
+        var o = A(e),
+            s = A(t),
             u = o ? ot : et(e),
             l = s ? ot : et(t);
         u = u == it ? Q : u, l = l == it ? Q : l;
         var p = u == Q,
             c = l == Q,
             d = u == l;
         if (d && ne(e)) {
@@ -1045,15 +1045,15 @@
     function ii(e, t, r) {
         t = ue(t, e);
         for (var n = -1, a = t.length, i = !1; ++n < a;) {
             var o = z(t[n]);
             if (!(i = e != null && r(e, o))) break;
             e = e[o]
         }
-        return i || ++n != a ? i : (a = e == null ? 0 : e.length, !!a && re(a) && ee(o, a) && (m(e) || Ge(e)))
+        return i || ++n != a ? i : (a = e == null ? 0 : e.length, !!a && re(a) && ee(o, a) && (A(e) || Ne(e)))
     }
 
     function oi(e, t) {
         return e != null && ii(e, t, ai)
     }
     var si = 1,
         ui = 2;
@@ -1078,15 +1078,15 @@
     }
 
     function pi(e) {
         return oe(e) ? fi(z(e)) : li(e)
     }
 
     function di(e) {
-        return typeof e == "function" ? e : e == null ? zt : typeof e == "object" ? m(e) ? ci(e[0], e[1]) : ni(e) : pi(e)
+        return typeof e == "function" ? e : e == null ? zt : typeof e == "object" ? A(e) ? ci(e[0], e[1]) : ni(e) : pi(e)
     }
 
     function hi(e, t, r, n) {
         for (var a = -1, i = e == null ? 0 : e.length; ++a < i;) {
             var o = e[a];
             t(n, o, r(o), e)
         }
@@ -1123,30 +1123,30 @@
 
     function Ti(e, t, r, n) {
         return Oi(e, function(a, i, o) {
             t(n, a, r(a), o)
         }), n
     }
 
-    function Ai(e, t) {
+    function mi(e, t) {
         return function(r, n) {
-            var a = m(r) ? hi : Ti,
+            var a = A(r) ? hi : Ti,
                 i = t ? t() : {};
             return a(r, e, di(n), i)
         }
     }
 
-    function mi(e, t, r) {
+    function Ai(e, t, r) {
         for (var n = -1, a = e == null ? 0 : e.length; ++n < a;)
             if (r(t, e[n])) return !0;
         return !1
     }
     var $i = Object.prototype,
         Pi = $i.hasOwnProperty,
-        xi = Ai(function(e, t, r) {
+        xi = mi(function(e, t, r) {
             Pi.call(e, r) ? e[r].push(t) : De(e, r, [t])
         });
     const Ei = xi;
 
     function Ii(e, t, r, n) {
         if (!L(e)) return e;
         t = ue(t, e);
@@ -1163,28 +1163,28 @@
         return e
     }
 
     function W(e, t, r) {
         return e == null ? e : Ii(e, t, r)
     }
     var Si = 1 / 0,
-        Ci = N && 1 / le(new N([, -0]))[1] == Si ? function(e) {
-            return new N(e)
+        Ci = G && 1 / le(new G([, -0]))[1] == Si ? function(e) {
+            return new G(e)
         } : ur;
     const Fi = Ci;
     var Ri = 200;
 
     function Di(e, t, r) {
         var n = -1,
             a = hr,
             i = e.length,
             o = !0,
             s = [],
             u = s;
-        if (r) o = !1, a = mi;
+        if (r) o = !1, a = Ai;
         else if (i >= Ri) {
             var l = t ? null : Fi(e);
             if (l) return le(l);
             o = !1, a = rt, u = new H
         } else u = t ? [] : s;
         e: for (; ++n < i;) {
             var p = e[n],
@@ -1202,15 +1202,15 @@
         return e && e.length ? Di(e) : []
     }
     const Mi = {
         uniq: ji,
         groupBy: Ei
     };
 
-    function Ni(e, t) {
+    function Gi(e, t) {
         const r = new Function("utils", "rows", "fields", e ?? "");
 
         function n(a) {
             switch (t) {
                 case "udf":
                     if (e !== null) return r(Mi, a.rows, a.fields);
                     break;
@@ -1220,15 +1220,15 @@
             }
         }
         return {
             map: n
         }
     }
 
-    function Gi(e, t, r, n, a) {
+    function Ni(e, t, r, n, a) {
         const i = n.db.parse2sqlValueBaseFieldType(a.table, a.field, e),
             o = X(t, r);
         n.dataset.addFilter(o, a.table, `${a.field}=${i}`)
     }
 
     function Li() {
         return function() {
@@ -1266,15 +1266,15 @@
             })
         })
     }
 
     function zi(e, t, r, n, a, i) {
         let o = null;
         return e.updateInfos.forEach(s => {
-            s.actionType === t && (o = r(s), Gi(o, n, a, i, s))
+            s.actionType === t && (o = r(s), Ni(o, n, a, i, s))
         }), o
     }
 
     function Hi(e) {
         return e.updateInfos.some(t => t.actionType === "click")
     }
 
@@ -1306,36 +1306,42 @@
         throw new Error(`scatter chart not support value type : ${t.valueType}`)
     }
 
     function Xi(e, t) {
         if (t.valueType === "name") return e.name;
         throw new Error(`scatter chart not support value type : ${t.valueType}`)
     }
+
+    function Zi(e, t) {
+        if (t.valueType === "name") return e.name;
+        throw new Error(`radar chart not support value type : ${t.valueType}`)
+    }
     const ft = new Map([
         ["bar", qi],
         ["line", Qi],
         ["pie", Wi],
         ["scatter", Yi],
-        ["map", Xi]
+        ["map", Xi],
+        ["radar", Zi]
     ]);
 
     function lt(e, t) {
         const r = e.seriesType;
         if (ft.has(r)) return ft.get(r)(e, t);
         throw new Error(`ParamValueGetter not support chart type:[${r}]`)
     }
 
-    function Zi(e, t) {
+    function Ji(e, t) {
         if (t.seriesHasData()) {
             const r = t.series.data[0];
             r.length > 0 && (typeof r[0] == "string" && e.setProps(`xAxis[${t.getXAxisIndex()}].type`, "category"), typeof r[1] == "string" && e.setProps(`yAxis[${t.getYAxisIndex()}].type`, "category"))
         }
     }
 
-    function Ji(e) {
+    function ki(e) {
         "xAxis" in e && !Array.isArray(e.xAxis) && (e.xAxis = [e.xAxis]), "yAxis" in e && !Array.isArray(e.yAxis) && (e.yAxis = [e.yAxis]), e.xAxis, e.yAxis;
 
         function t(a, i) {
             W(e, a, i)
         }
 
         function r(a, i, o) {
@@ -1351,15 +1357,15 @@
             options: e,
             setProps: t,
             setSeriesProps: r,
             seriesHasData: n
         }
     }
 
-    function ki(e) {
+    function eo(e) {
         function t(i, o) {
             W(e, i, o)
         }
 
         function r() {
             return "data" in e && e.data.length > 0
         }
@@ -1376,58 +1382,58 @@
             setProps: t,
             seriesHasData: r,
             getXAxisIndex: n,
             getYAxisIndex: a
         }
     }
 
-    function eo(e) {
+    function to(e) {
         for (const t of e.series) {
             if (!("type" in t)) continue;
-            const r = Ji(e),
-                n = ki(t);
+            const r = ki(e),
+                n = eo(t);
             switch (t.type) {
                 case "line":
                     break;
                 case "bar":
                     break;
                 case "pie":
                     break;
                 case "scatter":
-                    Zi(r, n);
+                    Ji(r, n);
                     break
             }
         }
     }
 
-    function to(e) {
+    function ro(e) {
         return new Function(`f= ${e};return f `)()
     }
 
-    function ro(e, t, r, n) {
+    function no(e, t, r, n) {
         const a = e.chartInfos[t],
             i = a.options,
             o = Li(),
             s = Hi(a);
         a.jsCodes.forEach(h => {
-            const g = to(h.code);
+            const g = ro(h.code);
             W(i, h.path, g)
         });
 
         function u() {
             switch (a.datasetInfos.forEach(h => {
                     const _ = n.utils.createSqlQuery(X(e, t), h.sqlInfo.sql).query(),
-                        w = Ni(h.sqlInfo.jsMap, h.sqlInfo.type).map(_);
+                        w = Gi(h.sqlInfo.jsMap, h.sqlInfo.type).map(_);
                     W(i, h.path, w)
                 }), r.value) {
                 case "forward":
                     Vi(i, o);
                     break
             }
-            return eo(i), i
+            return to(i), i
         }
 
         function l() {
             a.updateInfos.forEach(h => {
                 const g = X(e, t);
                 n.dataset.removeFilters(g, h.table)
             })
@@ -1458,18 +1464,18 @@
             drillStartPos: c,
             setDataGroupValue: d,
             getValueFromParams: lt,
             hasClickInfo: s
         }
     }
 
-    function no(e, t) {
+    function ao(e, t) {
         const r = f.ref("none");
         let n = [];
-        e.optionType === "dict" && (n = e.chartInfos.map((c, d) => ro(e, d, r, t)));
+        e.optionType === "dict" && (n = e.chartInfos.map((c, d) => no(e, d, r, t)));
         const a = f.ref(0),
             i = f.computed(() => a.value > 0),
             o = f.computed(() => a.value < n.length - 1),
             s = f.computed(() => n[a.value]);
 
         function u(c, d, h) {
             s.value.hasClickInfo && (r.value = "forward", s.value.drillStartPos(c), a.value += 1, s.value.setDataGroupValue(h))
@@ -1491,16 +1497,16 @@
             canBack: i,
             canForward: o,
             back: l,
             setSeriesKeys: p
         }
     }
 
-    function ao(e, t) {
-        const r = no(e, t);
+    function io(e, t) {
+        const r = ao(e, t);
 
         function n() {
             return f.computed(() => r.curController.value.useOptions())
         }
 
         function a() {
             r.curController.value.removeFilter()
@@ -1512,57 +1518,57 @@
         return {
             getData: n,
             addFilter: i,
             removeFilter: a,
             chartController: r
         }
     }
-    const io = "sqlAnalyzeKey",
-        oo = "componentKey",
-        so = "datasetKey",
-        uo = "dbKey",
-        co = "utilsKey",
-        fo = "webResourcesServiceKey",
-        lo = ["data-tag"],
-        po = {
+    const oo = "sqlAnalyzeKey",
+        so = "componentKey",
+        uo = "datasetKey",
+        co = "dbKey",
+        fo = "utilsKey",
+        lo = "webResourcesServiceKey",
+        po = ["data-tag"],
+        ho = {
             key: 0,
             class: "debug-box"
         },
-        ho = {
+        go = {
             key: 0,
             rows: "25",
             cols: "50",
             readonly: ""
         },
-        go = f.defineComponent({
+        yo = f.defineComponent({
             __name: "EChart",
             props: {
                 model: null
             },
             setup(e) {
                 const t = e;
                 f.useCssVars(v => ({
-                    b21c2e2a: f.unref(g)
+                    "7bb46307": f.unref(g)
                 }));
-                const r = f.inject(so),
-                    n = f.inject(io),
-                    a = f.inject(uo),
-                    i = f.inject(oo),
-                    o = f.inject(co),
-                    s = f.inject(fo),
+                const r = f.inject(uo),
+                    n = f.inject(oo),
+                    a = f.inject(co),
+                    i = f.inject(so),
+                    o = f.inject(fo),
+                    s = f.inject(lo),
                     u = t.model,
                     l = [];
                 u.chartInfos.forEach(v => {
                     v == null || v.mapIds.forEach(T => {
-                        const A = s.getResource(T);
-                        l.push(A)
+                        const m = s.getResource(T);
+                        l.push(m)
                     })
                 });
                 const p = f.computed(() => l.every(v => v.value)),
-                    c = ao(u, {
+                    c = io(u, {
                         sqlAnalyze: n,
                         dataset: r,
                         db: a,
                         utils: o
                     }),
                     d = c.getData(),
                     h = f.ref(null);
@@ -1571,71 +1577,72 @@
                 let _ = null;
                 f.onUnmounted(() => {
                     _ == null || _.dispose()
                 }), f.watch([p, h], ([v, T]) => {
                     if (!(v && T) || (_ = echarts.init(T, null, {
                             renderer: i.getApp().echartsRenderer
                         }), _ === null)) return;
-                    const A = _;
+                    const m = _;
                     f.watchEffect(() => {
-                        c.chartController.setSeriesKeys(A, d.value.series.map($ => $.id)), A.setOption(d.value, !0)
-                    }), A.on("mouseover", "series", $ => {
+                        c.chartController.setSeriesKeys(m, d.value.series.map($ => $.id)), m.setOption(d.value, !0)
+                    }), m.on("mouseover", "series", $ => {
                         c.chartController.curController.value.hasClickInfo || c.addFilter($, "hover")
-                    }), A.on("mouseout", "series", $ => {
+                    }), m.on("mouseout", "series", $ => {
                         c.chartController.curController.value.hasClickInfo || c.removeFilter()
                     });
 
-                    function yo() {
+                    function _o() {
                         c.chartController.curController.value.hasClickInfo && c.removeFilter()
                     }
-                    A.getZr().on("click", function($) {
-                        $.target || yo()
-                    }), A.on("click", "series", $ => {
+                    m.getZr().on("click", function($) {
+                        $.target || _o()
+                    }), m.on("click", "series", $ => {
                         if (c.chartController.canForward.value) {
-                            const _o = c.addFilter($, "click");
-                            c.chartController.next(A, $, _o)
+                            const vo = c.addFilter($, "click");
+                            c.chartController.next(m, $, vo)
                         } else c.addFilter($, "click")
                     }), _t("resize", () => {
-                        A.resize()
+                        m.resize()
                     }), Tt(T, () => {
-                        A.resize()
+                        m.resize()
                     })
                 });
 
                 function b() {
                     c.chartController.back(_), c.chartController.curController.value.removeFilter()
                 }
                 const w = u.debugTag !== null,
                     O = f.ref(!1);
 
                 function Y() {
                     O.value = !O.value
                 }
                 return (v, T) => (f.openBlock(), f.createElementBlock("div", {
-                    class: "echart-box",
-                    "data-tag": f.unref(u).tag
+                    class: "echart-box pybi-container",
+                    "data-tag": f.unref(u).tag,
+                    "data-pybi-auto-width": ""
                 }, [f.withDirectives(f.createElementVNode("div", {
                     class: "back",
                     onClick: b
                 }, "上一级", 512), [
                     [f.vShow, f.unref(c).chartController.canBack.value]
-                ]), w ? (f.openBlock(), f.createElementBlock("div", po, [f.createElementVNode("button", {
+                ]), w ? (f.openBlock(), f.createElementBlock("div", ho, [f.createElementVNode("button", {
                     onClick: Y
-                }, "options view open"), O.value ? (f.openBlock(), f.createElementBlock("textarea", ho, f.toDisplayString(f.unref(d)), 1)) : f.createCommentVNode("", !0)])) : f.createCommentVNode("", !0), f.createElementVNode("div", {
+                }, "options view open"), O.value ? (f.openBlock(), f.createElementBlock("textarea", go, f.toDisplayString(f.unref(d)), 1)) : f.createCommentVNode("", !0)])) : f.createCommentVNode("", !0), f.createElementVNode("div", {
                     class: "echart",
                     ref_key: "chartDiv",
                     ref: h
-                }, null, 512)], 8, lo))
+                }, null, 512)], 8, po))
             }
         }),
-        bo = "";
+        wo = "";
     return [{
         tag: "EChart",
         cp: ((e, t) => {
             const r = e.__vccOpts || e;
             for (const [n, a] of t) r[n] = a;
             return r
-        })(go, [
-            ["__scopeId", "data-v-3b2c4827"]
+        })(yo, [
+            ["__scopeId", "data-v-74aab211"]
         ])
     }]
 }(Vue);
```

### Comparing `pybi-next-0.4.1/pybi/static/elementCps-style.css` & `pybi-next-0.4.2/pybi/static/elementCps-style.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-@charset "UTF-8";:root{--el-color-white:#ffffff;--el-color-black:#000000;--el-color-primary-rgb:64,158,255;--el-color-success-rgb:103,194,58;--el-color-warning-rgb:230,162,60;--el-color-danger-rgb:245,108,108;--el-color-error-rgb:245,108,108;--el-color-info-rgb:144,147,153;--el-font-size-extra-large:20px;--el-font-size-large:18px;--el-font-size-medium:16px;--el-font-size-base:14px;--el-font-size-small:13px;--el-font-size-extra-small:12px;--el-font-family:"Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","\5fae\8f6f\96c5\9ed1",Arial,sans-serif;--el-font-weight-primary:500;--el-font-line-height-primary:24px;--el-index-normal:1;--el-index-top:1000;--el-index-popper:2000;--el-border-radius-base:4px;--el-border-radius-small:2px;--el-border-radius-round:20px;--el-border-radius-circle:100%;--el-transition-duration:.3s;--el-transition-duration-fast:.2s;--el-transition-function-ease-in-out-bezier:cubic-bezier(.645, .045, .355, 1);--el-transition-function-fast-bezier:cubic-bezier(.23, 1, .32, 1);--el-transition-all:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);--el-transition-fade:opacity var(--el-transition-duration) var(--el-transition-function-fast-bezier);--el-transition-md-fade:transform var(--el-transition-duration) var(--el-transition-function-fast-bezier),opacity var(--el-transition-duration) var(--el-transition-function-fast-bezier);--el-transition-fade-linear:opacity var(--el-transition-duration-fast) linear;--el-transition-border:border-color var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-transition-box-shadow:box-shadow var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-transition-color:color var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-component-size-large:40px;--el-component-size:32px;--el-component-size-small:24px}:root{color-scheme:light;--el-color-white:#ffffff;--el-color-black:#000000;--el-color-primary:#409eff;--el-color-primary-light-3:#79bbff;--el-color-primary-light-5:#a0cfff;--el-color-primary-light-7:#c6e2ff;--el-color-primary-light-8:#d9ecff;--el-color-primary-light-9:#ecf5ff;--el-color-primary-dark-2:#337ecc;--el-color-success:#67c23a;--el-color-success-light-3:#95d475;--el-color-success-light-5:#b3e19d;--el-color-success-light-7:#d1edc4;--el-color-success-light-8:#e1f3d8;--el-color-success-light-9:#f0f9eb;--el-color-success-dark-2:#529b2e;--el-color-warning:#e6a23c;--el-color-warning-light-3:#eebe77;--el-color-warning-light-5:#f3d19e;--el-color-warning-light-7:#f8e3c5;--el-color-warning-light-8:#faecd8;--el-color-warning-light-9:#fdf6ec;--el-color-warning-dark-2:#b88230;--el-color-danger:#f56c6c;--el-color-danger-light-3:#f89898;--el-color-danger-light-5:#fab6b6;--el-color-danger-light-7:#fcd3d3;--el-color-danger-light-8:#fde2e2;--el-color-danger-light-9:#fef0f0;--el-color-danger-dark-2:#c45656;--el-color-error:#f56c6c;--el-color-error-light-3:#f89898;--el-color-error-light-5:#fab6b6;--el-color-error-light-7:#fcd3d3;--el-color-error-light-8:#fde2e2;--el-color-error-light-9:#fef0f0;--el-color-error-dark-2:#c45656;--el-color-info:#909399;--el-color-info-light-3:#b1b3b8;--el-color-info-light-5:#c8c9cc;--el-color-info-light-7:#dedfe0;--el-color-info-light-8:#e9e9eb;--el-color-info-light-9:#f4f4f5;--el-color-info-dark-2:#73767a;--el-bg-color:#ffffff;--el-bg-color-page:#f2f3f5;--el-bg-color-overlay:#ffffff;--el-text-color-primary:#303133;--el-text-color-regular:#606266;--el-text-color-secondary:#909399;--el-text-color-placeholder:#a8abb2;--el-text-color-disabled:#c0c4cc;--el-border-color:#dcdfe6;--el-border-color-light:#e4e7ed;--el-border-color-lighter:#ebeef5;--el-border-color-extra-light:#f2f6fc;--el-border-color-dark:#d4d7de;--el-border-color-darker:#cdd0d6;--el-fill-color:#f0f2f5;--el-fill-color-light:#f5f7fa;--el-fill-color-lighter:#fafafa;--el-fill-color-extra-light:#fafcff;--el-fill-color-dark:#ebedf0;--el-fill-color-darker:#e6e8eb;--el-fill-color-blank:#ffffff;--el-box-shadow:0px 12px 32px 4px rgba(0, 0, 0, .04),0px 8px 20px rgba(0, 0, 0, .08);--el-box-shadow-light:0px 0px 12px rgba(0, 0, 0, .12);--el-box-shadow-lighter:0px 0px 6px rgba(0, 0, 0, .12);--el-box-shadow-dark:0px 16px 48px 16px rgba(0, 0, 0, .08),0px 12px 32px rgba(0, 0, 0, .12),0px 8px 16px -8px rgba(0, 0, 0, .16);--el-disabled-bg-color:var(--el-fill-color-light);--el-disabled-text-color:var(--el-text-color-placeholder);--el-disabled-border-color:var(--el-border-color-light);--el-overlay-color:rgba(0, 0, 0, .8);--el-overlay-color-light:rgba(0, 0, 0, .7);--el-overlay-color-lighter:rgba(0, 0, 0, .5);--el-mask-color:rgba(255, 255, 255, .9);--el-mask-color-extra-light:rgba(255, 255, 255, .3);--el-border-width:1px;--el-border-style:solid;--el-border-color-hover:var(--el-text-color-disabled);--el-border:var(--el-border-width) var(--el-border-style) var(--el-border-color);--el-svg-monochrome-grey:var(--el-border-color)}.fade-in-linear-enter-active,.fade-in-linear-leave-active{transition:var(--el-transition-fade-linear)}.fade-in-linear-enter-from,.fade-in-linear-leave-to{opacity:0}.el-fade-in-linear-enter-active,.el-fade-in-linear-leave-active{transition:var(--el-transition-fade-linear)}.el-fade-in-linear-enter-from,.el-fade-in-linear-leave-to{opacity:0}.el-fade-in-enter-active,.el-fade-in-leave-active{transition:all var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-fade-in-enter-from,.el-fade-in-leave-active{opacity:0}.el-zoom-in-center-enter-active,.el-zoom-in-center-leave-active{transition:all var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-zoom-in-center-enter-from,.el-zoom-in-center-leave-active{opacity:0;transform:scaleX(0)}.el-zoom-in-top-enter-active,.el-zoom-in-top-leave-active{opacity:1;transform:scaleY(1);transition:var(--el-transition-md-fade);transform-origin:center top}.el-zoom-in-top-enter-active[data-popper-placement^=top],.el-zoom-in-top-leave-active[data-popper-placement^=top]{transform-origin:center bottom}.el-zoom-in-top-enter-from,.el-zoom-in-top-leave-active{opacity:0;transform:scaleY(0)}.el-zoom-in-bottom-enter-active,.el-zoom-in-bottom-leave-active{opacity:1;transform:scaleY(1);transition:var(--el-transition-md-fade);transform-origin:center bottom}.el-zoom-in-bottom-enter-from,.el-zoom-in-bottom-leave-active{opacity:0;transform:scaleY(0)}.el-zoom-in-left-enter-active,.el-zoom-in-left-leave-active{opacity:1;transform:scale(1);transition:var(--el-transition-md-fade);transform-origin:top left}.el-zoom-in-left-enter-from,.el-zoom-in-left-leave-active{opacity:0;transform:scale(.45)}.collapse-transition{transition:var(--el-transition-duration) height ease-in-out,var(--el-transition-duration) padding-top ease-in-out,var(--el-transition-duration) padding-bottom ease-in-out}.el-collapse-transition-enter-active,.el-collapse-transition-leave-active{transition:var(--el-transition-duration) max-height ease-in-out,var(--el-transition-duration) padding-top ease-in-out,var(--el-transition-duration) padding-bottom ease-in-out}.horizontal-collapse-transition{transition:var(--el-transition-duration) width ease-in-out,var(--el-transition-duration) padding-left ease-in-out,var(--el-transition-duration) padding-right ease-in-out}.el-list-enter-active,.el-list-leave-active{transition:all 1s}.el-list-enter-from,.el-list-leave-to{opacity:0;transform:translateY(-30px)}.el-list-leave-active{position:absolute!important}.el-opacity-transition{transition:opacity var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-icon-loading{-webkit-animation:rotating 2s linear infinite;animation:rotating 2s linear infinite}.el-icon--right{margin-left:5px}.el-icon--left{margin-right:5px}@-webkit-keyframes rotating{0%{transform:rotate(0)}to{transform:rotate(360deg)}}@keyframes rotating{0%{transform:rotate(0)}to{transform:rotate(360deg)}}.el-icon{--color:inherit;height:1em;width:1em;line-height:1em;display:inline-flex;justify-content:center;align-items:center;position:relative;fill:currentColor;color:var(--color);font-size:inherit}.el-icon.is-loading{-webkit-animation:rotating 2s linear infinite;animation:rotating 2s linear infinite}.el-icon svg{height:1em;width:1em}.el-textarea{--el-input-text-color:var(--el-text-color-regular);--el-input-border:var(--el-border);--el-input-hover-border:var(--el-border-color-hover);--el-input-focus-border:var(--el-color-primary);--el-input-transparent-border:0 0 0 1px transparent inset;--el-input-border-color:var(--el-border-color);--el-input-border-radius:var(--el-border-radius-base);--el-input-bg-color:var(--el-fill-color-blank);--el-input-icon-color:var(--el-text-color-placeholder);--el-input-placeholder-color:var(--el-text-color-placeholder);--el-input-hover-border-color:var(--el-border-color-hover);--el-input-clear-hover-color:var(--el-text-color-secondary);--el-input-focus-border-color:var(--el-color-primary)}.el-textarea{position:relative;display:inline-block;width:100%;vertical-align:bottom;font-size:var(--el-font-size-base)}.el-textarea__inner{position:relative;display:block;resize:vertical;padding:5px 11px;line-height:1.5;box-sizing:border-box;width:100%;font-size:inherit;font-family:inherit;color:var(--el-input-text-color,var(--el-text-color-regular));background-color:var(--el-input-bg-color,var(--el-fill-color-blank));background-image:none;-webkit-appearance:none;box-shadow:0 0 0 1px var(--el-input-border-color,var(--el-border-color)) inset;border-radius:var(--el-input-border-radius,var(--el-border-radius-base));transition:var(--el-transition-box-shadow);border:none}.el-textarea__inner::-moz-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner:-ms-input-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner::placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner:hover{box-shadow:0 0 0 1px var(--el-input-hover-border-color) inset}.el-textarea__inner:focus{outline:0;box-shadow:0 0 0 1px var(--el-input-focus-border-color) inset}.el-textarea .el-input__count{color:var(--el-color-info);background:var(--el-fill-color-blank);position:absolute;font-size:12px;line-height:14px;bottom:5px;right:10px}.el-textarea.is-disabled .el-textarea__inner{background-color:var(--el-disabled-bg-color);border-color:var(--el-disabled-border-color);color:var(--el-disabled-text-color);cursor:not-allowed}.el-textarea.is-disabled .el-textarea__inner::-moz-placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-disabled .el-textarea__inner:-ms-input-placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-disabled .el-textarea__inner::placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-exceed .el-textarea__inner{border-color:var(--el-color-danger)}.el-textarea.is-exceed .el-input__count{color:var(--el-color-danger)}.el-input{--el-input-text-color:var(--el-text-color-regular);--el-input-border:var(--el-border);--el-input-hover-border:var(--el-border-color-hover);--el-input-focus-border:var(--el-color-primary);--el-input-transparent-border:0 0 0 1px transparent inset;--el-input-border-color:var(--el-border-color);--el-input-border-radius:var(--el-border-radius-base);--el-input-bg-color:var(--el-fill-color-blank);--el-input-icon-color:var(--el-text-color-placeholder);--el-input-placeholder-color:var(--el-text-color-placeholder);--el-input-hover-border-color:var(--el-border-color-hover);--el-input-clear-hover-color:var(--el-text-color-secondary);--el-input-focus-border-color:var(--el-color-primary)}.el-input{--el-input-height:var(--el-component-size);position:relative;font-size:var(--el-font-size-base);display:inline-flex;width:100%;line-height:var(--el-input-height);box-sizing:border-box;vertical-align:middle}.el-input::-webkit-scrollbar{z-index:11;width:6px}.el-input::-webkit-scrollbar:horizontal{height:6px}.el-input::-webkit-scrollbar-thumb{border-radius:5px;width:6px;background:var(--el-text-color-disabled)}.el-input::-webkit-scrollbar-corner{background:var(--el-fill-color-blank)}.el-input::-webkit-scrollbar-track{background:var(--el-fill-color-blank)}.el-input::-webkit-scrollbar-track-piece{background:var(--el-fill-color-blank);width:6px}.el-input .el-input__clear,.el-input .el-input__password{color:var(--el-input-icon-color);font-size:14px;cursor:pointer}.el-input .el-input__clear:hover,.el-input .el-input__password:hover{color:var(--el-input-clear-hover-color)}.el-input .el-input__count{height:100%;display:inline-flex;align-items:center;color:var(--el-color-info);font-size:12px}.el-input .el-input__count .el-input__count-inner{background:var(--el-fill-color-blank);line-height:initial;display:inline-block;padding-left:8px}.el-input__wrapper{display:inline-flex;flex-grow:1;align-items:center;justify-content:center;padding:1px 11px;background-color:var(--el-input-bg-color,var(--el-fill-color-blank));background-image:none;border-radius:var(--el-input-border-radius,var(--el-border-radius-base));transition:var(--el-transition-box-shadow);box-shadow:0 0 0 1px var(--el-input-border-color,var(--el-border-color)) inset}.el-input__wrapper:hover{box-shadow:0 0 0 1px var(--el-input-hover-border-color) inset}.el-input__wrapper.is-focus{box-shadow:0 0 0 1px var(--el-input-focus-border-color) inset}.el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 32px) - 2px);width:100%;flex-grow:1;-webkit-appearance:none;color:var(--el-input-text-color,var(--el-text-color-regular));font-size:inherit;height:var(--el-input-inner-height);line-height:var(--el-input-inner-height);padding:0;outline:0;border:none;background:0 0;box-sizing:border-box}.el-input__inner:focus{outline:0}.el-input__inner::-moz-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner:-ms-input-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner::placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner[type=password]::-ms-reveal{display:none}.el-input__prefix{display:inline-flex;white-space:nowrap;flex-shrink:0;flex-wrap:nowrap;height:100%;text-align:center;color:var(--el-input-icon-color,var(--el-text-color-placeholder));transition:all var(--el-transition-duration);pointer-events:none}.el-input__prefix-inner{pointer-events:all;display:inline-flex;align-items:center;justify-content:center}.el-input__prefix-inner>:last-child{margin-right:8px}.el-input__prefix-inner>:first-child,.el-input__prefix-inner>:first-child.el-input__icon{margin-left:0}.el-input__suffix{display:inline-flex;white-space:nowrap;flex-shrink:0;flex-wrap:nowrap;height:100%;text-align:center;color:var(--el-input-icon-color,var(--el-text-color-placeholder));transition:all var(--el-transition-duration);pointer-events:none}.el-input__suffix-inner{pointer-events:all;display:inline-flex;align-items:center;justify-content:center}.el-input__suffix-inner>:first-child{margin-left:8px}.el-input .el-input__icon{height:inherit;line-height:inherit;display:flex;justify-content:center;align-items:center;transition:all var(--el-transition-duration);margin-left:8px}.el-input__validateIcon{pointer-events:none}.el-input.is-active .el-input__wrapper{box-shadow:0 0 0 1px var(--el-input-focus-color,) inset}.el-input.is-disabled{cursor:not-allowed}.el-input.is-disabled .el-input__wrapper{background-color:var(--el-disabled-bg-color);box-shadow:0 0 0 1px var(--el-disabled-border-color) inset}.el-input.is-disabled .el-input__inner{color:var(--el-disabled-text-color);-webkit-text-fill-color:var(--el-disabled-text-color);cursor:not-allowed}.el-input.is-disabled .el-input__inner::-moz-placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__inner:-ms-input-placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__inner::placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__icon{cursor:not-allowed}.el-input.is-exceed .el-input__wrapper{box-shadow:0 0 0 1px var(--el-color-danger) inset}.el-input.is-exceed .el-input__suffix .el-input__count{color:var(--el-color-danger)}.el-input--large{--el-input-height:var(--el-component-size-large);font-size:14px}.el-input--large .el-input__wrapper{padding:1px 15px}.el-input--large .el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 40px) - 2px)}.el-input--small{--el-input-height:var(--el-component-size-small);font-size:12px}.el-input--small .el-input__wrapper{padding:1px 7px}.el-input--small .el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 24px) - 2px)}.el-input-group{display:inline-flex;width:100%;align-items:stretch}.el-input-group__append,.el-input-group__prepend{background-color:var(--el-fill-color-light);color:var(--el-color-info);position:relative;display:inline-flex;align-items:center;justify-content:center;min-height:100%;border-radius:var(--el-input-border-radius);padding:0 20px;white-space:nowrap}.el-input-group__append:focus,.el-input-group__prepend:focus{outline:0}.el-input-group__append .el-button,.el-input-group__append .el-select,.el-input-group__prepend .el-button,.el-input-group__prepend .el-select{display:inline-block;margin:0 -20px}.el-input-group__append button.el-button,.el-input-group__append button.el-button:hover,.el-input-group__append div.el-select .el-input__wrapper,.el-input-group__append div.el-select:hover .el-input__wrapper,.el-input-group__prepend button.el-button,.el-input-group__prepend button.el-button:hover,.el-input-group__prepend div.el-select .el-input__wrapper,.el-input-group__prepend div.el-select:hover .el-input__wrapper{border-color:transparent;background-color:transparent;color:inherit}.el-input-group__append .el-button,.el-input-group__append .el-input,.el-input-group__prepend .el-button,.el-input-group__prepend .el-input{font-size:inherit}.el-input-group__prepend{border-right:0;border-top-right-radius:0;border-bottom-right-radius:0;box-shadow:1px 0 0 0 var(--el-input-border-color) inset,0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset}.el-input-group__append{border-left:0;border-top-left-radius:0;border-bottom-left-radius:0;box-shadow:0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset,-1px 0 0 0 var(--el-input-border-color) inset}.el-input-group--prepend>.el-input__wrapper{border-top-left-radius:0;border-bottom-left-radius:0}.el-input-group--prepend .el-input-group__prepend .el-select .el-input .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select .el-input .el-input__wrapper{border-top-right-radius:0;border-bottom-right-radius:0;box-shadow:1px 0 0 0 var(--el-input-border-color) inset,0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__wrapper{box-shadow:1px 0 0 0 var(--el-input-focus-border-color) inset,1px 0 0 0 var(--el-input-focus-border-color),0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important;z-index:2}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__wrapper:focus{outline:0;z-index:2;box-shadow:1px 0 0 0 var(--el-input-focus-border-color) inset,1px 0 0 0 var(--el-input-focus-border-color),0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important}.el-input-group--prepend .el-input-group__prepend .el-select:hover .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select:hover .el-input__wrapper{z-index:1;box-shadow:1px 0 0 0 var(--el-input-hover-border-color) inset,1px 0 0 0 var(--el-input-hover-border-color),0 1px 0 0 var(--el-input-hover-border-color) inset,0 -1px 0 0 var(--el-input-hover-border-color) inset!important}.el-input-group--append>.el-input__wrapper{border-top-right-radius:0;border-bottom-right-radius:0}.el-input-group--append .el-input-group__append .el-select .el-input .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select .el-input .el-input__wrapper{border-top-left-radius:0;border-bottom-left-radius:0;box-shadow:0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset,-1px 0 0 0 var(--el-input-border-color) inset}.el-input-group--append .el-input-group__append .el-select .el-input.is-focus .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select .el-input.is-focus .el-input__wrapper{z-index:2;box-shadow:-1px 0 0 0 var(--el-input-focus-border-color),-1px 0 0 0 var(--el-input-focus-border-color) inset,0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important}.el-input-group--append .el-input-group__append .el-select:hover .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select:hover .el-input__wrapper{z-index:1;box-shadow:-1px 0 0 0 var(--el-input-hover-border-color),-1px 0 0 0 var(--el-input-hover-border-color) inset,0 1px 0 0 var(--el-input-hover-border-color) inset,0 -1px 0 0 var(--el-input-hover-border-color) inset!important}.el-tag{--el-tag-font-size:12px;--el-tag-border-radius:4px;--el-tag-border-radius-rounded:9999px}.el-tag{--el-tag-bg-color:var(--el-color-primary-light-9);--el-tag-border-color:var(--el-color-primary-light-8);--el-tag-hover-color:var(--el-color-primary);--el-tag-text-color:var(--el-color-primary);background-color:var(--el-tag-bg-color);border-color:var(--el-tag-border-color);color:var(--el-tag-text-color);display:inline-flex;justify-content:center;align-items:center;height:24px;padding:0 9px;font-size:var(--el-tag-font-size);line-height:1;border-width:1px;border-style:solid;border-radius:var(--el-tag-border-radius);box-sizing:border-box;white-space:nowrap;--el-icon-size:14px}.el-tag.el-tag--primary{--el-tag-bg-color:var(--el-color-primary-light-9);--el-tag-border-color:var(--el-color-primary-light-8);--el-tag-hover-color:var(--el-color-primary)}.el-tag.el-tag--success{--el-tag-bg-color:var(--el-color-success-light-9);--el-tag-border-color:var(--el-color-success-light-8);--el-tag-hover-color:var(--el-color-success)}.el-tag.el-tag--warning{--el-tag-bg-color:var(--el-color-warning-light-9);--el-tag-border-color:var(--el-color-warning-light-8);--el-tag-hover-color:var(--el-color-warning)}.el-tag.el-tag--danger{--el-tag-bg-color:var(--el-color-danger-light-9);--el-tag-border-color:var(--el-color-danger-light-8);--el-tag-hover-color:var(--el-color-danger)}.el-tag.el-tag--error{--el-tag-bg-color:var(--el-color-error-light-9);--el-tag-border-color:var(--el-color-error-light-8);--el-tag-hover-color:var(--el-color-error)}.el-tag.el-tag--info{--el-tag-bg-color:var(--el-color-info-light-9);--el-tag-border-color:var(--el-color-info-light-8);--el-tag-hover-color:var(--el-color-info)}.el-tag.el-tag--primary{--el-tag-text-color:var(--el-color-primary)}.el-tag.el-tag--success{--el-tag-text-color:var(--el-color-success)}.el-tag.el-tag--warning{--el-tag-text-color:var(--el-color-warning)}.el-tag.el-tag--danger{--el-tag-text-color:var(--el-color-danger)}.el-tag.el-tag--error{--el-tag-text-color:var(--el-color-error)}.el-tag.el-tag--info{--el-tag-text-color:var(--el-color-info)}.el-tag.is-hit{border-color:var(--el-color-primary)}.el-tag.is-round{border-radius:var(--el-tag-border-radius-rounded)}.el-tag .el-tag__close{color:var(--el-tag-text-color)}.el-tag .el-tag__close:hover{color:var(--el-color-white);background-color:var(--el-tag-hover-color)}.el-tag .el-icon{border-radius:50%;cursor:pointer;font-size:calc(var(--el-icon-size) - 2px);height:var(--el-icon-size);width:var(--el-icon-size)}.el-tag .el-tag__close{margin-left:6px}.el-tag--dark{--el-tag-bg-color:var(--el-color-primary);--el-tag-border-color:var(--el-color-primary);--el-tag-hover-color:var(--el-color-primary-light-3);--el-tag-text-color:var(--el-color-white)}.el-tag--dark.el-tag--primary{--el-tag-bg-color:var(--el-color-primary);--el-tag-border-color:var(--el-color-primary);--el-tag-hover-color:var(--el-color-primary-light-3)}.el-tag--dark.el-tag--success{--el-tag-bg-color:var(--el-color-success);--el-tag-border-color:var(--el-color-success);--el-tag-hover-color:var(--el-color-success-light-3)}.el-tag--dark.el-tag--warning{--el-tag-bg-color:var(--el-color-warning);--el-tag-border-color:var(--el-color-warning);--el-tag-hover-color:var(--el-color-warning-light-3)}.el-tag--dark.el-tag--danger{--el-tag-bg-color:var(--el-color-danger);--el-tag-border-color:var(--el-color-danger);--el-tag-hover-color:var(--el-color-danger-light-3)}.el-tag--dark.el-tag--error{--el-tag-bg-color:var(--el-color-error);--el-tag-border-color:var(--el-color-error);--el-tag-hover-color:var(--el-color-error-light-3)}.el-tag--dark.el-tag--info{--el-tag-bg-color:var(--el-color-info);--el-tag-border-color:var(--el-color-info);--el-tag-hover-color:var(--el-color-info-light-3)}.el-tag--dark.el-tag--primary,.el-tag--dark.el-tag--success,.el-tag--dark.el-tag--warning,.el-tag--dark.el-tag--danger,.el-tag--dark.el-tag--error,.el-tag--dark.el-tag--info{--el-tag-text-color:var(--el-color-white)}.el-tag--plain{--el-tag-border-color:var(--el-color-primary-light-5);--el-tag-hover-color:var(--el-color-primary);--el-tag-bg-color:var(--el-fill-color-blank)}.el-tag--plain.el-tag--primary{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-primary-light-5);--el-tag-hover-color:var(--el-color-primary)}.el-tag--plain.el-tag--success{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-success-light-5);--el-tag-hover-color:var(--el-color-success)}.el-tag--plain.el-tag--warning{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-warning-light-5);--el-tag-hover-color:var(--el-color-warning)}.el-tag--plain.el-tag--danger{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-danger-light-5);--el-tag-hover-color:var(--el-color-danger)}.el-tag--plain.el-tag--error{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-error-light-5);--el-tag-hover-color:var(--el-color-error)}.el-tag--plain.el-tag--info{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-info-light-5);--el-tag-hover-color:var(--el-color-info)}.el-tag.is-closable{padding-right:5px}.el-tag--large{padding:0 11px;height:32px;--el-icon-size:16px}.el-tag--large .el-tag__close{margin-left:8px}.el-tag--large.is-closable{padding-right:7px}.el-tag--small{padding:0 7px;height:20px;--el-icon-size:12px}.el-tag--small .el-tag__close{margin-left:4px}.el-tag--small.is-closable{padding-right:3px}.el-tag--small .el-icon-close{transform:scale(.8)}.el-tag.el-tag--primary.is-hit{border-color:var(--el-color-primary)}.el-tag.el-tag--success.is-hit{border-color:var(--el-color-success)}.el-tag.el-tag--warning.is-hit{border-color:var(--el-color-warning)}.el-tag.el-tag--danger.is-hit{border-color:var(--el-color-danger)}.el-tag.el-tag--error.is-hit{border-color:var(--el-color-error)}.el-tag.el-tag--info.is-hit{border-color:var(--el-color-info)}.el-scrollbar{--el-scrollbar-opacity:.3;--el-scrollbar-bg-color:var(--el-text-color-secondary);--el-scrollbar-hover-opacity:.5;--el-scrollbar-hover-bg-color:var(--el-text-color-secondary)}.el-scrollbar{overflow:hidden;position:relative;height:100%}.el-scrollbar__wrap{overflow:auto;height:100%}.el-scrollbar__wrap--hidden-default{scrollbar-width:none}.el-scrollbar__wrap--hidden-default::-webkit-scrollbar{display:none}.el-scrollbar__thumb{position:relative;display:block;width:0;height:0;cursor:pointer;border-radius:inherit;background-color:var(--el-scrollbar-bg-color,var(--el-text-color-secondary));transition:var(--el-transition-duration) background-color;opacity:var(--el-scrollbar-opacity,.3)}.el-scrollbar__thumb:hover{background-color:var(--el-scrollbar-hover-bg-color,var(--el-text-color-secondary));opacity:var(--el-scrollbar-hover-opacity,.5)}.el-scrollbar__bar{position:absolute;right:2px;bottom:2px;z-index:1;border-radius:4px}.el-scrollbar__bar.is-vertical{width:6px;top:2px}.el-scrollbar__bar.is-vertical>div{width:100%}.el-scrollbar__bar.is-horizontal{height:6px;left:2px}.el-scrollbar__bar.is-horizontal>div{height:100%}.el-scrollbar-fade-enter-active{transition:opacity .34s ease-out}.el-scrollbar-fade-leave-active{transition:opacity .12s ease-out}.el-scrollbar-fade-enter-from,.el-scrollbar-fade-leave-active{opacity:0}.el-popper{--el-popper-border-radius:var(--el-popover-border-radius, 4px)}.el-popper{position:absolute;border-radius:var(--el-popper-border-radius);padding:5px 11px;z-index:2000;font-size:12px;line-height:20px;min-width:10px;word-wrap:break-word;visibility:visible}.el-popper.is-dark{color:var(--el-bg-color);background:var(--el-text-color-primary);border:1px solid var(--el-text-color-primary)}.el-popper.is-dark .el-popper__arrow:before{border:1px solid var(--el-text-color-primary);background:var(--el-text-color-primary);right:0}.el-popper.is-light{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light)}.el-popper.is-light .el-popper__arrow:before{border:1px solid var(--el-border-color-light);background:var(--el-bg-color-overlay);right:0}.el-popper.is-pure{padding:0}.el-popper__arrow{position:absolute;width:10px;height:10px;z-index:-1}.el-popper__arrow:before{position:absolute;width:10px;height:10px;z-index:-1;content:" ";transform:rotate(45deg);background:var(--el-text-color-primary);box-sizing:border-box}.el-popper[data-popper-placement^=top]>.el-popper__arrow{bottom:-5px}.el-popper[data-popper-placement^=top]>.el-popper__arrow:before{border-bottom-right-radius:2px}.el-popper[data-popper-placement^=bottom]>.el-popper__arrow{top:-5px}.el-popper[data-popper-placement^=bottom]>.el-popper__arrow:before{border-top-left-radius:2px}.el-popper[data-popper-placement^=left]>.el-popper__arrow{right:-5px}.el-popper[data-popper-placement^=left]>.el-popper__arrow:before{border-top-right-radius:2px}.el-popper[data-popper-placement^=right]>.el-popper__arrow{left:-5px}.el-popper[data-popper-placement^=right]>.el-popper__arrow:before{border-bottom-left-radius:2px}.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent!important;border-left-color:transparent!important}.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent!important;border-right-color:transparent!important}.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent!important;border-bottom-color:transparent!important}.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent!important;border-top-color:transparent!important}.el-vl__wrapper{position:relative}.el-vl__wrapper:hover .el-virtual-scrollbar,.el-vl__wrapper.always-on .el-virtual-scrollbar{opacity:1}.el-vl__window{scrollbar-width:none}.el-vl__window::-webkit-scrollbar{display:none}.el-virtual-scrollbar{opacity:0;transition:opacity .34s ease-out}.el-virtual-scrollbar.always-on{opacity:1}.el-vg__wrapper{position:relative}.el-select-dropdown__option-item.is-selected:not(.is-multiple).is-disabled{color:var(--el-text-color-disabled)}.el-select-dropdown__option-item.is-selected:not(.is-multiple).is-disabled:after{background-color:var(--el-text-color-disabled)}.el-select-dropdown__option-item:hover:not(.hover){background-color:transparent}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-disabled.is-selected{color:var(--el-text-color-disabled)}.el-select-dropdown__list{list-style:none;margin:6px 0!important;padding:0!important;box-sizing:border-box}.el-select-dropdown__option-item{font-size:var(--el-select-font-size);padding:0 32px 0 20px;position:relative;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--el-text-color-regular);height:34px;line-height:34px;box-sizing:border-box;cursor:pointer}.el-select-dropdown__option-item.is-disabled{color:var(--el-text-color-placeholder);cursor:not-allowed}.el-select-dropdown__option-item.is-disabled:hover{background-color:var(--el-bg-color)}.el-select-dropdown__option-item.is-selected{background-color:var(--el-fill-color-light);font-weight:700}.el-select-dropdown__option-item.is-selected:not(.is-multiple){color:var(--el-color-primary)}.el-select-dropdown__option-item.hover{background-color:var(--el-fill-color-light)!important}.el-select-dropdown__option-item:hover{background-color:var(--el-fill-color-light)}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay)}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected .el-icon{position:absolute;right:20px;top:0;height:inherit;font-size:12px}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected .el-icon svg{height:inherit;vertical-align:middle}.el-select-v2{--el-select-border-color-hover:var(--el-border-color-hover);--el-select-disabled-border:var(--el-disabled-border-color);--el-select-font-size:var(--el-font-size-base);--el-select-close-hover-color:var(--el-text-color-secondary);--el-select-input-color:var(--el-text-color-placeholder);--el-select-multiple-input-color:var(--el-text-color-regular);--el-select-input-focus-border-color:var(--el-color-primary);--el-select-input-font-size:14px}.el-select-v2{display:inline-block;position:relative;vertical-align:middle;font-size:14px}.el-select-v2__wrapper{display:flex;align-items:center;flex-wrap:wrap;position:relative;box-sizing:border-box;cursor:pointer;padding:1px 30px 1px 0;border:1px solid var(--el-border-color);border-radius:var(--el-border-radius-base);background-color:var(--el-fill-color-blank);transition:var(--el-transition-duration)}.el-select-v2__wrapper:hover{border-color:var(--el-text-color-placeholder)}.el-select-v2__wrapper.is-filterable{cursor:text}.el-select-v2__wrapper.is-focused{border-color:var(--el-color-primary)}.el-select-v2__wrapper.is-hovering:not(.is-focused){border-color:var(--el-border-color-hover)}.el-select-v2__wrapper.is-disabled{cursor:not-allowed;background-color:var(--el-fill-color-light);color:var(--el-text-color-placeholder);border-color:var(--el-select-disabled-border)}.el-select-v2__wrapper.is-disabled:hover{border-color:var(--el-select-disabled-border)}.el-select-v2__wrapper.is-disabled.is-focus{border-color:var(--el-input-focus-border-color)}.el-select-v2__wrapper.is-disabled .is-transparent{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-select-v2__wrapper.is-disabled .el-select-v2__caret,.el-select-v2__wrapper.is-disabled .el-select-v2__combobox-input{cursor:not-allowed}.el-select-v2__wrapper .el-select-v2__input-wrapper{box-sizing:border-box;position:relative;-webkit-margin-start:12px;margin-inline-start:12px;max-width:100%;overflow:hidden}.el-select-v2__wrapper,.el-select-v2__wrapper .el-select-v2__input-wrapper{line-height:32px}.el-select-v2__wrapper .el-select-v2__input-wrapper input{--el-input-inner-height:calc(var(--el-component-size, 32px) - 8px);height:var(--el-input-inner-height);line-height:var(--el-input-inner-height);min-width:4px;width:100%;background-color:transparent;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:0 0;border:none;margin:2px 0;outline:0;padding:0}.el-select-v2 .el-select-v2__tags-text{display:inline-block;line-height:normal;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-select-v2__empty{padding:10px 0;margin:0;text-align:center;color:var(--el-text-color-secondary);font-size:14px}.el-select-v2__popper.el-popper{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light);box-shadow:var(--el-box-shadow-light)}.el-select-v2__popper.el-popper .el-popper__arrow:before{border:1px solid var(--el-border-color-light)}.el-select-v2__popper.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent;border-left-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent;border-right-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent;border-bottom-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent;border-top-color:transparent}.el-select-v2--large .el-select-v2__wrapper .el-select-v2__combobox-input{height:32px}.el-select-v2--large .el-select-v2__caret,.el-select-v2--large .el-select-v2__suffix{height:40px}.el-select-v2--large .el-select-v2__placeholder{font-size:14px;line-height:40px}.el-select-v2--small .el-select-v2__wrapper .el-select-v2__combobox-input{height:16px}.el-select-v2--small .el-select-v2__caret,.el-select-v2--small .el-select-v2__suffix{height:24px}.el-select-v2--small .el-select-v2__placeholder{font-size:12px;line-height:24px}.el-select-v2 .el-select-v2__selection>span{display:inline-block}.el-select-v2:hover .el-select-v2__combobox-input{border-color:var(--el-select-border-color-hover)}.el-select-v2 .el-select__selection-text{text-overflow:ellipsis;display:inline-block;overflow-x:hidden;vertical-align:bottom}.el-select-v2 .el-select-v2__combobox-input{padding-right:35px;display:block;color:var(--el-text-color-regular)}.el-select-v2 .el-select-v2__combobox-input:focus{border-color:var(--el-select-input-focus-border-color)}.el-select-v2__input{border:none;outline:0;padding:0;margin-left:15px;color:var(--el-select-multiple-input-color);font-size:var(--el-select-font-size);-webkit-appearance:none;-moz-appearance:none;appearance:none;height:28px}.el-select-v2__input.is-small{height:14px}.el-select-v2__close{cursor:pointer;position:absolute;top:8px;z-index:var(--el-index-top);right:25px;color:var(--el-select-input-color);line-height:18px;font-size:var(--el-select-input-font-size)}.el-select-v2__close:hover{color:var(--el-select-close-hover-color)}.el-select-v2__suffix{display:inline-flex;position:absolute;right:12px;height:32px;top:50%;transform:translateY(-50%);color:var(--el-input-icon-color,var(--el-text-color-placeholder))}.el-select-v2__suffix .el-input__icon{height:inherit}.el-select-v2__caret{color:var(--el-select-input-color);font-size:var(--el-select-input-font-size);transition:var(--el-transition-duration);transform:rotate(180deg);cursor:pointer}.el-select-v2__caret.is-reverse{transform:rotate(0)}.el-select-v2__caret.is-show-close{font-size:var(--el-select-font-size);text-align:center;transform:rotate(180deg);border-radius:var(--el-border-radius-circle);color:var(--el-select-input-color);transition:var(--el-transition-color)}.el-select-v2__caret.is-show-close:hover{color:var(--el-select-close-hover-color)}.el-select-v2__caret.el-icon{height:inherit}.el-select-v2__caret.el-icon svg{vertical-align:middle}.el-select-v2__selection{white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap}.el-select-v2__input-calculator{left:0;position:absolute;top:0;visibility:hidden;white-space:pre;z-index:999}.el-select-v2__selected-item{line-height:inherit;height:inherit;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;display:flex;flex-wrap:wrap}.el-select-v2__placeholder{position:absolute;top:50%;transform:translateY(-50%);-webkit-margin-start:12px;margin-inline-start:12px;width:calc(100% - 52px);overflow:hidden;text-overflow:ellipsis;white-space:nowrap;color:var(--el-input-text-color,var(--el-text-color-regular))}.el-select-v2__placeholder.is-transparent{color:var(--el-text-color-placeholder)}.el-select-v2 .el-select-v2__selection .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 0 2px 6px;background-color:var(--el-fill-color)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;color:var(--el-color-white)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select-v2.el-select-v2--small .el-select-v2__selection .el-tag{margin:1px 0 1px 6px;height:18px}.el-select-dropdown__item{font-size:var(--el-font-size-base);padding:0 32px 0 20px;position:relative;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--el-text-color-regular);height:34px;line-height:34px;box-sizing:border-box;cursor:pointer}.el-select-dropdown__item.is-disabled{color:var(--el-text-color-placeholder);cursor:not-allowed}.el-select-dropdown__item.hover,.el-select-dropdown__item:hover{background-color:var(--el-fill-color-light)}.el-select-dropdown__item.selected{color:var(--el-color-primary);font-weight:700}.el-select-group{margin:0;padding:0}.el-select-group__wrap{position:relative;list-style:none;margin:0;padding:0}.el-select-group__wrap:not(:last-of-type){padding-bottom:24px}.el-select-group__wrap:not(:last-of-type):after{content:"";position:absolute;display:block;left:20px;right:20px;bottom:12px;height:1px;background:var(--el-border-color-light)}.el-select-group__split-dash{position:absolute;left:20px;right:20px;height:1px;background:var(--el-border-color-light)}.el-select-group__title{padding-left:20px;font-size:12px;color:var(--el-color-info);line-height:30px}.el-select-group .el-select-dropdown__item{padding-left:20px}.el-select-dropdown{z-index:calc(var(--el-index-top) + 1);border-radius:var(--el-border-radius-base);box-sizing:border-box}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay)}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected.hover{background-color:var(--el-fill-color-light)}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected:after{content:"";position:absolute;top:50%;right:20px;border-top:none;border-right:none;background-repeat:no-repeat;background-position:center;background-color:var(--el-color-primary);-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask-size:100% 100%;-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;-webkit-mask-size:100% 100%;transform:translateY(-50%);width:12px;height:12px}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected.is-disabled:after{background-color:var(--el-text-color-disabled)}.el-select-dropdown .el-select-dropdown__option-item.is-selected:after{content:"";position:absolute;top:50%;right:20px;border-top:none;border-right:none;background-repeat:no-repeat;background-position:center;background-color:var(--el-color-primary);-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask-size:100% 100%;-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;-webkit-mask-size:100% 100%;transform:translateY(-50%);width:12px;height:12px}.el-select-dropdown .el-scrollbar.is-empty .el-select-dropdown__list{padding:0}.el-select-dropdown .el-select-dropdown__item.is-disabled:hover{background-color:unset}.el-select-dropdown .el-select-dropdown__item.is-disabled.selected{color:var(--el-text-color-disabled)}.el-select-dropdown__empty{padding:10px 0;margin:0;text-align:center;color:var(--el-text-color-secondary);font-size:var(--el-select-font-size)}.el-select-dropdown__wrap{max-height:274px}.el-select-dropdown__list{list-style:none;padding:6px 0;margin:0;box-sizing:border-box}.el-select{--el-select-border-color-hover:var(--el-border-color-hover);--el-select-disabled-border:var(--el-disabled-border-color);--el-select-font-size:var(--el-font-size-base);--el-select-close-hover-color:var(--el-text-color-secondary);--el-select-input-color:var(--el-text-color-placeholder);--el-select-multiple-input-color:var(--el-text-color-regular);--el-select-input-focus-border-color:var(--el-color-primary);--el-select-input-font-size:14px}.el-select{display:inline-block;position:relative;vertical-align:middle;line-height:32px}.el-select__popper.el-popper{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light);box-shadow:var(--el-box-shadow-light)}.el-select__popper.el-popper .el-popper__arrow:before{border:1px solid var(--el-border-color-light)}.el-select__popper.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent;border-left-color:transparent}.el-select__popper.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent;border-right-color:transparent}.el-select__popper.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent;border-bottom-color:transparent}.el-select__popper.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent;border-top-color:transparent}.el-select .el-select-tags-wrapper.has-prefix{margin-left:6px}.el-select--large{line-height:40px}.el-select--large .el-select-tags-wrapper.has-prefix{margin-left:8px}.el-select--small{line-height:24px}.el-select--small .el-select-tags-wrapper.has-prefix{margin-left:4px}.el-select .el-select__tags>span{display:inline-block}.el-select:hover:not(.el-select--disabled) .el-input__wrapper{box-shadow:0 0 0 1px var(--el-select-border-color-hover) inset}.el-select .el-select__tags-text{display:inline-block;line-height:normal;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-select .el-input__wrapper{cursor:pointer}.el-select .el-input__wrapper.is-focus{box-shadow:0 0 0 1px var(--el-select-input-focus-border-color) inset!important}.el-select .el-input__inner{cursor:pointer}.el-select .el-input{display:flex}.el-select .el-input .el-select__caret{color:var(--el-select-input-color);font-size:var(--el-select-input-font-size);transition:transform var(--el-transition-duration);transform:rotate(0);cursor:pointer}.el-select .el-input .el-select__caret.is-reverse{transform:rotate(-180deg)}.el-select .el-input .el-select__caret.is-show-close{font-size:var(--el-select-font-size);text-align:center;transform:rotate(0);border-radius:var(--el-border-radius-circle);color:var(--el-select-input-color);transition:var(--el-transition-color)}.el-select .el-input .el-select__caret.is-show-close:hover{color:var(--el-select-close-hover-color)}.el-select .el-input .el-select__caret.el-icon{position:relative;height:inherit;z-index:2}.el-select .el-input.is-disabled .el-input__wrapper{cursor:not-allowed}.el-select .el-input.is-disabled .el-input__wrapper:hover{box-shadow:0 0 0 1px var(--el-select-disabled-border) inset}.el-select .el-input.is-disabled .el-input__inner,.el-select .el-input.is-disabled .el-select__caret{cursor:not-allowed}.el-select .el-input.is-focus .el-input__wrapper{box-shadow:0 0 0 1px var(--el-select-input-focus-border-color) inset!important}.el-select__input{border:none;outline:0;padding:0;margin-left:15px;color:var(--el-select-multiple-input-color);font-size:var(--el-select-font-size);-webkit-appearance:none;-moz-appearance:none;appearance:none;height:28px;background-color:transparent}.el-select__input.is-small{height:14px}.el-select__close{cursor:pointer;position:absolute;top:8px;z-index:var(--el-index-top);right:25px;color:var(--el-select-input-color);line-height:18px;font-size:var(--el-select-input-font-size)}.el-select__close:hover{color:var(--el-select-close-hover-color)}.el-select__tags{position:absolute;line-height:normal;top:50%;transform:translateY(-50%);white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap;cursor:pointer}.el-select__tags .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 6px 2px 0}.el-select__tags .el-tag:last-child{margin-right:0}.el-select__tags .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;top:0;color:#fff}.el-select__tags .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select__tags .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select__tags .el-tag--info{background-color:var(--el-fill-color)}.el-select__collapse-tags{white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap;cursor:pointer}.el-select__collapse-tags .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 6px 2px 0}.el-select__collapse-tags .el-tag:last-child{margin-right:0}.el-select__collapse-tags .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;top:0;color:#fff}.el-select__collapse-tags .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select__collapse-tags .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select__collapse-tags .el-tag--info{background-color:var(--el-fill-color)}.el-select__collapse-tag{line-height:inherit;height:inherit;display:flex}.slicer-box[data-v-ba3d65d0]{margin-right:.8rem}.slicer-box .cp-select[data-v-ba3d65d0]{min-width:11rem}.slicer-box .title[data-v-ba3d65d0]{display:block;margin-bottom:.5rem}.el-pagination{--el-pagination-font-size:14px;--el-pagination-bg-color:var(--el-fill-color-blank);--el-pagination-text-color:var(--el-text-color-primary);--el-pagination-border-radius:2px;--el-pagination-button-color:var(--el-text-color-primary);--el-pagination-button-width:32px;--el-pagination-button-height:32px;--el-pagination-button-disabled-color:var(--el-text-color-placeholder);--el-pagination-button-disabled-bg-color:var(--el-fill-color-blank);--el-pagination-button-bg-color:var(--el-fill-color);--el-pagination-hover-color:var(--el-color-primary);--el-pagination-font-size-small:12px;--el-pagination-button-width-small:24px;--el-pagination-button-height-small:24px;--el-pagination-item-gap:16px;white-space:nowrap;color:var(--el-pagination-text-color);font-size:var(--el-pagination-font-size);font-weight:400;display:flex;align-items:center}.el-pagination .el-input__inner{text-align:center;-moz-appearance:textfield}.el-pagination .el-select .el-input{width:128px}.el-pagination button{display:flex;justify-content:center;align-items:center;font-size:var(--el-pagination-font-size);min-width:var(--el-pagination-button-width);height:var(--el-pagination-button-height);line-height:var(--el-pagination-button-height);color:var(--el-pagination-button-color);background:var(--el-pagination-bg-color);padding:0 4px;border:none;border-radius:var(--el-pagination-border-radius);cursor:pointer;text-align:center;box-sizing:border-box}.el-pagination button *{pointer-events:none}.el-pagination button:focus{outline:0}.el-pagination button:hover{color:var(--el-pagination-hover-color)}.el-pagination button.is-active{color:var(--el-pagination-hover-color);cursor:default;font-weight:700}.el-pagination button.is-active.is-disabled{font-weight:700;color:var(--el-text-color-secondary)}.el-pagination button.is-disabled,.el-pagination button:disabled{color:var(--el-pagination-button-disabled-color);background-color:var(--el-pagination-button-disabled-bg-color);cursor:not-allowed}.el-pagination button:focus-visible{outline:1px solid var(--el-pagination-hover-color);outline-offset:-1px}.el-pagination .btn-next .el-icon,.el-pagination .btn-prev .el-icon{display:block;font-size:12px;font-weight:700;width:inherit}.el-pagination>.is-first{margin-left:0!important}.el-pagination>.is-last{margin-right:0!important}.el-pagination .btn-prev{margin-left:var(--el-pagination-item-gap)}.el-pagination__sizes,.el-pagination__total{margin-left:var(--el-pagination-item-gap);font-weight:400;color:var(--el-text-color-regular)}.el-pagination__total[disabled=true]{color:var(--el-text-color-placeholder)}.el-pagination__jump{display:flex;align-items:center;margin-left:var(--el-pagination-item-gap);font-weight:400;color:var(--el-text-color-regular)}.el-pagination__jump[disabled=true]{color:var(--el-text-color-placeholder)}.el-pagination__goto{margin-right:8px}.el-pagination__editor{text-align:center;box-sizing:border-box}.el-pagination__editor.el-input{width:56px}.el-pagination__editor .el-input__inner::-webkit-inner-spin-button,.el-pagination__editor .el-input__inner::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.el-pagination__classifier{margin-left:8px}.el-pagination__rightwrapper{flex:1;display:flex;align-items:center;justify-content:flex-end}.el-pagination.is-background .btn-next,.el-pagination.is-background .btn-prev,.el-pagination.is-background .el-pager li{margin:0 4px;background-color:var(--el-pagination-button-bg-color)}.el-pagination.is-background .btn-next.is-active,.el-pagination.is-background .btn-prev.is-active,.el-pagination.is-background .el-pager li.is-active{background-color:var(--el-color-primary);color:var(--el-color-white)}.el-pagination.is-background .btn-next.is-disabled,.el-pagination.is-background .btn-next:disabled,.el-pagination.is-background .btn-prev.is-disabled,.el-pagination.is-background .btn-prev:disabled,.el-pagination.is-background .el-pager li.is-disabled,.el-pagination.is-background .el-pager li:disabled{color:var(--el-text-color-placeholder);background-color:var(--el-disabled-bg-color)}.el-pagination.is-background .btn-next.is-disabled.is-active,.el-pagination.is-background .btn-next:disabled.is-active,.el-pagination.is-background .btn-prev.is-disabled.is-active,.el-pagination.is-background .btn-prev:disabled.is-active,.el-pagination.is-background .el-pager li.is-disabled.is-active,.el-pagination.is-background .el-pager li:disabled.is-active{color:var(--el-text-color-secondary);background-color:var(--el-fill-color-dark)}.el-pagination.is-background .btn-prev{margin-left:var(--el-pagination-item-gap)}.el-pagination--small .btn-next,.el-pagination--small .btn-prev,.el-pagination--small .el-pager li{height:var(--el-pagination-button-height-small);line-height:var(--el-pagination-button-height-small);font-size:var(--el-pagination-font-size-small);min-width:var(--el-pagination-button-width-small)}.el-pagination--small button,.el-pagination--small span:not([class*=suffix]){font-size:var(--el-pagination-font-size-small)}.el-pagination--small .el-select .el-input{width:100px}.el-pager{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;list-style:none;font-size:0;padding:0;margin:0;display:flex;align-items:center}.el-pager li{display:flex;justify-content:center;align-items:center;font-size:var(--el-pagination-font-size);min-width:var(--el-pagination-button-width);height:var(--el-pagination-button-height);line-height:var(--el-pagination-button-height);color:var(--el-pagination-button-color);background:var(--el-pagination-bg-color);padding:0 4px;border:none;border-radius:var(--el-pagination-border-radius);cursor:pointer;text-align:center;box-sizing:border-box}.el-pager li *{pointer-events:none}.el-pager li:focus{outline:0}.el-pager li:hover{color:var(--el-pagination-hover-color)}.el-pager li.is-active{color:var(--el-pagination-hover-color);cursor:default;font-weight:700}.el-pager li.is-active.is-disabled{font-weight:700;color:var(--el-text-color-secondary)}.el-pager li.is-disabled,.el-pager li:disabled{color:var(--el-pagination-button-disabled-color);background-color:var(--el-pagination-button-disabled-bg-color);cursor:not-allowed}.el-pager li:focus-visible{outline:1px solid var(--el-pagination-hover-color);outline-offset:-1px}.el-table{--el-table-border-color:var(--el-border-color-lighter);--el-table-border:1px solid var(--el-table-border-color);--el-table-text-color:var(--el-text-color-regular);--el-table-header-text-color:var(--el-text-color-secondary);--el-table-row-hover-bg-color:var(--el-fill-color-light);--el-table-current-row-bg-color:var(--el-color-primary-light-9);--el-table-header-bg-color:var(--el-bg-color);--el-table-fixed-box-shadow:var(--el-box-shadow-light);--el-table-bg-color:var(--el-fill-color-blank);--el-table-tr-bg-color:var(--el-fill-color-blank);--el-table-expanded-cell-bg-color:var(--el-fill-color-blank);--el-table-fixed-left-column:inset 10px 0 10px -10px rgba(0, 0, 0, .15);--el-table-fixed-right-column:inset -10px 0 10px -10px rgba(0, 0, 0, .15)}.el-table{position:relative;overflow:hidden;box-sizing:border-box;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;width:100%;max-width:100%;background-color:var(--el-table-bg-color);font-size:14px;color:var(--el-table-text-color)}.el-table__inner-wrapper{position:relative;display:flex;flex-direction:column;height:100%}.el-table__inner-wrapper:before{left:0;bottom:0;width:100%;height:1px}.el-table.has-footer.el-table--fluid-height tr:last-child td.el-table__cell,.el-table.has-footer.el-table--scrollable-y tr:last-child td.el-table__cell{border-bottom-color:transparent}.el-table__empty-block{position:-webkit-sticky;position:sticky;left:0;min-height:60px;text-align:center;width:100%;display:flex;justify-content:center;align-items:center}.el-table__empty-text{line-height:60px;width:50%;color:var(--el-text-color-secondary)}.el-table__expand-column .cell{padding:0;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-table__expand-icon{position:relative;cursor:pointer;color:var(--el-text-color-regular);font-size:12px;transition:transform var(--el-transition-duration-fast) ease-in-out;height:20px}.el-table__expand-icon--expanded{transform:rotate(90deg)}.el-table__expand-icon>.el-icon{font-size:12px}.el-table__expanded-cell{background-color:var(--el-table-expanded-cell-bg-color)}.el-table__expanded-cell[class*=cell]{padding:20px 50px}.el-table__expanded-cell:hover{background-color:transparent!important}.el-table__placeholder{display:inline-block;width:20px}.el-table__append-wrapper{overflow:hidden}.el-table--fit{border-right:0;border-bottom:0}.el-table--fit .el-table__cell.gutter{border-right-width:1px}.el-table thead{color:var(--el-table-header-text-color);font-weight:500}.el-table thead.is-group th.el-table__cell{background:var(--el-fill-color-light)}.el-table .el-table__cell{padding:8px 0;min-width:0;box-sizing:border-box;text-overflow:ellipsis;vertical-align:middle;position:relative;text-align:left;z-index:1}.el-table .el-table__cell.is-center{text-align:center}.el-table .el-table__cell.is-right{text-align:right}.el-table .el-table__cell.gutter{width:15px;border-right-width:0;border-bottom-width:0;padding:0}.el-table .el-table__cell.is-hidden>*{visibility:hidden}.el-table .cell{box-sizing:border-box;overflow:hidden;text-overflow:ellipsis;white-space:normal;word-break:break-all;line-height:23px;padding:0 12px}.el-table .cell.el-tooltip{white-space:nowrap;min-width:50px}.el-table--large{font-size:var(--el-font-size-base)}.el-table--large .el-table__cell{padding:12px 0}.el-table--large .cell{padding:0 16px}.el-table--default{font-size:14px}.el-table--default .el-table__cell{padding:8px 0}.el-table--default .cell{padding:0 12px}.el-table--small{font-size:12px}.el-table--small .el-table__cell{padding:4px 0}.el-table--small .cell{padding:0 8px}.el-table tr{background-color:var(--el-table-tr-bg-color)}.el-table tr input[type=checkbox]{margin:0}.el-table td.el-table__cell,.el-table th.el-table__cell.is-leaf{border-bottom:var(--el-table-border)}.el-table th.el-table__cell.is-sortable{cursor:pointer}.el-table th.el-table__cell{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-color:var(--el-table-header-bg-color)}.el-table th.el-table__cell>.cell.highlight{color:var(--el-color-primary)}.el-table th.el-table__cell.required>div:before{display:inline-block;content:"";width:8px;height:8px;border-radius:50%;background:#ff4d51;margin-right:5px;vertical-align:middle}.el-table td.el-table__cell div{box-sizing:border-box}.el-table td.el-table__cell.gutter{width:0}.el-table__footer-wrapper{border-top:var(--el-table-border)}.el-table--border .el-table__inner-wrapper:after,.el-table--border:after,.el-table--border:before,.el-table__inner-wrapper:before{content:"";position:absolute;background-color:var(--el-table-border-color);z-index:3}.el-table--border .el-table__inner-wrapper:after{left:0;top:0;width:100%;height:1px}.el-table--border:before{top:-1px;left:0;width:1px;height:100%}.el-table--border:after{top:-1px;right:0;width:1px;height:100%}.el-table--border .el-table__inner-wrapper{border-right:none;border-bottom:none}.el-table--border .el-table__footer-wrapper{position:relative;flex-shrink:0}.el-table--border .el-table__cell{border-right:var(--el-table-border)}.el-table--border th.el-table__cell.gutter:last-of-type{border-bottom:var(--el-table-border);border-bottom-width:1px}.el-table--border th.el-table__cell{border-bottom:var(--el-table-border)}.el-table--hidden{visibility:hidden}.el-table__body-wrapper,.el-table__footer-wrapper,.el-table__header-wrapper{width:100%}.el-table__body-wrapper tr td.el-table-fixed-column--left,.el-table__body-wrapper tr td.el-table-fixed-column--right,.el-table__body-wrapper tr th.el-table-fixed-column--left,.el-table__body-wrapper tr th.el-table-fixed-column--right,.el-table__footer-wrapper tr td.el-table-fixed-column--left,.el-table__footer-wrapper tr td.el-table-fixed-column--right,.el-table__footer-wrapper tr th.el-table-fixed-column--left,.el-table__footer-wrapper tr th.el-table-fixed-column--right,.el-table__header-wrapper tr td.el-table-fixed-column--left,.el-table__header-wrapper tr td.el-table-fixed-column--right,.el-table__header-wrapper tr th.el-table-fixed-column--left,.el-table__header-wrapper tr th.el-table-fixed-column--right{position:-webkit-sticky!important;position:sticky!important;z-index:2;background:var(--el-bg-color)}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-last-column:before{content:"";position:absolute;top:0;width:10px;bottom:-1px;overflow-x:hidden;overflow-y:hidden;box-shadow:none;touch-action:none;pointer-events:none}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-first-column:before{left:-10px}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-last-column:before{right:-10px;box-shadow:none}.el-table__body-wrapper tr td.el-table__fixed-right-patch,.el-table__body-wrapper tr th.el-table__fixed-right-patch,.el-table__footer-wrapper tr td.el-table__fixed-right-patch,.el-table__footer-wrapper tr th.el-table__fixed-right-patch,.el-table__header-wrapper tr td.el-table__fixed-right-patch,.el-table__header-wrapper tr th.el-table__fixed-right-patch{position:-webkit-sticky!important;position:sticky!important;z-index:2;background:#fff;right:0}.el-table__header-wrapper{flex-shrink:0}.el-table__header-wrapper tr th.el-table-fixed-column--left,.el-table__header-wrapper tr th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table__body,.el-table__footer,.el-table__header{table-layout:fixed;border-collapse:separate}.el-table__footer-wrapper,.el-table__header-wrapper{overflow:hidden}.el-table__footer-wrapper tbody td.el-table__cell,.el-table__header-wrapper tbody td.el-table__cell{background-color:var(--el-table-row-hover-bg-color);color:var(--el-table-text-color)}.el-table__body-wrapper .el-table-column--selection>.cell,.el-table__header-wrapper .el-table-column--selection>.cell{display:inline-flex;align-items:center;height:23px}.el-table__body-wrapper .el-table-column--selection .el-checkbox,.el-table__header-wrapper .el-table-column--selection .el-checkbox{height:unset}.el-table.is-scrolling-left .el-table-fixed-column--right.is-first-column:before{box-shadow:var(--el-table-fixed-right-column)}.el-table.is-scrolling-left.el-table--border .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:var(--el-table-border)}.el-table.is-scrolling-left th.el-table-fixed-column--left{background-color:var(--el-table-header-bg-color)}.el-table.is-scrolling-right .el-table-fixed-column--left.is-last-column:before{box-shadow:var(--el-table-fixed-left-column)}.el-table.is-scrolling-right .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:none}.el-table.is-scrolling-right th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table.is-scrolling-middle .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:none}.el-table.is-scrolling-middle .el-table-fixed-column--right.is-first-column:before{box-shadow:var(--el-table-fixed-right-column)}.el-table.is-scrolling-middle .el-table-fixed-column--left.is-last-column:before{box-shadow:var(--el-table-fixed-left-column)}.el-table.is-scrolling-none .el-table-fixed-column--left.is-first-column:before,.el-table.is-scrolling-none .el-table-fixed-column--left.is-last-column:before,.el-table.is-scrolling-none .el-table-fixed-column--right.is-first-column:before,.el-table.is-scrolling-none .el-table-fixed-column--right.is-last-column:before{box-shadow:none}.el-table.is-scrolling-none th.el-table-fixed-column--left,.el-table.is-scrolling-none th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table__body-wrapper{overflow:hidden;position:relative;flex:1}.el-table__body-wrapper .el-scrollbar__bar{z-index:2}.el-table .caret-wrapper{display:inline-flex;flex-direction:column;align-items:center;height:14px;width:24px;vertical-align:middle;cursor:pointer;overflow:initial;position:relative}.el-table .sort-caret{width:0;height:0;border:solid 5px transparent;position:absolute;left:7px}.el-table .sort-caret.ascending{border-bottom-color:var(--el-text-color-placeholder);top:-5px}.el-table .sort-caret.descending{border-top-color:var(--el-text-color-placeholder);bottom:-3px}.el-table .ascending .sort-caret.ascending{border-bottom-color:var(--el-color-primary)}.el-table .descending .sort-caret.descending{border-top-color:var(--el-color-primary)}.el-table .hidden-columns{visibility:hidden;position:absolute;z-index:-1}.el-table--striped .el-table__body tr.el-table__row--striped td.el-table__cell{background:var(--el-fill-color-lighter)}.el-table--striped .el-table__body tr.el-table__row--striped.current-row td.el-table__cell{background-color:var(--el-table-current-row-bg-color)}.el-table__body tr.hover-row.current-row>td.el-table__cell,.el-table__body tr.hover-row.el-table__row--striped.current-row>td.el-table__cell,.el-table__body tr.hover-row.el-table__row--striped>td.el-table__cell,.el-table__body tr.hover-row>td.el-table__cell{background-color:var(--el-table-row-hover-bg-color)}.el-table__body tr.current-row>td.el-table__cell{background-color:var(--el-table-current-row-bg-color)}.el-table__column-resize-proxy{position:absolute;left:200px;top:0;bottom:0;width:0;border-left:var(--el-table-border);z-index:10}.el-table__column-filter-trigger{display:inline-block;cursor:pointer}.el-table__column-filter-trigger i{color:var(--el-color-info);font-size:14px;vertical-align:middle}.el-table__border-left-patch{top:0;left:0;width:1px;height:100%;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table__border-bottom-patch{left:0;height:1px;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table__border-right-patch{top:0;height:100%;width:1px;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table--enable-row-transition .el-table__body td.el-table__cell{transition:background-color .25s ease}.el-table--enable-row-hover .el-table__body tr:hover>td.el-table__cell{background-color:var(--el-table-row-hover-bg-color)}.el-table [class*=el-table__row--level] .el-table__expand-icon{display:inline-block;width:12px;line-height:12px;height:12px;text-align:center;margin-right:8px}.el-table .el-table.el-table--border .el-table__cell{border-right:var(--el-table-border)}.el-table:not(.el-table--border) .el-table__cell{border-right:none}.el-table:not(.el-table--border)>.el-table__inner-wrapper:after{content:none}.el-checkbox{--el-checkbox-font-size:14px;--el-checkbox-font-weight:var(--el-font-weight-primary);--el-checkbox-text-color:var(--el-text-color-regular);--el-checkbox-input-height:14px;--el-checkbox-input-width:14px;--el-checkbox-border-radius:var(--el-border-radius-small);--el-checkbox-bg-color:var(--el-fill-color-blank);--el-checkbox-input-border:var(--el-border);--el-checkbox-disabled-border-color:var(--el-border-color);--el-checkbox-disabled-input-fill:var(--el-fill-color-light);--el-checkbox-disabled-icon-color:var(--el-text-color-placeholder);--el-checkbox-disabled-checked-input-fill:var(--el-border-color-extra-light);--el-checkbox-disabled-checked-input-border-color:var(--el-border-color);--el-checkbox-disabled-checked-icon-color:var(--el-text-color-placeholder);--el-checkbox-checked-text-color:var(--el-color-primary);--el-checkbox-checked-input-border-color:var(--el-color-primary);--el-checkbox-checked-bg-color:var(--el-color-primary);--el-checkbox-checked-icon-color:var(--el-color-white);--el-checkbox-input-border-color-hover:var(--el-color-primary)}.el-checkbox{color:var(--el-checkbox-text-color);font-weight:var(--el-checkbox-font-weight);font-size:var(--el-font-size-base);position:relative;cursor:pointer;display:inline-flex;align-items:center;white-space:nowrap;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;margin-right:30px;height:32px}.el-checkbox.is-bordered{padding:0 15px 0 9px;border-radius:var(--el-border-radius-base);border:var(--el-border);box-sizing:border-box}.el-checkbox.is-bordered.is-checked{border-color:var(--el-color-primary)}.el-checkbox.is-bordered.is-disabled{border-color:var(--el-border-color-lighter);cursor:not-allowed}.el-checkbox.is-bordered.el-checkbox--large{padding:0 19px 0 11px;border-radius:var(--el-border-radius-base)}.el-checkbox.is-bordered.el-checkbox--large .el-checkbox__label{font-size:var(--el-font-size-base)}.el-checkbox.is-bordered.el-checkbox--large .el-checkbox__inner{height:14px;width:14px}.el-checkbox.is-bordered.el-checkbox--small{padding:0 11px 0 7px;border-radius:calc(var(--el-border-radius-base) - 1px)}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__label{font-size:12px}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__inner{height:12px;width:12px}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__inner:after{height:6px;width:2px}.el-checkbox input:focus-visible+.el-checkbox__inner{outline:2px solid var(--el-checkbox-input-border-color-hover);outline-offset:1px;border-radius:var(--el-checkbox-border-radius)}.el-checkbox__input{white-space:nowrap;cursor:pointer;outline:0;display:inline-flex;position:relative}.el-checkbox__input.is-disabled .el-checkbox__inner{background-color:var(--el-checkbox-disabled-input-fill);border-color:var(--el-checkbox-disabled-border-color);cursor:not-allowed}.el-checkbox__input.is-disabled .el-checkbox__inner:after{cursor:not-allowed;border-color:var(--el-checkbox-disabled-icon-color)}.el-checkbox__input.is-disabled .el-checkbox__inner+.el-checkbox__label{cursor:not-allowed}.el-checkbox__input.is-disabled.is-checked .el-checkbox__inner{background-color:var(--el-checkbox-disabled-checked-input-fill);border-color:var(--el-checkbox-disabled-checked-input-border-color)}.el-checkbox__input.is-disabled.is-checked .el-checkbox__inner:after{border-color:var(--el-checkbox-disabled-checked-icon-color)}.el-checkbox__input.is-disabled.is-indeterminate .el-checkbox__inner{background-color:var(--el-checkbox-disabled-checked-input-fill);border-color:var(--el-checkbox-disabled-checked-input-border-color)}.el-checkbox__input.is-disabled.is-indeterminate .el-checkbox__inner:before{background-color:var(--el-checkbox-disabled-checked-icon-color);border-color:var(--el-checkbox-disabled-checked-icon-color)}.el-checkbox__input.is-disabled+span.el-checkbox__label{color:var(--el-disabled-text-color);cursor:not-allowed}.el-checkbox__input.is-checked .el-checkbox__inner{background-color:var(--el-checkbox-checked-bg-color);border-color:var(--el-checkbox-checked-input-border-color)}.el-checkbox__input.is-checked .el-checkbox__inner:after{transform:rotate(45deg) scaleY(1)}.el-checkbox__input.is-checked+.el-checkbox__label{color:var(--el-checkbox-checked-text-color)}.el-checkbox__input.is-focus:not(.is-checked) .el-checkbox__original:not(:focus-visible){border-color:var(--el-checkbox-input-border-color-hover)}.el-checkbox__input.is-indeterminate .el-checkbox__inner{background-color:var(--el-checkbox-checked-bg-color);border-color:var(--el-checkbox-checked-input-border-color)}.el-checkbox__input.is-indeterminate .el-checkbox__inner:before{content:"";position:absolute;display:block;background-color:var(--el-checkbox-checked-icon-color);height:2px;transform:scale(.5);left:0;right:0;top:5px}.el-checkbox__input.is-indeterminate .el-checkbox__inner:after{display:none}.el-checkbox__inner{display:inline-block;position:relative;border:var(--el-checkbox-input-border);border-radius:var(--el-checkbox-border-radius);box-sizing:border-box;width:var(--el-checkbox-input-width);height:var(--el-checkbox-input-height);background-color:var(--el-checkbox-bg-color);z-index:var(--el-index-normal);transition:border-color .25s cubic-bezier(.71,-.46,.29,1.46),background-color .25s cubic-bezier(.71,-.46,.29,1.46),outline .25s cubic-bezier(.71,-.46,.29,1.46)}.el-checkbox__inner:hover{border-color:var(--el-checkbox-input-border-color-hover)}.el-checkbox__inner:after{box-sizing:content-box;content:"";border:1px solid var(--el-checkbox-checked-icon-color);border-left:0;border-top:0;height:7px;left:4px;position:absolute;top:1px;transform:rotate(45deg) scaleY(0);width:3px;transition:transform .15s ease-in 50ms;transform-origin:center}.el-checkbox__original{opacity:0;outline:0;position:absolute;margin:0;width:0;height:0;z-index:-1}.el-checkbox__label{display:inline-block;padding-left:8px;line-height:1;font-size:var(--el-checkbox-font-size)}.el-checkbox.el-checkbox--large{height:40px}.el-checkbox.el-checkbox--large .el-checkbox__label{font-size:14px}.el-checkbox.el-checkbox--large .el-checkbox__inner{width:14px;height:14px}.el-checkbox.el-checkbox--small{height:24px}.el-checkbox.el-checkbox--small .el-checkbox__label{font-size:12px}.el-checkbox.el-checkbox--small .el-checkbox__inner{width:12px;height:12px}.el-checkbox.el-checkbox--small .el-checkbox__input.is-indeterminate .el-checkbox__inner:before{top:4px}.el-checkbox.el-checkbox--small .el-checkbox__inner:after{width:2px;height:6px}.el-checkbox:last-of-type{margin-right:0}.el-table-column--selection .cell{padding-left:14px;padding-right:14px}.el-table-filter{border:solid 1px var(--el-border-color-lighter);border-radius:2px;background-color:#fff;box-shadow:var(--el-box-shadow-light);box-sizing:border-box}.el-table-filter__list{padding:5px 0;margin:0;list-style:none;min-width:100px}.el-table-filter__list-item{line-height:36px;padding:0 10px;cursor:pointer;font-size:var(--el-font-size-base)}.el-table-filter__list-item:hover{background-color:var(--el-color-primary-light-9);color:var(--el-color-primary)}.el-table-filter__list-item.is-active{background-color:var(--el-color-primary);color:#fff}.el-table-filter__content{min-width:100px}.el-table-filter__bottom{border-top:1px solid var(--el-border-color-lighter);padding:8px}.el-table-filter__bottom button{background:0 0;border:none;color:var(--el-text-color-regular);cursor:pointer;font-size:var(--el-font-size-small);padding:0 3px}.el-table-filter__bottom button:hover{color:var(--el-color-primary)}.el-table-filter__bottom button:focus{outline:0}.el-table-filter__bottom button.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-table-filter__wrap{max-height:280px}.el-table-filter__checkbox-group{padding:10px}.el-table-filter__checkbox-group label.el-checkbox{display:flex;align-items:center;margin-right:5px;margin-bottom:12px;margin-left:5px;height:unset}.el-table-filter__checkbox-group .el-checkbox:last-child{margin-bottom:0}.bi-table[data-v-4fd4d173]{overflow:auto;height:var(--9c25e776)}.bi-table .table-fix[data-v-4fd4d173]{flex:1;min-width:var(--21675e16);width:var(--6bc0968e)}.bi-table .table[data-v-4fd4d173]{margin-bottom:2rem}.bi-table[data-v-4fd4d173] .table-header th{font-size:1.1em;font-weight:700;background-color:#8fe1fd16}.el-upload{--el-upload-dragger-padding-horizontal:40px;--el-upload-dragger-padding-vertical:10px}.el-upload{display:inline-flex;justify-content:center;align-items:center;cursor:pointer;outline:0}.el-upload__input{display:none}.el-upload__tip{font-size:12px;color:var(--el-text-color-regular);margin-top:7px}.el-upload iframe{position:absolute;z-index:-1;top:0;left:0;opacity:0}.el-upload--picture-card{--el-upload-picture-card-size:148px;background-color:var(--el-fill-color-lighter);border:1px dashed var(--el-border-color-darker);border-radius:6px;box-sizing:border-box;width:var(--el-upload-picture-card-size);height:var(--el-upload-picture-card-size);cursor:pointer;vertical-align:top;display:inline-flex;justify-content:center;align-items:center}.el-upload--picture-card i{font-size:28px;color:var(--el-text-color-secondary)}.el-upload--picture-card:hover{border-color:var(--el-color-primary);color:var(--el-color-primary)}.el-upload.is-drag{display:block}.el-upload:focus{border-color:var(--el-color-primary);color:var(--el-color-primary)}.el-upload:focus .el-upload-dragger{border-color:var(--el-color-primary)}.el-upload-dragger{padding:var(--el-upload-dragger-padding-horizontal) var(--el-upload-dragger-padding-vertical);background-color:var(--el-fill-color-blank);border:1px dashed var(--el-border-color);border-radius:6px;box-sizing:border-box;text-align:center;cursor:pointer;position:relative;overflow:hidden}.el-upload-dragger .el-icon--upload{font-size:67px;color:var(--el-text-color-placeholder);margin-bottom:16px;line-height:50px}.el-upload-dragger+.el-upload__tip{text-align:center}.el-upload-dragger~.el-upload__files{border-top:var(--el-border);margin-top:7px;padding-top:5px}.el-upload-dragger .el-upload__text{color:var(--el-text-color-regular);font-size:14px;text-align:center}.el-upload-dragger .el-upload__text em{color:var(--el-color-primary);font-style:normal}.el-upload-dragger:hover{border-color:var(--el-color-primary)}.el-upload-dragger.is-dragover{padding:calc(var(--el-upload-dragger-padding-horizontal) - 1px) calc(var(--el-upload-dragger-padding-vertical) - 1px);background-color:var(--el-color-primary-light-9);border:2px dashed var(--el-color-primary)}.el-upload-list{margin:10px 0 0;padding:0;list-style:none;position:relative}.el-upload-list__item{transition:all .5s cubic-bezier(.55,0,.1,1);font-size:14px;color:var(--el-text-color-regular);margin-bottom:5px;position:relative;box-sizing:border-box;border-radius:4px;width:100%}.el-upload-list__item .el-progress{position:absolute;top:20px;width:100%}.el-upload-list__item .el-progress__text{position:absolute;right:0;top:-13px}.el-upload-list__item .el-progress-bar{margin-right:0;padding-right:0}.el-upload-list__item .el-icon--upload-success{color:var(--el-color-success)}.el-upload-list__item .el-icon--close{display:none;position:absolute;right:5px;top:50%;cursor:pointer;opacity:.75;color:var(--el-text-color-regular);transition:opacity var(--el-transition-duration);transform:translateY(-50%)}.el-upload-list__item .el-icon--close:hover{opacity:1;color:var(--el-color-primary)}.el-upload-list__item .el-icon--close-tip{display:none;position:absolute;top:1px;right:5px;font-size:12px;cursor:pointer;opacity:1;color:var(--el-color-primary);font-style:normal}.el-upload-list__item:hover{background-color:var(--el-fill-color-light)}.el-upload-list__item:hover .el-icon--close{display:inline-flex}.el-upload-list__item:hover .el-progress__text{display:none}.el-upload-list__item .el-upload-list__item-info{display:inline-flex;justify-content:center;flex-direction:column;width:calc(100% - 30px);margin-left:4px}.el-upload-list__item.is-success .el-upload-list__item-status-label{display:inline-flex}.el-upload-list__item.is-success .el-upload-list__item-name:focus,.el-upload-list__item.is-success .el-upload-list__item-name:hover{color:var(--el-color-primary);cursor:pointer}.el-upload-list__item.is-success:focus:not(:hover) .el-icon--close-tip{display:inline-block}.el-upload-list__item.is-success:active,.el-upload-list__item.is-success:not(.focusing):focus{outline-width:0}.el-upload-list__item.is-success:active .el-icon--close-tip,.el-upload-list__item.is-success:not(.focusing):focus .el-icon--close-tip{display:none}.el-upload-list__item.is-success:focus .el-upload-list__item-status-label,.el-upload-list__item.is-success:hover .el-upload-list__item-status-label{display:none;opacity:0}.el-upload-list.is-disabled .el-upload-list__item-status-label,.el-upload-list.is-disabled .el-upload-list__item:hover{display:block}.el-upload-list__item-name{color:var(--el-text-color-regular);display:inline-flex;text-align:center;align-items:center;padding:0 4px;transition:color var(--el-transition-duration);font-size:var(--el-font-size-base)}.el-upload-list__item-name .el-icon{margin-right:6px;color:var(--el-text-color-secondary)}.el-upload-list__item-file-name{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-upload-list__item-status-label{position:absolute;right:5px;top:0;line-height:inherit;display:none;height:100%;justify-content:center;align-items:center;transition:opacity var(--el-transition-duration)}.el-upload-list__item-delete{position:absolute;right:10px;top:0;font-size:12px;color:var(--el-text-color-regular);display:none}.el-upload-list__item-delete:hover{color:var(--el-color-primary)}.el-upload-list--picture-card{--el-upload-list-picture-card-size:148px;display:inline-flex;flex-wrap:wrap;margin:0}.el-upload-list--picture-card .el-upload-list__item{overflow:hidden;background-color:var(--el-fill-color-blank);border:1px solid var(--el-border-color);border-radius:6px;box-sizing:border-box;width:var(--el-upload-list-picture-card-size);height:var(--el-upload-list-picture-card-size);margin:0 8px 8px 0;padding:0;display:inline-flex}.el-upload-list--picture-card .el-upload-list__item .el-icon--check,.el-upload-list--picture-card .el-upload-list__item .el-icon--circle-check{color:#fff}.el-upload-list--picture-card .el-upload-list__item .el-icon--close{display:none}.el-upload-list--picture-card .el-upload-list__item:hover .el-upload-list__item-status-label{opacity:0;display:block}.el-upload-list--picture-card .el-upload-list__item:hover .el-progress__text{display:block}.el-upload-list--picture-card .el-upload-list__item .el-upload-list__item-name{display:none}.el-upload-list--picture-card .el-upload-list__item-thumbnail{width:100%;height:100%;-o-object-fit:contain;object-fit:contain}.el-upload-list--picture-card .el-upload-list__item-status-label{right:-15px;top:-6px;width:40px;height:24px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-list--picture-card .el-upload-list__item-status-label i{font-size:12px;margin-top:11px;transform:rotate(-45deg)}.el-upload-list--picture-card .el-upload-list__item-actions{position:absolute;width:100%;height:100%;left:0;top:0;cursor:default;display:inline-flex;justify-content:center;align-items:center;color:#fff;opacity:0;font-size:20px;background-color:var(--el-overlay-color-lighter);transition:opacity var(--el-transition-duration)}.el-upload-list--picture-card .el-upload-list__item-actions span{display:none;cursor:pointer}.el-upload-list--picture-card .el-upload-list__item-actions span+span{margin-left:1rem}.el-upload-list--picture-card .el-upload-list__item-actions .el-upload-list__item-delete{position:static;font-size:inherit;color:inherit}.el-upload-list--picture-card .el-upload-list__item-actions:hover{opacity:1}.el-upload-list--picture-card .el-upload-list__item-actions:hover span{display:inline-flex}.el-upload-list--picture-card .el-progress{top:50%;left:50%;transform:translate(-50%,-50%);bottom:auto;width:126px}.el-upload-list--picture-card .el-progress .el-progress__text{top:50%}.el-upload-list--picture .el-upload-list__item{overflow:hidden;z-index:0;background-color:var(--el-fill-color-blank);border:1px solid var(--el-border-color);border-radius:6px;box-sizing:border-box;margin-top:10px;padding:10px;display:flex;align-items:center}.el-upload-list--picture .el-upload-list__item .el-icon--check,.el-upload-list--picture .el-upload-list__item .el-icon--circle-check{color:#fff}.el-upload-list--picture .el-upload-list__item:hover .el-upload-list__item-status-label{opacity:0;display:block}.el-upload-list--picture .el-upload-list__item:hover .el-progress__text{display:block}.el-upload-list--picture .el-upload-list__item.is-success .el-upload-list__item-name i{display:none}.el-upload-list--picture .el-upload-list__item .el-icon--close{top:5px;transform:translateY(0)}.el-upload-list--picture .el-upload-list__item-thumbnail{display:inline-flex;justify-content:center;align-items:center;width:70px;height:70px;-o-object-fit:contain;object-fit:contain;position:relative;z-index:1;background-color:var(--el-color-white)}.el-upload-list--picture .el-upload-list__item-status-label{position:absolute;right:-17px;top:-7px;width:46px;height:26px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-list--picture .el-upload-list__item-status-label i{font-size:12px;margin-top:12px;transform:rotate(-45deg)}.el-upload-list--picture .el-progress{position:relative;top:-7px}.el-upload-cover{position:absolute;left:0;top:0;width:100%;height:100%;overflow:hidden;z-index:10;cursor:default}.el-upload-cover:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-upload-cover img{display:block;width:100%;height:100%}.el-upload-cover__label{right:-15px;top:-6px;width:40px;height:24px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-cover__label i{font-size:12px;margin-top:11px;transform:rotate(-45deg);color:#fff}.el-upload-cover__progress{display:inline-block;vertical-align:middle;position:static;width:243px}.el-upload-cover__progress+.el-upload__inner{opacity:0}.el-upload-cover__content{position:absolute;top:0;left:0;width:100%;height:100%}.el-upload-cover__interact{position:absolute;bottom:0;left:0;width:100%;height:100%;background-color:var(--el-overlay-color-light);text-align:center}.el-upload-cover__interact .btn{display:inline-block;color:#fff;font-size:14px;cursor:pointer;vertical-align:middle;transition:var(--el-transition-md-fade);margin-top:60px}.el-upload-cover__interact .btn i{margin-top:0}.el-upload-cover__interact .btn span{opacity:0;transition:opacity .15s linear}.el-upload-cover__interact .btn:not(:first-child){margin-left:35px}.el-upload-cover__interact .btn:hover{transform:translateY(-13px)}.el-upload-cover__interact .btn:hover span{opacity:1}.el-upload-cover__interact .btn i{color:#fff;display:block;font-size:24px;line-height:inherit;margin:0 auto 5px}.el-upload-cover__title{position:absolute;bottom:0;left:0;background-color:#fff;height:36px;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-weight:400;text-align:left;padding:0 10px;margin:0;line-height:36px;font-size:14px;color:var(--el-text-color-primary)}.el-upload-cover+.el-upload__inner{opacity:0;position:relative;z-index:1}.el-progress{position:relative;line-height:1;display:flex;align-items:center}.el-progress__text{font-size:14px;color:var(--el-text-color-regular);margin-left:5px;min-width:50px;line-height:1}.el-progress__text i{vertical-align:middle;display:block}.el-progress--circle,.el-progress--dashboard{display:inline-block}.el-progress--circle .el-progress__text,.el-progress--dashboard .el-progress__text{position:absolute;top:50%;left:0;width:100%;text-align:center;margin:0;transform:translateY(-50%)}.el-progress--circle .el-progress__text i,.el-progress--dashboard .el-progress__text i{vertical-align:middle;display:inline-block}.el-progress--without-text .el-progress__text{display:none}.el-progress--without-text .el-progress-bar{padding-right:0;margin-right:0;display:block}.el-progress--text-inside .el-progress-bar{padding-right:0;margin-right:0}.el-progress.is-success .el-progress-bar__inner{background-color:var(--el-color-success)}.el-progress.is-success .el-progress__text{color:var(--el-color-success)}.el-progress.is-warning .el-progress-bar__inner{background-color:var(--el-color-warning)}.el-progress.is-warning .el-progress__text{color:var(--el-color-warning)}.el-progress.is-exception .el-progress-bar__inner{background-color:var(--el-color-danger)}.el-progress.is-exception .el-progress__text{color:var(--el-color-danger)}.el-progress-bar{flex-grow:1;box-sizing:border-box}.el-progress-bar__outer{height:6px;border-radius:100px;background-color:var(--el-border-color-lighter);overflow:hidden;position:relative;vertical-align:middle}.el-progress-bar__inner{position:absolute;left:0;top:0;height:100%;background-color:var(--el-color-primary);text-align:right;border-radius:100px;line-height:1;white-space:nowrap;transition:width .6s ease}.el-progress-bar__inner:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-progress-bar__inner--indeterminate{transform:translateZ(0);-webkit-animation:indeterminate 3s infinite;animation:indeterminate 3s infinite}.el-progress-bar__innerText{display:inline-block;vertical-align:middle;color:#fff;font-size:12px;margin:0 5px}@-webkit-keyframes progress{0%{background-position:0 0}to{background-position:32px 0}}@keyframes progress{0%{background-position:0 0}to{background-position:32px 0}}@-webkit-keyframes indeterminate{0%{left:-100%}to{left:100%}}@keyframes indeterminate{0%{left:-100%}to{left:100%}}.slicer-box[data-v-0804f81c]{display:inline-block;min-width:12rem;margin-right:.8rem}.title[data-v-0804f81c]{margin-bottom:.5rem}.el-tabs{--el-tabs-header-height:40px}.el-tabs__header{padding:0;position:relative;margin:0 0 15px}.el-tabs__active-bar{position:absolute;bottom:0;left:0;height:2px;background-color:var(--el-color-primary);z-index:1;transition:width var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier),transform var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);list-style:none}.el-tabs__new-tab{display:flex;align-items:center;justify-content:center;float:right;border:1px solid var(--el-border-color);height:20px;width:20px;line-height:20px;margin:10px 0 10px 10px;border-radius:3px;text-align:center;font-size:12px;color:var(--el-text-color-primary);cursor:pointer;transition:all .15s}.el-tabs__new-tab .is-icon-plus{height:inherit;width:inherit;transform:scale(.8)}.el-tabs__new-tab .is-icon-plus svg{vertical-align:middle}.el-tabs__new-tab:hover{color:var(--el-color-primary)}.el-tabs__nav-wrap{overflow:hidden;margin-bottom:-1px;position:relative}.el-tabs__nav-wrap:after{content:"";position:absolute;left:0;bottom:0;width:100%;height:2px;background-color:var(--el-border-color-light);z-index:var(--el-index-normal)}.el-tabs__nav-wrap.is-scrollable{padding:0 20px;box-sizing:border-box}.el-tabs__nav-scroll{overflow:hidden}.el-tabs__nav-next,.el-tabs__nav-prev{position:absolute;cursor:pointer;line-height:44px;font-size:12px;color:var(--el-text-color-secondary);width:20px;text-align:center}.el-tabs__nav-next{right:0}.el-tabs__nav-prev{left:0}.el-tabs__nav{white-space:nowrap;position:relative;transition:transform var(--el-transition-duration);float:left;z-index:calc(var(--el-index-normal) + 1)}.el-tabs__nav.is-stretch{min-width:100%;display:flex}.el-tabs__nav.is-stretch>*{flex:1;text-align:center}.el-tabs__item{padding:0 20px;height:var(--el-tabs-header-height);box-sizing:border-box;line-height:var(--el-tabs-header-height);display:inline-block;list-style:none;font-size:var(--el-font-size-base);font-weight:500;color:var(--el-text-color-primary);position:relative}.el-tabs__item:focus,.el-tabs__item:focus:active{outline:0}.el-tabs__item:focus-visible{box-shadow:0 0 2px 2px var(--el-color-primary) inset;border-radius:3px}.el-tabs__item .is-icon-close{border-radius:50%;text-align:center;transition:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);margin-left:5px}.el-tabs__item .is-icon-close:before{transform:scale(.9);display:inline-block}.el-tabs__item .is-icon-close:hover{background-color:var(--el-text-color-placeholder);color:#fff}.el-tabs__item .is-icon-close svg{margin-top:1px}.el-tabs__item.is-active{color:var(--el-color-primary)}.el-tabs__item:hover{color:var(--el-color-primary);cursor:pointer}.el-tabs__item.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-tabs__content{overflow:hidden;position:relative}.el-tabs--card>.el-tabs__header{border-bottom:1px solid var(--el-border-color-light);height:var(--el-tabs-header-height)}.el-tabs--card>.el-tabs__header .el-tabs__nav-wrap:after{content:none}.el-tabs--card>.el-tabs__header .el-tabs__nav{border:1px solid var(--el-border-color-light);border-bottom:none;border-radius:4px 4px 0 0;box-sizing:border-box}.el-tabs--card>.el-tabs__header .el-tabs__active-bar{display:none}.el-tabs--card>.el-tabs__header .el-tabs__item .is-icon-close{position:relative;font-size:12px;width:0;height:14px;vertical-align:middle;line-height:15px;overflow:hidden;top:-1px;right:-2px;transform-origin:100% 50%}.el-tabs--card>.el-tabs__header .el-tabs__item{border-bottom:1px solid transparent;border-left:1px solid var(--el-border-color-light);transition:color var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier),padding var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier)}.el-tabs--card>.el-tabs__header .el-tabs__item:first-child{border-left:none}.el-tabs--card>.el-tabs__header .el-tabs__item.is-closable:hover{padding-left:13px;padding-right:13px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-closable:hover .is-icon-close{width:14px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active{border-bottom-color:var(--el-bg-color)}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active.is-closable{padding-left:20px;padding-right:20px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active.is-closable .is-icon-close{width:14px}.el-tabs--border-card{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color)}.el-tabs--border-card>.el-tabs__content{padding:15px}.el-tabs--border-card>.el-tabs__header{background-color:var(--el-fill-color-light);border-bottom:1px solid var(--el-border-color-light);margin:0}.el-tabs--border-card>.el-tabs__header .el-tabs__nav-wrap:after{content:none}.el-tabs--border-card>.el-tabs__header .el-tabs__item{transition:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);border:1px solid transparent;margin-top:-1px;color:var(--el-text-color-secondary)}.el-tabs--border-card>.el-tabs__header .el-tabs__item:first-child{margin-left:-1px}.el-tabs--border-card>.el-tabs__header .el-tabs__item+.el-tabs__item{margin-left:-1px}.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay);border-right-color:var(--el-border-color);border-left-color:var(--el-border-color)}.el-tabs--border-card>.el-tabs__header .el-tabs__item:not(.is-disabled):hover{color:var(--el-color-primary)}.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-disabled{color:var(--el-disabled-text-color)}.el-tabs--border-card>.el-tabs__header .is-scrollable .el-tabs__item:first-child{margin-left:0}.el-tabs--bottom .el-tabs__item.is-bottom:nth-child(2),.el-tabs--bottom .el-tabs__item.is-top:nth-child(2),.el-tabs--top .el-tabs__item.is-bottom:nth-child(2),.el-tabs--top .el-tabs__item.is-top:nth-child(2){padding-left:0}.el-tabs--bottom .el-tabs__item.is-bottom:last-child,.el-tabs--bottom .el-tabs__item.is-top:last-child,.el-tabs--top .el-tabs__item.is-bottom:last-child,.el-tabs--top .el-tabs__item.is-top:last-child{padding-right:0}.el-tabs--bottom .el-tabs--left>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom .el-tabs--right>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom.el-tabs--border-card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom.el-tabs--card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top .el-tabs--left>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top .el-tabs--right>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top.el-tabs--border-card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top.el-tabs--card>.el-tabs__header .el-tabs__item:nth-child(2){padding-left:20px}.el-tabs--bottom .el-tabs--left>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom .el-tabs--right>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom.el-tabs--border-card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom.el-tabs--card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top .el-tabs--left>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top .el-tabs--right>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top.el-tabs--border-card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top.el-tabs--card>.el-tabs__header .el-tabs__item:last-child{padding-right:20px}.el-tabs--bottom .el-tabs__header.is-bottom{margin-bottom:0;margin-top:10px}.el-tabs--bottom.el-tabs--border-card .el-tabs__header.is-bottom{border-bottom:0;border-top:1px solid var(--el-border-color)}.el-tabs--bottom.el-tabs--border-card .el-tabs__nav-wrap.is-bottom{margin-top:-1px;margin-bottom:0}.el-tabs--bottom.el-tabs--border-card .el-tabs__item.is-bottom:not(.is-active){border:1px solid transparent}.el-tabs--bottom.el-tabs--border-card .el-tabs__item.is-bottom{margin:0 -1px -1px}.el-tabs--left,.el-tabs--right{overflow:hidden}.el-tabs--left .el-tabs__header.is-left,.el-tabs--left .el-tabs__header.is-right,.el-tabs--left .el-tabs__nav-scroll,.el-tabs--left .el-tabs__nav-wrap.is-left,.el-tabs--left .el-tabs__nav-wrap.is-right,.el-tabs--right .el-tabs__header.is-left,.el-tabs--right .el-tabs__header.is-right,.el-tabs--right .el-tabs__nav-scroll,.el-tabs--right .el-tabs__nav-wrap.is-left,.el-tabs--right .el-tabs__nav-wrap.is-right{height:100%}.el-tabs--left .el-tabs__active-bar.is-left,.el-tabs--left .el-tabs__active-bar.is-right,.el-tabs--right .el-tabs__active-bar.is-left,.el-tabs--right .el-tabs__active-bar.is-right{top:0;bottom:auto;width:2px;height:auto}.el-tabs--left .el-tabs__nav-wrap.is-left,.el-tabs--left .el-tabs__nav-wrap.is-right,.el-tabs--right .el-tabs__nav-wrap.is-left,.el-tabs--right .el-tabs__nav-wrap.is-right{margin-bottom:0}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev{height:30px;line-height:30px;width:100%;text-align:center;cursor:pointer}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next i,.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev i,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next i,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev i,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next i,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev i,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next i,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev i{transform:rotate(90deg)}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev{left:auto;top:0}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next{right:auto;bottom:0}.el-tabs--left .el-tabs__nav-wrap.is-left.is-scrollable,.el-tabs--left .el-tabs__nav-wrap.is-right.is-scrollable,.el-tabs--right .el-tabs__nav-wrap.is-left.is-scrollable,.el-tabs--right .el-tabs__nav-wrap.is-right.is-scrollable{padding:30px 0}.el-tabs--left .el-tabs__nav-wrap.is-left:after,.el-tabs--left .el-tabs__nav-wrap.is-right:after,.el-tabs--right .el-tabs__nav-wrap.is-left:after,.el-tabs--right .el-tabs__nav-wrap.is-right:after{height:100%;width:2px;bottom:auto;top:0}.el-tabs--left .el-tabs__nav.is-left,.el-tabs--left .el-tabs__nav.is-right,.el-tabs--right .el-tabs__nav.is-left,.el-tabs--right .el-tabs__nav.is-right{float:none}.el-tabs--left .el-tabs__item.is-left,.el-tabs--left .el-tabs__item.is-right,.el-tabs--right .el-tabs__item.is-left,.el-tabs--right .el-tabs__item.is-right{display:block}.el-tabs--left .el-tabs__header.is-left{float:left;margin-bottom:0;margin-right:10px}.el-tabs--left .el-tabs__nav-wrap.is-left{margin-right:-1px}.el-tabs--left .el-tabs__nav-wrap.is-left:after{left:auto;right:0}.el-tabs--left .el-tabs__active-bar.is-left{right:0;left:auto}.el-tabs--left .el-tabs__item.is-left{text-align:right}.el-tabs--left.el-tabs--card .el-tabs__active-bar.is-left{display:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left{border-left:none;border-right:1px solid var(--el-border-color-light);border-bottom:none;border-top:1px solid var(--el-border-color-light);text-align:left}.el-tabs--left.el-tabs--card .el-tabs__item.is-left:first-child{border-right:1px solid var(--el-border-color-light);border-top:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active{border:1px solid var(--el-border-color-light);border-right-color:#fff;border-left:none;border-bottom:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active:first-child{border-top:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active:last-child{border-bottom:none}.el-tabs--left.el-tabs--card .el-tabs__nav{border-radius:4px 0 0 4px;border-bottom:1px solid var(--el-border-color-light);border-right:none}.el-tabs--left.el-tabs--card .el-tabs__new-tab{float:none}.el-tabs--left.el-tabs--border-card .el-tabs__header.is-left{border-right:1px solid var(--el-border-color)}.el-tabs--left.el-tabs--border-card .el-tabs__item.is-left{border:1px solid transparent;margin:-1px 0 -1px -1px}.el-tabs--left.el-tabs--border-card .el-tabs__item.is-left.is-active{border-color:transparent;border-top-color:#d1dbe5;border-bottom-color:#d1dbe5}.el-tabs--right .el-tabs__header.is-right{float:right;margin-bottom:0;margin-left:10px}.el-tabs--right .el-tabs__nav-wrap.is-right{margin-left:-1px}.el-tabs--right .el-tabs__nav-wrap.is-right:after{left:0;right:auto}.el-tabs--right .el-tabs__active-bar.is-right{left:0}.el-tabs--right.el-tabs--card .el-tabs__active-bar.is-right{display:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right{border-bottom:none;border-top:1px solid var(--el-border-color-light)}.el-tabs--right.el-tabs--card .el-tabs__item.is-right:first-child{border-left:1px solid var(--el-border-color-light);border-top:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active{border:1px solid var(--el-border-color-light);border-left-color:#fff;border-right:none;border-bottom:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active:first-child{border-top:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active:last-child{border-bottom:none}.el-tabs--right.el-tabs--card .el-tabs__nav{border-radius:0 4px 4px 0;border-bottom:1px solid var(--el-border-color-light);border-left:none}.el-tabs--right.el-tabs--border-card .el-tabs__header.is-right{border-left:1px solid var(--el-border-color)}.el-tabs--right.el-tabs--border-card .el-tabs__item.is-right{border:1px solid transparent;margin:-1px -1px -1px 0}.el-tabs--right.el-tabs--border-card .el-tabs__item.is-right.is-active{border-color:transparent;border-top-color:#d1dbe5;border-bottom-color:#d1dbe5}.slideInLeft-transition,.slideInRight-transition{display:inline-block}.slideInRight-enter{-webkit-animation:slideInRight-enter var(--el-transition-duration);animation:slideInRight-enter var(--el-transition-duration)}.slideInRight-leave{position:absolute;left:0;right:0;-webkit-animation:slideInRight-leave var(--el-transition-duration);animation:slideInRight-leave var(--el-transition-duration)}.slideInLeft-enter{-webkit-animation:slideInLeft-enter var(--el-transition-duration);animation:slideInLeft-enter var(--el-transition-duration)}.slideInLeft-leave{position:absolute;left:0;right:0;-webkit-animation:slideInLeft-leave var(--el-transition-duration);animation:slideInLeft-leave var(--el-transition-duration)}@-webkit-keyframes slideInRight-enter{0%{opacity:0;transform-origin:0 0;transform:translate(100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@keyframes slideInRight-enter{0%{opacity:0;transform-origin:0 0;transform:translate(100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@-webkit-keyframes slideInRight-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(100%);opacity:0}}@keyframes slideInRight-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(100%);opacity:0}}@-webkit-keyframes slideInLeft-enter{0%{opacity:0;transform-origin:0 0;transform:translate(-100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@keyframes slideInLeft-enter{0%{opacity:0;transform-origin:0 0;transform:translate(-100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@-webkit-keyframes slideInLeft-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(-100%);opacity:0}}@keyframes slideInLeft-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(-100%);opacity:0}}.pybi-tabs .custom-tabs-label[data-v-2d2e93ca]{font-size:1.5em;width:100%;display:flex;flex-direction:row;justify-content:center;align-items:center}.pybi-tabs .custom-tabs-label .tab-name[data-v-2d2e93ca]{margin-left:.5em}.el-affix--fixed{position:fixed}.pybi-input[data-v-184ceae1]{width:18em}.el-slider{--el-slider-main-bg-color:var(--el-color-primary);--el-slider-runway-bg-color:var(--el-border-color-light);--el-slider-stop-bg-color:var(--el-color-white);--el-slider-disabled-color:var(--el-text-color-placeholder);--el-slider-border-radius:3px;--el-slider-height:6px;--el-slider-button-size:20px;--el-slider-button-wrapper-size:36px;--el-slider-button-wrapper-offset:-15px}.el-slider{width:100%;height:32px;display:flex;align-items:center}.el-slider__runway{flex:1;height:var(--el-slider-height);background-color:var(--el-slider-runway-bg-color);border-radius:var(--el-slider-border-radius);position:relative;cursor:pointer}.el-slider__runway.show-input{margin-right:30px;width:auto}.el-slider__runway.is-disabled{cursor:default}.el-slider__runway.is-disabled .el-slider__bar{background-color:var(--el-slider-disabled-color)}.el-slider__runway.is-disabled .el-slider__button{border-color:var(--el-slider-disabled-color)}.el-slider__runway.is-disabled .el-slider__button-wrapper.hover,.el-slider__runway.is-disabled .el-slider__button-wrapper:hover,.el-slider__runway.is-disabled .el-slider__button-wrapper.dragging{cursor:not-allowed}.el-slider__runway.is-disabled .el-slider__button.dragging,.el-slider__runway.is-disabled .el-slider__button.hover,.el-slider__runway.is-disabled .el-slider__button:hover{transform:scale(1)}.el-slider__runway.is-disabled .el-slider__button.hover,.el-slider__runway.is-disabled .el-slider__button:hover,.el-slider__runway.is-disabled .el-slider__button.dragging{cursor:not-allowed}.el-slider__input{flex-shrink:0;width:130px}.el-slider__bar{height:var(--el-slider-height);background-color:var(--el-slider-main-bg-color);border-top-left-radius:var(--el-slider-border-radius);border-bottom-left-radius:var(--el-slider-border-radius);position:absolute}.el-slider__button-wrapper{height:var(--el-slider-button-wrapper-size);width:var(--el-slider-button-wrapper-size);position:absolute;z-index:1;top:var(--el-slider-button-wrapper-offset);transform:translate(-50%);background-color:transparent;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;line-height:normal;outline:0}.el-slider__button-wrapper:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-slider__button-wrapper.hover,.el-slider__button-wrapper:hover{cursor:-webkit-grab;cursor:grab}.el-slider__button-wrapper.dragging{cursor:-webkit-grabbing;cursor:grabbing}.el-slider__button{display:inline-block;width:var(--el-slider-button-size);height:var(--el-slider-button-size);vertical-align:middle;border:solid 2px var(--el-slider-main-bg-color);background-color:var(--el-color-white);border-radius:50%;box-sizing:border-box;transition:var(--el-transition-duration-fast);-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-slider__button.dragging,.el-slider__button.hover,.el-slider__button:hover{transform:scale(1.2)}.el-slider__button.hover,.el-slider__button:hover{cursor:-webkit-grab;cursor:grab}.el-slider__button.dragging{cursor:-webkit-grabbing;cursor:grabbing}.el-slider__stop{position:absolute;height:var(--el-slider-height);width:var(--el-slider-height);border-radius:var(--el-border-radius-circle);background-color:var(--el-slider-stop-bg-color);transform:translate(-50%)}.el-slider__marks{top:0;left:12px;width:18px;height:100%}.el-slider__marks-text{position:absolute;transform:translate(-50%);font-size:14px;color:var(--el-color-info);margin-top:15px;white-space:pre}.el-slider.is-vertical{position:relative;display:inline-flex;width:auto;height:100%;flex:0}.el-slider.is-vertical .el-slider__runway{width:var(--el-slider-height);height:100%;margin:0 16px}.el-slider.is-vertical .el-slider__bar{width:var(--el-slider-height);height:auto;border-radius:0 0 3px 3px}.el-slider.is-vertical .el-slider__button-wrapper{top:auto;left:var(--el-slider-button-wrapper-offset);transform:translateY(50%)}.el-slider.is-vertical .el-slider__stop{transform:translateY(50%)}.el-slider.is-vertical .el-slider__marks-text{margin-top:0;left:15px;transform:translateY(50%)}.el-slider--large{height:40px}.el-slider--small{height:24px}.el-input-number{position:relative;display:inline-flex;width:150px;line-height:30px}.el-input-number .el-input__wrapper{padding-left:42px;padding-right:42px}.el-input-number .el-input__inner{-webkit-appearance:none;-moz-appearance:textfield;text-align:center;line-height:1}.el-input-number .el-input__inner::-webkit-inner-spin-button,.el-input-number .el-input__inner::-webkit-outer-spin-button{margin:0;-webkit-appearance:none}.el-input-number__decrease,.el-input-number__increase{display:flex;justify-content:center;align-items:center;height:auto;position:absolute;z-index:1;top:1px;bottom:1px;width:32px;background:var(--el-fill-color-light);color:var(--el-text-color-regular);cursor:pointer;font-size:13px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-input-number__decrease:hover,.el-input-number__increase:hover{color:var(--el-color-primary)}.el-input-number__decrease:hover~.el-input:not(.is-disabled) .el-input_wrapper,.el-input-number__increase:hover~.el-input:not(.is-disabled) .el-input_wrapper{box-shadow:0 0 0 1px var(--el-input-focus-border-color,var(--el-color-primary)) inset}.el-input-number__decrease.is-disabled,.el-input-number__increase.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-input-number__increase{right:1px;border-radius:0 var(--el-border-radius-base) var(--el-border-radius-base) 0;border-left:var(--el-border)}.el-input-number__decrease{left:1px;border-radius:var(--el-border-radius-base) 0 0 var(--el-border-radius-base);border-right:var(--el-border)}.el-input-number.is-disabled .el-input-number__decrease,.el-input-number.is-disabled .el-input-number__increase{border-color:var(--el-disabled-border-color);color:var(--el-disabled-border-color)}.el-input-number.is-disabled .el-input-number__decrease:hover,.el-input-number.is-disabled .el-input-number__increase:hover{color:var(--el-disabled-border-color);cursor:not-allowed}.el-input-number--large{width:180px;line-height:38px}.el-input-number--large .el-input-number__decrease,.el-input-number--large .el-input-number__increase{width:40px;font-size:14px}.el-input-number--large .el-input__wrapper{padding-left:47px;padding-right:47px}.el-input-number--small{width:120px;line-height:22px}.el-input-number--small .el-input-number__decrease,.el-input-number--small .el-input-number__increase{width:24px;font-size:12px}.el-input-number--small .el-input__wrapper{padding-left:31px;padding-right:31px}.el-input-number--small .el-input-number__decrease [class*=el-icon],.el-input-number--small .el-input-number__increase [class*=el-icon]{transform:scale(.9)}.el-input-number.is-without-controls .el-input__wrapper{padding-left:15px;padding-right:15px}.el-input-number.is-controls-right .el-input__wrapper{padding-left:15px;padding-right:42px}.el-input-number.is-controls-right .el-input-number__decrease,.el-input-number.is-controls-right .el-input-number__increase{--el-input-number-controls-height:15px;height:var(--el-input-number-controls-height);line-height:var(--el-input-number-controls-height)}.el-input-number.is-controls-right .el-input-number__decrease [class*=el-icon],.el-input-number.is-controls-right .el-input-number__increase [class*=el-icon]{transform:scale(.8)}.el-input-number.is-controls-right .el-input-number__increase{bottom:auto;left:auto;border-radius:0 var(--el-border-radius-base) 0 0;border-bottom:var(--el-border)}.el-input-number.is-controls-right .el-input-number__decrease{right:1px;top:auto;left:auto;border-right:none;border-left:var(--el-border);border-radius:0 0 var(--el-border-radius-base) 0}.el-input-number.is-controls-right[class*=large] [class*=decrease],.el-input-number.is-controls-right[class*=large] [class*=increase]{--el-input-number-controls-height:19px}.el-input-number.is-controls-right[class*=small] [class*=decrease],.el-input-number.is-controls-right[class*=small] [class*=increase]{--el-input-number-controls-height:11px}
+@charset "UTF-8";:root{--el-color-white:#ffffff;--el-color-black:#000000;--el-color-primary-rgb:64,158,255;--el-color-success-rgb:103,194,58;--el-color-warning-rgb:230,162,60;--el-color-danger-rgb:245,108,108;--el-color-error-rgb:245,108,108;--el-color-info-rgb:144,147,153;--el-font-size-extra-large:20px;--el-font-size-large:18px;--el-font-size-medium:16px;--el-font-size-base:14px;--el-font-size-small:13px;--el-font-size-extra-small:12px;--el-font-family:"Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","\5fae\8f6f\96c5\9ed1",Arial,sans-serif;--el-font-weight-primary:500;--el-font-line-height-primary:24px;--el-index-normal:1;--el-index-top:1000;--el-index-popper:2000;--el-border-radius-base:4px;--el-border-radius-small:2px;--el-border-radius-round:20px;--el-border-radius-circle:100%;--el-transition-duration:.3s;--el-transition-duration-fast:.2s;--el-transition-function-ease-in-out-bezier:cubic-bezier(.645, .045, .355, 1);--el-transition-function-fast-bezier:cubic-bezier(.23, 1, .32, 1);--el-transition-all:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);--el-transition-fade:opacity var(--el-transition-duration) var(--el-transition-function-fast-bezier);--el-transition-md-fade:transform var(--el-transition-duration) var(--el-transition-function-fast-bezier),opacity var(--el-transition-duration) var(--el-transition-function-fast-bezier);--el-transition-fade-linear:opacity var(--el-transition-duration-fast) linear;--el-transition-border:border-color var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-transition-box-shadow:box-shadow var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-transition-color:color var(--el-transition-duration-fast) var(--el-transition-function-ease-in-out-bezier);--el-component-size-large:40px;--el-component-size:32px;--el-component-size-small:24px}:root{color-scheme:light;--el-color-white:#ffffff;--el-color-black:#000000;--el-color-primary:#409eff;--el-color-primary-light-3:#79bbff;--el-color-primary-light-5:#a0cfff;--el-color-primary-light-7:#c6e2ff;--el-color-primary-light-8:#d9ecff;--el-color-primary-light-9:#ecf5ff;--el-color-primary-dark-2:#337ecc;--el-color-success:#67c23a;--el-color-success-light-3:#95d475;--el-color-success-light-5:#b3e19d;--el-color-success-light-7:#d1edc4;--el-color-success-light-8:#e1f3d8;--el-color-success-light-9:#f0f9eb;--el-color-success-dark-2:#529b2e;--el-color-warning:#e6a23c;--el-color-warning-light-3:#eebe77;--el-color-warning-light-5:#f3d19e;--el-color-warning-light-7:#f8e3c5;--el-color-warning-light-8:#faecd8;--el-color-warning-light-9:#fdf6ec;--el-color-warning-dark-2:#b88230;--el-color-danger:#f56c6c;--el-color-danger-light-3:#f89898;--el-color-danger-light-5:#fab6b6;--el-color-danger-light-7:#fcd3d3;--el-color-danger-light-8:#fde2e2;--el-color-danger-light-9:#fef0f0;--el-color-danger-dark-2:#c45656;--el-color-error:#f56c6c;--el-color-error-light-3:#f89898;--el-color-error-light-5:#fab6b6;--el-color-error-light-7:#fcd3d3;--el-color-error-light-8:#fde2e2;--el-color-error-light-9:#fef0f0;--el-color-error-dark-2:#c45656;--el-color-info:#909399;--el-color-info-light-3:#b1b3b8;--el-color-info-light-5:#c8c9cc;--el-color-info-light-7:#dedfe0;--el-color-info-light-8:#e9e9eb;--el-color-info-light-9:#f4f4f5;--el-color-info-dark-2:#73767a;--el-bg-color:#ffffff;--el-bg-color-page:#f2f3f5;--el-bg-color-overlay:#ffffff;--el-text-color-primary:#303133;--el-text-color-regular:#606266;--el-text-color-secondary:#909399;--el-text-color-placeholder:#a8abb2;--el-text-color-disabled:#c0c4cc;--el-border-color:#dcdfe6;--el-border-color-light:#e4e7ed;--el-border-color-lighter:#ebeef5;--el-border-color-extra-light:#f2f6fc;--el-border-color-dark:#d4d7de;--el-border-color-darker:#cdd0d6;--el-fill-color:#f0f2f5;--el-fill-color-light:#f5f7fa;--el-fill-color-lighter:#fafafa;--el-fill-color-extra-light:#fafcff;--el-fill-color-dark:#ebedf0;--el-fill-color-darker:#e6e8eb;--el-fill-color-blank:#ffffff;--el-box-shadow:0px 12px 32px 4px rgba(0, 0, 0, .04),0px 8px 20px rgba(0, 0, 0, .08);--el-box-shadow-light:0px 0px 12px rgba(0, 0, 0, .12);--el-box-shadow-lighter:0px 0px 6px rgba(0, 0, 0, .12);--el-box-shadow-dark:0px 16px 48px 16px rgba(0, 0, 0, .08),0px 12px 32px rgba(0, 0, 0, .12),0px 8px 16px -8px rgba(0, 0, 0, .16);--el-disabled-bg-color:var(--el-fill-color-light);--el-disabled-text-color:var(--el-text-color-placeholder);--el-disabled-border-color:var(--el-border-color-light);--el-overlay-color:rgba(0, 0, 0, .8);--el-overlay-color-light:rgba(0, 0, 0, .7);--el-overlay-color-lighter:rgba(0, 0, 0, .5);--el-mask-color:rgba(255, 255, 255, .9);--el-mask-color-extra-light:rgba(255, 255, 255, .3);--el-border-width:1px;--el-border-style:solid;--el-border-color-hover:var(--el-text-color-disabled);--el-border:var(--el-border-width) var(--el-border-style) var(--el-border-color);--el-svg-monochrome-grey:var(--el-border-color)}.fade-in-linear-enter-active,.fade-in-linear-leave-active{transition:var(--el-transition-fade-linear)}.fade-in-linear-enter-from,.fade-in-linear-leave-to{opacity:0}.el-fade-in-linear-enter-active,.el-fade-in-linear-leave-active{transition:var(--el-transition-fade-linear)}.el-fade-in-linear-enter-from,.el-fade-in-linear-leave-to{opacity:0}.el-fade-in-enter-active,.el-fade-in-leave-active{transition:all var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-fade-in-enter-from,.el-fade-in-leave-active{opacity:0}.el-zoom-in-center-enter-active,.el-zoom-in-center-leave-active{transition:all var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-zoom-in-center-enter-from,.el-zoom-in-center-leave-active{opacity:0;transform:scaleX(0)}.el-zoom-in-top-enter-active,.el-zoom-in-top-leave-active{opacity:1;transform:scaleY(1);transition:var(--el-transition-md-fade);transform-origin:center top}.el-zoom-in-top-enter-active[data-popper-placement^=top],.el-zoom-in-top-leave-active[data-popper-placement^=top]{transform-origin:center bottom}.el-zoom-in-top-enter-from,.el-zoom-in-top-leave-active{opacity:0;transform:scaleY(0)}.el-zoom-in-bottom-enter-active,.el-zoom-in-bottom-leave-active{opacity:1;transform:scaleY(1);transition:var(--el-transition-md-fade);transform-origin:center bottom}.el-zoom-in-bottom-enter-from,.el-zoom-in-bottom-leave-active{opacity:0;transform:scaleY(0)}.el-zoom-in-left-enter-active,.el-zoom-in-left-leave-active{opacity:1;transform:scale(1);transition:var(--el-transition-md-fade);transform-origin:top left}.el-zoom-in-left-enter-from,.el-zoom-in-left-leave-active{opacity:0;transform:scale(.45)}.collapse-transition{transition:var(--el-transition-duration) height ease-in-out,var(--el-transition-duration) padding-top ease-in-out,var(--el-transition-duration) padding-bottom ease-in-out}.el-collapse-transition-enter-active,.el-collapse-transition-leave-active{transition:var(--el-transition-duration) max-height ease-in-out,var(--el-transition-duration) padding-top ease-in-out,var(--el-transition-duration) padding-bottom ease-in-out}.horizontal-collapse-transition{transition:var(--el-transition-duration) width ease-in-out,var(--el-transition-duration) padding-left ease-in-out,var(--el-transition-duration) padding-right ease-in-out}.el-list-enter-active,.el-list-leave-active{transition:all 1s}.el-list-enter-from,.el-list-leave-to{opacity:0;transform:translateY(-30px)}.el-list-leave-active{position:absolute!important}.el-opacity-transition{transition:opacity var(--el-transition-duration) cubic-bezier(.55,0,.1,1)}.el-icon-loading{-webkit-animation:rotating 2s linear infinite;animation:rotating 2s linear infinite}.el-icon--right{margin-left:5px}.el-icon--left{margin-right:5px}@-webkit-keyframes rotating{0%{transform:rotate(0)}to{transform:rotate(360deg)}}@keyframes rotating{0%{transform:rotate(0)}to{transform:rotate(360deg)}}.el-icon{--color:inherit;height:1em;width:1em;line-height:1em;display:inline-flex;justify-content:center;align-items:center;position:relative;fill:currentColor;color:var(--color);font-size:inherit}.el-icon.is-loading{-webkit-animation:rotating 2s linear infinite;animation:rotating 2s linear infinite}.el-icon svg{height:1em;width:1em}.el-textarea{--el-input-text-color:var(--el-text-color-regular);--el-input-border:var(--el-border);--el-input-hover-border:var(--el-border-color-hover);--el-input-focus-border:var(--el-color-primary);--el-input-transparent-border:0 0 0 1px transparent inset;--el-input-border-color:var(--el-border-color);--el-input-border-radius:var(--el-border-radius-base);--el-input-bg-color:var(--el-fill-color-blank);--el-input-icon-color:var(--el-text-color-placeholder);--el-input-placeholder-color:var(--el-text-color-placeholder);--el-input-hover-border-color:var(--el-border-color-hover);--el-input-clear-hover-color:var(--el-text-color-secondary);--el-input-focus-border-color:var(--el-color-primary)}.el-textarea{position:relative;display:inline-block;width:100%;vertical-align:bottom;font-size:var(--el-font-size-base)}.el-textarea__inner{position:relative;display:block;resize:vertical;padding:5px 11px;line-height:1.5;box-sizing:border-box;width:100%;font-size:inherit;font-family:inherit;color:var(--el-input-text-color,var(--el-text-color-regular));background-color:var(--el-input-bg-color,var(--el-fill-color-blank));background-image:none;-webkit-appearance:none;box-shadow:0 0 0 1px var(--el-input-border-color,var(--el-border-color)) inset;border-radius:var(--el-input-border-radius,var(--el-border-radius-base));transition:var(--el-transition-box-shadow);border:none}.el-textarea__inner::-moz-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner:-ms-input-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner::placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-textarea__inner:hover{box-shadow:0 0 0 1px var(--el-input-hover-border-color) inset}.el-textarea__inner:focus{outline:0;box-shadow:0 0 0 1px var(--el-input-focus-border-color) inset}.el-textarea .el-input__count{color:var(--el-color-info);background:var(--el-fill-color-blank);position:absolute;font-size:12px;line-height:14px;bottom:5px;right:10px}.el-textarea.is-disabled .el-textarea__inner{background-color:var(--el-disabled-bg-color);border-color:var(--el-disabled-border-color);color:var(--el-disabled-text-color);cursor:not-allowed}.el-textarea.is-disabled .el-textarea__inner::-moz-placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-disabled .el-textarea__inner:-ms-input-placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-disabled .el-textarea__inner::placeholder{color:var(--el-text-color-placeholder)}.el-textarea.is-exceed .el-textarea__inner{border-color:var(--el-color-danger)}.el-textarea.is-exceed .el-input__count{color:var(--el-color-danger)}.el-input{--el-input-text-color:var(--el-text-color-regular);--el-input-border:var(--el-border);--el-input-hover-border:var(--el-border-color-hover);--el-input-focus-border:var(--el-color-primary);--el-input-transparent-border:0 0 0 1px transparent inset;--el-input-border-color:var(--el-border-color);--el-input-border-radius:var(--el-border-radius-base);--el-input-bg-color:var(--el-fill-color-blank);--el-input-icon-color:var(--el-text-color-placeholder);--el-input-placeholder-color:var(--el-text-color-placeholder);--el-input-hover-border-color:var(--el-border-color-hover);--el-input-clear-hover-color:var(--el-text-color-secondary);--el-input-focus-border-color:var(--el-color-primary)}.el-input{--el-input-height:var(--el-component-size);position:relative;font-size:var(--el-font-size-base);display:inline-flex;width:100%;line-height:var(--el-input-height);box-sizing:border-box;vertical-align:middle}.el-input::-webkit-scrollbar{z-index:11;width:6px}.el-input::-webkit-scrollbar:horizontal{height:6px}.el-input::-webkit-scrollbar-thumb{border-radius:5px;width:6px;background:var(--el-text-color-disabled)}.el-input::-webkit-scrollbar-corner{background:var(--el-fill-color-blank)}.el-input::-webkit-scrollbar-track{background:var(--el-fill-color-blank)}.el-input::-webkit-scrollbar-track-piece{background:var(--el-fill-color-blank);width:6px}.el-input .el-input__clear,.el-input .el-input__password{color:var(--el-input-icon-color);font-size:14px;cursor:pointer}.el-input .el-input__clear:hover,.el-input .el-input__password:hover{color:var(--el-input-clear-hover-color)}.el-input .el-input__count{height:100%;display:inline-flex;align-items:center;color:var(--el-color-info);font-size:12px}.el-input .el-input__count .el-input__count-inner{background:var(--el-fill-color-blank);line-height:initial;display:inline-block;padding-left:8px}.el-input__wrapper{display:inline-flex;flex-grow:1;align-items:center;justify-content:center;padding:1px 11px;background-color:var(--el-input-bg-color,var(--el-fill-color-blank));background-image:none;border-radius:var(--el-input-border-radius,var(--el-border-radius-base));transition:var(--el-transition-box-shadow);box-shadow:0 0 0 1px var(--el-input-border-color,var(--el-border-color)) inset}.el-input__wrapper:hover{box-shadow:0 0 0 1px var(--el-input-hover-border-color) inset}.el-input__wrapper.is-focus{box-shadow:0 0 0 1px var(--el-input-focus-border-color) inset}.el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 32px) - 2px);width:100%;flex-grow:1;-webkit-appearance:none;color:var(--el-input-text-color,var(--el-text-color-regular));font-size:inherit;height:var(--el-input-inner-height);line-height:var(--el-input-inner-height);padding:0;outline:0;border:none;background:0 0;box-sizing:border-box}.el-input__inner:focus{outline:0}.el-input__inner::-moz-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner:-ms-input-placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner::placeholder{color:var(--el-input-placeholder-color,var(--el-text-color-placeholder))}.el-input__inner[type=password]::-ms-reveal{display:none}.el-input__prefix{display:inline-flex;white-space:nowrap;flex-shrink:0;flex-wrap:nowrap;height:100%;text-align:center;color:var(--el-input-icon-color,var(--el-text-color-placeholder));transition:all var(--el-transition-duration);pointer-events:none}.el-input__prefix-inner{pointer-events:all;display:inline-flex;align-items:center;justify-content:center}.el-input__prefix-inner>:last-child{margin-right:8px}.el-input__prefix-inner>:first-child,.el-input__prefix-inner>:first-child.el-input__icon{margin-left:0}.el-input__suffix{display:inline-flex;white-space:nowrap;flex-shrink:0;flex-wrap:nowrap;height:100%;text-align:center;color:var(--el-input-icon-color,var(--el-text-color-placeholder));transition:all var(--el-transition-duration);pointer-events:none}.el-input__suffix-inner{pointer-events:all;display:inline-flex;align-items:center;justify-content:center}.el-input__suffix-inner>:first-child{margin-left:8px}.el-input .el-input__icon{height:inherit;line-height:inherit;display:flex;justify-content:center;align-items:center;transition:all var(--el-transition-duration);margin-left:8px}.el-input__validateIcon{pointer-events:none}.el-input.is-active .el-input__wrapper{box-shadow:0 0 0 1px var(--el-input-focus-color,) inset}.el-input.is-disabled{cursor:not-allowed}.el-input.is-disabled .el-input__wrapper{background-color:var(--el-disabled-bg-color);box-shadow:0 0 0 1px var(--el-disabled-border-color) inset}.el-input.is-disabled .el-input__inner{color:var(--el-disabled-text-color);-webkit-text-fill-color:var(--el-disabled-text-color);cursor:not-allowed}.el-input.is-disabled .el-input__inner::-moz-placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__inner:-ms-input-placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__inner::placeholder{color:var(--el-text-color-placeholder)}.el-input.is-disabled .el-input__icon{cursor:not-allowed}.el-input.is-exceed .el-input__wrapper{box-shadow:0 0 0 1px var(--el-color-danger) inset}.el-input.is-exceed .el-input__suffix .el-input__count{color:var(--el-color-danger)}.el-input--large{--el-input-height:var(--el-component-size-large);font-size:14px}.el-input--large .el-input__wrapper{padding:1px 15px}.el-input--large .el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 40px) - 2px)}.el-input--small{--el-input-height:var(--el-component-size-small);font-size:12px}.el-input--small .el-input__wrapper{padding:1px 7px}.el-input--small .el-input__inner{--el-input-inner-height:calc(var(--el-input-height, 24px) - 2px)}.el-input-group{display:inline-flex;width:100%;align-items:stretch}.el-input-group__append,.el-input-group__prepend{background-color:var(--el-fill-color-light);color:var(--el-color-info);position:relative;display:inline-flex;align-items:center;justify-content:center;min-height:100%;border-radius:var(--el-input-border-radius);padding:0 20px;white-space:nowrap}.el-input-group__append:focus,.el-input-group__prepend:focus{outline:0}.el-input-group__append .el-button,.el-input-group__append .el-select,.el-input-group__prepend .el-button,.el-input-group__prepend .el-select{display:inline-block;margin:0 -20px}.el-input-group__append button.el-button,.el-input-group__append button.el-button:hover,.el-input-group__append div.el-select .el-input__wrapper,.el-input-group__append div.el-select:hover .el-input__wrapper,.el-input-group__prepend button.el-button,.el-input-group__prepend button.el-button:hover,.el-input-group__prepend div.el-select .el-input__wrapper,.el-input-group__prepend div.el-select:hover .el-input__wrapper{border-color:transparent;background-color:transparent;color:inherit}.el-input-group__append .el-button,.el-input-group__append .el-input,.el-input-group__prepend .el-button,.el-input-group__prepend .el-input{font-size:inherit}.el-input-group__prepend{border-right:0;border-top-right-radius:0;border-bottom-right-radius:0;box-shadow:1px 0 0 0 var(--el-input-border-color) inset,0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset}.el-input-group__append{border-left:0;border-top-left-radius:0;border-bottom-left-radius:0;box-shadow:0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset,-1px 0 0 0 var(--el-input-border-color) inset}.el-input-group--prepend>.el-input__wrapper{border-top-left-radius:0;border-bottom-left-radius:0}.el-input-group--prepend .el-input-group__prepend .el-select .el-input .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select .el-input .el-input__wrapper{border-top-right-radius:0;border-bottom-right-radius:0;box-shadow:1px 0 0 0 var(--el-input-border-color) inset,0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__wrapper{box-shadow:1px 0 0 0 var(--el-input-focus-border-color) inset,1px 0 0 0 var(--el-input-focus-border-color),0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important;z-index:2}.el-input-group--prepend .el-input-group__prepend .el-select .el-input.is-focus .el-input__wrapper:focus{outline:0;z-index:2;box-shadow:1px 0 0 0 var(--el-input-focus-border-color) inset,1px 0 0 0 var(--el-input-focus-border-color),0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important}.el-input-group--prepend .el-input-group__prepend .el-select:hover .el-input__inner{box-shadow:none!important}.el-input-group--prepend .el-input-group__prepend .el-select:hover .el-input__wrapper{z-index:1;box-shadow:1px 0 0 0 var(--el-input-hover-border-color) inset,1px 0 0 0 var(--el-input-hover-border-color),0 1px 0 0 var(--el-input-hover-border-color) inset,0 -1px 0 0 var(--el-input-hover-border-color) inset!important}.el-input-group--append>.el-input__wrapper{border-top-right-radius:0;border-bottom-right-radius:0}.el-input-group--append .el-input-group__append .el-select .el-input .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select .el-input .el-input__wrapper{border-top-left-radius:0;border-bottom-left-radius:0;box-shadow:0 1px 0 0 var(--el-input-border-color) inset,0 -1px 0 0 var(--el-input-border-color) inset,-1px 0 0 0 var(--el-input-border-color) inset}.el-input-group--append .el-input-group__append .el-select .el-input.is-focus .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select .el-input.is-focus .el-input__wrapper{z-index:2;box-shadow:-1px 0 0 0 var(--el-input-focus-border-color),-1px 0 0 0 var(--el-input-focus-border-color) inset,0 1px 0 0 var(--el-input-focus-border-color) inset,0 -1px 0 0 var(--el-input-focus-border-color) inset!important}.el-input-group--append .el-input-group__append .el-select:hover .el-input__inner{box-shadow:none!important}.el-input-group--append .el-input-group__append .el-select:hover .el-input__wrapper{z-index:1;box-shadow:-1px 0 0 0 var(--el-input-hover-border-color),-1px 0 0 0 var(--el-input-hover-border-color) inset,0 1px 0 0 var(--el-input-hover-border-color) inset,0 -1px 0 0 var(--el-input-hover-border-color) inset!important}.el-tag{--el-tag-font-size:12px;--el-tag-border-radius:4px;--el-tag-border-radius-rounded:9999px}.el-tag{--el-tag-bg-color:var(--el-color-primary-light-9);--el-tag-border-color:var(--el-color-primary-light-8);--el-tag-hover-color:var(--el-color-primary);--el-tag-text-color:var(--el-color-primary);background-color:var(--el-tag-bg-color);border-color:var(--el-tag-border-color);color:var(--el-tag-text-color);display:inline-flex;justify-content:center;align-items:center;height:24px;padding:0 9px;font-size:var(--el-tag-font-size);line-height:1;border-width:1px;border-style:solid;border-radius:var(--el-tag-border-radius);box-sizing:border-box;white-space:nowrap;--el-icon-size:14px}.el-tag.el-tag--primary{--el-tag-bg-color:var(--el-color-primary-light-9);--el-tag-border-color:var(--el-color-primary-light-8);--el-tag-hover-color:var(--el-color-primary)}.el-tag.el-tag--success{--el-tag-bg-color:var(--el-color-success-light-9);--el-tag-border-color:var(--el-color-success-light-8);--el-tag-hover-color:var(--el-color-success)}.el-tag.el-tag--warning{--el-tag-bg-color:var(--el-color-warning-light-9);--el-tag-border-color:var(--el-color-warning-light-8);--el-tag-hover-color:var(--el-color-warning)}.el-tag.el-tag--danger{--el-tag-bg-color:var(--el-color-danger-light-9);--el-tag-border-color:var(--el-color-danger-light-8);--el-tag-hover-color:var(--el-color-danger)}.el-tag.el-tag--error{--el-tag-bg-color:var(--el-color-error-light-9);--el-tag-border-color:var(--el-color-error-light-8);--el-tag-hover-color:var(--el-color-error)}.el-tag.el-tag--info{--el-tag-bg-color:var(--el-color-info-light-9);--el-tag-border-color:var(--el-color-info-light-8);--el-tag-hover-color:var(--el-color-info)}.el-tag.el-tag--primary{--el-tag-text-color:var(--el-color-primary)}.el-tag.el-tag--success{--el-tag-text-color:var(--el-color-success)}.el-tag.el-tag--warning{--el-tag-text-color:var(--el-color-warning)}.el-tag.el-tag--danger{--el-tag-text-color:var(--el-color-danger)}.el-tag.el-tag--error{--el-tag-text-color:var(--el-color-error)}.el-tag.el-tag--info{--el-tag-text-color:var(--el-color-info)}.el-tag.is-hit{border-color:var(--el-color-primary)}.el-tag.is-round{border-radius:var(--el-tag-border-radius-rounded)}.el-tag .el-tag__close{color:var(--el-tag-text-color)}.el-tag .el-tag__close:hover{color:var(--el-color-white);background-color:var(--el-tag-hover-color)}.el-tag .el-icon{border-radius:50%;cursor:pointer;font-size:calc(var(--el-icon-size) - 2px);height:var(--el-icon-size);width:var(--el-icon-size)}.el-tag .el-tag__close{margin-left:6px}.el-tag--dark{--el-tag-bg-color:var(--el-color-primary);--el-tag-border-color:var(--el-color-primary);--el-tag-hover-color:var(--el-color-primary-light-3);--el-tag-text-color:var(--el-color-white)}.el-tag--dark.el-tag--primary{--el-tag-bg-color:var(--el-color-primary);--el-tag-border-color:var(--el-color-primary);--el-tag-hover-color:var(--el-color-primary-light-3)}.el-tag--dark.el-tag--success{--el-tag-bg-color:var(--el-color-success);--el-tag-border-color:var(--el-color-success);--el-tag-hover-color:var(--el-color-success-light-3)}.el-tag--dark.el-tag--warning{--el-tag-bg-color:var(--el-color-warning);--el-tag-border-color:var(--el-color-warning);--el-tag-hover-color:var(--el-color-warning-light-3)}.el-tag--dark.el-tag--danger{--el-tag-bg-color:var(--el-color-danger);--el-tag-border-color:var(--el-color-danger);--el-tag-hover-color:var(--el-color-danger-light-3)}.el-tag--dark.el-tag--error{--el-tag-bg-color:var(--el-color-error);--el-tag-border-color:var(--el-color-error);--el-tag-hover-color:var(--el-color-error-light-3)}.el-tag--dark.el-tag--info{--el-tag-bg-color:var(--el-color-info);--el-tag-border-color:var(--el-color-info);--el-tag-hover-color:var(--el-color-info-light-3)}.el-tag--dark.el-tag--primary,.el-tag--dark.el-tag--success,.el-tag--dark.el-tag--warning,.el-tag--dark.el-tag--danger,.el-tag--dark.el-tag--error,.el-tag--dark.el-tag--info{--el-tag-text-color:var(--el-color-white)}.el-tag--plain{--el-tag-border-color:var(--el-color-primary-light-5);--el-tag-hover-color:var(--el-color-primary);--el-tag-bg-color:var(--el-fill-color-blank)}.el-tag--plain.el-tag--primary{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-primary-light-5);--el-tag-hover-color:var(--el-color-primary)}.el-tag--plain.el-tag--success{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-success-light-5);--el-tag-hover-color:var(--el-color-success)}.el-tag--plain.el-tag--warning{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-warning-light-5);--el-tag-hover-color:var(--el-color-warning)}.el-tag--plain.el-tag--danger{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-danger-light-5);--el-tag-hover-color:var(--el-color-danger)}.el-tag--plain.el-tag--error{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-error-light-5);--el-tag-hover-color:var(--el-color-error)}.el-tag--plain.el-tag--info{--el-tag-bg-color:var(--el-fill-color-blank);--el-tag-border-color:var(--el-color-info-light-5);--el-tag-hover-color:var(--el-color-info)}.el-tag.is-closable{padding-right:5px}.el-tag--large{padding:0 11px;height:32px;--el-icon-size:16px}.el-tag--large .el-tag__close{margin-left:8px}.el-tag--large.is-closable{padding-right:7px}.el-tag--small{padding:0 7px;height:20px;--el-icon-size:12px}.el-tag--small .el-tag__close{margin-left:4px}.el-tag--small.is-closable{padding-right:3px}.el-tag--small .el-icon-close{transform:scale(.8)}.el-tag.el-tag--primary.is-hit{border-color:var(--el-color-primary)}.el-tag.el-tag--success.is-hit{border-color:var(--el-color-success)}.el-tag.el-tag--warning.is-hit{border-color:var(--el-color-warning)}.el-tag.el-tag--danger.is-hit{border-color:var(--el-color-danger)}.el-tag.el-tag--error.is-hit{border-color:var(--el-color-error)}.el-tag.el-tag--info.is-hit{border-color:var(--el-color-info)}.el-scrollbar{--el-scrollbar-opacity:.3;--el-scrollbar-bg-color:var(--el-text-color-secondary);--el-scrollbar-hover-opacity:.5;--el-scrollbar-hover-bg-color:var(--el-text-color-secondary)}.el-scrollbar{overflow:hidden;position:relative;height:100%}.el-scrollbar__wrap{overflow:auto;height:100%}.el-scrollbar__wrap--hidden-default{scrollbar-width:none}.el-scrollbar__wrap--hidden-default::-webkit-scrollbar{display:none}.el-scrollbar__thumb{position:relative;display:block;width:0;height:0;cursor:pointer;border-radius:inherit;background-color:var(--el-scrollbar-bg-color,var(--el-text-color-secondary));transition:var(--el-transition-duration) background-color;opacity:var(--el-scrollbar-opacity,.3)}.el-scrollbar__thumb:hover{background-color:var(--el-scrollbar-hover-bg-color,var(--el-text-color-secondary));opacity:var(--el-scrollbar-hover-opacity,.5)}.el-scrollbar__bar{position:absolute;right:2px;bottom:2px;z-index:1;border-radius:4px}.el-scrollbar__bar.is-vertical{width:6px;top:2px}.el-scrollbar__bar.is-vertical>div{width:100%}.el-scrollbar__bar.is-horizontal{height:6px;left:2px}.el-scrollbar__bar.is-horizontal>div{height:100%}.el-scrollbar-fade-enter-active{transition:opacity .34s ease-out}.el-scrollbar-fade-leave-active{transition:opacity .12s ease-out}.el-scrollbar-fade-enter-from,.el-scrollbar-fade-leave-active{opacity:0}.el-popper{--el-popper-border-radius:var(--el-popover-border-radius, 4px)}.el-popper{position:absolute;border-radius:var(--el-popper-border-radius);padding:5px 11px;z-index:2000;font-size:12px;line-height:20px;min-width:10px;word-wrap:break-word;visibility:visible}.el-popper.is-dark{color:var(--el-bg-color);background:var(--el-text-color-primary);border:1px solid var(--el-text-color-primary)}.el-popper.is-dark .el-popper__arrow:before{border:1px solid var(--el-text-color-primary);background:var(--el-text-color-primary);right:0}.el-popper.is-light{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light)}.el-popper.is-light .el-popper__arrow:before{border:1px solid var(--el-border-color-light);background:var(--el-bg-color-overlay);right:0}.el-popper.is-pure{padding:0}.el-popper__arrow{position:absolute;width:10px;height:10px;z-index:-1}.el-popper__arrow:before{position:absolute;width:10px;height:10px;z-index:-1;content:" ";transform:rotate(45deg);background:var(--el-text-color-primary);box-sizing:border-box}.el-popper[data-popper-placement^=top]>.el-popper__arrow{bottom:-5px}.el-popper[data-popper-placement^=top]>.el-popper__arrow:before{border-bottom-right-radius:2px}.el-popper[data-popper-placement^=bottom]>.el-popper__arrow{top:-5px}.el-popper[data-popper-placement^=bottom]>.el-popper__arrow:before{border-top-left-radius:2px}.el-popper[data-popper-placement^=left]>.el-popper__arrow{right:-5px}.el-popper[data-popper-placement^=left]>.el-popper__arrow:before{border-top-right-radius:2px}.el-popper[data-popper-placement^=right]>.el-popper__arrow{left:-5px}.el-popper[data-popper-placement^=right]>.el-popper__arrow:before{border-bottom-left-radius:2px}.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent!important;border-left-color:transparent!important}.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent!important;border-right-color:transparent!important}.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent!important;border-bottom-color:transparent!important}.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent!important;border-top-color:transparent!important}.el-vl__wrapper{position:relative}.el-vl__wrapper:hover .el-virtual-scrollbar,.el-vl__wrapper.always-on .el-virtual-scrollbar{opacity:1}.el-vl__window{scrollbar-width:none}.el-vl__window::-webkit-scrollbar{display:none}.el-virtual-scrollbar{opacity:0;transition:opacity .34s ease-out}.el-virtual-scrollbar.always-on{opacity:1}.el-vg__wrapper{position:relative}.el-select-dropdown__option-item.is-selected:not(.is-multiple).is-disabled{color:var(--el-text-color-disabled)}.el-select-dropdown__option-item.is-selected:not(.is-multiple).is-disabled:after{background-color:var(--el-text-color-disabled)}.el-select-dropdown__option-item:hover:not(.hover){background-color:transparent}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-disabled.is-selected{color:var(--el-text-color-disabled)}.el-select-dropdown__list{list-style:none;margin:6px 0!important;padding:0!important;box-sizing:border-box}.el-select-dropdown__option-item{font-size:var(--el-select-font-size);padding:0 32px 0 20px;position:relative;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--el-text-color-regular);height:34px;line-height:34px;box-sizing:border-box;cursor:pointer}.el-select-dropdown__option-item.is-disabled{color:var(--el-text-color-placeholder);cursor:not-allowed}.el-select-dropdown__option-item.is-disabled:hover{background-color:var(--el-bg-color)}.el-select-dropdown__option-item.is-selected{background-color:var(--el-fill-color-light);font-weight:700}.el-select-dropdown__option-item.is-selected:not(.is-multiple){color:var(--el-color-primary)}.el-select-dropdown__option-item.hover{background-color:var(--el-fill-color-light)!important}.el-select-dropdown__option-item:hover{background-color:var(--el-fill-color-light)}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay)}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected .el-icon{position:absolute;right:20px;top:0;height:inherit;font-size:12px}.el-select-dropdown.is-multiple .el-select-dropdown__option-item.is-selected .el-icon svg{height:inherit;vertical-align:middle}.el-select-v2{--el-select-border-color-hover:var(--el-border-color-hover);--el-select-disabled-border:var(--el-disabled-border-color);--el-select-font-size:var(--el-font-size-base);--el-select-close-hover-color:var(--el-text-color-secondary);--el-select-input-color:var(--el-text-color-placeholder);--el-select-multiple-input-color:var(--el-text-color-regular);--el-select-input-focus-border-color:var(--el-color-primary);--el-select-input-font-size:14px}.el-select-v2{display:inline-block;position:relative;vertical-align:middle;font-size:14px}.el-select-v2__wrapper{display:flex;align-items:center;flex-wrap:wrap;position:relative;box-sizing:border-box;cursor:pointer;padding:1px 30px 1px 0;border:1px solid var(--el-border-color);border-radius:var(--el-border-radius-base);background-color:var(--el-fill-color-blank);transition:var(--el-transition-duration)}.el-select-v2__wrapper:hover{border-color:var(--el-text-color-placeholder)}.el-select-v2__wrapper.is-filterable{cursor:text}.el-select-v2__wrapper.is-focused{border-color:var(--el-color-primary)}.el-select-v2__wrapper.is-hovering:not(.is-focused){border-color:var(--el-border-color-hover)}.el-select-v2__wrapper.is-disabled{cursor:not-allowed;background-color:var(--el-fill-color-light);color:var(--el-text-color-placeholder);border-color:var(--el-select-disabled-border)}.el-select-v2__wrapper.is-disabled:hover{border-color:var(--el-select-disabled-border)}.el-select-v2__wrapper.is-disabled.is-focus{border-color:var(--el-input-focus-border-color)}.el-select-v2__wrapper.is-disabled .is-transparent{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-select-v2__wrapper.is-disabled .el-select-v2__caret,.el-select-v2__wrapper.is-disabled .el-select-v2__combobox-input{cursor:not-allowed}.el-select-v2__wrapper .el-select-v2__input-wrapper{box-sizing:border-box;position:relative;-webkit-margin-start:12px;margin-inline-start:12px;max-width:100%;overflow:hidden}.el-select-v2__wrapper,.el-select-v2__wrapper .el-select-v2__input-wrapper{line-height:32px}.el-select-v2__wrapper .el-select-v2__input-wrapper input{--el-input-inner-height:calc(var(--el-component-size, 32px) - 8px);height:var(--el-input-inner-height);line-height:var(--el-input-inner-height);min-width:4px;width:100%;background-color:transparent;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:0 0;border:none;margin:2px 0;outline:0;padding:0}.el-select-v2 .el-select-v2__tags-text{display:inline-block;line-height:normal;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-select-v2__empty{padding:10px 0;margin:0;text-align:center;color:var(--el-text-color-secondary);font-size:14px}.el-select-v2__popper.el-popper{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light);box-shadow:var(--el-box-shadow-light)}.el-select-v2__popper.el-popper .el-popper__arrow:before{border:1px solid var(--el-border-color-light)}.el-select-v2__popper.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent;border-left-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent;border-right-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent;border-bottom-color:transparent}.el-select-v2__popper.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent;border-top-color:transparent}.el-select-v2--large .el-select-v2__wrapper .el-select-v2__combobox-input{height:32px}.el-select-v2--large .el-select-v2__caret,.el-select-v2--large .el-select-v2__suffix{height:40px}.el-select-v2--large .el-select-v2__placeholder{font-size:14px;line-height:40px}.el-select-v2--small .el-select-v2__wrapper .el-select-v2__combobox-input{height:16px}.el-select-v2--small .el-select-v2__caret,.el-select-v2--small .el-select-v2__suffix{height:24px}.el-select-v2--small .el-select-v2__placeholder{font-size:12px;line-height:24px}.el-select-v2 .el-select-v2__selection>span{display:inline-block}.el-select-v2:hover .el-select-v2__combobox-input{border-color:var(--el-select-border-color-hover)}.el-select-v2 .el-select__selection-text{text-overflow:ellipsis;display:inline-block;overflow-x:hidden;vertical-align:bottom}.el-select-v2 .el-select-v2__combobox-input{padding-right:35px;display:block;color:var(--el-text-color-regular)}.el-select-v2 .el-select-v2__combobox-input:focus{border-color:var(--el-select-input-focus-border-color)}.el-select-v2__input{border:none;outline:0;padding:0;margin-left:15px;color:var(--el-select-multiple-input-color);font-size:var(--el-select-font-size);-webkit-appearance:none;-moz-appearance:none;appearance:none;height:28px}.el-select-v2__input.is-small{height:14px}.el-select-v2__close{cursor:pointer;position:absolute;top:8px;z-index:var(--el-index-top);right:25px;color:var(--el-select-input-color);line-height:18px;font-size:var(--el-select-input-font-size)}.el-select-v2__close:hover{color:var(--el-select-close-hover-color)}.el-select-v2__suffix{display:inline-flex;position:absolute;right:12px;height:32px;top:50%;transform:translateY(-50%);color:var(--el-input-icon-color,var(--el-text-color-placeholder))}.el-select-v2__suffix .el-input__icon{height:inherit}.el-select-v2__caret{color:var(--el-select-input-color);font-size:var(--el-select-input-font-size);transition:var(--el-transition-duration);transform:rotate(180deg);cursor:pointer}.el-select-v2__caret.is-reverse{transform:rotate(0)}.el-select-v2__caret.is-show-close{font-size:var(--el-select-font-size);text-align:center;transform:rotate(180deg);border-radius:var(--el-border-radius-circle);color:var(--el-select-input-color);transition:var(--el-transition-color)}.el-select-v2__caret.is-show-close:hover{color:var(--el-select-close-hover-color)}.el-select-v2__caret.el-icon{height:inherit}.el-select-v2__caret.el-icon svg{vertical-align:middle}.el-select-v2__selection{white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap}.el-select-v2__input-calculator{left:0;position:absolute;top:0;visibility:hidden;white-space:pre;z-index:999}.el-select-v2__selected-item{line-height:inherit;height:inherit;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;display:flex;flex-wrap:wrap}.el-select-v2__placeholder{position:absolute;top:50%;transform:translateY(-50%);-webkit-margin-start:12px;margin-inline-start:12px;width:calc(100% - 52px);overflow:hidden;text-overflow:ellipsis;white-space:nowrap;color:var(--el-input-text-color,var(--el-text-color-regular))}.el-select-v2__placeholder.is-transparent{color:var(--el-text-color-placeholder)}.el-select-v2 .el-select-v2__selection .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 0 2px 6px;background-color:var(--el-fill-color)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;color:var(--el-color-white)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select-v2 .el-select-v2__selection .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select-v2.el-select-v2--small .el-select-v2__selection .el-tag{margin:1px 0 1px 6px;height:18px}.el-select-dropdown__item{font-size:var(--el-font-size-base);padding:0 32px 0 20px;position:relative;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:var(--el-text-color-regular);height:34px;line-height:34px;box-sizing:border-box;cursor:pointer}.el-select-dropdown__item.is-disabled{color:var(--el-text-color-placeholder);cursor:not-allowed}.el-select-dropdown__item.hover,.el-select-dropdown__item:hover{background-color:var(--el-fill-color-light)}.el-select-dropdown__item.selected{color:var(--el-color-primary);font-weight:700}.el-select-group{margin:0;padding:0}.el-select-group__wrap{position:relative;list-style:none;margin:0;padding:0}.el-select-group__wrap:not(:last-of-type){padding-bottom:24px}.el-select-group__wrap:not(:last-of-type):after{content:"";position:absolute;display:block;left:20px;right:20px;bottom:12px;height:1px;background:var(--el-border-color-light)}.el-select-group__split-dash{position:absolute;left:20px;right:20px;height:1px;background:var(--el-border-color-light)}.el-select-group__title{padding-left:20px;font-size:12px;color:var(--el-color-info);line-height:30px}.el-select-group .el-select-dropdown__item{padding-left:20px}.el-select-dropdown{z-index:calc(var(--el-index-top) + 1);border-radius:var(--el-border-radius-base);box-sizing:border-box}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay)}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected.hover{background-color:var(--el-fill-color-light)}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected:after{content:"";position:absolute;top:50%;right:20px;border-top:none;border-right:none;background-repeat:no-repeat;background-position:center;background-color:var(--el-color-primary);-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask-size:100% 100%;-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;-webkit-mask-size:100% 100%;transform:translateY(-50%);width:12px;height:12px}.el-select-dropdown.is-multiple .el-select-dropdown__item.selected.is-disabled:after{background-color:var(--el-text-color-disabled)}.el-select-dropdown .el-select-dropdown__option-item.is-selected:after{content:"";position:absolute;top:50%;right:20px;border-top:none;border-right:none;background-repeat:no-repeat;background-position:center;background-color:var(--el-color-primary);-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;mask-size:100% 100%;-webkit-mask:url("data:image/svg+xml;utf8,%3Csvg class='icon' width='200' height='200' viewBox='0 0 1024 1024' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M406.656 706.944L195.84 496.256a32 32 0 10-45.248 45.248l256 256 512-512a32 32 0 00-45.248-45.248L406.592 706.944z'%3E%3C/path%3E%3C/svg%3E") no-repeat;-webkit-mask-size:100% 100%;transform:translateY(-50%);width:12px;height:12px}.el-select-dropdown .el-scrollbar.is-empty .el-select-dropdown__list{padding:0}.el-select-dropdown .el-select-dropdown__item.is-disabled:hover{background-color:unset}.el-select-dropdown .el-select-dropdown__item.is-disabled.selected{color:var(--el-text-color-disabled)}.el-select-dropdown__empty{padding:10px 0;margin:0;text-align:center;color:var(--el-text-color-secondary);font-size:var(--el-select-font-size)}.el-select-dropdown__wrap{max-height:274px}.el-select-dropdown__list{list-style:none;padding:6px 0;margin:0;box-sizing:border-box}.el-select{--el-select-border-color-hover:var(--el-border-color-hover);--el-select-disabled-border:var(--el-disabled-border-color);--el-select-font-size:var(--el-font-size-base);--el-select-close-hover-color:var(--el-text-color-secondary);--el-select-input-color:var(--el-text-color-placeholder);--el-select-multiple-input-color:var(--el-text-color-regular);--el-select-input-focus-border-color:var(--el-color-primary);--el-select-input-font-size:14px}.el-select{display:inline-block;position:relative;vertical-align:middle;line-height:32px}.el-select__popper.el-popper{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color-light);box-shadow:var(--el-box-shadow-light)}.el-select__popper.el-popper .el-popper__arrow:before{border:1px solid var(--el-border-color-light)}.el-select__popper.el-popper[data-popper-placement^=top] .el-popper__arrow:before{border-top-color:transparent;border-left-color:transparent}.el-select__popper.el-popper[data-popper-placement^=bottom] .el-popper__arrow:before{border-bottom-color:transparent;border-right-color:transparent}.el-select__popper.el-popper[data-popper-placement^=left] .el-popper__arrow:before{border-left-color:transparent;border-bottom-color:transparent}.el-select__popper.el-popper[data-popper-placement^=right] .el-popper__arrow:before{border-right-color:transparent;border-top-color:transparent}.el-select .el-select-tags-wrapper.has-prefix{margin-left:6px}.el-select--large{line-height:40px}.el-select--large .el-select-tags-wrapper.has-prefix{margin-left:8px}.el-select--small{line-height:24px}.el-select--small .el-select-tags-wrapper.has-prefix{margin-left:4px}.el-select .el-select__tags>span{display:inline-block}.el-select:hover:not(.el-select--disabled) .el-input__wrapper{box-shadow:0 0 0 1px var(--el-select-border-color-hover) inset}.el-select .el-select__tags-text{display:inline-block;line-height:normal;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-select .el-input__wrapper{cursor:pointer}.el-select .el-input__wrapper.is-focus{box-shadow:0 0 0 1px var(--el-select-input-focus-border-color) inset!important}.el-select .el-input__inner{cursor:pointer}.el-select .el-input{display:flex}.el-select .el-input .el-select__caret{color:var(--el-select-input-color);font-size:var(--el-select-input-font-size);transition:transform var(--el-transition-duration);transform:rotate(0);cursor:pointer}.el-select .el-input .el-select__caret.is-reverse{transform:rotate(-180deg)}.el-select .el-input .el-select__caret.is-show-close{font-size:var(--el-select-font-size);text-align:center;transform:rotate(0);border-radius:var(--el-border-radius-circle);color:var(--el-select-input-color);transition:var(--el-transition-color)}.el-select .el-input .el-select__caret.is-show-close:hover{color:var(--el-select-close-hover-color)}.el-select .el-input .el-select__caret.el-icon{position:relative;height:inherit;z-index:2}.el-select .el-input.is-disabled .el-input__wrapper{cursor:not-allowed}.el-select .el-input.is-disabled .el-input__wrapper:hover{box-shadow:0 0 0 1px var(--el-select-disabled-border) inset}.el-select .el-input.is-disabled .el-input__inner,.el-select .el-input.is-disabled .el-select__caret{cursor:not-allowed}.el-select .el-input.is-focus .el-input__wrapper{box-shadow:0 0 0 1px var(--el-select-input-focus-border-color) inset!important}.el-select__input{border:none;outline:0;padding:0;margin-left:15px;color:var(--el-select-multiple-input-color);font-size:var(--el-select-font-size);-webkit-appearance:none;-moz-appearance:none;appearance:none;height:28px;background-color:transparent}.el-select__input.is-small{height:14px}.el-select__close{cursor:pointer;position:absolute;top:8px;z-index:var(--el-index-top);right:25px;color:var(--el-select-input-color);line-height:18px;font-size:var(--el-select-input-font-size)}.el-select__close:hover{color:var(--el-select-close-hover-color)}.el-select__tags{position:absolute;line-height:normal;top:50%;transform:translateY(-50%);white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap;cursor:pointer}.el-select__tags .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 6px 2px 0}.el-select__tags .el-tag:last-child{margin-right:0}.el-select__tags .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;top:0;color:#fff}.el-select__tags .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select__tags .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select__tags .el-tag--info{background-color:var(--el-fill-color)}.el-select__collapse-tags{white-space:normal;z-index:var(--el-index-normal);display:flex;align-items:center;flex-wrap:wrap;cursor:pointer}.el-select__collapse-tags .el-tag{box-sizing:border-box;border-color:transparent;margin:2px 6px 2px 0}.el-select__collapse-tags .el-tag:last-child{margin-right:0}.el-select__collapse-tags .el-tag .el-icon-close{background-color:var(--el-text-color-placeholder);right:-7px;top:0;color:#fff}.el-select__collapse-tags .el-tag .el-icon-close:hover{background-color:var(--el-text-color-secondary)}.el-select__collapse-tags .el-tag .el-icon-close:before{display:block;transform:translateY(.5px)}.el-select__collapse-tags .el-tag--info{background-color:var(--el-fill-color)}.el-select__collapse-tag{line-height:inherit;height:inherit;display:flex}.slicer-box[data-v-ba3d65d0]{margin-right:.8rem}.slicer-box .cp-select[data-v-ba3d65d0]{min-width:11rem}.slicer-box .title[data-v-ba3d65d0]{display:block;margin-bottom:.5rem}.el-pagination{--el-pagination-font-size:14px;--el-pagination-bg-color:var(--el-fill-color-blank);--el-pagination-text-color:var(--el-text-color-primary);--el-pagination-border-radius:2px;--el-pagination-button-color:var(--el-text-color-primary);--el-pagination-button-width:32px;--el-pagination-button-height:32px;--el-pagination-button-disabled-color:var(--el-text-color-placeholder);--el-pagination-button-disabled-bg-color:var(--el-fill-color-blank);--el-pagination-button-bg-color:var(--el-fill-color);--el-pagination-hover-color:var(--el-color-primary);--el-pagination-font-size-small:12px;--el-pagination-button-width-small:24px;--el-pagination-button-height-small:24px;--el-pagination-item-gap:16px;white-space:nowrap;color:var(--el-pagination-text-color);font-size:var(--el-pagination-font-size);font-weight:400;display:flex;align-items:center}.el-pagination .el-input__inner{text-align:center;-moz-appearance:textfield}.el-pagination .el-select .el-input{width:128px}.el-pagination button{display:flex;justify-content:center;align-items:center;font-size:var(--el-pagination-font-size);min-width:var(--el-pagination-button-width);height:var(--el-pagination-button-height);line-height:var(--el-pagination-button-height);color:var(--el-pagination-button-color);background:var(--el-pagination-bg-color);padding:0 4px;border:none;border-radius:var(--el-pagination-border-radius);cursor:pointer;text-align:center;box-sizing:border-box}.el-pagination button *{pointer-events:none}.el-pagination button:focus{outline:0}.el-pagination button:hover{color:var(--el-pagination-hover-color)}.el-pagination button.is-active{color:var(--el-pagination-hover-color);cursor:default;font-weight:700}.el-pagination button.is-active.is-disabled{font-weight:700;color:var(--el-text-color-secondary)}.el-pagination button.is-disabled,.el-pagination button:disabled{color:var(--el-pagination-button-disabled-color);background-color:var(--el-pagination-button-disabled-bg-color);cursor:not-allowed}.el-pagination button:focus-visible{outline:1px solid var(--el-pagination-hover-color);outline-offset:-1px}.el-pagination .btn-next .el-icon,.el-pagination .btn-prev .el-icon{display:block;font-size:12px;font-weight:700;width:inherit}.el-pagination>.is-first{margin-left:0!important}.el-pagination>.is-last{margin-right:0!important}.el-pagination .btn-prev{margin-left:var(--el-pagination-item-gap)}.el-pagination__sizes,.el-pagination__total{margin-left:var(--el-pagination-item-gap);font-weight:400;color:var(--el-text-color-regular)}.el-pagination__total[disabled=true]{color:var(--el-text-color-placeholder)}.el-pagination__jump{display:flex;align-items:center;margin-left:var(--el-pagination-item-gap);font-weight:400;color:var(--el-text-color-regular)}.el-pagination__jump[disabled=true]{color:var(--el-text-color-placeholder)}.el-pagination__goto{margin-right:8px}.el-pagination__editor{text-align:center;box-sizing:border-box}.el-pagination__editor.el-input{width:56px}.el-pagination__editor .el-input__inner::-webkit-inner-spin-button,.el-pagination__editor .el-input__inner::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.el-pagination__classifier{margin-left:8px}.el-pagination__rightwrapper{flex:1;display:flex;align-items:center;justify-content:flex-end}.el-pagination.is-background .btn-next,.el-pagination.is-background .btn-prev,.el-pagination.is-background .el-pager li{margin:0 4px;background-color:var(--el-pagination-button-bg-color)}.el-pagination.is-background .btn-next.is-active,.el-pagination.is-background .btn-prev.is-active,.el-pagination.is-background .el-pager li.is-active{background-color:var(--el-color-primary);color:var(--el-color-white)}.el-pagination.is-background .btn-next.is-disabled,.el-pagination.is-background .btn-next:disabled,.el-pagination.is-background .btn-prev.is-disabled,.el-pagination.is-background .btn-prev:disabled,.el-pagination.is-background .el-pager li.is-disabled,.el-pagination.is-background .el-pager li:disabled{color:var(--el-text-color-placeholder);background-color:var(--el-disabled-bg-color)}.el-pagination.is-background .btn-next.is-disabled.is-active,.el-pagination.is-background .btn-next:disabled.is-active,.el-pagination.is-background .btn-prev.is-disabled.is-active,.el-pagination.is-background .btn-prev:disabled.is-active,.el-pagination.is-background .el-pager li.is-disabled.is-active,.el-pagination.is-background .el-pager li:disabled.is-active{color:var(--el-text-color-secondary);background-color:var(--el-fill-color-dark)}.el-pagination.is-background .btn-prev{margin-left:var(--el-pagination-item-gap)}.el-pagination--small .btn-next,.el-pagination--small .btn-prev,.el-pagination--small .el-pager li{height:var(--el-pagination-button-height-small);line-height:var(--el-pagination-button-height-small);font-size:var(--el-pagination-font-size-small);min-width:var(--el-pagination-button-width-small)}.el-pagination--small button,.el-pagination--small span:not([class*=suffix]){font-size:var(--el-pagination-font-size-small)}.el-pagination--small .el-select .el-input{width:100px}.el-pager{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;list-style:none;font-size:0;padding:0;margin:0;display:flex;align-items:center}.el-pager li{display:flex;justify-content:center;align-items:center;font-size:var(--el-pagination-font-size);min-width:var(--el-pagination-button-width);height:var(--el-pagination-button-height);line-height:var(--el-pagination-button-height);color:var(--el-pagination-button-color);background:var(--el-pagination-bg-color);padding:0 4px;border:none;border-radius:var(--el-pagination-border-radius);cursor:pointer;text-align:center;box-sizing:border-box}.el-pager li *{pointer-events:none}.el-pager li:focus{outline:0}.el-pager li:hover{color:var(--el-pagination-hover-color)}.el-pager li.is-active{color:var(--el-pagination-hover-color);cursor:default;font-weight:700}.el-pager li.is-active.is-disabled{font-weight:700;color:var(--el-text-color-secondary)}.el-pager li.is-disabled,.el-pager li:disabled{color:var(--el-pagination-button-disabled-color);background-color:var(--el-pagination-button-disabled-bg-color);cursor:not-allowed}.el-pager li:focus-visible{outline:1px solid var(--el-pagination-hover-color);outline-offset:-1px}.el-table{--el-table-border-color:var(--el-border-color-lighter);--el-table-border:1px solid var(--el-table-border-color);--el-table-text-color:var(--el-text-color-regular);--el-table-header-text-color:var(--el-text-color-secondary);--el-table-row-hover-bg-color:var(--el-fill-color-light);--el-table-current-row-bg-color:var(--el-color-primary-light-9);--el-table-header-bg-color:var(--el-bg-color);--el-table-fixed-box-shadow:var(--el-box-shadow-light);--el-table-bg-color:var(--el-fill-color-blank);--el-table-tr-bg-color:var(--el-fill-color-blank);--el-table-expanded-cell-bg-color:var(--el-fill-color-blank);--el-table-fixed-left-column:inset 10px 0 10px -10px rgba(0, 0, 0, .15);--el-table-fixed-right-column:inset -10px 0 10px -10px rgba(0, 0, 0, .15)}.el-table{position:relative;overflow:hidden;box-sizing:border-box;height:-webkit-fit-content;height:-moz-fit-content;height:fit-content;width:100%;max-width:100%;background-color:var(--el-table-bg-color);font-size:14px;color:var(--el-table-text-color)}.el-table__inner-wrapper{position:relative;display:flex;flex-direction:column;height:100%}.el-table__inner-wrapper:before{left:0;bottom:0;width:100%;height:1px}.el-table.has-footer.el-table--fluid-height tr:last-child td.el-table__cell,.el-table.has-footer.el-table--scrollable-y tr:last-child td.el-table__cell{border-bottom-color:transparent}.el-table__empty-block{position:-webkit-sticky;position:sticky;left:0;min-height:60px;text-align:center;width:100%;display:flex;justify-content:center;align-items:center}.el-table__empty-text{line-height:60px;width:50%;color:var(--el-text-color-secondary)}.el-table__expand-column .cell{padding:0;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-table__expand-icon{position:relative;cursor:pointer;color:var(--el-text-color-regular);font-size:12px;transition:transform var(--el-transition-duration-fast) ease-in-out;height:20px}.el-table__expand-icon--expanded{transform:rotate(90deg)}.el-table__expand-icon>.el-icon{font-size:12px}.el-table__expanded-cell{background-color:var(--el-table-expanded-cell-bg-color)}.el-table__expanded-cell[class*=cell]{padding:20px 50px}.el-table__expanded-cell:hover{background-color:transparent!important}.el-table__placeholder{display:inline-block;width:20px}.el-table__append-wrapper{overflow:hidden}.el-table--fit{border-right:0;border-bottom:0}.el-table--fit .el-table__cell.gutter{border-right-width:1px}.el-table thead{color:var(--el-table-header-text-color);font-weight:500}.el-table thead.is-group th.el-table__cell{background:var(--el-fill-color-light)}.el-table .el-table__cell{padding:8px 0;min-width:0;box-sizing:border-box;text-overflow:ellipsis;vertical-align:middle;position:relative;text-align:left;z-index:1}.el-table .el-table__cell.is-center{text-align:center}.el-table .el-table__cell.is-right{text-align:right}.el-table .el-table__cell.gutter{width:15px;border-right-width:0;border-bottom-width:0;padding:0}.el-table .el-table__cell.is-hidden>*{visibility:hidden}.el-table .cell{box-sizing:border-box;overflow:hidden;text-overflow:ellipsis;white-space:normal;word-break:break-all;line-height:23px;padding:0 12px}.el-table .cell.el-tooltip{white-space:nowrap;min-width:50px}.el-table--large{font-size:var(--el-font-size-base)}.el-table--large .el-table__cell{padding:12px 0}.el-table--large .cell{padding:0 16px}.el-table--default{font-size:14px}.el-table--default .el-table__cell{padding:8px 0}.el-table--default .cell{padding:0 12px}.el-table--small{font-size:12px}.el-table--small .el-table__cell{padding:4px 0}.el-table--small .cell{padding:0 8px}.el-table tr{background-color:var(--el-table-tr-bg-color)}.el-table tr input[type=checkbox]{margin:0}.el-table td.el-table__cell,.el-table th.el-table__cell.is-leaf{border-bottom:var(--el-table-border)}.el-table th.el-table__cell.is-sortable{cursor:pointer}.el-table th.el-table__cell{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-color:var(--el-table-header-bg-color)}.el-table th.el-table__cell>.cell.highlight{color:var(--el-color-primary)}.el-table th.el-table__cell.required>div:before{display:inline-block;content:"";width:8px;height:8px;border-radius:50%;background:#ff4d51;margin-right:5px;vertical-align:middle}.el-table td.el-table__cell div{box-sizing:border-box}.el-table td.el-table__cell.gutter{width:0}.el-table__footer-wrapper{border-top:var(--el-table-border)}.el-table--border .el-table__inner-wrapper:after,.el-table--border:after,.el-table--border:before,.el-table__inner-wrapper:before{content:"";position:absolute;background-color:var(--el-table-border-color);z-index:3}.el-table--border .el-table__inner-wrapper:after{left:0;top:0;width:100%;height:1px}.el-table--border:before{top:-1px;left:0;width:1px;height:100%}.el-table--border:after{top:-1px;right:0;width:1px;height:100%}.el-table--border .el-table__inner-wrapper{border-right:none;border-bottom:none}.el-table--border .el-table__footer-wrapper{position:relative;flex-shrink:0}.el-table--border .el-table__cell{border-right:var(--el-table-border)}.el-table--border th.el-table__cell.gutter:last-of-type{border-bottom:var(--el-table-border);border-bottom-width:1px}.el-table--border th.el-table__cell{border-bottom:var(--el-table-border)}.el-table--hidden{visibility:hidden}.el-table__body-wrapper,.el-table__footer-wrapper,.el-table__header-wrapper{width:100%}.el-table__body-wrapper tr td.el-table-fixed-column--left,.el-table__body-wrapper tr td.el-table-fixed-column--right,.el-table__body-wrapper tr th.el-table-fixed-column--left,.el-table__body-wrapper tr th.el-table-fixed-column--right,.el-table__footer-wrapper tr td.el-table-fixed-column--left,.el-table__footer-wrapper tr td.el-table-fixed-column--right,.el-table__footer-wrapper tr th.el-table-fixed-column--left,.el-table__footer-wrapper tr th.el-table-fixed-column--right,.el-table__header-wrapper tr td.el-table-fixed-column--left,.el-table__header-wrapper tr td.el-table-fixed-column--right,.el-table__header-wrapper tr th.el-table-fixed-column--left,.el-table__header-wrapper tr th.el-table-fixed-column--right{position:-webkit-sticky!important;position:sticky!important;z-index:2;background:var(--el-bg-color)}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-last-column:before{content:"";position:absolute;top:0;width:10px;bottom:-1px;overflow-x:hidden;overflow-y:hidden;box-shadow:none;touch-action:none;pointer-events:none}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-first-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-first-column:before{left:-10px}.el-table__body-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__body-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__footer-wrapper tr th.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr td.el-table-fixed-column--right.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--left.is-last-column:before,.el-table__header-wrapper tr th.el-table-fixed-column--right.is-last-column:before{right:-10px;box-shadow:none}.el-table__body-wrapper tr td.el-table__fixed-right-patch,.el-table__body-wrapper tr th.el-table__fixed-right-patch,.el-table__footer-wrapper tr td.el-table__fixed-right-patch,.el-table__footer-wrapper tr th.el-table__fixed-right-patch,.el-table__header-wrapper tr td.el-table__fixed-right-patch,.el-table__header-wrapper tr th.el-table__fixed-right-patch{position:-webkit-sticky!important;position:sticky!important;z-index:2;background:#fff;right:0}.el-table__header-wrapper{flex-shrink:0}.el-table__header-wrapper tr th.el-table-fixed-column--left,.el-table__header-wrapper tr th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table__body,.el-table__footer,.el-table__header{table-layout:fixed;border-collapse:separate}.el-table__footer-wrapper,.el-table__header-wrapper{overflow:hidden}.el-table__footer-wrapper tbody td.el-table__cell,.el-table__header-wrapper tbody td.el-table__cell{background-color:var(--el-table-row-hover-bg-color);color:var(--el-table-text-color)}.el-table__body-wrapper .el-table-column--selection>.cell,.el-table__header-wrapper .el-table-column--selection>.cell{display:inline-flex;align-items:center;height:23px}.el-table__body-wrapper .el-table-column--selection .el-checkbox,.el-table__header-wrapper .el-table-column--selection .el-checkbox{height:unset}.el-table.is-scrolling-left .el-table-fixed-column--right.is-first-column:before{box-shadow:var(--el-table-fixed-right-column)}.el-table.is-scrolling-left.el-table--border .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:var(--el-table-border)}.el-table.is-scrolling-left th.el-table-fixed-column--left{background-color:var(--el-table-header-bg-color)}.el-table.is-scrolling-right .el-table-fixed-column--left.is-last-column:before{box-shadow:var(--el-table-fixed-left-column)}.el-table.is-scrolling-right .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:none}.el-table.is-scrolling-right th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table.is-scrolling-middle .el-table-fixed-column--left.is-last-column.el-table__cell{border-right:none}.el-table.is-scrolling-middle .el-table-fixed-column--right.is-first-column:before{box-shadow:var(--el-table-fixed-right-column)}.el-table.is-scrolling-middle .el-table-fixed-column--left.is-last-column:before{box-shadow:var(--el-table-fixed-left-column)}.el-table.is-scrolling-none .el-table-fixed-column--left.is-first-column:before,.el-table.is-scrolling-none .el-table-fixed-column--left.is-last-column:before,.el-table.is-scrolling-none .el-table-fixed-column--right.is-first-column:before,.el-table.is-scrolling-none .el-table-fixed-column--right.is-last-column:before{box-shadow:none}.el-table.is-scrolling-none th.el-table-fixed-column--left,.el-table.is-scrolling-none th.el-table-fixed-column--right{background-color:var(--el-table-header-bg-color)}.el-table__body-wrapper{overflow:hidden;position:relative;flex:1}.el-table__body-wrapper .el-scrollbar__bar{z-index:2}.el-table .caret-wrapper{display:inline-flex;flex-direction:column;align-items:center;height:14px;width:24px;vertical-align:middle;cursor:pointer;overflow:initial;position:relative}.el-table .sort-caret{width:0;height:0;border:solid 5px transparent;position:absolute;left:7px}.el-table .sort-caret.ascending{border-bottom-color:var(--el-text-color-placeholder);top:-5px}.el-table .sort-caret.descending{border-top-color:var(--el-text-color-placeholder);bottom:-3px}.el-table .ascending .sort-caret.ascending{border-bottom-color:var(--el-color-primary)}.el-table .descending .sort-caret.descending{border-top-color:var(--el-color-primary)}.el-table .hidden-columns{visibility:hidden;position:absolute;z-index:-1}.el-table--striped .el-table__body tr.el-table__row--striped td.el-table__cell{background:var(--el-fill-color-lighter)}.el-table--striped .el-table__body tr.el-table__row--striped.current-row td.el-table__cell{background-color:var(--el-table-current-row-bg-color)}.el-table__body tr.hover-row.current-row>td.el-table__cell,.el-table__body tr.hover-row.el-table__row--striped.current-row>td.el-table__cell,.el-table__body tr.hover-row.el-table__row--striped>td.el-table__cell,.el-table__body tr.hover-row>td.el-table__cell{background-color:var(--el-table-row-hover-bg-color)}.el-table__body tr.current-row>td.el-table__cell{background-color:var(--el-table-current-row-bg-color)}.el-table__column-resize-proxy{position:absolute;left:200px;top:0;bottom:0;width:0;border-left:var(--el-table-border);z-index:10}.el-table__column-filter-trigger{display:inline-block;cursor:pointer}.el-table__column-filter-trigger i{color:var(--el-color-info);font-size:14px;vertical-align:middle}.el-table__border-left-patch{top:0;left:0;width:1px;height:100%;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table__border-bottom-patch{left:0;height:1px;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table__border-right-patch{top:0;height:100%;width:1px;z-index:3;position:absolute;background-color:var(--el-table-border-color)}.el-table--enable-row-transition .el-table__body td.el-table__cell{transition:background-color .25s ease}.el-table--enable-row-hover .el-table__body tr:hover>td.el-table__cell{background-color:var(--el-table-row-hover-bg-color)}.el-table [class*=el-table__row--level] .el-table__expand-icon{display:inline-block;width:12px;line-height:12px;height:12px;text-align:center;margin-right:8px}.el-table .el-table.el-table--border .el-table__cell{border-right:var(--el-table-border)}.el-table:not(.el-table--border) .el-table__cell{border-right:none}.el-table:not(.el-table--border)>.el-table__inner-wrapper:after{content:none}.el-checkbox{--el-checkbox-font-size:14px;--el-checkbox-font-weight:var(--el-font-weight-primary);--el-checkbox-text-color:var(--el-text-color-regular);--el-checkbox-input-height:14px;--el-checkbox-input-width:14px;--el-checkbox-border-radius:var(--el-border-radius-small);--el-checkbox-bg-color:var(--el-fill-color-blank);--el-checkbox-input-border:var(--el-border);--el-checkbox-disabled-border-color:var(--el-border-color);--el-checkbox-disabled-input-fill:var(--el-fill-color-light);--el-checkbox-disabled-icon-color:var(--el-text-color-placeholder);--el-checkbox-disabled-checked-input-fill:var(--el-border-color-extra-light);--el-checkbox-disabled-checked-input-border-color:var(--el-border-color);--el-checkbox-disabled-checked-icon-color:var(--el-text-color-placeholder);--el-checkbox-checked-text-color:var(--el-color-primary);--el-checkbox-checked-input-border-color:var(--el-color-primary);--el-checkbox-checked-bg-color:var(--el-color-primary);--el-checkbox-checked-icon-color:var(--el-color-white);--el-checkbox-input-border-color-hover:var(--el-color-primary)}.el-checkbox{color:var(--el-checkbox-text-color);font-weight:var(--el-checkbox-font-weight);font-size:var(--el-font-size-base);position:relative;cursor:pointer;display:inline-flex;align-items:center;white-space:nowrap;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;margin-right:30px;height:32px}.el-checkbox.is-bordered{padding:0 15px 0 9px;border-radius:var(--el-border-radius-base);border:var(--el-border);box-sizing:border-box}.el-checkbox.is-bordered.is-checked{border-color:var(--el-color-primary)}.el-checkbox.is-bordered.is-disabled{border-color:var(--el-border-color-lighter);cursor:not-allowed}.el-checkbox.is-bordered.el-checkbox--large{padding:0 19px 0 11px;border-radius:var(--el-border-radius-base)}.el-checkbox.is-bordered.el-checkbox--large .el-checkbox__label{font-size:var(--el-font-size-base)}.el-checkbox.is-bordered.el-checkbox--large .el-checkbox__inner{height:14px;width:14px}.el-checkbox.is-bordered.el-checkbox--small{padding:0 11px 0 7px;border-radius:calc(var(--el-border-radius-base) - 1px)}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__label{font-size:12px}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__inner{height:12px;width:12px}.el-checkbox.is-bordered.el-checkbox--small .el-checkbox__inner:after{height:6px;width:2px}.el-checkbox input:focus-visible+.el-checkbox__inner{outline:2px solid var(--el-checkbox-input-border-color-hover);outline-offset:1px;border-radius:var(--el-checkbox-border-radius)}.el-checkbox__input{white-space:nowrap;cursor:pointer;outline:0;display:inline-flex;position:relative}.el-checkbox__input.is-disabled .el-checkbox__inner{background-color:var(--el-checkbox-disabled-input-fill);border-color:var(--el-checkbox-disabled-border-color);cursor:not-allowed}.el-checkbox__input.is-disabled .el-checkbox__inner:after{cursor:not-allowed;border-color:var(--el-checkbox-disabled-icon-color)}.el-checkbox__input.is-disabled .el-checkbox__inner+.el-checkbox__label{cursor:not-allowed}.el-checkbox__input.is-disabled.is-checked .el-checkbox__inner{background-color:var(--el-checkbox-disabled-checked-input-fill);border-color:var(--el-checkbox-disabled-checked-input-border-color)}.el-checkbox__input.is-disabled.is-checked .el-checkbox__inner:after{border-color:var(--el-checkbox-disabled-checked-icon-color)}.el-checkbox__input.is-disabled.is-indeterminate .el-checkbox__inner{background-color:var(--el-checkbox-disabled-checked-input-fill);border-color:var(--el-checkbox-disabled-checked-input-border-color)}.el-checkbox__input.is-disabled.is-indeterminate .el-checkbox__inner:before{background-color:var(--el-checkbox-disabled-checked-icon-color);border-color:var(--el-checkbox-disabled-checked-icon-color)}.el-checkbox__input.is-disabled+span.el-checkbox__label{color:var(--el-disabled-text-color);cursor:not-allowed}.el-checkbox__input.is-checked .el-checkbox__inner{background-color:var(--el-checkbox-checked-bg-color);border-color:var(--el-checkbox-checked-input-border-color)}.el-checkbox__input.is-checked .el-checkbox__inner:after{transform:rotate(45deg) scaleY(1)}.el-checkbox__input.is-checked+.el-checkbox__label{color:var(--el-checkbox-checked-text-color)}.el-checkbox__input.is-focus:not(.is-checked) .el-checkbox__original:not(:focus-visible){border-color:var(--el-checkbox-input-border-color-hover)}.el-checkbox__input.is-indeterminate .el-checkbox__inner{background-color:var(--el-checkbox-checked-bg-color);border-color:var(--el-checkbox-checked-input-border-color)}.el-checkbox__input.is-indeterminate .el-checkbox__inner:before{content:"";position:absolute;display:block;background-color:var(--el-checkbox-checked-icon-color);height:2px;transform:scale(.5);left:0;right:0;top:5px}.el-checkbox__input.is-indeterminate .el-checkbox__inner:after{display:none}.el-checkbox__inner{display:inline-block;position:relative;border:var(--el-checkbox-input-border);border-radius:var(--el-checkbox-border-radius);box-sizing:border-box;width:var(--el-checkbox-input-width);height:var(--el-checkbox-input-height);background-color:var(--el-checkbox-bg-color);z-index:var(--el-index-normal);transition:border-color .25s cubic-bezier(.71,-.46,.29,1.46),background-color .25s cubic-bezier(.71,-.46,.29,1.46),outline .25s cubic-bezier(.71,-.46,.29,1.46)}.el-checkbox__inner:hover{border-color:var(--el-checkbox-input-border-color-hover)}.el-checkbox__inner:after{box-sizing:content-box;content:"";border:1px solid var(--el-checkbox-checked-icon-color);border-left:0;border-top:0;height:7px;left:4px;position:absolute;top:1px;transform:rotate(45deg) scaleY(0);width:3px;transition:transform .15s ease-in 50ms;transform-origin:center}.el-checkbox__original{opacity:0;outline:0;position:absolute;margin:0;width:0;height:0;z-index:-1}.el-checkbox__label{display:inline-block;padding-left:8px;line-height:1;font-size:var(--el-checkbox-font-size)}.el-checkbox.el-checkbox--large{height:40px}.el-checkbox.el-checkbox--large .el-checkbox__label{font-size:14px}.el-checkbox.el-checkbox--large .el-checkbox__inner{width:14px;height:14px}.el-checkbox.el-checkbox--small{height:24px}.el-checkbox.el-checkbox--small .el-checkbox__label{font-size:12px}.el-checkbox.el-checkbox--small .el-checkbox__inner{width:12px;height:12px}.el-checkbox.el-checkbox--small .el-checkbox__input.is-indeterminate .el-checkbox__inner:before{top:4px}.el-checkbox.el-checkbox--small .el-checkbox__inner:after{width:2px;height:6px}.el-checkbox:last-of-type{margin-right:0}.el-table-column--selection .cell{padding-left:14px;padding-right:14px}.el-table-filter{border:solid 1px var(--el-border-color-lighter);border-radius:2px;background-color:#fff;box-shadow:var(--el-box-shadow-light);box-sizing:border-box}.el-table-filter__list{padding:5px 0;margin:0;list-style:none;min-width:100px}.el-table-filter__list-item{line-height:36px;padding:0 10px;cursor:pointer;font-size:var(--el-font-size-base)}.el-table-filter__list-item:hover{background-color:var(--el-color-primary-light-9);color:var(--el-color-primary)}.el-table-filter__list-item.is-active{background-color:var(--el-color-primary);color:#fff}.el-table-filter__content{min-width:100px}.el-table-filter__bottom{border-top:1px solid var(--el-border-color-lighter);padding:8px}.el-table-filter__bottom button{background:0 0;border:none;color:var(--el-text-color-regular);cursor:pointer;font-size:var(--el-font-size-small);padding:0 3px}.el-table-filter__bottom button:hover{color:var(--el-color-primary)}.el-table-filter__bottom button:focus{outline:0}.el-table-filter__bottom button.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-table-filter__wrap{max-height:280px}.el-table-filter__checkbox-group{padding:10px}.el-table-filter__checkbox-group label.el-checkbox{display:flex;align-items:center;margin-right:5px;margin-bottom:12px;margin-left:5px;height:unset}.el-table-filter__checkbox-group .el-checkbox:last-child{margin-bottom:0}.bi-table[data-v-4fd4d173]{overflow:auto;height:var(--9c25e776)}.bi-table .table-fix[data-v-4fd4d173]{flex:1;min-width:var(--21675e16);width:var(--6bc0968e)}.bi-table .table[data-v-4fd4d173]{margin-bottom:2rem}.bi-table[data-v-4fd4d173] .table-header th{font-size:1.1em;font-weight:700;background-color:#8fe1fd16}.el-upload{--el-upload-dragger-padding-horizontal:40px;--el-upload-dragger-padding-vertical:10px}.el-upload{display:inline-flex;justify-content:center;align-items:center;cursor:pointer;outline:0}.el-upload__input{display:none}.el-upload__tip{font-size:12px;color:var(--el-text-color-regular);margin-top:7px}.el-upload iframe{position:absolute;z-index:-1;top:0;left:0;opacity:0}.el-upload--picture-card{--el-upload-picture-card-size:148px;background-color:var(--el-fill-color-lighter);border:1px dashed var(--el-border-color-darker);border-radius:6px;box-sizing:border-box;width:var(--el-upload-picture-card-size);height:var(--el-upload-picture-card-size);cursor:pointer;vertical-align:top;display:inline-flex;justify-content:center;align-items:center}.el-upload--picture-card i{font-size:28px;color:var(--el-text-color-secondary)}.el-upload--picture-card:hover{border-color:var(--el-color-primary);color:var(--el-color-primary)}.el-upload.is-drag{display:block}.el-upload:focus{border-color:var(--el-color-primary);color:var(--el-color-primary)}.el-upload:focus .el-upload-dragger{border-color:var(--el-color-primary)}.el-upload-dragger{padding:var(--el-upload-dragger-padding-horizontal) var(--el-upload-dragger-padding-vertical);background-color:var(--el-fill-color-blank);border:1px dashed var(--el-border-color);border-radius:6px;box-sizing:border-box;text-align:center;cursor:pointer;position:relative;overflow:hidden}.el-upload-dragger .el-icon--upload{font-size:67px;color:var(--el-text-color-placeholder);margin-bottom:16px;line-height:50px}.el-upload-dragger+.el-upload__tip{text-align:center}.el-upload-dragger~.el-upload__files{border-top:var(--el-border);margin-top:7px;padding-top:5px}.el-upload-dragger .el-upload__text{color:var(--el-text-color-regular);font-size:14px;text-align:center}.el-upload-dragger .el-upload__text em{color:var(--el-color-primary);font-style:normal}.el-upload-dragger:hover{border-color:var(--el-color-primary)}.el-upload-dragger.is-dragover{padding:calc(var(--el-upload-dragger-padding-horizontal) - 1px) calc(var(--el-upload-dragger-padding-vertical) - 1px);background-color:var(--el-color-primary-light-9);border:2px dashed var(--el-color-primary)}.el-upload-list{margin:10px 0 0;padding:0;list-style:none;position:relative}.el-upload-list__item{transition:all .5s cubic-bezier(.55,0,.1,1);font-size:14px;color:var(--el-text-color-regular);margin-bottom:5px;position:relative;box-sizing:border-box;border-radius:4px;width:100%}.el-upload-list__item .el-progress{position:absolute;top:20px;width:100%}.el-upload-list__item .el-progress__text{position:absolute;right:0;top:-13px}.el-upload-list__item .el-progress-bar{margin-right:0;padding-right:0}.el-upload-list__item .el-icon--upload-success{color:var(--el-color-success)}.el-upload-list__item .el-icon--close{display:none;position:absolute;right:5px;top:50%;cursor:pointer;opacity:.75;color:var(--el-text-color-regular);transition:opacity var(--el-transition-duration);transform:translateY(-50%)}.el-upload-list__item .el-icon--close:hover{opacity:1;color:var(--el-color-primary)}.el-upload-list__item .el-icon--close-tip{display:none;position:absolute;top:1px;right:5px;font-size:12px;cursor:pointer;opacity:1;color:var(--el-color-primary);font-style:normal}.el-upload-list__item:hover{background-color:var(--el-fill-color-light)}.el-upload-list__item:hover .el-icon--close{display:inline-flex}.el-upload-list__item:hover .el-progress__text{display:none}.el-upload-list__item .el-upload-list__item-info{display:inline-flex;justify-content:center;flex-direction:column;width:calc(100% - 30px);margin-left:4px}.el-upload-list__item.is-success .el-upload-list__item-status-label{display:inline-flex}.el-upload-list__item.is-success .el-upload-list__item-name:focus,.el-upload-list__item.is-success .el-upload-list__item-name:hover{color:var(--el-color-primary);cursor:pointer}.el-upload-list__item.is-success:focus:not(:hover) .el-icon--close-tip{display:inline-block}.el-upload-list__item.is-success:active,.el-upload-list__item.is-success:not(.focusing):focus{outline-width:0}.el-upload-list__item.is-success:active .el-icon--close-tip,.el-upload-list__item.is-success:not(.focusing):focus .el-icon--close-tip{display:none}.el-upload-list__item.is-success:focus .el-upload-list__item-status-label,.el-upload-list__item.is-success:hover .el-upload-list__item-status-label{display:none;opacity:0}.el-upload-list.is-disabled .el-upload-list__item-status-label,.el-upload-list.is-disabled .el-upload-list__item:hover{display:block}.el-upload-list__item-name{color:var(--el-text-color-regular);display:inline-flex;text-align:center;align-items:center;padding:0 4px;transition:color var(--el-transition-duration);font-size:var(--el-font-size-base)}.el-upload-list__item-name .el-icon{margin-right:6px;color:var(--el-text-color-secondary)}.el-upload-list__item-file-name{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.el-upload-list__item-status-label{position:absolute;right:5px;top:0;line-height:inherit;display:none;height:100%;justify-content:center;align-items:center;transition:opacity var(--el-transition-duration)}.el-upload-list__item-delete{position:absolute;right:10px;top:0;font-size:12px;color:var(--el-text-color-regular);display:none}.el-upload-list__item-delete:hover{color:var(--el-color-primary)}.el-upload-list--picture-card{--el-upload-list-picture-card-size:148px;display:inline-flex;flex-wrap:wrap;margin:0}.el-upload-list--picture-card .el-upload-list__item{overflow:hidden;background-color:var(--el-fill-color-blank);border:1px solid var(--el-border-color);border-radius:6px;box-sizing:border-box;width:var(--el-upload-list-picture-card-size);height:var(--el-upload-list-picture-card-size);margin:0 8px 8px 0;padding:0;display:inline-flex}.el-upload-list--picture-card .el-upload-list__item .el-icon--check,.el-upload-list--picture-card .el-upload-list__item .el-icon--circle-check{color:#fff}.el-upload-list--picture-card .el-upload-list__item .el-icon--close{display:none}.el-upload-list--picture-card .el-upload-list__item:hover .el-upload-list__item-status-label{opacity:0;display:block}.el-upload-list--picture-card .el-upload-list__item:hover .el-progress__text{display:block}.el-upload-list--picture-card .el-upload-list__item .el-upload-list__item-name{display:none}.el-upload-list--picture-card .el-upload-list__item-thumbnail{width:100%;height:100%;-o-object-fit:contain;object-fit:contain}.el-upload-list--picture-card .el-upload-list__item-status-label{right:-15px;top:-6px;width:40px;height:24px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-list--picture-card .el-upload-list__item-status-label i{font-size:12px;margin-top:11px;transform:rotate(-45deg)}.el-upload-list--picture-card .el-upload-list__item-actions{position:absolute;width:100%;height:100%;left:0;top:0;cursor:default;display:inline-flex;justify-content:center;align-items:center;color:#fff;opacity:0;font-size:20px;background-color:var(--el-overlay-color-lighter);transition:opacity var(--el-transition-duration)}.el-upload-list--picture-card .el-upload-list__item-actions span{display:none;cursor:pointer}.el-upload-list--picture-card .el-upload-list__item-actions span+span{margin-left:1rem}.el-upload-list--picture-card .el-upload-list__item-actions .el-upload-list__item-delete{position:static;font-size:inherit;color:inherit}.el-upload-list--picture-card .el-upload-list__item-actions:hover{opacity:1}.el-upload-list--picture-card .el-upload-list__item-actions:hover span{display:inline-flex}.el-upload-list--picture-card .el-progress{top:50%;left:50%;transform:translate(-50%,-50%);bottom:auto;width:126px}.el-upload-list--picture-card .el-progress .el-progress__text{top:50%}.el-upload-list--picture .el-upload-list__item{overflow:hidden;z-index:0;background-color:var(--el-fill-color-blank);border:1px solid var(--el-border-color);border-radius:6px;box-sizing:border-box;margin-top:10px;padding:10px;display:flex;align-items:center}.el-upload-list--picture .el-upload-list__item .el-icon--check,.el-upload-list--picture .el-upload-list__item .el-icon--circle-check{color:#fff}.el-upload-list--picture .el-upload-list__item:hover .el-upload-list__item-status-label{opacity:0;display:block}.el-upload-list--picture .el-upload-list__item:hover .el-progress__text{display:block}.el-upload-list--picture .el-upload-list__item.is-success .el-upload-list__item-name i{display:none}.el-upload-list--picture .el-upload-list__item .el-icon--close{top:5px;transform:translateY(0)}.el-upload-list--picture .el-upload-list__item-thumbnail{display:inline-flex;justify-content:center;align-items:center;width:70px;height:70px;-o-object-fit:contain;object-fit:contain;position:relative;z-index:1;background-color:var(--el-color-white)}.el-upload-list--picture .el-upload-list__item-status-label{position:absolute;right:-17px;top:-7px;width:46px;height:26px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-list--picture .el-upload-list__item-status-label i{font-size:12px;margin-top:12px;transform:rotate(-45deg)}.el-upload-list--picture .el-progress{position:relative;top:-7px}.el-upload-cover{position:absolute;left:0;top:0;width:100%;height:100%;overflow:hidden;z-index:10;cursor:default}.el-upload-cover:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-upload-cover img{display:block;width:100%;height:100%}.el-upload-cover__label{right:-15px;top:-6px;width:40px;height:24px;background:var(--el-color-success);text-align:center;transform:rotate(45deg)}.el-upload-cover__label i{font-size:12px;margin-top:11px;transform:rotate(-45deg);color:#fff}.el-upload-cover__progress{display:inline-block;vertical-align:middle;position:static;width:243px}.el-upload-cover__progress+.el-upload__inner{opacity:0}.el-upload-cover__content{position:absolute;top:0;left:0;width:100%;height:100%}.el-upload-cover__interact{position:absolute;bottom:0;left:0;width:100%;height:100%;background-color:var(--el-overlay-color-light);text-align:center}.el-upload-cover__interact .btn{display:inline-block;color:#fff;font-size:14px;cursor:pointer;vertical-align:middle;transition:var(--el-transition-md-fade);margin-top:60px}.el-upload-cover__interact .btn i{margin-top:0}.el-upload-cover__interact .btn span{opacity:0;transition:opacity .15s linear}.el-upload-cover__interact .btn:not(:first-child){margin-left:35px}.el-upload-cover__interact .btn:hover{transform:translateY(-13px)}.el-upload-cover__interact .btn:hover span{opacity:1}.el-upload-cover__interact .btn i{color:#fff;display:block;font-size:24px;line-height:inherit;margin:0 auto 5px}.el-upload-cover__title{position:absolute;bottom:0;left:0;background-color:#fff;height:36px;width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;font-weight:400;text-align:left;padding:0 10px;margin:0;line-height:36px;font-size:14px;color:var(--el-text-color-primary)}.el-upload-cover+.el-upload__inner{opacity:0;position:relative;z-index:1}.el-progress{position:relative;line-height:1;display:flex;align-items:center}.el-progress__text{font-size:14px;color:var(--el-text-color-regular);margin-left:5px;min-width:50px;line-height:1}.el-progress__text i{vertical-align:middle;display:block}.el-progress--circle,.el-progress--dashboard{display:inline-block}.el-progress--circle .el-progress__text,.el-progress--dashboard .el-progress__text{position:absolute;top:50%;left:0;width:100%;text-align:center;margin:0;transform:translateY(-50%)}.el-progress--circle .el-progress__text i,.el-progress--dashboard .el-progress__text i{vertical-align:middle;display:inline-block}.el-progress--without-text .el-progress__text{display:none}.el-progress--without-text .el-progress-bar{padding-right:0;margin-right:0;display:block}.el-progress--text-inside .el-progress-bar{padding-right:0;margin-right:0}.el-progress.is-success .el-progress-bar__inner{background-color:var(--el-color-success)}.el-progress.is-success .el-progress__text{color:var(--el-color-success)}.el-progress.is-warning .el-progress-bar__inner{background-color:var(--el-color-warning)}.el-progress.is-warning .el-progress__text{color:var(--el-color-warning)}.el-progress.is-exception .el-progress-bar__inner{background-color:var(--el-color-danger)}.el-progress.is-exception .el-progress__text{color:var(--el-color-danger)}.el-progress-bar{flex-grow:1;box-sizing:border-box}.el-progress-bar__outer{height:6px;border-radius:100px;background-color:var(--el-border-color-lighter);overflow:hidden;position:relative;vertical-align:middle}.el-progress-bar__inner{position:absolute;left:0;top:0;height:100%;background-color:var(--el-color-primary);text-align:right;border-radius:100px;line-height:1;white-space:nowrap;transition:width .6s ease}.el-progress-bar__inner:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-progress-bar__inner--indeterminate{transform:translateZ(0);-webkit-animation:indeterminate 3s infinite;animation:indeterminate 3s infinite}.el-progress-bar__innerText{display:inline-block;vertical-align:middle;color:#fff;font-size:12px;margin:0 5px}@-webkit-keyframes progress{0%{background-position:0 0}to{background-position:32px 0}}@keyframes progress{0%{background-position:0 0}to{background-position:32px 0}}@-webkit-keyframes indeterminate{0%{left:-100%}to{left:100%}}@keyframes indeterminate{0%{left:-100%}to{left:100%}}.slicer-box[data-v-0804f81c]{display:inline-block;min-width:12rem;margin-right:.8rem}.title[data-v-0804f81c]{margin-bottom:.5rem}.el-tabs{--el-tabs-header-height:40px}.el-tabs__header{padding:0;position:relative;margin:0 0 15px}.el-tabs__active-bar{position:absolute;bottom:0;left:0;height:2px;background-color:var(--el-color-primary);z-index:1;transition:width var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier),transform var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);list-style:none}.el-tabs__new-tab{display:flex;align-items:center;justify-content:center;float:right;border:1px solid var(--el-border-color);height:20px;width:20px;line-height:20px;margin:10px 0 10px 10px;border-radius:3px;text-align:center;font-size:12px;color:var(--el-text-color-primary);cursor:pointer;transition:all .15s}.el-tabs__new-tab .is-icon-plus{height:inherit;width:inherit;transform:scale(.8)}.el-tabs__new-tab .is-icon-plus svg{vertical-align:middle}.el-tabs__new-tab:hover{color:var(--el-color-primary)}.el-tabs__nav-wrap{overflow:hidden;margin-bottom:-1px;position:relative}.el-tabs__nav-wrap:after{content:"";position:absolute;left:0;bottom:0;width:100%;height:2px;background-color:var(--el-border-color-light);z-index:var(--el-index-normal)}.el-tabs__nav-wrap.is-scrollable{padding:0 20px;box-sizing:border-box}.el-tabs__nav-scroll{overflow:hidden}.el-tabs__nav-next,.el-tabs__nav-prev{position:absolute;cursor:pointer;line-height:44px;font-size:12px;color:var(--el-text-color-secondary);width:20px;text-align:center}.el-tabs__nav-next{right:0}.el-tabs__nav-prev{left:0}.el-tabs__nav{white-space:nowrap;position:relative;transition:transform var(--el-transition-duration);float:left;z-index:calc(var(--el-index-normal) + 1)}.el-tabs__nav.is-stretch{min-width:100%;display:flex}.el-tabs__nav.is-stretch>*{flex:1;text-align:center}.el-tabs__item{padding:0 20px;height:var(--el-tabs-header-height);box-sizing:border-box;line-height:var(--el-tabs-header-height);display:inline-block;list-style:none;font-size:var(--el-font-size-base);font-weight:500;color:var(--el-text-color-primary);position:relative}.el-tabs__item:focus,.el-tabs__item:focus:active{outline:0}.el-tabs__item:focus-visible{box-shadow:0 0 2px 2px var(--el-color-primary) inset;border-radius:3px}.el-tabs__item .is-icon-close{border-radius:50%;text-align:center;transition:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);margin-left:5px}.el-tabs__item .is-icon-close:before{transform:scale(.9);display:inline-block}.el-tabs__item .is-icon-close:hover{background-color:var(--el-text-color-placeholder);color:#fff}.el-tabs__item .is-icon-close svg{margin-top:1px}.el-tabs__item.is-active{color:var(--el-color-primary)}.el-tabs__item:hover{color:var(--el-color-primary);cursor:pointer}.el-tabs__item.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-tabs__content{overflow:hidden;position:relative}.el-tabs--card>.el-tabs__header{border-bottom:1px solid var(--el-border-color-light);height:var(--el-tabs-header-height)}.el-tabs--card>.el-tabs__header .el-tabs__nav-wrap:after{content:none}.el-tabs--card>.el-tabs__header .el-tabs__nav{border:1px solid var(--el-border-color-light);border-bottom:none;border-radius:4px 4px 0 0;box-sizing:border-box}.el-tabs--card>.el-tabs__header .el-tabs__active-bar{display:none}.el-tabs--card>.el-tabs__header .el-tabs__item .is-icon-close{position:relative;font-size:12px;width:0;height:14px;vertical-align:middle;line-height:15px;overflow:hidden;top:-1px;right:-2px;transform-origin:100% 50%}.el-tabs--card>.el-tabs__header .el-tabs__item{border-bottom:1px solid transparent;border-left:1px solid var(--el-border-color-light);transition:color var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier),padding var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier)}.el-tabs--card>.el-tabs__header .el-tabs__item:first-child{border-left:none}.el-tabs--card>.el-tabs__header .el-tabs__item.is-closable:hover{padding-left:13px;padding-right:13px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-closable:hover .is-icon-close{width:14px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active{border-bottom-color:var(--el-bg-color)}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active.is-closable{padding-left:20px;padding-right:20px}.el-tabs--card>.el-tabs__header .el-tabs__item.is-active.is-closable .is-icon-close{width:14px}.el-tabs--border-card{background:var(--el-bg-color-overlay);border:1px solid var(--el-border-color)}.el-tabs--border-card>.el-tabs__content{padding:15px}.el-tabs--border-card>.el-tabs__header{background-color:var(--el-fill-color-light);border-bottom:1px solid var(--el-border-color-light);margin:0}.el-tabs--border-card>.el-tabs__header .el-tabs__nav-wrap:after{content:none}.el-tabs--border-card>.el-tabs__header .el-tabs__item{transition:all var(--el-transition-duration) var(--el-transition-function-ease-in-out-bezier);border:1px solid transparent;margin-top:-1px;color:var(--el-text-color-secondary)}.el-tabs--border-card>.el-tabs__header .el-tabs__item:first-child{margin-left:-1px}.el-tabs--border-card>.el-tabs__header .el-tabs__item+.el-tabs__item{margin-left:-1px}.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active{color:var(--el-color-primary);background-color:var(--el-bg-color-overlay);border-right-color:var(--el-border-color);border-left-color:var(--el-border-color)}.el-tabs--border-card>.el-tabs__header .el-tabs__item:not(.is-disabled):hover{color:var(--el-color-primary)}.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-disabled{color:var(--el-disabled-text-color)}.el-tabs--border-card>.el-tabs__header .is-scrollable .el-tabs__item:first-child{margin-left:0}.el-tabs--bottom .el-tabs__item.is-bottom:nth-child(2),.el-tabs--bottom .el-tabs__item.is-top:nth-child(2),.el-tabs--top .el-tabs__item.is-bottom:nth-child(2),.el-tabs--top .el-tabs__item.is-top:nth-child(2){padding-left:0}.el-tabs--bottom .el-tabs__item.is-bottom:last-child,.el-tabs--bottom .el-tabs__item.is-top:last-child,.el-tabs--top .el-tabs__item.is-bottom:last-child,.el-tabs--top .el-tabs__item.is-top:last-child{padding-right:0}.el-tabs--bottom .el-tabs--left>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom .el-tabs--right>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom.el-tabs--border-card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--bottom.el-tabs--card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top .el-tabs--left>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top .el-tabs--right>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top.el-tabs--border-card>.el-tabs__header .el-tabs__item:nth-child(2),.el-tabs--top.el-tabs--card>.el-tabs__header .el-tabs__item:nth-child(2){padding-left:20px}.el-tabs--bottom .el-tabs--left>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom .el-tabs--right>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom.el-tabs--border-card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--bottom.el-tabs--card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top .el-tabs--left>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top .el-tabs--right>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top.el-tabs--border-card>.el-tabs__header .el-tabs__item:last-child,.el-tabs--top.el-tabs--card>.el-tabs__header .el-tabs__item:last-child{padding-right:20px}.el-tabs--bottom .el-tabs__header.is-bottom{margin-bottom:0;margin-top:10px}.el-tabs--bottom.el-tabs--border-card .el-tabs__header.is-bottom{border-bottom:0;border-top:1px solid var(--el-border-color)}.el-tabs--bottom.el-tabs--border-card .el-tabs__nav-wrap.is-bottom{margin-top:-1px;margin-bottom:0}.el-tabs--bottom.el-tabs--border-card .el-tabs__item.is-bottom:not(.is-active){border:1px solid transparent}.el-tabs--bottom.el-tabs--border-card .el-tabs__item.is-bottom{margin:0 -1px -1px}.el-tabs--left,.el-tabs--right{overflow:hidden}.el-tabs--left .el-tabs__header.is-left,.el-tabs--left .el-tabs__header.is-right,.el-tabs--left .el-tabs__nav-scroll,.el-tabs--left .el-tabs__nav-wrap.is-left,.el-tabs--left .el-tabs__nav-wrap.is-right,.el-tabs--right .el-tabs__header.is-left,.el-tabs--right .el-tabs__header.is-right,.el-tabs--right .el-tabs__nav-scroll,.el-tabs--right .el-tabs__nav-wrap.is-left,.el-tabs--right .el-tabs__nav-wrap.is-right{height:100%}.el-tabs--left .el-tabs__active-bar.is-left,.el-tabs--left .el-tabs__active-bar.is-right,.el-tabs--right .el-tabs__active-bar.is-left,.el-tabs--right .el-tabs__active-bar.is-right{top:0;bottom:auto;width:2px;height:auto}.el-tabs--left .el-tabs__nav-wrap.is-left,.el-tabs--left .el-tabs__nav-wrap.is-right,.el-tabs--right .el-tabs__nav-wrap.is-left,.el-tabs--right .el-tabs__nav-wrap.is-right{margin-bottom:0}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev{height:30px;line-height:30px;width:100%;text-align:center;cursor:pointer}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next i,.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev i,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next i,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev i,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next i,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev i,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next i,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev i{transform:rotate(90deg)}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-prev,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-prev{left:auto;top:0}.el-tabs--left .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--left .el-tabs__nav-wrap.is-right>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-left>.el-tabs__nav-next,.el-tabs--right .el-tabs__nav-wrap.is-right>.el-tabs__nav-next{right:auto;bottom:0}.el-tabs--left .el-tabs__nav-wrap.is-left.is-scrollable,.el-tabs--left .el-tabs__nav-wrap.is-right.is-scrollable,.el-tabs--right .el-tabs__nav-wrap.is-left.is-scrollable,.el-tabs--right .el-tabs__nav-wrap.is-right.is-scrollable{padding:30px 0}.el-tabs--left .el-tabs__nav-wrap.is-left:after,.el-tabs--left .el-tabs__nav-wrap.is-right:after,.el-tabs--right .el-tabs__nav-wrap.is-left:after,.el-tabs--right .el-tabs__nav-wrap.is-right:after{height:100%;width:2px;bottom:auto;top:0}.el-tabs--left .el-tabs__nav.is-left,.el-tabs--left .el-tabs__nav.is-right,.el-tabs--right .el-tabs__nav.is-left,.el-tabs--right .el-tabs__nav.is-right{float:none}.el-tabs--left .el-tabs__item.is-left,.el-tabs--left .el-tabs__item.is-right,.el-tabs--right .el-tabs__item.is-left,.el-tabs--right .el-tabs__item.is-right{display:block}.el-tabs--left .el-tabs__header.is-left{float:left;margin-bottom:0;margin-right:10px}.el-tabs--left .el-tabs__nav-wrap.is-left{margin-right:-1px}.el-tabs--left .el-tabs__nav-wrap.is-left:after{left:auto;right:0}.el-tabs--left .el-tabs__active-bar.is-left{right:0;left:auto}.el-tabs--left .el-tabs__item.is-left{text-align:right}.el-tabs--left.el-tabs--card .el-tabs__active-bar.is-left{display:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left{border-left:none;border-right:1px solid var(--el-border-color-light);border-bottom:none;border-top:1px solid var(--el-border-color-light);text-align:left}.el-tabs--left.el-tabs--card .el-tabs__item.is-left:first-child{border-right:1px solid var(--el-border-color-light);border-top:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active{border:1px solid var(--el-border-color-light);border-right-color:#fff;border-left:none;border-bottom:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active:first-child{border-top:none}.el-tabs--left.el-tabs--card .el-tabs__item.is-left.is-active:last-child{border-bottom:none}.el-tabs--left.el-tabs--card .el-tabs__nav{border-radius:4px 0 0 4px;border-bottom:1px solid var(--el-border-color-light);border-right:none}.el-tabs--left.el-tabs--card .el-tabs__new-tab{float:none}.el-tabs--left.el-tabs--border-card .el-tabs__header.is-left{border-right:1px solid var(--el-border-color)}.el-tabs--left.el-tabs--border-card .el-tabs__item.is-left{border:1px solid transparent;margin:-1px 0 -1px -1px}.el-tabs--left.el-tabs--border-card .el-tabs__item.is-left.is-active{border-color:transparent;border-top-color:#d1dbe5;border-bottom-color:#d1dbe5}.el-tabs--right .el-tabs__header.is-right{float:right;margin-bottom:0;margin-left:10px}.el-tabs--right .el-tabs__nav-wrap.is-right{margin-left:-1px}.el-tabs--right .el-tabs__nav-wrap.is-right:after{left:0;right:auto}.el-tabs--right .el-tabs__active-bar.is-right{left:0}.el-tabs--right.el-tabs--card .el-tabs__active-bar.is-right{display:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right{border-bottom:none;border-top:1px solid var(--el-border-color-light)}.el-tabs--right.el-tabs--card .el-tabs__item.is-right:first-child{border-left:1px solid var(--el-border-color-light);border-top:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active{border:1px solid var(--el-border-color-light);border-left-color:#fff;border-right:none;border-bottom:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active:first-child{border-top:none}.el-tabs--right.el-tabs--card .el-tabs__item.is-right.is-active:last-child{border-bottom:none}.el-tabs--right.el-tabs--card .el-tabs__nav{border-radius:0 4px 4px 0;border-bottom:1px solid var(--el-border-color-light);border-left:none}.el-tabs--right.el-tabs--border-card .el-tabs__header.is-right{border-left:1px solid var(--el-border-color)}.el-tabs--right.el-tabs--border-card .el-tabs__item.is-right{border:1px solid transparent;margin:-1px -1px -1px 0}.el-tabs--right.el-tabs--border-card .el-tabs__item.is-right.is-active{border-color:transparent;border-top-color:#d1dbe5;border-bottom-color:#d1dbe5}.slideInLeft-transition,.slideInRight-transition{display:inline-block}.slideInRight-enter{-webkit-animation:slideInRight-enter var(--el-transition-duration);animation:slideInRight-enter var(--el-transition-duration)}.slideInRight-leave{position:absolute;left:0;right:0;-webkit-animation:slideInRight-leave var(--el-transition-duration);animation:slideInRight-leave var(--el-transition-duration)}.slideInLeft-enter{-webkit-animation:slideInLeft-enter var(--el-transition-duration);animation:slideInLeft-enter var(--el-transition-duration)}.slideInLeft-leave{position:absolute;left:0;right:0;-webkit-animation:slideInLeft-leave var(--el-transition-duration);animation:slideInLeft-leave var(--el-transition-duration)}@-webkit-keyframes slideInRight-enter{0%{opacity:0;transform-origin:0 0;transform:translate(100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@keyframes slideInRight-enter{0%{opacity:0;transform-origin:0 0;transform:translate(100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@-webkit-keyframes slideInRight-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(100%);opacity:0}}@keyframes slideInRight-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(100%);opacity:0}}@-webkit-keyframes slideInLeft-enter{0%{opacity:0;transform-origin:0 0;transform:translate(-100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@keyframes slideInLeft-enter{0%{opacity:0;transform-origin:0 0;transform:translate(-100%)}to{opacity:1;transform-origin:0 0;transform:translate(0)}}@-webkit-keyframes slideInLeft-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(-100%);opacity:0}}@keyframes slideInLeft-leave{0%{transform-origin:0 0;transform:translate(0);opacity:1}to{transform-origin:0 0;transform:translate(-100%);opacity:0}}.pybi-tabs[data-v-499efce4],.pybi-tabs .el-cp-tabs[data-v-499efce4]{width:100%}.pybi-tabs .custom-tabs-label[data-v-499efce4]{font-size:1.5em;width:100%;display:flex;flex-direction:row;justify-content:center;align-items:center}.pybi-tabs .custom-tabs-label .tab-name[data-v-499efce4]{margin-left:.5em}.el-affix--fixed{position:fixed}.pybi-input[data-v-184ceae1]{width:18em}.el-slider{--el-slider-main-bg-color:var(--el-color-primary);--el-slider-runway-bg-color:var(--el-border-color-light);--el-slider-stop-bg-color:var(--el-color-white);--el-slider-disabled-color:var(--el-text-color-placeholder);--el-slider-border-radius:3px;--el-slider-height:6px;--el-slider-button-size:20px;--el-slider-button-wrapper-size:36px;--el-slider-button-wrapper-offset:-15px}.el-slider{width:100%;height:32px;display:flex;align-items:center}.el-slider__runway{flex:1;height:var(--el-slider-height);background-color:var(--el-slider-runway-bg-color);border-radius:var(--el-slider-border-radius);position:relative;cursor:pointer}.el-slider__runway.show-input{margin-right:30px;width:auto}.el-slider__runway.is-disabled{cursor:default}.el-slider__runway.is-disabled .el-slider__bar{background-color:var(--el-slider-disabled-color)}.el-slider__runway.is-disabled .el-slider__button{border-color:var(--el-slider-disabled-color)}.el-slider__runway.is-disabled .el-slider__button-wrapper.hover,.el-slider__runway.is-disabled .el-slider__button-wrapper:hover,.el-slider__runway.is-disabled .el-slider__button-wrapper.dragging{cursor:not-allowed}.el-slider__runway.is-disabled .el-slider__button.dragging,.el-slider__runway.is-disabled .el-slider__button.hover,.el-slider__runway.is-disabled .el-slider__button:hover{transform:scale(1)}.el-slider__runway.is-disabled .el-slider__button.hover,.el-slider__runway.is-disabled .el-slider__button:hover,.el-slider__runway.is-disabled .el-slider__button.dragging{cursor:not-allowed}.el-slider__input{flex-shrink:0;width:130px}.el-slider__bar{height:var(--el-slider-height);background-color:var(--el-slider-main-bg-color);border-top-left-radius:var(--el-slider-border-radius);border-bottom-left-radius:var(--el-slider-border-radius);position:absolute}.el-slider__button-wrapper{height:var(--el-slider-button-wrapper-size);width:var(--el-slider-button-wrapper-size);position:absolute;z-index:1;top:var(--el-slider-button-wrapper-offset);transform:translate(-50%);background-color:transparent;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;line-height:normal;outline:0}.el-slider__button-wrapper:after{display:inline-block;content:"";height:100%;vertical-align:middle}.el-slider__button-wrapper.hover,.el-slider__button-wrapper:hover{cursor:-webkit-grab;cursor:grab}.el-slider__button-wrapper.dragging{cursor:-webkit-grabbing;cursor:grabbing}.el-slider__button{display:inline-block;width:var(--el-slider-button-size);height:var(--el-slider-button-size);vertical-align:middle;border:solid 2px var(--el-slider-main-bg-color);background-color:var(--el-color-white);border-radius:50%;box-sizing:border-box;transition:var(--el-transition-duration-fast);-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-slider__button.dragging,.el-slider__button.hover,.el-slider__button:hover{transform:scale(1.2)}.el-slider__button.hover,.el-slider__button:hover{cursor:-webkit-grab;cursor:grab}.el-slider__button.dragging{cursor:-webkit-grabbing;cursor:grabbing}.el-slider__stop{position:absolute;height:var(--el-slider-height);width:var(--el-slider-height);border-radius:var(--el-border-radius-circle);background-color:var(--el-slider-stop-bg-color);transform:translate(-50%)}.el-slider__marks{top:0;left:12px;width:18px;height:100%}.el-slider__marks-text{position:absolute;transform:translate(-50%);font-size:14px;color:var(--el-color-info);margin-top:15px;white-space:pre}.el-slider.is-vertical{position:relative;display:inline-flex;width:auto;height:100%;flex:0}.el-slider.is-vertical .el-slider__runway{width:var(--el-slider-height);height:100%;margin:0 16px}.el-slider.is-vertical .el-slider__bar{width:var(--el-slider-height);height:auto;border-radius:0 0 3px 3px}.el-slider.is-vertical .el-slider__button-wrapper{top:auto;left:var(--el-slider-button-wrapper-offset);transform:translateY(50%)}.el-slider.is-vertical .el-slider__stop{transform:translateY(50%)}.el-slider.is-vertical .el-slider__marks-text{margin-top:0;left:15px;transform:translateY(50%)}.el-slider--large{height:40px}.el-slider--small{height:24px}.el-input-number{position:relative;display:inline-flex;width:150px;line-height:30px}.el-input-number .el-input__wrapper{padding-left:42px;padding-right:42px}.el-input-number .el-input__inner{-webkit-appearance:none;-moz-appearance:textfield;text-align:center;line-height:1}.el-input-number .el-input__inner::-webkit-inner-spin-button,.el-input-number .el-input__inner::-webkit-outer-spin-button{margin:0;-webkit-appearance:none}.el-input-number__decrease,.el-input-number__increase{display:flex;justify-content:center;align-items:center;height:auto;position:absolute;z-index:1;top:1px;bottom:1px;width:32px;background:var(--el-fill-color-light);color:var(--el-text-color-regular);cursor:pointer;font-size:13px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.el-input-number__decrease:hover,.el-input-number__increase:hover{color:var(--el-color-primary)}.el-input-number__decrease:hover~.el-input:not(.is-disabled) .el-input_wrapper,.el-input-number__increase:hover~.el-input:not(.is-disabled) .el-input_wrapper{box-shadow:0 0 0 1px var(--el-input-focus-border-color,var(--el-color-primary)) inset}.el-input-number__decrease.is-disabled,.el-input-number__increase.is-disabled{color:var(--el-disabled-text-color);cursor:not-allowed}.el-input-number__increase{right:1px;border-radius:0 var(--el-border-radius-base) var(--el-border-radius-base) 0;border-left:var(--el-border)}.el-input-number__decrease{left:1px;border-radius:var(--el-border-radius-base) 0 0 var(--el-border-radius-base);border-right:var(--el-border)}.el-input-number.is-disabled .el-input-number__decrease,.el-input-number.is-disabled .el-input-number__increase{border-color:var(--el-disabled-border-color);color:var(--el-disabled-border-color)}.el-input-number.is-disabled .el-input-number__decrease:hover,.el-input-number.is-disabled .el-input-number__increase:hover{color:var(--el-disabled-border-color);cursor:not-allowed}.el-input-number--large{width:180px;line-height:38px}.el-input-number--large .el-input-number__decrease,.el-input-number--large .el-input-number__increase{width:40px;font-size:14px}.el-input-number--large .el-input__wrapper{padding-left:47px;padding-right:47px}.el-input-number--small{width:120px;line-height:22px}.el-input-number--small .el-input-number__decrease,.el-input-number--small .el-input-number__increase{width:24px;font-size:12px}.el-input-number--small .el-input__wrapper{padding-left:31px;padding-right:31px}.el-input-number--small .el-input-number__decrease [class*=el-icon],.el-input-number--small .el-input-number__increase [class*=el-icon]{transform:scale(.9)}.el-input-number.is-without-controls .el-input__wrapper{padding-left:15px;padding-right:15px}.el-input-number.is-controls-right .el-input__wrapper{padding-left:15px;padding-right:42px}.el-input-number.is-controls-right .el-input-number__decrease,.el-input-number.is-controls-right .el-input-number__increase{--el-input-number-controls-height:15px;height:var(--el-input-number-controls-height);line-height:var(--el-input-number-controls-height)}.el-input-number.is-controls-right .el-input-number__decrease [class*=el-icon],.el-input-number.is-controls-right .el-input-number__increase [class*=el-icon]{transform:scale(.8)}.el-input-number.is-controls-right .el-input-number__increase{bottom:auto;left:auto;border-radius:0 var(--el-border-radius-base) 0 0;border-bottom:var(--el-border)}.el-input-number.is-controls-right .el-input-number__decrease{right:1px;top:auto;left:auto;border-right:none;border-left:var(--el-border);border-radius:0 0 var(--el-border-radius-base) 0}.el-input-number.is-controls-right[class*=large] [class*=decrease],.el-input-number.is-controls-right[class*=large] [class*=increase]{--el-input-number-controls-height:19px}.el-input-number.is-controls-right[class*=small] [class*=decrease],.el-input-number.is-controls-right[class*=small] [class*=increase]{--el-input-number-controls-height:11px}.pybi-input[data-v-91c5aa8f]{min-width:15em;width:100%}
```

### Comparing `pybi-next-0.4.1/pybi/static/elementCps.iife.js` & `pybi-next-0.4.2/pybi/static/elementCps.iife.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -16789,14 +16789,15 @@
                         iconId: c
                     })),
                     a = t.ref(o.names[0]);
                 return (i, s) => {
                     const c = z2,
                         d = P2;
                     return t.openBlock(), t.createElementBlock("div", _v, [t.createVNode(d, t.mergeProps({
+                        class: "el-cp-tabs",
                         modelValue: a.value,
                         "onUpdate:modelValue": s[0] || (s[0] = u => a.value = u)
                     }, t.unref(o).tabsProps), {
                         default: t.withCtx(() => [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(t.unref(r), u => (t.openBlock(), t.createBlock(c, t.mergeProps(t.unref(o).panelsProps, {
                             name: u.name,
                             label: u.name
                         }), {
@@ -16817,15 +16818,15 @@
                         _: 1
                     }, 16, ["modelValue"])])
                 }
             }
         }),
         mk = "",
         xv = yn(Vv, [
-            ["__scopeId", "data-v-2d2e93ca"]
+            ["__scopeId", "data-v-499efce4"]
         ]),
         hk = "",
         Pv = {
             class: "pybi-container"
         },
         zv = t.defineComponent({
             __name: "Affix",
@@ -16885,15 +16886,16 @@
         gk = "",
         Mv = yn(Rv, [
             ["__scopeId", "data-v-184ceae1"]
         ]),
         bk = "",
         yk = "",
         Lv = {
-            class: "pybi-input"
+            class: "pybi-input",
+            "data-pybi-auto-width": ""
         },
         Av = t.defineComponent({
             __name: "NumberSlider",
             props: {
                 model: null
             },
             setup(e) {
@@ -16950,11 +16952,11 @@
         cp: zv
     }, {
         tag: "elInput",
         cp: Mv
     }, {
         tag: "elNumberSlider",
         cp: yn(Av, [
-            ["__scopeId", "data-v-0c578138"]
+            ["__scopeId", "data-v-91c5aa8f"]
         ])
     }]
 }(Vue);
```

### Comparing `pybi-next-0.4.1/pybi/static/mermaidCps.iife.js` & `pybi-next-0.4.2/pybi/static/mermaidCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/static/province_map_full.json` & `pybi-next-0.4.2/pybi/static/province_map_full.json`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/static/sysApp.iife.js` & `pybi-next-0.4.2/pybi/static/sysApp.iife.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,922 +1,908 @@
 var sysApp = function(K) {
     "use strict";
-    const qw = "";
-    var pA = (A => (A.App = "App", A.DataSource = "DataSource", A.Slicer = "Slicer", A.Markdown = "Markdown", A.Table = "Table", A.Box = "Box", A.ColBox = "ColBox", A.GridBox = "GridBox", A.FlowBox = "FlowBox", A.EChart = "EChart", A.Upload = "Upload", A.TextValue = "TextValue", A.Tabs = "Tabs", A.Icon = "Icon", A.SvgIcon = "SvgIcon", A))(pA || {});
-    const ZB = "sqlAnalyzeKey",
-        TB = "componentKey",
-        WB = "datasetKey",
-        OB = "dbKey",
-        xI = "utilsKey",
-        XB = "reactdataServicesKey",
-        vB = "dynamicComponentKey",
+    const Vw = "";
+    var pA = (A => (A.App = "App", A.DataSource = "DataSource", A.Slicer = "Slicer", A.Markdown = "Markdown", A.Table = "Table", A.Box = "Box", A.ColBox = "ColBox", A.GridBox = "GridBox", A.FlowBox = "FlowBox", A.EChart = "EChart", A.Upload = "Upload", A.TextValue = "TextValue", A.Tabs = "Tabs", A.Icon = "Icon", A.SvgIcon = "SvgIcon", A.Space = "Space", A))(pA || {});
+    const TB = "sqlAnalyzeKey",
+        WB = "componentKey",
+        OB = "datasetKey",
+        XB = "dbKey",
+        bI = "utilsKey",
+        vB = "reactdataServicesKey",
+        jB = "dynamicComponentKey",
         vg = "metaInfoKey",
-        jB = "webResourcesServiceKey",
-        PB = {
+        PB = "webResourcesServiceKey",
+        zB = {
             key: 1,
             class: "err"
         },
-        zB = K.defineComponent({
+        _B = K.defineComponent({
             __name: "Error",
             setup(A) {
                 const B = K.inject(vg),
                     g = K.ref({
                         has: !1,
                         msg: ""
                     });
                 return K.onErrorCaptured((o, t, E) => (console.log(o), g.value.has ? g.value.msg + "" + o.message : g.value = {
                     has: !0,
                     msg: o.message
-                }, !1)), (o, t) => g.value.has ? (K.openBlock(), K.createElementBlock("div", PB, [K.createElementVNode("p", null, "error[version:" + K.toDisplayString(K.unref(B).version) + "]:", 1), K.createElementVNode("p", null, K.toDisplayString(g.value.msg), 1)])) : K.renderSlot(o.$slots, "default", {
+                }, !1)), (o, t) => g.value.has ? (K.openBlock(), K.createElementBlock("div", zB, [K.createElementVNode("p", null, "error[version:" + K.toDisplayString(K.unref(B).version) + "]:", 1), K.createElementVNode("p", null, K.toDisplayString(g.value.msg), 1)])) : K.renderSlot(o.$slots, "default", {
                     key: 0
                 }, void 0, !0)
             }
         }),
-        xw = "",
+        mw = "",
         WA = (A, B) => {
             const g = A.__vccOpts || A;
             for (const [o, t] of B) g[o] = t;
             return g
         },
-        jg = WA(zB, [
+        jg = WA(_B, [
             ["__scopeId", "data-v-2e3c5a01"]
         ]),
-        _B = ["data-tag"],
-        $B = K.defineComponent({
+        $B = ["data-tag"],
+        AC = K.defineComponent({
             __name: "Box",
             props: {
                 model: null
             },
             setup(A) {
                 const B = A;
-                return (g, o) => (K.openBlock(), K.createElementBlock("div", {
+                K.useCssVars(o => ({
+                    ad671c62: K.unref(g)
+                }));
+                const g = B.model.align ?? "flex-start";
+                return (o, t) => (K.openBlock(), K.createElementBlock("div", {
                     class: K.normalizeClass(["pybi-box pybi-container", B.model.classes]),
-                    "data-tag": A.model.tag
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(B.model.children, t => (K.openBlock(), K.createBlock(jg, null, {
-                    default: K.withCtx(() => [K.createVNode(GI, {
-                        component: t
+                    "data-tag": A.model.tag,
+                    "data-pybi-auto-width": ""
+                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(B.model.children, E => (K.openBlock(), K.createBlock(jg, null, {
+                    default: K.withCtx(() => [K.createVNode(JI, {
+                        component: E
                     }, null, 8, ["component"])]),
                     _: 2
-                }, 1024))), 256))], 10, _B))
+                }, 1024))), 256))], 10, $B))
             }
         }),
-        bw = "",
-        AC = WA($B, [
-            ["__scopeId", "data-v-05391fd7"]
+        Zw = "",
+        IC = WA(AC, [
+            ["__scopeId", "data-v-c97c4d56"]
         ]),
-        IC = K.defineComponent({
+        gC = K.defineComponent({
             __name: "FlowBox",
             props: {
                 model: null
             },
             setup(A) {
                 const B = A;
-                return (g, o) => (K.openBlock(), K.createElementBlock("div", {
-                    class: K.normalizeClass(["flow-box", B.model.classes]),
-                    style: K.normalizeStyle(B.model.styles)
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(B.model.children, t => (K.openBlock(), K.createBlock(GI, {
-                    component: t
+                K.useCssVars(o => ({
+                    "34e782bf": K.unref(g)
+                }));
+                const g = B.model.align ?? "flex-start";
+                return (o, t) => (K.openBlock(), K.createElementBlock("div", {
+                    class: K.normalizeClass(["pybi-flow-box pybi-container", B.model.classes]),
+                    style: K.normalizeStyle(B.model.styles),
+                    "data-pybi-auto-width": ""
+                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(B.model.children, E => (K.openBlock(), K.createBlock(JI, {
+                    component: E
                 }, null, 8, ["component"]))), 256))], 6))
             }
         }),
-        Vw = "",
-        gC = WA(IC, [
-            ["__scopeId", "data-v-1462d739"]
+        Tw = "",
+        QC = WA(gC, [
+            ["__scopeId", "data-v-666489c8"]
         ]),
-        QC = K.defineComponent({
+        BC = K.defineComponent({
             __name: "GridBox",
             props: {
                 model: null
             },
             setup(A) {
                 const B = A;
                 K.useCssVars(s => ({
-                    "657644d0": K.unref(o),
-                    "3d257395": K.unref(t),
-                    "376ffdbe": K.unref(E)
+                    b7b51ffe: K.unref(o),
+                    "7bc4d6be": K.unref(t),
+                    cf4ad2d0: K.unref(E)
                 }));
                 const g = B.model.children,
                     o = B.model.areas,
                     t = B.model.gridTemplateColumns,
                     E = B.model.gridTemplateRows;
-                return (s, D) => (K.openBlock(), K.createElementBlock("div", {
-                    class: K.normalizeClass(["grid-box pybi-container", B.model.classes])
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(g), h => (K.openBlock(), K.createBlock(GI, {
+                return (s, i) => (K.openBlock(), K.createElementBlock("div", {
+                    class: K.normalizeClass(["grid-box pybi-container", B.model.classes]),
+                    "data-pybi-auto-width": ""
+                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(g), h => (K.openBlock(), K.createBlock(JI, {
                     component: h
                 }, null, 8, ["component"]))), 256))], 2))
             }
         }),
-        mw = "",
-        BC = WA(QC, [
-            ["__scopeId", "data-v-1c77f43e"]
-        ]),
-        CC = ["data-tag"],
-        EC = K.defineComponent({
-            __name: "ColBox",
-            props: {
-                model: null
-            },
-            setup(A) {
-                const B = A;
-                K.useCssVars(t => ({
-                    "52fb65ca": K.unref(o)
-                }));
-                const g = B.model.children,
-                    o = B.model.spec.map(t => `${t}fr`).join(" ");
-                return (t, E) => (K.openBlock(), K.createElementBlock("div", {
-                    class: K.normalizeClass(["col-box", B.model.classes]),
-                    "data-tag": A.model.tag
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(g), s => (K.openBlock(), K.createBlock(GI, {
-                    component: s
-                }, null, 8, ["component"]))), 256))], 10, CC))
-            }
-        }),
-        Zw = "",
-        iC = WA(EC, [
-            ["__scopeId", "data-v-11490321"]
+        Ww = "",
+        CC = WA(BC, [
+            ["__scopeId", "data-v-2aaf8f29"]
         ]);
-    var DC = typeof global == "object" && global && global.Object === Object && global;
-    const Pg = DC;
-    var oC = typeof self == "object" && self && self.Object === Object && self,
-        sC = Pg || oC || Function("return this")();
-    const zA = sC;
-    var wC = zA.Symbol;
-    const gI = wC;
+    var EC = typeof global == "object" && global && global.Object === Object && global;
+    const Pg = EC;
+    var iC = typeof self == "object" && self && self.Object === Object && self,
+        DC = Pg || iC || Function("return this")();
+    const zA = DC;
+    var oC = zA.Symbol;
+    const gI = oC;
     var zg = Object.prototype,
-        tC = zg.hasOwnProperty,
-        hC = zg.toString,
-        cI = gI ? gI.toStringTag : void 0;
-
-    function FC(A) {
-        var B = tC.call(A, cI),
-            g = A[cI];
+        sC = zg.hasOwnProperty,
+        wC = zg.toString,
+        eI = gI ? gI.toStringTag : void 0;
+
+    function tC(A) {
+        var B = sC.call(A, eI),
+            g = A[eI];
         try {
-            A[cI] = void 0;
+            A[eI] = void 0;
             var o = !0
         } catch {}
-        var t = hC.call(A);
-        return o && (B ? A[cI] = g : delete A[cI]), t
+        var t = wC.call(A);
+        return o && (B ? A[eI] = g : delete A[eI]), t
     }
-    var aC = Object.prototype,
-        RC = aC.toString;
+    var hC = Object.prototype,
+        FC = hC.toString;
 
-    function yC(A) {
-        return RC.call(A)
+    function aC(A) {
+        return FC.call(A)
     }
-    var GC = "[object Null]",
-        UC = "[object Undefined]",
+    var RC = "[object Null]",
+        yC = "[object Undefined]",
         _g = gI ? gI.toStringTag : void 0;
 
     function aI(A) {
-        return A == null ? A === void 0 ? UC : GC : _g && _g in Object(A) ? FC(A) : yC(A)
+        return A == null ? A === void 0 ? yC : RC : _g && _g in Object(A) ? tC(A) : aC(A)
     }
 
     function RI(A) {
         return A != null && typeof A == "object"
     }
-    var nC = "[object Symbol]";
+    var GC = "[object Symbol]";
 
-    function Eg(A) {
-        return typeof A == "symbol" || RI(A) && aI(A) == nC
+    function ig(A) {
+        return typeof A == "symbol" || RI(A) && aI(A) == GC
     }
 
-    function eC(A, B) {
+    function UC(A, B) {
         for (var g = -1, o = A == null ? 0 : A.length, t = Array(o); ++g < o;) t[g] = B(A[g], g, A);
         return t
     }
-    var cC = Array.isArray;
-    const OA = cC;
-    var NC = 1 / 0,
+    var nC = Array.isArray;
+    const OA = nC;
+    var eC = 1 / 0,
         $g = gI ? gI.prototype : void 0,
         AQ = $g ? $g.toString : void 0;
 
     function IQ(A) {
         if (typeof A == "string") return A;
-        if (OA(A)) return eC(A, IQ) + "";
-        if (Eg(A)) return AQ ? AQ.call(A) : "";
+        if (OA(A)) return UC(A, IQ) + "";
+        if (ig(A)) return AQ ? AQ.call(A) : "";
         var B = A + "";
-        return B == "0" && 1 / A == -NC ? "-0" : B
+        return B == "0" && 1 / A == -eC ? "-0" : B
     }
 
-    function ig(A) {
+    function Dg(A) {
         var B = typeof A;
         return A != null && (B == "object" || B == "function")
     }
 
-    function rC(A) {
+    function cC(A) {
         return A
     }
-    var MC = "[object AsyncFunction]",
-        LC = "[object Function]",
-        kC = "[object GeneratorFunction]",
-        SC = "[object Proxy]";
+    var NC = "[object AsyncFunction]",
+        rC = "[object Function]",
+        MC = "[object GeneratorFunction]",
+        LC = "[object Proxy]";
 
     function gQ(A) {
-        if (!ig(A)) return !1;
+        if (!Dg(A)) return !1;
         var B = aI(A);
-        return B == LC || B == kC || B == MC || B == SC
+        return B == rC || B == MC || B == NC || B == LC
     }
-    var JC = zA["__core-js_shared__"];
-    const Dg = JC;
+    var kC = zA["__core-js_shared__"];
+    const og = kC;
     var QQ = function() {
-        var A = /[^.]+$/.exec(Dg && Dg.keys && Dg.keys.IE_PROTO || "");
+        var A = /[^.]+$/.exec(og && og.keys && og.keys.IE_PROTO || "");
         return A ? "Symbol(src)_1." + A : ""
     }();
 
-    function KC(A) {
+    function SC(A) {
         return !!QQ && QQ in A
     }
-    var YC = Function.prototype,
-        HC = YC.toString;
+    var JC = Function.prototype,
+        KC = JC.toString;
 
     function iI(A) {
         if (A != null) {
             try {
-                return HC.call(A)
+                return KC.call(A)
             } catch {}
             try {
                 return A + ""
             } catch {}
         }
         return ""
     }
-    var lC = /[\\^$.*+?()[\]{}|]/g,
-        fC = /^\[object .+?Constructor\]$/,
-        dC = Function.prototype,
-        uC = Object.prototype,
-        pC = dC.toString,
-        qC = uC.hasOwnProperty,
-        xC = RegExp("^" + pC.call(qC).replace(lC, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
-
-    function bC(A) {
-        if (!ig(A) || KC(A)) return !1;
-        var B = gQ(A) ? xC : fC;
+    var YC = /[\\^$.*+?()[\]{}|]/g,
+        HC = /^\[object .+?Constructor\]$/,
+        lC = Function.prototype,
+        fC = Object.prototype,
+        dC = lC.toString,
+        uC = fC.hasOwnProperty,
+        pC = RegExp("^" + dC.call(uC).replace(YC, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
+
+    function qC(A) {
+        if (!Dg(A) || SC(A)) return !1;
+        var B = gQ(A) ? pC : HC;
         return B.test(iI(A))
     }
 
-    function VC(A, B) {
+    function xC(A, B) {
         return A == null ? void 0 : A[B]
     }
 
     function DI(A, B) {
-        var g = VC(A, B);
-        return bC(g) ? g : void 0
+        var g = xC(A, B);
+        return qC(g) ? g : void 0
     }
-    var mC = DI(zA, "WeakMap");
-    const og = mC;
+    var bC = DI(zA, "WeakMap");
+    const sg = bC;
 
-    function ZC() {}
-    var TC = function() {
+    function VC() {}
+    var mC = function() {
         try {
             var A = DI(Object, "defineProperty");
             return A({}, "", {}), A
         } catch {}
     }();
-    const BQ = TC;
+    const BQ = mC;
 
-    function WC(A, B, g, o) {
+    function ZC(A, B, g, o) {
         for (var t = A.length, E = g + (o ? 1 : -1); o ? E-- : ++E < t;)
             if (B(A[E], E, A)) return E;
         return -1
     }
 
-    function OC(A) {
+    function TC(A) {
         return A !== A
     }
 
-    function XC(A, B, g) {
+    function WC(A, B, g) {
         for (var o = g - 1, t = A.length; ++o < t;)
             if (A[o] === B) return o;
         return -1
     }
 
-    function vC(A, B, g) {
-        return B === B ? XC(A, B, g) : WC(A, OC, g)
+    function OC(A, B, g) {
+        return B === B ? WC(A, B, g) : ZC(A, TC, g)
     }
 
-    function jC(A, B) {
+    function XC(A, B) {
         var g = A == null ? 0 : A.length;
-        return !!g && vC(A, B, 0) > -1
+        return !!g && OC(A, B, 0) > -1
     }
-    var PC = 9007199254740991,
-        zC = /^(?:0|[1-9]\d*)$/;
+    var vC = 9007199254740991,
+        jC = /^(?:0|[1-9]\d*)$/;
 
     function CQ(A, B) {
         var g = typeof A;
-        return B = B ?? PC, !!B && (g == "number" || g != "symbol" && zC.test(A)) && A > -1 && A % 1 == 0 && A < B
+        return B = B ?? vC, !!B && (g == "number" || g != "symbol" && jC.test(A)) && A > -1 && A % 1 == 0 && A < B
     }
 
-    function _C(A, B, g) {
+    function PC(A, B, g) {
         B == "__proto__" && BQ ? BQ(A, B, {
             configurable: !0,
             enumerable: !0,
             value: g,
             writable: !0
         }) : A[B] = g
     }
 
     function EQ(A, B) {
         return A === B || A !== A && B !== B
     }
-    var $C = 9007199254740991;
+    var zC = 9007199254740991;
 
-    function sg(A) {
-        return typeof A == "number" && A > -1 && A % 1 == 0 && A <= $C
+    function wg(A) {
+        return typeof A == "number" && A > -1 && A % 1 == 0 && A <= zC
     }
 
     function iQ(A) {
-        return A != null && sg(A.length) && !gQ(A)
+        return A != null && wg(A.length) && !gQ(A)
     }
-    var AE = Object.prototype;
+    var _C = Object.prototype;
 
-    function IE(A) {
+    function $C(A) {
         var B = A && A.constructor,
-            g = typeof B == "function" && B.prototype || AE;
+            g = typeof B == "function" && B.prototype || _C;
         return A === g
     }
 
-    function gE(A, B) {
+    function AE(A, B) {
         for (var g = -1, o = Array(A); ++g < A;) o[g] = B(g);
         return o
     }
-    var QE = "[object Arguments]";
+    var IE = "[object Arguments]";
 
     function DQ(A) {
-        return RI(A) && aI(A) == QE
+        return RI(A) && aI(A) == IE
     }
     var oQ = Object.prototype,
-        BE = oQ.hasOwnProperty,
-        CE = oQ.propertyIsEnumerable,
-        EE = DQ(function() {
+        gE = oQ.hasOwnProperty,
+        QE = oQ.propertyIsEnumerable,
+        BE = DQ(function() {
             return arguments
         }()) ? DQ : function(A) {
-            return RI(A) && BE.call(A, "callee") && !CE.call(A, "callee")
+            return RI(A) && gE.call(A, "callee") && !QE.call(A, "callee")
         };
-    const sQ = EE;
+    const sQ = BE;
 
-    function iE() {
+    function CE() {
         return !1
     }
     var wQ = typeof exports == "object" && exports && !exports.nodeType && exports,
         tQ = wQ && typeof module == "object" && module && !module.nodeType && module,
-        DE = tQ && tQ.exports === wQ,
-        hQ = DE ? zA.Buffer : void 0,
-        oE = hQ ? hQ.isBuffer : void 0,
-        sE = oE || iE;
-    const wg = sE;
-    var wE = "[object Arguments]",
-        tE = "[object Array]",
-        hE = "[object Boolean]",
-        FE = "[object Date]",
-        aE = "[object Error]",
-        RE = "[object Function]",
-        yE = "[object Map]",
-        GE = "[object Number]",
-        UE = "[object Object]",
-        nE = "[object RegExp]",
-        eE = "[object Set]",
-        cE = "[object String]",
-        NE = "[object WeakMap]",
-        rE = "[object ArrayBuffer]",
-        ME = "[object DataView]",
-        LE = "[object Float32Array]",
-        kE = "[object Float64Array]",
-        SE = "[object Int8Array]",
-        JE = "[object Int16Array]",
-        KE = "[object Int32Array]",
-        YE = "[object Uint8Array]",
-        HE = "[object Uint8ClampedArray]",
-        lE = "[object Uint16Array]",
-        fE = "[object Uint32Array]",
+        EE = tQ && tQ.exports === wQ,
+        hQ = EE ? zA.Buffer : void 0,
+        iE = hQ ? hQ.isBuffer : void 0,
+        DE = iE || CE;
+    const tg = DE;
+    var oE = "[object Arguments]",
+        sE = "[object Array]",
+        wE = "[object Boolean]",
+        tE = "[object Date]",
+        hE = "[object Error]",
+        FE = "[object Function]",
+        aE = "[object Map]",
+        RE = "[object Number]",
+        yE = "[object Object]",
+        GE = "[object RegExp]",
+        UE = "[object Set]",
+        nE = "[object String]",
+        eE = "[object WeakMap]",
+        cE = "[object ArrayBuffer]",
+        NE = "[object DataView]",
+        rE = "[object Float32Array]",
+        ME = "[object Float64Array]",
+        LE = "[object Int8Array]",
+        kE = "[object Int16Array]",
+        SE = "[object Int32Array]",
+        JE = "[object Uint8Array]",
+        KE = "[object Uint8ClampedArray]",
+        YE = "[object Uint16Array]",
+        HE = "[object Uint32Array]",
         LA = {};
-    LA[LE] = LA[kE] = LA[SE] = LA[JE] = LA[KE] = LA[YE] = LA[HE] = LA[lE] = LA[fE] = !0, LA[wE] = LA[tE] = LA[rE] = LA[hE] = LA[ME] = LA[FE] = LA[aE] = LA[RE] = LA[yE] = LA[GE] = LA[UE] = LA[nE] = LA[eE] = LA[cE] = LA[NE] = !1;
+    LA[rE] = LA[ME] = LA[LE] = LA[kE] = LA[SE] = LA[JE] = LA[KE] = LA[YE] = LA[HE] = !0, LA[oE] = LA[sE] = LA[cE] = LA[wE] = LA[NE] = LA[tE] = LA[hE] = LA[FE] = LA[aE] = LA[RE] = LA[yE] = LA[GE] = LA[UE] = LA[nE] = LA[eE] = !1;
 
-    function dE(A) {
-        return RI(A) && sg(A.length) && !!LA[aI(A)]
+    function lE(A) {
+        return RI(A) && wg(A.length) && !!LA[aI(A)]
     }
 
-    function uE(A) {
+    function fE(A) {
         return function(B) {
             return A(B)
         }
     }
     var FQ = typeof exports == "object" && exports && !exports.nodeType && exports,
-        NI = FQ && typeof module == "object" && module && !module.nodeType && module,
-        pE = NI && NI.exports === FQ,
-        tg = pE && Pg.process,
-        qE = function() {
+        cI = FQ && typeof module == "object" && module && !module.nodeType && module,
+        dE = cI && cI.exports === FQ,
+        hg = dE && Pg.process,
+        uE = function() {
             try {
-                var A = NI && NI.require && NI.require("util").types;
-                return A || tg && tg.binding && tg.binding("util")
+                var A = cI && cI.require && cI.require("util").types;
+                return A || hg && hg.binding && hg.binding("util")
             } catch {}
         }();
-    const aQ = qE;
+    const aQ = uE;
     var RQ = aQ && aQ.isTypedArray,
-        xE = RQ ? uE(RQ) : dE;
-    const yQ = xE;
-    var bE = Object.prototype,
-        VE = bE.hasOwnProperty;
+        pE = RQ ? fE(RQ) : lE;
+    const yQ = pE;
+    var qE = Object.prototype,
+        xE = qE.hasOwnProperty;
 
-    function mE(A, B) {
+    function bE(A, B) {
         var g = OA(A),
             o = !g && sQ(A),
-            t = !g && !o && wg(A),
+            t = !g && !o && tg(A),
             E = !g && !o && !t && yQ(A),
             s = g || o || t || E,
-            D = s ? gE(A.length, String) : [],
-            h = D.length;
-        for (var C in A)(B || VE.call(A, C)) && !(s && (C == "length" || t && (C == "offset" || C == "parent") || E && (C == "buffer" || C == "byteLength" || C == "byteOffset") || CQ(C, h))) && D.push(C);
-        return D
+            i = s ? AE(A.length, String) : [],
+            h = i.length;
+        for (var C in A)(B || xE.call(A, C)) && !(s && (C == "length" || t && (C == "offset" || C == "parent") || E && (C == "buffer" || C == "byteLength" || C == "byteOffset") || CQ(C, h))) && i.push(C);
+        return i
     }
 
-    function ZE(A, B) {
+    function VE(A, B) {
         return function(g) {
             return A(B(g))
         }
     }
-    var TE = ZE(Object.keys, Object);
-    const WE = TE;
-    var OE = Object.prototype,
-        XE = OE.hasOwnProperty;
+    var mE = VE(Object.keys, Object);
+    const ZE = mE;
+    var TE = Object.prototype,
+        WE = TE.hasOwnProperty;
 
-    function vE(A) {
-        if (!IE(A)) return WE(A);
+    function OE(A) {
+        if (!$C(A)) return ZE(A);
         var B = [];
-        for (var g in Object(A)) XE.call(A, g) && g != "constructor" && B.push(g);
+        for (var g in Object(A)) WE.call(A, g) && g != "constructor" && B.push(g);
         return B
     }
 
-    function hg(A) {
-        return iQ(A) ? mE(A) : vE(A)
+    function Fg(A) {
+        return iQ(A) ? bE(A) : OE(A)
     }
-    var jE = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        PE = /^\w*$/;
+    var XE = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+        vE = /^\w*$/;
 
-    function Fg(A, B) {
+    function ag(A, B) {
         if (OA(A)) return !1;
         var g = typeof A;
-        return g == "number" || g == "symbol" || g == "boolean" || A == null || Eg(A) ? !0 : PE.test(A) || !jE.test(A) || B != null && A in Object(B)
+        return g == "number" || g == "symbol" || g == "boolean" || A == null || ig(A) ? !0 : vE.test(A) || !XE.test(A) || B != null && A in Object(B)
     }
-    var zE = DI(Object, "create");
-    const rI = zE;
+    var jE = DI(Object, "create");
+    const NI = jE;
 
-    function _E() {
-        this.__data__ = rI ? rI(null) : {}, this.size = 0
+    function PE() {
+        this.__data__ = NI ? NI(null) : {}, this.size = 0
     }
 
-    function $E(A) {
+    function zE(A) {
         var B = this.has(A) && delete this.__data__[A];
         return this.size -= B ? 1 : 0, B
     }
-    var Ai = "__lodash_hash_undefined__",
-        Ii = Object.prototype,
-        gi = Ii.hasOwnProperty;
+    var _E = "__lodash_hash_undefined__",
+        $E = Object.prototype,
+        Ai = $E.hasOwnProperty;
 
-    function Qi(A) {
+    function Ii(A) {
         var B = this.__data__;
-        if (rI) {
+        if (NI) {
             var g = B[A];
-            return g === Ai ? void 0 : g
+            return g === _E ? void 0 : g
         }
-        return gi.call(B, A) ? B[A] : void 0
+        return Ai.call(B, A) ? B[A] : void 0
     }
-    var Bi = Object.prototype,
-        Ci = Bi.hasOwnProperty;
+    var gi = Object.prototype,
+        Qi = gi.hasOwnProperty;
 
-    function Ei(A) {
+    function Bi(A) {
         var B = this.__data__;
-        return rI ? B[A] !== void 0 : Ci.call(B, A)
+        return NI ? B[A] !== void 0 : Qi.call(B, A)
     }
-    var ii = "__lodash_hash_undefined__";
+    var Ci = "__lodash_hash_undefined__";
 
-    function Di(A, B) {
+    function Ei(A, B) {
         var g = this.__data__;
-        return this.size += this.has(A) ? 0 : 1, g[A] = rI && B === void 0 ? ii : B, this
+        return this.size += this.has(A) ? 0 : 1, g[A] = NI && B === void 0 ? Ci : B, this
     }
 
     function oI(A) {
         var B = -1,
             g = A == null ? 0 : A.length;
         for (this.clear(); ++B < g;) {
             var o = A[B];
             this.set(o[0], o[1])
         }
     }
-    oI.prototype.clear = _E, oI.prototype.delete = $E, oI.prototype.get = Qi, oI.prototype.has = Ei, oI.prototype.set = Di;
+    oI.prototype.clear = PE, oI.prototype.delete = zE, oI.prototype.get = Ii, oI.prototype.has = Bi, oI.prototype.set = Ei;
 
-    function oi() {
+    function ii() {
         this.__data__ = [], this.size = 0
     }
 
-    function bI(A, B) {
+    function VI(A, B) {
         for (var g = A.length; g--;)
             if (EQ(A[g][0], B)) return g;
         return -1
     }
-    var si = Array.prototype,
-        wi = si.splice;
+    var Di = Array.prototype,
+        oi = Di.splice;
 
-    function ti(A) {
+    function si(A) {
         var B = this.__data__,
-            g = bI(B, A);
+            g = VI(B, A);
         if (g < 0) return !1;
         var o = B.length - 1;
-        return g == o ? B.pop() : wi.call(B, g, 1), --this.size, !0
+        return g == o ? B.pop() : oi.call(B, g, 1), --this.size, !0
     }
 
-    function hi(A) {
+    function wi(A) {
         var B = this.__data__,
-            g = bI(B, A);
+            g = VI(B, A);
         return g < 0 ? void 0 : B[g][1]
     }
 
-    function Fi(A) {
-        return bI(this.__data__, A) > -1
+    function ti(A) {
+        return VI(this.__data__, A) > -1
     }
 
-    function ai(A, B) {
+    function hi(A, B) {
         var g = this.__data__,
-            o = bI(g, A);
+            o = VI(g, A);
         return o < 0 ? (++this.size, g.push([A, B])) : g[o][1] = B, this
     }
 
     function _A(A) {
         var B = -1,
             g = A == null ? 0 : A.length;
         for (this.clear(); ++B < g;) {
             var o = A[B];
             this.set(o[0], o[1])
         }
     }
-    _A.prototype.clear = oi, _A.prototype.delete = ti, _A.prototype.get = hi, _A.prototype.has = Fi, _A.prototype.set = ai;
-    var Ri = DI(zA, "Map");
-    const MI = Ri;
+    _A.prototype.clear = ii, _A.prototype.delete = si, _A.prototype.get = wi, _A.prototype.has = ti, _A.prototype.set = hi;
+    var Fi = DI(zA, "Map");
+    const rI = Fi;
 
-    function yi() {
+    function ai() {
         this.size = 0, this.__data__ = {
             hash: new oI,
-            map: new(MI || _A),
+            map: new(rI || _A),
             string: new oI
         }
     }
 
-    function Gi(A) {
+    function Ri(A) {
         var B = typeof A;
         return B == "string" || B == "number" || B == "symbol" || B == "boolean" ? A !== "__proto__" : A === null
     }
 
-    function VI(A, B) {
+    function mI(A, B) {
         var g = A.__data__;
-        return Gi(B) ? g[typeof B == "string" ? "string" : "hash"] : g.map
+        return Ri(B) ? g[typeof B == "string" ? "string" : "hash"] : g.map
     }
 
-    function Ui(A) {
-        var B = VI(this, A).delete(A);
+    function yi(A) {
+        var B = mI(this, A).delete(A);
         return this.size -= B ? 1 : 0, B
     }
 
-    function ni(A) {
-        return VI(this, A).get(A)
+    function Gi(A) {
+        return mI(this, A).get(A)
     }
 
-    function ei(A) {
-        return VI(this, A).has(A)
+    function Ui(A) {
+        return mI(this, A).has(A)
     }
 
-    function ci(A, B) {
-        var g = VI(this, A),
+    function ni(A, B) {
+        var g = mI(this, A),
             o = g.size;
         return g.set(A, B), this.size += g.size == o ? 0 : 1, this
     }
 
     function $A(A) {
         var B = -1,
             g = A == null ? 0 : A.length;
         for (this.clear(); ++B < g;) {
             var o = A[B];
             this.set(o[0], o[1])
         }
     }
-    $A.prototype.clear = yi, $A.prototype.delete = Ui, $A.prototype.get = ni, $A.prototype.has = ei, $A.prototype.set = ci;
-    var Ni = "Expected a function";
+    $A.prototype.clear = ai, $A.prototype.delete = yi, $A.prototype.get = Gi, $A.prototype.has = Ui, $A.prototype.set = ni;
+    var ei = "Expected a function";
 
-    function ag(A, B) {
-        if (typeof A != "function" || B != null && typeof B != "function") throw new TypeError(Ni);
+    function Rg(A, B) {
+        if (typeof A != "function" || B != null && typeof B != "function") throw new TypeError(ei);
         var g = function() {
             var o = arguments,
                 t = B ? B.apply(this, o) : o[0],
                 E = g.cache;
             if (E.has(t)) return E.get(t);
             var s = A.apply(this, o);
             return g.cache = E.set(t, s) || E, s
         };
-        return g.cache = new(ag.Cache || $A), g
+        return g.cache = new(Rg.Cache || $A), g
     }
-    ag.Cache = $A;
-    var ri = 500;
+    Rg.Cache = $A;
+    var ci = 500;
 
-    function Mi(A) {
-        var B = ag(A, function(o) {
-                return g.size === ri && g.clear(), o
+    function Ni(A) {
+        var B = Rg(A, function(o) {
+                return g.size === ci && g.clear(), o
             }),
             g = B.cache;
         return B
     }
-    var Li = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        ki = /\\(\\)?/g,
-        Si = Mi(function(A) {
+    var ri = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
+        Mi = /\\(\\)?/g,
+        Li = Ni(function(A) {
             var B = [];
-            return A.charCodeAt(0) === 46 && B.push(""), A.replace(Li, function(g, o, t, E) {
-                B.push(t ? E.replace(ki, "$1") : o || g)
+            return A.charCodeAt(0) === 46 && B.push(""), A.replace(ri, function(g, o, t, E) {
+                B.push(t ? E.replace(Mi, "$1") : o || g)
             }), B
         });
-    const Ji = Si;
+    const ki = Li;
 
-    function Ki(A) {
+    function Si(A) {
         return A == null ? "" : IQ(A)
     }
 
     function GQ(A, B) {
-        return OA(A) ? A : Fg(A, B) ? [A] : Ji(Ki(A))
+        return OA(A) ? A : ag(A, B) ? [A] : ki(Si(A))
     }
-    var Yi = 1 / 0;
+    var Ji = 1 / 0;
 
-    function mI(A) {
-        if (typeof A == "string" || Eg(A)) return A;
+    function ZI(A) {
+        if (typeof A == "string" || ig(A)) return A;
         var B = A + "";
-        return B == "0" && 1 / A == -Yi ? "-0" : B
+        return B == "0" && 1 / A == -Ji ? "-0" : B
     }
 
     function UQ(A, B) {
         B = GQ(B, A);
-        for (var g = 0, o = B.length; A != null && g < o;) A = A[mI(B[g++])];
+        for (var g = 0, o = B.length; A != null && g < o;) A = A[ZI(B[g++])];
         return g && g == o ? A : void 0
     }
 
-    function Hi(A, B, g) {
+    function Ki(A, B, g) {
         var o = A == null ? void 0 : UQ(A, B);
         return o === void 0 ? g : o
     }
 
-    function li(A, B) {
+    function Yi(A, B) {
         for (var g = -1, o = B.length, t = A.length; ++g < o;) A[t + g] = B[g];
         return A
     }
 
-    function fi() {
+    function Hi() {
         this.__data__ = new _A, this.size = 0
     }
 
-    function di(A) {
+    function li(A) {
         var B = this.__data__,
             g = B.delete(A);
         return this.size = B.size, g
     }
 
-    function ui(A) {
+    function fi(A) {
         return this.__data__.get(A)
     }
 
-    function pi(A) {
+    function di(A) {
         return this.__data__.has(A)
     }
-    var qi = 200;
+    var ui = 200;
 
-    function xi(A, B) {
+    function pi(A, B) {
         var g = this.__data__;
         if (g instanceof _A) {
             var o = g.__data__;
-            if (!MI || o.length < qi - 1) return o.push([A, B]), this.size = ++g.size, this;
+            if (!rI || o.length < ui - 1) return o.push([A, B]), this.size = ++g.size, this;
             g = this.__data__ = new $A(o)
         }
         return g.set(A, B), this.size = g.size, this
     }
 
     function AI(A) {
         var B = this.__data__ = new _A(A);
         this.size = B.size
     }
-    AI.prototype.clear = fi, AI.prototype.delete = di, AI.prototype.get = ui, AI.prototype.has = pi, AI.prototype.set = xi;
+    AI.prototype.clear = Hi, AI.prototype.delete = li, AI.prototype.get = fi, AI.prototype.has = di, AI.prototype.set = pi;
 
-    function bi(A, B) {
+    function qi(A, B) {
         for (var g = -1, o = A == null ? 0 : A.length, t = 0, E = []; ++g < o;) {
             var s = A[g];
             B(s, g, A) && (E[t++] = s)
         }
         return E
     }
 
-    function Vi() {
+    function xi() {
         return []
     }
-    var mi = Object.prototype,
-        Zi = mi.propertyIsEnumerable,
+    var bi = Object.prototype,
+        Vi = bi.propertyIsEnumerable,
         nQ = Object.getOwnPropertySymbols,
-        Ti = nQ ? function(A) {
-            return A == null ? [] : (A = Object(A), bi(nQ(A), function(B) {
-                return Zi.call(A, B)
+        mi = nQ ? function(A) {
+            return A == null ? [] : (A = Object(A), qi(nQ(A), function(B) {
+                return Vi.call(A, B)
             }))
-        } : Vi;
-    const Wi = Ti;
+        } : xi;
+    const Zi = mi;
 
-    function Oi(A, B, g) {
+    function Ti(A, B, g) {
         var o = B(A);
-        return OA(A) ? o : li(o, g(A))
+        return OA(A) ? o : Yi(o, g(A))
     }
 
     function eQ(A) {
-        return Oi(A, hg, Wi)
+        return Ti(A, Fg, Zi)
     }
-    var Xi = DI(zA, "DataView");
-    const Rg = Xi;
-    var vi = DI(zA, "Promise");
-    const yg = vi;
-    var ji = DI(zA, "Set");
-    const yI = ji;
+    var Wi = DI(zA, "DataView");
+    const yg = Wi;
+    var Oi = DI(zA, "Promise");
+    const Gg = Oi;
+    var Xi = DI(zA, "Set");
+    const yI = Xi;
     var cQ = "[object Map]",
-        Pi = "[object Object]",
+        vi = "[object Object]",
         NQ = "[object Promise]",
         rQ = "[object Set]",
         MQ = "[object WeakMap]",
         LQ = "[object DataView]",
-        zi = iI(Rg),
-        _i = iI(MI),
-        $i = iI(yg),
-        AD = iI(yI),
-        ID = iI(og),
+        ji = iI(yg),
+        Pi = iI(rI),
+        zi = iI(Gg),
+        _i = iI(yI),
+        $i = iI(sg),
         sI = aI;
-    (Rg && sI(new Rg(new ArrayBuffer(1))) != LQ || MI && sI(new MI) != cQ || yg && sI(yg.resolve()) != NQ || yI && sI(new yI) != rQ || og && sI(new og) != MQ) && (sI = function(A) {
+    (yg && sI(new yg(new ArrayBuffer(1))) != LQ || rI && sI(new rI) != cQ || Gg && sI(Gg.resolve()) != NQ || yI && sI(new yI) != rQ || sg && sI(new sg) != MQ) && (sI = function(A) {
         var B = aI(A),
-            g = B == Pi ? A.constructor : void 0,
+            g = B == vi ? A.constructor : void 0,
             o = g ? iI(g) : "";
         if (o) switch (o) {
-            case zi:
+            case ji:
                 return LQ;
-            case _i:
+            case Pi:
                 return cQ;
-            case $i:
+            case zi:
                 return NQ;
-            case AD:
+            case _i:
                 return rQ;
-            case ID:
+            case $i:
                 return MQ
         }
         return B
     });
     const kQ = sI;
-    var gD = zA.Uint8Array;
-    const SQ = gD;
-    var QD = "__lodash_hash_undefined__";
+    var AD = zA.Uint8Array;
+    const SQ = AD;
+    var ID = "__lodash_hash_undefined__";
 
-    function BD(A) {
-        return this.__data__.set(A, QD), this
+    function gD(A) {
+        return this.__data__.set(A, ID), this
     }
 
-    function CD(A) {
+    function QD(A) {
         return this.__data__.has(A)
     }
 
-    function LI(A) {
+    function MI(A) {
         var B = -1,
             g = A == null ? 0 : A.length;
         for (this.__data__ = new $A; ++B < g;) this.add(A[B])
     }
-    LI.prototype.add = LI.prototype.push = BD, LI.prototype.has = CD;
+    MI.prototype.add = MI.prototype.push = gD, MI.prototype.has = QD;
 
-    function ED(A, B) {
+    function BD(A, B) {
         for (var g = -1, o = A == null ? 0 : A.length; ++g < o;)
             if (B(A[g], g, A)) return !0;
         return !1
     }
 
     function JQ(A, B) {
         return A.has(B)
     }
-    var iD = 1,
-        DD = 2;
+    var CD = 1,
+        ED = 2;
 
     function KQ(A, B, g, o, t, E) {
-        var s = g & iD,
-            D = A.length,
+        var s = g & CD,
+            i = A.length,
             h = B.length;
-        if (D != h && !(s && h > D)) return !1;
+        if (i != h && !(s && h > i)) return !1;
         var C = E.get(A),
             r = E.get(B);
         if (C && r) return C == B && r == A;
         var n = -1,
             M = !0,
-            R = g & DD ? new LI : void 0;
-        for (E.set(A, B), E.set(B, A); ++n < D;) {
+            R = g & ED ? new MI : void 0;
+        for (E.set(A, B), E.set(B, A); ++n < i;) {
             var N = A[n],
                 a = B[n];
             if (o) var G = s ? o(a, N, n, B, A, E) : o(N, a, n, A, B, E);
             if (G !== void 0) {
                 if (G) continue;
                 M = !1;
                 break
             }
             if (R) {
-                if (!ED(B, function(y, c) {
+                if (!BD(B, function(y, c) {
                         if (!JQ(R, c) && (N === y || t(N, y, g, o, E))) return R.push(c)
                     })) {
                     M = !1;
                     break
                 }
             } else if (!(N === a || t(N, a, g, o, E))) {
                 M = !1;
                 break
             }
         }
         return E.delete(A), E.delete(B), M
     }
 
-    function oD(A) {
+    function iD(A) {
         var B = -1,
             g = Array(A.size);
         return A.forEach(function(o, t) {
             g[++B] = [t, o]
         }), g
     }
 
-    function Gg(A) {
+    function Ug(A) {
         var B = -1,
             g = Array(A.size);
         return A.forEach(function(o) {
             g[++B] = o
         }), g
     }
-    var sD = 1,
-        wD = 2,
-        tD = "[object Boolean]",
-        hD = "[object Date]",
-        FD = "[object Error]",
-        aD = "[object Map]",
-        RD = "[object Number]",
-        yD = "[object RegExp]",
-        GD = "[object Set]",
-        UD = "[object String]",
-        nD = "[object Symbol]",
-        eD = "[object ArrayBuffer]",
-        cD = "[object DataView]",
+    var DD = 1,
+        oD = 2,
+        sD = "[object Boolean]",
+        wD = "[object Date]",
+        tD = "[object Error]",
+        hD = "[object Map]",
+        FD = "[object Number]",
+        aD = "[object RegExp]",
+        RD = "[object Set]",
+        yD = "[object String]",
+        GD = "[object Symbol]",
+        UD = "[object ArrayBuffer]",
+        nD = "[object DataView]",
         YQ = gI ? gI.prototype : void 0,
-        Ug = YQ ? YQ.valueOf : void 0;
+        ng = YQ ? YQ.valueOf : void 0;
 
-    function ND(A, B, g, o, t, E, s) {
+    function eD(A, B, g, o, t, E, s) {
         switch (g) {
-            case cD:
+            case nD:
                 if (A.byteLength != B.byteLength || A.byteOffset != B.byteOffset) return !1;
                 A = A.buffer, B = B.buffer;
-            case eD:
+            case UD:
                 return !(A.byteLength != B.byteLength || !E(new SQ(A), new SQ(B)));
-            case tD:
-            case hD:
-            case RD:
-                return EQ(+A, +B);
+            case sD:
+            case wD:
             case FD:
+                return EQ(+A, +B);
+            case tD:
                 return A.name == B.name && A.message == B.message;
+            case aD:
             case yD:
-            case UD:
                 return A == B + "";
-            case aD:
-                var D = oD;
-            case GD:
-                var h = o & sD;
-                if (D || (D = Gg), A.size != B.size && !h) return !1;
+            case hD:
+                var i = iD;
+            case RD:
+                var h = o & DD;
+                if (i || (i = Ug), A.size != B.size && !h) return !1;
                 var C = s.get(A);
                 if (C) return C == B;
-                o |= wD, s.set(A, B);
-                var r = KQ(D(A), D(B), o, t, E, s);
+                o |= oD, s.set(A, B);
+                var r = KQ(i(A), i(B), o, t, E, s);
                 return s.delete(A), r;
-            case nD:
-                if (Ug) return Ug.call(A) == Ug.call(B)
+            case GD:
+                if (ng) return ng.call(A) == ng.call(B)
         }
         return !1
     }
-    var rD = 1,
-        MD = Object.prototype,
-        LD = MD.hasOwnProperty;
-
-    function kD(A, B, g, o, t, E) {
-        var s = g & rD,
-            D = eQ(A),
-            h = D.length,
+    var cD = 1,
+        ND = Object.prototype,
+        rD = ND.hasOwnProperty;
+
+    function MD(A, B, g, o, t, E) {
+        var s = g & cD,
+            i = eQ(A),
+            h = i.length,
             C = eQ(B),
             r = C.length;
         if (h != r && !s) return !1;
         for (var n = h; n--;) {
-            var M = D[n];
-            if (!(s ? M in B : LD.call(B, M))) return !1
+            var M = i[n];
+            if (!(s ? M in B : rD.call(B, M))) return !1
         }
         var R = E.get(A),
             N = E.get(B);
         if (R && N) return R == B && N == A;
         var a = !0;
         E.set(A, B), E.set(B, A);
         for (var G = s; ++n < h;) {
-            M = D[n];
+            M = i[n];
             var y = A[M],
                 c = B[M];
             if (o) var k = s ? o(c, y, M, B, A, E) : o(y, c, M, A, B, E);
             if (!(k === void 0 ? y === c || t(y, c, g, o, E) : k)) {
                 a = !1;
                 break
             }
@@ -925,295 +911,295 @@
         if (a && !G) {
             var H = A.constructor,
                 l = B.constructor;
             H != l && "constructor" in A && "constructor" in B && !(typeof H == "function" && H instanceof H && typeof l == "function" && l instanceof l) && (a = !1)
         }
         return E.delete(A), E.delete(B), a
     }
-    var SD = 1,
+    var LD = 1,
         HQ = "[object Arguments]",
         lQ = "[object Array]",
-        ZI = "[object Object]",
-        JD = Object.prototype,
-        fQ = JD.hasOwnProperty;
+        TI = "[object Object]",
+        kD = Object.prototype,
+        fQ = kD.hasOwnProperty;
 
-    function KD(A, B, g, o, t, E) {
+    function SD(A, B, g, o, t, E) {
         var s = OA(A),
-            D = OA(B),
+            i = OA(B),
             h = s ? lQ : kQ(A),
-            C = D ? lQ : kQ(B);
-        h = h == HQ ? ZI : h, C = C == HQ ? ZI : C;
-        var r = h == ZI,
-            n = C == ZI,
+            C = i ? lQ : kQ(B);
+        h = h == HQ ? TI : h, C = C == HQ ? TI : C;
+        var r = h == TI,
+            n = C == TI,
             M = h == C;
-        if (M && wg(A)) {
-            if (!wg(B)) return !1;
+        if (M && tg(A)) {
+            if (!tg(B)) return !1;
             s = !0, r = !1
         }
-        if (M && !r) return E || (E = new AI), s || yQ(A) ? KQ(A, B, g, o, t, E) : ND(A, B, h, g, o, t, E);
-        if (!(g & SD)) {
+        if (M && !r) return E || (E = new AI), s || yQ(A) ? KQ(A, B, g, o, t, E) : eD(A, B, h, g, o, t, E);
+        if (!(g & LD)) {
             var R = r && fQ.call(A, "__wrapped__"),
                 N = n && fQ.call(B, "__wrapped__");
             if (R || N) {
                 var a = R ? A.value() : A,
                     G = N ? B.value() : B;
                 return E || (E = new AI), t(a, G, g, o, E)
             }
         }
-        return M ? (E || (E = new AI), kD(A, B, g, o, t, E)) : !1
+        return M ? (E || (E = new AI), MD(A, B, g, o, t, E)) : !1
     }
 
-    function ng(A, B, g, o, t) {
-        return A === B ? !0 : A == null || B == null || !RI(A) && !RI(B) ? A !== A && B !== B : KD(A, B, g, o, ng, t)
+    function eg(A, B, g, o, t) {
+        return A === B ? !0 : A == null || B == null || !RI(A) && !RI(B) ? A !== A && B !== B : SD(A, B, g, o, eg, t)
     }
-    var YD = 1,
-        HD = 2;
+    var JD = 1,
+        KD = 2;
 
-    function lD(A, B, g, o) {
+    function YD(A, B, g, o) {
         var t = g.length,
             E = t,
             s = !o;
         if (A == null) return !E;
         for (A = Object(A); t--;) {
-            var D = g[t];
-            if (s && D[2] ? D[1] !== A[D[0]] : !(D[0] in A)) return !1
+            var i = g[t];
+            if (s && i[2] ? i[1] !== A[i[0]] : !(i[0] in A)) return !1
         }
         for (; ++t < E;) {
-            D = g[t];
-            var h = D[0],
+            i = g[t];
+            var h = i[0],
                 C = A[h],
-                r = D[1];
-            if (s && D[2]) {
+                r = i[1];
+            if (s && i[2]) {
                 if (C === void 0 && !(h in A)) return !1
             } else {
                 var n = new AI;
                 if (o) var M = o(C, r, h, A, B, n);
-                if (!(M === void 0 ? ng(r, C, YD | HD, o, n) : M)) return !1
+                if (!(M === void 0 ? eg(r, C, JD | KD, o, n) : M)) return !1
             }
         }
         return !0
     }
 
     function dQ(A) {
-        return A === A && !ig(A)
+        return A === A && !Dg(A)
     }
 
-    function fD(A) {
-        for (var B = hg(A), g = B.length; g--;) {
+    function HD(A) {
+        for (var B = Fg(A), g = B.length; g--;) {
             var o = B[g],
                 t = A[o];
             B[g] = [o, t, dQ(t)]
         }
         return B
     }
 
     function uQ(A, B) {
         return function(g) {
             return g == null ? !1 : g[A] === B && (B !== void 0 || A in Object(g))
         }
     }
 
-    function dD(A) {
-        var B = fD(A);
+    function lD(A) {
+        var B = HD(A);
         return B.length == 1 && B[0][2] ? uQ(B[0][0], B[0][1]) : function(g) {
-            return g === A || lD(g, A, B)
+            return g === A || YD(g, A, B)
         }
     }
 
-    function uD(A, B) {
+    function fD(A, B) {
         return A != null && B in Object(A)
     }
 
-    function pD(A, B, g) {
+    function dD(A, B, g) {
         B = GQ(B, A);
         for (var o = -1, t = B.length, E = !1; ++o < t;) {
-            var s = mI(B[o]);
+            var s = ZI(B[o]);
             if (!(E = A != null && g(A, s))) break;
             A = A[s]
         }
-        return E || ++o != t ? E : (t = A == null ? 0 : A.length, !!t && sg(t) && CQ(s, t) && (OA(A) || sQ(A)))
+        return E || ++o != t ? E : (t = A == null ? 0 : A.length, !!t && wg(t) && CQ(s, t) && (OA(A) || sQ(A)))
     }
 
-    function qD(A, B) {
-        return A != null && pD(A, B, uD)
+    function uD(A, B) {
+        return A != null && dD(A, B, fD)
     }
-    var xD = 1,
-        bD = 2;
+    var pD = 1,
+        qD = 2;
 
-    function VD(A, B) {
-        return Fg(A) && dQ(B) ? uQ(mI(A), B) : function(g) {
-            var o = Hi(g, A);
-            return o === void 0 && o === B ? qD(g, A) : ng(B, o, xD | bD)
+    function xD(A, B) {
+        return ag(A) && dQ(B) ? uQ(ZI(A), B) : function(g) {
+            var o = Ki(g, A);
+            return o === void 0 && o === B ? uD(g, A) : eg(B, o, pD | qD)
         }
     }
 
-    function mD(A) {
+    function bD(A) {
         return function(B) {
             return B == null ? void 0 : B[A]
         }
     }
 
-    function ZD(A) {
+    function VD(A) {
         return function(B) {
             return UQ(B, A)
         }
     }
 
-    function TD(A) {
-        return Fg(A) ? mD(mI(A)) : ZD(A)
+    function mD(A) {
+        return ag(A) ? bD(ZI(A)) : VD(A)
     }
 
-    function WD(A) {
-        return typeof A == "function" ? A : A == null ? rC : typeof A == "object" ? OA(A) ? VD(A[0], A[1]) : dD(A) : TD(A)
+    function ZD(A) {
+        return typeof A == "function" ? A : A == null ? cC : typeof A == "object" ? OA(A) ? xD(A[0], A[1]) : lD(A) : mD(A)
     }
 
-    function OD(A, B, g, o) {
+    function TD(A, B, g, o) {
         for (var t = -1, E = A == null ? 0 : A.length; ++t < E;) {
             var s = A[t];
             B(o, s, g(s), A)
         }
         return o
     }
 
-    function XD(A) {
+    function WD(A) {
         return function(B, g, o) {
-            for (var t = -1, E = Object(B), s = o(B), D = s.length; D--;) {
-                var h = s[A ? D : ++t];
+            for (var t = -1, E = Object(B), s = o(B), i = s.length; i--;) {
+                var h = s[A ? i : ++t];
                 if (g(E[h], h, E) === !1) break
             }
             return B
         }
     }
-    var vD = XD();
-    const jD = vD;
+    var OD = WD();
+    const XD = OD;
 
-    function PD(A, B) {
-        return A && jD(A, B, hg)
+    function vD(A, B) {
+        return A && XD(A, B, Fg)
     }
 
-    function zD(A, B) {
+    function jD(A, B) {
         return function(g, o) {
             if (g == null) return g;
             if (!iQ(g)) return A(g, o);
             for (var t = g.length, E = B ? t : -1, s = Object(g);
                 (B ? E-- : ++E < t) && o(s[E], E, s) !== !1;);
             return g
         }
     }
-    var _D = zD(PD);
-    const $D = _D;
+    var PD = jD(vD);
+    const zD = PD;
 
-    function Ao(A, B, g, o) {
-        return $D(A, function(t, E, s) {
+    function _D(A, B, g, o) {
+        return zD(A, function(t, E, s) {
             B(o, t, g(t), s)
         }), o
     }
 
-    function Io(A, B) {
+    function $D(A, B) {
         return function(g, o) {
-            var t = OA(g) ? OD : Ao,
+            var t = OA(g) ? TD : _D,
                 E = B ? B() : {};
-            return t(g, A, WD(o), E)
+            return t(g, A, ZD(o), E)
         }
     }
 
-    function go(A, B, g) {
+    function Ao(A, B, g) {
         for (var o = -1, t = A == null ? 0 : A.length; ++o < t;)
             if (g(B, A[o])) return !0;
         return !1
     }
-    var Qo = Object.prototype,
-        Bo = Qo.hasOwnProperty,
-        Co = Io(function(A, B, g) {
-            Bo.call(A, g) ? A[g].push(B) : _C(A, g, [B])
+    var Io = Object.prototype,
+        go = Io.hasOwnProperty,
+        Qo = $D(function(A, B, g) {
+            go.call(A, g) ? A[g].push(B) : PC(A, g, [B])
         });
-    const Eo = Co;
-    var io = 1 / 0,
-        Do = yI && 1 / Gg(new yI([, -0]))[1] == io ? function(A) {
+    const Bo = Qo;
+    var Co = 1 / 0,
+        Eo = yI && 1 / Ug(new yI([, -0]))[1] == Co ? function(A) {
             return new yI(A)
-        } : ZC;
-    const oo = Do;
-    var so = 200;
+        } : VC;
+    const io = Eo;
+    var Do = 200;
 
-    function wo(A, B, g) {
+    function oo(A, B, g) {
         var o = -1,
-            t = jC,
+            t = XC,
             E = A.length,
             s = !0,
-            D = [],
-            h = D;
-        if (g) s = !1, t = go;
-        else if (E >= so) {
-            var C = B ? null : oo(A);
-            if (C) return Gg(C);
-            s = !1, t = JQ, h = new LI
-        } else h = B ? [] : D;
+            i = [],
+            h = i;
+        if (g) s = !1, t = Ao;
+        else if (E >= Do) {
+            var C = B ? null : io(A);
+            if (C) return Ug(C);
+            s = !1, t = JQ, h = new MI
+        } else h = B ? [] : i;
         A: for (; ++o < E;) {
             var r = A[o],
                 n = B ? B(r) : r;
             if (r = g || r !== 0 ? r : 0, s && n === n) {
                 for (var M = h.length; M--;)
                     if (h[M] === n) continue A;
-                B && h.push(n), D.push(r)
-            } else t(h, n, g) || (h !== D && h.push(n), D.push(r))
+                B && h.push(n), i.push(r)
+            } else t(h, n, g) || (h !== i && h.push(n), i.push(r))
         }
-        return D
+        return i
     }
 
-    function to(A) {
-        return A && A.length ? wo(A) : []
+    function so(A) {
+        return A && A.length ? oo(A) : []
     }
-    const ho = {
-        uniq: to,
-        groupBy: Eo
+    const wo = {
+        uniq: so,
+        groupBy: Bo
     };
 
     function pQ(A, B) {
         const g = new Function("utils", "rows", "fields", A ?? "");
 
         function o(t) {
             switch (B) {
                 case "udf":
-                    if (A !== null) return g(ho, t.rows, t.fields);
+                    if (A !== null) return g(wo, t.rows, t.fields);
                     break;
                 case "infer":
                 default:
                     return t.inferData()
             }
         }
         return {
             map: o
         }
     }
     var qQ;
-    const eg = typeof window < "u",
-        Fo = A => typeof A == "function",
-        ao = A => typeof A == "string",
+    const WI = typeof window < "u",
+        to = A => typeof A == "function",
+        ho = A => typeof A == "string",
         cg = () => {};
-    eg && ((qQ = window == null ? void 0 : window.navigator) != null && qQ.userAgent) && /iP(ad|hone|od)/.test(window.navigator.userAgent);
+    WI && ((qQ = window == null ? void 0 : window.navigator) != null && qQ.userAgent) && /iP(ad|hone|od)/.test(window.navigator.userAgent);
 
     function ZA(A) {
         return typeof A == "function" ? A() : K.unref(A)
     }
 
-    function Ro(A, B) {
+    function Fo(A, B) {
         function g(...o) {
             return new Promise((t, E) => {
                 Promise.resolve(A(() => B.apply(this, o), {
                     fn: B,
                     thisArg: this,
                     args: o
                 })).then(t).catch(E)
             })
         }
         return g
     }
     const xQ = A => A();
 
-    function yo(A = xQ) {
+    function ao(A = xQ) {
         const B = K.ref(!0);
 
         function g() {
             B.value = !1
         }
 
         function o() {
@@ -1231,52 +1217,52 @@
 
     function Ng(A, B = !1, g = "Timeout") {
         return new Promise((o, t) => {
             setTimeout(B ? () => t(g) : o, A)
         })
     }
 
-    function Go(A) {
+    function Ro(A) {
         return A
     }
 
-    function Uo(A, ...B) {
+    function yo(A, ...B) {
         return B.some(g => g in A)
     }
 
-    function TI(A) {
+    function LI(A) {
         return K.getCurrentScope() ? (K.onScopeDispose(A), !0) : !1
     }
 
     function rg() {
         const A = [],
             B = t => {
                 const E = A.indexOf(t);
                 E !== -1 && A.splice(E, 1)
             };
         return {
             on: t => {
                 A.push(t);
                 const E = () => B(t);
-                return TI(E), {
+                return LI(E), {
                     off: E
                 }
             },
             off: B,
             trigger: t => {
                 A.forEach(E => E(t))
             }
         }
     }
 
     function Mg(A) {
         return typeof A == "function" ? K.computed(A) : K.ref(A)
     }
 
-    function no(A, B = !0) {
+    function bQ(A, B = !0) {
         K.getCurrentInstance() ? K.onMounted(A) : B ? A() : K.nextTick(A)
     }
 
     function Lg(A, B = !1) {
         function g(n, {
             flush: M = "sync",
             deep: R = !1,
@@ -1325,15 +1311,15 @@
             return o(null, n)
         }
 
         function s(n) {
             return o(void 0, n)
         }
 
-        function D(n) {
+        function i(n) {
             return g(Number.isNaN, n)
         }
 
         function h(n, M) {
             return g(R => {
                 const N = Array.from(R);
                 return N.includes(n) || N.includes(ZA(n))
@@ -1357,165 +1343,166 @@
                 return Lg(A, !B)
             }
         } : {
             toMatch: g,
             toBe: o,
             toBeTruthy: t,
             toBeNull: E,
-            toBeNaN: D,
+            toBeNaN: i,
             toBeUndefined: s,
             changed: C,
             changedTimes: r,
             get not() {
                 return Lg(A, !B)
             }
         }
     }
 
-    function eo(A) {
+    function Go(A) {
         return Lg(A)
     }
 
-    function co(A, B, g = {}) {
+    function Uo(A, B, g = {}) {
         const {
             immediate: o = !0
         } = g, t = K.ref(!1);
         let E = null;
 
         function s() {
             E && (clearTimeout(E), E = null)
         }
 
-        function D() {
+        function i() {
             t.value = !1, s()
         }
 
         function h(...C) {
             s(), t.value = !0, E = setTimeout(() => {
                 t.value = !1, E = null, A(...C)
             }, ZA(B))
         }
-        return o && (t.value = !0, eg && h()), TI(D), {
+        return o && (t.value = !0, WI && h()), LI(i), {
             isPending: t,
             start: h,
-            stop: D
+            stop: i
         }
     }
-    var bQ = Object.getOwnPropertySymbols,
-        No = Object.prototype.hasOwnProperty,
-        ro = Object.prototype.propertyIsEnumerable,
-        Mo = (A, B) => {
+    var VQ = Object.getOwnPropertySymbols,
+        no = Object.prototype.hasOwnProperty,
+        eo = Object.prototype.propertyIsEnumerable,
+        co = (A, B) => {
             var g = {};
-            for (var o in A) No.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
-            if (A != null && bQ)
-                for (var o of bQ(A)) B.indexOf(o) < 0 && ro.call(A, o) && (g[o] = A[o]);
+            for (var o in A) no.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
+            if (A != null && VQ)
+                for (var o of VQ(A)) B.indexOf(o) < 0 && eo.call(A, o) && (g[o] = A[o]);
             return g
         };
 
-    function Lo(A, B, g = {}) {
+    function No(A, B, g = {}) {
         const o = g,
             {
                 eventFilter: t = xQ
             } = o,
-            E = Mo(o, ["eventFilter"]);
-        return K.watch(A, Ro(t, B), E)
+            E = co(o, ["eventFilter"]);
+        return K.watch(A, Fo(t, B), E)
     }
 
-    function VQ(A, B, g) {
+    function mQ(A, B, g) {
         const o = K.watch(A, (...t) => (K.nextTick(() => o()), B(...t)), g)
     }
-    var ko = Object.defineProperty,
-        So = Object.defineProperties,
-        Jo = Object.getOwnPropertyDescriptors,
-        WI = Object.getOwnPropertySymbols,
-        mQ = Object.prototype.hasOwnProperty,
-        ZQ = Object.prototype.propertyIsEnumerable,
-        TQ = (A, B, g) => B in A ? ko(A, B, {
+    var ro = Object.defineProperty,
+        Mo = Object.defineProperties,
+        Lo = Object.getOwnPropertyDescriptors,
+        OI = Object.getOwnPropertySymbols,
+        ZQ = Object.prototype.hasOwnProperty,
+        TQ = Object.prototype.propertyIsEnumerable,
+        WQ = (A, B, g) => B in A ? ro(A, B, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: g
         }) : A[B] = g,
-        Ko = (A, B) => {
-            for (var g in B || (B = {})) mQ.call(B, g) && TQ(A, g, B[g]);
-            if (WI)
-                for (var g of WI(B)) ZQ.call(B, g) && TQ(A, g, B[g]);
+        ko = (A, B) => {
+            for (var g in B || (B = {})) ZQ.call(B, g) && WQ(A, g, B[g]);
+            if (OI)
+                for (var g of OI(B)) TQ.call(B, g) && WQ(A, g, B[g]);
             return A
         },
-        Yo = (A, B) => So(A, Jo(B)),
-        Ho = (A, B) => {
+        So = (A, B) => Mo(A, Lo(B)),
+        Jo = (A, B) => {
             var g = {};
-            for (var o in A) mQ.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
-            if (A != null && WI)
-                for (var o of WI(A)) B.indexOf(o) < 0 && ZQ.call(A, o) && (g[o] = A[o]);
+            for (var o in A) ZQ.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
+            if (A != null && OI)
+                for (var o of OI(A)) B.indexOf(o) < 0 && TQ.call(A, o) && (g[o] = A[o]);
             return g
         };
 
-    function lo(A, B, g = {}) {
+    function Ko(A, B, g = {}) {
         const o = g,
             {
                 eventFilter: t
             } = o,
-            E = Ho(o, ["eventFilter"]),
+            E = Jo(o, ["eventFilter"]),
             {
                 eventFilter: s,
-                pause: D,
+                pause: i,
                 resume: h,
                 isActive: C
-            } = yo(t);
+            } = ao(t);
         return {
-            stop: Lo(A, B, Yo(Ko({}, E), {
+            stop: No(A, B, So(ko({}, E), {
                 eventFilter: s
             })),
-            pause: D,
+            pause: i,
             resume: h,
             isActive: C
         }
     }
 
     function kg(A) {
         var B;
         const g = ZA(A);
         return (B = g == null ? void 0 : g.$el) != null ? B : g
     }
-    const kI = eg ? window : void 0;
+    const kI = WI ? window : void 0,
+        Yo = WI ? window.document : void 0;
 
-    function WQ(...A) {
+    function OQ(...A) {
         let B, g, o, t;
-        if (ao(A[0]) || Array.isArray(A[0]) ? ([g, o, t] = A, B = kI) : [B, g, o, t] = A, !B) return cg;
+        if (ho(A[0]) || Array.isArray(A[0]) ? ([g, o, t] = A, B = kI) : [B, g, o, t] = A, !B) return cg;
         Array.isArray(g) || (g = [g]), Array.isArray(o) || (o = [o]);
         const E = [],
             s = () => {
                 E.forEach(r => r()), E.length = 0
             },
-            D = (r, n, M) => (r.addEventListener(n, M, t), () => r.removeEventListener(n, M, t)),
+            i = (r, n, M) => (r.addEventListener(n, M, t), () => r.removeEventListener(n, M, t)),
             h = K.watch(() => kg(B), r => {
-                s(), r && E.push(...g.flatMap(n => o.map(M => D(r, n, M))))
+                s(), r && E.push(...g.flatMap(n => o.map(M => i(r, n, M))))
             }, {
                 immediate: !0,
                 flush: "post"
             }),
             C = () => {
                 h(), s()
             };
-        return TI(C), C
+        return LI(C), C
     }
 
-    function OQ(A, B, g) {
+    function XQ(A, B, g) {
         const {
             immediate: o = !0,
             delay: t = 0,
             onError: E = cg,
             onSuccess: s = cg,
-            resetOnExecute: D = !0,
+            resetOnExecute: i = !0,
             shallow: h = !0,
             throwError: C
         } = g ?? {}, r = h ? K.shallowRef(B) : K.ref(B), n = K.ref(!1), M = K.ref(!1), R = K.ref(void 0);
         async function N(a = 0, ...G) {
-            D && (r.value = B), R.value = void 0, n.value = !1, M.value = !0, a > 0 && await Ng(a);
+            i && (r.value = B), R.value = void 0, n.value = !1, M.value = !0, a > 0 && await Ng(a);
             const y = typeof A == "function" ? A(...G) : A;
             try {
                 const c = await y;
                 r.value = c, n.value = !0, s(c)
             } catch (c) {
                 if (R.value = c, E(c), C) throw R
             } finally {
@@ -1528,48 +1515,48 @@
             isReady: n,
             isLoading: M,
             error: R,
             execute: N
         }
     }
 
-    function fo(A, B = !1) {
+    function Ho(A, B = !1) {
         const g = K.ref(),
             o = () => g.value = !!A();
-        return o(), no(o, B), g
+        return o(), bQ(o, B), g
     }
     const Sg = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {},
         Jg = "__vueuse_ssr_handlers__";
     Sg[Jg] = Sg[Jg] || {};
-    const uo = Sg[Jg];
+    const lo = Sg[Jg];
 
-    function po(A, B) {
-        return uo[A] || B
+    function fo(A, B) {
+        return lo[A] || B
     }
 
-    function qo(A) {
+    function uo(A) {
         return A == null ? "any" : A instanceof Set ? "set" : A instanceof Map ? "map" : A instanceof Date ? "date" : typeof A == "boolean" ? "boolean" : typeof A == "string" ? "string" : typeof A == "object" ? "object" : Number.isNaN(A) ? "any" : "number"
     }
-    var xo = Object.defineProperty,
-        XQ = Object.getOwnPropertySymbols,
-        bo = Object.prototype.hasOwnProperty,
-        Vo = Object.prototype.propertyIsEnumerable,
-        vQ = (A, B, g) => B in A ? xo(A, B, {
+    var po = Object.defineProperty,
+        vQ = Object.getOwnPropertySymbols,
+        qo = Object.prototype.hasOwnProperty,
+        xo = Object.prototype.propertyIsEnumerable,
+        jQ = (A, B, g) => B in A ? po(A, B, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: g
         }) : A[B] = g,
-        jQ = (A, B) => {
-            for (var g in B || (B = {})) bo.call(B, g) && vQ(A, g, B[g]);
-            if (XQ)
-                for (var g of XQ(B)) Vo.call(B, g) && vQ(A, g, B[g]);
+        PQ = (A, B) => {
+            for (var g in B || (B = {})) qo.call(B, g) && jQ(A, g, B[g]);
+            if (vQ)
+                for (var g of vQ(B)) xo.call(B, g) && jQ(A, g, B[g]);
             return A
         };
-    const mo = {
+    const bo = {
         boolean: {
             read: A => A === "true",
             write: A => String(A)
         },
         object: {
             read: A => JSON.parse(A),
             write: A => JSON.stringify(A)
@@ -1596,50 +1583,50 @@
         },
         date: {
             read: A => new Date(A),
             write: A => A.toISOString()
         }
     };
 
-    function Zo(A, B, g, o = {}) {
+    function Vo(A, B, g, o = {}) {
         var t;
         const {
             flush: E = "pre",
             deep: s = !0,
-            listenToStorageChanges: D = !0,
+            listenToStorageChanges: i = !0,
             writeDefaults: h = !0,
             mergeDefaults: C = !1,
             shallow: r,
             window: n = kI,
             eventFilter: M,
             onError: R = p => {
                 console.error(p)
             }
         } = o, N = (r ? K.shallowRef : K.ref)(B);
         if (!g) try {
-            g = po("getDefaultStorage", () => {
+            g = fo("getDefaultStorage", () => {
                 var p;
                 return (p = kI) == null ? void 0 : p.localStorage
             })()
         } catch (p) {
             R(p)
         }
         if (!g) return N;
         const a = ZA(B),
-            G = qo(a),
-            y = (t = o.serializer) != null ? t : mo[G],
+            G = uo(a),
+            y = (t = o.serializer) != null ? t : bo[G],
             {
                 pause: c,
                 resume: k
-            } = lo(N, () => H(N.value), {
+            } = Ko(N, () => H(N.value), {
                 flush: E,
                 deep: s,
                 eventFilter: M
             });
-        return n && D && WQ(n, "storage", T), T(), N;
+        return n && i && OQ(n, "storage", T), T(), N;
 
         function H(p) {
             try {
                 if (p == null) g.removeItem(A);
                 else {
                     const j = y.write(p),
                         b = g.getItem(A);
@@ -1656,15 +1643,15 @@
         }
 
         function l(p) {
             const j = p ? p.newValue : g.getItem(A);
             if (j == null) return h && a !== null && g.setItem(A, y.write(a)), a;
             if (!p && C) {
                 const b = y.read(j);
-                return Fo(C) ? C(b, a) : G === "object" && !Array.isArray(b) ? jQ(jQ({}, a), b) : b
+                return to(C) ? C(b, a) : G === "object" && !Array.isArray(b) ? PQ(PQ({}, a), b) : b
             } else return typeof j != "string" ? j : y.read(j)
         }
 
         function T(p) {
             if (!(p && p.storageArea !== g)) {
                 if (p && p.key == null) {
                     N.value = a;
@@ -1679,162 +1666,162 @@
                     } finally {
                         p ? K.nextTick(k) : k()
                     }
                 }
             }
         }
     }
-    var PQ = Object.getOwnPropertySymbols,
-        To = Object.prototype.hasOwnProperty,
-        Wo = Object.prototype.propertyIsEnumerable,
-        Oo = (A, B) => {
+    var zQ = Object.getOwnPropertySymbols,
+        mo = Object.prototype.hasOwnProperty,
+        Zo = Object.prototype.propertyIsEnumerable,
+        To = (A, B) => {
             var g = {};
-            for (var o in A) To.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
-            if (A != null && PQ)
-                for (var o of PQ(A)) B.indexOf(o) < 0 && Wo.call(A, o) && (g[o] = A[o]);
+            for (var o in A) mo.call(A, o) && B.indexOf(o) < 0 && (g[o] = A[o]);
+            if (A != null && zQ)
+                for (var o of zQ(A)) B.indexOf(o) < 0 && Zo.call(A, o) && (g[o] = A[o]);
             return g
         };
 
-    function Xo(A, B, g = {}) {
+    function Wo(A, B, g = {}) {
         const o = g,
             {
                 window: t = kI
             } = o,
-            E = Oo(o, ["window"]);
+            E = To(o, ["window"]);
         let s;
-        const D = fo(() => t && "ResizeObserver" in t),
+        const i = Ho(() => t && "ResizeObserver" in t),
             h = () => {
                 s && (s.disconnect(), s = void 0)
             },
             C = K.watch(() => kg(A), n => {
-                h(), D.value && t && n && (s = new ResizeObserver(B), s.observe(n, E))
+                h(), i.value && t && n && (s = new ResizeObserver(B), s.observe(n, E))
             }, {
                 immediate: !0,
                 flush: "post"
             }),
             r = () => {
                 h(), C()
             };
-        return TI(r), {
-            isSupported: D,
+        return LI(r), {
+            isSupported: i,
             stop: r
         }
     }
 
-    function zQ(A, B = {
+    function _Q(A, B = {
         width: 0,
         height: 0
     }, g = {}) {
         const {
             box: o = "content-box"
         } = g, t = K.ref(B.width), E = K.ref(B.height);
-        return Xo(A, ([s]) => {
-            const D = o === "border-box" ? s.borderBoxSize : o === "content-box" ? s.contentBoxSize : s.devicePixelContentBoxSize;
-            D ? (t.value = D.reduce((h, {
+        return Wo(A, ([s]) => {
+            const i = o === "border-box" ? s.borderBoxSize : o === "content-box" ? s.contentBoxSize : s.devicePixelContentBoxSize;
+            i ? (t.value = i.reduce((h, {
                 inlineSize: C
-            }) => h + C, 0), E.value = D.reduce((h, {
+            }) => h + C, 0), E.value = i.reduce((h, {
                 blockSize: C
             }) => h + C, 0)) : (t.value = s.contentRect.width, E.value = s.contentRect.height)
         }, g), K.watch(() => kg(A), s => {
             t.value = s ? B.width : 0, E.value = s ? B.height : 0
         }), {
             width: t,
             height: E
         }
     }
-    var vo = Object.defineProperty,
-        jo = Object.defineProperties,
-        Po = Object.getOwnPropertyDescriptors,
-        _Q = Object.getOwnPropertySymbols,
-        zo = Object.prototype.hasOwnProperty,
-        _o = Object.prototype.propertyIsEnumerable,
-        $Q = (A, B, g) => B in A ? vo(A, B, {
+    var Oo = Object.defineProperty,
+        Xo = Object.defineProperties,
+        vo = Object.getOwnPropertyDescriptors,
+        $Q = Object.getOwnPropertySymbols,
+        jo = Object.prototype.hasOwnProperty,
+        Po = Object.prototype.propertyIsEnumerable,
+        AB = (A, B, g) => B in A ? Oo(A, B, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: g
         }) : A[B] = g,
         fA = (A, B) => {
-            for (var g in B || (B = {})) zo.call(B, g) && $Q(A, g, B[g]);
-            if (_Q)
-                for (var g of _Q(B)) _o.call(B, g) && $Q(A, g, B[g]);
+            for (var g in B || (B = {})) jo.call(B, g) && AB(A, g, B[g]);
+            if ($Q)
+                for (var g of $Q(B)) Po.call(B, g) && AB(A, g, B[g]);
             return A
         },
-        SI = (A, B) => jo(A, Po(B));
-    const $o = {
+        SI = (A, B) => Xo(A, vo(B));
+    const zo = {
         json: "application/json",
         text: "text/plain"
     };
 
-    function AB(A) {
-        return Uo(A, "immediate", "refetch", "initialData", "timeout", "beforeFetch", "afterFetch", "onFetchError", "fetch")
+    function IB(A) {
+        return yo(A, "immediate", "refetch", "initialData", "timeout", "beforeFetch", "afterFetch", "onFetchError", "fetch")
     }
 
     function Kg(A) {
         return typeof Headers < "u" && A instanceof Headers ? Object.fromEntries([...A.entries()]) : A
     }
 
-    function As(A, ...B) {
+    function _o(A, ...B) {
         var g;
         const o = typeof AbortController == "function";
         let t = {},
             E = {
                 immediate: !0,
                 refetch: !1,
                 timeout: 0
             };
         const s = {
             method: "GET",
             type: "text",
             payload: void 0
         };
-        B.length > 0 && (AB(B[0]) ? E = fA(fA({}, E), B[0]) : t = B[0]), B.length > 1 && AB(B[1]) && (E = fA(fA({}, E), B[1]));
+        B.length > 0 && (IB(B[0]) ? E = fA(fA({}, E), B[0]) : t = B[0]), B.length > 1 && IB(B[1]) && (E = fA(fA({}, E), B[1]));
         const {
-            fetch: D = (g = kI) == null ? void 0 : g.fetch,
+            fetch: i = (g = kI) == null ? void 0 : g.fetch,
             initialData: h,
             timeout: C
         } = E, r = rg(), n = rg(), M = rg(), R = K.ref(!1), N = K.ref(!1), a = K.ref(!1), G = K.ref(null), y = K.shallowRef(null), c = K.shallowRef(null), k = K.shallowRef(h), H = K.computed(() => o && N.value);
         let l, T;
         const p = () => {
                 o && l && l.abort()
             },
             j = Z => {
                 N.value = Z, R.value = !Z
             };
-        C && (T = co(p, C, {
+        C && (T = Uo(p, C, {
             immediate: !1
         }));
         const b = async (Z = !1) => {
             var iA;
             j(!0), c.value = null, G.value = null, a.value = !1, l = void 0, o && (l = new AbortController, l.signal.onabort = () => a.value = !0, t = SI(fA({}, t), {
                 signal: l.signal
             }));
             const W = {
                 method: s.method,
                 headers: {}
             };
             if (s.payload) {
                 const f = Kg(W.headers);
-                s.payloadType && (f["Content-Type"] = (iA = $o[s.payloadType]) != null ? iA : s.payloadType);
+                s.payloadType && (f["Content-Type"] = (iA = zo[s.payloadType]) != null ? iA : s.payloadType);
                 const q = ZA(s.payload);
                 W.body = s.payloadType === "json" ? JSON.stringify(q) : q
             }
             let tA = !1;
             const _ = {
                 url: ZA(A),
                 options: fA(fA({}, W), t),
                 cancel: () => {
                     tA = !0
                 }
             };
-            if (E.beforeFetch && Object.assign(_, await E.beforeFetch(_)), tA || !D) return j(!1), Promise.resolve(null);
+            if (E.beforeFetch && Object.assign(_, await E.beforeFetch(_)), tA || !i) return j(!1), Promise.resolve(null);
             let AA = null;
             return T && T.start(), new Promise((f, q) => {
                 var sA;
-                D(_.url, SI(fA(fA({}, W), _.options), {
+                i(_.url, SI(fA(fA({}, W), _.options), {
                     headers: fA(fA({}, Kg(W.headers)), Kg((sA = _.options) == null ? void 0 : sA.headers))
                 })).then(async CA => {
                     if (y.value = CA, G.value = CA.status, AA = await CA[s.type](), E.afterFetch && G.value >= 200 && G.value < 300 && ({
                             data: AA
                         } = await E.afterFetch({
                             data: AA,
                             response: CA
@@ -1900,15 +1887,15 @@
                     })
                 }
             }
         }
 
         function x() {
             return new Promise((Z, iA) => {
-                eo(R).toBe(!0).then(() => Z(oA)).catch(W => iA(W))
+                Go(R).toBe(!0).then(() => Z(oA)).catch(W => iA(W))
             })
         }
 
         function F(Z) {
             return () => {
                 if (!N.value) return s.type = Z, SI(fA({}, oA), {
                     then(iA, W) {
@@ -1919,36 +1906,68 @@
         }
         return E.immediate && setTimeout(b, 0), SI(fA({}, oA), {
             then(Z, iA) {
                 return x().then(Z, iA)
             }
         })
     }
-    var IB;
+    var gB;
     (function(A) {
         A.UP = "UP", A.RIGHT = "RIGHT", A.DOWN = "DOWN", A.LEFT = "LEFT", A.NONE = "NONE"
-    })(IB || (IB = {}));
+    })(gB || (gB = {}));
+    let $o = 0;
+
+    function As(A, B = {}) {
+        const g = K.ref(!1),
+            {
+                document: o = Yo,
+                immediate: t = !0,
+                manual: E = !1,
+                id: s = `vueuse_styletag_${++$o}`
+            } = B,
+            i = K.ref(A);
+        let h = () => {};
+        const C = () => {
+                if (!o) return;
+                const n = o.getElementById(s) || o.createElement("style");
+                n.isConnected || (n.type = "text/css", n.id = s, B.media && (n.media = B.media), o.head.appendChild(n)), !g.value && (h = K.watch(i, M => {
+                    n.textContent = M
+                }, {
+                    immediate: !0
+                }), g.value = !0)
+            },
+            r = () => {
+                !o || !g.value || (h(), o.head.removeChild(o.getElementById(s)), g.value = !1)
+            };
+        return t && !E && bQ(C), E || LI(r), {
+            id: s,
+            css: i,
+            unload: r,
+            load: C,
+            isLoaded: K.readonly(g)
+        }
+    }
     var Is = Object.defineProperty,
-        gB = Object.getOwnPropertySymbols,
+        QB = Object.getOwnPropertySymbols,
         gs = Object.prototype.hasOwnProperty,
         Qs = Object.prototype.propertyIsEnumerable,
-        QB = (A, B, g) => B in A ? Is(A, B, {
+        BB = (A, B, g) => B in A ? Is(A, B, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: g
         }) : A[B] = g,
         Bs = (A, B) => {
-            for (var g in B || (B = {})) gs.call(B, g) && QB(A, g, B[g]);
-            if (gB)
-                for (var g of gB(B)) Qs.call(B, g) && QB(A, g, B[g]);
+            for (var g in B || (B = {})) gs.call(B, g) && BB(A, g, B[g]);
+            if (QB)
+                for (var g of QB(B)) Qs.call(B, g) && BB(A, g, B[g]);
             return A
         };
     Bs({
-        linear: Go
+        linear: Ro
     }, {
         easeInSine: [.12, 0, .39, 0],
         easeOutSine: [.61, 1, .88, 1],
         easeInOutSine: [.37, 0, .63, 1],
         easeInQuad: [.11, 0, .5, 0],
         easeOutQuad: [.5, 1, .89, 1],
         easeInOutQuad: [.45, 0, .55, 1],
@@ -1975,90 +1994,92 @@
             __name: "TextValue",
             props: {
                 model: null
             },
             setup(A) {
                 const B = A;
                 K.useCssVars(h => ({
-                    "1d4d298a": s.value
+                    "4832b7db": s.value
                 }));
-                const g = K.inject(xI),
+                const g = K.inject(bI),
                     o = B.model,
                     t = o.contexts.map(h => {
                         if (typeof h == "string") return K.computed(() => h);
                         const C = h,
                             r = g.createSqlQuery(o.id, C.sql),
                             n = pQ(C.jsMap, C.type);
                         return K.computed(() => {
                             const M = r.query();
                             return M.rows.length === 0 ? null : n.map(M)
                         })
                     }),
                     E = K.ref(null),
                     s = K.ref("initial"),
                     {
-                        height: D
-                    } = zQ(E);
-                return VQ(D, h => {
+                        height: i
+                    } = _Q(E);
+                return mQ(i, h => {
                     s.value = h + "px"
                 }), (h, C) => (K.openBlock(), K.createElementBlock("div", {
                     ref_key: "boxRef",
                     ref: E,
-                    class: K.normalizeClass(["textValue-box", B.model.classes])
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(t), r => (K.openBlock(), K.createElementBlock("span", null, K.toDisplayString(r.value), 1))), 256))], 2))
+                    class: K.normalizeClass(["textValue-box", B.model.classes]),
+                    style: K.normalizeStyle(B.model.styles)
+                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(t), r => (K.openBlock(), K.createElementBlock("span", null, K.toDisplayString(r.value), 1))), 256))], 6))
             }
         }),
-        Ww = "",
+        Xw = "",
         Es = WA(Cs, [
-            ["__scopeId", "data-v-e4e5740d"]
+            ["__scopeId", "data-v-7901b929"]
         ]),
         is = ["innerHTML"],
         Ds = K.defineComponent({
             __name: "Markdown",
             props: {
                 model: null
             },
             setup(A) {
                 const B = A;
                 K.useCssVars(C => ({
-                    "07bc4221": s.value
+                    "6b8d9ae4": s.value
                 }));
-                const g = K.inject(xI),
+                const g = K.inject(bI),
                     o = B.model,
                     t = o.contexts.map(C => {
                         if (typeof C == "string") return K.computed(() => C);
                         const r = C,
                             n = g.createSqlQuery(o.id, r.sql),
                             M = pQ(r.jsMap, r.type);
                         return K.computed(() => {
                             const R = n.query();
                             return R.rows.length === 0 ? null : JSON.stringify(M.map(R))
                         })
                     }),
                     E = K.ref(null),
                     s = K.ref("initial"),
                     {
-                        height: D
-                    } = zQ(E);
-                VQ(D, C => {
+                        height: i
+                    } = _Q(E);
+                mQ(i, C => {
                     s.value = C + "px"
                 });
                 const h = K.computed(() => t.map(C => C.value).join(""));
                 return (C, r) => (K.openBlock(), K.createElementBlock("div", {
                     ref_key: "boxRef",
                     ref: E,
-                    class: K.normalizeClass(["md-box", B.model.classes])
+                    class: K.normalizeClass(["md-box", B.model.classes]),
+                    style: K.normalizeStyle(K.unref(o).styles)
                 }, [K.createElementVNode("span", {
                     innerHTML: K.unref(h)
-                }, null, 8, is)], 2))
+                }, null, 8, is)], 6))
             }
         }),
-        Ow = "",
+        vw = "",
         os = WA(Ds, [
-            ["__scopeId", "data-v-85715e33"]
+            ["__scopeId", "data-v-836262bc"]
         ]),
         ss = K.defineComponent({
             __name: "Icon",
             props: {
                 model: null
             },
             setup(A) {
@@ -2075,15 +2096,15 @@
                     class: K.normalizeClass(["pybi-svg-icon", B.model.classes]),
                     style: o
                 }, [K.createElementVNode("use", {
                     href: t
                 })], 2))
             }
         }),
-        Xw = "",
+        jw = "",
         ws = WA(ss, [
             ["__scopeId", "data-v-b780493d"]
         ]),
         ts = ["innerHTML"],
         hs = K.defineComponent({
             __name: "SvgIcon",
             props: {
@@ -2100,188 +2121,210 @@
                 return (t, E) => (K.openBlock(), K.createElementBlock("div", {
                     class: K.normalizeClass(["pybi-svg-icon", K.unref(g).classes]),
                     innerHTML: K.unref(g).svg,
                     style: o
                 }, null, 10, ts))
             }
         }),
-        vw = "",
+        Pw = "",
         Fs = WA(hs, [
             ["__scopeId", "data-v-71dedf8c"]
         ]),
-        as = new Map([
-            [pA.Box, AC],
-            [pA.ColBox, iC],
-            [pA.FlowBox, gC],
-            [pA.GridBox, BC],
+        as = ["data-auto-grow"],
+        Rs = K.defineComponent({
+            __name: "Space",
+            props: {
+                model: null
+            },
+            setup(A) {
+                const B = A;
+                K.useCssVars(o => ({
+                    "04fcf714": K.unref(g)
+                }));
+                const g = B.model.space ?? "0.2em";
+                return (o, t) => (K.openBlock(), K.createElementBlock("div", {
+                    class: K.normalizeClass(["pybi-space", B.model.classes]),
+                    "data-auto-grow": B.model.autoFillRow
+                }, null, 10, as))
+            }
+        }),
+        zw = "",
+        ys = WA(Rs, [
+            ["__scopeId", "data-v-7f41dd6f"]
+        ]),
+        Gs = new Map([
+            [pA.Box, IC],
+            [pA.FlowBox, QC],
+            [pA.GridBox, CC],
             [pA.TextValue, Es],
             [pA.Markdown, os],
             [pA.Icon, ws],
-            [pA.SvgIcon, Fs]
+            [pA.SvgIcon, Fs],
+            [pA.Space, ys]
         ]);
 
-    function Rs(A) {
-        return as.get(A) ?? A
+    function Us(A) {
+        return Gs.get(A) ?? A
     }
-    const GI = K.defineComponent({
+    const JI = K.defineComponent({
             __name: "Dynamic",
             props: {
                 component: null
             },
             setup(A) {
                 const B = A,
-                    g = K.inject(xI),
+                    g = K.inject(bI),
                     o = B.component,
-                    t = Rs(B.component.tag),
+                    t = Us(B.component.tag),
                     E = K.computed(() => {
                         if (o.visible === void 0) return !0;
                         if (typeof o.visible != "boolean") {
-                            const D = o.visible,
-                                C = g.createSqlQuery(o.id, D.sql).query();
+                            const i = o.visible,
+                                C = g.createSqlQuery(o.id, i.sql).query();
                             return C.rows.length === 0 ? !1 : C.rows[0][C.fields[0]]
                         }
                         return o.visible
                     });
                 let s = o.styles;
                 return o.gridArea && (s = {
                     ...s,
                     gridArea: o.gridArea
-                }), (D, h) => K.unref(E) ? (K.openBlock(), K.createBlock(jg, {
+                }), (i, h) => K.unref(E) ? (K.openBlock(), K.createBlock(jg, {
                     key: 0
                 }, {
                     default: K.withCtx(() => [(K.openBlock(), K.createBlock(K.resolveDynamicComponent(K.unref(t)), {
                         style: K.normalizeStyle(K.unref(s)),
                         id: B.component.id,
                         "data-cp-tag": B.component.tag,
                         "data-debug-tag": B.component.debugTag,
                         model: B.component
                     }, null, 8, ["style", "id", "data-cp-tag", "data-debug-tag", "model"]))]),
                     _: 1
                 })) : K.createCommentVNode("", !0)
             }
         }),
-        ys = /(?:from|join)\s+(\w+\b)/igm,
-        Gs = /(?:select)\s+?(.+?)\s+from/ims;
+        ns = /(?:from|join)\s+(\w+\b)/igm,
+        es = /(?:select)\s+?(.+?)\s+from/ims;
 
-    function Us() {
+    function cs() {
         function A(o) {
-            const t = Array.from(o.matchAll(ys));
+            const t = Array.from(o.matchAll(ns));
             if (t.length === 0) throw new Error(`table name not found in [${o}]`);
             return t.map(E => E[1])
         }
 
         function B(o) {
-            const t = o.match(Gs);
+            const t = o.match(es);
             if (t === null) throw new Error(`fields not found in [${o}]`);
             const E = [];
-            for (const s of ns(t[1])) {
-                const D = s.split(" as ");
-                D.length === 1 ? E.push(s.trim()) : E.push(D[1].trim())
+            for (const s of Ns(t[1])) {
+                const i = s.split(" as ");
+                i.length === 1 ? E.push(s.trim()) : E.push(i[1].trim())
             }
             return E
         }
 
         function g(o, t, E) {
-            return o.replace(new RegExp(`${BB.pat}${t}`, BB.flags), `$1 (${E})`)
+            return o.replace(new RegExp(`${CB.pat}${t}`, CB.flags), `$1 (${E})`)
         }
         return {
             getTableNames: A,
             getFieldsForHeader: B,
             replaceTableToFilterQuery: g
         }
     }
 
-    function* ns(A) {
+    function* Ns(A) {
         let B = 0,
             g = 0;
         for (let o = 0; o < A.length; o++) {
             const t = A[o];
             t == "," && B == 0 ? (yield A.slice(g, o), g = o + 1) : t == "(" ? B += 1 : t == ")" && (B -= 1)
         }
         g <= A.length - 1 && (yield A.slice(g, A.length))
     }
 
-    function es() {
+    function rs() {
         return {
             pat: "(from|left\\s*?(outer)?\\s*?join|right\\s*?(outer)?\\s*?join|(inner)?\\s*?join|cross\\s*?join)\\s+?",
             flags: "gim"
         }
     }
-    const BB = es();
+    const CB = rs();
 
-    function CB(A, B) {
+    function EB(A, B) {
         return `${A.id}_opt${B}`
     }
 
-    function cs(A) {
+    function Ms(A) {
         const B = new Map,
             g = new Map;
-        for (const s of EB(A)) {
+        for (const s of iB(A)) {
             if (B.set(s.id, s), s.tag === pA.EChart) {
-                const D = s;
-                D.chartInfos.forEach((h, C) => {
-                    const r = CB(D, C);
-                    g.set(r, D.id)
+                const i = s;
+                i.chartInfos.forEach((h, C) => {
+                    const r = EB(i, C);
+                    g.set(r, i.id)
                 })
             } else "updateInfos" in s && g.set(s.id, s.id);
             "visible" in s && typeof s.visible != "boolean" && g.set(s.id, s.id)
         }
 
         function o(s) {
-            const D = B.get(s);
-            if (!D) throw new Error(`not found Component[id:${s}]`);
-            return D
+            const i = B.get(s);
+            if (!i) throw new Error(`not found Component[id:${s}]`);
+            return i
         }
 
         function t(s) {
-            const D = g.get(s);
-            if (!D) throw new Error(`not found updateId[${s}]`);
-            return o(D)
+            const i = g.get(s);
+            if (!i) throw new Error(`not found updateId[${s}]`);
+            return o(i)
         }
 
         function E() {
             return A
         }
         return {
             getComponent: o,
             getComponentByUpdateId: t,
             getApp: E
         }
     }
 
-    function* EB(A) {
+    function* iB(A) {
         const B = [A];
         for (; B.length > 0;) {
             const g = B.pop();
             for (const o of g.children) o.children && B.push(o), yield o
         }
     }
-    const Ns = new Map([
+    const Ls = new Map([
             ["elSlicer", new Set([pA.EChart, "elTable", "qsTable"])],
             ["qsSlicer", new Set([pA.EChart, "elTable", "qsTable"])]
         ]),
-        iB = A => !1;
+        DB = A => !1;
 
-    function rs(A, B) {
+    function ks(A, B) {
         const g = B.getComponentByUpdateId;
         if (A) {
             const o = g(A),
-                t = Ns.get(o.tag);
-            return t ? E => t.has(g(E).tag) : iB
+                t = Ls.get(o.tag);
+            return t ? E => t.has(g(E).tag) : DB
         }
-        return iB
+        return DB
     }
 
     function* Yg(A, B, g, o) {
         const t = new Set([...g, B]),
-            E = rs(B, o);
-        for (const [s, D] of A.entries()) !t.has(s) && !E(s) && D.value !== "" && (yield K.readonly(D))
+            E = ks(B, o);
+        for (const [s, i] of A.entries()) !t.has(s) && !E(s) && i.value !== "" && (yield K.readonly(i))
     }
 
-    function Ms(A, B) {
+    function Ss(A, B) {
         const g = new Map;
 
         function o(h, C = !1) {
             const r = `select * from ${A}`;
             return C ? K.ref(r) : K.computed(() => {
                 const M = Array.from(Yg(g, h, [], B.component)).map(R => R.value).join(" and ");
                 return M ? `${r} where ${M}` : r
@@ -2297,37 +2340,37 @@
             g.get(h).value = ""
         }
 
         function s(h) {
             g.set(h, K.ref(""))
         }
 
-        function D() {
+        function i() {
             return Array.from(g.entries()).map(([h, C]) => ({
                 id: h,
                 filter: C
             }))
         }
         return {
             typeName: "dataSource",
             name: A,
             toSqlWithFilters: o,
             addFilter: t,
             removeFilters: E,
             initFilter: s,
-            getAllFilters: D
+            getAllFilters: i
         }
     }
 
-    function DB(A, B, g = [], o) {
+    function oB(A, B, g = [], o) {
         const t = [],
             E = new Map,
             s = new Set(g);
 
-        function D(R, N = !1) {
+        function i(R, N = !1) {
             let a = B;
             return K.computed(() => {
                 if (t.forEach(c => {
                         const k = s.has(c.name),
                             H = c.toSqlWithFilters(R, k);
                         a = o.sqlAnalyze.replaceTableToFilterQuery(a, c.name, H.value)
                     }), N) return a;
@@ -2359,41 +2402,41 @@
             }))
         }
         return {
             typeName: "dataView",
             name: A,
             sql: B,
             addLinkageDataset: h,
-            toSqlWithFilters: D,
+            toSqlWithFilters: i,
             addFilter: C,
             removeFilters: r,
             initFilter: n,
             cp2FilterMap: E,
             getAllFilters: M
         }
     }
-    const oB = /\$\{\}/;
+    const sB = /\$\{\}/;
 
-    function Ls(A, B, g, o = [], t) {
-        const E = DB(A, "", o, t);
+    function Js(A, B, g, o = [], t) {
+        const E = oB(A, "", o, t);
         let s = null,
-            D = g.agg;
-        D.match(oB) || (D = `${D}(\${})`);
+            i = g.agg;
+        i.match(sB) || (i = `${i}(\${})`);
 
         function h(r) {
             return K.computed(() => {
                 if (s === null) throw new Error("pivot dataset not found source");
                 const n = s.toSqlWithFilters(r);
 
                 function M() {
                     const G = t.db.query2tempory(`temp_${A}`, n.value),
                         k = t.db.queryAll(`select distinct ${g.column} as value from ${G}`).rows.map(H => H.value).map(H => {
                             const l = t.db.parse2sqlValueBaseFieldType(G, g.column, H),
                                 T = `${g.cell}) filter (where ${g.column} = ${l}`;
-                            return `${D.replace(oB,T)} as "${H}"`
+                            return `${i.replace(sB,T)} as "${H}"`
                         }).join(",");
                     return g.excludeRowFields ? `select  ${k} from ${G} group by ${g.row} order by ${g.row}` : `select ${g.row} , ${k} from ${G} group by ${g.row} order by ${g.row}`
                 }
                 const R = M(),
                     a = Array.from(Yg(E.cp2FilterMap, r, [], t.component)).map(G => G.value).join(" and ");
                 return a ? `select * from (${R}) where ${a}` : R
             })
@@ -2410,119 +2453,119 @@
             addLinkageDataset: C,
             addFilter: E.addFilter,
             removeFilters: E.removeFilters,
             initFilter: E.initFilter
         }
     }
 
-    function ks(A, B) {
-        const g = Ss(A.dataSources, A.dataViews, B);
-        Js(A, g);
+    function Ks(A, B) {
+        const g = Ys(A.dataSources, A.dataViews, B);
+        Hs(A, g);
 
-        function o(s, D) {
-            return g.getDataset(s).toSqlWithFilters(D)
+        function o(s, i) {
+            return g.getDataset(s).toSqlWithFilters(i)
         }
 
-        function t(s, D, h) {
-            g.getDataset(D).addFilter(s, h)
+        function t(s, i, h) {
+            g.getDataset(i).addFilter(s, h)
         }
 
-        function E(s, D) {
-            g.getDataset(D).removeFilters(s)
+        function E(s, i) {
+            g.getDataset(i).removeFilters(s)
         }
         return {
             createSql: o,
             addFilter: t,
             removeFilters: E,
             getDataset: g.getDataset,
             getAllDataset: g.getAllDataset
         }
     }
 
-    function Ss(A, B, g) {
+    function Ys(A, B, g) {
         const o = new Map;
 
-        function t(D) {
-            const h = o.get(D);
-            if (!h) throw new Error(`not found dataset[name:${D}] in mapping`);
+        function t(i) {
+            const h = o.get(i);
+            if (!h) throw new Error(`not found dataset[name:${i}] in mapping`);
             return h
         }
-        A.forEach(D => {
-            const h = Ms(D.name, {
+        A.forEach(i => {
+            const h = Ss(i.name, {
                 component: g.component
             });
-            o.set(D.name, h)
-        }), B.forEach(D => {
-            switch (D.type) {
+            o.set(i.name, h)
+        }), B.forEach(i => {
+            switch (i.type) {
                 case "sql": {
-                    const h = D,
-                        C = DB(h.name, h.sql, h.excludeLinkages, {
+                    const h = i,
+                        C = oB(h.name, h.sql, h.excludeLinkages, {
                             component: g.component,
                             sqlAnalyze: g.sqlAnalyze
                         });
-                    o.set(D.name, C)
+                    o.set(i.name, C)
                 }
                 break;
                 case "pivot": {
-                    const h = D,
-                        C = Ls(h.name, h.source, h.pivotOptions, h.excludeLinkages, g);
-                    o.set(D.name, C)
+                    const h = i,
+                        C = Js(h.name, h.source, h.pivotOptions, h.excludeLinkages, g);
+                    o.set(i.name, C)
                 }
                 break
             }
         });
-        for (const D of o.values()) {
-            if (D.typeName === "dataView") {
-                const h = D;
+        for (const i of o.values()) {
+            if (i.typeName === "dataView") {
+                const h = i;
                 g.sqlAnalyze.getTableNames(h.sql).forEach(r => {
                     const n = t(r);
                     h.addLinkageDataset(n)
                 })
             }
-            if (D.typeName === "pivot-dataView") {
-                const h = D,
+            if (i.typeName === "pivot-dataView") {
+                const h = i,
                     C = t(h.sourceDatasetName);
                 h.addLinkageDataset(C)
             }
         }
 
-        function E(D) {
-            return t(D)
+        function E(i) {
+            return t(i)
         }
 
         function s() {
             return Array.from(o.values())
         }
         return {
             getDataset: E,
             getAllDataset: s
         }
     }
 
-    function Js(A, B) {
-        for (const g of EB(A)) {
+    function Hs(A, B) {
+        for (const g of iB(A)) {
             if (g.tag === pA.EChart) {
                 const o = g;
                 o.chartInfos.forEach((t, E) => {
                     t.updateInfos.forEach(s => {
-                        const D = B.getDataset(s.table),
-                            h = CB(o, E);
-                        D.initFilter(h)
+                        const i = B.getDataset(s.table),
+                            h = EB(o, E);
+                        i.initFilter(h)
                     })
                 });
                 continue
             }
             "updateInfos" in g && g.updateInfos.forEach(o => {
                 B.getDataset(o.table).initFilter(g.id)
             })
         }
     }
-    var OI = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+    var XI = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-    function Ks(A) {
+    function ls(A) {
         if (A.__esModule) return A;
         var B = A.default;
         if (typeof B == "function") {
             var g = function o() {
                 if (this instanceof o) {
                     var t = [null];
                     t.push.apply(t, arguments);
@@ -2542,178 +2585,178 @@
                 get: function() {
                     return A[o]
                 }
             })
         }), g
     }
     var Hg = {},
-        Ys = {
+        fs = {
             get exports() {
                 return Hg
             },
             set exports(A) {
                 Hg = A
             }
         };
-    const XI = Ks(Object.freeze(Object.defineProperty({
+    const vI = ls(Object.freeze(Object.defineProperty({
         __proto__: null,
         default: {}
     }, Symbol.toStringTag, {
         value: "Module"
     })));
     (function(A, B) {
         var g = void 0,
             o = function(t) {
                 return g || (g = new Promise(function(E, s) {
-                    var D = typeof t < "u" ? t : {},
-                        h = D.onAbort;
-                    D.onAbort = function(I) {
+                    var i = typeof t < "u" ? t : {},
+                        h = i.onAbort;
+                    i.onAbort = function(I) {
                         s(new Error(I)), h && h(I)
-                    }, D.postRun = D.postRun || [], D.postRun.push(function() {
-                        E(D)
+                    }, i.postRun = i.postRun || [], i.postRun.push(function() {
+                        E(i)
                     }), A = void 0;
                     var C;
-                    C || (C = typeof D < "u" ? D : {}), C.onRuntimeInitialized = function() {
+                    C || (C = typeof i < "u" ? i : {}), C.onRuntimeInitialized = function() {
                         function I(d, $) {
                             switch (typeof $) {
                                 case "boolean":
-                                    dw(d, $ ? 1 : 0);
+                                    qw(d, $ ? 1 : 0);
                                     break;
                                 case "number":
-                                    Hw(d, $);
+                                    dw(d, $);
                                     break;
                                 case "string":
-                                    lw(d, $, -1, -1);
+                                    uw(d, $, -1, -1);
                                     break;
                                 case "object":
-                                    if ($ === null) VB(d);
+                                    if ($ === null) mB(d);
                                     else if ($.length != null) {
                                         var DA = Xg($);
-                                        fw(d, DA, $.length, -1), Qg(DA)
-                                    } else Cg(d, "Wrong API use : tried to return a value of an unknown type (" + $ + ").", -1);
+                                        pw(d, DA, $.length, -1), Bg(DA)
+                                    } else Eg(d, "Wrong API use : tried to return a value of an unknown type (" + $ + ").", -1);
                                     break;
                                 default:
-                                    VB(d)
+                                    mB(d)
                             }
                         }
 
                         function Q(d, $) {
                             for (var DA = [], FA = 0; FA < d; FA += 1) {
                                 var yA = P($ + 4 * FA, "i32"),
-                                    cA = kw(yA);
-                                if (cA === 1 || cA === 2) yA = Yw(yA);
-                                else if (cA === 3) yA = Jw(yA);
+                                    cA = Kw(yA);
+                                if (cA === 1 || cA === 2) yA = fw(yA);
+                                else if (cA === 3) yA = Hw(yA);
                                 else if (cA === 4) {
-                                    cA = yA, yA = Sw(cA), cA = Kw(cA);
+                                    cA = yA, yA = Yw(cA), cA = lw(cA);
                                     for (var PA = new Uint8Array(yA), bA = 0; bA < yA; bA += 1) PA[bA] = W[cA + bA];
                                     yA = PA
                                 } else yA = null;
                                 DA.push(yA)
                             }
                             return DA
                         }
 
                         function w(d, $) {
                             this.La = d, this.db = $, this.Ja = 1, this.fb = []
                         }
 
                         function e(d, $) {
-                            if (this.db = $, $ = Z(d) + 1, this.Ya = gg($), this.Ya === null) throw Error("Unable to allocate memory for the SQL string");
+                            if (this.db = $, $ = Z(d) + 1, this.Ya = Qg($), this.Ya === null) throw Error("Unable to allocate memory for the SQL string");
                             F(d, tA, this.Ya, $), this.eb = this.Ya, this.Ua = this.ib = null
                         }
 
                         function S(d) {
                             if (this.filename = "dbfile_" + (4294967295 * Math.random() >>> 0), d != null) {
                                 var $ = this.filename,
                                     DA = "/",
                                     FA = $;
-                                if (DA && (DA = typeof DA == "string" ? DA : YI(DA), FA = $ ? EA(DA + "/" + $) : DA), $ = SB(!0, !0), FA = jI(FA, ($ !== void 0 ? $ : 438) & 4095 | 32768, 0), d) {
+                                if (DA && (DA = typeof DA == "string" ? DA : HI(DA), FA = $ ? EA(DA + "/" + $) : DA), $ = JB(!0, !0), FA = PI(FA, ($ !== void 0 ? $ : 438) & 4095 | 32768, 0), d) {
                                     if (typeof d == "string") {
                                         DA = Array(d.length);
                                         for (var yA = 0, cA = d.length; yA < cA; ++yA) DA[yA] = d.charCodeAt(yA);
                                         d = DA
                                     }
-                                    zI(FA, $ | 146), DA = eI(FA, 577), MB(DA, d, 0, d.length, 0), xg(DA), zI(FA, $)
+                                    _I(FA, $ | 146), DA = nI(FA, 577), LB(DA, d, 0, d.length, 0), xg(DA), _I(FA, $)
                                 }
                             }
-                            this.handleError(aA(this.filename, m)), this.db = P(m, "i32"), uw(this.db), this.Za = {}, this.Na = {}
+                            this.handleError(aA(this.filename, m)), this.db = P(m, "i32"), xw(this.db), this.Za = {}, this.Na = {}
                         }
                         var m = EI(4),
                             v = C.cwrap,
                             aA = v("sqlite3_open", "number", ["string", "number"]),
                             eA = v("sqlite3_close_v2", "number", ["number"]),
                             UA = v("sqlite3_exec", "number", ["number", "string", "number", "number", "number"]),
                             KA = v("sqlite3_changes", "number", ["number"]),
                             II = v("sqlite3_prepare_v2", "number", ["number", "string", "number", "number", "number"]),
-                            uB = v("sqlite3_sql", "string", ["number"]),
-                            sw = v("sqlite3_normalized_sql", "string", ["number"]),
-                            pB = v("sqlite3_prepare_v2", "number", ["number", "number", "number", "number", "number"]),
-                            ww = v("sqlite3_bind_text", "number", ["number", "number", "number", "number", "number"]),
-                            qB = v("sqlite3_bind_blob", "number", ["number", "number", "number", "number", "number"]),
-                            tw = v("sqlite3_bind_double", "number", ["number", "number", "number"]),
-                            hw = v("sqlite3_bind_int", "number", ["number", "number", "number"]),
-                            Fw = v("sqlite3_bind_parameter_index", "number", ["number", "string"]),
-                            aw = v("sqlite3_step", "number", ["number"]),
-                            Rw = v("sqlite3_errmsg", "string", ["number"]),
-                            yw = v("sqlite3_column_count", "number", ["number"]),
-                            Gw = v("sqlite3_data_count", "number", ["number"]),
-                            Uw = v("sqlite3_column_double", "number", ["number", "number"]),
-                            xB = v("sqlite3_column_text", "string", ["number", "number"]),
-                            nw = v("sqlite3_column_blob", "number", ["number", "number"]),
-                            ew = v("sqlite3_column_bytes", "number", ["number", "number"]),
-                            cw = v("sqlite3_column_type", "number", ["number", "number"]),
-                            Nw = v("sqlite3_column_name", "string", ["number", "number"]),
-                            rw = v("sqlite3_reset", "number", ["number"]),
-                            Mw = v("sqlite3_clear_bindings", "number", ["number"]),
-                            Lw = v("sqlite3_finalize", "number", ["number"]),
-                            bB = v("sqlite3_create_function_v2", "number", "number string number number number number number number number".split(" ")),
-                            kw = v("sqlite3_value_type", "number", ["number"]),
-                            Sw = v("sqlite3_value_bytes", "number", ["number"]),
-                            Jw = v("sqlite3_value_text", "string", ["number"]),
-                            Kw = v("sqlite3_value_blob", "number", ["number"]),
-                            Yw = v("sqlite3_value_double", "number", ["number"]),
-                            Hw = v("sqlite3_result_double", "", ["number", "number"]),
-                            VB = v("sqlite3_result_null", "", ["number"]),
-                            lw = v("sqlite3_result_text", "", ["number", "string", "number", "number"]),
-                            fw = v("sqlite3_result_blob", "", ["number", "number", "number", "number"]),
-                            dw = v("sqlite3_result_int", "", ["number", "number"]),
-                            Cg = v("sqlite3_result_error", "", ["number", "string", "number"]),
-                            mB = v("sqlite3_aggregate_context", "number", ["number", "number"]),
-                            uw = v("RegisterExtensionFunctions", "number", ["number"]);
+                            pB = v("sqlite3_sql", "string", ["number"]),
+                            hw = v("sqlite3_normalized_sql", "string", ["number"]),
+                            qB = v("sqlite3_prepare_v2", "number", ["number", "number", "number", "number", "number"]),
+                            Fw = v("sqlite3_bind_text", "number", ["number", "number", "number", "number", "number"]),
+                            xB = v("sqlite3_bind_blob", "number", ["number", "number", "number", "number", "number"]),
+                            aw = v("sqlite3_bind_double", "number", ["number", "number", "number"]),
+                            Rw = v("sqlite3_bind_int", "number", ["number", "number", "number"]),
+                            yw = v("sqlite3_bind_parameter_index", "number", ["number", "string"]),
+                            Gw = v("sqlite3_step", "number", ["number"]),
+                            Uw = v("sqlite3_errmsg", "string", ["number"]),
+                            nw = v("sqlite3_column_count", "number", ["number"]),
+                            ew = v("sqlite3_data_count", "number", ["number"]),
+                            cw = v("sqlite3_column_double", "number", ["number", "number"]),
+                            bB = v("sqlite3_column_text", "string", ["number", "number"]),
+                            Nw = v("sqlite3_column_blob", "number", ["number", "number"]),
+                            rw = v("sqlite3_column_bytes", "number", ["number", "number"]),
+                            Mw = v("sqlite3_column_type", "number", ["number", "number"]),
+                            Lw = v("sqlite3_column_name", "string", ["number", "number"]),
+                            kw = v("sqlite3_reset", "number", ["number"]),
+                            Sw = v("sqlite3_clear_bindings", "number", ["number"]),
+                            Jw = v("sqlite3_finalize", "number", ["number"]),
+                            VB = v("sqlite3_create_function_v2", "number", "number string number number number number number number number".split(" ")),
+                            Kw = v("sqlite3_value_type", "number", ["number"]),
+                            Yw = v("sqlite3_value_bytes", "number", ["number"]),
+                            Hw = v("sqlite3_value_text", "string", ["number"]),
+                            lw = v("sqlite3_value_blob", "number", ["number"]),
+                            fw = v("sqlite3_value_double", "number", ["number"]),
+                            dw = v("sqlite3_result_double", "", ["number", "number"]),
+                            mB = v("sqlite3_result_null", "", ["number"]),
+                            uw = v("sqlite3_result_text", "", ["number", "string", "number", "number"]),
+                            pw = v("sqlite3_result_blob", "", ["number", "number", "number", "number"]),
+                            qw = v("sqlite3_result_int", "", ["number", "number"]),
+                            Eg = v("sqlite3_result_error", "", ["number", "string", "number"]),
+                            ZB = v("sqlite3_aggregate_context", "number", ["number", "number"]),
+                            xw = v("RegisterExtensionFunctions", "number", ["number"]);
                         w.prototype.bind = function(d) {
                             if (!this.La) throw "Statement closed";
                             return this.reset(), Array.isArray(d) ? this.xb(d) : d != null && typeof d == "object" ? this.yb(d) : !0
                         }, w.prototype.step = function() {
                             if (!this.La) throw "Statement closed";
                             this.Ja = 1;
-                            var d = aw(this.La);
+                            var d = Gw(this.La);
                             switch (d) {
                                 case 100:
                                     return !0;
                                 case 101:
                                     return !1;
                                 default:
                                     throw this.db.handleError(d)
                             }
                         }, w.prototype.sb = function(d) {
-                            return d == null && (d = this.Ja, this.Ja += 1), Uw(this.La, d)
+                            return d == null && (d = this.Ja, this.Ja += 1), cw(this.La, d)
                         }, w.prototype.Cb = function(d) {
-                            if (d == null && (d = this.Ja, this.Ja += 1), d = xB(this.La, d), typeof BigInt != "function") throw Error("BigInt is not supported");
+                            if (d == null && (d = this.Ja, this.Ja += 1), d = bB(this.La, d), typeof BigInt != "function") throw Error("BigInt is not supported");
                             return BigInt(d)
                         }, w.prototype.Db = function(d) {
-                            return d == null && (d = this.Ja, this.Ja += 1), xB(this.La, d)
+                            return d == null && (d = this.Ja, this.Ja += 1), bB(this.La, d)
                         }, w.prototype.getBlob = function(d) {
                             d == null && (d = this.Ja, this.Ja += 1);
-                            var $ = ew(this.La, d);
-                            d = nw(this.La, d);
+                            var $ = rw(this.La, d);
+                            d = Nw(this.La, d);
                             for (var DA = new Uint8Array($), FA = 0; FA < $; FA += 1) DA[FA] = W[d + FA];
                             return DA
                         }, w.prototype.get = function(d, $) {
                             $ = $ || {}, d != null && this.bind(d) && this.step(), d = [];
-                            for (var DA = Gw(this.La), FA = 0; FA < DA; FA += 1) switch (cw(this.La, FA)) {
+                            for (var DA = ew(this.La), FA = 0; FA < DA; FA += 1) switch (Mw(this.La, FA)) {
                                 case 1:
                                     var yA = $.useBigInt ? this.Cb(FA) : this.sb(FA);
                                     d.push(yA);
                                     break;
                                 case 2:
                                     d.push(this.sb(FA));
                                     break;
@@ -2724,38 +2767,38 @@
                                     d.push(this.getBlob(FA));
                                     break;
                                 default:
                                     d.push(null)
                             }
                             return d
                         }, w.prototype.getColumnNames = function() {
-                            for (var d = [], $ = yw(this.La), DA = 0; DA < $; DA += 1) d.push(Nw(this.La, DA));
+                            for (var d = [], $ = nw(this.La), DA = 0; DA < $; DA += 1) d.push(Lw(this.La, DA));
                             return d
                         }, w.prototype.getAsObject = function(d, $) {
                             d = this.get(d, $), $ = this.getColumnNames();
                             for (var DA = {}, FA = 0; FA < $.length; FA += 1) DA[$[FA]] = d[FA];
                             return DA
                         }, w.prototype.getSQL = function() {
-                            return uB(this.La)
+                            return pB(this.La)
                         }, w.prototype.getNormalizedSQL = function() {
-                            return sw(this.La)
+                            return hw(this.La)
                         }, w.prototype.run = function(d) {
                             return d != null && this.bind(d), this.step(), this.reset()
                         }, w.prototype.nb = function(d, $) {
                             $ == null && ($ = this.Ja, this.Ja += 1), d = lA(d);
                             var DA = Xg(d);
-                            this.fb.push(DA), this.db.handleError(ww(this.La, $, DA, d.length - 1, 0))
+                            this.fb.push(DA), this.db.handleError(Fw(this.La, $, DA, d.length - 1, 0))
                         }, w.prototype.wb = function(d, $) {
                             $ == null && ($ = this.Ja, this.Ja += 1);
                             var DA = Xg(d);
-                            this.fb.push(DA), this.db.handleError(qB(this.La, $, DA, d.length, 0))
+                            this.fb.push(DA), this.db.handleError(xB(this.La, $, DA, d.length, 0))
                         }, w.prototype.mb = function(d, $) {
-                            $ == null && ($ = this.Ja, this.Ja += 1), this.db.handleError((d === (d | 0) ? hw : tw)(this.La, $, d))
+                            $ == null && ($ = this.Ja, this.Ja += 1), this.db.handleError((d === (d | 0) ? Rw : aw)(this.La, $, d))
                         }, w.prototype.zb = function(d) {
-                            d == null && (d = this.Ja, this.Ja += 1), qB(this.La, d, 0, 0, 0)
+                            d == null && (d = this.Ja, this.Ja += 1), xB(this.La, d, 0, 0, 0)
                         }, w.prototype.ob = function(d, $) {
                             switch ($ == null && ($ = this.Ja, this.Ja += 1), typeof d) {
                                 case "string":
                                     this.nb(d, $);
                                     return;
                                 case "number":
                                     this.mb(d, $);
@@ -2776,53 +2819,53 @@
                                         return
                                     }
                             }
                             throw "Wrong API use : tried to bind a value of an unknown type (" + d + ")."
                         }, w.prototype.yb = function(d) {
                             var $ = this;
                             return Object.keys(d).forEach(function(DA) {
-                                var FA = Fw($.La, DA);
+                                var FA = yw($.La, DA);
                                 FA !== 0 && $.ob(d[DA], FA)
                             }), !0
                         }, w.prototype.xb = function(d) {
                             for (var $ = 0; $ < d.length; $ += 1) this.ob(d[$], $ + 1);
                             return !0
                         }, w.prototype.reset = function() {
-                            return this.freemem(), Mw(this.La) === 0 && rw(this.La) === 0
+                            return this.freemem(), Sw(this.La) === 0 && kw(this.La) === 0
                         }, w.prototype.freemem = function() {
                             for (var d;
-                                (d = this.fb.pop()) !== void 0;) Qg(d)
+                                (d = this.fb.pop()) !== void 0;) Bg(d)
                         }, w.prototype.free = function() {
                             this.freemem();
-                            var d = Lw(this.La) === 0;
+                            var d = Jw(this.La) === 0;
                             return delete this.db.Za[this.La], this.La = 0, d
                         }, e.prototype.next = function() {
                             if (this.Ya === null) return {
                                 done: !0
                             };
                             if (this.Ua !== null && (this.Ua.free(), this.Ua = null), !this.db.db) throw this.gb(), Error("Database closed");
-                            var d = uI(),
+                            var d = pI(),
                                 $ = EI(4);
                             u(m), u($);
                             try {
-                                this.db.handleError(pB(this.db.db, this.eb, -1, m, $)), this.eb = P($, "i32");
+                                this.db.handleError(qB(this.db.db, this.eb, -1, m, $)), this.eb = P($, "i32");
                                 var DA = P(m, "i32");
                                 return DA === 0 ? (this.gb(), {
                                     done: !0
                                 }) : (this.Ua = new w(DA, this.db), this.db.Za[DA] = this.Ua, {
                                     value: this.Ua,
                                     done: !1
                                 })
                             } catch (FA) {
                                 throw this.ib = x(this.eb), this.gb(), FA
                             } finally {
-                                pI(d)
+                                qI(d)
                             }
                         }, e.prototype.gb = function() {
-                            Qg(this.Ya), this.Ya = null
+                            Bg(this.Ya), this.Ya = null
                         }, e.prototype.getRemainingSQL = function() {
                             return this.ib !== null ? this.ib : x(this.eb)
                         }, typeof Symbol == "function" && typeof Symbol.iterator == "symbol" && (e.prototype[Symbol.iterator] = function() {
                             return this
                         }), S.prototype.run = function(d, $) {
                             if (!this.db) throw "Database closed";
                             if ($) {
@@ -2832,38 +2875,38 @@
                                 } finally {
                                     d.free()
                                 }
                             } else this.handleError(UA(this.db, d, 0, 0, m));
                             return this
                         }, S.prototype.exec = function(d, $, DA) {
                             if (!this.db) throw "Database closed";
-                            var FA = uI(),
+                            var FA = pI(),
                                 yA = null;
                             try {
                                 var cA = Z(d) + 1,
                                     PA = EI(cA);
                                 F(d, W, PA, cA);
                                 var bA = PA,
                                     VA = EI(4);
                                 for (d = []; P(bA, "i8") !== 0;) {
-                                    u(m), u(VA), this.handleError(pB(this.db, bA, -1, m, VA));
+                                    u(m), u(VA), this.handleError(qB(this.db, bA, -1, m, VA));
                                     var mA = P(m, "i32");
                                     if (bA = P(VA, "i32"), mA !== 0) {
                                         for (cA = null, yA = new w(mA, this), $ != null && yA.bind($); yA.step();) cA === null && (cA = {
                                             columns: yA.getColumnNames(),
                                             values: []
                                         }, d.push(cA)), cA.values.push(yA.get(null, DA));
                                         yA.free()
                                     }
                                 }
                                 return d
-                            } catch (qI) {
-                                throw yA && yA.free(), qI
+                            } catch (xI) {
+                                throw yA && yA.free(), xI
                             } finally {
-                                pI(FA)
+                                qI(FA)
                             }
                         }, S.prototype.each = function(d, $, DA, FA, yA) {
                             typeof $ == "function" && (FA = DA, DA = $, $ = void 0), d = this.prepare(d, $);
                             try {
                                 for (; d.step();) DA(d.getAsObject(null, yA))
                             } finally {
                                 d.free()
@@ -2874,81 +2917,81 @@
                             var DA = new w(d, this);
                             return $ != null && DA.bind($), this.Za[d] = DA
                         }, S.prototype.iterateStatements = function(d) {
                             return new e(d, this)
                         }, S.prototype.export = function() {
                             Object.values(this.Za).forEach(function($) {
                                 $.free()
-                            }), Object.values(this.Na).forEach(dI), this.Na = {}, this.handleError(eA(this.db));
-                            var d = Ew(this.filename);
+                            }), Object.values(this.Na).forEach(uI), this.Na = {}, this.handleError(eA(this.db));
+                            var d = ow(this.filename);
                             return this.handleError(aA(this.filename, m)), this.db = P(m, "i32"), d
                         }, S.prototype.close = function() {
                             this.db !== null && (Object.values(this.Za).forEach(function(d) {
                                 d.free()
-                            }), Object.values(this.Na).forEach(dI), this.Na = {}, this.handleError(eA(this.db)), UB("/" + this.filename), this.db = null)
+                            }), Object.values(this.Na).forEach(uI), this.Na = {}, this.handleError(eA(this.db)), nB("/" + this.filename), this.db = null)
                         }, S.prototype.handleError = function(d) {
                             if (d === 0) return null;
-                            throw d = Rw(this.db), Error(d)
+                            throw d = Uw(this.db), Error(d)
                         }, S.prototype.getRowsModified = function() {
                             return KA(this.db)
                         }, S.prototype.create_function = function(d, $) {
-                            Object.prototype.hasOwnProperty.call(this.Na, d) && (dI(this.Na[d]), delete this.Na[d]);
+                            Object.prototype.hasOwnProperty.call(this.Na, d) && (uI(this.Na[d]), delete this.Na[d]);
                             var DA = Og(function(FA, yA, cA) {
                                 yA = Q(yA, cA);
                                 try {
                                     var PA = $.apply(null, yA)
                                 } catch (bA) {
-                                    Cg(FA, bA, -1);
+                                    Eg(FA, bA, -1);
                                     return
                                 }
                                 I(FA, PA)
                             }, "viii");
-                            return this.Na[d] = DA, this.handleError(bB(this.db, d, $.length, 1, 0, DA, 0, 0, 0)), this
+                            return this.Na[d] = DA, this.handleError(VB(this.db, d, $.length, 1, 0, DA, 0, 0, 0)), this
                         }, S.prototype.create_aggregate = function(d, $) {
                             var DA = $.init || function() {
                                     return null
                                 },
                                 FA = $.finalize || function(VA) {
                                     return VA
                                 },
                                 yA = $.step;
                             if (!yA) throw "An aggregate function must have a step function in " + d;
                             var cA = {};
-                            Object.hasOwnProperty.call(this.Na, d) && (dI(this.Na[d]), delete this.Na[d]), $ = d + "__finalize", Object.hasOwnProperty.call(this.Na, $) && (dI(this.Na[$]), delete this.Na[$]);
-                            var PA = Og(function(VA, mA, qI) {
-                                    var FI = mB(VA, 1);
-                                    Object.hasOwnProperty.call(cA, FI) || (cA[FI] = DA()), mA = Q(mA, qI), mA = [cA[FI]].concat(mA);
+                            Object.hasOwnProperty.call(this.Na, d) && (uI(this.Na[d]), delete this.Na[d]), $ = d + "__finalize", Object.hasOwnProperty.call(this.Na, $) && (uI(this.Na[$]), delete this.Na[$]);
+                            var PA = Og(function(VA, mA, xI) {
+                                    var FI = ZB(VA, 1);
+                                    Object.hasOwnProperty.call(cA, FI) || (cA[FI] = DA()), mA = Q(mA, xI), mA = [cA[FI]].concat(mA);
                                     try {
                                         cA[FI] = yA.apply(null, mA)
-                                    } catch (pw) {
-                                        delete cA[FI], Cg(VA, pw, -1)
+                                    } catch (bw) {
+                                        delete cA[FI], Eg(VA, bw, -1)
                                     }
                                 }, "viii"),
                                 bA = Og(function(VA) {
-                                    var mA = mB(VA, 1);
+                                    var mA = ZB(VA, 1);
                                     try {
-                                        var qI = FA(cA[mA])
+                                        var xI = FA(cA[mA])
                                     } catch (FI) {
-                                        delete cA[mA], Cg(VA, FI, -1);
+                                        delete cA[mA], Eg(VA, FI, -1);
                                         return
                                     }
-                                    I(VA, qI), delete cA[mA]
+                                    I(VA, xI), delete cA[mA]
                                 }, "vi");
-                            return this.Na[d] = PA, this.Na[$] = bA, this.handleError(bB(this.db, d, yA.length - 1, 1, 0, 0, PA, bA, 0)), this
+                            return this.Na[d] = PA, this.Na[$] = bA, this.handleError(VB(this.db, d, yA.length - 1, 1, 0, 0, PA, bA, 0)), this
                         }, C.Database = S
                     };
                     var r = Object.assign({}, C),
                         n = "./this.program",
                         M = typeof window == "object",
                         R = typeof importScripts == "function",
                         N = typeof process == "object" && typeof process.versions == "object" && typeof process.versions.node == "string",
                         a = "",
                         G, y, c, k, H, l;
-                    N ? (a = R ? XI.dirname(a) + "/" : __dirname + "/", l = () => {
-                        H || (k = XI, H = XI)
+                    N ? (a = R ? vI.dirname(a) + "/" : __dirname + "/", l = () => {
+                        H || (k = vI, H = vI)
                     }, G = function(I, Q) {
                         return l(), I = H.normalize(I), k.readFileSync(I, Q ? void 0 : "utf8")
                     }, c = I => (I = G(I, !0), I.buffer || (I = new Uint8Array(I)), I), y = (I, Q, w) => {
                         l(), I = H.normalize(I), k.readFile(I, function(e, S) {
                             e ? w(e) : Q(S.buffer)
                         })
                     }, 1 < process.argv.length && (n = process.argv[1].replace(/\\/g, "/")), process.argv.slice(2), A.exports = C, C.inspect = function() {
@@ -3053,45 +3096,45 @@
                         rA = null;
 
                     function HA(I) {
                         throw C.onAbort && C.onAbort(I), I = "Aborted(" + I + ")", p(I), gA = !0, new WebAssembly.RuntimeError(I + ". Build with -sASSERTIONS for more info.")
                     }
 
                     function dA() {
-                        return i.startsWith("data:application/octet-stream;base64,")
+                        return D.startsWith("data:application/octet-stream;base64,")
                     }
-                    var i;
-                    if (i = "sql-wasm.wasm", !dA()) {
-                        var X = i;
-                        i = C.locateFile ? C.locateFile(X, a) : a + X
+                    var D;
+                    if (D = "sql-wasm.wasm", !dA()) {
+                        var X = D;
+                        D = C.locateFile ? C.locateFile(X, a) : a + X
                     }
 
                     function V() {
-                        var I = i;
+                        var I = D;
                         try {
-                            if (I == i && j) return new Uint8Array(j);
+                            if (I == D && j) return new Uint8Array(j);
                             if (c) return c(I);
                             throw "both async and sync fetching of the wasm failed"
                         } catch (Q) {
                             HA(Q)
                         }
                     }
 
                     function L() {
                         if (!j && (M || R)) {
-                            if (typeof fetch == "function" && !i.startsWith("file://")) return fetch(i, {
+                            if (typeof fetch == "function" && !D.startsWith("file://")) return fetch(D, {
                                 credentials: "same-origin"
                             }).then(function(I) {
-                                if (!I.ok) throw "failed to load wasm binary file at '" + i + "'";
+                                if (!I.ok) throw "failed to load wasm binary file at '" + D + "'";
                                 return I.arrayBuffer()
                             }).catch(function() {
                                 return V()
                             });
                             if (y) return new Promise(function(I, Q) {
-                                y(i, function(w) {
+                                y(D, function(w) {
                                     I(new Uint8Array(w))
                                 }, Q)
                             })
                         }
                         return Promise.resolve().then(function() {
                             return V()
                         })
@@ -3184,15 +3227,15 @@
 
                     function NA() {
                         if (typeof crypto == "object" && typeof crypto.getRandomValues == "function") {
                             var I = new Uint8Array(1);
                             return () => (crypto.getRandomValues(I), I[0])
                         }
                         if (N) try {
-                            var Q = XI;
+                            var Q = vI;
                             return () => Q.randomBytes(1)[0]
                         } catch {}
                         return () => HA("randomDevice")
                     }
 
                     function RA() {
                         for (var I = "", Q = !1, w = arguments.length - 1; - 1 <= w && !Q; w--) {
@@ -3277,15 +3320,15 @@
                             jb: function(I, Q) {
                                 Q === null || Q === 10 ? (T(J(I.output, 0)), I.output = []) : Q != 0 && I.output.push(Q)
                             },
                             fsync: function(I) {
                                 I.output && 0 < I.output.length && (T(J(I.output, 0)), I.output = [])
                             }
                         },
-                        UI = {
+                        GI = {
                             jb: function(I, Q) {
                                 Q === null || Q === 10 ? (p(J(I.output, 0)), I.output = []) : Q != 0 && I.output.push(Q)
                             },
                             fsync: function(I) {
                                 I.output && 0 < I.output.length && (p(J(I.output, 0)), I.output = [])
                             }
                         },
@@ -3336,17 +3379,17 @@
                                         stream: {}
                                     },
                                     pb: {
                                         node: {
                                             Pa: hA.Ga.Pa,
                                             Oa: hA.Ga.Oa
                                         },
-                                        stream: Cw
+                                        stream: Dw
                                     }
-                                }), w = tB(I, Q, w, e), (w.mode & 61440) === 16384 ? (w.Ga = hA.Qa.dir.node, w.Ha = hA.Qa.dir.stream, w.Ia = {}) : (w.mode & 61440) === 32768 ? (w.Ga = hA.Qa.file.node, w.Ha = hA.Qa.file.stream, w.Ma = 0, w.Ia = null) : (w.mode & 61440) === 40960 ? (w.Ga = hA.Qa.link.node, w.Ha = hA.Qa.link.stream) : (w.mode & 61440) === 8192 && (w.Ga = hA.Qa.pb.node, w.Ha = hA.Qa.pb.stream), w.timestamp = Date.now(), I && (I.Ia[Q] = w, I.timestamp = w.timestamp), w
+                                }), w = hB(I, Q, w, e), (w.mode & 61440) === 16384 ? (w.Ga = hA.Qa.dir.node, w.Ha = hA.Qa.dir.stream, w.Ia = {}) : (w.mode & 61440) === 32768 ? (w.Ga = hA.Qa.file.node, w.Ha = hA.Qa.file.stream, w.Ma = 0, w.Ia = null) : (w.mode & 61440) === 40960 ? (w.Ga = hA.Qa.link.node, w.Ha = hA.Qa.link.stream) : (w.mode & 61440) === 8192 && (w.Ga = hA.Qa.pb.node, w.Ha = hA.Qa.pb.stream), w.timestamp = Date.now(), I && (I.Ia[Q] = w, I.timestamp = w.timestamp), w
                             },
                             Jb: function(I) {
                                 return I.Ia ? I.Ia.subarray ? I.Ia.subarray(0, I.Ma) : new Uint8Array(I.Ia) : new Uint8Array(0)
                             },
                             qb: function(I, Q) {
                                 var w = I.Ia ? I.Ia.length : 0;
                                 w >= Q || (Q = Math.max(Q, w * (1048576 > w ? 2 : 1.125) >>> 0), w != 0 && (Q = Math.max(Q, 256)), w = I.Ia, I.Ia = new Uint8Array(Q), 0 < I.Ma && I.Ia.set(w.subarray(0, I.Ma), 0))
@@ -3433,34 +3476,34 @@
                                 },
                                 lb: function(I, Q, w) {
                                     hA.qb(I.node, Q + w), I.node.Ma = Math.max(I.node.Ma, Q + w)
                                 },
                                 bb: function(I, Q, w, e, S) {
                                     if ((I.node.mode & 61440) !== 32768) throw new O(43);
                                     if (I = I.node.Ia, S & 2 || I.buffer !== iA) {
-                                        if ((0 < w || w + Q < I.length) && (I.subarray ? I = I.subarray(w, w + Q) : I = Array.prototype.slice.call(I, w, w + Q)), w = !0, Q = 65536 * Math.ceil(Q / 65536), (S = fB(65536, Q)) ? (tA.fill(0, S, S + Q), Q = S) : Q = 0, !Q) throw new O(48);
+                                        if ((0 < w || w + Q < I.length) && (I.subarray ? I = I.subarray(w, w + Q) : I = Array.prototype.slice.call(I, w, w + Q)), w = !0, Q = 65536 * Math.ceil(Q / 65536), (S = dB(65536, Q)) ? (tA.fill(0, S, S + Q), Q = S) : Q = 0, !Q) throw new O(48);
                                         W.set(I, Q)
                                     } else w = !1, Q = I.byteOffset;
                                     return {
                                         Fb: Q,
                                         vb: w
                                     }
                                 },
                                 cb: function(I, Q, w, e, S) {
                                     if ((I.node.mode & 61440) !== 32768) throw new O(43);
                                     return S & 2 || hA.Ha.write(I, Q, 0, e, w, !1), 0
                                 }
                             }
                         },
                         xA = null,
-                        JI = {},
+                        KI = {},
                         XA = [],
                         dg = 1,
                         vA = null,
-                        KI = !0,
+                        YI = !0,
                         O = null,
                         BI = {},
                         uA = (I, Q = {}) => {
                             if (I = RA("/", I), !I) return {
                                 path: "",
                                 node: null
                             };
@@ -3471,102 +3514,102 @@
                             I = IA(I.split("/").filter(v => !!v), !1);
                             for (var w = xA, e = "/", S = 0; S < I.length; S++) {
                                 var m = S === I.length - 1;
                                 if (m && Q.parent) break;
                                 if (w = tI(w, I[S]), e = EA(e + "/" + I[S]), w.Va && (!m || m && Q.rb) && (w = w.Va.root), !m || Q.Sa) {
                                     for (m = 0;
                                         (w.mode & 61440) === 40960;)
-                                        if (w = nB(e), e = RA(BA(e), w), w = uA(e, {
+                                        if (w = eB(e), e = RA(BA(e), w), w = uA(e, {
                                                 kb: Q.kb + 1
                                             }).node, 40 < m++) throw new O(32)
                                 }
                             }
                             return {
                                 path: e,
                                 node: w
                             }
                         },
-                        YI = I => {
+                        HI = I => {
                             for (var Q;;) {
                                 if (I === I.parent) return I = I.Ra.ub, Q ? I[I.length - 1] !== "/" ? I + "/" + Q : I + Q : I;
                                 Q = Q ? I.name + "/" + Q : I.name, I = I.parent
                             }
                         },
                         ug = (I, Q) => {
                             for (var w = 0, e = 0; e < Q.length; e++) w = (w << 5) - w + Q.charCodeAt(e) | 0;
                             return (I + w >>> 0) % vA.length
                         },
-                        wB = I => {
+                        tB = I => {
                             var Q = ug(I.parent.id, I.name);
                             if (vA[Q] === I) vA[Q] = I.Wa;
                             else
                                 for (Q = vA[Q]; Q;) {
                                     if (Q.Wa === I) {
                                         Q.Wa = I.Wa;
                                         break
                                     }
                                     Q = Q.Wa
                                 }
                         },
                         tI = (I, Q) => {
                             var w;
-                            if (w = (w = nI(I, "x")) ? w : I.Ga.lookup ? 0 : 2) throw new O(w, I);
+                            if (w = (w = UI(I, "x")) ? w : I.Ga.lookup ? 0 : 2) throw new O(w, I);
                             for (w = vA[ug(I.id, Q)]; w; w = w.Wa) {
                                 var e = w.name;
                                 if (w.parent.id === I.id && e === Q) return w
                             }
                             return I.Ga.lookup(I, Q)
                         },
-                        tB = (I, Q, w, e) => (I = new HB(I, Q, w, e), Q = ug(I.parent.id, I.name), I.Wa = vA[Q], vA[Q] = I),
-                        Qw = {
+                        hB = (I, Q, w, e) => (I = new lB(I, Q, w, e), Q = ug(I.parent.id, I.name), I.Wa = vA[Q], vA[Q] = I),
+                        Ew = {
                             r: 0,
                             "r+": 2,
                             w: 577,
                             "w+": 578,
                             a: 1089,
                             "a+": 1090
                         },
-                        hB = I => {
+                        FB = I => {
                             var Q = ["r", "w", "rw"][I & 3];
                             return I & 512 && (Q += "w"), Q
                         },
-                        nI = (I, Q) => {
-                            if (KI) return 0;
+                        UI = (I, Q) => {
+                            if (YI) return 0;
                             if (!Q.includes("r") || I.mode & 292) {
                                 if (Q.includes("w") && !(I.mode & 146) || Q.includes("x") && !(I.mode & 73)) return 2
                             } else return 2;
                             return 0
                         },
-                        FB = (I, Q) => {
+                        aB = (I, Q) => {
                             try {
                                 return tI(I, Q), 20
                             } catch {}
-                            return nI(I, "wx")
+                            return UI(I, "wx")
                         },
-                        aB = (I, Q, w) => {
+                        RB = (I, Q, w) => {
                             try {
                                 var e = tI(I, Q)
                             } catch (S) {
                                 return S.Ka
                             }
-                            if (I = nI(I, "wx")) return I;
+                            if (I = UI(I, "wx")) return I;
                             if (w) {
                                 if ((e.mode & 61440) !== 16384) return 54;
-                                if (e === e.parent || YI(e) === "/") return 10
+                                if (e === e.parent || HI(e) === "/") return 10
                             } else if ((e.mode & 61440) === 16384) return 31;
                             return 0
                         },
-                        Bw = (I = 0) => {
+                        iw = (I = 0) => {
                             for (; 4096 >= I; I++)
                                 if (!XA[I]) return I;
                             throw new O(33)
                         },
-                        RB = (I, Q) => (fI || (fI = function() {
+                        yB = (I, Q) => (dI || (dI = function() {
                             this.$a = {}
-                        }, fI.prototype = {}, Object.defineProperties(fI.prototype, {
+                        }, dI.prototype = {}, Object.defineProperties(dI.prototype, {
                             object: {
                                 get: function() {
                                     return this.node
                                 },
                                 set: function(w) {
                                     this.node = w
                                 }
@@ -3583,29 +3626,29 @@
                                 get: function() {
                                     return this.$a.position
                                 },
                                 set: function(w) {
                                     this.$a.position = w
                                 }
                             }
-                        })), I = Object.assign(new fI, I), Q = Bw(Q), I.fd = Q, XA[Q] = I),
-                        Cw = {
+                        })), I = Object.assign(new dI, I), Q = iw(Q), I.fd = Q, XA[Q] = I),
+                        Dw = {
                             open: I => {
-                                I.Ha = JI[I.node.rdev].Ha, I.Ha.open && I.Ha.open(I)
+                                I.Ha = KI[I.node.rdev].Ha, I.Ha.open && I.Ha.open(I)
                             },
                             Ta: () => {
                                 throw new O(70)
                             }
                         },
                         pg = (I, Q) => {
-                            JI[I] = {
+                            KI[I] = {
                                 Ha: Q
                             }
                         },
-                        yB = (I, Q) => {
+                        GB = (I, Q) => {
                             var w = Q === "/",
                                 e = !Q;
                             if (w && xA) throw new O(10);
                             if (!w && !e) {
                                 var S = uA(Q, {
                                     rb: !1
                                 });
@@ -3615,105 +3658,105 @@
                             Q = {
                                 type: I,
                                 Kb: {},
                                 ub: Q,
                                 Eb: []
                             }, I = I.Ra(Q), I.Ra = Q, Q.root = I, w ? xA = I : S && (S.Va = Q, S.Ra && S.Ra.Eb.push(Q))
                         },
-                        jI = (I, Q, w) => {
+                        PI = (I, Q, w) => {
                             var e = uA(I, {
                                 parent: !0
                             }).node;
                             if (I = wA(I), !I || I === "." || I === "..") throw new O(28);
-                            var S = FB(e, I);
+                            var S = aB(e, I);
                             if (S) throw new O(S);
                             if (!e.Ga.ab) throw new O(63);
                             return e.Ga.ab(e, I, Q, w)
                         },
-                        jA = (I, Q) => jI(I, (Q !== void 0 ? Q : 511) & 1023 | 16384, 0),
-                        PI = (I, Q, w) => {
-                            typeof w > "u" && (w = Q, Q = 438), jI(I, Q | 8192, w)
+                        jA = (I, Q) => PI(I, (Q !== void 0 ? Q : 511) & 1023 | 16384, 0),
+                        zI = (I, Q, w) => {
+                            typeof w > "u" && (w = Q, Q = 438), PI(I, Q | 8192, w)
                         },
                         qg = (I, Q) => {
                             if (!RA(I)) throw new O(44);
                             var w = uA(Q, {
                                 parent: !0
                             }).node;
                             if (!w) throw new O(44);
                             Q = wA(Q);
-                            var e = FB(w, Q);
+                            var e = aB(w, Q);
                             if (e) throw new O(e);
                             if (!w.Ga.symlink) throw new O(63);
                             w.Ga.symlink(w, Q, I)
                         },
-                        GB = I => {
+                        UB = I => {
                             var Q = uA(I, {
                                 parent: !0
                             }).node;
                             I = wA(I);
                             var w = tI(Q, I),
-                                e = aB(Q, I, !0);
+                                e = RB(Q, I, !0);
                             if (e) throw new O(e);
                             if (!Q.Ga.rmdir) throw new O(63);
                             if (w.Va) throw new O(10);
-                            Q.Ga.rmdir(Q, I), wB(w)
+                            Q.Ga.rmdir(Q, I), tB(w)
                         },
-                        UB = I => {
+                        nB = I => {
                             var Q = uA(I, {
                                 parent: !0
                             }).node;
                             if (!Q) throw new O(44);
                             I = wA(I);
                             var w = tI(Q, I),
-                                e = aB(Q, I, !1);
+                                e = RB(Q, I, !1);
                             if (e) throw new O(e);
                             if (!Q.Ga.unlink) throw new O(63);
                             if (w.Va) throw new O(10);
-                            Q.Ga.unlink(Q, I), wB(w)
+                            Q.Ga.unlink(Q, I), tB(w)
                         },
-                        nB = I => {
+                        eB = I => {
                             if (I = uA(I).node, !I) throw new O(44);
                             if (!I.Ga.readlink) throw new O(28);
-                            return RA(YI(I.parent), I.Ga.readlink(I))
+                            return RA(HI(I.parent), I.Ga.readlink(I))
                         },
-                        HI = (I, Q) => {
+                        lI = (I, Q) => {
                             if (I = uA(I, {
                                     Sa: !Q
                                 }).node, !I) throw new O(44);
                             if (!I.Ga.Pa) throw new O(63);
                             return I.Ga.Pa(I)
                         },
-                        eB = I => HI(I, !0),
-                        zI = (I, Q) => {
+                        cB = I => lI(I, !0),
+                        _I = (I, Q) => {
                             if (I = typeof I == "string" ? uA(I, {
                                     Sa: !0
                                 }).node : I, !I.Ga.Oa) throw new O(63);
                             I.Ga.Oa(I, {
                                 mode: Q & 4095 | I.mode & -4096,
                                 timestamp: Date.now()
                             })
                         },
-                        cB = (I, Q) => {
+                        NB = (I, Q) => {
                             if (0 > Q) throw new O(28);
                             if (I = typeof I == "string" ? uA(I, {
                                     Sa: !0
                                 }).node : I, !I.Ga.Oa) throw new O(63);
                             if ((I.mode & 61440) === 16384) throw new O(31);
                             if ((I.mode & 61440) !== 32768) throw new O(28);
-                            var w = nI(I, "w");
+                            var w = UI(I, "w");
                             if (w) throw new O(w);
                             I.Ga.Oa(I, {
                                 size: Q,
                                 timestamp: Date.now()
                             })
                         },
-                        eI = (I, Q, w) => {
+                        nI = (I, Q, w) => {
                             if (I === "") throw new O(44);
                             if (typeof Q == "string") {
-                                var e = Qw[Q];
+                                var e = Ew[Q];
                                 if (typeof e > "u") throw Error("Unknown file open mode: " + Q);
                                 Q = e
                             }
                             if (w = Q & 64 ? (typeof w > "u" ? 438 : w) & 4095 | 32768 : 0, typeof I == "object") var S = I;
                             else {
                                 I = EA(I);
                                 try {
@@ -3721,92 +3764,92 @@
                                         Sa: !(Q & 131072)
                                     }).node
                                 } catch {}
                             }
                             if (e = !1, Q & 64)
                                 if (S) {
                                     if (Q & 128) throw new O(20)
-                                } else S = jI(I, w, 0), e = !0;
+                                } else S = PI(I, w, 0), e = !0;
                             if (!S) throw new O(44);
                             if ((S.mode & 61440) === 8192 && (Q &= -513), Q & 65536 && (S.mode & 61440) !== 16384) throw new O(54);
-                            if (!e && (w = S ? (S.mode & 61440) === 40960 ? 32 : (S.mode & 61440) === 16384 && (hB(Q) !== "r" || Q & 512) ? 31 : nI(S, hB(Q)) : 44)) throw new O(w);
-                            return Q & 512 && !e && cB(S, 0), Q &= -131713, S = RB({
+                            if (!e && (w = S ? (S.mode & 61440) === 40960 ? 32 : (S.mode & 61440) === 16384 && (FB(Q) !== "r" || Q & 512) ? 31 : UI(S, FB(Q)) : 44)) throw new O(w);
+                            return Q & 512 && !e && NB(S, 0), Q &= -131713, S = yB({
                                 node: S,
-                                path: YI(S),
+                                path: HI(S),
                                 flags: Q,
                                 seekable: !0,
                                 position: 0,
                                 Ha: S.Ha,
                                 Ib: [],
                                 error: !1
-                            }), S.Ha.open && S.Ha.open(S), !C.logReadFiles || Q & 1 || (_I || (_I = {}), I in _I || (_I[I] = 1)), S
+                            }), S.Ha.open && S.Ha.open(S), !C.logReadFiles || Q & 1 || ($I || ($I = {}), I in $I || ($I[I] = 1)), S
                         },
                         xg = I => {
                             if (I.fd === null) throw new O(8);
                             I.hb && (I.hb = null);
                             try {
                                 I.Ha.close && I.Ha.close(I)
                             } catch (Q) {
                                 throw Q
                             } finally {
                                 XA[I.fd] = null
                             }
                             I.fd = null
                         },
-                        NB = (I, Q, w) => {
+                        rB = (I, Q, w) => {
                             if (I.fd === null) throw new O(8);
                             if (!I.seekable || !I.Ha.Ta) throw new O(70);
                             if (w != 0 && w != 1 && w != 2) throw new O(28);
                             I.position = I.Ha.Ta(I, Q, w), I.Ib = []
                         },
-                        rB = (I, Q, w, e, S) => {
+                        MB = (I, Q, w, e, S) => {
                             if (0 > e || 0 > S) throw new O(28);
                             if (I.fd === null) throw new O(8);
                             if ((I.flags & 2097155) === 1) throw new O(8);
                             if ((I.node.mode & 61440) === 16384) throw new O(31);
                             if (!I.Ha.read) throw new O(28);
                             var m = typeof S < "u";
                             if (!m) S = I.position;
                             else if (!I.seekable) throw new O(70);
                             return Q = I.Ha.read(I, Q, w, e, S), m || (I.position += Q), Q
                         },
-                        MB = (I, Q, w, e, S) => {
+                        LB = (I, Q, w, e, S) => {
                             if (0 > e || 0 > S) throw new O(28);
                             if (I.fd === null) throw new O(8);
                             if (!(I.flags & 2097155)) throw new O(8);
                             if ((I.node.mode & 61440) === 16384) throw new O(31);
                             if (!I.Ha.write) throw new O(28);
-                            I.seekable && I.flags & 1024 && NB(I, 0, 2);
+                            I.seekable && I.flags & 1024 && rB(I, 0, 2);
                             var m = typeof S < "u";
                             if (!m) S = I.position;
                             else if (!I.seekable) throw new O(70);
                             return Q = I.Ha.write(I, Q, w, e, S, void 0), m || (I.position += Q), Q
                         },
-                        Ew = I => {
-                            var Q, w = eI(I, w || 0);
-                            I = HI(I).size;
+                        ow = I => {
+                            var Q, w = nI(I, w || 0);
+                            I = lI(I).size;
                             var e = new Uint8Array(I);
-                            return rB(w, e, 0, I, 0), Q = e, xg(w), Q
+                            return MB(w, e, 0, I, 0), Q = e, xg(w), Q
                         },
-                        LB = () => {
+                        kB = () => {
                             O || (O = function(I, Q) {
                                 this.node = Q, this.Hb = function(w) {
                                     this.Ka = w
                                 }, this.Hb(I), this.message = "FS error"
                             }, O.prototype = Error(), O.prototype.constructor = O, [44].forEach(I => {
                                 BI[I] = new O(I), BI[I].stack = "<generic error, no stack>"
                             }))
                         },
-                        kB, SB = (I, Q) => {
+                        SB, JB = (I, Q) => {
                             var w = 0;
                             return I && (w |= 365), Q && (w |= 146), w
                         },
-                        lI = (I, Q, w) => {
+                        fI = (I, Q, w) => {
                             I = EA("/dev/" + I);
-                            var e = SB(!!Q, !!w);
+                            var e = JB(!!Q, !!w);
                             bg || (bg = 64);
                             var S = bg++ << 8 | 0;
                             pg(S, {
                                 open: m => {
                                     m.seekable = !1
                                 },
                                 close: () => {
@@ -3829,81 +3872,81 @@
                                     for (var UA = 0; UA < eA; UA++) try {
                                         w(v[aA + UA])
                                     } catch {
                                         throw new O(29)
                                     }
                                     return eA && (m.node.timestamp = Date.now()), UA
                                 }
-                            }), PI(I, e, S)
+                            }), zI(I, e, S)
                         },
                         bg, kA = {},
-                        fI, _I;
+                        dI, $I;
 
                     function hI(I, Q, w) {
                         if (Q.charAt(0) === "/") return Q;
                         if (I = I === -100 ? "/" : TA(I).path, Q.length == 0) {
                             if (!w) throw new O(44);
                             return I
                         }
                         return EA(I + "/" + Q)
                     }
 
-                    function $I(I, Q, w) {
+                    function Ag(I, Q, w) {
                         try {
                             var e = I(Q)
                         } catch (S) {
-                            if (S && S.node && EA(Q) !== EA(YI(S.node))) return -54;
+                            if (S && S.node && EA(Q) !== EA(HI(S.node))) return -54;
                             throw S
                         }
                         return AA[w >> 2] = e.dev, AA[w + 8 >> 2] = e.ino, AA[w + 12 >> 2] = e.mode, f[w + 16 >> 2] = e.nlink, AA[w + 20 >> 2] = e.uid, AA[w + 24 >> 2] = e.gid, AA[w + 28 >> 2] = e.rdev, Y = [e.size >>> 0, (U = e.size, 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[w + 40 >> 2] = Y[0], AA[w + 44 >> 2] = Y[1], AA[w + 48 >> 2] = 4096, AA[w + 52 >> 2] = e.blocks, Y = [Math.floor(e.atime.getTime() / 1e3) >>> 0, (U = Math.floor(e.atime.getTime() / 1e3), 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[w + 56 >> 2] = Y[0], AA[w + 60 >> 2] = Y[1], f[w + 64 >> 2] = 0, Y = [Math.floor(e.mtime.getTime() / 1e3) >>> 0, (U = Math.floor(e.mtime.getTime() / 1e3), 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[w + 72 >> 2] = Y[0], AA[w + 76 >> 2] = Y[1], f[w + 80 >> 2] = 0, Y = [Math.floor(e.ctime.getTime() / 1e3) >>> 0, (U = Math.floor(e.ctime.getTime() / 1e3), 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[w + 88 >> 2] = Y[0], AA[w + 92 >> 2] = Y[1], f[w + 96 >> 2] = 0, Y = [e.ino >>> 0, (U = e.ino, 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[w + 104 >> 2] = Y[0], AA[w + 108 >> 2] = Y[1], 0
                     }
-                    var Ag = void 0;
+                    var Ig = void 0;
 
-                    function Ig() {
-                        return Ag += 4, AA[Ag - 4 >> 2]
+                    function gg() {
+                        return Ig += 4, AA[Ig - 4 >> 2]
                     }
 
                     function TA(I) {
                         if (I = XA[I], !I) throw new O(8);
                         return I
                     }
 
                     function Vg(I) {
                         return f[I >> 2] + 4294967296 * AA[I + 4 >> 2]
                     }
 
-                    function JB(I) {
+                    function KB(I) {
                         var Q = Z(I) + 1,
-                            w = gg(Q);
+                            w = Qg(Q);
                         return w && F(I, W, w, Q), w
                     }
 
-                    function iw(I, Q, w) {
+                    function sw(I, Q, w) {
                         function e(eA) {
                             return (eA = eA.toTimeString().match(/\(([A-Za-z ]+)\)$/)) ? eA[1] : "GMT"
                         }
                         var S = new Date().getFullYear(),
                             m = new Date(S, 0, 1),
                             v = new Date(S, 6, 1);
                         S = m.getTimezoneOffset();
                         var aA = v.getTimezoneOffset();
-                        AA[I >> 2] = 60 * Math.max(S, aA), AA[Q >> 2] = +(S != aA), I = e(m), Q = e(v), I = JB(I), Q = JB(Q), aA < S ? (f[w >> 2] = I, f[w + 4 >> 2] = Q) : (f[w >> 2] = Q, f[w + 4 >> 2] = I)
+                        AA[I >> 2] = 60 * Math.max(S, aA), AA[Q >> 2] = +(S != aA), I = e(m), Q = e(v), I = KB(I), Q = KB(Q), aA < S ? (f[w >> 2] = I, f[w + 4 >> 2] = Q) : (f[w >> 2] = Q, f[w + 4 >> 2] = I)
                     }
 
                     function mg(I, Q, w) {
-                        mg.Bb || (mg.Bb = !0, iw(I, Q, w))
+                        mg.Bb || (mg.Bb = !0, sw(I, Q, w))
                     }
-                    var KB;
-                    KB = N ? () => {
+                    var YB;
+                    YB = N ? () => {
                         var I = process.hrtime();
                         return 1e3 * I[0] + I[1] / 1e6
                     } : () => performance.now();
                     var Zg = {};
 
-                    function YB() {
+                    function HB() {
                         if (!Tg) {
                             var I = {
                                     USER: "web_user",
                                     LOGNAME: "web_user",
                                     PATH: "/",
                                     PWD: "/",
                                     HOME: "/home/web_user",
@@ -3973,24 +4016,24 @@
                                 }).exports.f
                             }
                             QA.set(w, Q)
                         }
                         return CI.set(I, w), w
                     }
 
-                    function dI(I) {
+                    function uI(I) {
                         CI.delete(QA.get(I)), Wg.push(I)
                     }
 
                     function Xg(I) {
-                        var Q = gg(I.length);
+                        var Q = Qg(I.length);
                         return I.subarray || I.slice || (I = new Uint8Array(I)), tA.set(I, Q), Q
                     }
 
-                    function Dw(I, Q, w, e) {
+                    function ww(I, Q, w, e) {
                         var S = {
                             string: UA => {
                                 var KA = 0;
                                 if (UA != null && UA !== 0) {
                                     var II = (UA.length << 2) + 1;
                                     KA = EI(II), F(UA, tA, KA, II)
                                 }
@@ -4003,25 +4046,25 @@
                         };
                         I = C["_" + I];
                         var m = [],
                             v = 0;
                         if (e)
                             for (var aA = 0; aA < e.length; aA++) {
                                 var eA = S[w[aA]];
-                                eA ? (v === 0 && (v = uI()), m[aA] = eA(e[aA])) : m[aA] = e[aA]
+                                eA ? (v === 0 && (v = pI()), m[aA] = eA(e[aA])) : m[aA] = e[aA]
                             }
                         return w = I.apply(null, m), w = function(UA) {
-                            return v !== 0 && pI(v), Q === "string" ? x(UA) : Q === "boolean" ? !!UA : UA
+                            return v !== 0 && qI(v), Q === "string" ? x(UA) : Q === "boolean" ? !!UA : UA
                         }(w)
                     }
 
-                    function HB(I, Q, w, e) {
+                    function lB(I, Q, w, e) {
                         I || (I = this), this.parent = I, this.Ra = I.Ra, this.Va = null, this.id = dg++, this.name = Q, this.mode = w, this.Ga = {}, this.Ha = {}, this.rdev = e
                     }
-                    Object.defineProperties(HB.prototype, {
+                    Object.defineProperties(lB.prototype, {
                         read: {
                             get: function() {
                                 return (this.mode & 365) === 365
                             },
                             set: function(I) {
                                 I ? this.mode |= 365 : this.mode &= -366
                             }
@@ -4030,27 +4073,27 @@
                             get: function() {
                                 return (this.mode & 146) === 146
                             },
                             set: function(I) {
                                 I ? this.mode |= 146 : this.mode &= -147
                             }
                         }
-                    }), LB(), vA = Array(4096), yB(hA, "/"), jA("/tmp"), jA("/home"), jA("/home/web_user"), (() => {
+                    }), kB(), vA = Array(4096), GB(hA, "/"), jA("/tmp"), jA("/home"), jA("/home/web_user"), (() => {
                         jA("/dev"), pg(259, {
                             read: () => 0,
                             write: (Q, w, e, S) => S
-                        }), PI("/dev/null", 259), qA(1280, JA), qA(1536, UI), PI("/dev/tty", 1280), PI("/dev/tty1", 1536);
+                        }), zI("/dev/null", 259), qA(1280, JA), qA(1536, GI), zI("/dev/tty", 1280), zI("/dev/tty1", 1536);
                         var I = NA();
-                        lI("random", I), lI("urandom", I), jA("/dev/shm"), jA("/dev/shm/tmp")
+                        fI("random", I), fI("urandom", I), jA("/dev/shm"), jA("/dev/shm/tmp")
                     })(), (() => {
                         jA("/proc");
                         var I = jA("/proc/self");
-                        jA("/proc/self/fd"), yB({
+                        jA("/proc/self/fd"), GB({
                             Ra: () => {
-                                var Q = tB(I, "fd", 16895, 73);
+                                var Q = hB(I, "fd", 16895, 73);
                                 return Q.Ga = {
                                     lookup: (w, e) => {
                                         var S = XA[+e];
                                         if (!S) throw new O(8);
                                         return w = {
                                             parent: null,
                                             Ra: {
@@ -4061,43 +4104,43 @@
                                             }
                                         }, w.parent = w
                                     }
                                 }, Q
                             }
                         }, "/proc/self/fd")
                     })();
-                    var ow = {
+                    var tw = {
                         a: function(I, Q, w, e) {
                             HA("Assertion failed: " + x(I) + ", at: " + [Q ? x(Q) : "unknown filename", w, e ? x(e) : "unknown function"])
                         },
                         h: function(I, Q) {
                             try {
-                                return I = x(I), zI(I, Q), 0
+                                return I = x(I), _I(I, Q), 0
                             } catch (w) {
                                 if (typeof kA > "u" || !(w instanceof O)) throw w;
                                 return -w.Ka
                             }
                         },
                         H: function(I, Q, w) {
                             try {
                                 if (Q = x(Q), Q = hI(I, Q), w & -8) return -28;
                                 var e = uA(Q, {
                                     Sa: !0
                                 }).node;
-                                return e ? (I = "", w & 4 && (I += "r"), w & 2 && (I += "w"), w & 1 && (I += "x"), I && nI(e, I) ? -2 : 0) : -44
+                                return e ? (I = "", w & 4 && (I += "r"), w & 2 && (I += "w"), w & 1 && (I += "x"), I && UI(e, I) ? -2 : 0) : -44
                             } catch (S) {
                                 if (typeof kA > "u" || !(S instanceof O)) throw S;
                                 return -S.Ka
                             }
                         },
                         i: function(I, Q) {
                             try {
                                 var w = XA[I];
                                 if (!w) throw new O(8);
-                                return zI(w.node, Q), 0
+                                return _I(w.node, Q), 0
                             } catch (e) {
                                 if (typeof kA > "u" || !(e instanceof O)) throw e;
                                 return -e.Ka
                             }
                         },
                         g: function(I) {
                             try {
@@ -4113,62 +4156,62 @@
                                 }), 0
                             } catch (S) {
                                 if (typeof kA > "u" || !(S instanceof O)) throw S;
                                 return -S.Ka
                             }
                         },
                         b: function(I, Q, w) {
-                            Ag = w;
+                            Ig = w;
                             try {
                                 var e = TA(I);
                                 switch (Q) {
                                     case 0:
-                                        var S = Ig();
-                                        return 0 > S ? -28 : RB(e, S).fd;
+                                        var S = gg();
+                                        return 0 > S ? -28 : yB(e, S).fd;
                                     case 1:
                                     case 2:
                                         return 0;
                                     case 3:
                                         return e.flags;
                                     case 4:
-                                        return S = Ig(), e.flags |= S, 0;
+                                        return S = gg(), e.flags |= S, 0;
                                     case 5:
-                                        return S = Ig(), _[S + 0 >> 1] = 2, 0;
+                                        return S = gg(), _[S + 0 >> 1] = 2, 0;
                                     case 6:
                                     case 7:
                                         return 0;
                                     case 16:
                                     case 8:
                                         return -28;
                                     case 9:
-                                        return AA[lB() >> 2] = 28, -1;
+                                        return AA[fB() >> 2] = 28, -1;
                                     default:
                                         return -28
                                 }
                             } catch (m) {
                                 if (typeof kA > "u" || !(m instanceof O)) throw m;
                                 return -m.Ka
                             }
                         },
                         G: function(I, Q) {
                             try {
                                 var w = TA(I);
-                                return $I(HI, w.path, Q)
+                                return Ag(lI, w.path, Q)
                             } catch (e) {
                                 if (typeof kA > "u" || !(e instanceof O)) throw e;
                                 return -e.Ka
                             }
                         },
                         l: function(I, Q, w) {
                             try {
                                 if (Q = w + 2097152 >>> 0 < 4194305 - !!Q ? (Q >>> 0) + 4294967296 * w : NaN, isNaN(Q)) return -61;
                                 var e = XA[I];
                                 if (!e) throw new O(8);
                                 if (!(e.flags & 2097155)) throw new O(28);
-                                return cB(e.node, Q), 0
+                                return NB(e.node, Q), 0
                             } catch (S) {
                                 if (typeof kA > "u" || !(S instanceof O)) throw S;
                                 return -S.Ka
                             }
                         },
                         B: function(I, Q) {
                             try {
@@ -4178,15 +4221,15 @@
                             } catch (e) {
                                 if (typeof kA > "u" || !(e instanceof O)) throw e;
                                 return -e.Ka
                             }
                         },
                         E: function(I, Q) {
                             try {
-                                return I = x(I), $I(eB, I, Q)
+                                return I = x(I), Ag(cB, I, Q)
                             } catch (w) {
                                 if (typeof kA > "u" || !(w instanceof O)) throw w;
                                 return -w.Ka
                             }
                         },
                         y: function(I, Q, w) {
                             try {
@@ -4196,62 +4239,62 @@
                                 return -e.Ka
                             }
                         },
                         D: function(I, Q, w, e) {
                             try {
                                 Q = x(Q);
                                 var S = e & 256;
-                                return Q = hI(I, Q, e & 4096), $I(S ? eB : HI, Q, w)
+                                return Q = hI(I, Q, e & 4096), Ag(S ? cB : lI, Q, w)
                             } catch (m) {
                                 if (typeof kA > "u" || !(m instanceof O)) throw m;
                                 return -m.Ka
                             }
                         },
                         v: function(I, Q, w, e) {
-                            Ag = e;
+                            Ig = e;
                             try {
                                 Q = x(Q), Q = hI(I, Q);
-                                var S = e ? Ig() : 0;
-                                return eI(Q, w, S).fd
+                                var S = e ? gg() : 0;
+                                return nI(Q, w, S).fd
                             } catch (m) {
                                 if (typeof kA > "u" || !(m instanceof O)) throw m;
                                 return -m.Ka
                             }
                         },
                         t: function(I, Q, w, e) {
                             try {
                                 if (Q = x(Q), Q = hI(I, Q), 0 >= e) return -28;
-                                var S = nB(Q),
+                                var S = eB(Q),
                                     m = Math.min(e, Z(S)),
                                     v = W[w + m];
                                 return F(S, tA, w, e + 1), W[w + m] = v, m
                             } catch (aA) {
                                 if (typeof kA > "u" || !(aA instanceof O)) throw aA;
                                 return -aA.Ka
                             }
                         },
                         s: function(I) {
                             try {
-                                return I = x(I), GB(I), 0
+                                return I = x(I), UB(I), 0
                             } catch (Q) {
                                 if (typeof kA > "u" || !(Q instanceof O)) throw Q;
                                 return -Q.Ka
                             }
                         },
                         F: function(I, Q) {
                             try {
-                                return I = x(I), $I(HI, I, Q)
+                                return I = x(I), Ag(lI, I, Q)
                             } catch (w) {
                                 if (typeof kA > "u" || !(w instanceof O)) throw w;
                                 return -w.Ka
                             }
                         },
                         p: function(I, Q, w) {
                             try {
-                                return Q = x(Q), Q = hI(I, Q), w === 0 ? UB(Q) : w === 512 ? GB(Q) : HA("Invalid flags passed to unlinkat"), 0
+                                return Q = x(Q), Q = hI(I, Q), w === 0 ? nB(Q) : w === 512 ? UB(Q) : HA("Invalid flags passed to unlinkat"), 0
                             } catch (e) {
                                 if (typeof kA > "u" || !(e instanceof O)) throw e;
                                 return -e.Ka
                             }
                         },
                         o: function(I, Q, w) {
                             try {
@@ -4309,15 +4352,15 @@
                                 return -eA.Ka
                             }
                         },
                         n: mg,
                         q: function() {
                             return 2147483648
                         },
-                        d: KB,
+                        d: YB,
                         c: function(I) {
                             var Q = tA.length;
                             if (I >>>= 0, 2147483648 < I) return !1;
                             for (var w = 1; 4 >= w; w *= 2) {
                                 var e = Q * (1 + .2 / w);
                                 e = Math.min(e, I + 100663296);
                                 var S = Math;
@@ -4332,22 +4375,22 @@
                                 }
                                 if (m) return !0
                             }
                             return !1
                         },
                         z: function(I, Q) {
                             var w = 0;
-                            return YB().forEach(function(e, S) {
+                            return HB().forEach(function(e, S) {
                                 var m = Q + w;
                                 for (S = f[I + 4 * S >> 2] = m, m = 0; m < e.length; ++m) W[S++ >> 0] = e.charCodeAt(m);
                                 W[S >> 0] = 0, w += e.length + 1
                             }), 0
                         },
                         A: function(I, Q) {
-                            var w = YB();
+                            var w = HB();
                             f[I >> 2] = w.length;
                             var e = 0;
                             return w.forEach(function(S) {
                                 e += S.length + 1
                             }), f[Q >> 2] = e, 0
                         },
                         f: function(I) {
@@ -4372,15 +4415,15 @@
                             try {
                                 A: {
                                     var S = TA(I);I = Q;
                                     for (var m = Q = 0; m < w; m++) {
                                         var v = f[I >> 2],
                                             aA = f[I + 4 >> 2];
                                         I += 8;
-                                        var eA = rB(S, W, v, aA);
+                                        var eA = MB(S, W, v, aA);
                                         if (0 > eA) {
                                             var UA = -1;
                                             break A
                                         }
                                         if (Q += eA, eA < aA) break
                                     }
                                     UA = Q
@@ -4393,15 +4436,15 @@
                                 return KA.Ka
                             }
                         },
                         k: function(I, Q, w, e, S) {
                             try {
                                 if (Q = w + 2097152 >>> 0 < 4194305 - !!Q ? (Q >>> 0) + 4294967296 * w : NaN, isNaN(Q)) return 61;
                                 var m = TA(I);
-                                return NB(m, Q, e), Y = [m.position >>> 0, (U = m.position, 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[S >> 2] = Y[0], AA[S + 4 >> 2] = Y[1], m.hb && Q === 0 && e === 0 && (m.hb = null), 0
+                                return rB(m, Q, e), Y = [m.position >>> 0, (U = m.position, 1 <= +Math.abs(U) ? 0 < U ? (Math.min(+Math.floor(U / 4294967296), 4294967295) | 0) >>> 0 : ~~+Math.ceil((U - +(~~U >>> 0)) / 4294967296) >>> 0 : 0)], AA[S >> 2] = Y[0], AA[S + 4 >> 2] = Y[1], m.hb && Q === 0 && e === 0 && (m.hb = null), 0
                             } catch (v) {
                                 if (typeof kA > "u" || !(v instanceof O)) throw v;
                                 return v.Ka
                             }
                         },
                         C: function(I) {
                             try {
@@ -4416,15 +4459,15 @@
                             try {
                                 A: {
                                     var S = TA(I);I = Q;
                                     for (var m = Q = 0; m < w; m++) {
                                         var v = f[I >> 2],
                                             aA = f[I + 4 >> 2];
                                         I += 8;
-                                        var eA = MB(S, W, v, aA);
+                                        var eA = LB(S, W, v, aA);
                                         if (0 > eA) {
                                             var UA = -1;
                                             break A
                                         }
                                         Q += eA
                                     }
                                     UA = Q
@@ -4453,23 +4496,23 @@
                             }).then(function(m) {
                                 return m
                             }).then(S, function(m) {
                                 p("failed to asynchronously prepare wasm: " + m), HA(m)
                             })
                         }
                         var e = {
-                            a: ow
+                            a: tw
                         };
                         if (MA++, C.monitorRunDependencies && C.monitorRunDependencies(MA), C.instantiateWasm) try {
                             return C.instantiateWasm(e, I)
                         } catch (S) {
                             return p("Module.instantiateWasm callback failed with error: " + S), !1
                         }
                         return function() {
-                            return j || typeof WebAssembly.instantiateStreaming != "function" || dA() || i.startsWith("file://") || N || typeof fetch != "function" ? w(Q) : fetch(i, {
+                            return j || typeof WebAssembly.instantiateStreaming != "function" || dA() || D.startsWith("file://") || N || typeof fetch != "function" ? w(Q) : fetch(D, {
                                 credentials: "same-origin"
                             }).then(function(S) {
                                 return WebAssembly.instantiateStreaming(S, e).then(Q, function(m) {
                                     return p("wasm streaming compile failed: " + m), p("falling back to ArrayBuffer instantiation"), w(Q)
                                 })
                             })
                         }(), {}
@@ -4478,16 +4521,16 @@
                     }, C._sqlite3_free = function() {
                         return (C._sqlite3_free = C.asm.K).apply(null, arguments)
                     }, C._sqlite3_value_double = function() {
                         return (C._sqlite3_value_double = C.asm.L).apply(null, arguments)
                     }, C._sqlite3_value_text = function() {
                         return (C._sqlite3_value_text = C.asm.M).apply(null, arguments)
                     };
-                    var lB = C.___errno_location = function() {
-                        return (lB = C.___errno_location = C.asm.N).apply(null, arguments)
+                    var fB = C.___errno_location = function() {
+                        return (fB = C.___errno_location = C.asm.N).apply(null, arguments)
                     };
                     C._sqlite3_prepare_v2 = function() {
                         return (C._sqlite3_prepare_v2 = C.asm.O).apply(null, arguments)
                     }, C._sqlite3_step = function() {
                         return (C._sqlite3_step = C.asm.P).apply(null, arguments)
                     }, C._sqlite3_finalize = function() {
                         return (C._sqlite3_finalize = C.asm.Q).apply(null, arguments)
@@ -4558,51 +4601,51 @@
                     }, C._sqlite3_close_v2 = function() {
                         return (C._sqlite3_close_v2 = C.asm.va).apply(null, arguments)
                     }, C._sqlite3_create_function_v2 = function() {
                         return (C._sqlite3_create_function_v2 = C.asm.wa).apply(null, arguments)
                     }, C._sqlite3_open = function() {
                         return (C._sqlite3_open = C.asm.xa).apply(null, arguments)
                     };
-                    var gg = C._malloc = function() {
-                            return (gg = C._malloc = C.asm.ya).apply(null, arguments)
+                    var Qg = C._malloc = function() {
+                            return (Qg = C._malloc = C.asm.ya).apply(null, arguments)
                         },
-                        Qg = C._free = function() {
-                            return (Qg = C._free = C.asm.za).apply(null, arguments)
+                        Bg = C._free = function() {
+                            return (Bg = C._free = C.asm.za).apply(null, arguments)
                         };
                     C._RegisterExtensionFunctions = function() {
                         return (C._RegisterExtensionFunctions = C.asm.Ba).apply(null, arguments)
                     };
-                    var fB = C._emscripten_builtin_memalign = function() {
-                            return (fB = C._emscripten_builtin_memalign = C.asm.Ca).apply(null, arguments)
+                    var dB = C._emscripten_builtin_memalign = function() {
+                            return (dB = C._emscripten_builtin_memalign = C.asm.Ca).apply(null, arguments)
                         },
-                        uI = C.stackSave = function() {
-                            return (uI = C.stackSave = C.asm.Da).apply(null, arguments)
+                        pI = C.stackSave = function() {
+                            return (pI = C.stackSave = C.asm.Da).apply(null, arguments)
                         },
-                        pI = C.stackRestore = function() {
-                            return (pI = C.stackRestore = C.asm.Ea).apply(null, arguments)
+                        qI = C.stackRestore = function() {
+                            return (qI = C.stackRestore = C.asm.Ea).apply(null, arguments)
                         },
                         EI = C.stackAlloc = function() {
                             return (EI = C.stackAlloc = C.asm.Fa).apply(null, arguments)
                         };
-                    C.UTF8ToString = x, C.stackAlloc = EI, C.stackSave = uI, C.stackRestore = pI, C.cwrap = function(I, Q, w, e) {
+                    C.UTF8ToString = x, C.stackAlloc = EI, C.stackSave = pI, C.stackRestore = qI, C.cwrap = function(I, Q, w, e) {
                         w = w || [];
                         var S = w.every(m => m === "number" || m === "boolean");
                         return Q !== "string" && S && !e ? C["_" + I] : function() {
-                            return Dw(I, Q, w, arguments)
+                            return ww(I, Q, w, arguments)
                         }
                     };
-                    var Bg;
+                    var Cg;
                     rA = function I() {
-                        Bg || dB(), Bg || (rA = I)
+                        Cg || uB(), Cg || (rA = I)
                     };
 
-                    function dB() {
+                    function uB() {
                         function I() {
-                            if (!Bg && (Bg = !0, C.calledRun = !0, !gA)) {
-                                if (C.noFSInit || kB || (kB = !0, LB(), C.stdin = C.stdin, C.stdout = C.stdout, C.stderr = C.stderr, C.stdin ? lI("stdin", C.stdin) : qg("/dev/tty", "/dev/stdin"), C.stdout ? lI("stdout", null, C.stdout) : qg("/dev/tty", "/dev/stdout"), C.stderr ? lI("stderr", null, C.stderr) : qg("/dev/tty1", "/dev/stderr"), eI("/dev/stdin", 0), eI("/dev/stdout", 1), eI("/dev/stderr", 1)), KI = !1, z(YA), C.onRuntimeInitialized && C.onRuntimeInitialized(), C.postRun)
+                            if (!Cg && (Cg = !0, C.calledRun = !0, !gA)) {
+                                if (C.noFSInit || SB || (SB = !0, kB(), C.stdin = C.stdin, C.stdout = C.stdout, C.stderr = C.stderr, C.stdin ? fI("stdin", C.stdin) : qg("/dev/tty", "/dev/stdin"), C.stdout ? fI("stdout", null, C.stdout) : qg("/dev/tty", "/dev/stdout"), C.stderr ? fI("stderr", null, C.stderr) : qg("/dev/tty1", "/dev/stderr"), nI("/dev/stdin", 0), nI("/dev/stdout", 1), nI("/dev/stderr", 1)), YI = !1, z(YA), C.onRuntimeInitialized && C.onRuntimeInitialized(), C.postRun)
                                     for (typeof C.postRun == "function" && (C.postRun = [C.postRun]); C.postRun.length;) {
                                         var Q = C.postRun.shift();
                                         GA.unshift(Q)
                                     }
                                 z(GA)
                             }
                         }
@@ -4614,26 +4657,26 @@
                                     C.setStatus("")
                                 }, 1), I()
                             }, 1)) : I())
                         }
                     }
                     if (C.preInit)
                         for (typeof C.preInit == "function" && (C.preInit = [C.preInit]); 0 < C.preInit.length;) C.preInit.pop()();
-                    return dB(), D
+                    return uB(), i
                 }), g)
             };
         A.exports = o, A.exports.default = o
-    })(Ys);
-    const Hs = Hg;
+    })(fs);
+    const ds = Hg;
 
-    function vI(A) {
+    function jI(A) {
         throw new Error('Could not dynamically require "' + A + '". Please configure the dynamicRequireTargets or/and ignoreDynamicRequires option of @rollup/plugin-commonjs appropriately for this require call to work.')
     }
     var lg = {},
-        ls = {
+        us = {
             get exports() {
                 return lg
             },
             set exports(A) {
                 lg = A
             }
         };
@@ -4652,58 +4695,58 @@
         (function(g) {
             A.exports = g()
         })(function() {
             return function g(o, t, E) {
                 function s(C, r) {
                     if (!t[C]) {
                         if (!o[C]) {
-                            var n = typeof vI == "function" && vI;
+                            var n = typeof jI == "function" && jI;
                             if (!r && n) return n(C, !0);
-                            if (D) return D(C, !0);
+                            if (i) return i(C, !0);
                             var M = new Error("Cannot find module '" + C + "'");
                             throw M.code = "MODULE_NOT_FOUND", M
                         }
                         var R = t[C] = {
                             exports: {}
                         };
                         o[C][0].call(R.exports, function(N) {
                             var a = o[C][1][N];
                             return s(a || N)
                         }, R, R.exports, g, o, t, E)
                     }
                     return t[C].exports
                 }
-                for (var D = typeof vI == "function" && vI, h = 0; h < E.length; h++) s(E[h]);
+                for (var i = typeof jI == "function" && jI, h = 0; h < E.length; h++) s(E[h]);
                 return s
             }({
                 1: [function(g, o, t) {
                     var E = g("./utils"),
                         s = g("./support"),
-                        D = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
+                        i = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
                     t.encode = function(h) {
-                        for (var C, r, n, M, R, N, a, G = [], y = 0, c = h.length, k = c, H = E.getTypeOf(h) !== "string"; y < h.length;) k = c - y, n = H ? (C = h[y++], r = y < c ? h[y++] : 0, y < c ? h[y++] : 0) : (C = h.charCodeAt(y++), r = y < c ? h.charCodeAt(y++) : 0, y < c ? h.charCodeAt(y++) : 0), M = C >> 2, R = (3 & C) << 4 | r >> 4, N = 1 < k ? (15 & r) << 2 | n >> 6 : 64, a = 2 < k ? 63 & n : 64, G.push(D.charAt(M) + D.charAt(R) + D.charAt(N) + D.charAt(a));
+                        for (var C, r, n, M, R, N, a, G = [], y = 0, c = h.length, k = c, H = E.getTypeOf(h) !== "string"; y < h.length;) k = c - y, n = H ? (C = h[y++], r = y < c ? h[y++] : 0, y < c ? h[y++] : 0) : (C = h.charCodeAt(y++), r = y < c ? h.charCodeAt(y++) : 0, y < c ? h.charCodeAt(y++) : 0), M = C >> 2, R = (3 & C) << 4 | r >> 4, N = 1 < k ? (15 & r) << 2 | n >> 6 : 64, a = 2 < k ? 63 & n : 64, G.push(i.charAt(M) + i.charAt(R) + i.charAt(N) + i.charAt(a));
                         return G.join("")
                     }, t.decode = function(h) {
                         var C, r, n, M, R, N, a = 0,
                             G = 0,
                             y = "data:";
                         if (h.substr(0, y.length) === y) throw new Error("Invalid base64 input, it looks like a data url.");
                         var c, k = 3 * (h = h.replace(/[^A-Za-z0-9+/=]/g, "")).length / 4;
-                        if (h.charAt(h.length - 1) === D.charAt(64) && k--, h.charAt(h.length - 2) === D.charAt(64) && k--, k % 1 != 0) throw new Error("Invalid base64 input, bad content length.");
-                        for (c = s.uint8array ? new Uint8Array(0 | k) : new Array(0 | k); a < h.length;) C = D.indexOf(h.charAt(a++)) << 2 | (M = D.indexOf(h.charAt(a++))) >> 4, r = (15 & M) << 4 | (R = D.indexOf(h.charAt(a++))) >> 2, n = (3 & R) << 6 | (N = D.indexOf(h.charAt(a++))), c[G++] = C, R !== 64 && (c[G++] = r), N !== 64 && (c[G++] = n);
+                        if (h.charAt(h.length - 1) === i.charAt(64) && k--, h.charAt(h.length - 2) === i.charAt(64) && k--, k % 1 != 0) throw new Error("Invalid base64 input, bad content length.");
+                        for (c = s.uint8array ? new Uint8Array(0 | k) : new Array(0 | k); a < h.length;) C = i.indexOf(h.charAt(a++)) << 2 | (M = i.indexOf(h.charAt(a++))) >> 4, r = (15 & M) << 4 | (R = i.indexOf(h.charAt(a++))) >> 2, n = (3 & R) << 6 | (N = i.indexOf(h.charAt(a++))), c[G++] = C, R !== 64 && (c[G++] = r), N !== 64 && (c[G++] = n);
                         return c
                     }
                 }, {
                     "./support": 30,
                     "./utils": 32
                 }],
                 2: [function(g, o, t) {
                     var E = g("./external"),
                         s = g("./stream/DataWorker"),
-                        D = g("./stream/Crc32Probe"),
+                        i = g("./stream/Crc32Probe"),
                         h = g("./stream/DataLengthProbe");
 
                     function C(r, n, M, R, N) {
                         this.compressedSize = r, this.uncompressedSize = n, this.crc32 = M, this.compression = R, this.compressedContent = N
                     }
                     C.prototype = {
                         getContentWorker: function() {
@@ -4713,15 +4756,15 @@
                                 if (this.streamInfo.data_length !== n.uncompressedSize) throw new Error("Bug : uncompressed data size mismatch")
                             }), r
                         },
                         getCompressedWorker: function() {
                             return new s(E.Promise.resolve(this.compressedContent)).withStreamInfo("compressedSize", this.compressedSize).withStreamInfo("uncompressedSize", this.uncompressedSize).withStreamInfo("crc32", this.crc32).withStreamInfo("compression", this.compression)
                         }
                     }, C.createWorkerFrom = function(r, n, M) {
-                        return r.pipe(new D).pipe(new h("uncompressedSize")).pipe(n.compressWorker(M)).pipe(new h("compressedSize")).withStreamInfo("compression", n)
+                        return r.pipe(new i).pipe(new h("uncompressedSize")).pipe(n.compressWorker(M)).pipe(new h("compressedSize")).withStreamInfo("compression", n)
                     }, o.exports = C
                 }, {
                     "./external": 6,
                     "./stream/Crc32Probe": 25,
                     "./stream/DataLengthProbe": 26,
                     "./stream/DataWorker": 27
                 }],
@@ -4739,35 +4782,35 @@
                 }, {
                     "./flate": 7,
                     "./stream/GenericWorker": 28
                 }],
                 4: [function(g, o, t) {
                     var E = g("./utils"),
                         s = function() {
-                            for (var D, h = [], C = 0; C < 256; C++) {
-                                D = C;
-                                for (var r = 0; r < 8; r++) D = 1 & D ? 3988292384 ^ D >>> 1 : D >>> 1;
-                                h[C] = D
+                            for (var i, h = [], C = 0; C < 256; C++) {
+                                i = C;
+                                for (var r = 0; r < 8; r++) i = 1 & i ? 3988292384 ^ i >>> 1 : i >>> 1;
+                                h[C] = i
                             }
                             return h
                         }();
-                    o.exports = function(D, h) {
-                        return D !== void 0 && D.length ? E.getTypeOf(D) !== "string" ? function(C, r, n, M) {
+                    o.exports = function(i, h) {
+                        return i !== void 0 && i.length ? E.getTypeOf(i) !== "string" ? function(C, r, n, M) {
                             var R = s,
                                 N = M + n;
                             C ^= -1;
                             for (var a = M; a < N; a++) C = C >>> 8 ^ R[255 & (C ^ r[a])];
                             return -1 ^ C
-                        }(0 | h, D, D.length, 0) : function(C, r, n, M) {
+                        }(0 | h, i, i.length, 0) : function(C, r, n, M) {
                             var R = s,
                                 N = M + n;
                             C ^= -1;
                             for (var a = M; a < N; a++) C = C >>> 8 ^ R[255 & (C ^ r.charCodeAt(a))];
                             return -1 ^ C
-                        }(0 | h, D, D.length, 0) : 0
+                        }(0 | h, i, i.length, 0) : 0
                     }
                 }, {
                     "./utils": 32
                 }],
                 5: [function(g, o, t) {
                     t.base64 = !1, t.binary = !1, t.dir = !1, t.createFolders = !0, t.date = null, t.compression = null, t.compressionOptions = null, t.comment = null, t.unixPermissions = null, t.dosPermissions = null
                 }, {}],
@@ -4778,23 +4821,23 @@
                     }
                 }, {
                     lie: 37
                 }],
                 7: [function(g, o, t) {
                     var E = typeof Uint8Array < "u" && typeof Uint16Array < "u" && typeof Uint32Array < "u",
                         s = g("pako"),
-                        D = g("./utils"),
+                        i = g("./utils"),
                         h = g("./stream/GenericWorker"),
                         C = E ? "uint8array" : "array";
 
                     function r(n, M) {
                         h.call(this, "FlateWorker/" + n), this._pako = null, this._pakoAction = n, this._pakoOptions = M, this.meta = {}
                     }
-                    t.magic = "\b\0", D.inherits(r, h), r.prototype.processChunk = function(n) {
-                        this.meta = n.meta, this._pako === null && this._createPako(), this._pako.push(D.transformTo(C, n.data), !1)
+                    t.magic = "\b\0", i.inherits(r, h), r.prototype.processChunk = function(n) {
+                        this.meta = n.meta, this._pako === null && this._createPako(), this._pako.push(i.transformTo(C, n.data), !1)
                     }, r.prototype.flush = function() {
                         h.prototype.flush.call(this), this._pako === null && this._createPako(), this._pako.push([], !0)
                     }, r.prototype.cleanUp = function() {
                         h.prototype.cleanUp.call(this), this._pako = null
                     }, r.prototype._createPako = function() {
                         this._pako = new s[this._pakoAction]({
                             raw: !0,
@@ -4824,19 +4867,19 @@
                         return G
                     }
 
                     function s(R, N, a, G, y, c) {
                         var k, H, l = R.file,
                             T = R.compression,
                             p = c !== C.utf8encode,
-                            j = D.transformTo("string", c(l.name)),
-                            b = D.transformTo("string", C.utf8encode(l.name)),
+                            j = i.transformTo("string", c(l.name)),
+                            b = i.transformTo("string", C.utf8encode(l.name)),
                             gA = l.comment,
-                            oA = D.transformTo("string", c(gA)),
-                            J = D.transformTo("string", C.utf8encode(gA)),
+                            oA = i.transformTo("string", c(gA)),
+                            J = i.transformTo("string", C.utf8encode(gA)),
                             x = b.length !== l.name.length,
                             F = J.length !== gA.length,
                             Z = "",
                             iA = "",
                             W = "",
                             tA = l.dir,
                             _ = l.date,
@@ -4859,24 +4902,24 @@
                         var CA = "";
                         return CA += `
 \0`, CA += E(f, 2), CA += T.magic, CA += E(k, 2), CA += E(H, 2), CA += E(AA.crc32, 4), CA += E(AA.compressedSize, 4), CA += E(AA.uncompressedSize, 4), CA += E(j.length, 2), CA += E(Z.length, 2), {
                             fileRecord: n.LOCAL_FILE_HEADER + CA + j + Z,
                             dirRecord: n.CENTRAL_FILE_HEADER + E(sA, 2) + CA + E(oA.length, 2) + "\0\0\0\0" + E(q, 4) + E(G, 4) + j + Z + oA
                         }
                     }
-                    var D = g("../utils"),
+                    var i = g("../utils"),
                         h = g("../stream/GenericWorker"),
                         C = g("../utf8"),
                         r = g("../crc32"),
                         n = g("../signature");
 
                     function M(R, N, a, G) {
                         h.call(this, "ZipFileWorker"), this.bytesWritten = 0, this.zipComment = N, this.zipPlatform = a, this.encodeFileName = G, this.streamFiles = R, this.accumulate = !1, this.contentBuffer = [], this.dirRecords = [], this.currentSourceOffset = 0, this.entriesCount = 0, this.currentFile = null, this._sources = []
                     }
-                    D.inherits(M, h), M.prototype.push = function(R) {
+                    i.inherits(M, h), M.prototype.push = function(R) {
                         var N = R.meta.percent || 0,
                             a = this.entriesCount,
                             G = this._sources.length;
                         this.accumulate ? this.contentBuffer.push(R) : (this.bytesWritten += R.data.length, h.prototype.push.call(this, {
                             data: R.data,
                             meta: {
                                 currentFile: this.currentFile,
@@ -4920,15 +4963,15 @@
                             data: this.dirRecords[N],
                             meta: {
                                 percent: 100
                             }
                         });
                         var a = this.bytesWritten - R,
                             G = function(y, c, k, H, l) {
-                                var T = D.transformTo("string", l(H));
+                                var T = i.transformTo("string", l(H));
                                 return n.CENTRAL_DIRECTORY_END + "\0\0\0\0" + E(y, 2) + E(y, 2) + E(c, 4) + E(k, 4) + E(T.length, 2) + T
                             }(this.dirRecords.length, a, R, this.zipComment, this.encodeFileName);
                         this.push({
                             data: G,
                             meta: {
                                 percent: 100
                             }
@@ -4964,19 +5007,19 @@
                     "../stream/GenericWorker": 28,
                     "../utf8": 31,
                     "../utils": 32
                 }],
                 9: [function(g, o, t) {
                     var E = g("../compressions"),
                         s = g("./ZipFileWorker");
-                    t.generateWorker = function(D, h, C) {
+                    t.generateWorker = function(i, h, C) {
                         var r = new s(h.streamFiles, C, h.platform, h.encodeFileName),
                             n = 0;
                         try {
-                            D.forEach(function(M, R) {
+                            i.forEach(function(M, R) {
                                 n++;
                                 var N = function(c, k) {
                                         var H = c || k,
                                             l = E[H];
                                         if (!l) throw new Error(H + " is not a valid compression method !");
                                         return l
                                     }(R.options.compression, h.compression),
@@ -5003,31 +5046,31 @@
                 }],
                 10: [function(g, o, t) {
                     function E() {
                         if (!(this instanceof E)) return new E;
                         if (arguments.length) throw new Error("The constructor with parameters has been removed in JSZip 3.0, please check the upgrade guide.");
                         this.files = Object.create(null), this.comment = null, this.root = "", this.clone = function() {
                             var s = new E;
-                            for (var D in this) typeof this[D] != "function" && (s[D] = this[D]);
+                            for (var i in this) typeof this[i] != "function" && (s[i] = this[i]);
                             return s
                         }
-                    }(E.prototype = g("./object")).loadAsync = g("./load"), E.support = g("./support"), E.defaults = g("./defaults"), E.version = "3.10.1", E.loadAsync = function(s, D) {
-                        return new E().loadAsync(s, D)
+                    }(E.prototype = g("./object")).loadAsync = g("./load"), E.support = g("./support"), E.defaults = g("./defaults"), E.version = "3.10.1", E.loadAsync = function(s, i) {
+                        return new E().loadAsync(s, i)
                     }, E.external = g("./external"), o.exports = E
                 }, {
                     "./defaults": 5,
                     "./external": 6,
                     "./load": 11,
                     "./object": 15,
                     "./support": 30
                 }],
                 11: [function(g, o, t) {
                     var E = g("./utils"),
                         s = g("./external"),
-                        D = g("./utf8"),
+                        i = g("./utf8"),
                         h = g("./zipEntries"),
                         C = g("./stream/Crc32Probe"),
                         r = g("./nodejsUtils");
 
                     function n(M) {
                         return new s.Promise(function(R, N) {
                             var a = M.decompressed.getContentWorker().pipe(new C);
@@ -5041,15 +5084,15 @@
                     o.exports = function(M, R) {
                         var N = this;
                         return R = E.extend(R || {}, {
                             base64: !1,
                             checkCRC32: !1,
                             optimizedBinaryString: !1,
                             createFolders: !1,
-                            decodeFileName: D.utf8decode
+                            decodeFileName: i.utf8decode
                         }), r.isNode && r.isStream(M) ? s.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file.")) : E.prepareContent("the loaded zip file", M, !0, R.optimizedBinaryString, R.base64).then(function(a) {
                             var G = new h(R);
                             return G.load(a), G
                         }).then(function(a) {
                             var G = [s.Promise.resolve(a)],
                                 y = a.files;
                             if (R.checkCRC32)
@@ -5082,47 +5125,47 @@
                     "./utils": 32,
                     "./zipEntries": 33
                 }],
                 12: [function(g, o, t) {
                     var E = g("../utils"),
                         s = g("../stream/GenericWorker");
 
-                    function D(h, C) {
+                    function i(h, C) {
                         s.call(this, "Nodejs stream input adapter for " + h), this._upstreamEnded = !1, this._bindStream(C)
                     }
-                    E.inherits(D, s), D.prototype._bindStream = function(h) {
+                    E.inherits(i, s), i.prototype._bindStream = function(h) {
                         var C = this;
                         (this._stream = h).pause(), h.on("data", function(r) {
                             C.push({
                                 data: r,
                                 meta: {
                                     percent: 0
                                 }
                             })
                         }).on("error", function(r) {
                             C.isPaused ? this.generatedError = r : C.error(r)
                         }).on("end", function() {
                             C.isPaused ? C._upstreamEnded = !0 : C.end()
                         })
-                    }, D.prototype.pause = function() {
+                    }, i.prototype.pause = function() {
                         return !!s.prototype.pause.call(this) && (this._stream.pause(), !0)
-                    }, D.prototype.resume = function() {
+                    }, i.prototype.resume = function() {
                         return !!s.prototype.resume.call(this) && (this._upstreamEnded ? this.end() : this._stream.resume(), !0)
-                    }, o.exports = D
+                    }, o.exports = i
                 }, {
                     "../stream/GenericWorker": 28,
                     "../utils": 32
                 }],
                 13: [function(g, o, t) {
                     var E = g("readable-stream").Readable;
 
-                    function s(D, h, C) {
-                        E.call(this, h), this._helper = D;
+                    function s(i, h, C) {
+                        E.call(this, h), this._helper = i;
                         var r = this;
-                        D.on("data", function(n, M) {
+                        i.on("data", function(n, M) {
                             r.push(n) || r._helper.pause(), C && C(M)
                         }).on("error", function(n) {
                             r.emit("error", n)
                         }).on("end", function() {
                             r.push(null)
                         })
                     }
@@ -5152,26 +5195,26 @@
                         isStream: function(E) {
                             return E && typeof E.on == "function" && typeof E.pause == "function" && typeof E.resume == "function"
                         }
                     }
                 }, {}],
                 15: [function(g, o, t) {
                     function E(l, T, p) {
-                        var j, b = D.getTypeOf(T),
-                            gA = D.extend(p || {}, r);
+                        var j, b = i.getTypeOf(T),
+                            gA = i.extend(p || {}, r);
                         gA.date = gA.date || new Date, gA.compression !== null && (gA.compression = gA.compression.toUpperCase()), typeof gA.unixPermissions == "string" && (gA.unixPermissions = parseInt(gA.unixPermissions, 8)), gA.unixPermissions && 16384 & gA.unixPermissions && (gA.dir = !0), gA.dosPermissions && 16 & gA.dosPermissions && (gA.dir = !0), gA.dir && (l = y(l)), gA.createFolders && (j = G(l)) && c.call(this, j, !0);
                         var oA = b === "string" && gA.binary === !1 && gA.base64 === !1;
                         p && p.binary !== void 0 || (gA.binary = !oA), (T instanceof n && T.uncompressedSize === 0 || gA.dir || !T || T.length === 0) && (gA.base64 = !1, gA.binary = !0, T = "", gA.compression = "STORE", b = "string");
                         var J = null;
-                        J = T instanceof n || T instanceof h ? T : N.isNode && N.isStream(T) ? new a(l, T) : D.prepareContent(l, T, gA.binary, gA.optimizedBinaryString, gA.base64);
+                        J = T instanceof n || T instanceof h ? T : N.isNode && N.isStream(T) ? new a(l, T) : i.prepareContent(l, T, gA.binary, gA.optimizedBinaryString, gA.base64);
                         var x = new M(l, J, gA);
                         this.files[l] = x
                     }
                     var s = g("./utf8"),
-                        D = g("./utils"),
+                        i = g("./utils"),
                         h = g("./stream/GenericWorker"),
                         C = g("./stream/StreamHelper"),
                         r = g("./defaults"),
                         n = g("./compressedObject"),
                         M = g("./zipObject"),
                         R = g("./generate"),
                         N = g("./nodejsUtils"),
@@ -5241,25 +5284,25 @@
                         },
                         generate: function() {
                             throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
                         },
                         generateInternalStream: function(l) {
                             var T, p = {};
                             try {
-                                if ((p = D.extend(l || {}, {
+                                if ((p = i.extend(l || {}, {
                                         streamFiles: !1,
                                         compression: "STORE",
                                         compressionOptions: null,
                                         type: "",
                                         platform: "DOS",
                                         comment: null,
                                         mimeType: "application/zip",
                                         encodeFileName: s.utf8encode
                                     })).type = p.type.toLowerCase(), p.compression = p.compression.toUpperCase(), p.type === "binarystring" && (p.type = "string"), !p.type) throw new Error("No output type specified.");
-                                D.checkSupport(p.type), p.platform !== "darwin" && p.platform !== "freebsd" && p.platform !== "linux" && p.platform !== "sunos" || (p.platform = "UNIX"), p.platform === "win32" && (p.platform = "DOS");
+                                i.checkSupport(p.type), p.platform !== "darwin" && p.platform !== "freebsd" && p.platform !== "linux" && p.platform !== "sunos" || (p.platform = "UNIX"), p.platform === "win32" && (p.platform = "DOS");
                                 var j = p.comment || this.comment || "";
                                 T = R.generateWorker(this, p, j)
                             } catch (b) {
                                 (T = new h("error")).error(b)
                             }
                             return new C(T, p.type || "string", p.mimeType)
                         },
@@ -5287,140 +5330,140 @@
                     o.exports = g("stream")
                 }, {
                     stream: void 0
                 }],
                 17: [function(g, o, t) {
                     var E = g("./DataReader");
 
-                    function s(D) {
-                        E.call(this, D);
-                        for (var h = 0; h < this.data.length; h++) D[h] = 255 & D[h]
-                    }
-                    g("../utils").inherits(s, E), s.prototype.byteAt = function(D) {
-                        return this.data[this.zero + D]
-                    }, s.prototype.lastIndexOfSignature = function(D) {
-                        for (var h = D.charCodeAt(0), C = D.charCodeAt(1), r = D.charCodeAt(2), n = D.charCodeAt(3), M = this.length - 4; 0 <= M; --M)
+                    function s(i) {
+                        E.call(this, i);
+                        for (var h = 0; h < this.data.length; h++) i[h] = 255 & i[h]
+                    }
+                    g("../utils").inherits(s, E), s.prototype.byteAt = function(i) {
+                        return this.data[this.zero + i]
+                    }, s.prototype.lastIndexOfSignature = function(i) {
+                        for (var h = i.charCodeAt(0), C = i.charCodeAt(1), r = i.charCodeAt(2), n = i.charCodeAt(3), M = this.length - 4; 0 <= M; --M)
                             if (this.data[M] === h && this.data[M + 1] === C && this.data[M + 2] === r && this.data[M + 3] === n) return M - this.zero;
                         return -1
-                    }, s.prototype.readAndCheckSignature = function(D) {
-                        var h = D.charCodeAt(0),
-                            C = D.charCodeAt(1),
-                            r = D.charCodeAt(2),
-                            n = D.charCodeAt(3),
+                    }, s.prototype.readAndCheckSignature = function(i) {
+                        var h = i.charCodeAt(0),
+                            C = i.charCodeAt(1),
+                            r = i.charCodeAt(2),
+                            n = i.charCodeAt(3),
                             M = this.readData(4);
                         return h === M[0] && C === M[1] && r === M[2] && n === M[3]
-                    }, s.prototype.readData = function(D) {
-                        if (this.checkOffset(D), D === 0) return [];
-                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + D);
-                        return this.index += D, h
+                    }, s.prototype.readData = function(i) {
+                        if (this.checkOffset(i), i === 0) return [];
+                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + i);
+                        return this.index += i, h
                     }, o.exports = s
                 }, {
                     "../utils": 32,
                     "./DataReader": 18
                 }],
                 18: [function(g, o, t) {
                     var E = g("../utils");
 
-                    function s(D) {
-                        this.data = D, this.length = D.length, this.index = 0, this.zero = 0
+                    function s(i) {
+                        this.data = i, this.length = i.length, this.index = 0, this.zero = 0
                     }
                     s.prototype = {
-                        checkOffset: function(D) {
-                            this.checkIndex(this.index + D)
+                        checkOffset: function(i) {
+                            this.checkIndex(this.index + i)
                         },
-                        checkIndex: function(D) {
-                            if (this.length < this.zero + D || D < 0) throw new Error("End of data reached (data length = " + this.length + ", asked index = " + D + "). Corrupted zip ?")
+                        checkIndex: function(i) {
+                            if (this.length < this.zero + i || i < 0) throw new Error("End of data reached (data length = " + this.length + ", asked index = " + i + "). Corrupted zip ?")
                         },
-                        setIndex: function(D) {
-                            this.checkIndex(D), this.index = D
+                        setIndex: function(i) {
+                            this.checkIndex(i), this.index = i
                         },
-                        skip: function(D) {
-                            this.setIndex(this.index + D)
+                        skip: function(i) {
+                            this.setIndex(this.index + i)
                         },
                         byteAt: function() {},
-                        readInt: function(D) {
+                        readInt: function(i) {
                             var h, C = 0;
-                            for (this.checkOffset(D), h = this.index + D - 1; h >= this.index; h--) C = (C << 8) + this.byteAt(h);
-                            return this.index += D, C
+                            for (this.checkOffset(i), h = this.index + i - 1; h >= this.index; h--) C = (C << 8) + this.byteAt(h);
+                            return this.index += i, C
                         },
-                        readString: function(D) {
-                            return E.transformTo("string", this.readData(D))
+                        readString: function(i) {
+                            return E.transformTo("string", this.readData(i))
                         },
                         readData: function() {},
                         lastIndexOfSignature: function() {},
                         readAndCheckSignature: function() {},
                         readDate: function() {
-                            var D = this.readInt(4);
-                            return new Date(Date.UTC(1980 + (D >> 25 & 127), (D >> 21 & 15) - 1, D >> 16 & 31, D >> 11 & 31, D >> 5 & 63, (31 & D) << 1))
+                            var i = this.readInt(4);
+                            return new Date(Date.UTC(1980 + (i >> 25 & 127), (i >> 21 & 15) - 1, i >> 16 & 31, i >> 11 & 31, i >> 5 & 63, (31 & i) << 1))
                         }
                     }, o.exports = s
                 }, {
                     "../utils": 32
                 }],
                 19: [function(g, o, t) {
                     var E = g("./Uint8ArrayReader");
 
-                    function s(D) {
-                        E.call(this, D)
+                    function s(i) {
+                        E.call(this, i)
                     }
-                    g("../utils").inherits(s, E), s.prototype.readData = function(D) {
-                        this.checkOffset(D);
-                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + D);
-                        return this.index += D, h
+                    g("../utils").inherits(s, E), s.prototype.readData = function(i) {
+                        this.checkOffset(i);
+                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + i);
+                        return this.index += i, h
                     }, o.exports = s
                 }, {
                     "../utils": 32,
                     "./Uint8ArrayReader": 21
                 }],
                 20: [function(g, o, t) {
                     var E = g("./DataReader");
 
-                    function s(D) {
-                        E.call(this, D)
+                    function s(i) {
+                        E.call(this, i)
                     }
-                    g("../utils").inherits(s, E), s.prototype.byteAt = function(D) {
-                        return this.data.charCodeAt(this.zero + D)
-                    }, s.prototype.lastIndexOfSignature = function(D) {
-                        return this.data.lastIndexOf(D) - this.zero
-                    }, s.prototype.readAndCheckSignature = function(D) {
-                        return D === this.readData(4)
-                    }, s.prototype.readData = function(D) {
-                        this.checkOffset(D);
-                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + D);
-                        return this.index += D, h
+                    g("../utils").inherits(s, E), s.prototype.byteAt = function(i) {
+                        return this.data.charCodeAt(this.zero + i)
+                    }, s.prototype.lastIndexOfSignature = function(i) {
+                        return this.data.lastIndexOf(i) - this.zero
+                    }, s.prototype.readAndCheckSignature = function(i) {
+                        return i === this.readData(4)
+                    }, s.prototype.readData = function(i) {
+                        this.checkOffset(i);
+                        var h = this.data.slice(this.zero + this.index, this.zero + this.index + i);
+                        return this.index += i, h
                     }, o.exports = s
                 }, {
                     "../utils": 32,
                     "./DataReader": 18
                 }],
                 21: [function(g, o, t) {
                     var E = g("./ArrayReader");
 
-                    function s(D) {
-                        E.call(this, D)
+                    function s(i) {
+                        E.call(this, i)
                     }
-                    g("../utils").inherits(s, E), s.prototype.readData = function(D) {
-                        if (this.checkOffset(D), D === 0) return new Uint8Array(0);
-                        var h = this.data.subarray(this.zero + this.index, this.zero + this.index + D);
-                        return this.index += D, h
+                    g("../utils").inherits(s, E), s.prototype.readData = function(i) {
+                        if (this.checkOffset(i), i === 0) return new Uint8Array(0);
+                        var h = this.data.subarray(this.zero + this.index, this.zero + this.index + i);
+                        return this.index += i, h
                     }, o.exports = s
                 }, {
                     "../utils": 32,
                     "./ArrayReader": 17
                 }],
                 22: [function(g, o, t) {
                     var E = g("../utils"),
                         s = g("../support"),
-                        D = g("./ArrayReader"),
+                        i = g("./ArrayReader"),
                         h = g("./StringReader"),
                         C = g("./NodeBufferReader"),
                         r = g("./Uint8ArrayReader");
                     o.exports = function(n) {
                         var M = E.getTypeOf(n);
-                        return E.checkSupport(M), M !== "string" || s.uint8array ? M === "nodebuffer" ? new C(n) : s.uint8array ? new r(E.transformTo("uint8array", n)) : new D(E.transformTo("array", n)) : new h(n)
+                        return E.checkSupport(M), M !== "string" || s.uint8array ? M === "nodebuffer" ? new C(n) : s.uint8array ? new r(E.transformTo("uint8array", n)) : new i(E.transformTo("array", n)) : new h(n)
                     }
                 }, {
                     "../support": 30,
                     "../utils": 32,
                     "./ArrayReader": 17,
                     "./NodeBufferReader": 19,
                     "./StringReader": 20,
@@ -5429,80 +5472,80 @@
                 23: [function(g, o, t) {
                     t.LOCAL_FILE_HEADER = "PK", t.CENTRAL_FILE_HEADER = "PK", t.CENTRAL_DIRECTORY_END = "PK", t.ZIP64_CENTRAL_DIRECTORY_LOCATOR = "PK\x07", t.ZIP64_CENTRAL_DIRECTORY_END = "PK", t.DATA_DESCRIPTOR = "PK\x07\b"
                 }, {}],
                 24: [function(g, o, t) {
                     var E = g("./GenericWorker"),
                         s = g("../utils");
 
-                    function D(h) {
+                    function i(h) {
                         E.call(this, "ConvertWorker to " + h), this.destType = h
                     }
-                    s.inherits(D, E), D.prototype.processChunk = function(h) {
+                    s.inherits(i, E), i.prototype.processChunk = function(h) {
                         this.push({
                             data: s.transformTo(this.destType, h.data),
                             meta: h.meta
                         })
-                    }, o.exports = D
+                    }, o.exports = i
                 }, {
                     "../utils": 32,
                     "./GenericWorker": 28
                 }],
                 25: [function(g, o, t) {
                     var E = g("./GenericWorker"),
                         s = g("../crc32");
 
-                    function D() {
+                    function i() {
                         E.call(this, "Crc32Probe"), this.withStreamInfo("crc32", 0)
                     }
-                    g("../utils").inherits(D, E), D.prototype.processChunk = function(h) {
+                    g("../utils").inherits(i, E), i.prototype.processChunk = function(h) {
                         this.streamInfo.crc32 = s(h.data, this.streamInfo.crc32 || 0), this.push(h)
-                    }, o.exports = D
+                    }, o.exports = i
                 }, {
                     "../crc32": 4,
                     "../utils": 32,
                     "./GenericWorker": 28
                 }],
                 26: [function(g, o, t) {
                     var E = g("../utils"),
                         s = g("./GenericWorker");
 
-                    function D(h) {
+                    function i(h) {
                         s.call(this, "DataLengthProbe for " + h), this.propName = h, this.withStreamInfo(h, 0)
                     }
-                    E.inherits(D, s), D.prototype.processChunk = function(h) {
+                    E.inherits(i, s), i.prototype.processChunk = function(h) {
                         if (h) {
                             var C = this.streamInfo[this.propName] || 0;
                             this.streamInfo[this.propName] = C + h.data.length
                         }
                         s.prototype.processChunk.call(this, h)
-                    }, o.exports = D
+                    }, o.exports = i
                 }, {
                     "../utils": 32,
                     "./GenericWorker": 28
                 }],
                 27: [function(g, o, t) {
                     var E = g("../utils"),
                         s = g("./GenericWorker");
 
-                    function D(h) {
+                    function i(h) {
                         s.call(this, "DataWorker");
                         var C = this;
                         this.dataIsReady = !1, this.index = 0, this.max = 0, this.data = null, this.type = "", this._tickScheduled = !1, h.then(function(r) {
                             C.dataIsReady = !0, C.data = r, C.max = r && r.length || 0, C.type = E.getTypeOf(r), C.isPaused || C._tickAndRepeat()
                         }, function(r) {
                             C.error(r)
                         })
                     }
-                    E.inherits(D, s), D.prototype.cleanUp = function() {
+                    E.inherits(i, s), i.prototype.cleanUp = function() {
                         s.prototype.cleanUp.call(this), this.data = null
-                    }, D.prototype.resume = function() {
+                    }, i.prototype.resume = function() {
                         return !!s.prototype.resume.call(this) && (!this._tickScheduled && this.dataIsReady && (this._tickScheduled = !0, E.delay(this._tickAndRepeat, [], this)), !0)
-                    }, D.prototype._tickAndRepeat = function() {
+                    }, i.prototype._tickAndRepeat = function() {
                         this._tickScheduled = !1, this.isPaused || this.isFinished || (this._tick(), this.isFinished || (E.delay(this._tickAndRepeat, [], this), this._tickScheduled = !0))
-                    }, D.prototype._tick = function() {
+                    }, i.prototype._tick = function() {
                         if (this.isPaused || this.isFinished) return !1;
                         var h = null,
                             C = Math.min(this.max, this.index + 16384);
                         if (this.index >= this.max) return this.end();
                         switch (this.type) {
                             case "string":
                                 h = this.data.substring(this.index, C);
@@ -5516,15 +5559,15 @@
                         }
                         return this.index = C, this.push({
                             data: h,
                             meta: {
                                 percent: this.max ? this.index / this.max * 100 : 0
                             }
                         })
-                    }, o.exports = D
+                    }, o.exports = i
                 }, {
                     "../utils": 32,
                     "./GenericWorker": 28
                 }],
                 28: [function(g, o, t) {
                     function E(s) {
                         this.name = s || "default", this.streamInfo = {}, this.generatedError = null, this.extraStreamInfo = {}, this.isPaused = !0, this.isFinished = !1, this.isLocked = !1, this._listeners = {
@@ -5546,53 +5589,53 @@
                                 this.emit("error", s)
                             }
                             return !0
                         },
                         error: function(s) {
                             return !this.isFinished && (this.isPaused ? this.generatedError = s : (this.isFinished = !0, this.emit("error", s), this.previous && this.previous.error(s), this.cleanUp()), !0)
                         },
-                        on: function(s, D) {
-                            return this._listeners[s].push(D), this
+                        on: function(s, i) {
+                            return this._listeners[s].push(i), this
                         },
                         cleanUp: function() {
                             this.streamInfo = this.generatedError = this.extraStreamInfo = null, this._listeners = []
                         },
-                        emit: function(s, D) {
+                        emit: function(s, i) {
                             if (this._listeners[s])
-                                for (var h = 0; h < this._listeners[s].length; h++) this._listeners[s][h].call(this, D)
+                                for (var h = 0; h < this._listeners[s].length; h++) this._listeners[s][h].call(this, i)
                         },
                         pipe: function(s) {
                             return s.registerPrevious(this)
                         },
                         registerPrevious: function(s) {
                             if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
                             this.streamInfo = s.streamInfo, this.mergeStreamInfo(), this.previous = s;
-                            var D = this;
+                            var i = this;
                             return s.on("data", function(h) {
-                                D.processChunk(h)
+                                i.processChunk(h)
                             }), s.on("end", function() {
-                                D.end()
+                                i.end()
                             }), s.on("error", function(h) {
-                                D.error(h)
+                                i.error(h)
                             }), this
                         },
                         pause: function() {
                             return !this.isPaused && !this.isFinished && (this.isPaused = !0, this.previous && this.previous.pause(), !0)
                         },
                         resume: function() {
                             if (!this.isPaused || this.isFinished) return !1;
                             var s = this.isPaused = !1;
                             return this.generatedError && (this.error(this.generatedError), s = !0), this.previous && this.previous.resume(), !s
                         },
                         flush: function() {},
                         processChunk: function(s) {
                             this.push(s)
                         },
-                        withStreamInfo: function(s, D) {
-                            return this.extraStreamInfo[s] = D, this.mergeStreamInfo(), this
+                        withStreamInfo: function(s, i) {
+                            return this.extraStreamInfo[s] = i, this.mergeStreamInfo(), this
                         },
                         mergeStreamInfo: function() {
                             for (var s in this.extraStreamInfo) Object.prototype.hasOwnProperty.call(this.extraStreamInfo, s) && (this.streamInfo[s] = this.extraStreamInfo[s])
                         },
                         lock: function() {
                             if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
                             this.isLocked = !0, this.previous && this.previous.lock()
@@ -5602,15 +5645,15 @@
                             return this.previous ? this.previous + " -> " + s : s
                         }
                     }, o.exports = E
                 }, {}],
                 29: [function(g, o, t) {
                     var E = g("../utils"),
                         s = g("./ConvertWorker"),
-                        D = g("./GenericWorker"),
+                        i = g("./GenericWorker"),
                         h = g("../base64"),
                         C = g("../support"),
                         r = g("../external"),
                         n = null;
                     if (C.nodestream) try {
                         n = g("../nodejs/NodejsStreamOutputAdapter")
                     } catch {}
@@ -5673,15 +5716,15 @@
                                 break;
                             case "base64":
                                 y = "string"
                         }
                         try {
                             this._internalType = y, this._outputType = a, this._mimeType = G, E.checkSupport(y), this._worker = N.pipe(new s(y)), N.lock()
                         } catch (c) {
-                            this._worker = new D("error"), this._worker.error(c)
+                            this._worker = new i("error"), this._worker.error(c)
                         }
                     }
                     R.prototype = {
                         accumulate: function(N) {
                             return M(this, N)
                         },
                         on: function(N, a) {
@@ -5736,26 +5779,26 @@
                     } catch {
                         t.nodestream = !1
                     }
                 }, {
                     "readable-stream": 16
                 }],
                 31: [function(g, o, t) {
-                    for (var E = g("./utils"), s = g("./support"), D = g("./nodejsUtils"), h = g("./stream/GenericWorker"), C = new Array(256), r = 0; r < 256; r++) C[r] = 252 <= r ? 6 : 248 <= r ? 5 : 240 <= r ? 4 : 224 <= r ? 3 : 192 <= r ? 2 : 1;
+                    for (var E = g("./utils"), s = g("./support"), i = g("./nodejsUtils"), h = g("./stream/GenericWorker"), C = new Array(256), r = 0; r < 256; r++) C[r] = 252 <= r ? 6 : 248 <= r ? 5 : 240 <= r ? 4 : 224 <= r ? 3 : 192 <= r ? 2 : 1;
                     C[254] = C[254] = 1;
 
                     function n() {
                         h.call(this, "utf-8 decode"), this.leftOver = null
                     }
 
                     function M() {
                         h.call(this, "utf-8 encode")
                     }
                     t.utf8encode = function(R) {
-                        return s.nodebuffer ? D.newBufferFrom(R, "utf-8") : function(N) {
+                        return s.nodebuffer ? i.newBufferFrom(R, "utf-8") : function(N) {
                             var a, G, y, c, k, H = N.length,
                                 l = 0;
                             for (c = 0; c < H; c++)(64512 & (G = N.charCodeAt(c))) == 55296 && c + 1 < H && (64512 & (y = N.charCodeAt(c + 1))) == 56320 && (G = 65536 + (G - 55296 << 10) + (y - 56320), c++), l += G < 128 ? 1 : G < 2048 ? 2 : G < 65536 ? 3 : 4;
                             for (a = s.uint8array ? new Uint8Array(l) : new Array(l), c = k = 0; k < l; c++)(64512 & (G = N.charCodeAt(c))) == 55296 && c + 1 < H && (64512 & (y = N.charCodeAt(c + 1))) == 56320 && (G = 65536 + (G - 55296 << 10) + (y - 56320), c++), G < 128 ? a[k++] = G : (G < 2048 ? a[k++] = 192 | G >>> 6 : (G < 65536 ? a[k++] = 224 | G >>> 12 : (a[k++] = 240 | G >>> 18, a[k++] = 128 | G >>> 12 & 63), a[k++] = 128 | G >>> 6 & 63), a[k++] = 128 | 63 & G);
                             return a
                         }(R)
                     }, t.utf8decode = function(R) {
@@ -5806,15 +5849,15 @@
                     "./stream/GenericWorker": 28,
                     "./support": 30,
                     "./utils": 32
                 }],
                 32: [function(g, o, t) {
                     var E = g("./support"),
                         s = g("./base64"),
-                        D = g("./nodejsUtils"),
+                        i = g("./nodejsUtils"),
                         h = g("./external");
 
                     function C(a) {
                         return a
                     }
 
                     function r(a, G) {
@@ -5855,15 +5898,15 @@
                                     return E.uint8array && String.fromCharCode.apply(null, new Uint8Array(1)).length === 1
                                 } catch {
                                     return !1
                                 }
                             }(),
                             nodebuffer: function() {
                                 try {
-                                    return E.nodebuffer && String.fromCharCode.apply(null, D.allocBuffer(1)).length === 1
+                                    return E.nodebuffer && String.fromCharCode.apply(null, i.allocBuffer(1)).length === 1
                                 } catch {
                                     return !1
                                 }
                             }()
                         }
                     };
 
@@ -5894,53 +5937,53 @@
                         arraybuffer: function(a) {
                             return N.string.uint8array(a).buffer
                         },
                         uint8array: function(a) {
                             return r(a, new Uint8Array(a.length))
                         },
                         nodebuffer: function(a) {
-                            return r(a, D.allocBuffer(a.length))
+                            return r(a, i.allocBuffer(a.length))
                         }
                     }, N.array = {
                         string: M,
                         array: C,
                         arraybuffer: function(a) {
                             return new Uint8Array(a).buffer
                         },
                         uint8array: function(a) {
                             return new Uint8Array(a)
                         },
                         nodebuffer: function(a) {
-                            return D.newBufferFrom(a)
+                            return i.newBufferFrom(a)
                         }
                     }, N.arraybuffer = {
                         string: function(a) {
                             return M(new Uint8Array(a))
                         },
                         array: function(a) {
                             return R(new Uint8Array(a), new Array(a.byteLength))
                         },
                         arraybuffer: C,
                         uint8array: function(a) {
                             return new Uint8Array(a)
                         },
                         nodebuffer: function(a) {
-                            return D.newBufferFrom(new Uint8Array(a))
+                            return i.newBufferFrom(new Uint8Array(a))
                         }
                     }, N.uint8array = {
                         string: M,
                         array: function(a) {
                             return R(a, new Array(a.length))
                         },
                         arraybuffer: function(a) {
                             return a.buffer
                         },
                         uint8array: C,
                         nodebuffer: function(a) {
-                            return D.newBufferFrom(a)
+                            return i.newBufferFrom(a)
                         }
                     }, N.nodebuffer = {
                         string: M,
                         array: function(a) {
                             return R(a, new Array(a.length))
                         },
                         arraybuffer: function(a) {
@@ -5958,15 +6001,15 @@
                     }, t.resolve = function(a) {
                         for (var G = a.split("/"), y = [], c = 0; c < G.length; c++) {
                             var k = G[c];
                             k === "." || k === "" && c !== 0 && c !== G.length - 1 || (k === ".." ? y.pop() : y.push(k))
                         }
                         return y.join("/")
                     }, t.getTypeOf = function(a) {
-                        return typeof a == "string" ? "string" : Object.prototype.toString.call(a) === "[object Array]" ? "array" : E.nodebuffer && D.isBuffer(a) ? "nodebuffer" : E.uint8array && a instanceof Uint8Array ? "uint8array" : E.arraybuffer && a instanceof ArrayBuffer ? "arraybuffer" : void 0
+                        return typeof a == "string" ? "string" : Object.prototype.toString.call(a) === "[object Array]" ? "array" : E.nodebuffer && i.isBuffer(a) ? "nodebuffer" : E.uint8array && a instanceof Uint8Array ? "uint8array" : E.arraybuffer && a instanceof ArrayBuffer ? "arraybuffer" : void 0
                     }, t.checkSupport = function(a) {
                         if (!E[a.toLowerCase()]) throw new Error(a + " is not supported by this platform")
                     }, t.MAX_VALUE_16BITS = 65535, t.MAX_VALUE_32BITS = -1, t.pretty = function(a) {
                         var G, y, c = "";
                         for (y = 0; y < (a || "").length; y++) c += "\\x" + ((G = a.charCodeAt(y)) < 16 ? "0" : "") + G.toString(16).toUpperCase();
                         return c
                     }, t.delay = function(a, G, y) {
@@ -6004,15 +6047,15 @@
                     "./nodejsUtils": 14,
                     "./support": 30,
                     setimmediate: 54
                 }],
                 33: [function(g, o, t) {
                     var E = g("./reader/readerFor"),
                         s = g("./utils"),
-                        D = g("./signature"),
+                        i = g("./signature"),
                         h = g("./zipEntry"),
                         C = g("./support");
 
                     function r(n) {
                         this.files = [], this.loadOptions = n
                     }
                     r.prototype = {
@@ -6045,37 +6088,37 @@
                             }
                         },
                         readBlockZip64EndOfCentralLocator: function() {
                             if (this.diskWithZip64CentralDirStart = this.reader.readInt(4), this.relativeOffsetEndOfZip64CentralDir = this.reader.readInt(8), this.disksCount = this.reader.readInt(4), 1 < this.disksCount) throw new Error("Multi-volumes zip are not supported")
                         },
                         readLocalFiles: function() {
                             var n, M;
-                            for (n = 0; n < this.files.length; n++) M = this.files[n], this.reader.setIndex(M.localHeaderOffset), this.checkSignature(D.LOCAL_FILE_HEADER), M.readLocalPart(this.reader), M.handleUTF8(), M.processAttributes()
+                            for (n = 0; n < this.files.length; n++) M = this.files[n], this.reader.setIndex(M.localHeaderOffset), this.checkSignature(i.LOCAL_FILE_HEADER), M.readLocalPart(this.reader), M.handleUTF8(), M.processAttributes()
                         },
                         readCentralDir: function() {
                             var n;
-                            for (this.reader.setIndex(this.centralDirOffset); this.reader.readAndCheckSignature(D.CENTRAL_FILE_HEADER);)(n = new h({
+                            for (this.reader.setIndex(this.centralDirOffset); this.reader.readAndCheckSignature(i.CENTRAL_FILE_HEADER);)(n = new h({
                                 zip64: this.zip64
                             }, this.loadOptions)).readCentralPart(this.reader), this.files.push(n);
                             if (this.centralDirRecords !== this.files.length && this.centralDirRecords !== 0 && this.files.length === 0) throw new Error("Corrupted zip or bug: expected " + this.centralDirRecords + " records in central dir, got " + this.files.length)
                         },
                         readEndOfCentral: function() {
-                            var n = this.reader.lastIndexOfSignature(D.CENTRAL_DIRECTORY_END);
-                            if (n < 0) throw this.isSignature(0, D.LOCAL_FILE_HEADER) ? new Error("Corrupted zip: can't find end of central directory") : new Error("Can't find end of central directory : is this a zip file ? If it is, see https://stuk.github.io/jszip/documentation/howto/read_zip.html");
+                            var n = this.reader.lastIndexOfSignature(i.CENTRAL_DIRECTORY_END);
+                            if (n < 0) throw this.isSignature(0, i.LOCAL_FILE_HEADER) ? new Error("Corrupted zip: can't find end of central directory") : new Error("Can't find end of central directory : is this a zip file ? If it is, see https://stuk.github.io/jszip/documentation/howto/read_zip.html");
                             this.reader.setIndex(n);
                             var M = n;
-                            if (this.checkSignature(D.CENTRAL_DIRECTORY_END), this.readBlockEndOfCentral(), this.diskNumber === s.MAX_VALUE_16BITS || this.diskWithCentralDirStart === s.MAX_VALUE_16BITS || this.centralDirRecordsOnThisDisk === s.MAX_VALUE_16BITS || this.centralDirRecords === s.MAX_VALUE_16BITS || this.centralDirSize === s.MAX_VALUE_32BITS || this.centralDirOffset === s.MAX_VALUE_32BITS) {
-                                if (this.zip64 = !0, (n = this.reader.lastIndexOfSignature(D.ZIP64_CENTRAL_DIRECTORY_LOCATOR)) < 0) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory locator");
-                                if (this.reader.setIndex(n), this.checkSignature(D.ZIP64_CENTRAL_DIRECTORY_LOCATOR), this.readBlockZip64EndOfCentralLocator(), !this.isSignature(this.relativeOffsetEndOfZip64CentralDir, D.ZIP64_CENTRAL_DIRECTORY_END) && (this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(D.ZIP64_CENTRAL_DIRECTORY_END), this.relativeOffsetEndOfZip64CentralDir < 0)) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory");
-                                this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir), this.checkSignature(D.ZIP64_CENTRAL_DIRECTORY_END), this.readBlockZip64EndOfCentral()
+                            if (this.checkSignature(i.CENTRAL_DIRECTORY_END), this.readBlockEndOfCentral(), this.diskNumber === s.MAX_VALUE_16BITS || this.diskWithCentralDirStart === s.MAX_VALUE_16BITS || this.centralDirRecordsOnThisDisk === s.MAX_VALUE_16BITS || this.centralDirRecords === s.MAX_VALUE_16BITS || this.centralDirSize === s.MAX_VALUE_32BITS || this.centralDirOffset === s.MAX_VALUE_32BITS) {
+                                if (this.zip64 = !0, (n = this.reader.lastIndexOfSignature(i.ZIP64_CENTRAL_DIRECTORY_LOCATOR)) < 0) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory locator");
+                                if (this.reader.setIndex(n), this.checkSignature(i.ZIP64_CENTRAL_DIRECTORY_LOCATOR), this.readBlockZip64EndOfCentralLocator(), !this.isSignature(this.relativeOffsetEndOfZip64CentralDir, i.ZIP64_CENTRAL_DIRECTORY_END) && (this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(i.ZIP64_CENTRAL_DIRECTORY_END), this.relativeOffsetEndOfZip64CentralDir < 0)) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory");
+                                this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir), this.checkSignature(i.ZIP64_CENTRAL_DIRECTORY_END), this.readBlockZip64EndOfCentral()
                             }
                             var R = this.centralDirOffset + this.centralDirSize;
                             this.zip64 && (R += 20, R += 12 + this.zip64EndOfCentralSize);
                             var N = M - R;
-                            if (0 < N) this.isSignature(M, D.CENTRAL_FILE_HEADER) || (this.reader.zero = N);
+                            if (0 < N) this.isSignature(M, i.CENTRAL_FILE_HEADER) || (this.reader.zero = N);
                             else if (N < 0) throw new Error("Corrupted zip: missing " + Math.abs(N) + " bytes.")
                         },
                         prepareReader: function(n) {
                             this.reader = E(n)
                         },
                         load: function(n) {
                             this.prepareReader(n), this.readEndOfCentral(), this.readCentralDir(), this.readLocalFiles()
@@ -6087,15 +6130,15 @@
                     "./support": 30,
                     "./utils": 32,
                     "./zipEntry": 34
                 }],
                 34: [function(g, o, t) {
                     var E = g("./reader/readerFor"),
                         s = g("./utils"),
-                        D = g("./compressedObject"),
+                        i = g("./compressedObject"),
                         h = g("./crc32"),
                         C = g("./utf8"),
                         r = g("./compressions"),
                         n = g("./support");
 
                     function M(R, N) {
                         this.options = R, this.loadOptions = N
@@ -6111,15 +6154,15 @@
                             var N, a;
                             if (R.skip(22), this.fileNameLength = R.readInt(2), a = R.readInt(2), this.fileName = R.readData(this.fileNameLength), R.skip(a), this.compressedSize === -1 || this.uncompressedSize === -1) throw new Error("Bug or corrupted zip : didn't get enough information from the central directory (compressedSize === -1 || uncompressedSize === -1)");
                             if ((N = function(G) {
                                     for (var y in r)
                                         if (Object.prototype.hasOwnProperty.call(r, y) && r[y].magic === G) return r[y];
                                     return null
                                 }(this.compressionMethod)) === null) throw new Error("Corrupted zip : compression " + s.pretty(this.compressionMethod) + " unknown (inner file : " + s.transformTo("string", this.fileName) + ")");
-                            this.decompressed = new D(this.compressedSize, this.uncompressedSize, this.crc32, N, R.readData(this.compressedSize))
+                            this.decompressed = new i(this.compressedSize, this.uncompressedSize, this.crc32, N, R.readData(this.compressedSize))
                         },
                         readCentralPart: function(R) {
                             this.versionMadeBy = R.readInt(2), R.skip(2), this.bitFlag = R.readInt(2), this.compressionMethod = R.readString(2), this.date = R.readDate(), this.crc32 = R.readInt(4), this.compressedSize = R.readInt(4), this.uncompressedSize = R.readInt(4);
                             var N = R.readInt(2);
                             if (this.extraFieldsLength = R.readInt(2), this.fileCommentLength = R.readInt(2), this.diskNumberStart = R.readInt(2), this.internalFileAttributes = R.readInt(2), this.externalFileAttributes = R.readInt(4), this.localHeaderOffset = R.readInt(4), this.isEncrypted()) throw new Error("Encrypted zip are not supported");
                             R.skip(N), this.readExtraFields(R), this.parseZIP64ExtraField(R), this.fileComment = R.readData(this.fileCommentLength)
                         },
@@ -6191,15 +6234,15 @@
                     function E(N, a, G) {
                         this.name = N, this.dir = G.dir, this.date = G.date, this.comment = G.comment, this.unixPermissions = G.unixPermissions, this.dosPermissions = G.dosPermissions, this._data = a, this._dataBinary = G.binary, this.options = {
                             compression: G.compression,
                             compressionOptions: G.compressionOptions
                         }
                     }
                     var s = g("./stream/StreamHelper"),
-                        D = g("./stream/DataWorker"),
+                        i = g("./stream/DataWorker"),
                         h = g("./utf8"),
                         C = g("./compressedObject"),
                         r = g("./stream/GenericWorker");
                     E.prototype = {
                         internalStream: function(N) {
                             var a = null,
                                 G = "string";
@@ -6222,15 +6265,15 @@
                         },
                         _compressWorker: function(N, a) {
                             if (this._data instanceof C && this._data.compression.magic === N.magic) return this._data.getCompressedWorker();
                             var G = this._decompressWorker();
                             return this._dataBinary || (G = G.pipe(new h.Utf8EncodeWorker)), C.createWorkerFrom(G, N, a)
                         },
                         _decompressWorker: function() {
-                            return this._data instanceof C ? this._data.getContentWorker() : this._data instanceof r ? this._data : new D(this._data)
+                            return this._data instanceof C ? this._data.getContentWorker() : this._data instanceof r ? this._data : new i(this._data)
                         }
                     };
                     for (var n = ["asText", "asBinary", "asNodeBuffer", "asUint8Array", "asArrayBuffer"], M = function() {
                             throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
                         }, R = 0; R < n.length; R++) E.prototype[n[R]] = M;
                     o.exports = E
                 }, {
@@ -6238,15 +6281,15 @@
                     "./stream/DataWorker": 27,
                     "./stream/GenericWorker": 28,
                     "./stream/StreamHelper": 29,
                     "./utf8": 31
                 }],
                 36: [function(g, o, t) {
                     (function(E) {
-                        var s, D, h = E.MutationObserver || E.WebKitMutationObserver;
+                        var s, i, h = E.MutationObserver || E.WebKitMutationObserver;
                         if (h) {
                             var C = 0,
                                 r = new h(N),
                                 n = E.document.createTextNode("");
                             r.observe(n, {
                                 characterData: !0
                             }), s = function() {
@@ -6266,31 +6309,31 @@
                                 M.port2.postMessage(0)
                             }
                         }
                         var R = [];
 
                         function N() {
                             var a, G;
-                            D = !0;
+                            i = !0;
                             for (var y = R.length; y;) {
                                 for (G = R, R = [], a = -1; ++a < y;) G[a]();
                                 y = R.length
                             }
-                            D = !1
+                            i = !1
                         }
                         o.exports = function(a) {
-                            R.push(a) !== 1 || D || s()
+                            R.push(a) !== 1 || i || s()
                         }
-                    }).call(this, typeof OI < "u" ? OI : typeof self < "u" ? self : typeof window < "u" ? window : {})
+                    }).call(this, typeof XI < "u" ? XI : typeof self < "u" ? self : typeof window < "u" ? window : {})
                 }, {}],
                 37: [function(g, o, t) {
                     var E = g("immediate");
 
                     function s() {}
-                    var D = {},
+                    var i = {},
                         h = ["REJECTED"],
                         C = ["FULFILLED"],
                         r = ["PENDING"];
 
                     function n(y) {
                         if (typeof y != "function") throw new TypeError("resolver must be a function");
                         this.state = r, this.queue = [], this.outcome = void 0, y !== s && a(this, y)
@@ -6302,36 +6345,36 @@
 
                     function R(y, c, k) {
                         E(function() {
                             var H;
                             try {
                                 H = c(k)
                             } catch (l) {
-                                return D.reject(y, l)
+                                return i.reject(y, l)
                             }
-                            H === y ? D.reject(y, new TypeError("Cannot resolve promise with itself")) : D.resolve(y, H)
+                            H === y ? i.reject(y, new TypeError("Cannot resolve promise with itself")) : i.resolve(y, H)
                         })
                     }
 
                     function N(y) {
                         var c = y && y.then;
                         if (y && (typeof y == "object" || typeof y == "function") && typeof c == "function") return function() {
                             c.apply(y, arguments)
                         }
                     }
 
                     function a(y, c) {
                         var k = !1;
 
                         function H(p) {
-                            k || (k = !0, D.reject(y, p))
+                            k || (k = !0, i.reject(y, p))
                         }
 
                         function l(p) {
-                            k || (k = !0, D.resolve(y, p))
+                            k || (k = !0, i.resolve(y, p))
                         }
                         var T = G(function() {
                             c(l, H)
                         });
                         T.status === "error" && H(T.value)
                     }
 
@@ -6358,66 +6401,66 @@
                     }, n.prototype.catch = function(y) {
                         return this.then(null, y)
                     }, n.prototype.then = function(y, c) {
                         if (typeof y != "function" && this.state === C || typeof c != "function" && this.state === h) return this;
                         var k = new this.constructor(s);
                         return this.state !== r ? R(k, this.state === C ? y : c, this.outcome) : this.queue.push(new M(k, y, c)), k
                     }, M.prototype.callFulfilled = function(y) {
-                        D.resolve(this.promise, y)
+                        i.resolve(this.promise, y)
                     }, M.prototype.otherCallFulfilled = function(y) {
                         R(this.promise, this.onFulfilled, y)
                     }, M.prototype.callRejected = function(y) {
-                        D.reject(this.promise, y)
+                        i.reject(this.promise, y)
                     }, M.prototype.otherCallRejected = function(y) {
                         R(this.promise, this.onRejected, y)
-                    }, D.resolve = function(y, c) {
+                    }, i.resolve = function(y, c) {
                         var k = G(N, c);
-                        if (k.status === "error") return D.reject(y, k.value);
+                        if (k.status === "error") return i.reject(y, k.value);
                         var H = k.value;
                         if (H) a(y, H);
                         else {
                             y.state = C, y.outcome = c;
                             for (var l = -1, T = y.queue.length; ++l < T;) y.queue[l].callFulfilled(c)
                         }
                         return y
-                    }, D.reject = function(y, c) {
+                    }, i.reject = function(y, c) {
                         y.state = h, y.outcome = c;
                         for (var k = -1, H = y.queue.length; ++k < H;) y.queue[k].callRejected(c);
                         return y
                     }, n.resolve = function(y) {
-                        return y instanceof this ? y : D.resolve(new this(s), y)
+                        return y instanceof this ? y : i.resolve(new this(s), y)
                     }, n.reject = function(y) {
                         var c = new this(s);
-                        return D.reject(c, y)
+                        return i.reject(c, y)
                     }, n.all = function(y) {
                         var c = this;
                         if (Object.prototype.toString.call(y) !== "[object Array]") return this.reject(new TypeError("must be an array"));
                         var k = y.length,
                             H = !1;
                         if (!k) return this.resolve([]);
                         for (var l = new Array(k), T = 0, p = -1, j = new this(s); ++p < k;) b(y[p], p);
                         return j;
 
                         function b(gA, oA) {
                             c.resolve(gA).then(function(J) {
-                                l[oA] = J, ++T !== k || H || (H = !0, D.resolve(j, l))
+                                l[oA] = J, ++T !== k || H || (H = !0, i.resolve(j, l))
                             }, function(J) {
-                                H || (H = !0, D.reject(j, J))
+                                H || (H = !0, i.reject(j, J))
                             })
                         }
                     }, n.race = function(y) {
                         var c = this;
                         if (Object.prototype.toString.call(y) !== "[object Array]") return this.reject(new TypeError("must be an array"));
                         var k = y.length,
                             H = !1;
                         if (!k) return this.resolve([]);
                         for (var l = -1, T = new this(s); ++l < k;) p = y[l], c.resolve(p).then(function(j) {
-                            H || (H = !0, D.resolve(T, j))
+                            H || (H = !0, i.resolve(T, j))
                         }, function(j) {
-                            H || (H = !0, D.reject(T, j))
+                            H || (H = !0, i.reject(T, j))
                         });
                         var p;
                         return T
                     }
                 }, {
                     immediate: 36
                 }],
@@ -6429,15 +6472,15 @@
                     "./lib/inflate": 40,
                     "./lib/utils/common": 41,
                     "./lib/zlib/constants": 44
                 }],
                 39: [function(g, o, t) {
                     var E = g("./zlib/deflate"),
                         s = g("./utils/common"),
-                        D = g("./utils/strings"),
+                        i = g("./utils/strings"),
                         h = g("./zlib/messages"),
                         C = g("./zlib/zstream"),
                         r = Object.prototype.toString,
                         n = 0,
                         M = -1,
                         R = 0,
                         N = 8;
@@ -6455,32 +6498,32 @@
                         }, y || {});
                         var c = this.options;
                         c.raw && 0 < c.windowBits ? c.windowBits = -c.windowBits : c.gzip && 0 < c.windowBits && c.windowBits < 16 && (c.windowBits += 16), this.err = 0, this.msg = "", this.ended = !1, this.chunks = [], this.strm = new C, this.strm.avail_out = 0;
                         var k = E.deflateInit2(this.strm, c.level, c.method, c.windowBits, c.memLevel, c.strategy);
                         if (k !== n) throw new Error(h[k]);
                         if (c.header && E.deflateSetHeader(this.strm, c.header), c.dictionary) {
                             var H;
-                            if (H = typeof c.dictionary == "string" ? D.string2buf(c.dictionary) : r.call(c.dictionary) === "[object ArrayBuffer]" ? new Uint8Array(c.dictionary) : c.dictionary, (k = E.deflateSetDictionary(this.strm, H)) !== n) throw new Error(h[k]);
+                            if (H = typeof c.dictionary == "string" ? i.string2buf(c.dictionary) : r.call(c.dictionary) === "[object ArrayBuffer]" ? new Uint8Array(c.dictionary) : c.dictionary, (k = E.deflateSetDictionary(this.strm, H)) !== n) throw new Error(h[k]);
                             this._dict_set = !0
                         }
                     }
 
                     function G(y, c) {
                         var k = new a(c);
                         if (k.push(y, !0), k.err) throw k.msg || h[k.err];
                         return k.result
                     }
                     a.prototype.push = function(y, c) {
                         var k, H, l = this.strm,
                             T = this.options.chunkSize;
                         if (this.ended) return !1;
-                        H = c === ~~c ? c : c === !0 ? 4 : 0, typeof y == "string" ? l.input = D.string2buf(y) : r.call(y) === "[object ArrayBuffer]" ? l.input = new Uint8Array(y) : l.input = y, l.next_in = 0, l.avail_in = l.input.length;
+                        H = c === ~~c ? c : c === !0 ? 4 : 0, typeof y == "string" ? l.input = i.string2buf(y) : r.call(y) === "[object ArrayBuffer]" ? l.input = new Uint8Array(y) : l.input = y, l.next_in = 0, l.avail_in = l.input.length;
                         do {
                             if (l.avail_out === 0 && (l.output = new s.Buf8(T), l.next_out = 0, l.avail_out = T), (k = E.deflate(l, H)) !== 1 && k !== n) return this.onEnd(k), !(this.ended = !0);
-                            l.avail_out !== 0 && (l.avail_in !== 0 || H !== 4 && H !== 2) || (this.options.to === "string" ? this.onData(D.buf2binstring(s.shrinkBuf(l.output, l.next_out))) : this.onData(s.shrinkBuf(l.output, l.next_out)))
+                            l.avail_out !== 0 && (l.avail_in !== 0 || H !== 4 && H !== 2) || (this.options.to === "string" ? this.onData(i.buf2binstring(s.shrinkBuf(l.output, l.next_out))) : this.onData(s.shrinkBuf(l.output, l.next_out)))
                         } while ((0 < l.avail_in || l.avail_out === 0) && k !== 1);
                         return H === 4 ? (k = E.deflateEnd(this.strm), this.onEnd(k), this.ended = !0, k === n) : H !== 2 || (this.onEnd(n), !(l.avail_out = 0))
                     }, a.prototype.onData = function(y) {
                         this.chunks.push(y)
                     }, a.prototype.onEnd = function(y) {
                         y === n && (this.options.to === "string" ? this.result = this.chunks.join("") : this.result = s.flattenChunks(this.chunks)), this.chunks = [], this.err = y, this.msg = this.strm.msg
                     }, t.Deflate = a, t.deflate = G, t.deflateRaw = function(y, c) {
@@ -6494,15 +6537,15 @@
                     "./zlib/deflate": 46,
                     "./zlib/messages": 51,
                     "./zlib/zstream": 53
                 }],
                 40: [function(g, o, t) {
                     var E = g("./zlib/inflate"),
                         s = g("./utils/common"),
-                        D = g("./utils/strings"),
+                        i = g("./utils/strings"),
                         h = g("./zlib/constants"),
                         C = g("./zlib/messages"),
                         r = g("./zlib/zstream"),
                         n = g("./zlib/gzheader"),
                         M = Object.prototype.toString;
 
                     function R(a) {
@@ -6526,18 +6569,18 @@
                     }
                     R.prototype.push = function(a, G) {
                         var y, c, k, H, l, T, p = this.strm,
                             j = this.options.chunkSize,
                             b = this.options.dictionary,
                             gA = !1;
                         if (this.ended) return !1;
-                        c = G === ~~G ? G : G === !0 ? h.Z_FINISH : h.Z_NO_FLUSH, typeof a == "string" ? p.input = D.binstring2buf(a) : M.call(a) === "[object ArrayBuffer]" ? p.input = new Uint8Array(a) : p.input = a, p.next_in = 0, p.avail_in = p.input.length;
+                        c = G === ~~G ? G : G === !0 ? h.Z_FINISH : h.Z_NO_FLUSH, typeof a == "string" ? p.input = i.binstring2buf(a) : M.call(a) === "[object ArrayBuffer]" ? p.input = new Uint8Array(a) : p.input = a, p.next_in = 0, p.avail_in = p.input.length;
                         do {
-                            if (p.avail_out === 0 && (p.output = new s.Buf8(j), p.next_out = 0, p.avail_out = j), (y = E.inflate(p, h.Z_NO_FLUSH)) === h.Z_NEED_DICT && b && (T = typeof b == "string" ? D.string2buf(b) : M.call(b) === "[object ArrayBuffer]" ? new Uint8Array(b) : b, y = E.inflateSetDictionary(this.strm, T)), y === h.Z_BUF_ERROR && gA === !0 && (y = h.Z_OK, gA = !1), y !== h.Z_STREAM_END && y !== h.Z_OK) return this.onEnd(y), !(this.ended = !0);
-                            p.next_out && (p.avail_out !== 0 && y !== h.Z_STREAM_END && (p.avail_in !== 0 || c !== h.Z_FINISH && c !== h.Z_SYNC_FLUSH) || (this.options.to === "string" ? (k = D.utf8border(p.output, p.next_out), H = p.next_out - k, l = D.buf2string(p.output, k), p.next_out = H, p.avail_out = j - H, H && s.arraySet(p.output, p.output, k, H, 0), this.onData(l)) : this.onData(s.shrinkBuf(p.output, p.next_out)))), p.avail_in === 0 && p.avail_out === 0 && (gA = !0)
+                            if (p.avail_out === 0 && (p.output = new s.Buf8(j), p.next_out = 0, p.avail_out = j), (y = E.inflate(p, h.Z_NO_FLUSH)) === h.Z_NEED_DICT && b && (T = typeof b == "string" ? i.string2buf(b) : M.call(b) === "[object ArrayBuffer]" ? new Uint8Array(b) : b, y = E.inflateSetDictionary(this.strm, T)), y === h.Z_BUF_ERROR && gA === !0 && (y = h.Z_OK, gA = !1), y !== h.Z_STREAM_END && y !== h.Z_OK) return this.onEnd(y), !(this.ended = !0);
+                            p.next_out && (p.avail_out !== 0 && y !== h.Z_STREAM_END && (p.avail_in !== 0 || c !== h.Z_FINISH && c !== h.Z_SYNC_FLUSH) || (this.options.to === "string" ? (k = i.utf8border(p.output, p.next_out), H = p.next_out - k, l = i.buf2string(p.output, k), p.next_out = H, p.avail_out = j - H, H && s.arraySet(p.output, p.output, k, H, 0), this.onData(l)) : this.onData(s.shrinkBuf(p.output, p.next_out)))), p.avail_in === 0 && p.avail_out === 0 && (gA = !0)
                         } while ((0 < p.avail_in || p.avail_out === 0) && y !== h.Z_STREAM_END);
                         return y === h.Z_STREAM_END && (c = h.Z_FINISH), c === h.Z_FINISH ? (y = E.inflateEnd(this.strm), this.onEnd(y), this.ended = !0, y === h.Z_OK) : c !== h.Z_SYNC_FLUSH || (this.onEnd(h.Z_OK), !(p.avail_out = 0))
                     }, R.prototype.onData = function(a) {
                         this.chunks.push(a)
                     }, R.prototype.onEnd = function(a) {
                         a === h.Z_OK && (this.options.to === "string" ? this.result = this.chunks.join("") : this.result = s.flattenChunks(this.chunks)), this.chunks = [], this.err = a, this.msg = this.strm.msg
                     }, t.Inflate = R, t.inflate = N, t.inflateRaw = function(a, G) {
@@ -6575,44 +6618,44 @@
                             flattenChunks: function(h) {
                                 var C, r, n, M, R, N;
                                 for (C = n = 0, r = h.length; C < r; C++) n += h[C].length;
                                 for (N = new Uint8Array(n), C = M = 0, r = h.length; C < r; C++) R = h[C], N.set(R, M), M += R.length;
                                 return N
                             }
                         },
-                        D = {
+                        i = {
                             arraySet: function(h, C, r, n, M) {
                                 for (var R = 0; R < n; R++) h[M + R] = C[r + R]
                             },
                             flattenChunks: function(h) {
                                 return [].concat.apply([], h)
                             }
                         };
                     t.setTyped = function(h) {
-                        h ? (t.Buf8 = Uint8Array, t.Buf16 = Uint16Array, t.Buf32 = Int32Array, t.assign(t, s)) : (t.Buf8 = Array, t.Buf16 = Array, t.Buf32 = Array, t.assign(t, D))
+                        h ? (t.Buf8 = Uint8Array, t.Buf16 = Uint16Array, t.Buf32 = Int32Array, t.assign(t, s)) : (t.Buf8 = Array, t.Buf16 = Array, t.Buf32 = Array, t.assign(t, i))
                     }, t.setTyped(E)
                 }, {}],
                 42: [function(g, o, t) {
                     var E = g("./common"),
                         s = !0,
-                        D = !0;
+                        i = !0;
                     try {
                         String.fromCharCode.apply(null, [0])
                     } catch {
                         s = !1
                     }
                     try {
                         String.fromCharCode.apply(null, new Uint8Array(1))
                     } catch {
-                        D = !1
+                        i = !1
                     }
                     for (var h = new E.Buf8(256), C = 0; C < 256; C++) h[C] = 252 <= C ? 6 : 248 <= C ? 5 : 240 <= C ? 4 : 224 <= C ? 3 : 192 <= C ? 2 : 1;
 
                     function r(n, M) {
-                        if (M < 65537 && (n.subarray && D || !n.subarray && s)) return String.fromCharCode.apply(null, E.shrinkBuf(n, M));
+                        if (M < 65537 && (n.subarray && i || !n.subarray && s)) return String.fromCharCode.apply(null, E.shrinkBuf(n, M));
                         for (var R = "", N = 0; N < M; N++) R += String.fromCharCode(n[N]);
                         return R
                     }
                     h[254] = h[254] = 1, t.string2buf = function(n) {
                         var M, R, N, a, G, y = n.length,
                             c = 0;
                         for (a = 0; a < y; a++)(64512 & (R = n.charCodeAt(a))) == 55296 && a + 1 < y && (64512 & (N = n.charCodeAt(a + 1))) == 56320 && (R = 65536 + (R - 55296 << 10) + (N - 56320), a++), c += R < 128 ? 1 : R < 2048 ? 2 : R < 65536 ? 3 : 4;
@@ -6639,17 +6682,17 @@
                         for ((M = M || n.length) > n.length && (M = n.length), R = M - 1; 0 <= R && (192 & n[R]) == 128;) R--;
                         return R < 0 || R === 0 ? M : R + h[n[R]] > M ? R : M
                     }
                 }, {
                     "./common": 41
                 }],
                 43: [function(g, o, t) {
-                    o.exports = function(E, s, D, h) {
-                        for (var C = 65535 & E | 0, r = E >>> 16 & 65535 | 0, n = 0; D !== 0;) {
-                            for (D -= n = 2e3 < D ? 2e3 : D; r = r + (C = C + s[h++] | 0) | 0, --n;);
+                    o.exports = function(E, s, i, h) {
+                        for (var C = 65535 & E | 0, r = E >>> 16 & 65535 | 0, n = 0; i !== 0;) {
+                            for (i -= n = 2e3 < i ? 2e3 : i; r = r + (C = C + s[h++] | 0) | 0, --n;);
                             C %= 65521, r %= 65521
                         }
                         return C | r << 16 | 0
                     }
                 }, {}],
                 44: [function(g, o, t) {
                     o.exports = {
@@ -6680,32 +6723,32 @@
                         Z_TEXT: 1,
                         Z_UNKNOWN: 2,
                         Z_DEFLATED: 8
                     }
                 }, {}],
                 45: [function(g, o, t) {
                     var E = function() {
-                        for (var s, D = [], h = 0; h < 256; h++) {
+                        for (var s, i = [], h = 0; h < 256; h++) {
                             s = h;
                             for (var C = 0; C < 8; C++) s = 1 & s ? 3988292384 ^ s >>> 1 : s >>> 1;
-                            D[h] = s
+                            i[h] = s
                         }
-                        return D
+                        return i
                     }();
-                    o.exports = function(s, D, h, C) {
+                    o.exports = function(s, i, h, C) {
                         var r = E,
                             n = C + h;
                         s ^= -1;
-                        for (var M = C; M < n; M++) s = s >>> 8 ^ r[255 & (s ^ D[M])];
+                        for (var M = C; M < n; M++) s = s >>> 8 ^ r[255 & (s ^ i[M])];
                         return -1 ^ s
                     }
                 }, {}],
                 46: [function(g, o, t) {
                     var E, s = g("../utils/common"),
-                        D = g("./trees"),
+                        i = g("./trees"),
                         h = g("./adler32"),
                         C = g("./crc32"),
                         r = g("./messages"),
                         n = 0,
                         M = 4,
                         R = 0,
                         N = -2,
@@ -6725,242 +6768,242 @@
                         J = 42,
                         x = 113,
                         F = 1,
                         Z = 2,
                         iA = 3,
                         W = 4;
 
-                    function tA(i, X) {
-                        return i.msg = r[X], X
+                    function tA(D, X) {
+                        return D.msg = r[X], X
                     }
 
-                    function _(i) {
-                        return (i << 1) - (4 < i ? 9 : 0)
+                    function _(D) {
+                        return (D << 1) - (4 < D ? 9 : 0)
                     }
 
-                    function AA(i) {
-                        for (var X = i.length; 0 <= --X;) i[X] = 0
+                    function AA(D) {
+                        for (var X = D.length; 0 <= --X;) D[X] = 0
                     }
 
-                    function f(i) {
-                        var X = i.state,
+                    function f(D) {
+                        var X = D.state,
                             V = X.pending;
-                        V > i.avail_out && (V = i.avail_out), V !== 0 && (s.arraySet(i.output, X.pending_buf, X.pending_out, V, i.next_out), i.next_out += V, X.pending_out += V, i.total_out += V, i.avail_out -= V, X.pending -= V, X.pending === 0 && (X.pending_out = 0))
+                        V > D.avail_out && (V = D.avail_out), V !== 0 && (s.arraySet(D.output, X.pending_buf, X.pending_out, V, D.next_out), D.next_out += V, X.pending_out += V, D.total_out += V, D.avail_out -= V, X.pending -= V, X.pending === 0 && (X.pending_out = 0))
                     }
 
-                    function q(i, X) {
-                        D._tr_flush_block(i, 0 <= i.block_start ? i.block_start : -1, i.strstart - i.block_start, X), i.block_start = i.strstart, f(i.strm)
+                    function q(D, X) {
+                        i._tr_flush_block(D, 0 <= D.block_start ? D.block_start : -1, D.strstart - D.block_start, X), D.block_start = D.strstart, f(D.strm)
                     }
 
-                    function sA(i, X) {
-                        i.pending_buf[i.pending++] = X
+                    function sA(D, X) {
+                        D.pending_buf[D.pending++] = X
                     }
 
-                    function CA(i, X) {
-                        i.pending_buf[i.pending++] = X >>> 8 & 255, i.pending_buf[i.pending++] = 255 & X
+                    function CA(D, X) {
+                        D.pending_buf[D.pending++] = X >>> 8 & 255, D.pending_buf[D.pending++] = 255 & X
                     }
 
-                    function QA(i, X) {
-                        var V, L, U = i.max_chain_length,
-                            Y = i.strstart,
-                            z = i.prev_length,
-                            P = i.nice_match,
-                            u = i.strstart > i.w_size - oA ? i.strstart - (i.w_size - oA) : 0,
-                            IA = i.window,
-                            EA = i.w_mask,
-                            BA = i.prev,
-                            wA = i.strstart + gA,
+                    function QA(D, X) {
+                        var V, L, U = D.max_chain_length,
+                            Y = D.strstart,
+                            z = D.prev_length,
+                            P = D.nice_match,
+                            u = D.strstart > D.w_size - oA ? D.strstart - (D.w_size - oA) : 0,
+                            IA = D.window,
+                            EA = D.w_mask,
+                            BA = D.prev,
+                            wA = D.strstart + gA,
                             NA = IA[Y + z - 1],
                             RA = IA[Y + z];
-                        i.prev_length >= i.good_match && (U >>= 2), P > i.lookahead && (P = i.lookahead);
+                        D.prev_length >= D.good_match && (U >>= 2), P > D.lookahead && (P = D.lookahead);
                         do
                             if (IA[(V = X) + z] === RA && IA[V + z - 1] === NA && IA[V] === IA[Y] && IA[++V] === IA[Y + 1]) {
                                 Y += 2, V++;
                                 do; while (IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && IA[++Y] === IA[++V] && Y < wA);
                                 if (L = gA - (wA - Y), Y = wA - gA, z < L) {
-                                    if (i.match_start = X, P <= (z = L)) break;
+                                    if (D.match_start = X, P <= (z = L)) break;
                                     NA = IA[Y + z - 1], RA = IA[Y + z]
                                 }
                             } while ((X = BA[X & EA]) > u && --U != 0);
-                        return z <= i.lookahead ? z : i.lookahead
+                        return z <= D.lookahead ? z : D.lookahead
                     }
 
-                    function SA(i) {
-                        var X, V, L, U, Y, z, P, u, IA, EA, BA = i.w_size;
+                    function SA(D) {
+                        var X, V, L, U, Y, z, P, u, IA, EA, BA = D.w_size;
                         do {
-                            if (U = i.window_size - i.lookahead - i.strstart, i.strstart >= BA + (BA - oA)) {
-                                for (s.arraySet(i.window, i.window, BA, BA, 0), i.match_start -= BA, i.strstart -= BA, i.block_start -= BA, X = V = i.hash_size; L = i.head[--X], i.head[X] = BA <= L ? L - BA : 0, --V;);
-                                for (X = V = BA; L = i.prev[--X], i.prev[X] = BA <= L ? L - BA : 0, --V;);
+                            if (U = D.window_size - D.lookahead - D.strstart, D.strstart >= BA + (BA - oA)) {
+                                for (s.arraySet(D.window, D.window, BA, BA, 0), D.match_start -= BA, D.strstart -= BA, D.block_start -= BA, X = V = D.hash_size; L = D.head[--X], D.head[X] = BA <= L ? L - BA : 0, --V;);
+                                for (X = V = BA; L = D.prev[--X], D.prev[X] = BA <= L ? L - BA : 0, --V;);
                                 U += BA
                             }
-                            if (i.strm.avail_in === 0) break;
-                            if (z = i.strm, P = i.window, u = i.strstart + i.lookahead, IA = U, EA = void 0, EA = z.avail_in, IA < EA && (EA = IA), V = EA === 0 ? 0 : (z.avail_in -= EA, s.arraySet(P, z.input, z.next_in, EA, u), z.state.wrap === 1 ? z.adler = h(z.adler, P, EA, u) : z.state.wrap === 2 && (z.adler = C(z.adler, P, EA, u)), z.next_in += EA, z.total_in += EA, EA), i.lookahead += V, i.lookahead + i.insert >= b)
-                                for (Y = i.strstart - i.insert, i.ins_h = i.window[Y], i.ins_h = (i.ins_h << i.hash_shift ^ i.window[Y + 1]) & i.hash_mask; i.insert && (i.ins_h = (i.ins_h << i.hash_shift ^ i.window[Y + b - 1]) & i.hash_mask, i.prev[Y & i.w_mask] = i.head[i.ins_h], i.head[i.ins_h] = Y, Y++, i.insert--, !(i.lookahead + i.insert < b)););
-                        } while (i.lookahead < oA && i.strm.avail_in !== 0)
+                            if (D.strm.avail_in === 0) break;
+                            if (z = D.strm, P = D.window, u = D.strstart + D.lookahead, IA = U, EA = void 0, EA = z.avail_in, IA < EA && (EA = IA), V = EA === 0 ? 0 : (z.avail_in -= EA, s.arraySet(P, z.input, z.next_in, EA, u), z.state.wrap === 1 ? z.adler = h(z.adler, P, EA, u) : z.state.wrap === 2 && (z.adler = C(z.adler, P, EA, u)), z.next_in += EA, z.total_in += EA, EA), D.lookahead += V, D.lookahead + D.insert >= b)
+                                for (Y = D.strstart - D.insert, D.ins_h = D.window[Y], D.ins_h = (D.ins_h << D.hash_shift ^ D.window[Y + 1]) & D.hash_mask; D.insert && (D.ins_h = (D.ins_h << D.hash_shift ^ D.window[Y + b - 1]) & D.hash_mask, D.prev[Y & D.w_mask] = D.head[D.ins_h], D.head[D.ins_h] = Y, Y++, D.insert--, !(D.lookahead + D.insert < b)););
+                        } while (D.lookahead < oA && D.strm.avail_in !== 0)
                     }
 
-                    function YA(i, X) {
+                    function YA(D, X) {
                         for (var V, L;;) {
-                            if (i.lookahead < oA) {
-                                if (SA(i), i.lookahead < oA && X === n) return F;
-                                if (i.lookahead === 0) break
-                            }
-                            if (V = 0, i.lookahead >= b && (i.ins_h = (i.ins_h << i.hash_shift ^ i.window[i.strstart + b - 1]) & i.hash_mask, V = i.prev[i.strstart & i.w_mask] = i.head[i.ins_h], i.head[i.ins_h] = i.strstart), V !== 0 && i.strstart - V <= i.w_size - oA && (i.match_length = QA(i, V)), i.match_length >= b)
-                                if (L = D._tr_tally(i, i.strstart - i.match_start, i.match_length - b), i.lookahead -= i.match_length, i.match_length <= i.max_lazy_match && i.lookahead >= b) {
-                                    for (i.match_length--; i.strstart++, i.ins_h = (i.ins_h << i.hash_shift ^ i.window[i.strstart + b - 1]) & i.hash_mask, V = i.prev[i.strstart & i.w_mask] = i.head[i.ins_h], i.head[i.ins_h] = i.strstart, --i.match_length != 0;);
-                                    i.strstart++
-                                } else i.strstart += i.match_length, i.match_length = 0, i.ins_h = i.window[i.strstart], i.ins_h = (i.ins_h << i.hash_shift ^ i.window[i.strstart + 1]) & i.hash_mask;
-                            else L = D._tr_tally(i, 0, i.window[i.strstart]), i.lookahead--, i.strstart++;
-                            if (L && (q(i, !1), i.strm.avail_out === 0)) return F
+                            if (D.lookahead < oA) {
+                                if (SA(D), D.lookahead < oA && X === n) return F;
+                                if (D.lookahead === 0) break
+                            }
+                            if (V = 0, D.lookahead >= b && (D.ins_h = (D.ins_h << D.hash_shift ^ D.window[D.strstart + b - 1]) & D.hash_mask, V = D.prev[D.strstart & D.w_mask] = D.head[D.ins_h], D.head[D.ins_h] = D.strstart), V !== 0 && D.strstart - V <= D.w_size - oA && (D.match_length = QA(D, V)), D.match_length >= b)
+                                if (L = i._tr_tally(D, D.strstart - D.match_start, D.match_length - b), D.lookahead -= D.match_length, D.match_length <= D.max_lazy_match && D.lookahead >= b) {
+                                    for (D.match_length--; D.strstart++, D.ins_h = (D.ins_h << D.hash_shift ^ D.window[D.strstart + b - 1]) & D.hash_mask, V = D.prev[D.strstart & D.w_mask] = D.head[D.ins_h], D.head[D.ins_h] = D.strstart, --D.match_length != 0;);
+                                    D.strstart++
+                                } else D.strstart += D.match_length, D.match_length = 0, D.ins_h = D.window[D.strstart], D.ins_h = (D.ins_h << D.hash_shift ^ D.window[D.strstart + 1]) & D.hash_mask;
+                            else L = i._tr_tally(D, 0, D.window[D.strstart]), D.lookahead--, D.strstart++;
+                            if (L && (q(D, !1), D.strm.avail_out === 0)) return F
                         }
-                        return i.insert = i.strstart < b - 1 ? i.strstart : b - 1, X === M ? (q(i, !0), i.strm.avail_out === 0 ? iA : W) : i.last_lit && (q(i, !1), i.strm.avail_out === 0) ? F : Z
+                        return D.insert = D.strstart < b - 1 ? D.strstart : b - 1, X === M ? (q(D, !0), D.strm.avail_out === 0 ? iA : W) : D.last_lit && (q(D, !1), D.strm.avail_out === 0) ? F : Z
                     }
 
-                    function GA(i, X) {
+                    function GA(D, X) {
                         for (var V, L, U;;) {
-                            if (i.lookahead < oA) {
-                                if (SA(i), i.lookahead < oA && X === n) return F;
-                                if (i.lookahead === 0) break
-                            }
-                            if (V = 0, i.lookahead >= b && (i.ins_h = (i.ins_h << i.hash_shift ^ i.window[i.strstart + b - 1]) & i.hash_mask, V = i.prev[i.strstart & i.w_mask] = i.head[i.ins_h], i.head[i.ins_h] = i.strstart), i.prev_length = i.match_length, i.prev_match = i.match_start, i.match_length = b - 1, V !== 0 && i.prev_length < i.max_lazy_match && i.strstart - V <= i.w_size - oA && (i.match_length = QA(i, V), i.match_length <= 5 && (i.strategy === 1 || i.match_length === b && 4096 < i.strstart - i.match_start) && (i.match_length = b - 1)), i.prev_length >= b && i.match_length <= i.prev_length) {
-                                for (U = i.strstart + i.lookahead - b, L = D._tr_tally(i, i.strstart - 1 - i.prev_match, i.prev_length - b), i.lookahead -= i.prev_length - 1, i.prev_length -= 2; ++i.strstart <= U && (i.ins_h = (i.ins_h << i.hash_shift ^ i.window[i.strstart + b - 1]) & i.hash_mask, V = i.prev[i.strstart & i.w_mask] = i.head[i.ins_h], i.head[i.ins_h] = i.strstart), --i.prev_length != 0;);
-                                if (i.match_available = 0, i.match_length = b - 1, i.strstart++, L && (q(i, !1), i.strm.avail_out === 0)) return F
-                            } else if (i.match_available) {
-                                if ((L = D._tr_tally(i, 0, i.window[i.strstart - 1])) && q(i, !1), i.strstart++, i.lookahead--, i.strm.avail_out === 0) return F
-                            } else i.match_available = 1, i.strstart++, i.lookahead--
+                            if (D.lookahead < oA) {
+                                if (SA(D), D.lookahead < oA && X === n) return F;
+                                if (D.lookahead === 0) break
+                            }
+                            if (V = 0, D.lookahead >= b && (D.ins_h = (D.ins_h << D.hash_shift ^ D.window[D.strstart + b - 1]) & D.hash_mask, V = D.prev[D.strstart & D.w_mask] = D.head[D.ins_h], D.head[D.ins_h] = D.strstart), D.prev_length = D.match_length, D.prev_match = D.match_start, D.match_length = b - 1, V !== 0 && D.prev_length < D.max_lazy_match && D.strstart - V <= D.w_size - oA && (D.match_length = QA(D, V), D.match_length <= 5 && (D.strategy === 1 || D.match_length === b && 4096 < D.strstart - D.match_start) && (D.match_length = b - 1)), D.prev_length >= b && D.match_length <= D.prev_length) {
+                                for (U = D.strstart + D.lookahead - b, L = i._tr_tally(D, D.strstart - 1 - D.prev_match, D.prev_length - b), D.lookahead -= D.prev_length - 1, D.prev_length -= 2; ++D.strstart <= U && (D.ins_h = (D.ins_h << D.hash_shift ^ D.window[D.strstart + b - 1]) & D.hash_mask, V = D.prev[D.strstart & D.w_mask] = D.head[D.ins_h], D.head[D.ins_h] = D.strstart), --D.prev_length != 0;);
+                                if (D.match_available = 0, D.match_length = b - 1, D.strstart++, L && (q(D, !1), D.strm.avail_out === 0)) return F
+                            } else if (D.match_available) {
+                                if ((L = i._tr_tally(D, 0, D.window[D.strstart - 1])) && q(D, !1), D.strstart++, D.lookahead--, D.strm.avail_out === 0) return F
+                            } else D.match_available = 1, D.strstart++, D.lookahead--
                         }
-                        return i.match_available && (L = D._tr_tally(i, 0, i.window[i.strstart - 1]), i.match_available = 0), i.insert = i.strstart < b - 1 ? i.strstart : b - 1, X === M ? (q(i, !0), i.strm.avail_out === 0 ? iA : W) : i.last_lit && (q(i, !1), i.strm.avail_out === 0) ? F : Z
+                        return D.match_available && (L = i._tr_tally(D, 0, D.window[D.strstart - 1]), D.match_available = 0), D.insert = D.strstart < b - 1 ? D.strstart : b - 1, X === M ? (q(D, !0), D.strm.avail_out === 0 ? iA : W) : D.last_lit && (q(D, !1), D.strm.avail_out === 0) ? F : Z
                     }
 
-                    function nA(i, X, V, L, U) {
-                        this.good_length = i, this.max_lazy = X, this.nice_length = V, this.max_chain = L, this.func = U
+                    function nA(D, X, V, L, U) {
+                        this.good_length = D, this.max_lazy = X, this.nice_length = V, this.max_chain = L, this.func = U
                     }
 
                     function MA() {
                         this.strm = null, this.status = 0, this.pending_buf = null, this.pending_buf_size = 0, this.pending_out = 0, this.pending = 0, this.wrap = 0, this.gzhead = null, this.gzindex = 0, this.method = c, this.last_flush = -1, this.w_size = 0, this.w_bits = 0, this.w_mask = 0, this.window = null, this.window_size = 0, this.prev = null, this.head = null, this.ins_h = 0, this.hash_size = 0, this.hash_bits = 0, this.hash_mask = 0, this.hash_shift = 0, this.block_start = 0, this.match_length = 0, this.prev_match = 0, this.match_available = 0, this.strstart = 0, this.match_start = 0, this.lookahead = 0, this.prev_length = 0, this.max_chain_length = 0, this.max_lazy_match = 0, this.level = 0, this.strategy = 0, this.good_match = 0, this.nice_match = 0, this.dyn_ltree = new s.Buf16(2 * p), this.dyn_dtree = new s.Buf16(2 * (2 * l + 1)), this.bl_tree = new s.Buf16(2 * (2 * T + 1)), AA(this.dyn_ltree), AA(this.dyn_dtree), AA(this.bl_tree), this.l_desc = null, this.d_desc = null, this.bl_desc = null, this.bl_count = new s.Buf16(j + 1), this.heap = new s.Buf16(2 * H + 1), AA(this.heap), this.heap_len = 0, this.heap_max = 0, this.depth = new s.Buf16(2 * H + 1), AA(this.depth), this.l_buf = 0, this.lit_bufsize = 0, this.last_lit = 0, this.d_buf = 0, this.opt_len = 0, this.static_len = 0, this.matches = 0, this.insert = 0, this.bi_buf = 0, this.bi_valid = 0
                     }
 
-                    function rA(i) {
+                    function rA(D) {
                         var X;
-                        return i && i.state ? (i.total_in = i.total_out = 0, i.data_type = y, (X = i.state).pending = 0, X.pending_out = 0, X.wrap < 0 && (X.wrap = -X.wrap), X.status = X.wrap ? J : x, i.adler = X.wrap === 2 ? 0 : 1, X.last_flush = n, D._tr_init(X), R) : tA(i, N)
+                        return D && D.state ? (D.total_in = D.total_out = 0, D.data_type = y, (X = D.state).pending = 0, X.pending_out = 0, X.wrap < 0 && (X.wrap = -X.wrap), X.status = X.wrap ? J : x, D.adler = X.wrap === 2 ? 0 : 1, X.last_flush = n, i._tr_init(X), R) : tA(D, N)
                     }
 
-                    function HA(i) {
-                        var X = rA(i);
+                    function HA(D) {
+                        var X = rA(D);
                         return X === R && function(V) {
                             V.window_size = 2 * V.w_size, AA(V.head), V.max_lazy_match = E[V.level].max_lazy, V.good_match = E[V.level].good_length, V.nice_match = E[V.level].nice_length, V.max_chain_length = E[V.level].max_chain, V.strstart = 0, V.block_start = 0, V.lookahead = 0, V.insert = 0, V.match_length = V.prev_length = b - 1, V.match_available = 0, V.ins_h = 0
-                        }(i.state), X
+                        }(D.state), X
                     }
 
-                    function dA(i, X, V, L, U, Y) {
-                        if (!i) return N;
+                    function dA(D, X, V, L, U, Y) {
+                        if (!D) return N;
                         var z = 1;
-                        if (X === a && (X = 6), L < 0 ? (z = 0, L = -L) : 15 < L && (z = 2, L -= 16), U < 1 || k < U || V !== c || L < 8 || 15 < L || X < 0 || 9 < X || Y < 0 || G < Y) return tA(i, N);
+                        if (X === a && (X = 6), L < 0 ? (z = 0, L = -L) : 15 < L && (z = 2, L -= 16), U < 1 || k < U || V !== c || L < 8 || 15 < L || X < 0 || 9 < X || Y < 0 || G < Y) return tA(D, N);
                         L === 8 && (L = 9);
                         var P = new MA;
-                        return (i.state = P).strm = i, P.wrap = z, P.gzhead = null, P.w_bits = L, P.w_size = 1 << P.w_bits, P.w_mask = P.w_size - 1, P.hash_bits = U + 7, P.hash_size = 1 << P.hash_bits, P.hash_mask = P.hash_size - 1, P.hash_shift = ~~((P.hash_bits + b - 1) / b), P.window = new s.Buf8(2 * P.w_size), P.head = new s.Buf16(P.hash_size), P.prev = new s.Buf16(P.w_size), P.lit_bufsize = 1 << U + 6, P.pending_buf_size = 4 * P.lit_bufsize, P.pending_buf = new s.Buf8(P.pending_buf_size), P.d_buf = 1 * P.lit_bufsize, P.l_buf = 3 * P.lit_bufsize, P.level = X, P.strategy = Y, P.method = V, HA(i)
+                        return (D.state = P).strm = D, P.wrap = z, P.gzhead = null, P.w_bits = L, P.w_size = 1 << P.w_bits, P.w_mask = P.w_size - 1, P.hash_bits = U + 7, P.hash_size = 1 << P.hash_bits, P.hash_mask = P.hash_size - 1, P.hash_shift = ~~((P.hash_bits + b - 1) / b), P.window = new s.Buf8(2 * P.w_size), P.head = new s.Buf16(P.hash_size), P.prev = new s.Buf16(P.w_size), P.lit_bufsize = 1 << U + 6, P.pending_buf_size = 4 * P.lit_bufsize, P.pending_buf = new s.Buf8(P.pending_buf_size), P.d_buf = 1 * P.lit_bufsize, P.l_buf = 3 * P.lit_bufsize, P.level = X, P.strategy = Y, P.method = V, HA(D)
                     }
-                    E = [new nA(0, 0, 0, 0, function(i, X) {
+                    E = [new nA(0, 0, 0, 0, function(D, X) {
                         var V = 65535;
-                        for (V > i.pending_buf_size - 5 && (V = i.pending_buf_size - 5);;) {
-                            if (i.lookahead <= 1) {
-                                if (SA(i), i.lookahead === 0 && X === n) return F;
-                                if (i.lookahead === 0) break
-                            }
-                            i.strstart += i.lookahead, i.lookahead = 0;
-                            var L = i.block_start + V;
-                            if ((i.strstart === 0 || i.strstart >= L) && (i.lookahead = i.strstart - L, i.strstart = L, q(i, !1), i.strm.avail_out === 0) || i.strstart - i.block_start >= i.w_size - oA && (q(i, !1), i.strm.avail_out === 0)) return F
-                        }
-                        return i.insert = 0, X === M ? (q(i, !0), i.strm.avail_out === 0 ? iA : W) : (i.strstart > i.block_start && (q(i, !1), i.strm.avail_out), F)
-                    }), new nA(4, 4, 8, 4, YA), new nA(4, 5, 16, 8, YA), new nA(4, 6, 32, 32, YA), new nA(4, 4, 16, 16, GA), new nA(8, 16, 32, 32, GA), new nA(8, 16, 128, 128, GA), new nA(8, 32, 128, 256, GA), new nA(32, 128, 258, 1024, GA), new nA(32, 258, 258, 4096, GA)], t.deflateInit = function(i, X) {
-                        return dA(i, X, c, 15, 8, 0)
-                    }, t.deflateInit2 = dA, t.deflateReset = HA, t.deflateResetKeep = rA, t.deflateSetHeader = function(i, X) {
-                        return i && i.state ? i.state.wrap !== 2 ? N : (i.state.gzhead = X, R) : N
-                    }, t.deflate = function(i, X) {
+                        for (V > D.pending_buf_size - 5 && (V = D.pending_buf_size - 5);;) {
+                            if (D.lookahead <= 1) {
+                                if (SA(D), D.lookahead === 0 && X === n) return F;
+                                if (D.lookahead === 0) break
+                            }
+                            D.strstart += D.lookahead, D.lookahead = 0;
+                            var L = D.block_start + V;
+                            if ((D.strstart === 0 || D.strstart >= L) && (D.lookahead = D.strstart - L, D.strstart = L, q(D, !1), D.strm.avail_out === 0) || D.strstart - D.block_start >= D.w_size - oA && (q(D, !1), D.strm.avail_out === 0)) return F
+                        }
+                        return D.insert = 0, X === M ? (q(D, !0), D.strm.avail_out === 0 ? iA : W) : (D.strstart > D.block_start && (q(D, !1), D.strm.avail_out), F)
+                    }), new nA(4, 4, 8, 4, YA), new nA(4, 5, 16, 8, YA), new nA(4, 6, 32, 32, YA), new nA(4, 4, 16, 16, GA), new nA(8, 16, 32, 32, GA), new nA(8, 16, 128, 128, GA), new nA(8, 32, 128, 256, GA), new nA(32, 128, 258, 1024, GA), new nA(32, 258, 258, 4096, GA)], t.deflateInit = function(D, X) {
+                        return dA(D, X, c, 15, 8, 0)
+                    }, t.deflateInit2 = dA, t.deflateReset = HA, t.deflateResetKeep = rA, t.deflateSetHeader = function(D, X) {
+                        return D && D.state ? D.state.wrap !== 2 ? N : (D.state.gzhead = X, R) : N
+                    }, t.deflate = function(D, X) {
                         var V, L, U, Y;
-                        if (!i || !i.state || 5 < X || X < 0) return i ? tA(i, N) : N;
-                        if (L = i.state, !i.output || !i.input && i.avail_in !== 0 || L.status === 666 && X !== M) return tA(i, i.avail_out === 0 ? -5 : N);
-                        if (L.strm = i, V = L.last_flush, L.last_flush = X, L.status === J)
-                            if (L.wrap === 2) i.adler = 0, sA(L, 31), sA(L, 139), sA(L, 8), L.gzhead ? (sA(L, (L.gzhead.text ? 1 : 0) + (L.gzhead.hcrc ? 2 : 0) + (L.gzhead.extra ? 4 : 0) + (L.gzhead.name ? 8 : 0) + (L.gzhead.comment ? 16 : 0)), sA(L, 255 & L.gzhead.time), sA(L, L.gzhead.time >> 8 & 255), sA(L, L.gzhead.time >> 16 & 255), sA(L, L.gzhead.time >> 24 & 255), sA(L, L.level === 9 ? 2 : 2 <= L.strategy || L.level < 2 ? 4 : 0), sA(L, 255 & L.gzhead.os), L.gzhead.extra && L.gzhead.extra.length && (sA(L, 255 & L.gzhead.extra.length), sA(L, L.gzhead.extra.length >> 8 & 255)), L.gzhead.hcrc && (i.adler = C(i.adler, L.pending_buf, L.pending, 0)), L.gzindex = 0, L.status = 69) : (sA(L, 0), sA(L, 0), sA(L, 0), sA(L, 0), sA(L, 0), sA(L, L.level === 9 ? 2 : 2 <= L.strategy || L.level < 2 ? 4 : 0), sA(L, 3), L.status = x);
+                        if (!D || !D.state || 5 < X || X < 0) return D ? tA(D, N) : N;
+                        if (L = D.state, !D.output || !D.input && D.avail_in !== 0 || L.status === 666 && X !== M) return tA(D, D.avail_out === 0 ? -5 : N);
+                        if (L.strm = D, V = L.last_flush, L.last_flush = X, L.status === J)
+                            if (L.wrap === 2) D.adler = 0, sA(L, 31), sA(L, 139), sA(L, 8), L.gzhead ? (sA(L, (L.gzhead.text ? 1 : 0) + (L.gzhead.hcrc ? 2 : 0) + (L.gzhead.extra ? 4 : 0) + (L.gzhead.name ? 8 : 0) + (L.gzhead.comment ? 16 : 0)), sA(L, 255 & L.gzhead.time), sA(L, L.gzhead.time >> 8 & 255), sA(L, L.gzhead.time >> 16 & 255), sA(L, L.gzhead.time >> 24 & 255), sA(L, L.level === 9 ? 2 : 2 <= L.strategy || L.level < 2 ? 4 : 0), sA(L, 255 & L.gzhead.os), L.gzhead.extra && L.gzhead.extra.length && (sA(L, 255 & L.gzhead.extra.length), sA(L, L.gzhead.extra.length >> 8 & 255)), L.gzhead.hcrc && (D.adler = C(D.adler, L.pending_buf, L.pending, 0)), L.gzindex = 0, L.status = 69) : (sA(L, 0), sA(L, 0), sA(L, 0), sA(L, 0), sA(L, 0), sA(L, L.level === 9 ? 2 : 2 <= L.strategy || L.level < 2 ? 4 : 0), sA(L, 3), L.status = x);
                             else {
                                 var z = c + (L.w_bits - 8 << 4) << 8;
-                                z |= (2 <= L.strategy || L.level < 2 ? 0 : L.level < 6 ? 1 : L.level === 6 ? 2 : 3) << 6, L.strstart !== 0 && (z |= 32), z += 31 - z % 31, L.status = x, CA(L, z), L.strstart !== 0 && (CA(L, i.adler >>> 16), CA(L, 65535 & i.adler)), i.adler = 1
+                                z |= (2 <= L.strategy || L.level < 2 ? 0 : L.level < 6 ? 1 : L.level === 6 ? 2 : 3) << 6, L.strstart !== 0 && (z |= 32), z += 31 - z % 31, L.status = x, CA(L, z), L.strstart !== 0 && (CA(L, D.adler >>> 16), CA(L, 65535 & D.adler)), D.adler = 1
                             } if (L.status === 69)
                             if (L.gzhead.extra) {
-                                for (U = L.pending; L.gzindex < (65535 & L.gzhead.extra.length) && (L.pending !== L.pending_buf_size || (L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), f(i), U = L.pending, L.pending !== L.pending_buf_size));) sA(L, 255 & L.gzhead.extra[L.gzindex]), L.gzindex++;
-                                L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), L.gzindex === L.gzhead.extra.length && (L.gzindex = 0, L.status = 73)
+                                for (U = L.pending; L.gzindex < (65535 & L.gzhead.extra.length) && (L.pending !== L.pending_buf_size || (L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), f(D), U = L.pending, L.pending !== L.pending_buf_size));) sA(L, 255 & L.gzhead.extra[L.gzindex]), L.gzindex++;
+                                L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), L.gzindex === L.gzhead.extra.length && (L.gzindex = 0, L.status = 73)
                             } else L.status = 73;
                         if (L.status === 73)
                             if (L.gzhead.name) {
                                 U = L.pending;
                                 do {
-                                    if (L.pending === L.pending_buf_size && (L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), f(i), U = L.pending, L.pending === L.pending_buf_size)) {
+                                    if (L.pending === L.pending_buf_size && (L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), f(D), U = L.pending, L.pending === L.pending_buf_size)) {
                                         Y = 1;
                                         break
                                     }
                                     Y = L.gzindex < L.gzhead.name.length ? 255 & L.gzhead.name.charCodeAt(L.gzindex++) : 0, sA(L, Y)
                                 } while (Y !== 0);
-                                L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), Y === 0 && (L.gzindex = 0, L.status = 91)
+                                L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), Y === 0 && (L.gzindex = 0, L.status = 91)
                             } else L.status = 91;
                         if (L.status === 91)
                             if (L.gzhead.comment) {
                                 U = L.pending;
                                 do {
-                                    if (L.pending === L.pending_buf_size && (L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), f(i), U = L.pending, L.pending === L.pending_buf_size)) {
+                                    if (L.pending === L.pending_buf_size && (L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), f(D), U = L.pending, L.pending === L.pending_buf_size)) {
                                         Y = 1;
                                         break
                                     }
                                     Y = L.gzindex < L.gzhead.comment.length ? 255 & L.gzhead.comment.charCodeAt(L.gzindex++) : 0, sA(L, Y)
                                 } while (Y !== 0);
-                                L.gzhead.hcrc && L.pending > U && (i.adler = C(i.adler, L.pending_buf, L.pending - U, U)), Y === 0 && (L.status = 103)
+                                L.gzhead.hcrc && L.pending > U && (D.adler = C(D.adler, L.pending_buf, L.pending - U, U)), Y === 0 && (L.status = 103)
                             } else L.status = 103;
-                        if (L.status === 103 && (L.gzhead.hcrc ? (L.pending + 2 > L.pending_buf_size && f(i), L.pending + 2 <= L.pending_buf_size && (sA(L, 255 & i.adler), sA(L, i.adler >> 8 & 255), i.adler = 0, L.status = x)) : L.status = x), L.pending !== 0) {
-                            if (f(i), i.avail_out === 0) return L.last_flush = -1, R
-                        } else if (i.avail_in === 0 && _(X) <= _(V) && X !== M) return tA(i, -5);
-                        if (L.status === 666 && i.avail_in !== 0) return tA(i, -5);
-                        if (i.avail_in !== 0 || L.lookahead !== 0 || X !== n && L.status !== 666) {
+                        if (L.status === 103 && (L.gzhead.hcrc ? (L.pending + 2 > L.pending_buf_size && f(D), L.pending + 2 <= L.pending_buf_size && (sA(L, 255 & D.adler), sA(L, D.adler >> 8 & 255), D.adler = 0, L.status = x)) : L.status = x), L.pending !== 0) {
+                            if (f(D), D.avail_out === 0) return L.last_flush = -1, R
+                        } else if (D.avail_in === 0 && _(X) <= _(V) && X !== M) return tA(D, -5);
+                        if (L.status === 666 && D.avail_in !== 0) return tA(D, -5);
+                        if (D.avail_in !== 0 || L.lookahead !== 0 || X !== n && L.status !== 666) {
                             var P = L.strategy === 2 ? function(u, IA) {
                                 for (var EA;;) {
                                     if (u.lookahead === 0 && (SA(u), u.lookahead === 0)) {
                                         if (IA === n) return F;
                                         break
                                     }
-                                    if (u.match_length = 0, EA = D._tr_tally(u, 0, u.window[u.strstart]), u.lookahead--, u.strstart++, EA && (q(u, !1), u.strm.avail_out === 0)) return F
+                                    if (u.match_length = 0, EA = i._tr_tally(u, 0, u.window[u.strstart]), u.lookahead--, u.strstart++, EA && (q(u, !1), u.strm.avail_out === 0)) return F
                                 }
                                 return u.insert = 0, IA === M ? (q(u, !0), u.strm.avail_out === 0 ? iA : W) : u.last_lit && (q(u, !1), u.strm.avail_out === 0) ? F : Z
                             }(L, X) : L.strategy === 3 ? function(u, IA) {
                                 for (var EA, BA, wA, NA, RA = u.window;;) {
                                     if (u.lookahead <= gA) {
                                         if (SA(u), u.lookahead <= gA && IA === n) return F;
                                         if (u.lookahead === 0) break
                                     }
                                     if (u.match_length = 0, u.lookahead >= b && 0 < u.strstart && (BA = RA[wA = u.strstart - 1]) === RA[++wA] && BA === RA[++wA] && BA === RA[++wA]) {
                                         NA = u.strstart + gA;
                                         do; while (BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && BA === RA[++wA] && wA < NA);
                                         u.match_length = gA - (NA - wA), u.match_length > u.lookahead && (u.match_length = u.lookahead)
                                     }
-                                    if (u.match_length >= b ? (EA = D._tr_tally(u, 1, u.match_length - b), u.lookahead -= u.match_length, u.strstart += u.match_length, u.match_length = 0) : (EA = D._tr_tally(u, 0, u.window[u.strstart]), u.lookahead--, u.strstart++), EA && (q(u, !1), u.strm.avail_out === 0)) return F
+                                    if (u.match_length >= b ? (EA = i._tr_tally(u, 1, u.match_length - b), u.lookahead -= u.match_length, u.strstart += u.match_length, u.match_length = 0) : (EA = i._tr_tally(u, 0, u.window[u.strstart]), u.lookahead--, u.strstart++), EA && (q(u, !1), u.strm.avail_out === 0)) return F
                                 }
                                 return u.insert = 0, IA === M ? (q(u, !0), u.strm.avail_out === 0 ? iA : W) : u.last_lit && (q(u, !1), u.strm.avail_out === 0) ? F : Z
                             }(L, X) : E[L.level].func(L, X);
-                            if (P !== iA && P !== W || (L.status = 666), P === F || P === iA) return i.avail_out === 0 && (L.last_flush = -1), R;
-                            if (P === Z && (X === 1 ? D._tr_align(L) : X !== 5 && (D._tr_stored_block(L, 0, 0, !1), X === 3 && (AA(L.head), L.lookahead === 0 && (L.strstart = 0, L.block_start = 0, L.insert = 0))), f(i), i.avail_out === 0)) return L.last_flush = -1, R
+                            if (P !== iA && P !== W || (L.status = 666), P === F || P === iA) return D.avail_out === 0 && (L.last_flush = -1), R;
+                            if (P === Z && (X === 1 ? i._tr_align(L) : X !== 5 && (i._tr_stored_block(L, 0, 0, !1), X === 3 && (AA(L.head), L.lookahead === 0 && (L.strstart = 0, L.block_start = 0, L.insert = 0))), f(D), D.avail_out === 0)) return L.last_flush = -1, R
                         }
-                        return X !== M ? R : L.wrap <= 0 ? 1 : (L.wrap === 2 ? (sA(L, 255 & i.adler), sA(L, i.adler >> 8 & 255), sA(L, i.adler >> 16 & 255), sA(L, i.adler >> 24 & 255), sA(L, 255 & i.total_in), sA(L, i.total_in >> 8 & 255), sA(L, i.total_in >> 16 & 255), sA(L, i.total_in >> 24 & 255)) : (CA(L, i.adler >>> 16), CA(L, 65535 & i.adler)), f(i), 0 < L.wrap && (L.wrap = -L.wrap), L.pending !== 0 ? R : 1)
-                    }, t.deflateEnd = function(i) {
+                        return X !== M ? R : L.wrap <= 0 ? 1 : (L.wrap === 2 ? (sA(L, 255 & D.adler), sA(L, D.adler >> 8 & 255), sA(L, D.adler >> 16 & 255), sA(L, D.adler >> 24 & 255), sA(L, 255 & D.total_in), sA(L, D.total_in >> 8 & 255), sA(L, D.total_in >> 16 & 255), sA(L, D.total_in >> 24 & 255)) : (CA(L, D.adler >>> 16), CA(L, 65535 & D.adler)), f(D), 0 < L.wrap && (L.wrap = -L.wrap), L.pending !== 0 ? R : 1)
+                    }, t.deflateEnd = function(D) {
                         var X;
-                        return i && i.state ? (X = i.state.status) !== J && X !== 69 && X !== 73 && X !== 91 && X !== 103 && X !== x && X !== 666 ? tA(i, N) : (i.state = null, X === x ? tA(i, -3) : R) : N
-                    }, t.deflateSetDictionary = function(i, X) {
+                        return D && D.state ? (X = D.state.status) !== J && X !== 69 && X !== 73 && X !== 91 && X !== 103 && X !== x && X !== 666 ? tA(D, N) : (D.state = null, X === x ? tA(D, -3) : R) : N
+                    }, t.deflateSetDictionary = function(D, X) {
                         var V, L, U, Y, z, P, u, IA, EA = X.length;
-                        if (!i || !i.state || (Y = (V = i.state).wrap) === 2 || Y === 1 && V.status !== J || V.lookahead) return N;
-                        for (Y === 1 && (i.adler = h(i.adler, X, EA, 0)), V.wrap = 0, EA >= V.w_size && (Y === 0 && (AA(V.head), V.strstart = 0, V.block_start = 0, V.insert = 0), IA = new s.Buf8(V.w_size), s.arraySet(IA, X, EA - V.w_size, V.w_size, 0), X = IA, EA = V.w_size), z = i.avail_in, P = i.next_in, u = i.input, i.avail_in = EA, i.next_in = 0, i.input = X, SA(V); V.lookahead >= b;) {
+                        if (!D || !D.state || (Y = (V = D.state).wrap) === 2 || Y === 1 && V.status !== J || V.lookahead) return N;
+                        for (Y === 1 && (D.adler = h(D.adler, X, EA, 0)), V.wrap = 0, EA >= V.w_size && (Y === 0 && (AA(V.head), V.strstart = 0, V.block_start = 0, V.insert = 0), IA = new s.Buf8(V.w_size), s.arraySet(IA, X, EA - V.w_size, V.w_size, 0), X = IA, EA = V.w_size), z = D.avail_in, P = D.next_in, u = D.input, D.avail_in = EA, D.next_in = 0, D.input = X, SA(V); V.lookahead >= b;) {
                             for (L = V.strstart, U = V.lookahead - (b - 1); V.ins_h = (V.ins_h << V.hash_shift ^ V.window[L + b - 1]) & V.hash_mask, V.prev[L & V.w_mask] = V.head[V.ins_h], V.head[V.ins_h] = L, L++, --U;);
                             V.strstart = L, V.lookahead = b - 1, SA(V)
                         }
-                        return V.strstart += V.lookahead, V.block_start = V.strstart, V.insert = V.lookahead, V.lookahead = 0, V.match_length = V.prev_length = b - 1, V.match_available = 0, i.next_in = P, i.input = u, i.avail_in = z, V.wrap = Y, R
+                        return V.strstart += V.lookahead, V.block_start = V.strstart, V.insert = V.lookahead, V.lookahead = 0, V.match_length = V.prev_length = b - 1, V.match_available = 0, D.next_in = P, D.input = u, D.avail_in = z, V.wrap = Y, R
                     }, t.deflateInfo = "pako deflate (from Nodeca project)"
                 }, {
                     "../utils/common": 41,
                     "./adler32": 43,
                     "./crc32": 45,
                     "./messages": 51,
                     "./trees": 52
@@ -6968,50 +7011,50 @@
                 47: [function(g, o, t) {
                     o.exports = function() {
                         this.text = 0, this.time = 0, this.xflags = 0, this.os = 0, this.extra = null, this.extra_len = 0, this.name = "", this.comment = "", this.hcrc = 0, this.done = !1
                     }
                 }, {}],
                 48: [function(g, o, t) {
                     o.exports = function(E, s) {
-                        var D, h, C, r, n, M, R, N, a, G, y, c, k, H, l, T, p, j, b, gA, oA, J, x, F, Z;
-                        D = E.state, h = E.next_in, F = E.input, C = h + (E.avail_in - 5), r = E.next_out, Z = E.output, n = r - (s - E.avail_out), M = r + (E.avail_out - 257), R = D.dmax, N = D.wsize, a = D.whave, G = D.wnext, y = D.window, c = D.hold, k = D.bits, H = D.lencode, l = D.distcode, T = (1 << D.lenbits) - 1, p = (1 << D.distbits) - 1;
+                        var i, h, C, r, n, M, R, N, a, G, y, c, k, H, l, T, p, j, b, gA, oA, J, x, F, Z;
+                        i = E.state, h = E.next_in, F = E.input, C = h + (E.avail_in - 5), r = E.next_out, Z = E.output, n = r - (s - E.avail_out), M = r + (E.avail_out - 257), R = i.dmax, N = i.wsize, a = i.whave, G = i.wnext, y = i.window, c = i.hold, k = i.bits, H = i.lencode, l = i.distcode, T = (1 << i.lenbits) - 1, p = (1 << i.distbits) - 1;
                         A: do {
                             k < 15 && (c += F[h++] << k, k += 8, c += F[h++] << k, k += 8), j = H[c & T];
                             I: for (;;) {
                                 if (c >>>= b = j >>> 24, k -= b, (b = j >>> 16 & 255) === 0) Z[r++] = 65535 & j;
                                 else {
                                     if (!(16 & b)) {
                                         if (!(64 & b)) {
                                             j = H[(65535 & j) + (c & (1 << b) - 1)];
                                             continue I
                                         }
                                         if (32 & b) {
-                                            D.mode = 12;
+                                            i.mode = 12;
                                             break A
                                         }
-                                        E.msg = "invalid literal/length code", D.mode = 30;
+                                        E.msg = "invalid literal/length code", i.mode = 30;
                                         break A
                                     }
                                     gA = 65535 & j, (b &= 15) && (k < b && (c += F[h++] << k, k += 8), gA += c & (1 << b) - 1, c >>>= b, k -= b), k < 15 && (c += F[h++] << k, k += 8, c += F[h++] << k, k += 8), j = l[c & p];
                                     g: for (;;) {
                                         if (c >>>= b = j >>> 24, k -= b, !(16 & (b = j >>> 16 & 255))) {
                                             if (!(64 & b)) {
                                                 j = l[(65535 & j) + (c & (1 << b) - 1)];
                                                 continue g
                                             }
-                                            E.msg = "invalid distance code", D.mode = 30;
+                                            E.msg = "invalid distance code", i.mode = 30;
                                             break A
                                         }
                                         if (oA = 65535 & j, k < (b &= 15) && (c += F[h++] << k, (k += 8) < b && (c += F[h++] << k, k += 8)), R < (oA += c & (1 << b) - 1)) {
-                                            E.msg = "invalid distance too far back", D.mode = 30;
+                                            E.msg = "invalid distance too far back", i.mode = 30;
                                             break A
                                         }
                                         if (c >>>= b, k -= b, (b = r - n) < oA) {
-                                            if (a < (b = oA - b) && D.sane) {
-                                                E.msg = "invalid distance too far back", D.mode = 30;
+                                            if (a < (b = oA - b) && i.sane) {
+                                                E.msg = "invalid distance too far back", i.mode = 30;
                                                 break A
                                             }
                                             if (x = y, (J = 0) === G) {
                                                 if (J += N - b, b < gA) {
                                                     for (gA -= b; Z[r++] = y[J++], --b;);
                                                     J = r - oA, x = Z
                                                 }
@@ -7035,21 +7078,21 @@
                                         }
                                         break
                                     }
                                 }
                                 break
                             }
                         } while (h < C && r < M);
-                        h -= gA = k >> 3, c &= (1 << (k -= gA << 3)) - 1, E.next_in = h, E.next_out = r, E.avail_in = h < C ? C - h + 5 : 5 - (h - C), E.avail_out = r < M ? M - r + 257 : 257 - (r - M), D.hold = c, D.bits = k
+                        h -= gA = k >> 3, c &= (1 << (k -= gA << 3)) - 1, E.next_in = h, E.next_out = r, E.avail_in = h < C ? C - h + 5 : 5 - (h - C), E.avail_out = r < M ? M - r + 257 : 257 - (r - M), i.hold = c, i.bits = k
                     }
                 }, {}],
                 49: [function(g, o, t) {
                     var E = g("../utils/common"),
                         s = g("./adler32"),
-                        D = g("./crc32"),
+                        i = g("./crc32"),
                         h = g("./inffast"),
                         C = g("./inftrees"),
                         r = 1,
                         n = 2,
                         M = 0,
                         R = -2,
                         N = 1,
@@ -7105,15 +7148,15 @@
                     function oA(J, x, F, Z) {
                         var iA, W = J.state;
                         return W.window === null && (W.wsize = 1 << W.wbits, W.wnext = 0, W.whave = 0, W.window = new E.Buf8(W.wsize)), Z >= W.wsize ? (E.arraySet(W.window, x, F - W.wsize, W.wsize, 0), W.wnext = 0, W.whave = W.wsize) : (Z < (iA = W.wsize - W.wnext) && (iA = Z), E.arraySet(W.window, x, F - Z, iA, W.wnext), (Z -= iA) ? (E.arraySet(W.window, x, F - Z, Z, 0), W.wnext = Z, W.whave = W.wsize) : (W.wnext += iA, W.wnext === W.wsize && (W.wnext = 0), W.whave < W.wsize && (W.whave += iA))), 0
                     }
                     t.inflateReset = H, t.inflateReset2 = l, t.inflateResetKeep = k, t.inflateInit = function(J) {
                         return T(J, 15)
                     }, t.inflateInit2 = T, t.inflate = function(J, x) {
-                        var F, Z, iA, W, tA, _, AA, f, q, sA, CA, QA, SA, YA, GA, nA, MA, rA, HA, dA, i, X, V, L, U = 0,
+                        var F, Z, iA, W, tA, _, AA, f, q, sA, CA, QA, SA, YA, GA, nA, MA, rA, HA, dA, D, X, V, L, U = 0,
                             Y = new E.Buf8(4),
                             z = [16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15];
                         if (!J || !J.state || !J.output || !J.input && J.avail_in !== 0) return R;
                         (F = J.state).mode === 12 && (F.mode = 13), tA = J.next_out, iA = J.output, AA = J.avail_out, W = J.next_in, Z = J.input, _ = J.avail_in, f = F.hold, q = F.bits, sA = _, CA = AA, X = M;
                         A: for (;;) switch (F.mode) {
                             case N:
                                 if (F.wrap === 0) {
@@ -7121,82 +7164,82 @@
                                     break
                                 }
                                 for (; q < 16;) {
                                     if (_ === 0) break A;
                                     _--, f += Z[W++] << q, q += 8
                                 }
                                 if (2 & F.wrap && f === 35615) {
-                                    Y[F.check = 0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = D(F.check, Y, 2, 0), q = f = 0, F.mode = 2;
+                                    Y[F.check = 0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = i(F.check, Y, 2, 0), q = f = 0, F.mode = 2;
                                     break
                                 }
                                 if (F.flags = 0, F.head && (F.head.done = !1), !(1 & F.wrap) || (((255 & f) << 8) + (f >> 8)) % 31) {
                                     J.msg = "incorrect header check", F.mode = 30;
                                     break
                                 }
                                 if ((15 & f) != 8) {
                                     J.msg = "unknown compression method", F.mode = 30;
                                     break
                                 }
-                                if (q -= 4, i = 8 + (15 & (f >>>= 4)), F.wbits === 0) F.wbits = i;
-                                else if (i > F.wbits) {
+                                if (q -= 4, D = 8 + (15 & (f >>>= 4)), F.wbits === 0) F.wbits = D;
+                                else if (D > F.wbits) {
                                     J.msg = "invalid window size", F.mode = 30;
                                     break
                                 }
-                                F.dmax = 1 << i, J.adler = F.check = 1, F.mode = 512 & f ? 10 : 12, q = f = 0;
+                                F.dmax = 1 << D, J.adler = F.check = 1, F.mode = 512 & f ? 10 : 12, q = f = 0;
                                 break;
                             case 2:
                                 for (; q < 16;) {
                                     if (_ === 0) break A;
                                     _--, f += Z[W++] << q, q += 8
                                 }
                                 if (F.flags = f, (255 & F.flags) != 8) {
                                     J.msg = "unknown compression method", F.mode = 30;
                                     break
                                 }
                                 if (57344 & F.flags) {
                                     J.msg = "unknown header flags set", F.mode = 30;
                                     break
                                 }
-                                F.head && (F.head.text = f >> 8 & 1), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = D(F.check, Y, 2, 0)), q = f = 0, F.mode = 3;
+                                F.head && (F.head.text = f >> 8 & 1), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = i(F.check, Y, 2, 0)), q = f = 0, F.mode = 3;
                             case 3:
                                 for (; q < 32;) {
                                     if (_ === 0) break A;
                                     _--, f += Z[W++] << q, q += 8
                                 }
-                                F.head && (F.head.time = f), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, Y[2] = f >>> 16 & 255, Y[3] = f >>> 24 & 255, F.check = D(F.check, Y, 4, 0)), q = f = 0, F.mode = 4;
+                                F.head && (F.head.time = f), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, Y[2] = f >>> 16 & 255, Y[3] = f >>> 24 & 255, F.check = i(F.check, Y, 4, 0)), q = f = 0, F.mode = 4;
                             case 4:
                                 for (; q < 16;) {
                                     if (_ === 0) break A;
                                     _--, f += Z[W++] << q, q += 8
                                 }
-                                F.head && (F.head.xflags = 255 & f, F.head.os = f >> 8), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = D(F.check, Y, 2, 0)), q = f = 0, F.mode = 5;
+                                F.head && (F.head.xflags = 255 & f, F.head.os = f >> 8), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = i(F.check, Y, 2, 0)), q = f = 0, F.mode = 5;
                             case 5:
                                 if (1024 & F.flags) {
                                     for (; q < 16;) {
                                         if (_ === 0) break A;
                                         _--, f += Z[W++] << q, q += 8
                                     }
-                                    F.length = f, F.head && (F.head.extra_len = f), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = D(F.check, Y, 2, 0)), q = f = 0
+                                    F.length = f, F.head && (F.head.extra_len = f), 512 & F.flags && (Y[0] = 255 & f, Y[1] = f >>> 8 & 255, F.check = i(F.check, Y, 2, 0)), q = f = 0
                                 } else F.head && (F.head.extra = null);
                                 F.mode = 6;
                             case 6:
-                                if (1024 & F.flags && (_ < (QA = F.length) && (QA = _), QA && (F.head && (i = F.head.extra_len - F.length, F.head.extra || (F.head.extra = new Array(F.head.extra_len)), E.arraySet(F.head.extra, Z, W, QA, i)), 512 & F.flags && (F.check = D(F.check, Z, QA, W)), _ -= QA, W += QA, F.length -= QA), F.length)) break A;
+                                if (1024 & F.flags && (_ < (QA = F.length) && (QA = _), QA && (F.head && (D = F.head.extra_len - F.length, F.head.extra || (F.head.extra = new Array(F.head.extra_len)), E.arraySet(F.head.extra, Z, W, QA, D)), 512 & F.flags && (F.check = i(F.check, Z, QA, W)), _ -= QA, W += QA, F.length -= QA), F.length)) break A;
                                 F.length = 0, F.mode = 7;
                             case 7:
                                 if (2048 & F.flags) {
                                     if (_ === 0) break A;
-                                    for (QA = 0; i = Z[W + QA++], F.head && i && F.length < 65536 && (F.head.name += String.fromCharCode(i)), i && QA < _;);
-                                    if (512 & F.flags && (F.check = D(F.check, Z, QA, W)), _ -= QA, W += QA, i) break A
+                                    for (QA = 0; D = Z[W + QA++], F.head && D && F.length < 65536 && (F.head.name += String.fromCharCode(D)), D && QA < _;);
+                                    if (512 & F.flags && (F.check = i(F.check, Z, QA, W)), _ -= QA, W += QA, D) break A
                                 } else F.head && (F.head.name = null);
                                 F.length = 0, F.mode = 8;
                             case 8:
                                 if (4096 & F.flags) {
                                     if (_ === 0) break A;
-                                    for (QA = 0; i = Z[W + QA++], F.head && i && F.length < 65536 && (F.head.comment += String.fromCharCode(i)), i && QA < _;);
-                                    if (512 & F.flags && (F.check = D(F.check, Z, QA, W)), _ -= QA, W += QA, i) break A
+                                    for (QA = 0; D = Z[W + QA++], F.head && D && F.length < 65536 && (F.head.comment += String.fromCharCode(D)), D && QA < _;);
+                                    if (512 & F.flags && (F.check = i(F.check, Z, QA, W)), _ -= QA, W += QA, D) break A
                                 } else F.head && (F.head.comment = null);
                                 F.mode = 9;
                             case 9:
                                 if (512 & F.flags) {
                                     for (; q < 16;) {
                                         if (_ === 0) break A;
                                         _--, f += Z[W++] << q, q += 8
@@ -7304,33 +7347,33 @@
                                                 if (_ === 0) break A;
                                                 _--, f += Z[W++] << q, q += 8
                                             }
                                             if (f >>>= GA, q -= GA, F.have === 0) {
                                                 J.msg = "invalid bit length repeat", F.mode = 30;
                                                 break
                                             }
-                                            i = F.lens[F.have - 1], QA = 3 + (3 & f), f >>>= 2, q -= 2
+                                            D = F.lens[F.have - 1], QA = 3 + (3 & f), f >>>= 2, q -= 2
                                         } else if (MA === 17) {
                                             for (L = GA + 3; q < L;) {
                                                 if (_ === 0) break A;
                                                 _--, f += Z[W++] << q, q += 8
                                             }
-                                            q -= GA, i = 0, QA = 3 + (7 & (f >>>= GA)), f >>>= 3, q -= 3
+                                            q -= GA, D = 0, QA = 3 + (7 & (f >>>= GA)), f >>>= 3, q -= 3
                                         } else {
                                             for (L = GA + 7; q < L;) {
                                                 if (_ === 0) break A;
                                                 _--, f += Z[W++] << q, q += 8
                                             }
-                                            q -= GA, i = 0, QA = 11 + (127 & (f >>>= GA)), f >>>= 7, q -= 7
+                                            q -= GA, D = 0, QA = 11 + (127 & (f >>>= GA)), f >>>= 7, q -= 7
                                         }
                                         if (F.have + QA > F.nlen + F.ndist) {
                                             J.msg = "invalid bit length repeat", F.mode = 30;
                                             break
                                         }
-                                        for (; QA--;) F.lens[F.have++] = i
+                                        for (; QA--;) F.lens[F.have++] = D
                                     }
                                 }
                                 if (F.mode === 30) break;
                                 if (F.lens[256] === 0) {
                                     J.msg = "invalid code -- missing end-of-block", F.mode = 30;
                                     break
                                 }
@@ -7435,15 +7478,15 @@
                                 break;
                             case 27:
                                 if (F.wrap) {
                                     for (; q < 32;) {
                                         if (_ === 0) break A;
                                         _--, f |= Z[W++] << q, q += 8
                                     }
-                                    if (CA -= AA, J.total_out += CA, F.total += CA, CA && (J.adler = F.check = F.flags ? D(F.check, iA, CA, tA - CA) : s(F.check, iA, CA, tA - CA)), CA = AA, (F.flags ? f : y(f)) !== F.check) {
+                                    if (CA -= AA, J.total_out += CA, F.total += CA, CA && (J.adler = F.check = F.flags ? i(F.check, iA, CA, tA - CA) : s(F.check, iA, CA, tA - CA)), CA = AA, (F.flags ? f : y(f)) !== F.check) {
                                         J.msg = "incorrect data check", F.mode = 30;
                                         break
                                     }
                                     q = f = 0
                                 }
                                 F.mode = 28;
                             case 28:
@@ -7467,15 +7510,15 @@
                                 break A;
                             case 31:
                                 return -4;
                             case 32:
                             default:
                                 return R
                         }
-                        return J.next_out = tA, J.avail_out = AA, J.next_in = W, J.avail_in = _, F.hold = f, F.bits = q, (F.wsize || CA !== J.avail_out && F.mode < 30 && (F.mode < 27 || x !== 4)) && oA(J, J.output, J.next_out, CA - J.avail_out) ? (F.mode = 31, -4) : (sA -= J.avail_in, CA -= J.avail_out, J.total_in += sA, J.total_out += CA, F.total += CA, F.wrap && CA && (J.adler = F.check = F.flags ? D(F.check, iA, CA, J.next_out - CA) : s(F.check, iA, CA, J.next_out - CA)), J.data_type = F.bits + (F.last ? 64 : 0) + (F.mode === 12 ? 128 : 0) + (F.mode === 20 || F.mode === 15 ? 256 : 0), (sA == 0 && CA === 0 || x === 4) && X === M && (X = -5), X)
+                        return J.next_out = tA, J.avail_out = AA, J.next_in = W, J.avail_in = _, F.hold = f, F.bits = q, (F.wsize || CA !== J.avail_out && F.mode < 30 && (F.mode < 27 || x !== 4)) && oA(J, J.output, J.next_out, CA - J.avail_out) ? (F.mode = 31, -4) : (sA -= J.avail_in, CA -= J.avail_out, J.total_in += sA, J.total_out += CA, F.total += CA, F.wrap && CA && (J.adler = F.check = F.flags ? i(F.check, iA, CA, J.next_out - CA) : s(F.check, iA, CA, J.next_out - CA)), J.data_type = F.bits + (F.last ? 64 : 0) + (F.mode === 12 ? 128 : 0) + (F.mode === 20 || F.mode === 15 ? 256 : 0), (sA == 0 && CA === 0 || x === 4) && X === M && (X = -5), X)
                     }, t.inflateEnd = function(J) {
                         if (!J || !J.state) return R;
                         var x = J.state;
                         return x.window && (x.window = null), J.state = null, M
                     }, t.inflateGetHeader = function(J, x) {
                         var F;
                         return J && J.state && 2 & (F = J.state).wrap ? ((F.head = x).done = !1, M) : R
@@ -7489,15 +7532,15 @@
                     "./crc32": 45,
                     "./inffast": 48,
                     "./inftrees": 50
                 }],
                 50: [function(g, o, t) {
                     var E = g("../utils/common"),
                         s = [3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 15, 17, 19, 23, 27, 31, 35, 43, 51, 59, 67, 83, 99, 115, 131, 163, 195, 227, 258, 0, 0],
-                        D = [16, 16, 16, 16, 16, 16, 16, 16, 17, 17, 17, 17, 18, 18, 18, 18, 19, 19, 19, 19, 20, 20, 20, 20, 21, 21, 21, 21, 16, 72, 78],
+                        i = [16, 16, 16, 16, 16, 16, 16, 16, 17, 17, 17, 17, 18, 18, 18, 18, 19, 19, 19, 19, 20, 20, 20, 20, 21, 21, 21, 21, 16, 72, 78],
                         h = [1, 2, 3, 4, 5, 7, 9, 13, 17, 25, 33, 49, 65, 97, 129, 193, 257, 385, 513, 769, 1025, 1537, 2049, 3073, 4097, 6145, 8193, 12289, 16385, 24577, 0, 0],
                         C = [16, 16, 16, 16, 17, 17, 18, 18, 19, 19, 20, 20, 21, 21, 22, 22, 23, 23, 24, 24, 25, 25, 26, 26, 27, 27, 28, 28, 29, 29, 64, 64];
                     o.exports = function(r, n, M, R, N, a, G, y) {
                         var c, k, H, l, T, p, j, b, gA, oA = y.bits,
                             J = 0,
                             x = 0,
                             F = 0,
@@ -7520,15 +7563,15 @@
                         if (Z < iA && (iA = Z), Z === 0) return N[a++] = 20971520, N[a++] = 20971520, y.bits = 1, 0;
                         for (F = 1; F < Z && CA[F] === 0; F++);
                         for (iA < F && (iA = F), J = _ = 1; J <= 15; J++)
                             if (_ <<= 1, (_ -= CA[J]) < 0) return -1;
                         if (0 < _ && (r === 0 || Z !== 1)) return -1;
                         for (QA[1] = 0, J = 1; J < 15; J++) QA[J + 1] = QA[J] + CA[J];
                         for (x = 0; x < R; x++) n[M + x] !== 0 && (G[QA[n[M + x]]++] = x);
-                        if (p = r === 0 ? (q = SA = G, 19) : r === 1 ? (q = s, sA -= 257, SA = D, YA -= 257, 256) : (q = h, SA = C, -1), J = F, T = a, tA = x = f = 0, H = -1, l = (AA = 1 << (W = iA)) - 1, r === 1 && 852 < AA || r === 2 && 592 < AA) return 1;
+                        if (p = r === 0 ? (q = SA = G, 19) : r === 1 ? (q = s, sA -= 257, SA = i, YA -= 257, 256) : (q = h, SA = C, -1), J = F, T = a, tA = x = f = 0, H = -1, l = (AA = 1 << (W = iA)) - 1, r === 1 && 852 < AA || r === 2 && 592 < AA) return 1;
                         for (;;) {
                             for (j = J - tA, gA = G[x] < p ? (b = 0, G[x]) : G[x] > p ? (b = SA[YA + G[x]], q[sA + G[x]]) : (b = 96, 0), c = 1 << J - tA, F = k = 1 << W; N[T + (f >> tA) + (k -= c)] = j << 24 | b << 16 | gA | 0, k !== 0;);
                             for (c = 1 << J - 1; f & c;) c >>= 1;
                             if (c !== 0 ? (f &= c - 1, f += c) : f = 0, x++, --CA[J] == 0) {
                                 if (J === Z) break;
                                 J = n[M + G[x]]
                             }
@@ -7555,15 +7598,15 @@
                         "-5": "buffer error",
                         "-6": "incompatible version"
                     }
                 }, {}],
                 52: [function(g, o, t) {
                     var E = g("../utils/common"),
                         s = 0,
-                        D = 1;
+                        i = 1;
 
                     function h(U) {
                         for (var Y = U.length; 0 <= --Y;) U[Y] = 0
                     }
                     var C = 0,
                         r = 29,
                         n = 256,
@@ -7671,36 +7714,36 @@
                             NA = -1;
                         for (U.heap_len = 0, U.heap_max = a, z = 0; z < wA; z++) IA[2 * z] !== 0 ? (U.heap[++U.heap_len] = NA = z, U.depth[z] = 0) : IA[2 * z + 1] = 0;
                         for (; U.heap_len < 2;) IA[2 * (u = U.heap[++U.heap_len] = NA < 2 ? ++NA : 0)] = 1, U.depth[u] = 0, U.opt_len--, BA && (U.static_len -= EA[2 * u + 1]);
                         for (Y.max_code = NA, z = U.heap_len >> 1; 1 <= z; z--) rA(U, IA, z);
                         for (u = wA; z = U.heap[1], U.heap[1] = U.heap[U.heap_len--], rA(U, IA, 1), P = U.heap[1], U.heap[--U.heap_max] = z, U.heap[--U.heap_max] = P, IA[2 * u] = IA[2 * z] + IA[2 * P], U.depth[u] = (U.depth[z] >= U.depth[P] ? U.depth[z] : U.depth[P]) + 1, IA[2 * z + 1] = IA[2 * P + 1] = u, U.heap[1] = u++, rA(U, IA, 1), 2 <= U.heap_len;);
                         U.heap[--U.heap_max] = U.heap[1],
                             function(RA, lA) {
-                                var QI, qA, wI, JA, UI, hA, xA = lA.dyn_tree,
-                                    JI = lA.max_code,
+                                var QI, qA, wI, JA, GI, hA, xA = lA.dyn_tree,
+                                    KI = lA.max_code,
                                     XA = lA.stat_desc.static_tree,
                                     dg = lA.stat_desc.has_stree,
                                     vA = lA.stat_desc.extra_bits,
-                                    KI = lA.stat_desc.extra_base,
+                                    YI = lA.stat_desc.extra_base,
                                     O = lA.stat_desc.max_length,
                                     BI = 0;
                                 for (JA = 0; JA <= G; JA++) RA.bl_count[JA] = 0;
-                                for (xA[2 * RA.heap[RA.heap_max] + 1] = 0, QI = RA.heap_max + 1; QI < a; QI++) O < (JA = xA[2 * xA[2 * (qA = RA.heap[QI]) + 1] + 1] + 1) && (JA = O, BI++), xA[2 * qA + 1] = JA, JI < qA || (RA.bl_count[JA]++, UI = 0, KI <= qA && (UI = vA[qA - KI]), hA = xA[2 * qA], RA.opt_len += hA * (JA + UI), dg && (RA.static_len += hA * (XA[2 * qA + 1] + UI)));
+                                for (xA[2 * RA.heap[RA.heap_max] + 1] = 0, QI = RA.heap_max + 1; QI < a; QI++) O < (JA = xA[2 * xA[2 * (qA = RA.heap[QI]) + 1] + 1] + 1) && (JA = O, BI++), xA[2 * qA + 1] = JA, KI < qA || (RA.bl_count[JA]++, GI = 0, YI <= qA && (GI = vA[qA - YI]), hA = xA[2 * qA], RA.opt_len += hA * (JA + GI), dg && (RA.static_len += hA * (XA[2 * qA + 1] + GI)));
                                 if (BI !== 0) {
                                     do {
                                         for (JA = O - 1; RA.bl_count[JA] === 0;) JA--;
                                         RA.bl_count[JA]--, RA.bl_count[JA + 1] += 2, RA.bl_count[O]--, BI -= 2
                                     } while (0 < BI);
                                     for (JA = O; JA !== 0; JA--)
-                                        for (qA = RA.bl_count[JA]; qA !== 0;) JI < (wI = RA.heap[--QI]) || (xA[2 * wI + 1] !== JA && (RA.opt_len += (JA - xA[2 * wI + 1]) * xA[2 * wI], xA[2 * wI + 1] = JA), qA--)
+                                        for (qA = RA.bl_count[JA]; qA !== 0;) KI < (wI = RA.heap[--QI]) || (xA[2 * wI + 1] !== JA && (RA.opt_len += (JA - xA[2 * wI + 1]) * xA[2 * wI], xA[2 * wI + 1] = JA), qA--)
                                 }
                             }(U, Y), YA(IA, NA, U.bl_count)
                     }
 
-                    function i(U, Y, z) {
+                    function D(U, Y, z) {
                         var P, u, IA = -1,
                             EA = Y[1],
                             BA = 0,
                             wA = 7,
                             NA = 4;
                         for (EA === 0 && (wA = 138, NA = 3), Y[2 * (z + 1) + 1] = 65535, P = 0; P <= z; P++) u = EA, EA = Y[2 * (P + 1) + 1], ++BA < wA && u === EA || (BA < NA ? U.bl_tree[2 * u] += BA : u !== 0 ? (u !== IA && U.bl_tree[2 * u]++, U.bl_tree[2 * H]++) : BA <= 10 ? U.bl_tree[2 * l]++ : U.bl_tree[2 * T]++, IA = u, NA = (BA = 0) === EA ? (wA = 138, 3) : u === EA ? (wA = 6, 3) : (wA = 7, 4))
                     }
@@ -7747,21 +7790,21 @@
                         }(), V = !0), U.l_desc = new f(U.dyn_ltree, iA), U.d_desc = new f(U.dyn_dtree, W), U.bl_desc = new f(U.bl_tree, tA), U.bi_buf = 0, U.bi_valid = 0, GA(U)
                     }, t._tr_stored_block = L, t._tr_flush_block = function(U, Y, z, P) {
                         var u, IA, EA = 0;
                         0 < U.level ? (U.strm.data_type === 2 && (U.strm.data_type = function(BA) {
                             var wA, NA = 4093624447;
                             for (wA = 0; wA <= 31; wA++, NA >>>= 1)
                                 if (1 & NA && BA.dyn_ltree[2 * wA] !== 0) return s;
-                            if (BA.dyn_ltree[18] !== 0 || BA.dyn_ltree[20] !== 0 || BA.dyn_ltree[26] !== 0) return D;
+                            if (BA.dyn_ltree[18] !== 0 || BA.dyn_ltree[20] !== 0 || BA.dyn_ltree[26] !== 0) return i;
                             for (wA = 32; wA < n; wA++)
-                                if (BA.dyn_ltree[2 * wA] !== 0) return D;
+                                if (BA.dyn_ltree[2 * wA] !== 0) return i;
                             return s
                         }(U)), dA(U, U.l_desc), dA(U, U.d_desc), EA = function(BA) {
                             var wA;
-                            for (i(BA, BA.dyn_ltree, BA.l_desc.max_code), i(BA, BA.dyn_dtree, BA.d_desc.max_code), dA(BA, BA.bl_desc), wA = N - 1; 3 <= wA && BA.bl_tree[2 * gA[wA] + 1] === 0; wA--);
+                            for (D(BA, BA.dyn_ltree, BA.l_desc.max_code), D(BA, BA.dyn_dtree, BA.d_desc.max_code), dA(BA, BA.bl_desc), wA = N - 1; 3 <= wA && BA.bl_tree[2 * gA[wA] + 1] === 0; wA--);
                             return BA.opt_len += 3 * (wA + 1) + 5 + 5 + 4, wA
                         }(U), u = U.opt_len + 3 + 7 >>> 3, (IA = U.static_len + 3 + 7 >>> 3) <= u && (u = IA)) : u = IA = z + 5, z + 4 <= u && Y !== -1 ? L(U, Y, z, P) : U.strategy === 4 || IA === u ? (CA(U, 2 + (P ? 1 : 0), 3), HA(U, oA, J)) : (CA(U, 4 + (P ? 1 : 0), 3), function(BA, wA, NA, RA) {
                             var lA;
                             for (CA(BA, wA - 257, 5), CA(BA, NA - 1, 5), CA(BA, RA - 4, 4), lA = 0; lA < RA; lA++) CA(BA, BA.bl_tree[2 * gA[lA] + 1], 3);
                             X(BA, BA.dyn_ltree, wA - 1), X(BA, BA.dyn_dtree, NA - 1)
                         }(U, U.l_desc.max_code + 1, U.d_desc.max_code + 1, EA + 1), HA(U, U.dyn_ltree, U.dyn_dtree)), GA(U), P && nA(U)
                     }, t._tr_tally = function(U, Y, z) {
@@ -7778,15 +7821,15 @@
                 53: [function(g, o, t) {
                     o.exports = function() {
                         this.input = null, this.next_in = 0, this.avail_in = 0, this.total_in = 0, this.output = null, this.next_out = 0, this.avail_out = 0, this.total_out = 0, this.msg = "", this.state = null, this.data_type = 2, this.adler = 0
                     }
                 }, {}],
                 54: [function(g, o, t) {
                     (function(E) {
-                        (function(s, D) {
+                        (function(s, i) {
                             if (!s.setImmediate) {
                                 var h, C, r, n, M = 1,
                                     R = {},
                                     N = !1,
                                     a = s.document,
                                     G = Object.getPrototypeOf && Object.getPrototypeOf(s);
                                 G = G && G.setTimeout ? G : s, h = {}.toString.call(s.process) === "[object process]" ? function(H) {
@@ -7849,62 +7892,62 @@
                                                     case 2:
                                                         p(j[0], j[1]);
                                                         break;
                                                     case 3:
                                                         p(j[0], j[1], j[2]);
                                                         break;
                                                     default:
-                                                        p.apply(D, j)
+                                                        p.apply(i, j)
                                                 }
                                             })(l)
                                         } finally {
                                             y(H), N = !1
                                         }
                                     }
                                 }
                             }
 
                             function k(H) {
                                 H.source === s && typeof H.data == "string" && H.data.indexOf(n) === 0 && c(+H.data.slice(n.length))
                             }
                         })(typeof self > "u" ? E === void 0 ? this : E : self)
-                    }).call(this, typeof OI < "u" ? OI : typeof self < "u" ? self : typeof window < "u" ? window : {})
+                    }).call(this, typeof XI < "u" ? XI : typeof self < "u" ? self : typeof window < "u" ? window : {})
                 }, {}]
             }, {}, [10])(10)
         })
-    })(ls);
-    const fs = lg;
+    })(us);
+    const ps = lg;
 
-    function ds(A) {
+    function qs(A) {
         for (var B = window.atob(A), g = B.length, o = new Uint8Array(g), t = 0; t < g; t++) o[t] = B.charCodeAt(t);
         return o
     }
-    async function us(A) {
-        const B = await fs.loadAsync(A),
+    async function xs(A) {
+        const B = await ps.loadAsync(A),
             g = Object.keys(B.files)[0];
         return B.files[g].async("uint8array")
     }
-    async function sB(A) {
-        const B = ds(A);
-        return await us(B)
+    async function wB(A) {
+        const B = qs(A);
+        return await xs(B)
     }
 
-    function ps(A, B, g) {
+    function bs(A, B, g) {
         const {
             isReady: o,
             sqlEngine: t,
             sqlDb: E,
             dbFileBs64Storage: s
-        } = Vs(A, B, g), D = qs(C);
+        } = Ts(A, B, g), i = Vs(C);
 
         function h(G) {
             let y = new FileReader;
             y.onload = async function(c) {
                 var k;
-                s.value = (k = c.target) == null ? void 0 : k.result, E.value = new t.value.Database(await sB(s.value))
+                s.value = (k = c.target) == null ? void 0 : k.result, E.value = new t.value.Database(await wB(s.value))
             }, y.readAsText(G, "utf8")
         }
 
         function C(G) {
             let y = null,
                 c = [];
             const k = [];
@@ -7947,15 +7990,15 @@
 
         function n(G, y) {
             const c = `CREATE TABLE ${G} as ${y}`;
             return E.value.run(c), G
         }
 
         function M(G, y, c) {
-            const k = D.getFieldType(G, y);
+            const k = i.getFieldType(G, y);
             return k === "INTEGER" ? parseInt(c, 10) : k === "float" ? parseFloat(c) : typeof c == "string" ? `"${c}"` : c === null ? "null" : c
         }
 
         function R(G) {
             return typeof G == "string" ? `"${G}"` : G === null ? "null" : G
         }
 
@@ -7972,300 +8015,306 @@
         }
         return {
             isReady: o,
             uploadDbFile: h,
             queryAll: C,
             query2tempory: n,
             runOnTransaction: r,
-            getTableFields: D.getTableFields,
-            getFieldType: D.getFieldType,
+            getTableFields: i.getTableFields,
+            getFieldType: i.getFieldType,
             parse2sqlValueBaseFieldType: M,
             parse2sqlValue: R,
             valuesArray2sqlArray: N,
             extractNullInValues: a
         }
     }
 
-    function qs(A) {
+    function Vs(A) {
         const B = new Map;
 
         function g(s) {
             return A(`PRAGMA table_info(${s})`).rows
         }
 
         function o(s) {
             return B.has(s) || B.set(s, g(s)), B.get(s)
         }
 
         function t(s) {
             return o(s).map(h => h.name)
         }
 
-        function E(s, D) {
-            return o(s).filter(C => C.name === D).map(C => C.type)[0]
+        function E(s, i) {
+            return o(s).filter(C => C.name === i).map(C => C.type)[0]
         }
         return {
             getTableFields: t,
             getFieldType: E
         }
     }
 
-    function xs(A) {
+    function ms(A) {
         const B = Uint8Array.from(window.atob(A.file), t => t.charCodeAt(0)).buffer,
             g = new Blob([B], {
                 type: "application/wasm"
             }),
             {
                 state: o
-            } = OQ(async () => await Hs({
+            } = XQ(async () => await ds({
                 locateFile: t => URL.createObjectURL(g)
             }), null);
         return o
     }
 
-    function bs(A, B) {
+    function Zs(A, B) {
         const g = K.ref(null);
         return K.watch([A, B], ([o, t]) => {
             o === null || t === null || (g.value = new o.Database(t))
         }), g
     }
 
-    function Vs(A, B, g) {
-        const o = xs(B),
+    function Ts(A, B, g) {
+        const o = ms(B),
             t = g.getDbFile(),
-            E = bs(o, t),
-            s = Zo("pybi-db", null);
+            E = Zs(o, t),
+            s = Vo("pybi-db", null);
         return {
             isReady: K.computed(() => E.value !== null),
             sqlEngine: o,
             sqlDb: E,
             dbFileBs64Storage: s
         }
     }
 
-    function ms(A, B, g) {
+    function Ws(A, B, g) {
         function o(t, E) {
             const s = B.getTableNames(E);
 
-            function D() {
+            function i() {
                 let h = E;
                 return g.runOnTransaction(() => (s.forEach(C => {
                     const r = A.createSql(C, t);
                     h = B.replaceTableToFilterQuery(h, C, r.value)
                 }), g.queryAll(h)), "ROLLBACK")
             }
             return {
-                query: D
+                query: i
             }
         }
         return {
             createSqlQuery: o
         }
     }
 
-    function Zs(A) {
+    function Os(A) {
         function B(o) {
             const t = A.sqlAnalyze.getTableNames(o.sqlInfo.sql)[0],
                 E = A.utils.createSqlQuery(o.id, o.sqlInfo.sql),
                 s = g(o);
 
-            function D() {
+            function i() {
                 return K.computed(() => E.query())
             }
 
             function h() {
                 A.dataset.removeFilters(o.id, t), s.removeFilter()
             }
             return {
-                getData: D,
+                getData: i,
                 addFilter: s.addFilter,
                 addFilterWithExprFn: s.addFilterWithExprFn,
                 removeFilter: h
             }
         }
 
         function g(o) {
             function t() {
-                o.updateInfos.forEach(D => {
-                    A.dataset.removeFilters(o.id, D.table)
+                o.updateInfos.forEach(i => {
+                    A.dataset.removeFilters(o.id, i.table)
                 })
             }
 
-            function E(D) {
+            function E(i) {
                 o.updateInfos.forEach(h => {
-                    A.dataset.addFilter(o.id, h.table, `${h.field} ${D}`)
+                    A.dataset.addFilter(o.id, h.table, `${h.field} ${i}`)
                 })
             }
 
-            function s(D) {
+            function s(i) {
                 o.updateInfos.forEach(h => {
-                    A.dataset.addFilter(o.id, h.table, D(h.field))
+                    A.dataset.addFilter(o.id, h.table, i(h.field))
                 })
             }
             return {
                 removeFilter: t,
                 addFilter: E,
                 addFilterWithExprFn: s
             }
         }
         return {
             getFilterUtils: B,
             getFilterHandler: g
         }
     }
 
-    function Ts(A) {
+    function Xs(A) {
         const B = new Map;
         A.webResources.forEach(t => {
-            const E = Xs(t);
+            const E = Ps(t);
             B.set(t.id, E)
         });
 
         function g(t) {
             if (!B.has(t)) throw new Error(`web Resource[${t}] not found`);
             return B.get(t)()
         }
 
         function o() {
             const t = g("DbFile"),
                 {
                     state: E
-                } = OQ(async () => await sB(t), null);
+                } = XQ(async () => await wB(t), null);
             return K.readonly(E)
         }
         return {
             getResource: g,
             getDbFile: o
         }
     }
 
     function fg(A) {
         let B = null;
         return () => B || (B = A(), B)
     }
 
-    function Ws(A) {
+    function vs(A) {
         return fg(() => A.input)
     }
 
-    function Os(A) {
+    function js(A) {
         if (A.input) return fg(() => (echarts.registerMap(A.id, {
             geoJSON: A.input
         }), K.ref(!0)));
         const g = A.actionPipe[0].args;
         return fg(() => {
             const {
                 isFinished: t,
                 data: E
-            } = As(g.url, g.options).get().json();
+            } = _o(g.url, g.options).get().json();
             return K.watch(E, s => {
                 echarts.registerMap(A.id, {
                     geoJSON: s
                 })
             }), t
         })
     }
 
-    function Xs(A) {
+    function Ps(A) {
         switch (A.type) {
             case "DbFile":
-                return Ws(A);
+                return vs(A);
             case "echarts-map":
-                return Os(A);
+                return js(A);
             default:
                 throw new Error("not suport")
         }
     }
-    const vs = {
+    const zs = {
     };
 
-    function js(A) {
-        const B = Ts(A),
-            g = ps(A, vs, B),
-            o = cs(A),
-            t = Us(),
-            E = ks(A, {
+    function _s(A) {
+        const B = Xs(A),
+            g = bs(A, zs, B),
+            o = Ms(A),
+            t = cs(),
+            E = Ks(A, {
                 sqlAnalyze: t,
                 component: o,
                 db: g
             }),
-            s = ms(E, t, g),
-            D = Zs({
+            s = Ws(E, t, g),
+            i = Os({
                 dataset: E,
                 sqlAnalyze: t,
                 db: g,
                 utils: s
             });
         return {
             cpServices: o,
             sqlServices: t,
             datasetServices: E,
             dbServices: g,
             utilsServices: s,
-            reactdataServices: D,
+            reactdataServices: i,
             webResourcesServices: B
         }
     }
 
-    function Ps() {
+    function $s() {
         function A() {
             if (document.body.clientWidth < 1e3 && document.body.clientWidth >= 300) {
                 const g = 1 - (1 - (document.body.clientWidth - 300) / 700) * .7;
                 document.documentElement.style.fontSize = `${g*100}%`;
                 return
             }
             document.body.clientWidth < 300 || (document.documentElement.style.fontSize = "100%")
         }
-        WQ("resize", A), A()
+        OQ("resize", A), A()
     }
-    const zs = A => (K.pushScopeId("data-v-553b879a"), A = A(), K.popScopeId(), A),
-        _s = {
+    const Aw = A => (K.pushScopeId("data-v-f536d765"), A = A(), K.popScopeId(), A),
+        Iw = {
             key: 0,
             style: {
                 display: "flex",
                 height: "100vh"
             }
         },
-        $s = [zs(() => K.createElementVNode("p", {
+        gw = [Aw(() => K.createElementVNode("p", {
             style: {
                 margin: "auto"
             }
         }, "加载中", -1))],
-        Aw = K.defineComponent({
+        Qw = K.defineComponent({
             __name: "AppLibs",
             props: {
                 app: null
             },
             setup(A) {
+                var E;
                 const B = A;
-                Ps();
+                $s();
                 const g = B.app;
-                document.title = g.docTitle ?? "pybi-next", console.log(`pybi-next:[${g.version}]`);
-                const o = js(g);
-                K.provide(ZB, o.sqlServices), K.provide(TB, o.cpServices), K.provide(WB, o.datasetServices), K.provide(OB, o.dbServices), K.provide(xI, o.utilsServices), K.provide(XB, o.reactdataServices), K.provide(jB, o.webResourcesServices), K.provide(vB, GI), K.provide(vg, {
+                document.title = g.docTitle ?? "pybi-next", console.log(`pybi-next:[${g.version}]`), (E = g.styleTags) == null || E.forEach(s => {
+                    As(s.css, {
+                        id: s.id,
+                        media: s.media
+                    })
+                });
+                const o = _s(g);
+                K.provide(TB, o.sqlServices), K.provide(WB, o.cpServices), K.provide(OB, o.datasetServices), K.provide(XB, o.dbServices), K.provide(bI, o.utilsServices), K.provide(vB, o.reactdataServices), K.provide(PB, o.webResourcesServices), K.provide(jB, JI), K.provide(vg, {
                     version: g.version
                 });
                 const t = o.dbServices.isReady;
-                return (E, s) => K.unref(t) ? (K.openBlock(), K.createElementBlock("div", {
+                return (s, i) => K.unref(t) ? (K.openBlock(), K.createElementBlock("div", {
                     key: 1,
                     class: K.normalizeClass(["app-box pybi-container", K.unref(g).classes]),
                     style: K.normalizeStyle(K.unref(g).styles)
-                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(g).children, D => (K.openBlock(), K.createBlock(GI, {
-                    component: D
-                }, null, 8, ["component"]))), 256))], 6)) : (K.openBlock(), K.createElementBlock("div", _s, $s))
+                }, [(K.openBlock(!0), K.createElementBlock(K.Fragment, null, K.renderList(K.unref(g).children, h => (K.openBlock(), K.createBlock(JI, {
+                    component: h
+                }, null, 8, ["component"]))), 256))], 6)) : (K.openBlock(), K.createElementBlock("div", Iw, gw))
             }
         }),
-        $w = "",
-        Iw = WA(Aw, [
-            ["__scopeId", "data-v-553b879a"]
+        gt = "",
+        Bw = WA(Qw, [
+            ["__scopeId", "data-v-f536d765"]
         ]);
 
-    function gw(A) {
-        return K.createApp(Iw, {
+    function Cw(A) {
+        return K.createApp(Bw, {
             app: A
         })
     }
     return {
-        initApp: gw
+        initApp: Cw
     }
 }(Vue);
```

### Comparing `pybi-next-0.4.1/pybi/static/vue.global.prod.min.js` & `pybi-next-0.4.2/pybi/static/vue.global.prod.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/template/index.html` & `pybi-next-0.4.2/pybi/template/index.html`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/dataSourceUtils.py` & `pybi-next-0.4.2/pybi/utils/dataSourceUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/data_gen.py` & `pybi-next-0.4.2/pybi/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/dictUtils.py` & `pybi-next-0.4.2/pybi/utils/dictUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/echarts_opts_utils.py` & `pybi-next-0.4.2/pybi/utils/echarts_opts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/helper.py` & `pybi-next-0.4.2/pybi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/markdown2.py` & `pybi-next-0.4.2/pybi/utils/markdown2.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/pyecharts_utils.py` & `pybi-next-0.4.2/pybi/utils/pyecharts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi/utils/sql.py` & `pybi-next-0.4.2/pybi/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.1/pybi_next.egg-info/SOURCES.txt` & `pybi-next-0.4.2/pybi_next.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,30 @@
 pybi/core/components/reactiveComponent/input.py
 pybi/core/components/reactiveComponent/markdown.py
 pybi/core/components/reactiveComponent/numberSlider.py
 pybi/core/components/reactiveComponent/slicer.py
 pybi/core/components/reactiveComponent/table.py
 pybi/core/components/reactiveComponent/textValue.py
 pybi/core/styles/__init__.py
+pybi/core/styles/styleTag.py
 pybi/core/styles/styles.py
 pybi/core/styles/utils.py
 pybi/core/styles/tailwindStyles/__init__.py
 pybi/core/styles/tailwindStyles/boxShadow.py
 pybi/core/styles/tailwindStyles/textAlign.py
 pybi/core/styles/tailwindStyles/textColor.py
 pybi/core/styles/tailwindStyles/textSize.py
 pybi/easyEcharts/__init__.py
 pybi/easyEcharts/bar.py
 pybi/easyEcharts/base.py
+pybi/easyEcharts/candlestick.py
 pybi/easyEcharts/line.py
 pybi/easyEcharts/map.py
 pybi/easyEcharts/pie.py
+pybi/easyEcharts/radar.py
 pybi/easyEcharts/scatter.py
 pybi/easyEcharts/utils.py
 pybi/icons/__init__.py
 pybi/icons/iconManager.py
 pybi/icons/material_icons.py
 pybi/static/echarts.min.js
 pybi/static/echartsCps-style.css
```

### Comparing `pybi-next-0.4.1/setup.py` & `pybi-next-0.4.2/setup.py`

 * *Files identical despite different names*
