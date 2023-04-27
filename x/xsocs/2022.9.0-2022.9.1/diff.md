# Comparing `tmp/xsocs-2022.9.0.tar.gz` & `tmp/xsocs-2022.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsocs-2022.9.0.tar", last modified: Fri Sep 16 13:40:33 2022, max compression
+gzip compressed data, was "xsocs-2022.9.1.tar", last modified: Mon Sep 19 13:04:07 2022, max compression
```

## Comparing `xsocs-2022.9.0.tar` & `xsocs-2022.9.1.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.891885 xsocs-2022.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     4324 2022-09-16 13:30:47.000000 xsocs-2022.9.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     1101 2022-09-16 09:38:19.000000 xsocs-2022.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-09-16 09:38:19.000000 xsocs-2022.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2059 2022-09-16 13:40:33.891885 xsocs-2022.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1034 2022-09-16 09:38:19.000000 xsocs-2022.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.775885 xsocs-2022.9.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7705 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/fileformat.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.775885 xsocs-2022.9.0/doc/img/
--rw-rw-rw-   0 root         (0) root         (0)    99637 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/img/input_file.png
--rw-rw-rw-   0 root         (0) root         (0)     1032 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2664 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1313 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/troubleshooting.rst
--rw-rw-rw-   0 root         (0) root         (0)     1204 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/tutorials.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.795885 xsocs-2022.9.0/doc/usage/
--rw-rw-rw-   0 root         (0) root         (0)     2340 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/conversion.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.835885 xsocs-2022.9.0/doc/usage/img/
--rw-rw-rw-   0 root         (0) root         (0)   114617 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/com_results_view.png
--rw-rw-rw-   0 root         (0) root         (0)    83045 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/conversion_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)      622 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/draw_roi_button.png
--rw-rw-rw-   0 root         (0) root         (0)     1403 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/export_fit_button.png
--rw-rw-rw-   0 root         (0) root         (0)     1113 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/fit_results_button.png
--rw-rw-rw-   0 root         (0) root         (0)   156322 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/fit_results_view.png
--rw-rw-rw-   0 root         (0) root         (0)     1113 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/intensity_plot_button.png
--rw-rw-rw-   0 root         (0) root         (0)   136848 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/intensity_view.png
--rw-rw-rw-   0 root         (0) root         (0)     7280 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/main_view.png
--rw-rw-rw-   0 root         (0) root         (0)    41461 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/merge_window.png
--rw-rw-rw-   0 root         (0) root         (0)    37829 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/open_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)      926 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/open_icon.png
--rw-rw-rw-   0 root         (0) root         (0)    34780 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/project_tree.png
--rw-rw-rw-   0 root         (0) root         (0)    86754 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/qspace_stack_view.png
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/qspace_view_button.png
--rw-rw-rw-   0 root         (0) root         (0)   110038 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/qspace_window.png
--rw-rw-rw-   0 root         (0) root         (0)   145447 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/shift_editor.png
--rw-rw-rw-   0 root         (0) root         (0)     2876 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/img/to_qspace_button.png
--rw-rw-rw-   0 root         (0) root         (0)     2898 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/intensity_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     6397 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/project.rst
--rw-rw-rw-   0 root         (0) root         (0)     2535 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/project_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     3053 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/qspace_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     1763 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/results_view.rst
--rw-rw-rw-   0 root         (0) root         (0)      786 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/usage/starting.rst
--rw-rw-rw-   0 root         (0) root         (0)      388 2022-09-16 09:38:19.000000 xsocs-2022.9.0/doc/using.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-09-16 09:38:19.000000 xsocs-2022.9.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1558 2022-09-16 13:40:33.891885 xsocs-2022.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-09-16 09:38:19.000000 xsocs-2022.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.763885 xsocs-2022.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.839885 xsocs-2022.9.0/src/xsocs/
--rw-rw-rw-   0 root         (0) root         (0)      523 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.851885 xsocs-2022.9.0/src/xsocs/_app/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/_app/concat.py
--rw-rw-rw-   0 root         (0) root         (0)     1162 2022-09-16 13:30:47.000000 xsocs-2022.9.0/src/xsocs/_app/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2022-09-16 13:30:47.000000 xsocs-2022.9.0/src/xsocs/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.851885 xsocs-2022.9.0/src/xsocs/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2600 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/examples/id01_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1985 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/examples/id01_peak.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/examples/id01_qspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.855885 xsocs-2022.9.0/src/xsocs/gui/
--rw-rw-rw-   0 root         (0) root         (0)      335 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/XsocsGui.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.859886 xsocs-2022.9.0/src/xsocs/gui/model/
--rw-rw-rw-   0 root         (0) root         (0)     5309 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/Model.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/ModelDef.py
--rw-rw-rw-   0 root         (0) root         (0)    39327 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/Node.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/NodeEditor.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/Nodes.py
--rw-rw-rw-   0 root         (0) root         (0)    13616 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/model/TreeView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.859886 xsocs-2022.9.0/src/xsocs/gui/process/
--rw-rw-rw-   0 root         (0) root         (0)     8467 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/process/FitWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    43218 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/process/MergeWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    34945 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/process/QSpaceWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/process/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.863885 xsocs-2022.9.0/src/xsocs/gui/project/
--rw-rw-rw-   0 root         (0) root         (0)      964 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/AcqDataGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/FitGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     8312 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/Hdf5Nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/IntensityGroup.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/ProjectDef.py
--rw-rw-rw-   0 root         (0) root         (0)     9049 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/ProjectItem.py
--rw-rw-rw-   0 root         (0) root         (0)    22762 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/ProjectNodes.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/QSpaceGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/ScanPositionsItem.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/ShiftGroup.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/XsocsH5Factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2956 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/project/XsocsProject.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.863885 xsocs-2022.9.0/src/xsocs/gui/silx_imports/
--rw-rw-rw-   0 root         (0) root         (0)    25717 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/silx_imports/ImageRois.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/silx_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.867885 xsocs-2022.9.0/src/xsocs/gui/view/
--rw-rw-rw-   0 root         (0) root         (0)    11545 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/FitView.py
--rw-rw-rw-   0 root         (0) root         (0)    28432 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/QspaceView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.867885 xsocs-2022.9.0/src/xsocs/gui/view/fitview/
--rw-rw-rw-   0 root         (0) root         (0)     3085 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/fitview/DropPlotWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     7576 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/fitview/FitModel.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/fitview/Plotter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/view/fitview/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.867885 xsocs-2022.9.0/src/xsocs/gui/view/intensity/
--rw-rw-rw-   0 root         (0) root         (0)    25464 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/intensity/IntensityView.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/intensity/RectRoiWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/view/intensity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.871885 xsocs-2022.9.0/src/xsocs/gui/view/shift/
--rw-rw-rw-   0 root         (0) root         (0)    16552 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/shift/ShiftSubject.py
--rw-rw-rw-   0 root         (0) root         (0)    33144 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/view/shift/ShiftView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/view/shift/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.871885 xsocs-2022.9.0/src/xsocs/gui/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     6723 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/AcqParamsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/Buttons.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/Containers.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/FileChooser.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/Input.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/PlotGrabber.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/PointWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6984 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/ProjectChooser.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/RoiAxisWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/ScatterPlot.py
--rw-rw-rw-   0 root         (0) root         (0)     7985 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/Wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    38624 2022-09-16 13:30:47.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/XsocsPlot2D.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/gui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.875885 xsocs-2022.9.0/src/xsocs/io/
--rw-rw-rw-   0 root         (0) root         (0)    12367 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/FitH5.py
--rw-rw-rw-   0 root         (0) root         (0)    19829 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/QSpaceH5.py
--rw-rw-rw-   0 root         (0) root         (0)     5248 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/ShiftH5.py
--rw-rw-rw-   0 root         (0) root         (0)    14240 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/XsocsH5.py
--rw-rw-rw-   0 root         (0) root         (0)     8222 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/XsocsH5Base.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/io/_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.875885 xsocs-2022.9.0/src/xsocs/process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/process/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.875885 xsocs-2022.9.0/src/xsocs/process/fit/
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/fit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20367 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/fit/peak_fit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.875885 xsocs-2022.9.0/src/xsocs/process/merge/
--rw-rw-rw-   0 root         (0) root         (0)    26919 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/merge/KmapMerger.py
--rw-rw-rw-   0 root         (0) root         (0)    10973 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/merge/KmapSpecParser.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/merge/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.875885 xsocs-2022.9.0/src/xsocs/process/qspace/
--rw-rw-rw-   0 root         (0) root         (0)    58203 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/qspace/QSpaceConverter.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/qspace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/qspace/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.879886 xsocs-2022.9.0/src/xsocs/process/shift/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-16 13:40:13.000000 xsocs-2022.9.0/src/xsocs/process/shift/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12929 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/shift/shift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.879886 xsocs-2022.9.0/src/xsocs/process/test/
--rw-rw-rw-   0 root         (0) root         (0)      479 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5248 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/test/test_fitter.py
--rw-rw-rw-   0 root         (0) root         (0)     4847 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/test/test_merger.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/test/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/process/test/test_qspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.879886 xsocs-2022.9.0/src/xsocs/resources/
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.767885 xsocs-2022.9.0/src/xsocs/resources/gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.891885 xsocs-2022.9.0/src/xsocs/resources/gui/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/create_project.png
--rw-rw-rw-   0 root         (0) root         (0)     6666 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/create_project.svg
--rw-rw-rw-   0 root         (0) root         (0)    16556 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/gears.png
--rw-rw-rw-   0 root         (0) root         (0)     6931 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/gears.svg
--rw-rw-rw-   0 root         (0) root         (0)     4224 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/logo.png
--rw-rw-rw-   0 root         (0) root         (0)   182541 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1478 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/save_2dscatter.png
--rw-rw-rw-   0 root         (0) root         (0)     3737 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/save_2dscatter.svg
--rw-rw-rw-   0 root         (0) root         (0)     1558 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/spec.png
--rw-rw-rw-   0 root         (0) root         (0)     2260 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/spec.svg
--rw-rw-rw-   0 root         (0) root         (0)     4661 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/xsocs.png
--rw-rw-rw-   0 root         (0) root         (0)     3252 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/resources/gui/icons/xsocs.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.891885 xsocs-2022.9.0/src/xsocs/test/
--rw-rw-rw-   0 root         (0) root         (0)      684 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/test/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/test/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.891885 xsocs-2022.9.0/src/xsocs/util/
--rw-rw-rw-   0 root         (0) root         (0)     2141 2022-09-16 09:38:19.000000 xsocs-2022.9.0/src/xsocs/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 13:40:33.847885 xsocs-2022.9.0/src/xsocs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2059 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4983 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      193 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-09-16 13:40:33.000000 xsocs-2022.9.0/src/xsocs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.103132 xsocs-2022.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2022-09-19 11:51:48.000000 xsocs-2022.9.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-09-19 10:01:27.000000 xsocs-2022.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2022-09-19 10:01:27.000000 xsocs-2022.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2059 2022-09-19 13:04:07.103132 xsocs-2022.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2022-09-19 10:01:27.000000 xsocs-2022.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.003132 xsocs-2022.9.1/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7705 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/fileformat.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.003132 xsocs-2022.9.1/doc/img/
+-rw-rw-rw-   0 root         (0) root         (0)    99637 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/img/input_file.png
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      614 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/troubleshooting.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/tutorials.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.007132 xsocs-2022.9.1/doc/usage/
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/conversion.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.043132 xsocs-2022.9.1/doc/usage/img/
+-rw-rw-rw-   0 root         (0) root         (0)   114617 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/com_results_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    83045 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/conversion_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)      622 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/draw_roi_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/export_fit_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/fit_results_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   156322 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/fit_results_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/intensity_plot_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   136848 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/intensity_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     7280 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/main_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    41461 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/merge_window.png
+-rw-rw-rw-   0 root         (0) root         (0)    37829 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/open_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)      926 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/open_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    34780 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/project_tree.png
+-rw-rw-rw-   0 root         (0) root         (0)    86754 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/qspace_stack_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/qspace_view_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   110038 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/qspace_window.png
+-rw-rw-rw-   0 root         (0) root         (0)   145447 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/shift_editor.png
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/img/to_qspace_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/intensity_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2022-09-19 11:10:27.000000 xsocs-2022.9.1/doc/usage/project.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/project_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/qspace_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1763 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/results_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)      786 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/usage/starting.rst
+-rw-rw-rw-   0 root         (0) root         (0)      388 2022-09-19 10:01:27.000000 xsocs-2022.9.1/doc/using.rst
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-09-19 10:01:27.000000 xsocs-2022.9.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2022-09-19 13:04:07.103132 xsocs-2022.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       70 2022-09-19 10:01:27.000000 xsocs-2022.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:06.991132 xsocs-2022.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.043132 xsocs-2022.9.1/src/xsocs/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.051132 xsocs-2022.9.1/src/xsocs/_app/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/_app/concat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/_app/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2022-09-19 11:51:48.000000 xsocs-2022.9.1/src/xsocs/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.055132 xsocs-2022.9.1/src/xsocs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/examples/id01_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/examples/id01_peak.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/examples/id01_qspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.063132 xsocs-2022.9.1/src/xsocs/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/XsocsGui.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.063132 xsocs-2022.9.1/src/xsocs/gui/model/
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/ModelDef.py
+-rw-rw-rw-   0 root         (0) root         (0)    39327 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/Node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/NodeEditor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/Nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13616 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/model/TreeView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.067132 xsocs-2022.9.1/src/xsocs/gui/process/
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/process/FitWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    43218 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/process/MergeWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    34945 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/process/QSpaceWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/process/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.071132 xsocs-2022.9.1/src/xsocs/gui/project/
+-rw-rw-rw-   0 root         (0) root         (0)      964 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/AcqDataGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/FitGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8312 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/Hdf5Nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/IntensityGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/ProjectDef.py
+-rw-rw-rw-   0 root         (0) root         (0)     9049 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/ProjectItem.py
+-rw-rw-rw-   0 root         (0) root         (0)    22762 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/ProjectNodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/QSpaceGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/ScanPositionsItem.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/ShiftGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/XsocsH5Factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2956 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/project/XsocsProject.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.075132 xsocs-2022.9.1/src/xsocs/gui/silx_imports/
+-rw-rw-rw-   0 root         (0) root         (0)    25717 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/silx_imports/ImageRois.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/silx_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.075132 xsocs-2022.9.1/src/xsocs/gui/view/
+-rw-rw-rw-   0 root         (0) root         (0)    11545 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/FitView.py
+-rw-rw-rw-   0 root         (0) root         (0)    28432 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/QspaceView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.075132 xsocs-2022.9.1/src/xsocs/gui/view/fitview/
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/fitview/DropPlotWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     7576 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/fitview/FitModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/fitview/Plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/view/fitview/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.075132 xsocs-2022.9.1/src/xsocs/gui/view/intensity/
+-rw-rw-rw-   0 root         (0) root         (0)    25464 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/intensity/IntensityView.py
+-rw-rw-rw-   0 root         (0) root         (0)     6050 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/intensity/RectRoiWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/view/intensity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.079132 xsocs-2022.9.1/src/xsocs/gui/view/shift/
+-rw-rw-rw-   0 root         (0) root         (0)    16552 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/shift/ShiftSubject.py
+-rw-rw-rw-   0 root         (0) root         (0)    33144 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/view/shift/ShiftView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/view/shift/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.079132 xsocs-2022.9.1/src/xsocs/gui/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     6723 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/AcqParamsWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/Buttons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/Containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/FileChooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/Input.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/PlotGrabber.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/PointWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6984 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/ProjectChooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/RoiAxisWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/ScatterPlot.py
+-rw-rw-rw-   0 root         (0) root         (0)    10134 2022-09-19 11:44:59.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/Wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    38624 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/XsocsPlot2D.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/gui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.083132 xsocs-2022.9.1/src/xsocs/io/
+-rw-rw-rw-   0 root         (0) root         (0)    12367 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/FitH5.py
+-rw-rw-rw-   0 root         (0) root         (0)    19829 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/QSpaceH5.py
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/ShiftH5.py
+-rw-rw-rw-   0 root         (0) root         (0)    14240 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/XsocsH5.py
+-rw-rw-rw-   0 root         (0) root         (0)     8222 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/XsocsH5Base.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9142 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/io/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.083132 xsocs-2022.9.1/src/xsocs/process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/process/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.083132 xsocs-2022.9.1/src/xsocs/process/fit/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/fit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20367 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/fit/peak_fit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.083132 xsocs-2022.9.1/src/xsocs/process/merge/
+-rw-rw-rw-   0 root         (0) root         (0)    26919 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/merge/KmapMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)    10973 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/merge/KmapSpecParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/merge/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.087132 xsocs-2022.9.1/src/xsocs/process/qspace/
+-rw-rw-rw-   0 root         (0) root         (0)    58203 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/qspace/QSpaceConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/qspace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/qspace/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.087132 xsocs-2022.9.1/src/xsocs/process/shift/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-19 13:03:44.000000 xsocs-2022.9.1/src/xsocs/process/shift/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12929 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/shift/shift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.087132 xsocs-2022.9.1/src/xsocs/process/test/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/test/test_fitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4847 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/test/test_merger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/test/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/process/test/test_qspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.087132 xsocs-2022.9.1/src/xsocs/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:06.995132 xsocs-2022.9.1/src/xsocs/resources/gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.099132 xsocs-2022.9.1/src/xsocs/resources/gui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     7819 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/bliss.png
+-rw-rw-rw-   0 root         (0) root         (0)    14896 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/bliss.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/create_project.png
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/create_project.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16556 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/gears.png
+-rw-rw-rw-   0 root         (0) root         (0)     6931 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/gears.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   182541 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/save_2dscatter.png
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/save_2dscatter.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/spec.png
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/spec.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/xsocs.png
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/resources/gui/icons/xsocs.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.103132 xsocs-2022.9.1/src/xsocs/test/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/test/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/test/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.103132 xsocs-2022.9.1/src/xsocs/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2022-09-19 10:01:27.000000 xsocs-2022.9.1/src/xsocs/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 13:04:07.047132 xsocs-2022.9.1/src/xsocs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2059 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5085 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      193 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-09-19 13:04:06.000000 xsocs-2022.9.1/src/xsocs.egg-info/top_level.txt
```

### Comparing `xsocs-2022.9.0/CHANGELOG.rst` & `xsocs-2022.9.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+v2022.9.1: 2022/09/20
+---------------------
+
+- Added support of ID01 bliss data (MR: !151)
+
 v2022.9.0: 2022/09/16
 ----------------------
 
 Python >= 3.7 and silx >= 1.0.0 are required.
 X-Socs is now a pure Python package (i.e., it does not contain compiled code).
 
 * Bug fix:
