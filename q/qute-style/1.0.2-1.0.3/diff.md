# Comparing `tmp/qute_style-1.0.2.tar.gz` & `tmp/qute_style-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qute_style-1.0.2.tar", max compression
+gzip compressed data, was "qute_style-1.0.3.tar", max compression
```

## Comparing `qute_style-1.0.2.tar` & `qute_style-1.0.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0     1087 2023-03-22 13:41:23.178106 qute_style-1.0.2/LICENSE
--rw-r--r--   0        0        0     5391 2023-03-22 13:41:23.178106 qute_style-1.0.2/README.md
--rw-r--r--   0        0        0     1064 2023-03-22 13:41:23.178106 qute_style-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.178106 qute_style-1.0.2/qute_style/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.178106 qute_style-1.0.2/qute_style/dev/__init__.py
--rw-r--r--   0        0        0     6132 2023-03-22 13:41:23.178106 qute_style-1.0.2/qute_style/dev/dev_functions.py
--rw-r--r--   0        0        0     8916 2023-03-22 13:41:23.178106 qute_style-1.0.2/qute_style/dev/mocks.py
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/gen/__init__.py
--rw-r--r--   0        0        0    29363 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/gen/ui_test_window.py
--rw-r--r--   0        0        0     5388 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/gen/ui_whats_new_window.py
--rw-r--r--   0        0        0     1813 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/helper.py
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/py.typed
--rw-r--r--   0        0        0     8198 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/qs_application.py
--rw-r--r--   0        0        0    28986 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/qs_main_window.py
--rw-r--r--   0        0        0     6436 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/qs_message_box.py
--rw-r--r--   0        0        0    26591 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/qute_style.py
--rw-r--r--   0        0        0      104 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/png_icons/transparent_icon.png
--rw-r--r--   0        0        0      466 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/accept.svg
--rw-r--r--   0        0        0     3012 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/accept_circle.svg
--rw-r--r--   0        0        0     2379 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/active_menu.svg
--rw-r--r--   0        0        0     2139 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/add.svg
--rw-r--r--   0        0        0     2160 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/add_circle.svg
--rw-r--r--   0        0        0     1939 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/admin.svg
--rw-r--r--   0        0        0     2721 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/admin_panel.svg
--rw-r--r--   0        0        0     2002 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/arrow_back.svg
--rw-r--r--   0        0        0      394 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/arrow_down.svg
--rw-r--r--   0        0        0      398 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/arrow_right.svg
--rw-r--r--   0        0        0     2004 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/block.svg
--rw-r--r--   0        0        0     3858 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/bug.svg
--rw-r--r--   0        0        0     2145 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/check_circle.svg
--rw-r--r--   0        0        0      208 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/checked.svg
--rw-r--r--   0        0        0      324 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/chevron_left.svg
--rw-r--r--   0        0        0      441 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/clipboard.svg
--rw-r--r--   0        0        0     2271 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/close.svg
--rw-r--r--   0        0        0     2289 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/close_circle.svg
--rw-r--r--   0        0        0      363 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/cloud_upload.svg
--rw-r--r--   0        0        0     2068 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/copy.svg
--rw-r--r--   0        0        0     2255 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/cps_trends.svg
--rw-r--r--   0        0        0     2019 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/delete.svg
--rw-r--r--   0        0        0      699 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/delete_forever.svg
--rw-r--r--   0        0        0     1928 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/delete_import.svg
--rw-r--r--   0        0        0     1881 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/document.svg
--rw-r--r--   0        0        0      785 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/document_scanner.svg
--rw-r--r--   0        0        0     1989 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/error.svg
--rw-r--r--   0        0        0     1575 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/expand_less.svg
--rw-r--r--   0        0        0     2062 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/expand_more.svg
--rw-r--r--   0        0        0     1961 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/file_distributor.svg
--rw-r--r--   0        0        0      482 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/filter.svg
--rw-r--r--   0        0        0     2023 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/folder_open.svg
--rw-r--r--   0        0        0     2880 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/fullscreen.svg
--rw-r--r--   0        0        0     2877 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/fullscreen_exit.svg
--rw-r--r--   0        0        0     2236 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/heart_broken.svg
--rw-r--r--   0        0        0     2642 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/help.svg
--rw-r--r--   0        0        0     2206 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/home.svg
--rw-r--r--   0        0        0     4370 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/ian_manager.svg
--rw-r--r--   0        0        0     4191 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/icon_PSE.svg
--rw-r--r--   0        0        0     2597 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/import.svg
--rw-r--r--   0        0        0     1939 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/info.svg
--rw-r--r--   0        0        0      491 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/inventory.svg
--rw-r--r--   0        0        0     2018 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/lidl_budget.svg
--rw-r--r--   0        0        0     2485 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/menu.svg
--rw-r--r--   0        0        0     1747 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/minimize.svg
--rw-r--r--   0        0        0     2498 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/nav_updater.svg
--rw-r--r--   0        0        0     2505 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/new_releases.svg
--rw-r--r--   0        0        0     2932 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/news.svg
--rw-r--r--   0        0        0     3184 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/no_icon.svg
--rw-r--r--   0        0        0     2214 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/package_commander.svg
--rw-r--r--   0        0        0     2475 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/palette.svg
--rw-r--r--   0        0        0     2709 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/pap.svg
--rw-r--r--   0        0        0      175 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/partial_checked.svg
--rw-r--r--   0        0        0     2236 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/protocol_creator.svg
--rw-r--r--   0        0        0      549 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/pzf_widget.svg
--rw-r--r--   0        0        0     3073 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/qt.svg
--rw-r--r--   0        0        0     2684 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/read_more.svg
--rw-r--r--   0        0        0     2468 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/refresh.svg
--rw-r--r--   0        0        0     1910 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/report_merger.svg
--rw-r--r--   0        0        0     2113 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/sap_excel.svg
--rw-r--r--   0        0        0     2244 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/save.svg
--rw-r--r--   0        0        0     2390 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/save_alt.svg
--rw-r--r--   0        0        0     2398 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/search.svg
--rw-r--r--   0        0        0     2103 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/send.svg
--rw-r--r--   0        0        0     3472 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/settings.svg
--rw-r--r--   0        0        0      184 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/status.svg
--rw-r--r--   0        0        0     2448 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/swap.svg
--rw-r--r--   0        0        0     2778 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/sync.svg
--rw-r--r--   0        0        0     2336 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/template_selector.svg
--rw-r--r--   0        0        0     2531 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/testbase_manager.svg
--rw-r--r--   0        0        0     1965 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/todo_circle.svg
--rw-r--r--   0        0        0     2257 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_icons/undo.svg
--rw-r--r--   0        0        0    32469 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_images/banner_qute_style.svg
--rw-r--r--   0        0        0     7237 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_images/logo_chemistry.svg
--rw-r--r--   0        0        0     8429 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_images/logo_labmonitor.svg
--rw-r--r--   0        0        0    39983 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_images/logo_qute_style.svg
--rw-r--r--   0        0        0     8278 2023-03-22 13:41:23.182106 qute_style-1.0.2/qute_style/resources/svg_images/logo_toolbox.svg
--rw-r--r--   0        0        0   323159 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/resources_rc.py
--rw-r--r--   0        0        0     1657 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/startup_threads.py
--rw-r--r--   0        0        0    23017 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/style.py
--rw-r--r--   0        0        0    20184 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/ui/test_window.ui
--rw-r--r--   0        0        0     3001 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/ui/whats_new_window.ui
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/__init__.py
--rw-r--r--   0        0        0     1165 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/background_frame.py
--rw-r--r--   0        0        0     3720 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/base_widgets.py
--rw-r--r--   0        0        0     5533 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/color_manager.py
--rw-r--r--   0        0        0     1089 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/credit_bar.py
--rw-r--r--   0        0        0     4440 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/custom_icon_engine.py
--rw-r--r--   0        0        0      483 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/div.py
--rw-r--r--   0        0        0     1745 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/drop_label.py
--rw-r--r--   0        0        0     7164 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/grips.py
--rw-r--r--   0        0        0    16374 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/home_page.py
--rw-r--r--   0        0        0     2049 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/icon.py
--rw-r--r--   0        0        0     7697 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/icon_button.py
--rw-r--r--   0        0        0     3474 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/icon_tooltip_button.py
--rw-r--r--   0        0        0     6849 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/left_column.py
--rw-r--r--   0        0        0      808 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/left_column_close_button.py
--rw-r--r--   0        0        0     8775 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/left_menu.py
--rw-r--r--   0        0        0     7075 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/left_menu_button.py
--rw-r--r--   0        0        0    11127 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/spinner.py
--rw-r--r--   0        0        0    10811 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/styled_combobox.py
--rw-r--r--   0        0        0     1878 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/text_truncator.py
--rw-r--r--   0        0        0     6869 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/title_bar.py
--rw-r--r--   0        0        0     1733 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/title_button.py
--rw-r--r--   0        0        0     4334 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/toggle.py
--rw-r--r--   0        0        0     1046 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style/widgets/tooltip.py
--rw-r--r--   0        0        0        0 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style_examples/__init__.py
--rw-r--r--   0        0        0      136 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style_examples/__main__.py
--rw-r--r--   0        0        0    21042 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style_examples/example_images/color_manager.PNG
--rw-r--r--   0        0        0    79278 2023-03-22 13:41:23.186107 qute_style-1.0.2/qute_style_examples/example_images/custom_style.PNG
--rw-r--r--   0        0        0    62693 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/darcula.PNG
--rw-r--r--   0        0        0     3902 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/drop_label.PNG
--rw-r--r--   0        0        0    50435 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/highbridge_grey.PNG
--rw-r--r--   0        0        0     4594 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/information_messagebox.PNG
--rw-r--r--   0        0        0    30905 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/princesspink.PNG
--rw-r--r--   0        0        0    30041 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/rubyred.PNG
--rw-r--r--   0        0        0    30867 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/snowwhite.PNG
--rw-r--r--   0        0        0    56113 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/example_images/widgets_display.PNG
--rw-r--r--   0        0        0     2818 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/main.py
--rw-r--r--   0        0        0      646 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/sample_classes.py
--rw-r--r--   0        0        0     3414 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/sample_main_window.py
--rw-r--r--   0        0        0     9665 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/sample_widgets.py
--rw-r--r--   0        0        0      110 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.01/1.json
--rw-r--r--   0        0        0      211 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.01/2.json
--rw-r--r--   0        0        0    45119 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.01/bug.png
--rw-r--r--   0        0        0      167 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.10/1.json
--rw-r--r--   0        0        0      209 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.10/2.json
--rw-r--r--   0        0        0    45119 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.10/bug.png
--rw-r--r--   0        0        0      114 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.100/1.json
--rw-r--r--   0        0        0       97 2023-03-22 13:41:23.190106 qute_style-1.0.2/qute_style_examples/test_changelog/1.100/2.json
--rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 qute_style-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-04-27 09:33:45.449041 qute_style-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5391 2023-04-27 09:33:45.449041 qute_style-1.0.3/README.md
+-rw-r--r--   0        0        0     1042 2023-04-27 09:33:45.449041 qute_style-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/dev_functions.py
+-rw-r--r--   0        0        0     8916 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/mocks.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/gen/__init__.py
+-rw-r--r--   0        0        0    29831 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/gen/ui_test_window.py
+-rw-r--r--   0        0        0     5330 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/gen/ui_whats_new_window.py
+-rw-r--r--   0        0        0     1813 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/helper.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/py.typed
+-rw-r--r--   0        0        0     8198 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_application.py
+-rw-r--r--   0        0        0    29069 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_main_window.py
+-rw-r--r--   0        0        0     6436 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_message_box.py
+-rw-r--r--   0        0        0    26591 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qute_style.py
+-rw-r--r--   0        0        0      104 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/png_icons/transparent_icon.png
+-rw-r--r--   0        0        0      466 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/accept.svg
+-rw-r--r--   0        0        0     3012 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/accept_circle.svg
+-rw-r--r--   0        0        0     2379 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/active_menu.svg
+-rw-r--r--   0        0        0     2139 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/add.svg
+-rw-r--r--   0        0        0     2160 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/add_circle.svg
+-rw-r--r--   0        0        0     1939 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/admin.svg
+-rw-r--r--   0        0        0     2721 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/admin_panel.svg
+-rw-r--r--   0        0        0     2002 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_back.svg
+-rw-r--r--   0        0        0      394 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_down.svg
+-rw-r--r--   0        0        0      398 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_right.svg
+-rw-r--r--   0        0        0     2004 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/block.svg
+-rw-r--r--   0        0        0     3858 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/bug.svg
+-rw-r--r--   0        0        0     2145 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/check_circle.svg
+-rw-r--r--   0        0        0      208 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/checked.svg
+-rw-r--r--   0        0        0      324 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/chevron_left.svg
+-rw-r--r--   0        0        0      441 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/clipboard.svg
+-rw-r--r--   0        0        0     2271 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/close.svg
+-rw-r--r--   0        0        0     2289 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/close_circle.svg
+-rw-r--r--   0        0        0      363 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/cloud_upload.svg
+-rw-r--r--   0        0        0     2068 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/copy.svg
+-rw-r--r--   0        0        0     2255 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/cps_trends.svg
+-rw-r--r--   0        0        0     2019 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete.svg
+-rw-r--r--   0        0        0      699 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete_forever.svg
+-rw-r--r--   0        0        0     1928 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete_import.svg
+-rw-r--r--   0        0        0     1881 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/document.svg
+-rw-r--r--   0        0        0      785 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/document_scanner.svg
+-rw-r--r--   0        0        0     1989 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/error.svg
+-rw-r--r--   0        0        0     1575 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/expand_less.svg
+-rw-r--r--   0        0        0     2062 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/expand_more.svg
+-rw-r--r--   0        0        0     1961 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/file_distributor.svg
+-rw-r--r--   0        0        0      482 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/filter.svg
+-rw-r--r--   0        0        0     2023 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/folder_open.svg
+-rw-r--r--   0        0        0     2880 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen.svg
+-rw-r--r--   0        0        0     2877 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen_exit.svg
+-rw-r--r--   0        0        0     2236 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/heart_broken.svg
+-rw-r--r--   0        0        0     2642 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/help.svg
+-rw-r--r--   0        0        0     2206 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/home.svg
+-rw-r--r--   0        0        0     4370 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/ian_manager.svg
+-rw-r--r--   0        0        0     4191 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/icon_PSE.svg
+-rw-r--r--   0        0        0     2597 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/import.svg
+-rw-r--r--   0        0        0     1939 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/info.svg
+-rw-r--r--   0        0        0      491 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/inventory.svg
+-rw-r--r--   0        0        0     2018 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/lidl_budget.svg
+-rw-r--r--   0        0        0     2485 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/menu.svg
+-rw-r--r--   0        0        0     1747 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/minimize.svg
+-rw-r--r--   0        0        0     2498 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/nav_updater.svg
+-rw-r--r--   0        0        0     2505 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/new_releases.svg
+-rw-r--r--   0        0        0     2932 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/news.svg
+-rw-r--r--   0        0        0     3184 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/no_icon.svg
+-rw-r--r--   0        0        0     2214 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/package_commander.svg
+-rw-r--r--   0        0        0     2475 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/palette.svg
+-rw-r--r--   0        0        0     2709 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/pap.svg
+-rw-r--r--   0        0        0      175 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/partial_checked.svg
+-rw-r--r--   0        0        0     2236 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/protocol_creator.svg
+-rw-r--r--   0        0        0      549 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/pzf_widget.svg
+-rw-r--r--   0        0        0     3073 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/qt.svg
+-rw-r--r--   0        0        0     2684 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/read_more.svg
+-rw-r--r--   0        0        0     2468 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/refresh.svg
+-rw-r--r--   0        0        0     1910 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/report_merger.svg
+-rw-r--r--   0        0        0     2113 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/sap_excel.svg
+-rw-r--r--   0        0        0     2244 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/save.svg
+-rw-r--r--   0        0        0     2390 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/save_alt.svg
+-rw-r--r--   0        0        0     2398 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/search.svg
+-rw-r--r--   0        0        0     2103 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/send.svg
+-rw-r--r--   0        0        0     3472 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/settings.svg
+-rw-r--r--   0        0        0      184 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/status.svg
+-rw-r--r--   0        0        0     2448 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/swap.svg
+-rw-r--r--   0        0        0     2778 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/sync.svg
+-rw-r--r--   0        0        0     2336 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/template_selector.svg
+-rw-r--r--   0        0        0     2531 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/testbase_manager.svg
+-rw-r--r--   0        0        0     1965 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/todo_circle.svg
+-rw-r--r--   0        0        0     2257 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/undo.svg
+-rw-r--r--   0        0        0    32469 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/banner_qute_style.svg
+-rw-r--r--   0        0        0     7237 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_chemistry.svg
+-rw-r--r--   0        0        0     8429 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_labmonitor.svg
+-rw-r--r--   0        0        0    39983 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_qute_style.svg
+-rw-r--r--   0        0        0     8278 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_toolbox.svg
+-rw-r--r--   0        0        0   323159 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/resources_rc.py
+-rw-r--r--   0        0        0     1657 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/startup_threads.py
+-rw-r--r--   0        0        0    23017 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/style.py
+-rw-r--r--   0        0        0    20664 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/ui/test_window.ui
+-rw-r--r--   0        0        0     3001 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/ui/whats_new_window.ui
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/__init__.py
+-rw-r--r--   0        0        0     1165 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/background_frame.py
+-rw-r--r--   0        0        0     2967 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/base_widgets.py
+-rw-r--r--   0        0        0     5533 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/color_manager.py
+-rw-r--r--   0        0        0     1089 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/credit_bar.py
+-rw-r--r--   0        0        0     4440 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/custom_icon_engine.py
+-rw-r--r--   0        0        0      483 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/div.py
+-rw-r--r--   0        0        0     1745 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/drop_label.py
+-rw-r--r--   0        0        0     7164 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/grips.py
+-rw-r--r--   0        0        0    16374 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/home_page.py
+-rw-r--r--   0        0        0     2049 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon.py
+-rw-r--r--   0        0        0     7697 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon_button.py
+-rw-r--r--   0        0        0     3474 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon_tooltip_button.py
+-rw-r--r--   0        0        0     6849 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_column.py
+-rw-r--r--   0        0        0      808 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_column_close_button.py
+-rw-r--r--   0        0        0     8775 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_menu.py
+-rw-r--r--   0        0        0     7075 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_menu_button.py
+-rw-r--r--   0        0        0    11127 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/spinner.py
+-rw-r--r--   0        0        0    14486 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/styled_combobox.py
+-rw-r--r--   0        0        0     1878 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/text_truncator.py
+-rw-r--r--   0        0        0     6869 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/title_bar.py
+-rw-r--r--   0        0        0     1733 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/title_button.py
+-rw-r--r--   0        0        0     4334 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/toggle.py
+-rw-r--r--   0        0        0     1046 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/tooltip.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/__main__.py
+-rw-r--r--   0        0        0    21042 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/example_images/color_manager.PNG
+-rw-r--r--   0        0        0    79278 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/example_images/custom_style.PNG
+-rw-r--r--   0        0        0    62693 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/darcula.PNG
+-rw-r--r--   0        0        0     3902 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/drop_label.PNG
+-rw-r--r--   0        0        0    50435 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/highbridge_grey.PNG
+-rw-r--r--   0        0        0     4594 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/information_messagebox.PNG
+-rw-r--r--   0        0        0    30905 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/princesspink.PNG
+-rw-r--r--   0        0        0    30041 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/rubyred.PNG
+-rw-r--r--   0        0        0    30867 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/snowwhite.PNG
+-rw-r--r--   0        0        0    56113 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/widgets_display.PNG
+-rw-r--r--   0        0        0     2818 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/main.py
+-rw-r--r--   0        0        0     1244 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_classes.py
+-rw-r--r--   0        0        0     3414 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_main_window.py
+-rw-r--r--   0        0        0     9665 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_widgets.py
+-rw-r--r--   0        0        0      110 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/1.json
+-rw-r--r--   0        0        0      211 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/2.json
+-rw-r--r--   0        0        0    45119 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/bug.png
+-rw-r--r--   0        0        0      167 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/1.json
+-rw-r--r--   0        0        0      209 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/2.json
+-rw-r--r--   0        0        0    45119 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/bug.png
+-rw-r--r--   0        0        0      114 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.100/1.json
+-rw-r--r--   0        0        0       97 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.100/2.json
+-rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 qute_style-1.0.3/PKG-INFO
```

### Comparing `qute_style-1.0.2/LICENSE` & `qute_style-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/README.md` & `qute_style-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/pyproject.toml` & `qute_style-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qute_style"
-version = "1.0.2"
+version = "1.0.3"
 description = "QuteStyle is an expandable application framework for PySide6"
 authors = ["Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke <PS-TF-Entwicklung@tuev-sued.de>"]
 readme = "README.md"
 repository = "https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle"
 license = "MIT"
 packages = [
     {include = "qute_style"},
@@ -12,28 +12,27 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 PySide6 = "6.4.2"
 
 [tool.poetry.dev-dependencies]
-astroid = "2.12.14"
-pytest = "7.2.0"
+pytest = "7.3.1"
 pytest-qt = "4.2.0"
-requests = "2.28.2"
-black = "22.12.0"
-coverage = "7.0.5"
-isort = "5.11.4"
-mypy = "0.991"
-pre-commit = "2.21.0"
-pydocstyle = "6.2.3"
-pylint = "^2.15.10"
+requests = "2.29.0"
+black = "23.3.0"
+coverage = "7.2.3"
+isort = "5.12.0"
+mypy = "1.2.0"
+pre-commit = "3.2.2"
+pydocstyle = "6.3.0"
+pylint = "^2.17.3"
 pytest-cov = "^4.0.0"
 pytest-github-actions-annotate-failures = "^0.1.8"
-types-requests = "2.28.11.7"
+types-requests = "2.28.11.17"
 
 
 [tool.poetry.scripts]
 qute-style-example = "qute_style_examples.main:main_method"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `qute_style-1.0.2/qute_style/dev/dev_functions.py` & `qute_style-1.0.3/qute_style/dev/dev_functions.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/dev/mocks.py` & `qute_style-1.0.3/qute_style/dev/mocks.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/gen/ui_test_window.py` & `qute_style-1.0.3/qute_style/gen/ui_test_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,107 +70,120 @@
     QVBoxLayout,
     QWidget,
 )
 
 from qute_style.widgets.icon_button import IconButton
 from qute_style.widgets.styled_combobox import StyledComboBox
 from qute_style.widgets.toggle import Toggle
-from qute_style_examples.sample_classes import TestComboBox
+from qute_style_examples.sample_classes import (
+    SelectAllTestComboBox,
+    TestComboBox,
+)
 
 
 class Ui_test_widget(object):
     def setupUi(self, test_widget):
         if not test_widget.objectName():
             test_widget.setObjectName("test_widget")
         test_widget.resize(1219, 886)
         self.gridLayout_2 = QGridLayout(test_widget)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.groupBox_3 = QGroupBox(test_widget)
         self.groupBox_3.setObjectName("groupBox_3")
         self.groupBox_3.setCheckable(False)
         self.gridLayout = QGridLayout(self.groupBox_3)
         self.gridLayout.setObjectName("gridLayout")
-        self.horizontalSlider = QSlider(self.groupBox_3)
-        self.horizontalSlider.setObjectName("horizontalSlider")
-        self.horizontalSlider.setMaximum(100)
-        self.horizontalSlider.setValue(30)
-        self.horizontalSlider.setOrientation(Qt.Horizontal)
-
-        self.gridLayout.addWidget(self.horizontalSlider, 9, 1, 1, 1)
-
-        self.spinBox = QSpinBox(self.groupBox_3)
-        self.spinBox.setObjectName("spinBox")
-
-        self.gridLayout.addWidget(self.spinBox, 5, 0, 1, 2)
-
-        self.label = QLabel(self.groupBox_3)
-        self.label.setObjectName("label")
-
-        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
-
-        self.label_3 = QLabel(self.groupBox_3)
-        self.label_3.setObjectName("label_3")
+        self.lineEdit = QLineEdit(self.groupBox_3)
+        self.lineEdit.setObjectName("lineEdit")
+        self.lineEdit.setEchoMode(QLineEdit.Normal)
 
-        self.gridLayout.addWidget(self.label_3, 9, 0, 1, 1)
+        self.gridLayout.addWidget(self.lineEdit, 6, 0, 1, 2)
 
         self.horizontalScrollBar = QScrollBar(self.groupBox_3)
         self.horizontalScrollBar.setObjectName("horizontalScrollBar")
         self.horizontalScrollBar.setValue(25)
         self.horizontalScrollBar.setOrientation(Qt.Horizontal)
 
-        self.gridLayout.addWidget(self.horizontalScrollBar, 8, 1, 1, 1)
+        self.gridLayout.addWidget(self.horizontalScrollBar, 10, 1, 1, 1)
 
-        self.lineEdit = QLineEdit(self.groupBox_3)
-        self.lineEdit.setObjectName("lineEdit")
-        self.lineEdit.setEchoMode(QLineEdit.Normal)
+        self.label_3 = QLabel(self.groupBox_3)
+        self.label_3.setObjectName("label_3")
+
+        self.gridLayout.addWidget(self.label_3, 11, 0, 1, 1)
+
+        self.dateTimeEdit = QDateTimeEdit(self.groupBox_3)
+        self.dateTimeEdit.setObjectName("dateTimeEdit")
 
-        self.gridLayout.addWidget(self.lineEdit, 4, 0, 1, 2)
+        self.gridLayout.addWidget(self.dateTimeEdit, 8, 0, 1, 2)
 
         self.label_2 = QLabel(self.groupBox_3)
         self.label_2.setObjectName("label_2")
 
-        self.gridLayout.addWidget(self.label_2, 2, 0, 1, 1)
+        self.gridLayout.addWidget(self.label_2, 3, 0, 1, 1)
 
         self.dial = QDial(self.groupBox_3)
         self.dial.setObjectName("dial")
         self.dial.setValue(30)
 
-        self.gridLayout.addWidget(self.dial, 8, 0, 1, 1)
+        self.gridLayout.addWidget(self.dial, 10, 0, 1, 1)
 
-        self.dateTimeEdit = QDateTimeEdit(self.groupBox_3)
-        self.dateTimeEdit.setObjectName("dateTimeEdit")
+        self.styled_combobox = StyledComboBox(self.groupBox_3)
+        self.styled_combobox.addItem("")
+        self.styled_combobox.addItem("")
+        self.styled_combobox.addItem("")
+        self.styled_combobox.setObjectName("styled_combobox")
 
-        self.gridLayout.addWidget(self.dateTimeEdit, 6, 0, 1, 2)
+        self.gridLayout.addWidget(self.styled_combobox, 0, 1, 1, 1)
 
         self.transparent_combobox = StyledComboBox(self.groupBox_3)
         self.transparent_combobox.addItem("")
         self.transparent_combobox.addItem("")
         self.transparent_combobox.addItem("")
         self.transparent_combobox.setObjectName("transparent_combobox")
 
-        self.gridLayout.addWidget(self.transparent_combobox, 2, 1, 1, 1)
-
-        self.styled_combobox = StyledComboBox(self.groupBox_3)
-        self.styled_combobox.addItem("")
-        self.styled_combobox.addItem("")
-        self.styled_combobox.addItem("")
-        self.styled_combobox.setObjectName("styled_combobox")
-
-        self.gridLayout.addWidget(self.styled_combobox, 0, 1, 1, 1)
+        self.gridLayout.addWidget(self.transparent_combobox, 3, 1, 1, 1)
 
         self.label_4 = QLabel(self.groupBox_3)
         self.label_4.setObjectName("label_4")
 
         self.gridLayout.addWidget(self.label_4, 1, 0, 1, 1)
 
         self.checkable_combobox = TestComboBox(self.groupBox_3)
         self.checkable_combobox.setObjectName("checkable_combobox")
 
         self.gridLayout.addWidget(self.checkable_combobox, 1, 1, 1, 1)
 
+        self.horizontalSlider = QSlider(self.groupBox_3)
+        self.horizontalSlider.setObjectName("horizontalSlider")
+        self.horizontalSlider.setMaximum(100)
+        self.horizontalSlider.setValue(30)
+        self.horizontalSlider.setOrientation(Qt.Horizontal)
+
+        self.gridLayout.addWidget(self.horizontalSlider, 11, 1, 1, 1)
+
+        self.spinBox = QSpinBox(self.groupBox_3)
+        self.spinBox.setObjectName("spinBox")
+
+        self.gridLayout.addWidget(self.spinBox, 7, 0, 1, 2)
+
+        self.label = QLabel(self.groupBox_3)
+        self.label.setObjectName("label")
+
+        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
+
+        self.label_5 = QLabel(self.groupBox_3)
+        self.label_5.setObjectName("label_5")
+
+        self.gridLayout.addWidget(self.label_5, 2, 0, 1, 1)
+
+        self.comboBox = SelectAllTestComboBox(self.groupBox_3)
+        self.comboBox.setObjectName("comboBox")
+
+        self.gridLayout.addWidget(self.comboBox, 2, 1, 1, 1)
+
         self.gridLayout_2.addWidget(self.groupBox_3, 4, 1, 1, 1)
 
         self.groupBox_2 = QGroupBox(test_widget)
         self.groupBox_2.setObjectName("groupBox_2")
         self.verticalLayout_3 = QVBoxLayout(self.groupBox_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.pushButton = QPushButton(self.groupBox_2)
@@ -454,66 +467,69 @@
         self.gridLayout_2.addWidget(self.tabWidget, 4, 0, 1, 1)
 
         self.retranslateUi(test_widget)
 
         self.pushButton_4.setDefault(False)
         self.tabWidget.setCurrentIndex(4)
 
-        QMetaObject.connectSlotsByName(test_widget)
-
     # setupUi
 
     def retranslateUi(self, test_widget):
         test_widget.setWindowTitle(
             QCoreApplication.translate("test_widget", "Form", None)
         )
         self.groupBox_3.setTitle(
             QCoreApplication.translate("test_widget", "GroupBox", None)
         )
-        self.label.setText(
-            QCoreApplication.translate("test_widget", "Styled ComboBox", None)
+        self.lineEdit.setText(
+            QCoreApplication.translate("test_widget", "test", None)
         )
         self.label_3.setText(
             QCoreApplication.translate(
                 "test_widget", "Test QProgressBar:", None
             )
         )
-        self.lineEdit.setText(
-            QCoreApplication.translate("test_widget", "test", None)
-        )
         self.label_2.setText(
             QCoreApplication.translate(
                 "test_widget", "Transparent ComboBox", None
             )
         )
-        self.transparent_combobox.setItemText(
+        self.styled_combobox.setItemText(
             0, QCoreApplication.translate("test_widget", "New Item", None)
         )
-        self.transparent_combobox.setItemText(
+        self.styled_combobox.setItemText(
             1, QCoreApplication.translate("test_widget", "New Item 2", None)
         )
-        self.transparent_combobox.setItemText(
+        self.styled_combobox.setItemText(
             2, QCoreApplication.translate("test_widget", "New Item 3", None)
         )
 
-        self.styled_combobox.setItemText(
+        self.transparent_combobox.setItemText(
             0, QCoreApplication.translate("test_widget", "New Item", None)
         )
-        self.styled_combobox.setItemText(
+        self.transparent_combobox.setItemText(
             1, QCoreApplication.translate("test_widget", "New Item 2", None)
         )
-        self.styled_combobox.setItemText(
+        self.transparent_combobox.setItemText(
             2, QCoreApplication.translate("test_widget", "New Item 3", None)
         )
 
         self.label_4.setText(
             QCoreApplication.translate(
                 "test_widget", "Checkable ComboBox", None
             )
         )
+        self.label.setText(
+            QCoreApplication.translate("test_widget", "Styled ComboBox", None)
+        )
+        self.label_5.setText(
+            QCoreApplication.translate(
+                "test_widget", "SelectAll ComboBox", None
+            )
+        )
         self.groupBox_2.setTitle(
             QCoreApplication.translate("test_widget", "GroupBox", None)
         )
         self.pushButton.setText(
             QCoreApplication.translate("test_widget", "PushButton", None)
         )
         self.pushButton_2.setText(
```

### Comparing `qute_style-1.0.2/qute_style/gen/ui_whats_new_window.py` & `qute_style-1.0.3/qute_style/gen/ui_whats_new_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,14 @@
         whats_new_window.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(whats_new_window)
         self.statusbar.setObjectName("statusbar")
         whats_new_window.setStatusBar(self.statusbar)
 
         self.retranslateUi(whats_new_window)
 
-        QMetaObject.connectSlotsByName(whats_new_window)
-
     # setupUi
 
     def retranslateUi(self, whats_new_window):
         whats_new_window.setWindowTitle(
             QCoreApplication.translate(
                 "whats_new_window", "StyledMainWindow", None
             )
```

### Comparing `qute_style-1.0.2/qute_style/helper.py` & `qute_style-1.0.3/qute_style/helper.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/qs_application.py` & `qute_style-1.0.3/qute_style/qs_application.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/qs_main_window.py` & `qute_style-1.0.3/qute_style/qs_main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,15 +730,19 @@
 
         for widget in widgets:
             widget.store_settings()
             widget.shutdown_completed.connect(self.on_widget_shutdown)
             widget.shutdown()
 
     def on_widget_shutdown(self, widget: MainWidget) -> None:
-        """Handle a completed widget shutdown."""
+        """
+        Handle a completed widget shutdown.
+
+        If all widgets have shutdown the application is closed.
+        """
         log.debug("Widget completed shutdown: %s", widget)
         self._content.removeWidget(widget)
         if not self._content.count():
             log.debug("All widgets have shut down.")
             self.shutdown_complete.emit()
         else:
             log.debug(
```

### Comparing `qute_style-1.0.2/qute_style/qs_message_box.py` & `qute_style-1.0.3/qute_style/qs_message_box.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/qute_style.py` & `qute_style-1.0.3/qute_style/qute_style.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/accept_circle.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/accept_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/active_menu.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/add.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/add.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/add_circle.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/add_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/admin.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/admin.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/admin_panel.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/admin_panel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/arrow_back.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/arrow_back.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/block.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/block.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/bug.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/bug.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/check_circle.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/check_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/close.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/close.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/close_circle.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/close_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/copy.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/copy.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/cps_trends.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/cps_trends.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/delete.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/delete_forever.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/delete_forever.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/delete_import.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/delete_import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/document.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/document.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/document_scanner.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/document_scanner.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/error.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/error.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/expand_less.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/expand_less.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/expand_more.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/expand_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/file_distributor.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/file_distributor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/folder_open.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/folder_open.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/fullscreen.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/fullscreen_exit.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen_exit.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/heart_broken.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/heart_broken.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/help.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/help.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/home.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/home.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/ian_manager.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/ian_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/icon_PSE.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/icon_PSE.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/import.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/info.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/info.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/lidl_budget.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/lidl_budget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/menu.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/minimize.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/minimize.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/nav_updater.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/nav_updater.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/new_releases.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/new_releases.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/news.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/news.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/no_icon.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/package_commander.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/package_commander.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/palette.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/palette.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/pap.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/pap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/protocol_creator.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/protocol_creator.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/pzf_widget.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/pzf_widget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/qt.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/qt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/read_more.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/read_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/refresh.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/report_merger.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/report_merger.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/sap_excel.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/sap_excel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/save.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/save.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/save_alt.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/save_alt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/search.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/search.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/send.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/send.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/settings.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/settings.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/swap.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/swap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/sync.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/sync.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/template_selector.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/template_selector.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/testbase_manager.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/testbase_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/todo_circle.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/todo_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_icons/undo.svg` & `qute_style-1.0.3/qute_style/resources/svg_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_images/banner_qute_style.svg` & `qute_style-1.0.3/qute_style/resources/svg_images/banner_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_images/logo_chemistry.svg` & `qute_style-1.0.3/qute_style/resources/svg_images/logo_chemistry.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_images/logo_labmonitor.svg` & `qute_style-1.0.3/qute_style/resources/svg_images/logo_labmonitor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_images/logo_qute_style.svg` & `qute_style-1.0.3/qute_style/resources/svg_images/logo_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources/svg_images/logo_toolbox.svg` & `qute_style-1.0.3/qute_style/resources/svg_images/logo_toolbox.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/resources_rc.py` & `qute_style-1.0.3/qute_style/resources_rc.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/startup_threads.py` & `qute_style-1.0.3/qute_style/startup_threads.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/style.py` & `qute_style-1.0.3/qute_style/style.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/ui/test_window.ui` & `qute_style-1.0.3/qute_style/ui/test_window.ui`

 * *Files 4% similar despite different names*

#### Comparing `qute_style-1.0.2/qute_style/ui/test_window.ui` & `qute_style-1.0.3/qute_style/ui/test_window.ui`

```diff
@@ -19,83 +19,60 @@
           <property name="title">
             <string>GroupBox</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
           <layout class="QGridLayout" name="gridLayout">
-            <item row="9" column="1">
-              <widget class="QSlider" name="horizontalSlider">
-                <property name="maximum">
-                  <number>100</number>
-                </property>
-                <property name="value">
-                  <number>30</number>
-                </property>
-                <property name="orientation">
-                  <enum>Qt::Horizontal</enum>
-                </property>
-              </widget>
-            </item>
-            <item row="5" column="0" colspan="2">
-              <widget class="QSpinBox" name="spinBox"/>
-            </item>
-            <item row="0" column="0">
-              <widget class="QLabel" name="label">
+            <item row="6" column="0" colspan="2">
+              <widget class="QLineEdit" name="lineEdit">
                 <property name="text">
-                  <string>Styled ComboBox</string>
+                  <string>test</string>
                 </property>
-              </widget>
-            </item>
-            <item row="9" column="0">
-              <widget class="QLabel" name="label_3">
-                <property name="text">
-                  <string>Test QProgressBar:</string>
+                <property name="echoMode">
+                  <enum>QLineEdit::Normal</enum>
                 </property>
               </widget>
             </item>
-            <item row="8" column="1">
+            <item row="10" column="1">
               <widget class="QScrollBar" name="horizontalScrollBar">
                 <property name="value">
                   <number>25</number>
                 </property>
                 <property name="orientation">
                   <enum>Qt::Horizontal</enum>
                 </property>
               </widget>
             </item>
-            <item row="4" column="0" colspan="2">
-              <widget class="QLineEdit" name="lineEdit">
+            <item row="11" column="0">
+              <widget class="QLabel" name="label_3">
                 <property name="text">
-                  <string>test</string>
-                </property>
-                <property name="echoMode">
-                  <enum>QLineEdit::Normal</enum>
+                  <string>Test QProgressBar:</string>
                 </property>
               </widget>
             </item>
-            <item row="2" column="0">
+            <item row="8" column="0" colspan="2">
+              <widget class="QDateTimeEdit" name="dateTimeEdit"/>
+            </item>
+            <item row="3" column="0">
               <widget class="QLabel" name="label_2">
                 <property name="text">
                   <string>Transparent ComboBox</string>
                 </property>
               </widget>
             </item>
-            <item row="8" column="0">
+            <item row="10" column="0">
               <widget class="QDial" name="dial">
                 <property name="value">
                   <number>30</number>
                 </property>
               </widget>
             </item>
-            <item row="6" column="0" colspan="2">
-              <widget class="QDateTimeEdit" name="dateTimeEdit"/>
-            </item>
-            <item row="2" column="1">
-              <widget class="StyledComboBox" name="transparent_combobox">
+            <item row="0" column="1">
+              <widget class="StyledComboBox" name="styled_combobox">
                 <item>
                   <property name="text">
                     <string>New Item</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
@@ -105,16 +82,16 @@
                 <item>
                   <property name="text">
                     <string>New Item 3</string>
                   </property>
                 </item>
               </widget>
             </item>
-            <item row="0" column="1">
-              <widget class="StyledComboBox" name="styled_combobox">
+            <item row="3" column="1">
+              <widget class="StyledComboBox" name="transparent_combobox">
                 <item>
                   <property name="text">
                     <string>New Item</string>
                   </property>
                 </item>
                 <item>
                   <property name="text">
@@ -134,14 +111,47 @@
                   <string>Checkable ComboBox</string>
                 </property>
               </widget>
             </item>
             <item row="1" column="1">
               <widget class="TestComboBox" name="checkable_combobox"/>
             </item>
+            <item row="11" column="1">
+              <widget class="QSlider" name="horizontalSlider">
+                <property name="maximum">
+                  <number>100</number>
+                </property>
+                <property name="value">
+                  <number>30</number>
+                </property>
+                <property name="orientation">
+                  <enum>Qt::Horizontal</enum>
+                </property>
+              </widget>
+            </item>
+            <item row="7" column="0" colspan="2">
+              <widget class="QSpinBox" name="spinBox"/>
+            </item>
+            <item row="0" column="0">
+              <widget class="QLabel" name="label">
+                <property name="text">
+                  <string>Styled ComboBox</string>
+                </property>
+              </widget>
+            </item>
+            <item row="2" column="0">
+              <widget class="QLabel" name="label_5">
+                <property name="text">
+                  <string>SelectAll ComboBox</string>
+                </property>
+              </widget>
+            </item>
+            <item row="2" column="1">
+              <widget class="SelectAllTestComboBox" name="comboBox"/>
+            </item>
           </layout>
         </widget>
       </item>
       <item row="2" column="1">
         <widget class="QGroupBox" name="groupBox_2">
           <property name="title">
             <string>GroupBox</string>
@@ -659,11 +669,16 @@
       <header>qute_style.widgets.styled_combobox</header>
     </customwidget>
     <customwidget>
       <class>TestComboBox</class>
       <extends>QComboBox</extends>
       <header>qute_style_examples.sample_classes</header>
     </customwidget>
+    <customwidget>
+      <class>SelectAllTestComboBox</class>
+      <extends>QComboBox</extends>
+      <header>qute_style_examples.sample_classes</header>
+    </customwidget>
   </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `qute_style-1.0.2/qute_style/ui/whats_new_window.ui` & `qute_style-1.0.3/qute_style/ui/whats_new_window.ui`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/background_frame.py` & `qute_style-1.0.3/qute_style/widgets/background_frame.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/base_widgets.py` & `qute_style-1.0.3/qute_style/widgets/base_widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Base widget definitions."""
 from __future__ import annotations
 
 import logging
 from typing import cast
 
-from PySide6.QtCore import QThread, Signal, Slot
+from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QGridLayout, QVBoxLayout, QWidget
 
 log = logging.getLogger(
     f"qute_style.{__name__}"
 )  # pylint: disable=invalid-name
 
 
@@ -21,54 +21,44 @@
 
 
 class MainWidget(BaseWidget):
     """Base class for a widget that is display in the main section."""
 
     shutdown_completed = Signal(QWidget, name="shutdown_completed")
 
-    def __init__(self, parent: QWidget | None = None) -> None:
-        """Init the BaseWidget for a Widget in QuteStyle."""
-        self._thread: QThread | None = None
-        super().__init__(parent)
-
     def __repr__(self) -> str:
         """Return a str representation for the MainWidget."""
         return f"<{self.__class__} {self.NAME} {id(self)}>"
 
     def shutdown(self) -> None:
-        """Shutdown the application."""
+        """
+        Shutdown the application.
+
+        Can be overriden in case some special actions (finish threads, ...) are
+        needed to shutdown the widget. At the end shutdown_completed signal
+        must be emitted.
+        """
         log.debug("Shutting down tab %s", self.NAME)
-        if self._thread is not None and self._thread.isRunning():
-            log.debug("Thread is in running state %s", self.NAME)
-            # Disconnect the current handlers before attaching a new slot.
-            # In case of nav_loader a new thread would be started in the
-            # original finished handler which will then lead to an error
-            # when closing the app because this thread is still running.
-            # Restarting the app in this case fails.
-            self._thread.finished.disconnect()
-            self._thread.finished.connect(self.on_thread_finished)
-        else:
-            self.on_thread_finished()
+        self.shutdown_completed.emit(self)
 
     def store_settings(self) -> None:  # pragma: no cover
-        """Store the settings."""
+        """
+        Store the settings.
+
+        Can be overriden to store widget based information when the application
+        is closed.
+        """
 
     @property
     def settings_widget(
         self,
     ) -> None | QWidget:
         """Get the settings widget. Implemented by custom classes."""
         return None
 
-    @Slot(name="on_thread_finished")
-    def on_thread_finished(self) -> None:
-        """Handle the shutdown when the thread has finished."""
-        log.debug("On thread finished base class %s", self.NAME)
-        self.shutdown_completed.emit(self)
-
     def request_shutdown(self) -> bool:
         """
         Request shutdown from a widget so that the widget can interfere.
 
         If a widget wants to cancel the shutdown, it must reimplement this
         method and return False.
         """
```

### Comparing `qute_style-1.0.2/qute_style/widgets/color_manager.py` & `qute_style-1.0.3/qute_style/widgets/color_manager.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/credit_bar.py` & `qute_style-1.0.3/qute_style/widgets/credit_bar.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/custom_icon_engine.py` & `qute_style-1.0.3/qute_style/widgets/custom_icon_engine.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/drop_label.py` & `qute_style-1.0.3/qute_style/widgets/drop_label.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/grips.py` & `qute_style-1.0.3/qute_style/widgets/grips.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/home_page.py` & `qute_style-1.0.3/qute_style/widgets/home_page.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/icon.py` & `qute_style-1.0.3/qute_style/widgets/icon.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/icon_button.py` & `qute_style-1.0.3/qute_style/widgets/icon_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/icon_tooltip_button.py` & `qute_style-1.0.3/qute_style/widgets/icon_tooltip_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/left_column.py` & `qute_style-1.0.3/qute_style/widgets/left_column.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/left_column_close_button.py` & `qute_style-1.0.3/qute_style/widgets/left_column_close_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/left_menu.py` & `qute_style-1.0.3/qute_style/widgets/left_menu.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/left_menu_button.py` & `qute_style-1.0.3/qute_style/widgets/left_menu_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/spinner.py` & `qute_style-1.0.3/qute_style/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/text_truncator.py` & `qute_style-1.0.3/qute_style/widgets/text_truncator.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/title_bar.py` & `qute_style-1.0.3/qute_style/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/title_button.py` & `qute_style-1.0.3/qute_style/widgets/title_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/toggle.py` & `qute_style-1.0.3/qute_style/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style/widgets/tooltip.py` & `qute_style-1.0.3/qute_style/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/color_manager.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/color_manager.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/custom_style.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/custom_style.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/darcula.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/darcula.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/drop_label.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/drop_label.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/highbridge_grey.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/highbridge_grey.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/information_messagebox.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/information_messagebox.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/princesspink.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/princesspink.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/rubyred.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/rubyred.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/snowwhite.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/snowwhite.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/example_images/widgets_display.PNG` & `qute_style-1.0.3/qute_style_examples/example_images/widgets_display.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/main.py` & `qute_style-1.0.3/qute_style_examples/main.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/sample_main_window.py` & `qute_style-1.0.3/qute_style_examples/sample_main_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/sample_widgets.py` & `qute_style-1.0.3/qute_style_examples/sample_widgets.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/test_changelog/1.01/bug.png` & `qute_style-1.0.3/qute_style_examples/test_changelog/1.01/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/qute_style_examples/test_changelog/1.10/bug.png` & `qute_style-1.0.3/qute_style_examples/test_changelog/1.10/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.2/PKG-INFO` & `qute_style-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qute-style
-Version: 1.0.2
+Version: 1.0.3
 Summary: QuteStyle is an expandable application framework for PySide6
 Home-page: https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle
 License: MIT
 Author: Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke
 Author-email: PS-TF-Entwicklung@tuev-sued.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

