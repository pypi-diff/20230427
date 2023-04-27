# Comparing `tmp/PyQtGuiLib-2.8.20.0.tar.gz` & `tmp/PyQtGuiLib-2.8.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-2.8.20.0.tar", last modified: Tue Apr 25 08:32:57 2023, max compression
+gzip compressed data, was "PyQtGuiLib-2.8.21.0.tar", last modified: Thu Apr 27 03:49:56 2023, max compression
```

## Comparing `PyQtGuiLib-2.8.20.0.tar` & `PyQtGuiLib-2.8.21.0.tar`

### file list

```diff
@@ -1,247 +1,251 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.248136 PyQtGuiLib-2.8.20.0/
--rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.8.20.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.005160 PyQtGuiLib-2.8.20.0/Log/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/Log/__init__.py
--rw-rw-rw-   0        0        0    10517 2023-04-25 08:27:49.000000 PyQtGuiLib-2.8.20.0/Log/developmentLog.py
--rw-rw-rw-   0        0        0    17824 2023-04-25 08:32:57.247138 PyQtGuiLib-2.8.20.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.006157 PyQtGuiLib-2.8.20.0/PyQtGuiLib/
--rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.016132 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0     6805 2023-04-20 03:22:30.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/PropertyAnimation.py
--rw-rw-rw-   0        0        0      232 2023-04-25 06:49:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0     6552 2023-04-20 09:28:51.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/animation.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.029096 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0      682 2023-04-25 08:12:03.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/__init__.py
--rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/bubbleWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.031090 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/
--rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboBox.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.036077 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/
--rw-rw-rw-   0        0        0      107 2023-04-25 08:09:32.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
--rw-rw-rw-   0        0        0    21095 2023-04-25 08:15:03.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
--rw-rw-rw-   0        0        0     2327 2023-04-25 08:09:33.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
--rw-rw-rw-   0        0        0    28106 2023-04-25 03:37:41.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.038072 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-04-25 06:51:00.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/drawer.py
--rw-rw-rw-   0        0        0     4203 2023-04-17 07:41:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/expansionBar.py
--rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/flowLayout.py
--rw-rw-rw-   0        0        0     2583 2023-04-17 06:05:25.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/imageButton.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.040067 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/
--rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/dynamicTLine.py
--rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/listWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.046079 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/
--rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/loadLogTh.py
--rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logBrowser.py
--rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logSizeTh.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.048045 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/
--rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/notice.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.051037 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/__init__.py
--rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/colorHsv.py
--rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/paletteFrame.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.058035 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularBar.py
--rw-rw-rw-   0        0        0     6372 2023-04-25 07:41:31.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularProgressBar.py
--rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/gradientBar.py
--rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/loadBar.py
--rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/waterBar.py
--rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/pullOver.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.061027 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/
--rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/__init__.py
--rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/controls.py
--rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/rollWidget.py
--rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.063022 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/
--rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/__init__.py
--rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/slider.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.065024 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/swButton.py
--rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolBox.py
--rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.071998 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/
--rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/WidgetABC.py
--rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/statusBar.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.075987 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/
--rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/1.py
--rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/2.py
--rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/__init__.py
--rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.082968 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.089949 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     5834 2023-04-25 06:29:09.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0      534 2023-04-25 05:53:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0      502 2023-04-25 05:53:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0      460 2023-04-25 04:13:46.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      763 2023-04-25 05:46:15.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-25 05:54:19.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/customStyle.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.091944 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     3658 2023-04-25 05:55:44.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.094936 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/
--rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.096931 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/
--rw-rw-rw-   0        0        0      107 2023-04-20 06:55:28.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/__init__.py
--rw-rw-rw-   0        0        0     2729 2023-04-20 09:11:21.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/particle.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.100921 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      364 2023-04-25 07:58:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.105907 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/
--rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
--rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
--rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
--rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.107901 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/__init__.py
--rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/buttonStyle.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.111891 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.114883 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/config.py
--rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.118872 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/
--rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/image_rc.py
--rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/qssFile.py
--rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/qssFile.py
--rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/test.py
--rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/skinABC.py
--rw-rw-rw-   0        0        0     8591 2023-04-24 09:43:40.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.121864 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    13068 2023-04-21 01:53:12.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.122862 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.125854 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/
--rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.127848 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/
--rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/__init__.py
--rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
--rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.012170 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/
--rw-rw-rw-   0        0        0    17824 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6721 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-25 08:32:56.000000 PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.8.20.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.137833 PyQtGuiLib-2.8.20.0/abandonCase/
--rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.143416 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/
--rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/acrylicWidget.py
--rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/cstruct.py
--rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/acrylic/windowEffect.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.150397 PyQtGuiLib-2.8.20.0/abandonCase/animation/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/__init__.py
--rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animation.py
--rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationDrawType.py
--rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationFactory.py
--rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/animationLayout.py
--rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.8.20.0/abandonCase/animation/customAniTest.py
--rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget.py
--rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget_case.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.156381 PyQtGuiLib-2.8.20.0/abandonCase/linker/
--rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/component.py
--rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/controlType.py
--rw-rw-rw-   0        0        0    11488 2023-04-25 08:02:33.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinker.py
--rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinkerUi.py
--rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/nodeBar.py
--rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/slideShow.py
--rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/slideShow2.py
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/spaceWidget.py
--rw-rw-rw-   0        0        0    17813 2023-04-25 08:21:59.000000 PyQtGuiLib-2.8.20.0/abandonCase/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.170344 PyQtGuiLib-2.8.20.0/abandonCase/widgets/
--rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessFrame.py
--rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessStackedWidget.py
--rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidgetABC.py
--rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/statusBar.py
--rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/abandonCase/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.173337 PyQtGuiLib-2.8.20.0/auxiliaryMeans/
--rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.8.20.0/auxiliaryMeans/__init__.py
--rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.8.20.0/auxiliaryMeans/toolNewProject.py
--rw-rw-rw-   0        0        0       42 2023-04-25 08:32:57.248136 PyQtGuiLib-2.8.20.0/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-25 08:26:52.000000 PyQtGuiLib-2.8.20.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.214227 PyQtGuiLib-2.8.20.0/tests/
--rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.8.20.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.217218 PyQtGuiLib-2.8.20.0/tests/test_Animation/
--rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.220212 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-04-25 07:55:39.000000 PyQtGuiLib-2.8.20.0/tests/test_Animation/test_animation.py
--rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_BubbleWidget.py
--rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.8.20.0/tests/test_CircularProgressBar.py
--rw-rw-rw-   0        0        0     1288 2023-04-25 08:18:48.000000 PyQtGuiLib-2.8.20.0/tests/test_ComboCheckBox.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.8.20.0/tests/test_Notice.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.230184 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg1.py
--rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg2.py
--rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg3.py
--rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg4.py
--rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg5.py
--rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg6.py
--rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg7.py
--rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/test.py
--rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis.py
--rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.8.20.0/tests/test_SlideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.239161 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/
--rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/1.py
--rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg1.py
--rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg2.py
--rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg3.py
--rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg4.py
--rw-rw-rw-   0        0        0     2538 2023-04-21 02:10:44.000000 PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/test.py
--rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.8.20.0/tests/test_barset.py
--rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_circularBar.py
--rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_colorPalette.py
--rw-rw-rw-   0        0        0     1161 2023-04-21 06:51:11.000000 PyQtGuiLib-2.8.20.0/tests/test_drawer.py
--rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_dumpStructure.py
--rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_dynamicTLine.py
--rw-rw-rw-   0        0        0      613 2023-04-17 06:35:12.000000 PyQtGuiLib-2.8.20.0/tests/test_expansionBar.py
--rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_flowLayot.py
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_gradientBar.py
--rw-rw-rw-   0        0        0      903 2023-04-17 05:57:17.000000 PyQtGuiLib-2.8.20.0/tests/test_imageButton.py
--rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_listWidget.py
--rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_loadbar.py
--rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_no_border.py
--rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_no_border_pullOver.py
--rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_pullOverWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.242152 PyQtGuiLib-2.8.20.0/tests/test_qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.8.20.0/tests/test_qssFile/__init__.py
--rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.8.20.0/tests/test_qssFile/test.py
--rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_rollWidget.py
--rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_slider.py
--rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.8.20.0/tests/test_statusBar.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_styles.py
--rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_switchButton.py
--rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.8.20.0/tests/test_template.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.244146 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/
--rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/__init__.py
--rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.8.20.0/tests/test_templateWindow/test_listTemplateWindow.py
--rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.8.20.0/tests/test_toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-25 08:32:57.246141 PyQtGuiLib-2.8.20.0/tests/test_uic/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_uic/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_uic/test_uic.py
--rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.20.0/tests/test_waterBar.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.584079 PyQtGuiLib-2.8.21.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.8.21.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.358631 PyQtGuiLib-2.8.21.0/Log/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/Log/__init__.py
+-rw-rw-rw-   0        0        0    10719 2023-04-26 01:52:39.000000 PyQtGuiLib-2.8.21.0/Log/developmentLog.py
+-rw-rw-rw-   0        0        0    17824 2023-04-27 03:49:56.583083 PyQtGuiLib-2.8.21.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.359627 PyQtGuiLib-2.8.21.0/PyQtGuiLib/
+-rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.370599 PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0     6805 2023-04-20 03:22:30.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/PropertyAnimation.py
+-rw-rw-rw-   0        0        0      232 2023-04-25 06:49:49.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0     6552 2023-04-20 09:28:51.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/animation.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.383563 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      763 2023-04-26 01:41:17.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/__init__.py
+-rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/bubbleWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.386555 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/
+-rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboBox.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.390889 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/
+-rw-rw-rw-   0        0        0      107 2023-04-25 08:09:32.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
+-rw-rw-rw-   0        0        0    21095 2023-04-25 08:15:03.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
+-rw-rw-rw-   0        0        0     2327 2023-04-25 08:09:33.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
+-rw-rw-rw-   0        0        0    28106 2023-04-25 03:37:41.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.392885 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/drawers/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/drawers/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-04-25 06:51:00.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/drawers/drawer.py
+-rw-rw-rw-   0        0        0     4203 2023-04-17 07:41:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/expansionBar.py
+-rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/flowLayout.py
+-rw-rw-rw-   0        0        0     2583 2023-04-17 06:05:25.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/imageButton.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.394880 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/lineedit/
+-rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/lineedit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/lineedit/dynamicTLine.py
+-rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/listWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.399492 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/
+-rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/loadLogTh.py
+-rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/logBrowser.py
+-rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/logSizeTh.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.400491 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/notice/
+-rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/notice/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/notice/notice.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.403483 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/pager/
+-rw-rw-rw-   0        0        0      106 2023-04-26 01:41:17.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/pager/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-04-26 01:48:10.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/pager/pageCuttingButtonGroup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.406476 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.413457 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/circularBar.py
+-rw-rw-rw-   0        0        0     6372 2023-04-25 07:41:31.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/circularProgressBar.py
+-rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/loadBar.py
+-rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/waterBar.py
+-rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/pullOver.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.415451 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/resolver/
+-rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/resolver/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/resolver/controls.py
+-rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/rollWidget.py
+-rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.417446 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slider/
+-rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slider/__init__.py
+-rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slider/slider.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.419441 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/switchButtons/swButton.py
+-rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/toolBox.py
+-rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.426190 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/
+-rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/WidgetABC.py
+-rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/statusBar.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.429182 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/tets/
+-rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/tets/1.py
+-rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/tets/2.py
+-rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/tets/__init__.py
+-rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.434169 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.442148 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     6038 2023-04-26 01:43:34.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0      534 2023-04-25 05:53:49.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 05:53:10.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0      460 2023-04-25 04:13:46.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      763 2023-04-25 05:46:15.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-25 05:54:19.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/customStyle.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.444142 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     3658 2023-04-25 05:55:44.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.446137 PyQtGuiLib-2.8.21.0/PyQtGuiLib/layoutDeformation/
+-rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/layoutDeformation/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/layoutDeformation/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.448131 PyQtGuiLib-2.8.21.0/PyQtGuiLib/particle/
+-rw-rw-rw-   0        0        0      107 2023-04-20 06:55:28.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/particle/__init__.py
+-rw-rw-rw-   0        0        0     2729 2023-04-20 09:11:21.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/particle/particle.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.452121 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      364 2023-04-25 07:58:50.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.456110 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/
+-rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
+-rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
+-rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.458105 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/buttons/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/buttons/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/buttons/buttonStyle.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.462096 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.466085 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/drak/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/drak/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/drak/config.py
+-rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.469077 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/image/
+-rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/image/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/image/image_rc.py
+-rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/image/qssFile.py
+-rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/qssFile.py
+-rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/test.py
+-rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/skinABC.py
+-rw-rw-rw-   0        0        0     8593 2023-04-26 10:22:16.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.471072 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    13068 2023-04-21 01:53:12.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/superPainter/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.472069 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.474063 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/UI/
+-rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/UI/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.476058 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/Window/
+-rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/Window/__init__.py
+-rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.365612 PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/
+-rw-rw-rw-   0        0        0    17824 2023-04-27 03:49:56.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6840 2023-04-27 03:49:56.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 03:49:56.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-27 03:49:56.000000 PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.8.21.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.485721 PyQtGuiLib-2.8.21.0/abandonCase/
+-rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.489729 PyQtGuiLib-2.8.21.0/abandonCase/acrylic/
+-rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/acrylic/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/acrylic/acrylicWidget.py
+-rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/acrylic/cstruct.py
+-rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/acrylic/windowEffect.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.496692 PyQtGuiLib-2.8.21.0/abandonCase/animation/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/__init__.py
+-rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/animation.py
+-rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/animationDrawType.py
+-rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/animationFactory.py
+-rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/animationLayout.py
+-rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.8.21.0/abandonCase/animation/customAniTest.py
+-rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/bubbleWidget.py
+-rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/bubbleWidget_case.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.503673 PyQtGuiLib-2.8.21.0/abandonCase/linker/
+-rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.8.21.0/abandonCase/linker/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.8.21.0/abandonCase/linker/component.py
+-rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/linker/controlType.py
+-rw-rw-rw-   0        0        0    11488 2023-04-25 08:02:33.000000 PyQtGuiLib-2.8.21.0/abandonCase/linker/styleLinker.py
+-rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.8.21.0/abandonCase/linker/styleLinkerUi.py
+-rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/nodeBar.py
+-rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/slideShow.py
+-rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/slideShow2.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/spaceWidget.py
+-rw-rw-rw-   0        0        0    17813 2023-04-25 08:21:59.000000 PyQtGuiLib-2.8.21.0/abandonCase/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.512650 PyQtGuiLib-2.8.21.0/abandonCase/widgets/
+-rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessFrame.py
+-rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessStackedWidget.py
+-rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessWidgetABC.py
+-rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/statusBar.py
+-rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/abandonCase/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.514645 PyQtGuiLib-2.8.21.0/auxiliaryMeans/
+-rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.8.21.0/auxiliaryMeans/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.8.21.0/auxiliaryMeans/toolNewProject.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 03:49:56.584079 PyQtGuiLib-2.8.21.0/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-27 03:48:38.000000 PyQtGuiLib-2.8.21.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.550169 PyQtGuiLib-2.8.21.0/tests/
+-rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.8.21.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.553161 PyQtGuiLib-2.8.21.0/tests/test_Animation/
+-rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.8.21.0/tests/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.8.21.0/tests/test_Animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.556153 PyQtGuiLib-2.8.21.0/tests/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.8.21.0/tests/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.8.21.0/tests/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-04-25 07:55:39.000000 PyQtGuiLib-2.8.21.0/tests/test_Animation/test_animation.py
+-rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_BubbleWidget.py
+-rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.8.21.0/tests/test_CircularProgressBar.py
+-rw-rw-rw-   0        0        0     1288 2023-04-25 08:18:48.000000 PyQtGuiLib-2.8.21.0/tests/test_ComboCheckBox.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.8.21.0/tests/test_Notice.py
+-rw-rw-rw-   0        0        0     1829 2023-04-26 01:49:56.000000 PyQtGuiLib-2.8.21.0/tests/test_PageCuttingButtonGroup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.567124 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg1.py
+-rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg2.py
+-rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg3.py
+-rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg4.py
+-rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg5.py
+-rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg6.py
+-rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg7.py
+-rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/test.py
+-rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis.py
+-rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.8.21.0/tests/test_SlideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.575103 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/
+-rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/1.py
+-rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/__init__.py
+-rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg1.py
+-rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg2.py
+-rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg3.py
+-rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg4.py
+-rw-rw-rw-   0        0        0     2538 2023-04-21 02:10:44.000000 PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/test.py
+-rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.8.21.0/tests/test_barset.py
+-rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_circularBar.py
+-rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_colorPalette.py
+-rw-rw-rw-   0        0        0     1161 2023-04-21 06:51:11.000000 PyQtGuiLib-2.8.21.0/tests/test_drawer.py
+-rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_dumpStructure.py
+-rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_dynamicTLine.py
+-rw-rw-rw-   0        0        0      613 2023-04-17 06:35:12.000000 PyQtGuiLib-2.8.21.0/tests/test_expansionBar.py
+-rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_flowLayot.py
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_gradientBar.py
+-rw-rw-rw-   0        0        0      903 2023-04-17 05:57:17.000000 PyQtGuiLib-2.8.21.0/tests/test_imageButton.py
+-rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_listWidget.py
+-rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_loadbar.py
+-rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_no_border.py
+-rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_no_border_pullOver.py
+-rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_pullOverWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.577097 PyQtGuiLib-2.8.21.0/tests/test_qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.8.21.0/tests/test_qssFile/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.8.21.0/tests/test_qssFile/test.py
+-rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_rollWidget.py
+-rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_slider.py
+-rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.8.21.0/tests/test_statusBar.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_styles.py
+-rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_switchButton.py
+-rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.8.21.0/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.579098 PyQtGuiLib-2.8.21.0/tests/test_templateWindow/
+-rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.21.0/tests/test_templateWindow/__init__.py
+-rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.8.21.0/tests/test_templateWindow/test_listTemplateWindow.py
+-rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.8.21.0/tests/test_toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:49:56.582086 PyQtGuiLib-2.8.21.0/tests/test_uic/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_uic/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_uic/test_uic.py
+-rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.21.0/tests/test_waterBar.py
```

### Comparing `PyQtGuiLib-2.8.20.0/LICENSE.txt` & `PyQtGuiLib-2.8.21.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/Log/developmentLog.py` & `PyQtGuiLib-2.8.21.0/Log/developmentLog.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,18 @@
     -所有由其他人贡献的功能模块里面都会有一个author()方法来记录作者信息
     -新增控件ComboCheckBox,该控件是一个具体提示的输入框,同时也是一个多项选择框,
         控件由 "PyQt5学习爱好群-知行合一" 贡献
         该控件目前PySide系列支持性比较好,PyQt系列存在提示BUG
         导入方式 from PyQtGuiLib.core import ComboCheckBox
     -删除老版本的超级画师代码,重构版本的超级画师目前代码提示还不完善
     -目前所有文档还未更新,