```

### Comparing `xsocs-2022.9.0/LICENSE` & `xsocs-2022.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/PKG-INFO` & `xsocs-2022.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsocs
-Version: 2022.9.0
+Version: 2022.9.1
 Summary: Xray Strain Orientation Calculation Software
 Home-page: https://gitlab.esrf.fr/kmap/xsocs
 Author: ESRF
 Author-email: silx@esrf.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `xsocs-2022.9.0/README.rst` & `xsocs-2022.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/conf.py` & `xsocs-2022.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/fileformat.rst` & `xsocs-2022.9.1/doc/fileformat.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/img/input_file.png` & `xsocs-2022.9.1/doc/img/input_file.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/index.rst` & `xsocs-2022.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/install.rst` & `xsocs-2022.9.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/modules.rst` & `xsocs-2022.9.1/doc/modules.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/troubleshooting.rst` & `xsocs-2022.9.1/doc/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/tutorials.rst` & `xsocs-2022.9.1/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/conversion.rst` & `xsocs-2022.9.1/doc/usage/conversion.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/com_results_view.png` & `xsocs-2022.9.1/doc/usage/img/com_results_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/conversion_dialog.png` & `xsocs-2022.9.1/doc/usage/img/conversion_dialog.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/draw_roi_button.png` & `xsocs-2022.9.1/doc/usage/img/draw_roi_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/export_fit_button.png` & `xsocs-2022.9.1/doc/usage/img/export_fit_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/fit_results_button.png` & `xsocs-2022.9.1/doc/usage/img/fit_results_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/fit_results_view.png` & `xsocs-2022.9.1/doc/usage/img/fit_results_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/intensity_plot_button.png` & `xsocs-2022.9.1/doc/usage/img/intensity_plot_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/intensity_view.png` & `xsocs-2022.9.1/doc/usage/img/intensity_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/main_view.png` & `xsocs-2022.9.1/doc/usage/img/main_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/merge_window.png` & `xsocs-2022.9.1/doc/usage/img/merge_window.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/open_dialog.png` & `xsocs-2022.9.1/doc/usage/img/open_dialog.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/open_icon.png` & `xsocs-2022.9.1/doc/usage/img/open_icon.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/project_tree.png` & `xsocs-2022.9.1/doc/usage/img/project_tree.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/qspace_stack_view.png` & `xsocs-2022.9.1/doc/usage/img/qspace_stack_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/qspace_view_button.png` & `xsocs-2022.9.1/doc/usage/img/qspace_view_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/qspace_window.png` & `xsocs-2022.9.1/doc/usage/img/qspace_window.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/shift_editor.png` & `xsocs-2022.9.1/doc/usage/img/shift_editor.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/img/to_qspace_button.png` & `xsocs-2022.9.1/doc/usage/img/to_qspace_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/intensity_view.rst` & `xsocs-2022.9.1/doc/usage/intensity_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/project.rst` & `xsocs-2022.9.1/doc/usage/project.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,34 @@
 
 .. warning::
     There can be only one project per folder!
     A confirmation dialog will pop up if a project file is already present in the chosen directory.
 
 The next page gives you the choice between:
 
+#. |bliss_icon| **Load Bliss data (HDF5)** to import data in HDF5 format acquired with Bliss.
+
+   Select the HDF5 `master` file of the dataset (the file that contains links to all the scans).
+   Once the project is created, the `Project summary`_ page is displayed.
+
 #. **Load X-Socs data (HDF5)** to import K-map data already in HDF5 format.
 
    To load data that has already been merged, select the `master` file of the merged data (the file that contains links to all entries).
    Once the project is created, the `Project summary`_ page is displayed.
 
 #. **Import SPEC data** to import K-map data SPEC and EDF files from the ESRF ID01 beamline.
 
    X-SOCS will merge the SPEC file and the EDF images into HDF5 files.
 
    See `Merge ID01 SPEC and EDF to HDF5`_ below.
 
 
+.. |bliss_icon| image:: ../../src/xsocs/resources/gui/icons/bliss.png
+   :width: 32px
+
 Merge ID01 SPEC and EDF to HDF5
 --------------------------------
 
 When using X-SOCS to merge data the following window is displayed:
 
 .. _figure_merge_window:
 .. figure:: img/merge_window.png
```

