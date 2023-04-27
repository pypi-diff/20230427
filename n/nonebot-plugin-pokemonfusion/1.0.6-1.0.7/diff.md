# Comparing `tmp/nonebot_plugin_pokemonfusion-1.0.6.tar.gz` & `tmp/nonebot_plugin_pokemonfusion-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.6.tar", last modified: Mon Apr 10 05:55:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_pokemonfusion-1.0.7.tar", last modified: Thu Apr 27 18:00:09 2023, max compression
```

## Comparing `nonebot_plugin_pokemonfusion-1.0.6.tar` & `nonebot_plugin_pokemonfusion-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/
--rw-rw-rw-   0        0        0     1084 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      590 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-04-10 02:55:37.000000 nonebot_plugin_pokemonfusion-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.058283 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/
--rw-rw-rw-   0        0        0     3497 2023-04-10 05:36:37.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.064290 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/resources/
--rw-rw-rw-   0        0        0    13834 2023-04-09 07:34:55.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/resources/pokemons.json
-drwxrwxrwx   0        0        0        0 2023-04-10 05:55:43.063292 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/
--rw-rw-rw-   0        0        0      590 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-04-10 05:55:43.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 05:55:42.000000 nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:55:43.065291 nonebot_plugin_pokemonfusion-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-10 05:55:41.000000 nonebot_plugin_pokemonfusion-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:00:09.861925 nonebot_plugin_pokemonfusion-1.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-04-25 23:35:43.000000 nonebot_plugin_pokemonfusion-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1671 2023-04-27 18:00:09.860923 nonebot_plugin_pokemonfusion-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-04-27 17:57:10.000000 nonebot_plugin_pokemonfusion-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 18:00:09.856924 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion/
+-rw-rw-rw-   0        0        0     3457 2023-04-27 17:55:00.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:00:09.860923 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/
+-rw-rw-rw-   0        0        0     1671 2023-04-27 18:00:09.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-27 18:00:09.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:00:09.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-27 18:00:09.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-27 18:00:09.000000 nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:00:09.861925 nonebot_plugin_pokemonfusion-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-27 17:55:20.000000 nonebot_plugin_pokemonfusion-1.0.7/setup.py
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.6/LICENSE` & `nonebot_plugin_pokemonfusion-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pokemonfusion-1.0.6/nonebot_plugin_pokemonfusion/__init__.py` & `nonebot_plugin_pokemonfusion-1.0.7/nonebot_plugin_pokemonfusion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,21 +42,21 @@
         p = Image.new('RGBA', im.size, (255,255,255))
         p.paste(im, (0, 0),mask=im)
         newim = BytesIO()
         p.save(newim,format="png")
         return newim
 
 async def get_image(fusionid):
-    fusionUrl = "https://ghproxy.com/https://raw.githubusercontent.com/Aegide/custom-fusion-sprites/main/CustomBattlers/" + fusionid
+    fusionUrl = "https://raw.githubusercontent.com/Aegide/custom-fusion-sprites/main/CustomBattlers/" + fusionid
     async with httpx.AsyncClient() as client:
         res = await client.get(fusionUrl)
     if res.status_code != 404:
         return(res2BytesIO(res))
     else:
-        fallbackFusionRepository = "https://ghproxy.com/https://raw.githubusercontent.com/Aegide/autogen-fusion-sprites/master/Battlers/"
+        fallbackFusionRepository = "https://raw.githubusercontent.com/Aegide/autogen-fusion-sprites/master/Battlers/"
         headId = fusionid.split(".")[0]
         fallbackFusionUrl = fallbackFusionRepository + headId + "/" + fusionid
         async with httpx.AsyncClient() as client:
             res = await client.get(fallbackFusionUrl)
         return(res2BytesIO(res))
 
 fusion = on_command("融合", aliases={"融合"},priority=3)
```

### Comparing `nonebot_plugin_pokemonfusion-1.0.6/setup.py` & `nonebot_plugin_pokemonfusion-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='utf-8') as fh:
   long_description = fh.read()
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setuptools.setup(
   name="nonebot_plugin_pokemonfusion",
-  version="1.0.6",
+  version="1.0.7",
   author="IllusiveBull",
   author_email="xjn233@gmail.com",
   description="Nonebot2的Pokemon Infinite Fusion中文版融合计算器插件",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/IllusiveBull/nonebot_plugin_pokemonfusion",
   include_package_data = True,
```