+2023.4.26
+    新增控件 PageCuttingButtonGroup 分页组件
+        控件由 "PyQt5学习爱好群-(讨厌自己)" 贡献
+        导入方式 from PyQtGuiLib.core import PageCuttingButtonGroup
 '''
 
 
 # -------------------------------
 '''
     暂时搁浅的任务
 1.新无边框窗口主窗口,(还没有设计完成,暂时先放下 2023.1.31)
```

### Comparing `PyQtGuiLib-2.8.20.0/PKG-INFO` & `PyQtGuiLib-2.8.21.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.8.20.0
+Version: 2.8.21.0
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/PropertyAnimation.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/PropertyAnimation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/__init__.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 from PyQtGuiLib.core.listWidget import ListWidget
 from PyQtGuiLib.core.rollWidget import RollWidget
 from PyQtGuiLib.core.palettes.paletteFrame import PaletteFrame
 from PyQtGuiLib.core.notice.notice import Notice,Notices
 from PyQtGuiLib.core.slider.slider import Slider
 from PyQtGuiLib.core.toolList import ToolListWidget,ToolListItem
 from PyQtGuiLib.core.drawers.drawer import DrawerItem,Drawer
-from PyQtGuiLib.core.comboBox.comboCheckBox.comboCheckBox import ComboCheckBox
+from PyQtGuiLib.core.comboBox.comboCheckBox.comboCheckBox import ComboCheckBox
+from PyQtGuiLib.core.pager.pageCuttingButtonGroup import PageCuttingButtonGroup
```

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/bubbleWidget.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboBox.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/drawers/drawer.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/drawers/drawer.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/expansionBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/expansionBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/flowLayout.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/imageButton.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/imageButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/lineedit/dynamicTLine.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/lineedit/dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/listWidget.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/loadLogTh.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/loadLogTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logBrowser.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/logBrowser.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/logBrowser/logSizeTh.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/logBrowser/logSizeTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/notice/notice.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/notice/notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/colorHsv.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/colorHsv.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/palettes/paletteFrame.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/palettes/paletteFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/circularProgressBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/circularProgressBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/loadBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/loadBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/progressBar/waterBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/progressBar/waterBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/pullOver.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/resolver/controls.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/resolver/controls.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/rollWidget.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slideShow.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/slider/slider.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/slider/slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolBox.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/toolBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/toolList.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/WidgetABC.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/WidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/statusBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/tets/2.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/tets/2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/core/widgets/titleBar.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/core/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qt.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     AscendingOrder=Qt.AscendingOrder
     DescendingOrder = Qt.DescendingOrder
     MatchContains = Qt.MatchContains
     PopupCompletion = QCompleter.PopupCompletion
     Key_Enter = Qt.Key_Enter
     Key_Backspace = Qt.Key_Backspace
     Key_Return = Qt.Key_Return
+    PointingHandCursor = Qt.PointingHandCursor
+    ForbiddenCursor = Qt.ForbiddenCursor
 
 
 if PYQT_VERSIONS in ["PyQt6","PySide2","PySide6"]:
     WindowTransparentForInput = Qt.WindowType.WindowTransparentForInput
     FramelessWindowHint = Qt.WindowType.FramelessWindowHint
     Window = Qt.WindowType.Window
     WindingFill = Qt.FillRule.WindingFill
@@ -136,7 +138,9 @@
     AscendingOrder = Qt.SortOrder.AscendingOrder
     DescendingOrder = Qt.SortOrder.DescendingOrder
     MatchContains = Qt.MatchFlag.MatchContains
     PopupCompletion = QCompleter.CompletionMode.PopupCompletion
     Key_Enter = Qt.Key.Key_Enter
     Key_Backspace = Qt.Key.Key_Backspace
     Key_Return = Qt.Key.Key_Return
+    PointingHandCursor = Qt.CursorShape.PointingHandCursor
+    ForbiddenCursor = Qt.CursorShape.ForbiddenCursor
```

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/Qt/qtCore.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/Qt/qtCore.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/__init__.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/customStyle.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/customStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/header/utility.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/layoutDeformation/test.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/layoutDeformation/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/particle/particle.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/particle/particle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/buttons/buttonStyle.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/buttons/buttonStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/image/image_rc.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/image/image_rc.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/qssFile.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/qssFile.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/qssFile/test.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/skinABC.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/skinABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 import typing
 import re
 
 Ang = typing.TypeVar("Any",str,int)
 
 