### Comparing `xsocs-2022.9.0/doc/usage/project_view.rst` & `xsocs-2022.9.1/doc/usage/project_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/qspace_view.rst` & `xsocs-2022.9.1/doc/usage/qspace_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/results_view.rst` & `xsocs-2022.9.1/doc/usage/results_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/doc/usage/starting.rst` & `xsocs-2022.9.1/doc/usage/starting.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/setup.cfg` & `xsocs-2022.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/__init__.py` & `xsocs-2022.9.1/src/xsocs/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/__main__.py` & `xsocs-2022.9.1/src/xsocs/__main__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/_app/concat.py` & `xsocs-2022.9.1/src/xsocs/_app/concat.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/_app/gui.py` & `xsocs-2022.9.1/src/xsocs/_app/gui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/_config.py` & `xsocs-2022.9.1/src/xsocs/_config.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/_version.py` & `xsocs-2022.9.1/src/xsocs/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 RELEASE_LEVEL_VALUE = {"dev": 0, "alpha": 10, "beta": 11, "candidate": 12, "final": 15}
 
 PRERELEASE_NORMALIZED_NAME = {"dev": "a", "alpha": "a", "beta": "b", "candidate": "rc"}
 
 MAJOR = 2022
 MINOR = 9
-MICRO = 0
+MICRO = 1
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
 )
