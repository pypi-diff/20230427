# Comparing `tmp/carefree-drawboard-0.0.0a8.tar.gz` & `tmp/carefree-drawboard-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a8.tar", last modified: Mon Apr 24 12:23:31 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a9.tar", last modified: Thu Apr 27 15:24:45 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a8.tar` & `carefree-drawboard-0.0.0a9.tar`

### file list

```diff
@@ -1,197 +1,202 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.736194 carefree-drawboard-0.0.0a8/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     8996 2023-04-24 12:23:31.736194 carefree-drawboard-0.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     8713 2023-04-24 10:36:28.000000 carefree-drawboard-0.0.0a8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.664644 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     8996 2023-04-24 12:23:29.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5639 2023-04-24 12:23:31.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:23:29.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:23:29.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-04-24 12:23:29.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 12:23:29.000000 carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.666644 carefree-drawboard-0.0.0a8/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.670194 carefree-drawboard-0.0.0a8/cfdraw/.web/
--rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.674194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      977 2023-04-24 08:35:50.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1454 2023-04-24 07:30:21.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     5803 2023-04-24 07:18:40.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.677193 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     2249 2023-04-19 04:21:39.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5952 2023-04-23 08:04:37.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1292 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.631100 carefree-drawboard-0.0.0a8/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.678193 carefree-drawboard-0.0.0a8/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.682194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      723 2023-04-22 13:46:05.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      640 2023-04-24 02:04:13.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFCircularProgress.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.683194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.683194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.686194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5200 2023-04-24 11:28:15.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.690193 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2302 2023-04-23 08:04:44.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     7075 2023-04-21 10:12:04.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1788 2023-04-24 03:25:59.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.695193 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/
--rw-rw-rw-   0        0        0     2806 2023-04-23 04:26:50.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      876 2023-04-23 04:26:57.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4807 2023-04-23 04:27:02.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      852 2023-04-23 04:27:13.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3471 2023-04-23 04:27:24.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1081 2023-04-23 04:27:32.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1121 2023-04-23 04:21:09.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     1309 2023-04-24 04:42:50.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/MetaPlugin.tsx
--rw-rw-rw-   0        0        0     6478 2023-04-23 04:27:51.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5072 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2372 2023-04-23 04:28:10.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0     1251 2023-04-24 08:34:30.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.699194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0      685 2023-04-21 06:07:38.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
--rw-rw-rw-   0        0        0     3923 2023-04-24 04:50:52.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2825 2023-04-24 11:29:08.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1945 2023-04-24 04:47:37.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
--rw-rw-rw-   0        0        0     1730 2023-04-24 11:29:19.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      851 2023-04-24 04:49:31.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.701194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.704194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0    11011 2023-04-24 11:37:21.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7028 2023-04-24 06:13:05.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0      225 2023-04-21 05:52:53.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/hooks.ts
--rw-rw-rw-   0        0        0     2343 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.707194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.708194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0     1028 2023-04-19 04:57:46.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     2546 2023-04-24 07:30:12.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.709194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.712195 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     3827 2023-04-24 11:27:58.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1758 2023-04-24 04:08:41.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3137 2023-04-24 06:12:21.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.718195 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     1531 2023-04-24 07:46:09.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0      586 2023-04-24 06:37:16.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/debug.ts
--rw-rw-rw-   0        0        0     1495 2023-04-21 10:35:17.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-24 08:27:40.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/pluginVisible.ts
--rw-rw-rw-   0        0        0     2505 2023-04-24 08:59:38.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     6076 2023-04-24 07:30:05.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/socket.ts
--rw-rw-rw-   0        0        0     3845 2023-04-24 08:00:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2031 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/ui.ts
--rw-rw-rw-   0        0        0      866 2023-04-23 10:06:41.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/user.ts
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.721194 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      533 2023-04-24 02:26:58.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1091 2023-04-24 04:41:20.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a8/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      487 2023-04-24 10:12:18.000000 carefree-drawboard-0.0.0a8/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.722194 carefree-drawboard-0.0.0a8/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-23 08:15:58.000000 carefree-drawboard-0.0.0a8/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.725195 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      139 2023-04-23 08:15:42.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      745 2023-04-21 12:01:39.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/assets.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     5713 2023-04-19 04:49:15.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     6044 2023-04-24 12:21:12.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/queue.py
--rw-rw-rw-   0        0        0     2158 2023-04-19 04:21:46.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     3323 2023-04-24 09:42:32.000000 carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0     1392 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a8/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3333 2023-04-22 02:31:01.000000 carefree-drawboard-0.0.0a8/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2245 2023-04-21 12:04:53.000000 carefree-drawboard-0.0.0a8/cfdraw/config.py
--rw-rw-rw-   0        0        0     1456 2023-04-21 11:42:04.000000 carefree-drawboard-0.0.0a8/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.726194 carefree-drawboard-0.0.0a8/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a8/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a8/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6847 2023-04-24 01:38:38.000000 carefree-drawboard-0.0.0a8/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.728194 carefree-drawboard-0.0.0a8/cfdraw/plugins/
--rw-rw-rw-   0        0        0       92 2023-04-23 04:40:40.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4832 2023-04-24 11:50:35.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.728194 carefree-drawboard-0.0.0a8/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-04-22 12:17:12.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.730194 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0      100 2023-04-23 09:08:34.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0      908 2023-04-23 09:30:55.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      728 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/send_message.py
--rw-rw-rw-   0        0        0      500 2023-04-23 09:31:13.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      962 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0      920 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a8/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.731194 carefree-drawboard-0.0.0a8/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a8/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a8/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0    12906 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a8/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:23:31.735194 carefree-drawboard-0.0.0a8/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     6414 2023-04-24 12:16:17.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/data_structures.py
--rw-rw-rw-   0        0        0     2622 2023-04-22 02:30:59.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0     2040 2023-04-24 11:54:48.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/misc.py
--rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2691 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a8/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-24 12:23:31.740193 carefree-drawboard-0.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-04-24 12:23:06.000000 carefree-drawboard-0.0.0a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     9233 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     8950 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.475951 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9233 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5867 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.477949 carefree-drawboard-0.0.0a9/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.481949 carefree-drawboard-0.0.0a9/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.485949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      992 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1454 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     6410 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.489949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9418 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1776 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     1970 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1292 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3304 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1018 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.451465 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.489949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.495950 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      763 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.496949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1484 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.497949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFText.tsx
+-rw-rw-rw-   0        0        0      408 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFTooltip.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.499949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     2924 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     2003 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5154 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      131 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.503949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1508 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2302 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     7075 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     2343 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/tooltip.ts
+-rw-rw-rw-   0        0        0     1788 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.503949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.507949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0      681 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+-rw-rw-rw-   0        0        0     4421 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2699 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1936 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0     1627 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0      847 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.513949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/
+-rw-rw-rw-   0        0        0     2690 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      714 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3430 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1083 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1123 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1311 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     6321 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5074 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2374 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1253 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.515949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.517949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1317 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      689 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      780 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1129 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      580 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0    11507 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7028 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      225 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2441 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.518949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.519949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1028 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     3151 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.520949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.522949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     4081 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/fields.ts
+-rw-rw-rw-   0        0        0     1806 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0      190 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3154 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.529950 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     2918 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0      586 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0     1457 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pluginVisible.ts
+-rw-rw-rw-   0        0        0     2874 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     2060 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pointerEvents.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0      525 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/settings.ts
+-rw-rw-rw-   0        0        0     7004 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     3859 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2031 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      866 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.531949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      533 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1091 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0     2012 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1849 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   214083 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      487 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.532948 carefree-drawboard-0.0.0a9/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a9/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.535948 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     5713 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     6920 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     2158 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3674 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1277 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3333 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2245 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/config.py
+-rw-rw-rw-   0        0        0     1456 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.536948 carefree-drawboard-0.0.0a9/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6847 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.538948 carefree-drawboard-0.0.0a9/cfdraw/plugins/
+-rw-rw-rw-   0        0        0       92 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4774 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.538948 carefree-drawboard-0.0.0a9/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.540948 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0      100 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      735 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      500 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      643 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0      959 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.541949 carefree-drawboard-0.0.0a9/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3153 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    14769 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     6551 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/data_structures.py
+-rw-rw-rw-   0        0        0     2622 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     2337 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2744 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-27 15:24:45.550951 carefree-drawboard-0.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-04-27 15:24:12.000000 carefree-drawboard-0.0.0a9/setup.py
```