-def dictTostr(qss_dict)->str:
+def dictTostr(qss_dict) -> str:
     combination = ""
     for selector, attribute in qss_dict.items():
         combination += selector + "{\n"
         for attrk, attrv in attribute.items():
             combination += "%s:%s;\n" % (attrk, attrv)
         combination += "}\n"
     return combination
```

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/PKG-INFO` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.8.20.0
+Version: 2.8.21.0
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.8.20.0/PyQtGuiLib.egg-info/SOURCES.txt` & `PyQtGuiLib-2.8.21.0/PyQtGuiLib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 PyQtGuiLib/core/lineedit/dynamicTLine.py
 PyQtGuiLib/core/logBrowser/__init__.py
 PyQtGuiLib/core/logBrowser/loadLogTh.py
 PyQtGuiLib/core/logBrowser/logBrowser.py
 PyQtGuiLib/core/logBrowser/logSizeTh.py
 PyQtGuiLib/core/notice/__init__.py
 PyQtGuiLib/core/notice/notice.py
+PyQtGuiLib/core/pager/__init__.py
+PyQtGuiLib/core/pager/pageCuttingButtonGroup.py
 PyQtGuiLib/core/palettes/__init__.py
 PyQtGuiLib/core/palettes/colorHsv.py
 PyQtGuiLib/core/palettes/paletteFrame.py
 PyQtGuiLib/core/progressBar/__init__.py
 PyQtGuiLib/core/progressBar/circularBar.py
 PyQtGuiLib/core/progressBar/circularProgressBar.py
 PyQtGuiLib/core/progressBar/gradientBar.py