```

### Comparing `xsocs-2022.9.0/src/xsocs/examples/id01_merge.py` & `xsocs-2022.9.1/src/xsocs/examples/id01_merge.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/examples/id01_peak.py` & `xsocs-2022.9.1/src/xsocs/examples/id01_peak.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/examples/id01_qspace.py` & `xsocs-2022.9.1/src/xsocs/examples/id01_qspace.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/XsocsGui.py` & `xsocs-2022.9.1/src/xsocs/gui/XsocsGui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/__init__.py` & `xsocs-2022.9.1/src/xsocs/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/gui.py` & `xsocs-2022.9.1/src/xsocs/gui/gui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/model/Model.py` & `xsocs-2022.9.1/src/xsocs/gui/model/Model.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/model/Node.py` & `xsocs-2022.9.1/src/xsocs/gui/model/Node.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/model/NodeEditor.py` & `xsocs-2022.9.1/src/xsocs/gui/model/NodeEditor.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/model/Nodes.py` & `xsocs-2022.9.1/src/xsocs/gui/model/Nodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/model/TreeView.py` & `xsocs-2022.9.1/src/xsocs/gui/model/TreeView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/process/FitWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/process/FitWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/process/MergeWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/process/MergeWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/process/QSpaceWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/process/QSpaceWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/AcqDataGroup.py` & `xsocs-2022.9.1/src/xsocs/gui/project/AcqDataGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/FitGroup.py` & `xsocs-2022.9.1/src/xsocs/gui/project/FitGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/Hdf5Nodes.py` & `xsocs-2022.9.1/src/xsocs/gui/project/Hdf5Nodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/IntensityGroup.py` & `xsocs-2022.9.1/src/xsocs/gui/project/IntensityGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/ProjectDef.py` & `xsocs-2022.9.1/src/xsocs/gui/project/ProjectDef.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/ProjectItem.py` & `xsocs-2022.9.1/src/xsocs/gui/project/ProjectItem.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/ProjectNodes.py` & `xsocs-2022.9.1/src/xsocs/gui/project/ProjectNodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/QSpaceGroup.py` & `xsocs-2022.9.1/src/xsocs/gui/project/QSpaceGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/ScanPositionsItem.py` & `xsocs-2022.9.1/src/xsocs/gui/project/ScanPositionsItem.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/ShiftGroup.py` & `xsocs-2022.9.1/src/xsocs/gui/project/ShiftGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/XsocsH5Factory.py` & `xsocs-2022.9.1/src/xsocs/gui/project/XsocsH5Factory.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/project/XsocsProject.py` & `xsocs-2022.9.1/src/xsocs/gui/project/XsocsProject.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/silx_imports/ImageRois.py` & `xsocs-2022.9.1/src/xsocs/gui/silx_imports/ImageRois.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/FitView.py` & `xsocs-2022.9.1/src/xsocs/gui/view/FitView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/QspaceView.py` & `xsocs-2022.9.1/src/xsocs/gui/view/QspaceView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/fitview/DropPlotWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/view/fitview/DropPlotWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/fitview/FitModel.py` & `xsocs-2022.9.1/src/xsocs/gui/view/fitview/FitModel.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/fitview/Plotter.py` & `xsocs-2022.9.1/src/xsocs/gui/view/fitview/Plotter.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/intensity/IntensityView.py` & `xsocs-2022.9.1/src/xsocs/gui/view/intensity/IntensityView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/intensity/RectRoiWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/view/intensity/RectRoiWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/shift/ShiftSubject.py` & `xsocs-2022.9.1/src/xsocs/gui/view/shift/ShiftSubject.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/view/shift/ShiftView.py` & `xsocs-2022.9.1/src/xsocs/gui/view/shift/ShiftView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/AcqParamsWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/AcqParamsWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/Buttons.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/Buttons.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/Containers.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/Containers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/FileChooser.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/FileChooser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/Input.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/Input.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/PlotGrabber.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/PlotGrabber.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/PointWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/PointWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/ProjectChooser.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/ProjectChooser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/RoiAxisWidget.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/RoiAxisWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/ScatterPlot.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/ScatterPlot.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/Wizard.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/Wizard.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """X-Socs new project wizard"""
 