### Comparing `carefree-drawboard-0.0.0a8/LICENSE` & `carefree-drawboard-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/PKG-INFO` & `carefree-drawboard-0.0.0a9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,15 +69,15 @@
 
 > When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
 
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
-[Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
+[Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
@@ -86,15 +86,15 @@
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
 
-`carefree-drawboard` 🎨 is at a VERY early stage. It is launched in April 2023, and is not production ready (yet).
+`carefree-drawboard` 🎨 is at a VERY early stage (it is launched in April 2023), so although it could be production ready (see [here](https://github.com/carefree0910/carefree-drawboard/wiki/Production) for more details), it does not have many real world use cases (yet).
 
 But we will rapidly update this project and launch new features every week (or, even everyday), so ⭐ star and 👀 watch this repository to stay up to date!
 
 ## Contributing
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
@@ -152,8 +152,9 @@
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
+- [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
```

### Comparing `carefree-drawboard-0.0.0a8/README.md` & `carefree-drawboard-0.0.0a9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 > When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
 
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
-[Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
+[Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
@@ -76,15 +76,15 @@
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
 
-`carefree-drawboard` 🎨 is at a VERY early stage. It is launched in April 2023, and is not production ready (yet).
+`carefree-drawboard` 🎨 is at a VERY early stage (it is launched in April 2023), so although it could be production ready (see [here](https://github.com/carefree0910/carefree-drawboard/wiki/Production) for more details), it does not have many real world use cases (yet).
 
 But we will rapidly update this project and launch new features every week (or, even everyday), so ⭐ star and 👀 watch this repository to stay up to date!
 
 ## Contributing
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
@@ -142,8 +142,9 @@
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
+- [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
```

### Comparing `carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,15 +69,15 @@
 
 > When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
 
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
-[Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
+[Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
@@ -86,15 +86,15 @@
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
 
-`carefree-drawboard` 🎨 is at a VERY early stage. It is launched in April 2023, and is not production ready (yet).
+`carefree-drawboard` 🎨 is at a VERY early stage (it is launched in April 2023), so although it could be production ready (see [here](https://github.com/carefree0910/carefree-drawboard/wiki/Production) for more details), it does not have many real world use cases (yet).
 
 But we will rapidly update this project and launch new features every week (or, even everyday), so ⭐ star and 👀 watch this repository to stay up to date!
 
 ## Contributing
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
@@ -152,8 +152,9 @@
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
+- [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
```

### Comparing `carefree-drawboard-0.0.0a8/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 cfdraw/.web/src/components/CFDivider.tsx
 cfdraw/.web/src/components/CFHeading.tsx
 cfdraw/.web/src/components/CFImageUploader.tsx
 cfdraw/.web/src/components/CFInput.tsx
 cfdraw/.web/src/components/CFSlider.tsx
 cfdraw/.web/src/components/CFSwitch.tsx
 cfdraw/.web/src/components/CFText.tsx
+cfdraw/.web/src/components/CFTooltip.tsx
 cfdraw/.web/src/components/CFIcon/index.scss
 cfdraw/.web/src/components/CFIcon/index.tsx
 cfdraw/.web/src/components/CFSelect/index.scss
 cfdraw/.web/src/components/CFSelect/index.tsx
 cfdraw/.web/src/hooks/useFileDropper.ts
 cfdraw/.web/src/hooks/useGridLines.ts
 cfdraw/.web/src/hooks/useInitBoard.ts
@@ -64,34 +65,35 @@
 cfdraw/.web/src/lang/download.ts
 cfdraw/.web/src/lang/index.ts
 cfdraw/.web/src/lang/nodeEditor.ts
 cfdraw/.web/src/lang/plugins.ts
 cfdraw/.web/src/lang/projects.ts
 cfdraw/.web/src/lang/settings.ts
 cfdraw/.web/src/lang/toast.ts
+cfdraw/.web/src/lang/tooltip.ts
 cfdraw/.web/src/lang/ui.ts
-cfdraw/.web/src/plugins/AddPlugin.tsx
-cfdraw/.web/src/plugins/ArrangePlugin.tsx
-cfdraw/.web/src/plugins/BrushPlugin.tsx
-cfdraw/.web/src/plugins/DeletePlugin.tsx
-cfdraw/.web/src/plugins/DownloadPlugin.tsx
-cfdraw/.web/src/plugins/GroupPlugin.tsx
-cfdraw/.web/src/plugins/LinksPlugin.tsx
-cfdraw/.web/src/plugins/MetaPlugin.tsx
-cfdraw/.web/src/plugins/ProjectPlugin.tsx
-cfdraw/.web/src/plugins/SettingsPlugin.tsx
-cfdraw/.web/src/plugins/TextEditorPlugin.tsx
-cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/index.tsx
 cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
 cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
 cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
 cfdraw/.web/src/plugins/_python/QAPlugin.tsx
 cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
+cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
 cfdraw/.web/src/plugins/components/hooks.ts
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
@@ -100,28 +102,30 @@
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
 cfdraw/.web/src/requests/actions.ts
 cfdraw/.web/src/requests/hooks.ts
 cfdraw/.web/src/requests/interceptors/_python.ts
 cfdraw/.web/src/requests/interceptors/index.ts
 cfdraw/.web/src/schema/_python.ts
+cfdraw/.web/src/schema/fields.ts
 cfdraw/.web/src/schema/meta.ts
-cfdraw/.web/src/schema/metaFields.ts
 cfdraw/.web/src/schema/misc.ts
 cfdraw/.web/src/schema/plugins.ts
 cfdraw/.web/src/schema/requests.ts
 cfdraw/.web/src/stores/_python.ts
 cfdraw/.web/src/stores/debug.ts
 cfdraw/.web/src/stores/gridLines.ts
 cfdraw/.web/src/stores/hooks.ts
 cfdraw/.web/src/stores/init.ts
 cfdraw/.web/src/stores/meta.ts
 cfdraw/.web/src/stores/pluginVisible.ts
 cfdraw/.web/src/stores/plugins.ts
+cfdraw/.web/src/stores/pointerEvents.ts
 cfdraw/.web/src/stores/projects.ts
+cfdraw/.web/src/stores/settings.ts
 cfdraw/.web/src/stores/socket.ts
 cfdraw/.web/src/stores/theme.ts
 cfdraw/.web/src/stores/ui.ts
 cfdraw/.web/src/stores/user.ts
 cfdraw/.web/src/utils/bem.ts
 cfdraw/.web/src/utils/constants.ts
 cfdraw/.web/src/utils/event.ts
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/package.json` & `carefree-drawboard-0.0.0a9/cfdraw/.web/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961734693877551%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '~0.4.10-alpha.4', '@carefree0910/core': "*

 * *                   "'~0.4.10-alpha.1', '@carefree0910/native': '~0.4.10-alpha.4'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "dependencies": {
-        "@carefree0910/business": "^0.4.10-alpha.2",
-        "@carefree0910/core": "^0.4.10-alpha.1",
-        "@carefree0910/native": "^0.4.10-alpha.2",
+        "@carefree0910/business": "~0.4.10-alpha.4",
+        "@carefree0910/core": "~0.4.10-alpha.1",
+        "@carefree0910/native": "~0.4.10-alpha.4",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/App.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
-import { langStore } from "@carefree0910/business";
-
 import { useWebSocket } from "./stores/socket";
+import { usePointerEvents } from "./stores/pointerEvents";
 import { useUserInitialization } from "./stores/user";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
 import { useSyncPython } from "./hooks/usePython";
 import BoardPanel from "./BoardPanel";
 
 function App() {
   useWebSocket();
   useUserInitialization();
   useSyncPython();
   useInitBoard();
-  useFileDropper(langStore.tgt);
+  useFileDropper();
   useGridLines();
   usePreventDefaults();
+  usePointerEvents();
 
   return (
     <Flex h="100vh" className="p-editor" direction="column" userSelect="none">
       <Flex w="100%" flex={1}>
         <BoardPanel />
       </Flex>
     </Flex>
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/_settings.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,256 @@
 import type { AvailablePlugins, IMakePlugin } from "@/schema/plugins";
 
 export const reactPluginSettings: IMakePlugin<AvailablePlugins>[] = [
   {
-    type: "meta",
-    props: {
-      nodeConstraint: "singleNode",
-      renderInfo: {
-        w: 400,
-        h: 400,
-        offsetY: 48,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/0ec1b08f9c3e4ef4813ecb80bebf3b42.png",
-        pivot: "rt",
-        follow: true,
-      },
-      pluginInfo: {},
-    },
-  },
-  {
     type: "settings",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 400,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/49223052f17f4f249c56ba00f43b3043.png",
+        src: "https://user-images.githubusercontent.com/15677328/234536549-87e94432-9f25-490f-8dee-7ed166bcbeed.svg",
+        tooltip: "settings-tooltip",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
   {
     type: "project",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 400,
         offsetY: 64,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/255c1c20b5754815b759969218f8a87c.png",
+        src: "https://user-images.githubusercontent.com/15677328/234536679-103c6d6a-f882-4a99-baaf-02f71fefeea5.svg",
+        tooltip: "project-management-tooltip",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
   {
     type: "add",
     props: {
-      p: "14px",
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 225,
         offsetY: 120,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/81a82eca03224bc2bb8de65c08f2f48a.png",
+        src: "https://user-images.githubusercontent.com/15677328/234536800-4e2d9090-8958-4da9-8600-1e708f86759a.svg",
+        tooltip: "add-new-stuff-tooltip",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
   {
-    type: "arrange",
+    type: "brush",
     props: {
-      nodeConstraint: "multiNode",
+      nodeConstraint: "none",
       renderInfo: {
-        w: 0,
-        h: 0,
-        offsetY: 48,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/7fcc3fb8a25248b0a1f2ca68b0c975f4.png",
+        w: 300,
+        h: 220,
+        offsetY: 176,
+        src: "https://user-images.githubusercontent.com/15677328/234537027-20b3ea26-a6d0-4e07-8186-e2649917a893.svg",
+        tooltip: "enter-sketch-mode-tooltip",
         pivot: "rt",
-        follow: true,
+        follow: false,
       },
       pluginInfo: {},
-      noExpand: true,
     },
   },
   {
     type: "undo",
     props: {
-      p: "14px",
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
         offsetX: -28,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/069122c037d34d97ba10157438af131b.png",
+        src: "https://user-images.githubusercontent.com/15677328/234537508-b7ef4494-f2db-438b-b7cb-2f8d04833cb0.svg",
+        tooltip: "undo-tooltip",
         pivot: "top",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "redo",
     props: {
-      p: "14px",
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
         offsetX: 28,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/4c0b2343838344fdb574520006aa83c9.png",
+        src: "https://user-images.githubusercontent.com/15677328/234537560-552bc9bc-b0dc-45a5-af77-f14a2f2dbf80.svg",
+        tooltip: "redo-tooltip",
         pivot: "top",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
+    type: "meta",
+    props: {
+      nodeConstraint: "singleNode",
+      renderInfo: {
+        w: 400,
+        h: 400,
+        offsetY: 48,
+        src: "https://user-images.githubusercontent.com/15677328/234533823-12d27a77-155a-4743-a0af-1fc5b86014fd.svg",
+        pivot: "rt",
+        follow: true,
+      },
+      pluginInfo: {},
+    },
+  },
+  {
     type: "download",
     props: {
       nodeConstraint: "anyNode",
       renderInfo: {
         w: 240,
         h: 230,
         offsetY: -48,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/d871d80a875146fa8aabc09fbbdef47e.png",
+        src: "https://user-images.githubusercontent.com/15677328/234537900-4f52af0b-3be0-4a9a-b70b-ec28198323f0.svg",
         pivot: "rb",
         follow: true,
       },
       pluginInfo: {},
     },
   },
   {
     type: "delete",
     props: {
       nodeConstraint: "anyNode",
       renderInfo: {
         w: 0,
         h: 0,
         offsetY: -48,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/384b2261faa748e6b57e14e697e19520.png",
+        src: "https://user-images.githubusercontent.com/15677328/234538170-7374b2a1-edac-45c5-9615-96adf310a4c4.svg",
         pivot: "lb",
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "textEditor",
     props: {
-      p: "13px",
       nodeConstraint: "text",
       renderInfo: {
         w: 300,
         h: 400,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/06dc5af9d77944c8ae06d1ae1124b6a2.png",
+        src: "https://user-images.githubusercontent.com/15677328/234545067-1da07d56-9d53-4fbb-83cc-395ff953b4c6.svg",
+        tooltip: "text-editor-tooltip",
         pivot: "right",
         follow: true,
       },
       pluginInfo: {},
     },
   },
   {
     type: "groupEditor",
     props: {
-      // p: "13px",
       nodeConstraint: "group",
       renderInfo: {
         w: 0,
         h: 0,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/b767f4a99956498a922470174a2051df.png",
+        src: "https://user-images.githubusercontent.com/15677328/234545700-0d33471a-b43b-47af-a371-b2b3b8a98794.svg",
+        tooltip: "ungroup-the-nodes-tooltip",
         pivot: "rt",
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "multiEditor",
     props: {
-      // p: "13px",
       nodeConstraint: "multiNode",
       renderInfo: {
         w: 0,
         h: 0,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/669c405bee944a9a91fc4aa68f858cc3.png",
+        src: "https://user-images.githubusercontent.com/15677328/234545875-ff953782-7a18-4e0a-997c-37522fcbd2fd.svg",
+        tooltip: "group-the-nodes-tooltip",
         pivot: "rt",
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
-    type: "brush",
+    type: "arrange",
     props: {
-      p: "0px",
-      pl: "10px",
-      pr: "7px",
-      nodeConstraint: "none",
+      nodeConstraint: "multiNode",
       renderInfo: {
-        w: 300,
-        h: 220,
-        offsetY: 176,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/static/brush.svg",
+        w: 0,
+        h: 0,
+        offsetY: 48,
+        src: "https://user-images.githubusercontent.com/15677328/234545341-870f888e-0dfc-4d8e-a79b-fcb9ddbe0977.svg",
+        tooltip: "auto-arrange-tooltip",
         pivot: "rt",
-        follow: false,
+        follow: true,
       },
       pluginInfo: {},
+      noExpand: true,
     },
   },
   {
     type: "wiki",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/7ca6f41cad574f35ab117d6cfbe53be4.png",
+        src: "https://user-images.githubusercontent.com/15677328/234538371-88891a34-1b30-4c2b-bd2e-a80e2030210d.svg",
+        tooltip: "wiki-tooltip",
         pivot: "rb",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
-    type: "email",
+    type: "github",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
-        offsetX: -120,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/7ff42ebb21664a9abb55331463951126.png",
+        offsetX: -61,
+        src: "https://user-images.githubusercontent.com/15677328/234538604-3017a411-e5f1-4564-8bc0-5090e973d86b.svg",
+        tooltip: "github-tooltip",
         pivot: "rb",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
-    type: "github",
+    type: "email",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
-        offsetX: -64,
-        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/4fb8d24d515744f6ac6836b3ba12a649.png",
+        offsetX: -120,
+        src: "https://user-images.githubusercontent.com/15677328/234538781-b59b514f-99be-4ca2-859d-601f024cd7e0.svg",
+        tooltip: "email-tooltip",
         pivot: "rb",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
 ];
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/arrange.ts`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,24 @@
   Coordinate,
   Dictionary,
   getCenteredBBox,
   HitTest,
   INode,
   INodes,
   INodeType,
-  Lang,
   Matrix2DFields,
   range,
   runGroupContext,
   setDefault,
   sortBy,
 } from "@carefree0910/core";
-import { BoardStore, translate } from "@carefree0910/business";
+import { BoardStore } from "@carefree0910/business";
 
-import type { IToast } from "@/schema/misc";
 import { checkMeta, getOriginMeta, IMeta } from "@/schema/meta";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 
 const schedules = {
   easeInOutElastic: (x: number): number => {
     const c5 = (2 * Math.PI) / 4.5;
     return x === 0
       ? 0
@@ -110,24 +108,22 @@
   packs.forEach(({ node, attachTo }) => {
     if (!attachTo) return;
     const centerTarget = attachTo.node.bbox.center.add(attachTo.delta);
     node.bbox = node.bbox.move(centerTarget.subtract(node.bbox.center));
   });
 }
 async function animateArrangement(
-  t: IToast,
-  lang: Lang,
   original: INode[],
   targets: INode[],
   numFrame: number,
   trace: boolean,
   schedule: ScheduleType,
 ): Promise<void> {
   if (original.every((node, i) => node.bbox.closeTo(targets[i].bbox, { atol: 0.1, rtol: 0.1 }))) {
-    toast(t, "info", translate(Toast_Words["auto-arrange-no-need-message"], lang));
+    toastWord("info", Toast_Words["auto-arrange-no-need-message"]);
     return;
   }
 
   async function matchBBox(trace: boolean, fields: Dictionary<Matrix2DFields>): Promise<void> {
     const existingNodes = BoardStore.board.getNodes();
     await BoardStore.board.executer.executeNoBusiness(
       "matchBBox",
@@ -208,40 +204,40 @@
     const meta = node.type === "group" ? undefined : node.meta;
     let key, origin;
     if (!checkMeta(meta)) {
       key = `${defaultPrefix}${node.alias.split(".").slice(0, -1).join(".")}`;
       origin = undefined;
     } else {
       origin = getOriginMeta(meta);
-      key = !origin ? defaultPrefix : origin.data.timestamp?.toString() ?? "";
+      key = !origin ? defaultPrefix : origin.data.elapsedTimes?.endTime?.toString() ?? "";
     }
     const packs = setDefault(packsGroupByKey, key, []);
     packs.push({
       node,
       resized: resizedAABBs[node.alias],
       origin,
       attachTo: attachToMapping[node.alias],
     });
     groupLatestTimestamps[key] = Math.max(
-      meta?.data?.timestamp ?? 0,
+      meta?.data?.elapsedTimes?.endTime ?? 0,
       groupLatestTimestamps[key] ?? 0,
     );
   });
 
   const allSortedPacks: ArrangePack[] = [];
   const allKeys = Object.keys(packsGroupByKey);
   const sortedKeys = sortBy(
     allKeys,
     allKeys.map((key) => (key.startsWith(defaultPrefix) ? 0 : groupLatestTimestamps[key])),
   );
   sortedKeys.forEach((key) => {
     const packs = packsGroupByKey[key];
     const sortedPacks = sortBy(
       packs,
-      packs.map(({ origin }) => origin?.data.timestamp ?? 0),
+      packs.map(({ origin }) => origin?.data.elapsedTimes?.endTime ?? 0),
     );
     sortedPacks.forEach((pack) => allSortedPacks.push(pack));
   });
   // arrange to grid
   arrangeWith(allSortedPacks, commonW, padding);
   // align to center
   runGroupContext(
@@ -262,28 +258,25 @@
     new INodes(targets),
     { forceGroup: true },
   );
 
   return { original, targets };
 }
 export async function autoArrange(
-  t: IToast,
-  lang: Lang,
   nodes: INode[],
   opt?: Partial<AutoArrangeOptions>,
 ): Promise<void> {
   const { original, targets } = getArrangements(nodes, opt);
   const { numFrame, trace, schedule } = getDefaultArrangeOptions(opt);
-  animateArrangement(t, lang, original, targets, numFrame, trace, schedule);
+  animateArrangement(original, targets, numFrame, trace, schedule);
 }
-export function onArrange(
-  t: IToast,
-  lang: Lang,
-  { type, nodes }: { type: "none" | "multiple"; nodes: INodeType[] },
-): void {
-  autoArrange(
-    t,
-    lang,
-    type === "none" ? BoardStore.graph.rootNodes.filter((node) => !node.noSave) : nodes,
-    { fitContainer: type === "none" },
-  );
+export function onArrange({
+  type,
+  nodes,
+}: {
+  type: "none" | "multiple";
+  nodes: INodeType[];
+}): void {
+  autoArrange(type === "none" ? BoardStore.graph.rootNodes.filter((node) => !node.noSave) : nodes, {
+    fitContainer: type === "none",
+  });
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/download.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 import JSZip from "jszip";
 
-import { Graph, INode, Lang, download, toJsonBlob } from "@carefree0910/core";
-import { translate } from "@carefree0910/business";
+import { Graph, INode, download, toJsonBlob } from "@carefree0910/core";
 
-import type { DownloadFormat, IToast } from "@/schema/misc";
-import { toast } from "@/utils/toast";
+import type { DownloadFormat } from "@/schema/misc";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { useCurrentFullProject } from "./manageProjects";
 import { Exporter } from "./export";
 
-export function downloadCurrentFullProject(t: IToast, lang: Lang): void {
+export function downloadCurrentFullProject(): void {
   const fullProject = useCurrentFullProject();
-  toast(t, "info", translate(Toast_Words["downloading-project-message"], lang));
+  toastWord("info", Toast_Words["downloading-project-message"]);
   const blob = toJsonBlob(fullProject);
   download(blob, `${fullProject.name}.cfdraw`);
 }
 
 export async function downloadNodes(
-  t: IToast,
-  lang: Lang,
   nodes: INode[],
   format: DownloadFormat,
   exportOriginalSize: boolean,
 ): Promise<void> {
-  toast(t, "info", translate(Toast_Words["downloading-nodes-message"], lang));
+  toastWord("info", Toast_Words["downloading-nodes-message"]);
   if (format === "NOLI") {
     const graph = Graph.fromNodes(nodes);
     await download(toJsonBlob(graph.toJsonInfo()), "exported.noli");
   } else {
     const blobs = await Promise.all(
-      nodes.map((node) => Exporter.exportOne(t, lang, node, format, exportOriginalSize)),
+      nodes.map((node) => Exporter.exportOne(node, format, exportOriginalSize)),
     );
     const valid = blobs
       .map((blob, i) => ({ blob, node: nodes[i] }))
       .filter(({ blob }) => !!blob) as { blob: Blob; node: INode }[];
     if (valid.length === 0) return;
     const appendix = format.toLowerCase();
     if (valid.length === 1) {
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/export.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,51 @@
-import { INode, ISingleNode, Lang, toJsonBlob } from "@carefree0910/core";
+import { INode, ISingleNode, toJsonBlob } from "@carefree0910/core";
 import { ExportBlobOptions, exportBlob, exportNodes } from "@carefree0910/svg";
-import { translate } from "@carefree0910/business";
 
-import type { DownloadFormat, IToast, ImageFormat } from "@/schema/misc";
-import { toast } from "@/utils/toast";
+import type { DownloadFormat, ImageFormat } from "@/schema/misc";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Requests } from "@/requests/actions";
 import { uploadImage } from "./uploadImage";
 
 const isImage = (format: DownloadFormat) => format === "JPG" || format === "PNG";
 
 function fetchImage(data: { url: string; jpeg: boolean }): Promise<Blob> {
   return Requests.postJson<Blob>("_python", "/fetch_image", data, "blob");
 }
 
-export type IExportBlob = ExportBlobOptions & { t: IToast; lang: Lang };
 export class Exporter {
-  static async exportBlob(
-    nodes: ISingleNode[],
-    { t, lang, ...others }: IExportBlob,
-  ): Promise<Blob | void> {
+  static async exportBlob(nodes: ISingleNode[], opt: ExportBlobOptions): Promise<Blob | void> {
     return exportBlob(nodes, {
-      failedCallback: async () =>
-        toast(t, "error", translate(Toast_Words["export-blob-error-message"], lang)),
-      ...others,
+      failedCallback: async () => toastWord("error", Toast_Words["export-blob-error-message"]),
+      ...opt,
     });
   }
 
   static async exportOne(
-    t: IToast,
-    lang: Lang,
     node: INode,
     format: ImageFormat,
     exportOriginalSize: boolean,
   ): Promise<Blob | void> {
     const jpeg = format === "JPG";
     if (isImage(format) && node.type === "image" && exportOriginalSize) {
       return fetchImage({ url: node.renderParams.src, jpeg });
     }
     const bounding = node.bbox.bounding.toAABB();
     const targetNodes = node.type === "group" ? node.allChildrenNodes : [node];
     if (isImage(format)) {
       const blob = await Exporter.exportBlob(targetNodes, {
-        t,
-        lang,
         exportOptions: { exportBox: bounding },
       });
       if (!blob || format !== "JPG") return blob;
-      const res = await uploadImage(t, lang, blob, { failed: async () => void 0 });
+      const res = await uploadImage(blob, { failed: async () => void 0 });
       if (!res) return;
       return fetchImage({ url: res.url, jpeg: true });
     }
     const res = await exportNodes(targetNodes, { exportBox: bounding });
     if (!res) {
-      toast(t, "error", translate(Toast_Words["export-blob-error-message"], lang));
+      toastWord("error", Toast_Words["export-blob-error-message"]);
       return;
     }
     return toJsonBlob(res.svg.svg());
   }
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,93 +1,87 @@
-import { Dictionary, RectangleShapeNode, getRandomHash, shallowCopy } from "@carefree0910/core";
-import { BoardStore, translate, useAddNode } from "@carefree0910/business";
+import { RectangleShapeNode, getRandomHash, shallowCopy } from "@carefree0910/core";
+import { BoardStore, useAddNode } from "@carefree0910/business";
 
 import type { IMetaData, IPythonFieldsMetaData, MetaType } from "@/schema/meta";
 import type { IImportMeta } from "@/schema/meta";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { updateMeta } from "./update";
 import { addNewText } from "./addText";
 import { addNewImage, getNewRectangle, INewRectangle, NewImageInfo } from "./addImage";
 import { getArrangements } from "./arrange";
 
 // consumers
 
-function updateTimestamps(alias: string, createTime?: number): void {
+function updateElapsedTimes(alias: string): void {
   const node = BoardStore.graph.getNode(alias);
   if (!node || node.type === "group" || !node.params.meta?.data) return;
-  const now = Date.now();
-  node.params.meta.data.timestamp = now;
-  if (createTime) {
-    node.params.meta.data.duration = now - createTime;
-  }
+  node.params.meta.data.elapsedTimes = { endTime: Date.now() };
   updateMeta(alias, node.params.meta);
 }
 
 const consumers: Record<MetaType, (input: IImportMeta<any>) => void> = {
   upload: consumeUpload,
   "add.text": consumeAddText,
   "add.sketch.path": consumeAddSketchPath,
   "python.fields": consumePythonFields,
 };
-function consumeUpload({ t, lang, type, metaData }: IImportMeta<"upload">): void {
+function consumeUpload({ type, metaData }: IImportMeta<"upload">): void {
   const success = async () => {
-    toast(t, "success", translate(Toast_Words["upload-image-success-message"], lang));
-    updateTimestamps(newAlias);
+    toastWord("success", Toast_Words["upload-image-success-message"]);
+    updateElapsedTimes(newAlias);
   };
   const failed = async () => {
-    toast(t, "error", translate(Toast_Words["upload-image-error-message"], lang));
+    toastWord("error", Toast_Words["upload-image-error-message"]);
   };
   const { w, h, url, isDrag } = metaData;
   const prefix = isDrag ? "drag-" : "";
   const newAlias = `${prefix}upload.${getRandomHash()}`;
   metaData.alias = newAlias;
   const bboxInfo: NewImageInfo = { w, h };
   addNewImage(newAlias, url, {
     info: bboxInfo,
     meta: { type, data: metaData },
     callbacks: { success, failed },
     noSelect: false,
   });
 }
-function consumeAddText({ t, lang, type, metaData }: IImportMeta<"add.text">): void {
+function consumeAddText({ lang, type, metaData }: IImportMeta<"add.text">): void {
   const newAlias = `add.text.${getRandomHash()}`;
   const { textColor } = themeStore.styles;
 
   const success = async () => {
-    toast(t, "success", translate(Toast_Words["add-text-success-message"], lang));
-    updateTimestamps(newAlias);
+    toastWord("success", Toast_Words["add-text-success-message"]);
+    updateElapsedTimes(newAlias);
   };
   const failed = async () => {
-    toast(t, "error", translate(Toast_Words["add-text-error-message"], lang));
+    toastWord("error", Toast_Words["add-text-error-message"]);
   };
   const { addText } = useAddNode({ success, failed });
   metaData.alias = newAlias;
   addText({ trace: true })({
     alias: newAlias,
     initColor: textColor,
     lang,
     autoFit: true,
     meta: { type, data: metaData },
   });
 }
 function consumeAddSketchPath(): void {
   throw Error("Add sketch path by `importMeta` is not supported yet.");
 }
-function consumePythonFields({ t, lang, type, metaData }: IImportMeta<"python.fields">): void {
+function consumePythonFields({ type, metaData }: IImportMeta<"python.fields">): void {
   const success = async () => {
-    toast(t, "success", translate(Toast_Words["generate-image-success-message"], lang));
+    toastWord("success", Toast_Words["generate-image-success-message"]);
   };
   const failed = async (err: any) => {
-    toast(
-      t,
-      "error",
-      `${translate(Toast_Words["post-python-http-fields-plugin-error-message"], lang)} (${err})`,
-    );
+    toastWord("error", Toast_Words["post-python-http-fields-plugin-error-message"], {
+      appendix: ` (${err})`,
+    });
   };
   const getNewAlias = () => `${type}.${metaData.identifier}.${getRandomHash()}`;
   interface IPack<R> {
     data: R;
     alias: string;
     rectangle: RectangleShapeNode;
     metaData: IPythonFieldsMetaData;
@@ -100,15 +94,14 @@
     const packs: IPack<R>[] = [];
     responses.forEach((res, i) => {
       const newAlias = getNewAlias();
       const rectangle = getNewRectangle(`${i}.${getRandomHash()}`, getRectangleInfo(res));
       const iMetaData = shallowCopy(metaData);
       iMetaData.response.value = metaData.response.value[i] as any;
       iMetaData.alias = newAlias;
-      iMetaData.timestamp = Date.now();
       packs.push({ data: getData(res), alias: newAlias, rectangle, metaData: iMetaData });
     });
     return packs;
   }
   function getCallbacks(isLast: boolean) {
     return { success: isLast ? success : async () => void 0, failed };
   }
@@ -152,15 +145,11 @@
       });
     });
   }
 }
 
 // import api
 
-export function importMeta<T extends MetaType>({
-  t,
-  lang,
-  type,
-  metaData,
-}: Omit<IImportMeta<T>, "metaData"> & { metaData?: IMetaData[T] }): void {
-  consumers[type]({ t, lang, type, metaData });
+export function importMeta<T extends MetaType>({ lang, type, metaData }: IImportMeta<T>): void {
+  metaData.lang = lang;
+  consumers[type]({ lang, type, metaData });
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import { INodePack, Lang, Matrix2D, Matrix2DFields, safeCall } from "@carefree0910/core";
+import { INodePack, Matrix2D, Matrix2DFields, safeCall } from "@carefree0910/core";
 import {
   BoardStore,
   safeClearExecuterStack,
-  translate,
   useGlobalTransform,
   useSafeExecute,
 } from "@carefree0910/business";
 
-import type { IToast } from "@/schema/misc";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Requests } from "@/requests/actions";
 import {
   IProjectsStore,
   updateCurrentProject,
   updateCurrentProjectUpdateTime,
   useCurrentProject,
@@ -27,37 +25,33 @@
   const data = useCurrentProject();
   const graphInfo = BoardStore.graph.toJsonInfo();
   const globalTransform = useGlobalTransform().globalTransform.fields;
   return { ...data, graphInfo, globalTransform };
 }
 
 export async function saveProject(
-  t: IToast,
-  lang: Lang,
   onSuccess: () => Promise<void>,
   noToast?: boolean,
 ): Promise<void> {
   updateCurrentProjectUpdateTime();
   const fullProject = useCurrentFullProject();
   if (!noToast) {
-    toast(t, "info", translate(Toast_Words["uploading-project-message"], lang));
+    toastWord("info", Toast_Words["uploading-project-message"]);
   }
 
   return safeCall(
     async () => {
       const res = await Requests.postJson<{
         success: boolean;
         message: string;
       }>("_python", "/save_project", fullProject);
       if (!res.success) {
-        toast(
-          t,
-          "warning",
-          `${translate(Toast_Words["save-project-error-message"], lang)} - ${res.message}`,
-        );
+        toastWord("warning", Toast_Words["save-project-error-message"], {
+          appendix: ` - ${res.message}`,
+        });
         throw Error;
       }
     },
     {
       success: onSuccess,
       failed: async () => void 0,
     },
@@ -79,41 +73,37 @@
       updateCurrentProject(res);
       onSuccess(res);
     },
     failed: async () => void 0,
   })({ json: JSON.stringify(res.graphInfo), apiInfos: {}, noFit: true });
 }
 export async function loadProject(
-  t: IToast,
-  lang: Lang,
   uid: string,
   onSuccess: (res: ILoadedProject) => Promise<void>,
 ): Promise<void> {
-  toast(t, "info", translate(Toast_Words["loading-project-message"], lang));
+  toastWord("info", Toast_Words["loading-project-message"]);
 
   return safeCall(
     async () =>
       Requests.get<ILoadedProject>("_python", `/get_project/${uid}`).then((res) =>
         replaceProjectWith(res, onSuccess),
       ),
     {
       success: async () => void 0,
       failed: async () => void 0,
     },
   );
 }
 export function loadLocalProject(
-  t: IToast,
-  lang: Lang,
   res: ILoadedProject,
   onSuccess: (res: ILoadedProject) => Promise<void>,
   noToast?: boolean,
 ): void {
   if (!noToast) {
-    toast(t, "info", translate(Toast_Words["loading-project-message"], lang));
+    toastWord("info", Toast_Words["loading-project-message"]);
   }
   replaceProjectWith(res, onSuccess);
 }
 
 interface IProjectItem {
   uid: string;
   name: string;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-import { Lang, safeCall } from "@carefree0910/core";
-import { translate } from "@carefree0910/business";
+import { safeCall } from "@carefree0910/core";
 
-import type { IToast } from "@/schema/misc";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Requests } from "@/requests/actions";
 
 type UploadImageOptions = {
   failed: (e: any) => Promise<void>;
 };
 
 interface IUploadImageResponseData {
   w: number;
   h: number;
   url: string;
 }
 
 export async function uploadImage(
-  t: IToast,
-  lang: Lang,
   blob: Blob,
   { failed }: UploadImageOptions,
 ): Promise<IUploadImageResponseData | void> {
   return safeCall(
     async () => {
       const res = await Requests.postBlob<{
         success: boolean;
         message: string;
         data: IUploadImageResponseData;
       }>("_python", "/upload_image", { key: "image", blob });
       if (!res.success) {
-        toast(
-          t,
-          "warning",
-          `${translate(Toast_Words["upload-image-error-message"], lang)} - ${res.message}`,
-        );
+        toastWord("warning", Toast_Words["upload-image-error-message"], {
+          appendix: ` - ${res.message}`,
+        });
         throw Error;
       }
       return res.data;
     },
     {
       success: async () => void 0,
       failed,
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFButton.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFButton.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import { observer } from "mobx-react-lite";
-import { Button, ButtonProps, Tooltip } from "@chakra-ui/react";
+import { Button, ButtonProps } from "@chakra-ui/react";
 
 import { themeStore } from "@/stores/theme";
+import CFTooltip from "./CFTooltip";
 
 function CFButton(props: ButtonProps) {
   const { textColor } = themeStore.styles;
 
   return <Button color={textColor} flexShrink={0} {...props}></Button>;
 }
 interface ICFButtonWithBusyProps extends ButtonProps {
   busy: boolean;
   tooltip: string;
 }
 export function CFButtonWithBusyTooltip({ busy, tooltip, ...others }: ICFButtonWithBusyProps) {
   return (
-    <Tooltip label={busy ? tooltip : ""} hasArrow shouldWrapChildren>
+    <CFTooltip label={busy ? tooltip : undefined} hasArrow shouldWrapChildren>
       <CFButton w="100%" isDisabled={busy} {...others} />
-    </Tooltip>
+    </CFTooltip>
   );
 }
 
 export default observer(CFButton);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFCircularProgress.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFCircularProgress.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import Upload from "rc-upload";
 import React, { ReactNode } from "react";
 import { observer } from "mobx-react-lite";
-import { useToast } from "@chakra-ui/react";
 
-import { langStore, translate } from "@carefree0910/business";
+import { langStore } from "@carefree0910/business";
 
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { importMeta } from "@/actions/importMeta";
 import { uploadImage } from "@/actions/uploadImage";
 
 export interface CFImageUploaderProps {
   className?: string;
   children: ReactNode;
@@ -19,32 +18,33 @@
 
 const CFImageUploader: React.FC<CFImageUploaderProps> = ({
   className,
   children,
   onUpload,
   addToBoard = true,
 }) => {
-  const t = useToast();
-  const lang = langStore.tgt;
-
   return (
     <Upload
       className={className}
       accept=".png, .jpeg, .jpg, .webp"
       customRequest={async ({ file }) => {
         async function failed(e: any): Promise<void> {
-          toast(t, "error", `${translate(Toast_Words["upload-image-error-message"], lang)} - ${e}`);
+          toastWord("error", Toast_Words["upload-image-error-message"], { appendix: ` - ${e}` });
         }
-        toast(t, "info", translate(Toast_Words["uploading-image-message"], lang));
+        toastWord("info", Toast_Words["uploading-image-message"]);
         const blob = file as Blob;
-        const uploadRes = await uploadImage(t, lang, blob, { failed });
+        const uploadRes = await uploadImage(blob, { failed });
         if (!uploadRes) return;
         onUpload?.(uploadRes.url);
         if (!addToBoard) return;
-        importMeta({ t, lang, type: "upload", metaData: { ...uploadRes, isDrag: false } });
+        importMeta({
+          lang: langStore.tgt,
+          type: "upload",
+          metaData: { ...uploadRes, isDrag: false },
+        });
       }}>
       {children}
     </Upload>
   );
 };
 
 export default observer(CFImageUploader);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 import { useEffect } from "react";
-import { useToast } from "@chakra-ui/toast";
 
-import { FileDropper, FileDropperResponse, Lang } from "@carefree0910/core";
-import { translate, useIsReady } from "@carefree0910/business";
+import { FileDropper, FileDropperResponse } from "@carefree0910/core";
+import { langStore, useIsReady } from "@carefree0910/business";
 
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { BOARD_CONTAINER_ID } from "@/utils/constants";
 import { setDropping, hooksStore } from "@/stores/hooks";
 import { uploadImage } from "@/actions/uploadImage";
 import { importMeta } from "@/actions/importMeta";
 
-export function useFileDropper(lang: Lang): void {
+export function useFileDropper(): void {
   function onDrop(): void {
     setDropping(true);
     setTimeout(() => {
       if (hooksStore.dropping) {
-        toast(t, "info", translate(Toast_Words["dropping-message"], lang));
+        toastWord("info", Toast_Words["dropping-message"]);
       }
     }, dropPatience);
   }
 
   async function failed(): Promise<void> {
-    toast(t, "error", translate(Toast_Words["upload-image-error-message"], lang));
+    toastWord("error", Toast_Words["upload-image-error-message"]);
   }
 
   type UploadResponse = { success: boolean; reason: "none" | "unknown" | "type" | "upload" };
   async function onSuccessOne(res: FileDropperResponse): Promise<UploadResponse> {
     if (res.type !== "success" || !res.data) return { success: false, reason: "unknown" };
     const { type, source } = res.data;
     if (type !== "png" && type !== "jpeg") {
       return { success: false, reason: "type" };
     }
 
     const file = new File([source], `image.${type}`, { type });
-    const uploadRes = await uploadImage(t, lang, file, {
-      failed: async () => void 0,
-    });
+    const uploadRes = await uploadImage(file, { failed: async () => void 0 });
     if (!uploadRes) {
       return { success: false, reason: "upload" };
     }
     importMeta({
-      t,
-      lang,
+      lang: langStore.tgt,
       type: "upload",
       metaData: { ...uploadRes, isDrag: true },
     });
     return { success: true, reason: "none" };
   }
   async function onSuccess(resList: FileDropperResponse[]): Promise<void> {
     setDropping(false);
     if (resList.length === 0) return;
-    toast(t, "info", translate(Toast_Words["uploading-image-message"], lang));
+    toastWord("info", Toast_Words["uploading-image-message"]);
     const uploadResList = await Promise.all(resList.map((res) => onSuccessOne(res)));
     if (uploadResList.some((res) => res.reason === "type")) {
-      toast(t, "error", translate(Toast_Words["strange-image-error-message"], lang));
+      toastWord("error", Toast_Words["strange-image-error-message"]);
     }
     if (uploadResList.some((res) => res.reason === "upload")) {
       failed();
     }
   }
 
   async function onError(resList: FileDropperResponse[]): Promise<void> {
     setDropping(false);
     console.log("fileDropper.error", resList);
     failed();
     if (resList.length === 0) return;
     resList.forEach((res) => {
       if (res.reason) {
-        toast(t, "error", translate(res.reason, lang));
+        toastWord("error", res.reason);
       }
     });
   }
 
-  const t = useToast();
   const dropPatience = 500;
 
   useEffect(() => {
     const dropper = new FileDropper({
       onDrop,
       onSuccess,
       onError,
@@ -85,9 +80,9 @@
       listenTarget: document.getElementById(BOARD_CONTAINER_ID) as HTMLElement,
       bypassWHCheck: true,
     });
     dropper.init();
     return () => {
       dropper.destroy();
     };
-  }, [useIsReady(), lang]);
+  }, [useIsReady()]);
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePython.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import { useCallback } from "react";
 
+import type { ExportBlobOptions } from "@carefree0910/svg";
 import { BBox, INode, INodes, Logger } from "@carefree0910/core";
 
 import type { IMeta } from "@/schema/meta";
 import type {
   INodeData,
   IPythonSocketRequest,
   IUsePythonInfo,
@@ -11,17 +12,17 @@
   IPythonOnSocketMessage,
 } from "@/schema/_python";
 import { userStore } from "@/stores/user";
 import { debugStore } from "@/stores/debug";
 import { IPythonStore, updatePythonStore } from "@/stores/_python";
 import { useWebSocketHook } from "@/requests/hooks";
 import { uploadImage } from "@/actions/uploadImage";
-import { Exporter, IExportBlob } from "@/actions/export";
+import { Exporter } from "@/actions/export";
 
-type IGetNodeData = IExportBlob & { exportBox: BBox };
+type IGetNodeData = ExportBlobOptions & { exportBox: BBox };
 async function getNodeData(node: INode | null, opt: IGetNodeData): Promise<INodeData> {
   if (!node) return {};
   const { x, y } = node.position;
   const { w, h } = node.wh;
   const transform = node.transform.fields;
   const text = node.type === "text" ? node.params.content : undefined;
   let src: string | undefined = undefined;
@@ -30,15 +31,15 @@
   } else if (node.type === "path") {
     // should export the `PathNode` as an image based on the `exportBox`
     opt.exportOptions ??= {};
     opt.exportOptions.exportBox = opt.exportBox;
     src = await Exporter.exportBlob([node], opt)
       .then((blob) => {
         if (!blob) throw Error("export blob for `PathNode` failed");
-        return uploadImage(opt.t, opt.lang, blob, { failed: async () => void 0 });
+        return uploadImage(blob, { failed: async () => void 0 });
       })
       .then((res) => {
         if (!res) throw Error("upload image for `PathNode` failed");
         return res.url;
       });
   }
   const meta = (node.type === "group" ? undefined : node.params.meta) as IMeta | undefined;
@@ -51,77 +52,72 @@
 async function getPythonRequest({
   node,
   nodes,
   identifier,
   getExtraRequestData,
   opt,
 }: Omit<IUsePythonInfo, "isInvisible"> & {
-  opt: IExportBlob;
+  opt: ExportBlobOptions;
 }): Promise<Omit<IPythonSocketRequest, "hash">> {
   const exportBox = new INodes(nodes).bbox;
   const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
   const nodeData = await getNodeData(node, getNodeDataOpt);
   const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
   return {
     userId: userStore.userId,
     identifier,
     nodeData,
     nodeDataList,
     extraData: getExtraRequestData ? getExtraRequestData() : {},
   };
 }
 
-/**
- * this function will integrate a simple but useful retry mechanism, so we only need to
- * focus on the core logics in `onMessage` function.
- */
 export function useSocketPython<R>({
-  t,
-  lang,
   hash,
   node,
   nodes,
   identifier,
   isInvisible,
+  retryInterval,
   updateInterval,
   getExtraRequestData,
   onMessage,
   onSocketError,
 }: IUseSocketPython<R>) {
   const deps = [
-    t,
-    lang,
     hash,
     node?.alias,
     nodes.map((n) => n.alias).join("_"),
     identifier,
+    retryInterval,
     updateInterval,
     isInvisible,
     getExtraRequestData,
   ];
 
   const getMessage = useCallback(
     () =>
       getPythonRequest({
         node,
         nodes,
         identifier,
         getExtraRequestData,
-        opt: { t, lang },
+        opt: {},
       }).then((req) => ({ hash: hash!, ...req })),
     [deps],
   );
 
   const requestFn = useCallback(() => {
     useWebSocketHook({
       isInvisible,
       hash,
       getMessage,
       onMessage,
       onSocketError,
+      retryInterval,
       updateInterval,
     });
   }, [getMessage, onMessage, onSocketError]);
 
   requestFn();
 }
 
@@ -162,9 +158,15 @@
         }
         return debugStore.pollSync ? { newMessage: getMessage } : {};
       }
     },
     [],
   );
 
-  useWebSocketHook<IPythonStore>({ isInvisible: false, hash, getMessage, onMessage });
+  useWebSocketHook<IPythonStore>({
+    isInvisible: false,
+    hash,
+    getMessage,
+    onMessage,
+    isInternal: true,
+  });
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import { Lang } from "@carefree0910/core";
 import { langDescriptions, langStore, updateDictionary } from "@carefree0910/business";
 
 import { uiLangRecords } from "./ui";
 import { addLangRecords } from "./add";
 import { brushLangRecords } from "./brush";
 import { toastLangRecords } from "./toast";
+import { tooltipLangRecords } from "./tooltip";
 import { pluginsLangRecords } from "./plugins";
 import { downloadLangRecords } from "./download";
 import { projectsLangRecords } from "./projects";
 import { settingsLangRecords } from "./settings";
 import { nodeEditorLangRecords } from "./nodeEditor";
 
 const initLangDirs = [
   uiLangRecords,
   toastLangRecords,
+  tooltipLangRecords,
   pluginsLangRecords,
   settingsLangRecords,
   projectsLangRecords,
   addLangRecords,
   downloadLangRecords,
   nodeEditorLangRecords,
   brushLangRecords,
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/lang/ui.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/AddPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
-import { Flex, useToast } from "@chakra-ui/react";
+import { Flex } from "@chakra-ui/react";
 
 import { getRandomHash, identityMatrix2DFields } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Add_Words } from "@/lang/add";
 import { Toast_Words } from "@/lang/toast";
 import { importMeta } from "@/actions/importMeta";
 import { loadLocalProject, saveProject } from "@/actions/manageProjects";
 import { getNewProject } from "@/stores/projects";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import CFImageUploader from "@/components/CFImageUploader";
-import { drawboardPluginFactory } from "./utils/factory";
-import { floatingEvent } from "./components/Floating";
-import Render from "./components/Render";
-import { useClosePanel } from "./components/hooks";
+import { drawboardPluginFactory } from "../utils/factory";
+import { floatingEvent } from "../components/Floating";
+import Render from "../components/Render";
+import { useClosePanel } from "../components/hooks";
 
 const AddPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `add_${getRandomHash()}`, []);
-  const t = useToast();
   const lang = langStore.tgt;
 
   const closePanel = useClosePanel(id);
   const onNewProject = () => {
-    toast(t, "info", translate(Toast_Words["adding-project-message"], lang));
+    toastWord("info", Toast_Words["adding-project-message"]);
     saveProject(
-      t,
-      lang,
       async () =>
         loadLocalProject(
-          t,
-          lang,
           { graphInfo: [], globalTransform: identityMatrix2DFields, ...getNewProject() },
           async () => {
             floatingEvent.emit({ type: "newProject", data: {} });
-            toast(t, "success", translate(Toast_Words["add-project-success-message"], lang));
+            toastWord("success", Toast_Words["add-project-success-message"]);
             closePanel();
           },
           true,
         ),
       true,
     );
   };
@@ -61,15 +56,15 @@
             {translate(Add_Words["upload-image-button"], lang)}
           </CFButton>
         </CFImageUploader>
         <CFButton
           w="100%"
           mt="12px"
           onClick={() => {
-            importMeta({ t, lang, type: "add.text", metaData: {} });
+            importMeta({ lang, type: "add.text", metaData: {} });
             closePanel();
           }}>
           {translate(Add_Words["add-text-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
-import { useToast } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
-import { langStore } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
 import { onArrange } from "@/actions/arrange";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 const ArrangePlugin = ({ pluginInfo: { nodes }, ...props }: IPlugin) => {
   const id = useMemo(() => `arrange_${getRandomHash()}`, []);
-  const t = useToast();
-  const lang = langStore.tgt;
 
   return (
     <Render
       id={id}
-      onFloatingButtonClick={async () => onArrange(t, lang, { type: "multiple", nodes })}
+      onFloatingButtonClick={async () => onArrange({ type: "multiple", nodes })}
       {...props}
     />
   );
 };
 drawboardPluginFactory.register("arrange", true)(observer(ArrangePlugin));
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 import { useEffect, useMemo } from "react";
 import { observer } from "mobx-react-lite";
-import { useToast } from "@chakra-ui/react";
 import { runInAction } from "mobx";
 
-import { IPathOptions, Lang, getRandomHash } from "@carefree0910/core";
+import { IPathOptions, getRandomHash } from "@carefree0910/core";
 import {
   BoardStore,
   langStore,
   toolbarStore,
   translate,
   updateBrushOptions,
 } from "@carefree0910/business";
 
-import type { IToast } from "@/schema/misc";
 import type { ICommonMetaData, IMeta } from "@/schema/meta";
 import type { IPlugin } from "@/schema/plugins";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Brush_Words } from "@/lang/brush";
 import { Toast_Words } from "@/lang/toast";
-import { VisibleManager, uiStore } from "@/stores/ui";
 import { themeStore } from "@/stores/theme";
+import { VisibleManager, uiStore } from "@/stores/ui";
 import { hideAllPlugins } from "@/actions/managePlugins";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
 import CFButton from "@/components/CFButton";
 import CFSlider from "@/components/CFSlider";
 import CFSwitch from "@/components/CFSwitch";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
-import { floatingControlEvent } from "./components/Floating";
+import { drawboardPluginFactory } from "../utils/factory";
+import { floatingControlEvent } from "../components/Floating";
+import Render from "../components/Render";
 
-const useSwitchBrushMode = (t: IToast, lang: Lang) => async (): Promise<void> => {
+const useSwitchBrushMode = () => async (): Promise<void> => {
   const { defaultBrushStyles } = themeStore.styles;
   const previousInBrushMode = toolbarStore.inBrushMode;
   // handle drawboard
   if (!previousInBrushMode) {
-    toast(t, "success", translate(Toast_Words["enter-brush-mode-message"], lang));
+    toastWord("success", Toast_Words["enter-brush-mode-message"]);
     toolbarStore.switchBrushMode(defaultBrushStyles);
   } else {
     toolbarStore.switchBrushMode({
       nodeCallback: (node) => {
-        toast(t, "success", translate(Toast_Words["exit-brush-mode-message"], lang));
+        toastWord("success", Toast_Words["exit-brush-mode-message"]);
         node.active = true;
         node.params.meta = {
           type: "add.sketch.path",
-          data: { timestamp: Date.now() },
+          data: { elapsedTimes: { endTime: Date.now() } },
         } as IMeta<ICommonMetaData>;
       },
     });
   }
   // handle plugin visibilities
   runInAction(() => {
     const inBrushMode = !previousInBrushMode;
@@ -59,27 +57,21 @@
     } else {
       uiStore.disablePluginSettings = false;
       VisibleManager.restoreVisibleBackup();
     }
   });
 };
 
-function SingleBrushEditor({
-  lang,
-  pathIndex,
-  options,
-}: {
-  lang: Lang;
-  pathIndex: number;
-  options: IPathOptions;
-}) {
+function SingleBrushEditor({ pathIndex, options }: { pathIndex: number; options: IPathOptions }) {
   const brushManager = BoardStore.board.brushPluginNullable;
   if (!brushManager) {
     return null;
   }
+
+  const lang = langStore.tgt;
   const { fill, stroke, width, linecap } = options;
 
   const setOpt = (opt: Partial<IPathOptions>) => {
     updateBrushOptions({ fill, stroke, width, linecap, ...opt, index: pathIndex });
   };
 
   const setColor = (color: string) => setOpt({ stroke: color, fill: color });
@@ -105,33 +97,32 @@
       />
     </>
   );
 }
 
 const BrushPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `brush_${getRandomHash()}`, []);
-  const t = useToast();
   const lang = langStore.tgt;
   const options = toolbarStore.allBrushOptions;
   const inBrushMode = toolbarStore.inBrushMode;
-  const switchBrushMode = useSwitchBrushMode(t, lang);
+  const switchBrushMode = useSwitchBrushMode();
   const optionsList = !options ? [] : Array.isArray(options) ? options : [options];
 
   useEffect(() => {
     if (inBrushMode) {
       floatingControlEvent.emit({ id, expand: true });
     }
   });
 
   return (
     <Render id={id} onFloatingButtonClick={switchBrushMode} {...props}>
       <CFHeading>{translate(Brush_Words["brush-plugin-header"], lang)}</CFHeading>
       <CFDivider />
       {optionsList.map((opt, i) => (
-        <SingleBrushEditor key={`brush-${i}`} lang={lang} pathIndex={i} options={opt} />
+        <SingleBrushEditor key={`brush-${i}`} pathIndex={i} options={opt} />
       ))}
       <CFDivider my="16px" />
       <CFButton
         isDisabled={!inBrushMode}
         onClick={() => {
           floatingControlEvent.emit({ id, expand: false });
           switchBrushMode();
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
 import { useSafeExecute, useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 const DeletePlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `delete_${getRandomHash()}`, []);
   const { type, nodes } = useSelecting("raw");
   if (type === "none") return null;
   function onDelete(): void {
     useSafeExecute("remove", null, true)(nodes.map((node) => node.alias));
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import { useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
-import { Flex, Spacer, useToast } from "@chakra-ui/react";
+import { Flex, Spacer } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate, useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { DownloadFormat, allDownloadFormat } from "@/schema/misc";
 import { Download_Words } from "@/lang/download";
 import { themeStore } from "@/stores/theme";
 import { downloadNodes } from "@/actions/download";
 import CFSelect, { CFSrollableSelect } from "@/components/CFSelect";
 import CFText from "@/components/CFText";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
-import { useClosePanel } from "./components/hooks";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
+import { useClosePanel } from "../components/hooks";
 
 const DownloadPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `download_${getRandomHash()}`, []);
-  const t = useToast();
   const lang = langStore.tgt;
   const { type, nodes } = useSelecting("raw");
   const { w, h, imgWH } = useSelecting("basic")({ fixed: 0 }) ?? {};
   const { captionColor } = themeStore.styles;
   const [format, setFormat] = useState<DownloadFormat>("PNG");
   const [keepOriginal, setKeepOriginal] = useState(true);
   const sizeString = useMemo(() => {
@@ -43,15 +42,15 @@
       keepOriginal === "true"
         ? Download_Words["download-image-size-original"]
         : Download_Words["download-image-size-drawboard"],
       lang,
     );
   const closePanel = useClosePanel(id);
   const onDownload = () => {
-    downloadNodes(t, lang, nodes, format, keepOriginal);
+    downloadNodes(nodes, format, keepOriginal);
     closePanel();
   };
 
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         <Flex align="center">
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
 import { useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import Render from "./components/Render";
-import { drawboardPluginFactory } from "./utils/factory";
+import Render from "../components/Render";
+import { drawboardPluginFactory } from "../utils/factory";
 
 const GroupEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `groupEditor_${getRandomHash()}`, []);
   const { unGroup } = useSelecting("group") ?? {};
   return <Render id={id} onFloatingButtonClick={async () => unGroup?.()} {...props} />;
 };
 const MultiEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
 
 import type { IPlugin } from "@/schema/plugins";
-import { drawboardPluginFactory } from "./utils/factory";
-import { Link } from "./components/Link";
+import { drawboardPluginFactory } from "../utils/factory";
+import { Link } from "../components/Link";
 
 const WikiPlugin = (props: IPlugin) => {
   const id = useMemo(() => `wikiLink_${getRandomHash()}`, []);
   return <Link id={id} url="https://github.com/carefree0910/carefree-drawboard/wiki" {...props} />;
 };
 const EmailPlugin = (props: IPlugin) => {
   const id = useMemo(() => `emailLink_${getRandomHash()}`, []);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/MetaPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import { Textarea } from "@chakra-ui/react";
 
 import { useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { IMeta, getMetaTrace } from "@/schema/meta";
 import { getPluginIds } from "@/stores/plugins";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 function getMetaRepresentation(meta: IMeta): string {
   const { type, data } = meta;
   if (type.startsWith("python.")) {
     return data.identifier ?? "unknown";
   }
   return type;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import Upload from "rc-upload";
 import { observer } from "mobx-react-lite";
 import { useMemo, useState, useEffect, useCallback } from "react";
-import { Flex, useToast } from "@chakra-ui/react";
+import { Flex } from "@chakra-ui/react";
 
 import { Dictionary, Graph, INodePack, getRandomHash } from "@carefree0910/core";
 import { langStore, translate, useSafeExecute } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Projects_Words } from "@/lang/projects";
 import { setCurrentProjectName, useCurrentProject } from "@/stores/projects";
 import {
   ILoadedProject,
   fetchAllProjects,
   loadProject,
@@ -20,23 +20,22 @@
 import { downloadCurrentFullProject } from "@/actions/download";
 import CFText from "@/components/CFText";
 import CFInput from "@/components/CFInput";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { CFSrollableSelect } from "@/components/CFSelect";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
-import { floatingEvent, floatingRenderEvent } from "./components/Floating";
-import { useClosePanel } from "./components/hooks";
+import { drawboardPluginFactory } from "../utils/factory";
+import { floatingEvent, floatingRenderEvent } from "../components/Floating";
+import { useClosePanel } from "../components/hooks";
+import Render from "../components/Render";
 
 type IImportLocal = ILoadedProject | INodePack[];
 const ProjectPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `project_${getRandomHash()}`, []);
-  const t = useToast();
   const lang = langStore.tgt;
   const { uid, name } = useCurrentProject();
   const [selectedUid, setSelectedUid] = useState("");
   const [userInputName, setUserInputName] = useState(name);
   const [allProjects, setAllProjects] = useState<Dictionary<string> | undefined>();
   const allProjectUids = useMemo(() => Object.keys(allProjects ?? {}), [allProjects]);
 
@@ -81,51 +80,50 @@
 
   function onRenameProject() {
     setCurrentProjectName(userInputName);
     onSaveProject();
     closePanel();
   }
   function onSaveProject() {
-    saveProject(t, lang, async () => {
-      toast(t, "success", translate(Toast_Words["save-project-success-message"], lang));
+    saveProject(async () => {
+      toastWord("success", Toast_Words["save-project-success-message"]);
       updateUids();
       closePanel();
     });
   }
   async function onLoadProjectSuccess(res: ILoadedProject) {
     updateProjectStates(res.uid, res.name);
-    toast(t, "success", translate(Toast_Words["load-project-success-message"], lang));
+    toastWord("success", Toast_Words["load-project-success-message"]);
     closePanel();
   }
   function onLoadProject() {
     if (!selectedUid) {
-      toast(t, "warning", translate(Toast_Words["please-select-project-message"], lang));
+      toastWord("warning", Toast_Words["please-select-project-message"]);
       return;
     }
-    loadProject(t, lang, selectedUid, onLoadProjectSuccess);
+    loadProject(selectedUid, onLoadProjectSuccess);
   }
   function onDownloadProject(): void {
-    downloadCurrentFullProject(t, lang);
+    downloadCurrentFullProject();
     closePanel();
   }
   function onImportLocalProject(res: IImportLocal) {
-    toast(t, "info", translate(Toast_Words["importing-local-project-message"], lang));
+    toastWord("info", Toast_Words["importing-local-project-message"]);
     if ((res as ILoadedProject).uid) {
       res = (res as ILoadedProject).graphInfo;
     }
     const json = Graph.fromJsonInfo(res as INodePack[])
       .clone()
       .toJson();
     useSafeExecute("addGraph", null, true, {
       success: async () => {
-        toast(t, "success", translate(Toast_Words["import-local-project-success-message"], lang));
+        toastWord("success", Toast_Words["import-local-project-success-message"]);
         closePanel();
       },
-      failed: async () =>
-        toast(t, "error", translate(Toast_Words["import-local-project-error-message"], lang)),
+      failed: async () => toastWord("error", Toast_Words["import-local-project-error-message"]),
     })({ json });
   }
 
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         <CFHeading>{translate(Projects_Words["project-plugin-header"], lang)}</CFHeading>
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 } from "@/stores/pluginVisible";
 import { hideAllPlugins, showAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSelect from "@/components/CFSelect";
 import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 const SettingsPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `settings_${getRandomHash()}`, []);
   const lang = langStore.tgt;
   const commonProps = { fontWeight: 400, size: "md" };
   const disablePluginSettings = uiStore.disablePluginSettings;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import { observer } from "mobx-react-lite";
 import { Flex, Textarea } from "@chakra-ui/react";
 
 import { getRandomHash, isUndefined } from "@carefree0910/core";
 import { langStore, translate, useEditText } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import Render from "./components/Render";
-import { drawboardPluginFactory } from "./utils/factory";
+import { NodeEditor_Words } from "@/lang/nodeEditor";
 import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
-import { NodeEditor_Words } from "@/lang/nodeEditor";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 const TextEditorPlugin = ({ pluginInfo: { node }, ...props }: IPlugin) => {
   const id = useMemo(() => `textEditor_${getRandomHash()}`, []);
   const lang = langStore.tgt;
   const { nodeContent, nodeFontSize } = useMemo<{
     nodeContent?: string;
     nodeFontSize?: number;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
 import { safeRedo, safeUndo, useUndoRedoSteps } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { setPluginVisible } from "@/stores/pluginVisible";
-import { drawboardPluginFactory } from "./utils/factory";
-import Render from "./components/Render";
+import { drawboardPluginFactory } from "../utils/factory";
+import Render from "../components/Render";
 
 const UndoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `undo_${getRandomHash()}`, []);
   const { undoSteps } = useUndoRedoSteps();
   useEffect(() => setPluginVisible("undo", undoSteps > 0), [undoSteps]);
 
   return <Render id={id} onFloatingButtonClick={async () => safeUndo()} {...props} />;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
-import type { IDefinitions } from "@/schema/metaFields";
+import type { IDefinitions } from "@/schema/fields";
 import { useDefinitions } from "../components/Fields";
 
 interface IDefinitionFields {
   definitions: IDefinitions;
   numColumns?: number;
 }
 function DefinitionFields({ definitions, numColumns }: IDefinitionFields) {
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,104 @@
 import { useCallback } from "react";
 import { observer } from "mobx-react-lite";
 import { CloseIcon } from "@chakra-ui/icons";
-import { Flex, Spacer, useToast } from "@chakra-ui/react";
+import { Flex, Spacer } from "@chakra-ui/react";
 
+import { isUndefined } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IPythonResults } from "@/schema/meta";
 import type { IPythonFieldsPlugin, IPythonOnSocketMessage } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
 import { Toast_Words } from "@/lang/toast";
-import { toast } from "@/utils/toast";
+import { toastWord } from "@/utils/toast";
 import { titleCaseWord } from "@/utils/misc";
-import { removeSocketHook, socketLog } from "@/stores/socket";
+import { removeSocketHooks, socketLog } from "@/stores/socket";
 import { getPluginIds, removePluginMessage, updatePluginMessage } from "@/stores/plugins";
 import { importMeta } from "@/actions/importMeta";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import { useClosePanel } from "../components/hooks";
 import { useCurrentMeta, useDefinitionsRequestDataFn } from "./hooks";
 import PythonPluginWithSubmit, { socketFinishedEvent } from "./PluginWithSubmit";
 import DefinitionFields from "./DefinitionFields";
 
 const PythonFieldsPlugin = ({ pluginInfo, ...props }: IPythonFieldsPlugin) => {
   const { id, pureIdentifier } = getPluginIds(pluginInfo.identifier);
-  const t = useToast();
   const lang = langStore.tgt;
-  const definitions = pluginInfo.definitions;
+  const { definitions, retryInterval, noErrorToast } = pluginInfo;
   const getExtraRequestData = useDefinitionsRequestDataFn(definitions);
   const currentMeta = useCurrentMeta(pluginInfo.node);
   const emitClose = useClosePanel(id);
 
   const onMessage = useCallback<IPythonOnSocketMessage<IPythonResults>>(
     async (message) => {
       const {
         hash,
         status,
-        data: { final },
+        data: { final, elapsedTimes },
       } = message;
       switch (status) {
         case "pending": {
           updatePluginMessage(id, message);
           break;
         }
         case "working": {
           updatePluginMessage(id, message);
           break;
         }
         case "finished": {
           removePluginMessage(id);
           socketFinishedEvent.emit({ id });
           if (!final) {
-            toast(
-              t,
-              "success",
-              `${translate(Toast_Words["submit-task-finished-message"], lang)} (${pureIdentifier})`,
-            );
+            toastWord("success", Toast_Words["submit-task-finished-message"], {
+              appendix: ` (${pureIdentifier})`,
+            });
           } else {
-            const { _duration, ...response } = final;
             importMeta({
-              t,
               lang,
               type: "python.fields",
               metaData: {
                 identifier: pureIdentifier,
                 parameters: getExtraRequestData(),
-                response,
-                duration: _duration,
+                response: final,
+                elapsedTimes,
                 from: currentMeta,
               },
             });
           }
           socketLog(`> remove hook (${hash})`);
-          removeSocketHook(hash);
+          removeSocketHooks(hash);
+          break;
+        }
+        case "exception": {
+          if (!noErrorToast) {
+            toastWord("error", Toast_Words["submit-task-error-message"], {
+              appendix: ` - ${message.message}`,
+            });
+          }
+          // cleanup if retry is not specified
+          if (isUndefined(retryInterval)) {
+            socketFinishedEvent.emit({ id });
+            removePluginMessage(id);
+            socketLog(`> remove hook (${hash})`);
+            removeSocketHooks(hash);
+          }
           break;
         }
       }
       return {};
     },
-    [id, lang, pureIdentifier, currentMeta, getExtraRequestData],
+    [id, lang, pureIdentifier, currentMeta, retryInterval, noErrorToast, getExtraRequestData],
   );
   const onSocketError = useCallback(
     async (err: any) => {
-      toast(t, "error", `${translate(Toast_Words["submit-task-error-message"], lang)} - ${err}`);
+      toastWord("error", Toast_Words["submit-task-error-message"], { appendix: ` - ${err}` });
     },
-    [t, lang],
+    [lang],
   );
 
   const header = pluginInfo.header ?? titleCaseWord(pureIdentifier);
   return (
     <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import { useCallback, useEffect, useState } from "react";
 import { observer } from "mobx-react-lite";
-import { useToast } from "@chakra-ui/react";
 
-import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IPythonSocketPluginWithSubmit } from "@/schema/_python";
 import { Event } from "@/utils/event";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { userStore } from "@/stores/user";
@@ -20,53 +18,52 @@
 export const socketFinishedEvent = new Event<{ id: string }>();
 function PythonPluginWithSubmit<R>({
   id,
   pluginInfo: {
     node,
     nodes,
     identifier,
+    retryInterval,
     updateInterval,
     closeOnSubmit = true,
     toastOnSubmit = true,
     toastMessageOnSubmit,
   },
   buttonText,
   onMessage,
   onSocketError,
   getExtraRequestData,
   children,
   ...props
 }: IPythonSocketPluginWithSubmit<R>) {
-  const t = useToast();
   const lang = langStore.tgt;
   const [hash, setHash] = useState<string | undefined>(undefined);
   const [busy, setBusy] = useState(false);
   const onClick = useCallback(() => {
     if (busy) return;
     if (!userStore.canAlwaysSubmit) {
       setBusy(true);
     }
     setHash(getPluginHash(id));
     if (closeOnSubmit) {
       floatingControlEvent.emit({ id, expand: false });
     }
     if (toastOnSubmit) {
       toastMessageOnSubmit ??= translate(Toast_Words["submit-task-success-message"], lang);
-      toast(t, "info", toastMessageOnSubmit);
+      toast("info", toastMessageOnSubmit);
     }
-  }, [id, t, lang, closeOnSubmit, toastOnSubmit, toastMessageOnSubmit, busy]);
+  }, [id, lang, closeOnSubmit, toastOnSubmit, toastMessageOnSubmit, busy]);
 
   useSocketPython<R>({
-    t,
-    lang,
     hash,
     node,
     nodes,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
+    retryInterval,
     updateInterval,
     onMessage,
     onSocketError,
     getExtraRequestData,
   });
 
   useEffect(() => {
@@ -84,15 +81,15 @@
 
   return (
     <Render id={id} {...props}>
       {children}
       <CFDivider />
       <CFButtonWithBusyTooltip
         busy={busy}
-        tooltip={translate(Toast_Words["submit-task-busy-message"], lang)}
+        tooltip={Toast_Words["submit-task-busy-message"]}
         onClick={onClick}>
         {buttonText}
       </CFButtonWithBusyTooltip>
     </Render>
   );
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/QAPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,14 @@
       <Textarea w="100%" h="40%" minH="0px" value={serverText} readOnly />
       <CFInput
         w="100%"
         h="30%"
         mt="16px"
         value={userInput}
         onChange={(event) => setUserInput(event.target.value)}
-        placeholder={translate(UI_Words["qa-field-placeholder"], langStore.tgt)}
+        placeholder={translate(UI_Words["qa-field-placeholder"], lang)}
       />
     </PythonPluginWithSubmit>
   );
 };
 
 drawboardPluginFactory.registerPython("_python.QA", true)(observer(PythonQAPlugin));
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import { useCallback, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
-import { Textarea, useToast } from "@chakra-ui/react";
+import { Textarea } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
-import { langStore } from "@carefree0910/business";
 
 import type { IPythonTextAreaPlugin, IPythonOnSocketMessage } from "@/schema/_python";
 import { getPluginIds } from "@/stores/plugins";
 import { useSocketPython } from "@/hooks/usePython";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import Render from "@/plugins/components/Render";
 
 const PythonTextAreaPlugin = ({
-  pluginInfo: { node, nodes, identifier, updateInterval, noLoading, textAlign },
+  pluginInfo: { node, nodes, identifier, retryInterval, updateInterval, noLoading, textAlign },
   ...props
 }: IPythonTextAreaPlugin) => {
-  const t = useToast();
-  const lang = langStore.tgt;
   const id = getPluginIds(`textArea_${identifier}`);
   const hash = useMemo(() => getRandomHash().toString(), [id]);
   const [value, setValue] = useState("");
   const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
     async ({ status, data }) => {
       if (status === "finished") {
         setValue(data.final?.text ?? "");
@@ -29,21 +26,20 @@
       }
       return {};
     },
     [setValue],
   );
 
   useSocketPython({
-    t,
-    lang,
     hash,
     node,
     nodes,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
+    retryInterval,
     updateInterval,
     onMessage,
   });
 
   return (
     <Render id={id} {...props}>
       <Textarea w="100%" h="100%" minH="0px" value={value} textAlign={textAlign} readOnly />
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/_python/hooks.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/hooks.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { useCallback, useMemo } from "react";
 
 import { Dictionary, INode } from "@carefree0910/core";
 
 import type { IMeta } from "@/schema/meta";
-import type { IDefinitions } from "@/schema/metaFields";
+import type { IDefinitions } from "@/schema/fields";
 import { getMetaField } from "@/stores/meta";
 
 export function useDefinitionsRequestDataFn(definitions: IDefinitions): () => Dictionary<any> {
   return useCallback(() => {
     const data: Dictionary<any> = {};
     Object.keys(definitions).forEach((field) => {
       data[field] = getMetaField(field);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import { observer } from "mobx-react-lite";
 
 import { isUndefined } from "@carefree0910/core";
-import { langStore } from "@carefree0910/business";
 
 import type { IField } from "@/schema/plugins";
-import type { INumberField } from "@/schema/metaFields";
+import type { INumberField } from "@/schema/fields";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import CFSlider from "@/components/CFSlider";
 import TextField from "./TextField";
 import { getLabel } from "./utils";
 
 export interface NumberFieldProps extends IField<INumberField> {}
 function NumberField({ field, definition }: NumberFieldProps) {
   if (isUndefined(definition.min) || isUndefined(definition.max)) {
     return <TextField field={field} definition={{ type: "text", props: definition.props }} />;
   }
-  const lang = langStore.tgt;
   if (isUndefined(getMetaField(field))) setMetaField(field, definition.default);
   let step = definition.step;
   if (!isUndefined(step) && definition.isInt) step = Math.round(step);
   return (
     <CFSlider
       min={definition.min}
       max={definition.max}
       step={step}
       value={getMetaField(field) as number}
       onSliderChange={(value) => setMetaField(field, value)}
       scale={definition.scale}
-      label={definition.label ?? getLabel(field, lang)}
+      label={definition.label ?? getLabel(field)}
       precision={definition.isInt ? 0 : definition.precision}
       {...definition.props}
     />
   );
 }
 
 export default observer(NumberField);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { observer } from "mobx-react-lite";
 
 import type { IField } from "@/schema/plugins";
-import type { ISelectField } from "@/schema/metaFields";
+import type { ISelectField } from "@/schema/fields";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import { CFSrollableSelect } from "@/components/CFSelect";
 
 export interface SelectFieldProps extends IField<ISelectField<string>> {}
 function SelectField({ field, definition }: SelectFieldProps) {
   return (
     <CFSrollableSelect
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import { observer } from "mobx-react-lite";
 
-import { langStore } from "@carefree0910/business";
-
 import type { IField } from "@/schema/plugins";
-import type { ITextField } from "@/schema/metaFields";
+import type { ITextField } from "@/schema/fields";
 import { getMetaField, setMetaField } from "@/stores/meta";
 import CFInput from "@/components/CFInput";
 import { getPlaceholder } from "./utils";
 
 export interface TextFieldProps extends IField<ITextField> {}
 function TextField({ field, definition }: TextFieldProps) {
   return (
     <CFInput
       value={getMetaField(field) ?? ""}
       onChange={(event) => {
         setMetaField(field, event.target.value);
         definition.props?.onChange?.(event);
       }}
-      placeholder={definition.placeholder ?? getPlaceholder(field, langStore.tgt)}
+      placeholder={definition.placeholder ?? getPlaceholder(field)}
       {...definition.props}
     />
   );
 }
 
 export default observer(TextField);
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { isUndefined } from "@carefree0910/core";
 
-import type { IDefinitions } from "@/schema/metaFields";
+import type { IDefinitions } from "@/schema/fields";
 import TextField from "./TextField";
 import NumberField from "./NumberField";
 import SelectField from "./SelectField";
 
 export function useDefinitions(definitions: IDefinitions, numColumns?: number) {
   const nc = numColumns ?? 1;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import type { Lang } from "@carefree0910/core";
-import { translate } from "@carefree0910/business";
+import { langStore, translate } from "@carefree0910/business";
 
 import { UI_Words } from "@/lang/ui";
 import { titleCaseWord } from "@/utils/misc";
 
-export function getLabel(field: string, lang: Lang): string {
+export function getLabel(field: string): string {
   const labelWord = `${field}-field-label`;
-  return labelWord in UI_Words ? translate(labelWord, lang) : titleCaseWord(field);
+  return labelWord in UI_Words ? translate(labelWord, langStore.tgt) : titleCaseWord(field);
 }
-export function getPlaceholder(field: string, lang: Lang): string {
+export function getPlaceholder(field: string): string {
   const placeholderWord = `${field}-field-placeholder`;
-  return placeholderWord in UI_Words ? translate(placeholderWord, lang) : titleCaseWord(field);
+  return placeholderWord in UI_Words
+    ? translate(placeholderWord, langStore.tgt)
+    : titleCaseWord(field);
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 import type { IFloating, IExpandPositionInfo } from "@/schema/plugins";
 import { Event } from "@/utils/event";
 import { BG_TRANSITION, DEFAULT_PLUGIN_SETTINGS, VISIBILITY_TRANSITION } from "@/utils/constants";
 import { UI_Words } from "@/lang/ui";
 import { themeStore } from "@/stores/theme";
 import { getPluginMessage } from "@/stores/plugins";
+import { isInteractingWithBoard } from "@/stores/pointerEvents";
 import CFText from "@/components/CFText";
+import CFTooltip from "@/components/CFTooltip";
 import { CFPendingProgress, CFWorkingProgress } from "@/components/CFCircularProgress";
 
 export function getExpandId(id: string): string {
   return `${id}_expand`;
 }
 export function getExpandPosition(
   isModal: boolean,
@@ -130,15 +132,15 @@
       iconW,
       iconH,
       pivot,
       follow,
       expandOffsetX,
       expandOffsetY,
       src,
-      offsetX,
+      tooltip,
       offsetY,
       bgOpacity,
       renderFilter,
       useModal,
       modalOpacity,
       expandProps,
       isInvisible,
@@ -149,14 +151,15 @@
     ...props
   }: IFloating,
   ref,
 ) {
   const lang = langStore.tgt;
   const taskMessage = getPluginMessage(id);
   const needRender = useIsReady() && (!renderFilter || renderFilter(useSelecting("raw")));
+  const interactingWithBoard = isInteractingWithBoard();
   const [expand, setExpand] = useState(false);
   const [transform, setTransform] = useState<string | undefined>();
   const isBusy = useMemo(
     () => ["pending", "working"].includes(taskMessage?.status ?? ""),
     [taskMessage?.status],
   );
   const expandId = useMemo(() => getExpandId(id), [id]);
@@ -166,21 +169,22 @@
     panelBg,
     floatingColors: { busyColor },
   } = themeStore.styles;
   bgOpacity ??= DEFAULT_PLUGIN_SETTINGS.bgOpacity;
   const bgOpacityHex = Math.round(bgOpacity * 255).toString(16);
   const commonProps = useMemo<BoxProps>(
     () => ({
-      p: "12px",
+      p: "8px",
       bg: `${isBusy ? busyColor : panelBg}${bgOpacityHex}`,
       position: "absolute",
       // boxShadow: "2px 2px 4px rgba(0, 0, 0, 0.25)",
       borderRadius: "4px",
+      pointerEvents: interactingWithBoard ? "none" : "auto",
     }),
-    [panelBg, busyColor, bgOpacityHex, isBusy],
+    [panelBg, busyColor, bgOpacityHex, isBusy, interactingWithBoard],
   );
   const progressProps = useMemo<CircularProgressProps>(() => {
     const size = Math.floor(Math.min(iconW, iconH) * 0.8);
     return {
       size: `${size}px`,
       px: `${0.5 * (iconW - size)}px`,
       py: `${0.5 * (iconH - size)}px`,
@@ -279,80 +283,84 @@
     };
   }, [id, expand, needRender, noExpand]);
 
   if (!needRender) return null;
 
   return (
     <>
-      <Box
-        as="button"
-        id={id}
-        w={`${iconW}px`}
-        h={`${iconH}px`}
-        onClick={() => {
-          const self = document.querySelector<HTMLDivElement>(`#${id}`);
-          if (self && self.dataset.x && self.dataset.y) {
-            let x = parseFloat(self.dataset.x);
-            let y = parseFloat(self.dataset.y);
-            ({ x, y } = getExpandPosition(useModal ?? false, {
-              x,
-              y,
-              w,
-              h,
-              iconW,
-              iconH,
-              pivot,
-              follow,
-              expandOffsetX,
-              expandOffsetY,
-            }));
-            setTransform(`matrix(1,0,0,1,${x},${y})`);
-          }
-          if (!noExpand) {
-            setExpand(!expand);
-          }
-          onFloatingButtonClick?.();
-        }}
-        opacity={isInvisible ? 0 : 1}
-        visibility={isInvisible ? "hidden" : "visible"}
-        transition={`${VISIBILITY_TRANSITION}, ${BG_TRANSITION}`}
-        {...commonProps}
-        {...props}>
-        <Image
-          src={src}
-          draggable={false}
-          opacity={iconOpacity}
-          transition={VISIBILITY_TRANSITION}
-        />
-        {taskMessage && isBusy && (
-          <Box w={`${iconW}px`} h={`${iconH}px`} position="absolute" left="0px" top="0px">
-            {taskMessage.status === "pending" ? (
-              <CFPendingProgress
-                {...progressProps}
-                value={(1.0 - taskMessage.pending / Math.max(taskMessage.total, 1)) * 100}
-              />
-            ) : (
-              <CFWorkingProgress
-                {...progressProps}
-                value={(taskMessage.data.progress ?? 0.0) * 100}
-              />
-            )}
-          </Box>
-        )}
-        {taskMessage && isBusy && (
-          <CFText {...progressCaptionProps}>
-            {translate(
-              taskMessage.status === "pending"
-                ? UI_Words["task-pending-caption"]
-                : UI_Words["task-working-caption"],
-              lang,
-            )}
-          </CFText>
-        )}
-      </Box>
+      <CFTooltip label={tooltip} hasArrow>
+        <Box
+          as="button"
+          id={id}
+          w={`${iconW}px`}
+          h={`${iconH}px`}
+          onClick={() => {
+            const self = document.querySelector<HTMLDivElement>(`#${id}`);
+            if (self && self.dataset.x && self.dataset.y) {
+              let x = parseFloat(self.dataset.x);
+              let y = parseFloat(self.dataset.y);
+              ({ x, y } = getExpandPosition(useModal ?? false, {
+                x,
+                y,
+                w,
+                h,
+                iconW,
+                iconH,
+                pivot,
+                follow,
+                expandOffsetX,
+                expandOffsetY,
+              }));
+              setTransform(`matrix(1,0,0,1,${x},${y})`);
+            }
+            if (!noExpand) {
+              setExpand(!expand);
+            }
+            onFloatingButtonClick?.();
+          }}
+          opacity={isInvisible ? 0 : 1}
+          visibility={isInvisible ? "hidden" : "visible"}
+          transition={`${VISIBILITY_TRANSITION}, ${BG_TRANSITION}`}
+          {...commonProps}
+          {...props}>
+          <Image
+            src={src}
+            w="100%"
+            h="100%"
+            draggable={false}
+            opacity={iconOpacity}
+            transition={VISIBILITY_TRANSITION}
+          />
+          {taskMessage && isBusy && (
+            <Box w={`${iconW}px`} h={`${iconH}px`} position="absolute" left="0px" top="0px">
+              {taskMessage.status === "pending" ? (
+                <CFPendingProgress
+                  {...progressProps}
+                  value={(1.0 - taskMessage.pending / Math.max(taskMessage.total, 1)) * 100}
+                />
+              ) : (
+                <CFWorkingProgress
+                  {...progressProps}
+                  value={(taskMessage.data.progress ?? 0.0) * 100}
+                />
+              )}
+            </Box>
+          )}
+          {taskMessage && isBusy && (
+            <CFText {...progressCaptionProps}>
+              {translate(
+                taskMessage.status === "pending"
+                  ? UI_Words["task-pending-caption"]
+                  : UI_Words["task-working-caption"],
+                lang,
+              )}
+            </CFText>
+          )}
+        </Box>
+      </CFTooltip>
       {!noExpand && (
         <Portal containerRef={ref as any}>
           <Flex
             id={expandId}
             w={`${w}px`}
             h={`${h}px`}
             overflowY="auto"
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/hooks.ts`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 import type {
   IPythonOnSocketMessage,
   IPythonSocketRequest,
   IPythonSocketCallbacks,
 } from "@/schema/_python";
 import { pythonStore } from "@/stores/_python";
 import { useInceptors } from "./interceptors";
-import { getSocketHooks, pushSocketHook, runSocketHook, socketLog } from "@/stores/socket";
+import {
+  checkSocketHookExists,
+  getSocketHooks,
+  pushSocketHook,
+  runSocketHook,
+  socketLog,
+} from "@/stores/socket";
 
 // cannot use `useMemo` here
 export function useAPI<T extends APISources>(source: T): APIs[T] {
   const timeout = pythonStore.globalSettings?.timeout ?? 300000;
   let baseURL = import.meta.env.VITE_CFDRAW_API_URL;
   if (!baseURL) {
     let backendPort = import.meta.env.VITE_CFDRAW_BE_PORT;
@@ -27,60 +33,74 @@
   const apis = {
     _python: axios.create({ baseURL, timeout }),
   };
   useInceptors(apis);
   return apis[source];
 }
 
+/**
+ * this function will try to inject a simple but useful retry mechanism, so we only need to
+ * focus on the core logics in `onMessage` function.
+ */
 function useOnSocketMessageWithRetry<R>(
   getMessage: () => Promise<IPythonSocketRequest>,
   onMessage: IPythonOnSocketMessage<R>,
+  retryInterval?: number,
 ): IPythonOnSocketMessage<R> {
   return useCallback(
     (message) => {
-      if (message.status === "exception") {
-        Logger.warn(`socket exception occurred: ${message.message}`);
-        return Promise.resolve({ newMessage: getMessage });
-      }
-      return onMessage(message);
+      return onMessage(message).then((res) => {
+        let { newMessage, newMessageInterval } = res ?? {};
+        if (!isUndefined(retryInterval) && message.status === "exception") {
+          Logger.warn(
+            `socket exception occurred: ${message.message}, ` +
+              `will retry after ${retryInterval}ms`,
+          );
+          newMessage ??= getMessage;
+          newMessageInterval ??= retryInterval;
+        }
+        return { newMessage, newMessageInterval };
+      });
     },
-    [getMessage, onMessage],
+    [getMessage, onMessage, retryInterval],
   );
 }
 export function useWebSocketHook<R>({
   isInvisible,
   hash: _hash,
   getMessage,
   onMessage,
   onSocketError,
   dependencies,
-  useRetry = true,
+  retryInterval,
   updateInterval,
+  isInternal,
 }: IPythonSocketCallbacks<R> & {
   isInvisible: boolean;
   hash?: string;
   dependencies?: any[];
-  useRetry?: boolean;
-  updateInterval?: number;
+  isInternal?: boolean;
 }) {
   const hash = useMemo(() => (isInvisible ? undefined : _hash), [isInvisible, _hash]);
-  const onMessageWithRetry = useOnSocketMessageWithRetry(getMessage, onMessage);
-  const chosenOnMessage = useRetry ? onMessageWithRetry : onMessage;
+  const onMessageWithRetry = useOnSocketMessageWithRetry(getMessage, onMessage, retryInterval);
 
   useEffect(() => {
     if (isUndefined(hash)) return;
+    if (checkSocketHookExists(hash)) return;
     socketLog(`> add hook (${hash})`);
     pushSocketHook({
       key: hash,
       getMessage,
-      onMessage: chosenOnMessage,
+      onMessage: onMessageWithRetry,
       onSocketError,
       updateInterval,
+      isInternal,
+    }).then(() => {
+      socketLog(
+        `> current hooks: ${getSocketHooks()
+          .map((h) => h.key)
+          .join(", ")}`,
+      );
+      runSocketHook(hash);
     });
-    socketLog(
-      `> current hooks: ${getSocketHooks()
-        .map((h) => h.key)
-        .join(", ")}`,
-    );
-    runSocketHook(hash);
-  }, [hash, ...(dependencies ?? [])]);
+  }, [hash, onMessageWithRetry, onSocketError, isInternal, ...(dependencies ?? [])]);
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/_python.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import type { TextareaProps } from "@chakra-ui/react";
 
-import type { Dictionary, INode, Lang, Matrix2DFields } from "@carefree0910/core";
+import type { Dictionary, INode, Matrix2DFields } from "@carefree0910/core";
 
-import type { IMeta } from "./meta";
-import type { IToast } from "./misc";
+import type { IElapsedTimes, IMeta } from "./meta";
 import type { IPlugin, IPluginInfo } from "./plugins";
-import type { IDefinitions } from "./metaFields";
+import type { IDefinitions } from "./fields";
 
 // general
 
-interface IPythonPluginInfo extends IPluginInfo {
+interface IPythonPluginInfo extends IPluginInfo, IPythonSocketIntervals {
   identifier: string;
-  updateInterval?: number;
 }
 export interface IPythonPlugin extends IPlugin {
   pluginInfo: IPythonPluginInfo;
 }
 interface IPythonCallbacks {
   getExtraRequestData?: () => Dictionary<any>;
 }
@@ -49,14 +47,15 @@
 }
 export interface IPythonFieldsPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo &
     IPythonPluginWithSubmitPluginInfo & {
       header?: string;
       definitions: IDefinitions;
       numColumns?: number;
+      noErrorToast?: boolean;
     };
 }
 
 export interface IPythonTextAreaPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
     noLoading?: boolean;
     textAlign?: TextareaProps["textAlign"];
@@ -97,38 +96,43 @@
        * will be used, which means the message will be sent after 1000ms by default.
        * > if you want to send the new message immediately, you can set it to 0.
        */
       newMessageInterval?: number;
     }
   | undefined
 >;
-export interface IPythonSocketCallbacks<R> extends IPythonCallbacks {
+export interface IPythonSocketIntervals {
+  // if set, will retry in `retryInterval` ms when exception occurred
+  retryInterval?: number;
+  // if set, will re-send message every `updateInterval` ms
+  updateInterval?: number;
+}
+export interface IPythonSocketCallbacks<R> extends IPythonCallbacks, IPythonSocketIntervals {
   getMessage: () => Promise<IPythonSocketRequest>;
   onMessage: IPythonOnSocketMessage<R>;
   onSocketError?: (err: any) => void;
 }
 
 export type PythonSocketStatus = "pending" | "working" | "finished" | "exception";
 interface IPythonSocketIntermediate {
   imageList?: string[]; // intermediate images, if any
   textList?: string[]; // intermediate texts, if any
 }
 export interface IPythonSocketResponse<R> {
   progress?: number; // progress of current task, should be within [0, 1]
   intermediate?: IPythonSocketIntermediate;
   final?: R;
+  elapsedTimes?: IElapsedTimes;
 }
 export interface IPythonSocketMessage<R> {
   hash: string;
   status: PythonSocketStatus;
   total: number;
   pending: number;
   message: string;
   data: IPythonSocketResponse<R>;
 }
 export interface IUseSocketPython<R>
   extends IUsePythonInfo,
     Omit<IPythonSocketCallbacks<R>, "getMessage"> {
-  t: IToast;
-  lang: Lang;
   hash?: string;
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/meta.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import type { Dictionary, Lang } from "@carefree0910/core";
 
-import type { IToast } from "./misc";
+export interface IElapsedTimes {
+  createTime?: number;
+  startTime?: number;
+  endTime?: number;
+  duration?: number;
+}
 
 // general
 
 export const allMetaTypes = ["upload", "add.text", "add.sketch.path", "python.fields"] as const;
 export type MetaType = (typeof allMetaTypes)[number];
 export interface ICommonMetaData<T extends _IMetaData = _IMetaData> {
+  lang?: Lang;
   alias?: string;
-  timestamp?: number;
-  duration?: number;
+  elapsedTimes?: IElapsedTimes;
   from?: IMeta<T>;
 }
 type _IMetaData = ICommonMetaData & Dictionary<any>;
 export interface IMeta<T extends _IMetaData = _IMetaData> {
   type: MetaType;
   data: T;
 }
@@ -22,33 +27,31 @@
 
 interface IUploadMetaData extends ICommonMetaData {
   w: number;
   h: number;
   url: string;
   isDrag: boolean;
 }
-export type IPythonResults = { _duration?: number } & (
+export type IPythonResults =
   | { type: "text"; value: string[] }
-  | { type: "image"; value: { w: number; h: number; url: string }[] }
-);
+  | { type: "image"; value: { w: number; h: number; url: string }[] };
 export type IPythonFieldsMetaData = ICommonMetaData & {
   identifier: string;
   parameters: Dictionary<any>;
   response: IPythonResults;
 };
 
 export interface IMetaData {
   upload: IUploadMetaData;
   "add.text": ICommonMetaData;
   "add.sketch.path": ICommonMetaData;
   "python.fields": IPythonFieldsMetaData;
 }
 
 export interface IImportMeta<T extends MetaType> {
-  t: IToast;
   lang: Lang;
   type: T;
   metaData: IMetaData[T];
 }
 
 // utils
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/fields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/plugins.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import type { RefObject } from "react";
 import type { FlexProps } from "@chakra-ui/react";
 
 import type { INode, NodeType, PivotType } from "@carefree0910/core";
 import type { IResponse } from "@carefree0910/business";
 
-import type { IFieldDefinition, _IFieldDefinition } from "./metaFields";
+import type { IFieldDefinition, _IFieldDefinition } from "./fields";
 import type { IPythonFieldsPlugin, IPythonQAPlugin, IPythonTextAreaPlugin } from "./_python";
 
 // general
 
 export type NodeConstraints = NodeType | "none" | "anyNode" | "singleNode" | "multiNode";
 export interface IExpandPositionInfo {
   w: number;
@@ -18,14 +18,15 @@
   pivot: PivotType;
   follow: boolean;
   expandOffsetX: number;
   expandOffsetY: number;
 }
 export interface IRenderInfo extends IExpandPositionInfo {
   src?: string;
+  tooltip?: string;
   offsetX?: number;
   offsetY?: number;
   bgOpacity?: number;
   renderFilter?: (info?: IResponse) => boolean;
   useModal?: boolean;
   modalOpacity?: number;
   expandProps?: FlexProps;
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/debug.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/debug.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/pluginVisible.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pluginVisible.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/plugins.ts`

 * *Files 13% similar despite different names*

```diff
@@ -61,18 +61,26 @@
     const hashes = shallowCopy(pluginsStore.hashes);
     hashes[id] = getRandomHash().toString();
     pluginsStore.updateProperty("hashes", hashes);
   }
   return pluginsStore.hashes[id];
 };
 // messages
-export const getPluginMessage = (id: string) => pluginsStore.messages[id];
+export const getPluginMessage = (id: string): IPluginsStore["messages"][string] | undefined =>
+  pluginsStore.messages[id];
 export const updatePluginMessage = (id: string, message: IPythonSocketMessage<IPythonResults>) => {
   const messages = shallowCopy(pluginsStore.messages);
   messages[id] = message;
   pluginsStore.updateProperty("messages", messages);
 };
 export const removePluginMessage = (id: string) => {
   const messages = shallowCopy(pluginsStore.messages);
   delete messages[id];
   pluginsStore.updateProperty("messages", messages);
 };
+export const removePluginMessageFromHash = (hash: string) => {
+  const id = Object.keys(pluginsStore.messages).find((id) => pluginsStore.hashes[id] === hash);
+  if (!id) return;
+  const messages = shallowCopy(pluginsStore.messages);
+  delete messages[id];
+  pluginsStore.updateProperty("messages", messages);
+};
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/socket.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/socket.ts`

 * *Files 12% similar despite different names*

```diff
@@ -7,39 +7,44 @@
 import type {
   IPythonSocketRequest,
   IPythonSocketMessage,
   IPythonOnSocketMessage,
 } from "@/schema/_python";
 import { pythonStore } from "@/stores/_python";
 import { useAPI } from "@/requests/hooks";
+import { removePluginMessageFromHash } from "./plugins";
 
 const DEBUG = false;
 
 interface SocketHook<R> {
   key: string;
   getMessage: () => Promise<IPythonSocketRequest>;
   onMessage: IPythonOnSocketMessage<R>;
   onSocketError?: (err: any) => void;
   updateInterval?: number;
   timer?: any;
   shouldTerminate?: boolean;
+  isInternal?: boolean;
 }
 
 export interface ISocketStore {
   socket?: WebSocket;
+  shouldTerminate: boolean;
   hooks: Bundle<SocketHook<any>>;
 }
 class SocketStore extends ABCStore<ISocketStore> implements ISocketStore {
   socket?: WebSocket;
+  shouldTerminate: boolean = false;
   hooks = new Bundle<SocketHook<any>>([]);
 
   constructor() {
     super();
     makeObservable(this, {
       socket: observable,
+      shouldTerminate: observable,
       hooks: observable,
     });
   }
 
   get info(): ISocketStore {
     return this;
   }
@@ -56,14 +61,18 @@
 
       const send = () => {
         hook.getMessage().then((data) => {
           if (data.hash !== hash) {
             Logger.warn("Internal error: hash mismatched.");
             return;
           }
+          if (this.shouldTerminate) {
+            Logger.warn("Should terminate socket connection in `send`.");
+            return;
+          }
           socketStore.socket!.send(JSON.stringify(data));
           socketLog(`>>> message sent (${hash})`);
           if (hook.updateInterval && !hook.shouldTerminate) {
             hook.timer = setTimeout(send, hook.updateInterval);
           }
         });
       };
@@ -75,29 +84,35 @@
 }
 
 const socketStore = new SocketStore();
 export const socketLog = (...args: any[]) => DEBUG && console.log(...args);
 export const getSocketHooks = () => socketStore.hooks;
 export const runSocketHook = (key: string) => socketStore.run(key);
 export const pushSocketHook = <R>(hook: SocketHook<R>) => {
-  waitUntil(() => !!socketStore.socket).then(() => {
+  return waitUntil(() => !!socketStore.socket).then(() => {
     // need to wait until socket is ready, to avoid hooks being pushed too early that
     // `runSocketHook` will be executed twice (one at `onopen`, other at `useWebSocketHook`)
     const hooks = socketStore.hooks.clone();
     hooks.push(hook);
     socketStore.updateProperty("hooks", hooks);
   });
 };
-export const removeSocketHook = (hash: string) => {
-  const hooks = socketStore.hooks.clone();
-  const hook = hooks.remove(hash);
-  hook.shouldTerminate = true;
-  clearTimeout(hook.timer);
+export const removeSocketHooks = (...hashes: string[]) => {
+  const hooks = socketStore.hooks;
+  hashes.forEach((hash) => {
+    const hook = hooks.remove(hash);
+    hook.shouldTerminate = true;
+    clearTimeout(hook.timer);
+    removePluginMessageFromHash(hash);
+  });
   socketStore.updateProperty("hooks", hooks);
 };
+export const checkSocketHookExists = (key: string) => {
+  return socketStore.hooks.has(key);
+};
 
 const log = socketLog;
 interface IUseWebSocket {
   interval?: number;
 }
 export function useWebSocket(opt?: IUseWebSocket) {
   const interval = opt?.interval ?? 1000;
@@ -113,15 +128,14 @@
         log("> onopen");
         connected = true;
         if (shouldTerminate) {
           log(">> shouldTerminate");
           socket.close();
           return;
         }
-        socketStore.updateProperty("socket", socket);
         socket.onmessage = ({ data }) => {
           const alive = () => connected && !shouldTerminate;
           if (!alive()) {
             log(">> not alive");
             socket.close();
             return;
           }
@@ -148,26 +162,33 @@
                     });
                   }
                 }, newMessageInterval ?? interval);
               }
             });
           });
         };
-        // run existing hooks
+        // run existing hooks, mainly for hot reload
         socketStore.hooks.forEach(({ key }) => runSocketHook(key));
+        // tell the plugin that socket is ready
+        socketStore.updateProperty("socket", socket);
       };
       socket.onclose = (e) => {
         connected = false;
         log("> on close");
         if (shouldTerminate) {
           log(">> shouldTerminate");
           Logger.log("Socket connection terminated.");
           return;
         }
-        Logger.warn(`Socket connection closed (reason: ${e.reason}), retrying...`);
+        Logger.warn(
+          `Socket connection closed (reason: ${e.reason}), ` +
+            "cleaning up external hooks and retrying...",
+        );
+        const externalHooks = socketStore.hooks.filter((h) => !h.isInternal);
+        removeSocketHooks(...externalHooks.map((h) => h.key));
         timer = setTimeout(_connect, interval);
       };
       socket.onerror = (err) => {
         log("> on error");
         socketStore.hooks.forEach((hook) => hook.onSocketError?.(err));
         console.error("Socket error: ", err, ", retrying...");
         socket.close();
@@ -175,18 +196,20 @@
     }
 
     let timer: any;
     let newTimer: any;
     let socket: WebSocket;
     let connected = false;
     let shouldTerminate = false;
+    socketStore.updateProperty("shouldTerminate", false);
     _connect();
 
     return () => {
       log("cleanup...");
       shouldTerminate = true;
+      socketStore.updateProperty("shouldTerminate", true);
       clearTimeout(timer);
       clearTimeout(newTimer);
       if (connected) socket?.close();
     };
   }, []);
 }
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/theme.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import { computed, makeObservable, observable } from "mobx";
 
 import type { IPathOptions } from "@carefree0910/core";
 import { ABCStore } from "@carefree0910/business";
 
-type ThemeType = "light" | "dark";
-type ThemeStyles = {
+export type ThemeType = "light" | "dark";
+export type ThemeStyles = {
   // bg color of the infinite drawboard
   boardBg: string;
   // bg color of various panels (button, floating, expand, etc.)
   panelBg: string;
   // color of the text
   textColor: string;
   // color of the caption
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/stores/user.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/user.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/constants.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/constants.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.0a9/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.0a9/cfdraw/.web/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -213,41 +213,41 @@
   resolved "https://registry.yarnpkg.com/@babel/types/-/types-7.21.4.tgz#2d5d6bb7908699b3b416409ffd3b5daa25b030d4"
   integrity sha512-rU2oY501qDxE8Pyo7i/Orqma4ziCOrby0/9mvbDUGEfvZjb279Nk9k19e2fiCxHbRRpY2ZyrgW1eq22mvmOIzA==
   dependencies:
     "@babel/helper-string-parser" "^7.19.4"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@^0.4.10-alpha.2":
-  version "0.4.10-alpha.2"
-  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.4.10-alpha.2.tgz#b937f4e1a7c51ba44944dfaac375b3611f0caaae"
-  integrity sha512-tFNFwAtsEAYGOIAJuaBPcmohIlIimzeQp4LpRDhXeDctcEtoenrcfsd6r9Cdcd0Zd1LekjVj/y9CEpfQaBoXeA==
+"@carefree0910/business@~0.4.10-alpha.4":
+  version "0.4.10-alpha.4"
+  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.4.10-alpha.4.tgz#0f042da795388edbbab4de82b1d4e71c38e65594"
+  integrity sha512-B5plfUzIyuwB7N5w0jDpscZURsIgLPJgHsIyocBJcM7LPGMKrlmI8a6Em9Rel3gzjVGUu8TDLAtVkGuXy8uZEg==
   dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.1"
-    "@carefree0910/svg" "^0.4.10-alpha.1"
+    "@carefree0910/core" "~0.4.10-alpha.1"
+    "@carefree0910/svg" "~0.4.10-alpha.3"
 
-"@carefree0910/core@^0.4.10-alpha.1":
+"@carefree0910/core@~0.4.10-alpha.1":
   version "0.4.10-alpha.1"
   resolved "https://registry.yarnpkg.com/@carefree0910/core/-/core-0.4.10-alpha.1.tgz#8a1c579b7073a2119c8f30dae93bc1d1a21a3dbd"
   integrity sha512-bjKvuFAHawgNW/avS/vOh/J70MCw/Lu+04cQvlVmqzYxlOGAZPKsRFNtYgTO2CNo6vgRt3sa+WpnBXibWssw2Q==
 
-"@carefree0910/native@^0.4.10-alpha.2":
-  version "0.4.10-alpha.2"
-  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.4.10-alpha.2.tgz#0a1224046dcbc8ac5864721843a61aa1643a37c0"
-  integrity sha512-NsuHU2gff2PRK0NLVUU/4sfPT87K8gHuXAYaN1L01upOcIlzu6RgwsCoKKphh1uZtl9TYYt0VxjOAVxrONHvyg==
+"@carefree0910/native@~0.4.10-alpha.4":
+  version "0.4.10-alpha.4"
+  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.4.10-alpha.4.tgz#b9eedf92119b072e90ff0244d1b5f4f4da71967f"
+  integrity sha512-feNfSuqVRt/inXpTK+WDTxKoCuDXiG3YQ9kFBH3YDw/uX1tn5HRWZGQpkfMiXBTNdi4rqk62zWR3IuXSAjKTfg==
   dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.1"
-    "@carefree0910/svg" "^0.4.10-alpha.1"
+    "@carefree0910/core" "~0.4.10-alpha.1"
+    "@carefree0910/svg" "~0.4.10-alpha.3"
 
-"@carefree0910/svg@^0.4.10-alpha.1":
-  version "0.4.10-alpha.1"
-  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.4.10-alpha.1.tgz#b74bad3868c50033e691659e85deeeaa30ff9a32"
-  integrity sha512-r2BweoT2kiW5IOsack9c/W3EMwUnB6K6cIn1LgUm8gjMrRxc0OB0OmtIL4IHOyUjbDsFCQGP9WrsG7EqJ8mwJA==
+"@carefree0910/svg@~0.4.10-alpha.3":
+  version "0.4.10-alpha.3"
+  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.4.10-alpha.3.tgz#790a90eda3b9e4a30d96183450d1d1314ca53f68"
+  integrity sha512-QdeK8DQTPAp6JPb1xac0gMGEWN22H0boNSw76HlTmJ9x/ZdpRMNj24+nv5wKF+MOPu/xfNc+CKupBD76jWa6FQ==
   dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.1"
+    "@carefree0910/core" "~0.4.10-alpha.1"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.yarnpkg.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/assets.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/queue.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 import asyncio
 
-from typing import Any
 from typing import Dict
 from typing import Tuple
 from typing import Optional
 from cftool.misc import print_error
 from cftool.misc import random_hash
 from cftool.misc import print_warning
 
+from cfdraw.app.schema import IRequestQueue
+from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
 from cfdraw.utils.server import get_err_msg
 from cfdraw.utils.data_structures import Item
 from cfdraw.utils.data_structures import QueuesInQueue
+from cfdraw.schema.plugins import ISend
 from cfdraw.schema.plugins import SocketStatus
 from cfdraw.schema.plugins import ISocketMessage
-from cfdraw.app.schema import ISend
-from cfdraw.app.schema import IRequestQueue
-from cfdraw.app.schema import IRequestQueueData
 
 
 DEBUG = False
-log: Any = print if DEBUG else lambda *args, **kwargs: None
 
 
 class RequestQueue(IRequestQueue):
     def __init__(self) -> None:
         self._queues = QueuesInQueue[IRequestQueueData]()
         self._senders: Dict[str, Tuple[str, ISend]] = {}
         self._busy_uid: Optional[str] = None
 
     def push(self, data: IRequestQueueData, send_message: ISend) -> str:
         uid = random_hash()
         self._queues.push(data.request.userId, Item(uid, data))
-        hash = data.request.hash
-        self._senders[uid] = hash, send_message
-        log("~" * 50)
-        log("> push.uid", uid)
-        log("> push.userId", data.request.userId)
-        log("> push.hash", hash)
+        self._senders[uid] = data.request.hash, send_message
+        if DEBUG:
+            print("~" * 50)
+            print("> push.uid", uid)
+            print("> push.userId", data.request.userId)
+            print("> push.hash", data.request.hash)
         return uid
 
     async def run(self) -> None:
         if self._busy_uid is not None:
             return
         while True:
             user_id, request_item = self._queues.next()
             if user_id is None or request_item is None:
                 self._busy_uid = None
                 break
             uid = request_item.key
             plugin = request_item.data.plugin
             request = request_item.data.request
             self._busy_uid = uid
-            log(">>> run", uid)
+            if DEBUG:
+                print(">>> run", uid)
             try:
-                await self._broadcast_working(uid)
-                await offload(plugin(request))
+                plugin.elapsed_times.start()
+                if await self._broadcast_working(uid):
+                    await offload(plugin(request))
             except Exception as err:
                 await self._broadcast_exception(uid, get_err_msg(err))
             # cleanup
             request_item.data.event.set()
             self._queues.remove(user_id, uid)
             self._senders.pop(uid, None)
             await self._broadcast_pending()
             await asyncio.sleep(0)
-            log(">>> cleanup", uid)
+            if DEBUG:
+                print(">>> cleanup", uid)
 
     async def wait(self, user_id: str, uid: str) -> None:
         # Maybe in some rare cases, the task completes so fast that
         # the corresponding data has already been removed.
         # So here we simply warn instead of raise.
         queue_item = self._queues.get(user_id)
         if queue_item is None:
@@ -77,93 +78,109 @@
         request_item = queue_item.data.get(uid)
         if request_item is None:
             print_warning("cannot find request item after submitted")
             return
         await self._broadcast_pending()
         asyncio.create_task(self.run())
         await request_item.data.event.wait()
-        log("=" * 50)
-        log("> finished", uid)
-        log("^" * 50)
+        if DEBUG:
+            print("=" * 50)
+            print("> finished", uid)
+            print("^" * 50)
 
     # broadcast
 
     async def _broadcast_pending(self) -> None:
         for uid, (hash, sender) in self._senders.items():
             if uid == self._busy_uid:
                 continue
             pending = self._queues.get_pending(uid)
-            log("-" * 50)
-            log(">> uid", uid)
-            log(">> hash", hash)
-            log(
-                ">> queues\n\n",
-                "\n".join(
-                    [
-                        f"{queue_item.key} : "
-                        + ", ".join(
-                            [
-                                getattr(item.data.request, "hash", "None")
-                                for item in queue_item.data
-                            ]
-                        )
-                        for queue_item in self._queues
-                    ]
-                ),
-                "\n",
-            )
+            if DEBUG:
+                print("-" * 50)
+                print(">> uid", uid)
+                print(">> hash", hash)
+                print(
+                    ">> queues\n\n",
+                    "\n".join(
+                        [
+                            f"{queue_item.key} : "
+                            + ", ".join(
+                                [
+                                    getattr(item.data.request, "hash", "None")
+                                    for item in queue_item.data
+                                ]
+                            )
+                            for queue_item in self._queues
+                        ]
+                    ),
+                    "\n",
+                )
+            prefix = f"[broadcase_pending] [{hash}]"
+            success = True
+            message = "null"
             try:
                 if pending is None:
-                    await sender(
-                        ISocketMessage.make_exception(
-                            hash,
-                            message=(
-                                f"Internal error occurred: "
-                                f"cannot find pending request after submitted"
-                            ),
-                        )
+                    message = (
+                        f"{prefix} Internal error occurred: "
+                        "cannot find pending request after submitted"
                     )
+                    success = await sender(ISocketMessage.make_exception(hash, message))
                 elif len(pending) > 0:
-                    await sender(
+                    message = prefix
+                    success = await sender(
                         ISocketMessage(
                             hash=hash,
                             status=SocketStatus.PENDING,
                             total=self._queues.num_items,
                             pending=len(pending),
-                            message=f"in queue: {', '.join([str(item.data) for item in pending])}",
+                            message=message,
                         )
                     )
             except Exception as err:
-                print_error(get_err_msg(err))
+                print_error(f"{prefix} {get_err_msg(err)}")
+            if not success:
+                print_error(f"Failed to send following message: {message}")
 
-    async def _broadcast_working(self, uid: str) -> None:
+    async def _broadcast_working(self, uid: str) -> bool:
         sender_pack = self._senders.get(uid)
         if sender_pack is None:
-            return
+            return False
         hash, sender = sender_pack
+        prefix = f"[broadcase_working] [{hash}]"
+        success = True
         try:
-            await sender(
+            message = f"{prefix} working..."
+            success = await sender(
                 ISocketMessage(
                     hash=hash,
                     status=SocketStatus.WORKING,
                     total=0,
                     pending=0,
-                    message="",
+                    message=message,
                 )
             )
         except Exception as err:
-            print_error(get_err_msg(err))
+            print_error(f"{prefix} {get_err_msg(err)}")
+        if not success:
+            print_error(f"Failed to send following message: {message}")
+        return success
 
-    async def _broadcast_exception(self, uid: str, message: str) -> None:
+    async def _broadcast_exception(self, uid: str, message: str) -> bool:
         sender_pack = self._senders.get(uid)
         if sender_pack is None:
-            return
+            return False
         hash, sender = sender_pack
+        prefix = f"[broadcase_exception] [{hash}]"
+        success = True
         try:
-            await sender(ISocketMessage.make_exception(hash, message))
+            message = f"{prefix} {message}"
+            success = await sender(ISocketMessage.make_exception(hash, message))
         except Exception as err:
-            print_error(get_err_msg(err))
+            print_error(f"{prefix} {get_err_msg(err)}")
+        if not success:
+            print_error(f"Failed to send following message: {message}")
+        return success
 
 
 __all__ = [
     "RequestQueue",
 ]
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/upload.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/websocket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import json
 import asyncio
 import logging
 
-from asyncio import Event
 from fastapi import WebSocket
 from fastapi import WebSocketDisconnect
+from cftool.misc import print_error
+from starlette.websockets import WebSocketState
 
 from cfdraw import constants
 from cfdraw.app.schema import IApp
 from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
 from cfdraw.utils.server import get_err_msg
+from cfdraw.schema.plugins import ElapsedTimes
 from cfdraw.schema.plugins import ISocketRequest
 from cfdraw.schema.plugins import ISocketMessage
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 def add_websocket(app: IApp) -> None:
     @app.api.websocket(str(constants.Endpoint.WEBSOCKET))
@@ -26,16 +28,19 @@
                     ISocketMessage.make_exception(
                         hash,
                         message=f"Invalid data: {get_err_msg(e)}",
                     ).dict()
                 )
             )
 
-        async def send_message(data: ISocketMessage) -> None:
+        async def send_message(data: ISocketMessage) -> bool:
+            if websocket.client_state == WebSocketState.DISCONNECTED:
+                return False
             await websocket.send_text(json.dumps(data.dict()))
+            return True
 
         await websocket.accept()
         while True:
             try:
                 target_plugin = None
                 raw_data = await websocket.receive_text()
                 data = ISocketRequest(**json.loads(raw_data))
@@ -46,31 +51,31 @@
                     identifier = data.identifier.split(".", 1)[0]  # remove hash
                     target_plugin = app.plugins.make(identifier)
                 if target_plugin is not None:
                     # `send_message` should be handled by the plugin itself, or by
                     # the `SendSocketMessageMiddleWare` which will provide a default handling
                     target_plugin.task_hash = data.hash
                     target_plugin.send_message = send_message
+                    target_plugin.elapsed_times = ElapsedTimes()
                     if data.isInternal:
+                        target_plugin.elapsed_times.start()
                         await offload(target_plugin(data))
                     else:
-                        queue_data = IRequestQueueData(data, target_plugin, Event())
+                        queue_data = IRequestQueueData(data, target_plugin)
                         uid = app.request_queue.push(queue_data, send_message)
                         asyncio.create_task(app.request_queue.wait(data.userId, uid))
                 else:
                     plugin_str = "internal plugin" if data.isInternal else "plugin"
-                    await send_message(
-                        ISocketMessage.make_exception(
-                            data.hash,
-                            (
-                                f"incoming message subscribed {plugin_str} '{identifier}', "
-                                "but it is not found"
-                            ),
-                        )
+                    message = (
+                        f"incoming message subscribed {plugin_str} '{identifier}', "
+                        "but it is not found"
                     )
+                    exception = ISocketMessage.make_exception(data.hash, message)
+                    if not await send_message(exception):
+                        print_error(f"[websocket.loop] {message}")
             except WebSocketDisconnect:
                 break
             except Exception as e:
                 await on_failed(e, data.hash)
             finally:
                 del target_plugin
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/app/schema.py` & `carefree-drawboard-0.0.0a9/cfdraw/app/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 from abc import abstractmethod
 from abc import ABC
-from typing import Any
-from typing import Callable
-from typing import Coroutine
 from aiohttp import ClientSession
 from asyncio import Event
 from fastapi import FastAPI
-from dataclasses import dataclass
 
 from cfdraw.config import Config
+from cfdraw.schema.plugins import ISend
 from cfdraw.schema.plugins import IPlugin
 from cfdraw.schema.plugins import ISocketRequest
-from cfdraw.schema.plugins import ISocketMessage
 from cfdraw.plugins.factory import Plugins
 
 
-@dataclass
 class IRequestQueueData:
-    request: ISocketRequest
-    plugin: IPlugin
-    event: Event
+    def __init__(self, request: ISocketRequest, plugin: IPlugin):
+        self.request = request
+        self.plugin = plugin
+        self.event = Event()
 
     def __str__(self) -> str:
         return self.request.identifier.split(".")[0]
 
     __repr__ = __str__
 
 
-ISend = Callable[[ISocketMessage], Coroutine[Any, Any, None]]
-
-
 class IRequestQueue(ABC):
     @abstractmethod
     def push(self, data: IRequestQueueData, send_message: ISend) -> str:
         pass
 
     @abstractmethod
     async def run(self) -> None:
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/cli.py` & `carefree-drawboard-0.0.0a9/cfdraw/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/config.py` & `carefree-drawboard-0.0.0a9/cfdraw/config.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/constants.py` & `carefree-drawboard-0.0.0a9/cfdraw/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a9/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a9/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a9/cfdraw/plugins/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,28 @@
         pass
 
     # internal APIs
 
     @property
     def middlewares(self) -> List[IMiddleWare]:
         common_middlewares: List[IMiddleWare] = [
-            TextAreaMiddleWare(self.send_message),
-            FieldsMiddleWare(self.send_message),
-            TimerMiddleWare(self.send_message),
+            TextAreaMiddleWare(self),
+            FieldsMiddleWare(self),
+            TimerMiddleWare(self),
         ]
-        send_message_middleware = SendSocketMessageMiddleWare(self.send_message)
+        send_message_middleware = SendSocketMessageMiddleWare(self)
         return common_middlewares + [send_message_middleware]
 
     async def __call__(self, data: ISocketRequest) -> ISocketMessage:
         middlewares = self.middlewares
         for middleware in middlewares:
             await middleware.before(data)
         response = await self.process(data)
         for middleware in middlewares:
-            response = await middleware(self, response)
+            response = await middleware(response)
         return response
 
     def hash_identifier(self, identifier: str) -> str:
         return f"{identifier}.{self.hash}"
 
     def to_plugin_settings(self) -> Dict[str, Any]:
         d = self.settings.dict()
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a9/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/fields.py` & `carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/plugins/middlewares/send_message.py` & `carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/send_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,14 @@
         ]
 
     @property
     def can_handle_message(self) -> bool:
         return True
 
     async def process(self, response: ISocketMessage) -> ISocketMessage:
-        await self.send_message(response)
+        await self.plugin.send_message(response)
         return response
 
 
 __all__ = [
     "SendSocketMessageMiddleWare",
 ]
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a9/cfdraw/plugins/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
                     plugin_type().to_plugin_settings()
                     for plugin_type in PluginFactory.plugins.values()
                 ],
                 globalSettings=dict(
                     useStrictMode=config.use_react_strict_mode,
                     sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
                 ),
+                boardSettings=dict(),
             ),
         )
 
 
 __all__ = [
     "SyncSocketPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a9/cfdraw/schema/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Union
 from typing import Optional
 from pydantic import Extra
 from pydantic import Field
 from pydantic import BaseModel
 
 
-""" This file should be identical to `src/schema/metaFields.ts` """
+""" This file should be identical to `src/schema/fields.ts` """
 
 
 class FieldType(str, Enum):
     TEXT = "text"
     IMAGE = "image"
     NUMBER = "number"
     SELECT = "select"
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.0a9/cfdraw/schema/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import time
+
 from abc import abstractmethod
 from abc import ABC
 from PIL import Image
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
@@ -20,15 +22,15 @@
 from cfdraw.parsers.noli import PivotType
 from cfdraw.parsers.noli import NodeConstraints
 from cfdraw.parsers.chakra import IChakra
 from cfdraw.parsers.chakra import TextAlign
 
 
 TPluginModel = TypeVar("TPluginModel")
-ISendSocketMessage = Callable[["ISocketMessage"], Coroutine[Any, Any, None]]
+ISend = Callable[["ISocketMessage"], Coroutine[Any, Any, bool]]
 
 
 class PluginType(str, Enum):
     # These types should align with the `allAvailablePythonPlugins` locates at
     # `cfdraw/.web/src/schema/plugins.ts` (without the `_python.` prefix)
     TEXT_AREA = "textArea"
     QA = "QA"
@@ -37,20 +39,30 @@
     _INTERNAL = "_internal"
 
 
 # general
 
 
 class IPluginInfo(BaseModel):
-    """The common data used in `usePython` hook & each React component."""
+    """
+    This should align with:
+    * `cfdraw/.web/src/schema/_python.ts`
+    * `IPythonSocketIntervals`: `retryInterval`, `updateInterval`
+    * `IPythonPluginWithSubmitPluginInfo`: `closeOnSubmit`, `toastOnSubmit`, `toastMessageOnSubmit`
+    """
 
-    updateInterval: int = Field(
-        0,
+    retryInterval: Optional[int] = Field(
+        None,
         ge=0,
-        description="If > 0, the plugin will be called every `updateInterval` ms",
+        description="If not None, the plugin will retry in `retryInterval` ms when exception occurred",
+    )
+    updateInterval: Optional[int] = Field(
+        None,
+        gt=0,
+        description="If not None, the plugin will be called every `updateInterval` ms",
     )
     closeOnSubmit: Optional[bool] = Field(
         None,
         description="Whether close the expanded panel when the submit button is clicked",
     )
     toastOnSubmit: Optional[bool] = Field(
         None,
@@ -74,21 +86,29 @@
 > If set to 'anyNode', the plugin will be shown when any node is selected.
 > If set to 'singleNode', the plugin will be shown when only one node is selected.
 > If set to 'multiNode', the plugin will be shown when more than one node is selected.
 > Otherwise, the plugin will be shown when the selected node is of the specified type.
 """,
     )
     # style fields
-    src: str = Field(
-        "",
+    src: Optional[str] = Field(
+        None,
         description="""
 The image url that will be shown for the plugin.
 > If not specified, we will use a default plugin-ish image.
 """,
     )
+    tooltip: Optional[str] = Field(
+        None,
+        description="""
+The tooltip that will be shown for the plugin.
+> It is recommended to specify an informative tooltip, but it's also OK to leave it as `None`,
+in which case we will not show any tooltip for the plugin.
+""",
+    )
     pivot: Optional[PivotType] = Field(
         None,
         description="""
 Pivot of the plugin.
 > If `follow` is set to `true`, the plugin will be shown at the pivot of the selected node.
 > Otherwise, the plugin will be shown at the pivot of the entire drawboard.
 """,
@@ -116,14 +136,41 @@
         None,
         description="Extra (chakra) props of the plugin's expanded panel",
     )
     # React fields
     pluginInfo: IPluginInfo = Field(IPluginInfo(), description="Plugin info")
 
 
+class ElapsedTimes(BaseModel):
+    createTime: Optional[float]
+    startTime: Optional[float]
+    endTime: Optional[float]
+    pending: Optional[float]
+    executing: Optional[float]
+    total: Optional[float]
+
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+        self.createTime = time.time()
+
+    def start(self) -> None:
+        start = time.time()
+        self.startTime = start
+        if self.createTime is not None:
+            self.pending = start - self.createTime
+
+    def end(self) -> None:
+        end = time.time()
+        self.endTime = end
+        if self.startTime is not None:
+            self.executing = end - self.startTime
+        if self.createTime is not None:
+            self.total = end - self.createTime
+
+
 # web
 
 
 class INodeData(BaseModel):
     """This should align with `INodeData` at `src/schema/_python.ts`"""
 
     type: Optional[INodeType] = Field(None, description="Type of the node")
@@ -212,14 +259,15 @@
         description="Progress of current task, if any",
     )
     intermediate: Optional[ISocketIntermediate] = Field(
         None,
         description="Intermediate responses, if any",
     )
     final: Optional[Dict[str, Any]] = Field(None, description="Final response, if any")
+    elapsedTimes: Optional[ElapsedTimes] = Field(None, description="Elapsed times.")
 
 
 class ISocketMessage(BaseModel):
     """This should align with `IPythonSocketMessage` at `src/schema/_python.ts`"""
 
     hash: str = Field(..., description="Hash of the current task")
     status: SocketStatus = Field(..., description="Status of the current task")
@@ -271,15 +319,16 @@
 
 class IPlugin(ABC):
     hash: str
     identifier: str
     http_session: ClientSession
     # task specific
     task_hash: str
-    send_message: ISendSocketMessage
+    send_message: ISend
+    elapsed_times: ElapsedTimes
 
     @property
     @abstractmethod
     def type(self) -> PluginType:
         pass
 
     @property
@@ -298,15 +347,15 @@
     @abstractmethod
     async def load_image(self, src: str) -> Image.Image:
         pass
 
 
 class IMiddleWare(ABC):
     hash: str
-    send_message: ISendSocketMessage
+    plugin: IPlugin
 
     # abstract
 
     @property
     @abstractmethod
     def subscriptions(self) -> List[PluginType]:
         pass
@@ -326,54 +375,55 @@
         return False
 
     async def before(self, request: ISocketRequest) -> None:
         self.hash = request.hash
 
     # api
 
-    def __init__(self, send_message: ISendSocketMessage) -> None:
-        self.send_message = send_message
+    def __init__(self, plugin: IPlugin) -> None:
+        self.plugin = plugin
 
-    async def __call__(self, plugin: IPlugin, response: Any) -> ISocketMessage:
-        if plugin.type not in self.subscriptions:
+    async def __call__(self, response: Any) -> ISocketMessage:
+        if self.plugin.type not in self.subscriptions:
             return response
         if isinstance(response, ISocketMessage) and not self.can_handle_message:
             return response
         return await self.process(response)
 
     def make_success(self, final: Dict[str, Any]) -> ISocketMessage:
         return ISocketMessage.make_success(self.hash, final)
 
 
 # (react) bindings
 
 
 class IFieldsPluginInfo(IPluginInfo):
+    """This should align with `IPythonFieldsPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
+
     header: Optional[str] = Field(None, description="Header of the plugin")
     definitions: Dict[str, IFieldDefinition] = Field(
         ...,
         description="Field definitions",
     )
     numColumns: Optional[int] = Field(None, description="Number of columns")
-
-
-## text area
+    noErrorToast: Optional[bool] = Field(None, description="Whether not to toast error")
 
 
 class ITextAreaPluginInfo(IPluginInfo):
+    """This should align with `IPythonTextAreaPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
+
     noLoading: bool = Field(
         False, description="Whether to show the 'Loading...' text or not"
     )
     textAlign: Optional[TextAlign] = Field(None, description="Text align")
 
 
-## qa
-
-
 class IQAPluginInfo(IPluginInfo):
+    """This should align with `IPythonQAPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
+
     initialText: str = Field(
         ...,
         description="The initial text to be displayed in the text area",
     )
 
 
 ## deprecated
@@ -386,15 +436,15 @@
 
 @deprecated("please use `IQAPluginInfo` instead")
 class IHttpQAPluginInfo(IQAPluginInfo):
     pass
 
 
 __all__ = [
-    "ISendSocketMessage",
+    "ISend",
     "PluginType",
     # general
     "IPluginInfo",
     "IPluginSettings",
     # web
     "INodeData",
     "ISocketRequest",
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/data_structures.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self._queues: Bundle[Bundle[TItemData]] = Bundle(no_mapping=no_mapping)
 
     def __iter__(self) -> Iterator[Item[Bundle[TItemData]]]:
         return iter(self._queues)
 
     @property
     def is_empty(self) -> bool:
-        return self._queues.is_empty
+        return self.num_items == 0
 
     @property
     def num_queues(self) -> int:
         return len(self._queues)
 
     @property
     def num_items(self) -> int:
@@ -156,29 +156,32 @@
     def get_pending(self, item_key: str) -> Optional[List[Item[TItemData]]]:
         if self._queues.is_empty:
             return None
         layer = 0
         searched = False
         pending: List[Item[TItemData]] = []
         finished_searching = [False] * len(self._queues)
+
+        init = (self._cursor + len(self._queues) - 1) % len(self._queues)
+        cursor = init
         while not all(finished_searching):
-            for i, queue in enumerate(self._queues):
-                if finished_searching[i]:
-                    continue
+            if not finished_searching[cursor]:
+                queue = self._queues.get_index(cursor)
                 if layer >= len(queue.data):
-                    finished_searching[i] = True
-                    continue
-                item = queue.data.get_index(layer)
-                if item.key == item_key:
-                    searched = True
-                    break
-                pending.append(item)
-            if searched:
-                break
-            layer += 1
+                    finished_searching[cursor] = True
+                else:
+                    item = queue.data.get_index(layer)
+                    if item.key == item_key:
+                        searched = True
+                        break
+                    pending.append(item)
+            cursor = (cursor + 1) % len(self._queues)
+            if cursor == init:
+                layer += 1
+
         return pending if searched else None
 
 
 class Types(Generic[TTypes]):
     def __init__(self) -> None:
         self._types: Dict[str, Type[TTypes]] = {}
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/misc.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,34 @@
             lambda new_loop, _future: new_loop.run_until_complete(_future),
             asyncio.new_event_loop(),
             future,
         )
 
 
 # TODO : maybe there will be better solutions?
-# Return True if the `future` is successfully executed
-def offload_run(future: Coroutine[Any, Any, None]) -> bool:
+def offload_run(future: Coroutine[Any, Any, bool]) -> bool:
+    """
+    Return `True` if the `future` is successfully executed.
+
+    * future: Coroutine[Any, Any, bool]
+        should return `True` if successfully executed, and `False` otherwise.
+
+    """
+
     def _run() -> None:
         try:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
-            loop.run_until_complete(future)
+            success = loop.run_until_complete(future)
             loop.close()
-            event.set()
+            if success:
+                event.set()
+            else:
+                print_error("[offload_run] Failed to execute future")
         except Exception as err:
-            print_error(get_err_msg(err))
+            print_error(f"[offload_run] {get_err_msg(err)}")
 
     event = asyncio.Event()
     progress = threading.Thread(target=_run)
     progress.start()
     progress.join()
     return event.is_set()
```

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a8/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a9/cfdraw/utils/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 
 IMAGE_APP_TEMPLATE = f"""
 from PIL import Image
 from PIL import ImageFilter
 from cfdraw import *
 
-# This will perform a Gaussian blur on the image
+# This will apply Gaussian Blur to the image
 class Plugin(IFieldsPlugin):
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(
             w=300,
             h=180,
+            tooltip="Apply Gaussian Blur to the image",
             nodeConstraint=NodeConstraints.IMAGE,
             pivot=PivotType.RT,
             follow=True,
             pluginInfo=IFieldsPluginInfo(
                 definitions=dict(
                     size=INumberField(
                         default=3,
```

### Comparing `carefree-drawboard-0.0.0a8/setup.py` & `carefree-drawboard-0.0.0a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.8"
+VERSION = "0.0.0-alpha.9"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