@@ -139,14 +141,15 @@
 auxiliaryMeans/__init__.py
 auxiliaryMeans/toolNewProject.py
 tests/__init__.py
 tests/test_BubbleWidget.py
 tests/test_CircularProgressBar.py
 tests/test_ComboCheckBox.py
 tests/test_Notice.py
+tests/test_PageCuttingButtonGroup.py
 tests/test_QssStyleAnalysis.py
 tests/test_SlideShow.py
 tests/test_barset.py
 tests/test_circularBar.py
 tests/test_colorPalette.py
 tests/test_drawer.py
 tests/test_dumpStructure.py
```

### Comparing `PyQtGuiLib-2.8.20.0/README.md` & `PyQtGuiLib-2.8.21.0/README.md`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/acrylicWidget.py` & `PyQtGuiLib-2.8.21.0/abandonCase/acrylic/acrylicWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/cstruct.py` & `PyQtGuiLib-2.8.21.0/abandonCase/acrylic/cstruct.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/acrylic/windowEffect.py` & `PyQtGuiLib-2.8.21.0/abandonCase/acrylic/windowEffect.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/animation/animation.py` & `PyQtGuiLib-2.8.21.0/abandonCase/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationDrawType.py` & `PyQtGuiLib-2.8.21.0/abandonCase/animation/animationDrawType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationFactory.py` & `PyQtGuiLib-2.8.21.0/abandonCase/animation/animationFactory.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/animation/animationLayout.py` & `PyQtGuiLib-2.8.21.0/abandonCase/animation/animationLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/animation/customAniTest.py` & `PyQtGuiLib-2.8.21.0/abandonCase/animation/customAniTest.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget.py` & `PyQtGuiLib-2.8.21.0/abandonCase/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/bubbleWidget_case.py` & `PyQtGuiLib-2.8.21.0/abandonCase/bubbleWidget_case.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/linker/component.py` & `PyQtGuiLib-2.8.21.0/abandonCase/linker/component.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/linker/controlType.py` & `PyQtGuiLib-2.8.21.0/abandonCase/linker/controlType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinker.py` & `PyQtGuiLib-2.8.21.0/abandonCase/linker/styleLinker.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/linker/styleLinkerUi.py` & `PyQtGuiLib-2.8.21.0/abandonCase/linker/styleLinkerUi.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/nodeBar.py` & `PyQtGuiLib-2.8.21.0/abandonCase/nodeBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/slideShow.py` & `PyQtGuiLib-2.8.21.0/abandonCase/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/slideShow2.py` & `PyQtGuiLib-2.8.21.0/abandonCase/slideShow2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/superPainter.py` & `PyQtGuiLib-2.8.21.0/abandonCase/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessFrame.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessStackedWidget.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessStackedWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidget.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/borderlessWidgetABC.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/borderlessWidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/statusBar.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/abandonCase/widgets/titleBar.py` & `PyQtGuiLib-2.8.21.0/abandonCase/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/auxiliaryMeans/toolNewProject.py` & `PyQtGuiLib-2.8.21.0/auxiliaryMeans/toolNewProject.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/setup.py` & `PyQtGuiLib-2.8.21.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib",
     packages =find_packages(),
-    version="2.8.20.0",
+    version="2.8.21.0",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib",
     classifiers = [
```

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_Animation/1.py` & `PyQtGuiLib-2.8.21.0/tests/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_Animation/__init__.py` & `PyQtGuiLib-2.8.21.0/tests/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_Animation/test_ani/1.py` & `PyQtGuiLib-2.8.21.0/tests/test_Animation/test_ani/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_Animation/test_animation.py` & `PyQtGuiLib-2.8.21.0/tests/test_Animation/test_animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_BubbleWidget.py` & `PyQtGuiLib-2.8.21.0/tests/test_BubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_CircularProgressBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_CircularProgressBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_ComboCheckBox.py` & `PyQtGuiLib-2.8.21.0/tests/test_ComboCheckBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_Notice.py` & `PyQtGuiLib-2.8.21.0/tests/test_Notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/__init__.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg1.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg2.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg3.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg4.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg5.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg6.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/eg7.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/eg7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis/test.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_QssStyleAnalysis.py` & `PyQtGuiLib-2.8.21.0/tests/test_QssStyleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SlideShow.py` & `PyQtGuiLib-2.8.21.0/tests/test_SlideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/1.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg1.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg2.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg3.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/eg4.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_SuperPainter/test.py` & `PyQtGuiLib-2.8.21.0/tests/test_SuperPainter/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_barset.py` & `PyQtGuiLib-2.8.21.0/tests/test_barset.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_circularBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_colorPalette.py` & `PyQtGuiLib-2.8.21.0/tests/test_colorPalette.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_drawer.py` & `PyQtGuiLib-2.8.21.0/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_dynamicTLine.py` & `PyQtGuiLib-2.8.21.0/tests/test_dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_expansionBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_expansionBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_flowLayot.py` & `PyQtGuiLib-2.8.21.0/tests/test_flowLayot.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_gradientBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_imageButton.py` & `PyQtGuiLib-2.8.21.0/tests/test_imageButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_listWidget.py` & `PyQtGuiLib-2.8.21.0/tests/test_listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_loadbar.py` & `PyQtGuiLib-2.8.21.0/tests/test_loadbar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_no_border.py` & `PyQtGuiLib-2.8.21.0/tests/test_no_border.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_no_border_pullOver.py` & `PyQtGuiLib-2.8.21.0/tests/test_no_border_pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_pullOverWidget.py` & `PyQtGuiLib-2.8.21.0/tests/test_pullOverWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_qssFile/test.py` & `PyQtGuiLib-2.8.21.0/tests/test_qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_rollWidget.py` & `PyQtGuiLib-2.8.21.0/tests/test_rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_slider.py` & `PyQtGuiLib-2.8.21.0/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_statusBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_styles.py` & `PyQtGuiLib-2.8.21.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_switchButton.py` & `PyQtGuiLib-2.8.21.0/tests/test_switchButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_template.py` & `PyQtGuiLib-2.8.21.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_templateWindow/test_listTemplateWindow.py` & `PyQtGuiLib-2.8.21.0/tests/test_templateWindow/test_listTemplateWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_toolList.py` & `PyQtGuiLib-2.8.21.0/tests/test_toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.20.0/tests/test_waterBar.py` & `PyQtGuiLib-2.8.21.0/tests/test_waterBar.py`

 * *Files identical despite different names*