+import logging
 import os
-from functools import partial
+from pathlib import Path
+import traceback
 
 from silx.gui import qt as Qt
 from silx.gui import icons
 
 from .FileChooser import FileChooser
 from ..widgets.Containers import GroupBox
 from ..process.MergeWidget import MergeWidget
 from ..project.XsocsProject import XsocsProject
 from .ProjectChooser import ProjectSummaryWidget
+from ...io.bliss import make_xsocs_links
+
+
+_logger = logging.getLogger(__name__)
 
 
 class XsocsWizard(Qt.QWizard):
     """New project wizard class"""
 
-    (CreateId, SelectDataId, LoadXsocsId, ReviewId) = range(4)
+    (CreateId, SelectDataId, LoadXsocsId, LoadBlissId, ReviewId) = range(5)
 
     def __init__(self, parent=None):
         super(XsocsWizard, self).__init__(parent)
 
         self.__projectFile = None
 
         self.setPage(XsocsWizard.CreateId, NewProjectPage())
         self.setPage(XsocsWizard.SelectDataId, SelectDataPage())
         self.setPage(XsocsWizard.LoadXsocsId, LoadXsocsDataPage())
+        self.setPage(XsocsWizard.LoadBlissId, LoadBlissDataPage())
         self.setPage(XsocsWizard.ReviewId, ReviewProjectPage())
 
     projectFile = property(lambda self: self.__projectFile)
 
     @projectFile.setter
     def projectFile(self, projectFile):
         self.__projectFile = projectFile
@@ -84,85 +91,150 @@
         except Exception as ex:
             Qt.QMessageBox.critical(self, "Failed to set data file.", str(ex))
             return False
         self.setCommitPage(True)
         return True
 
 
+class LoadBlissDataPage(_BaseWizardPage):
+    """Create project from Bliss data HDF5 file page"""
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        self.setSubTitle("New project: Load Bliss data (HDF5)")
+
+        layout = Qt.QVBoxLayout(self)
+
+        group = GroupBox("Please select the Bliss data file to load")
+        layout.addWidget(group)
+        grpLayout = Qt.QHBoxLayout(group)
+        filePicker = FileChooser(fileMode=Qt.QFileDialog.ExistingFile)
+        grpLayout.addWidget(filePicker)
+
+        self.registerField("BlissDataFile*", filePicker.lineEdit)
+
+    def nextId(self):
+        return XsocsWizard.ReviewId
+
+    def validatePage(self):
+        projectFile = self.wizard().projectFile
+        blissFile = self.wizard().field("BlissDataFile")
+
+        try:
+            projectH5 = XsocsProject(projectFile, mode="a", gui=self)
+        except Exception as ex:
+            _logger.error(traceback.format_exc())
+            Qt.QMessageBox.critical(
+                self, "Error", f"Failed to open project file:\n{projectFile}\n\n{ex}"
+            )
+            return False
+
+        try:
+            xsocsFile = make_xsocs_links(
+                path_dset=blissFile,
+                path_out=str((Path(projectFile).parent / "xsocs_bliss_data").resolve()),
+                scan_nums=None,
+            )
+        except Exception as ex:
+            _logger.error(traceback.format_exc())
+            Qt.QMessageBox.critical(
+                self,
+                "Error",
+                f"Failed to create xsocs data file from:\n{blissFile}\n\n{ex}",
+            )
+            return False
+
+        try:
+            projectH5.xsocsFile = xsocsFile
+        except Exception as ex:
+            _logger.error(traceback.format_exc())
+            Qt.QMessageBox.critical(
+                self, "Error", f"Failed to set data file:\n{xsocsFile}\n\n{ex}"
+            )
+            return False
+        self.setCommitPage(True)
+        return True
+
+
 class SelectDataPage(_BaseWizardPage):
     """Choose between create project from HDF5 or from SPEC+EDF"""
 
     def __init__(self, parent=None):
         super(SelectDataPage, self).__init__(parent)
 
         self.setSubTitle("New project: Select data to load/import.")
         self.setTitle("Select input data.")
 
         self.__nextId = -1
 
-        layout = Qt.QGridLayout(self)
+        layout = Qt.QFormLayout(self)
+
+        icon = icons.getQIcon("xsocs:gui/icons/bliss")
+        blissBn = Qt.QToolButton()
+        blissBn.setIcon(icon)
+        layout.addRow(blissBn, Qt.QLabel("Load Bliss data (HDF5)"))
+
         icon = icons.getQIcon("xsocs:gui/icons/logo")
         xsocsBn = Qt.QToolButton()
         xsocsBn.setIcon(icon)
-        layout.addWidget(xsocsBn, 1, 1)
-        layout.addWidget(Qt.QLabel("Load X-Socs Data (HDF5)."), 1, 2)
+        layout.addRow(xsocsBn, Qt.QLabel("Load X-Socs data (HDF5)"))
 
         icon = icons.getQIcon("xsocs:gui/icons/spec")
         specBn = Qt.QToolButton()
         specBn.setIcon(icon)
-        layout.addWidget(specBn, 2, 1)
-        layout.addWidget(Qt.QLabel("Import SPEC data."), 2, 2)
+        layout.addRow(specBn, Qt.QLabel("Import SPEC data"))
 
-        layout.setRowStretch(0, 1)
-        layout.setRowStretch(3, 1)
-        layout.setColumnStretch(3, 1)
-
-        xsocsBn.clicked.connect(partial(self.__buttonClicked, source="XSOCS"))
-        specBn.clicked.connect(partial(self.__buttonClicked, source="SPEC"))
+        blissBn.clicked.connect(self.__loadBlissClicked)
+        xsocsBn.clicked.connect(self.__loadXSocsClicked)
+        specBn.clicked.connect(self.__importSpecClicked)
 
     def nextId(self):
         return self.__nextId
 
     def isComplete(self):
         return False
 
     def initializePage(self):
         self.setCommitPage(False)
 
-    def __buttonClicked(self, source=None):
+    def __loadBlissClicked(self):
+        self.__nextId = XsocsWizard.LoadBlissId
+        self.wizard().next()
+
+    def __loadXSocsClicked(self):
+        self.__nextId = XsocsWizard.LoadXsocsId
+        self.wizard().next()
+
+    def __importSpecClicked(self):
         self.__nextId = -1
-        if source == "XSOCS":
-            self.__nextId = XsocsWizard.LoadXsocsId
-        if source == "SPEC":
-            outputDir = os.path.dirname(self.wizard().projectFile)
-            mergeWid = MergeWidget(parent=self, output_dir=outputDir)
-            if mergeWid.exec_() == Qt.QDialog.Accepted:
-                xsocsH5 = mergeWid.xsocsH5
-                mergeWid.deleteLater()
-
-                if xsocsH5 is not None:
-                    projectFile = self.wizard().projectFile
-                    try:
-                        projectH5 = XsocsProject(projectFile, mode="a")
-                    except Exception as ex:
-                        Qt.QMessageBox.critical(
-                            self, "Failed to open project file.", str(ex)
-                        )
-                        return
-
-                    try:
-                        projectH5.xsocsFile = xsocsH5
-                    except Exception as ex:
-                        Qt.QMessageBox.critical(
-                            self, "Failed to set data file.", str(ex)
-                        )
-                        return
+        outputDir = os.path.dirname(self.wizard().projectFile)
+        mergeWid = MergeWidget(parent=self, output_dir=outputDir)
+        if mergeWid.exec_() == Qt.QDialog.Accepted:
+            xsocsH5 = mergeWid.xsocsH5
+            mergeWid.deleteLater()
+
+            if xsocsH5 is not None:
+                projectFile = self.wizard().projectFile
+                try:
+                    projectH5 = XsocsProject(projectFile, mode="a")
+                except Exception as ex:
+                    Qt.QMessageBox.critical(
+                        self, "Failed to open project file.", str(ex)
+                    )
+                    return
+
+                try:
+                    projectH5.xsocsFile = xsocsH5
+                except Exception as ex:
+                    Qt.QMessageBox.critical(self, "Failed to set data file.", str(ex))
+                    return
 
-                    self.__nextId = XsocsWizard.ReviewId
-                    self.setCommitPage(True)
+                self.__nextId = XsocsWizard.ReviewId
+                self.setCommitPage(True)
 
         if self.__nextId != -1:
             self.wizard().next()
 
 
 class ReviewProjectPage(_BaseWizardPage):
     """Last wizard page with project summary"""
```

### Comparing `xsocs-2022.9.0/src/xsocs/gui/widgets/XsocsPlot2D.py` & `xsocs-2022.9.1/src/xsocs/gui/widgets/XsocsPlot2D.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/FitH5.py` & `xsocs-2022.9.1/src/xsocs/io/FitH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/QSpaceH5.py` & `xsocs-2022.9.1/src/xsocs/io/QSpaceH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/ShiftH5.py` & `xsocs-2022.9.1/src/xsocs/io/ShiftH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/XsocsH5.py` & `xsocs-2022.9.1/src/xsocs/io/XsocsH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/XsocsH5Base.py` & `xsocs-2022.9.1/src/xsocs/io/XsocsH5Base.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/io/_utils.py` & `xsocs-2022.9.1/src/xsocs/io/_utils.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/fit/peak_fit.py` & `xsocs-2022.9.1/src/xsocs/process/fit/peak_fit.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/merge/KmapMerger.py` & `xsocs-2022.9.1/src/xsocs/process/merge/KmapMerger.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/merge/KmapSpecParser.py` & `xsocs-2022.9.1/src/xsocs/process/merge/KmapSpecParser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/merge/helpers.py` & `xsocs-2022.9.1/src/xsocs/process/merge/helpers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/qspace/QSpaceConverter.py` & `xsocs-2022.9.1/src/xsocs/process/qspace/QSpaceConverter.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/qspace/helpers.py` & `xsocs-2022.9.1/src/xsocs/process/qspace/helpers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/shift/shift.py` & `xsocs-2022.9.1/src/xsocs/process/shift/shift.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/test/test_fitter.py` & `xsocs-2022.9.1/src/xsocs/process/test/test_fitter.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/test/test_merger.py` & `xsocs-2022.9.1/src/xsocs/process/test/test_merger.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/test/test_parser.py` & `xsocs-2022.9.1/src/xsocs/process/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/process/test/test_qspace.py` & `xsocs-2022.9.1/src/xsocs/process/test/test_qspace.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/create_project.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/create_project.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/create_project.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/create_project.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/gears.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/gears.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/gears.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/gears.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/logo.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/logo.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/logo.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/save_2dscatter.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/save_2dscatter.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/save_2dscatter.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/save_2dscatter.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/spec.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/spec.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/spec.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/spec.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/xsocs.png` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/xsocs.png`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/resources/gui/icons/xsocs.svg` & `xsocs-2022.9.1/src/xsocs/resources/gui/icons/xsocs.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/test/__init__.py` & `xsocs-2022.9.1/src/xsocs/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs/util/__init__.py` & `xsocs-2022.9.1/src/xsocs/util/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2022.9.0/src/xsocs.egg-info/PKG-INFO` & `xsocs-2022.9.1/src/xsocs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsocs
-Version: 2022.9.0
+Version: 2022.9.1
 Summary: Xray Strain Orientation Calculation Software
 Home-page: https://gitlab.esrf.fr/kmap/xsocs
 Author: ESRF
 Author-email: silx@esrf.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `xsocs-2022.9.0/src/xsocs.egg-info/SOURCES.txt` & `xsocs-2022.9.1/src/xsocs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 src/xsocs/io/FitH5.py
 src/xsocs/io/QSpaceH5.py
 src/xsocs/io/ShiftH5.py
 src/xsocs/io/XsocsH5.py
 src/xsocs/io/XsocsH5Base.py
 src/xsocs/io/__init__.py
 src/xsocs/io/_utils.py
+src/xsocs/io/bliss.py
 src/xsocs/process/__init__.py
 src/xsocs/process/fit/__init__.py
 src/xsocs/process/fit/peak_fit.py
 src/xsocs/process/merge/KmapMerger.py
 src/xsocs/process/merge/KmapSpecParser.py
 src/xsocs/process/merge/__init__.py
 src/xsocs/process/merge/helpers.py
@@ -134,14 +135,16 @@
 src/xsocs/process/shift/shift.py
 src/xsocs/process/test/__init__.py
 src/xsocs/process/test/test_fitter.py
 src/xsocs/process/test/test_merger.py
 src/xsocs/process/test/test_parser.py
 src/xsocs/process/test/test_qspace.py
 src/xsocs/resources/__init__.py
+src/xsocs/resources/gui/icons/bliss.png
+src/xsocs/resources/gui/icons/bliss.svg
 src/xsocs/resources/gui/icons/create_project.png
 src/xsocs/resources/gui/icons/create_project.svg
 src/xsocs/resources/gui/icons/gears.png
 src/xsocs/resources/gui/icons/gears.svg
 src/xsocs/resources/gui/icons/logo.png
 src/xsocs/resources/gui/icons/logo.svg
 src/xsocs/resources/gui/icons/save_2dscatter.png
```

