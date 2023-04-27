# Comparing `tmp/BookerDownloadTool-2023.1.30.3.tar.gz` & `tmp/BookerDownloadTool-2023.4.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BookerDownloadTool-2023.1.30.3.tar", last modified: Fri Mar 10 08:18:13 2023, max compression
+gzip compressed data, was "dist\BookerDownloadTool-2023.4.27.0.tar", last modified: Thu Apr 27 01:52:11 2023, max compression
```

## Comparing `BookerDownloadTool-2023.1.30.3.tar` & `BookerDownloadTool-2023.4.27.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/
--rw-rw-rw-   0        0        0      234 2023-03-10 08:18:07.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/__init__.py
--rw-rw-rw-   0        0        0     4328 2023-01-30 17:11:16.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/__main__.py
--rw-rw-rw-   0        0        0     3312 2023-01-30 15:07:30.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/bili.py
--rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/dl_gh_book.py
--rw-rw-rw-   0        0        0     4649 2022-08-20 12:53:30.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/lightnovel.py
--rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/stealth.min.js
--rw-rw-rw-   0        0        0     1882 2023-01-30 17:07:12.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/util.py
--rw-rw-rw-   0        0        0     2273 2023-01-30 17:09:14.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/zhihu_ques.py
--rw-rw-rw-   0        0        0     4628 2022-08-20 13:02:41.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool/zhihu_ques_sele.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1192 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/PKG-INFO
--rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.1.30.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-10 08:18:13.000000 BookerDownloadTool-2023.1.30.3/setup.cfg
--rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.1.30.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/
+drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/
+-rw-rw-rw-   0        0        0      234 2023-04-27 01:49:50.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/__init__.py
+-rw-rw-rw-   0        0        0     8945 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/__main__.py
+-rw-rw-rw-   0        0        0     3408 2023-04-20 02:11:02.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/bili.py
+-rw-rw-rw-   0        0        0     8003 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/discuz.py
+-rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dl_gh_book.py
+-rw-rw-rw-   0        0        0     5202 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dmzj.py
+-rw-rw-rw-   0        0        0     4649 2022-08-20 12:53:30.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/lightnovel.py
+-rw-rw-rw-   0        0        0     3875 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/nhentai.py
+-rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/stealth.min.js
+-rw-rw-rw-   0        0        0     2784 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/util.py
+-rw-rw-rw-   0        0        0     2326 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques.py
+-rw-rw-rw-   0        0        0     4640 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques_sele.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1192 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/setup.py
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/bili.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/bili.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 def download_bili_safe(args):
     try: download_bili(args)
     except Exception as ex: print(ex)
 
 def download_bili(args):
     id = args.id
     to_audio = args.audio
+    sp = args.start_page
+    ep = args.end_page
+    opath = args.output_dir
+    safe_mkdir(opath)
     av = ''
     bv = ''
     if id.lower().startswith('av'):
         av = id[2:]
     else:
         bv = id
         
@@ -62,28 +66,27 @@
     if j['code'] != 0:
         print('获取 CID 失败：' + j['message'])
         return
     av = j['data']['aid']
     bv = j['data']['bvid']
     author = fname_escape(j['data']['owner']['name'])
     title1 = fname_escape(j['data']['title'])
-    for it in j['data']['pages']:
+    for it in j['data']['pages'][sp-1:ep]:
         cid = it['cid']
         pg = it['page']
         title2 = fname_escape(it['part'])
-        title = title1 if title1 == title2 \
-                else f'{title1} P{pg} - {title2}'
+        title = f'{title1} - P{pg}' if title1 == title2 \
+            else f'{title1} - P{pg}：{title2}'
         print(title, author)
         name = f'{title} - {author} - {bv}'
-        fname = f'out/{name}.mp3' if to_audio else f'out/{name}.flv'
+        ext = 'mp3' if to_audio else 'flv'
+        fname = path.join(opath, name + '.' + ext)
         if path.isfile(fname):
             print(f'{fname} 已存在')
             continue
-        try: os.mkdir('out')
-        except: pass
         url = f'https://api.bilibili.com/x/player/playurl?cid={cid}&otype=json&bvid={bv}&aid={av}'
         j = requests.get(url, headers=bili_hdrs).json()
         if j['code'] != 0:
             print('解析失败：' + j['message'])
             continue
         video_url = j['data']['durl'][0]['url']
         video = requests.get(video_url, headers=bili_hdrs).content
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/dl_gh_book.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dl_gh_book.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/lightnovel.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/lightnovel.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/stealth.min.js` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/stealth.min.js`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/util.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 import requests
 import os
 import shutil
 from os import path
 import imgyaso
+import subprocess as subp
+import tempfile
+import uuid
+
+RE_INFO = r'\[(.+?)\]([^\[]+)'
 
 bili_hdrs = {
     'User-Agent': 'PostmanRuntime/7.26.8',
     'Referer': 'https://www.bilibili.com/',
 }
 
+dmzj_hdrs = {
+    'Referer': 'http://manhua.dmzj.com/',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
+}
+
 default_hdrs = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
 }
 
 UA = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36'
 
 DIR = path.dirname(path.abspath(__file__))
 
-def d(name):
-    return path.join(DIR, name)
+d = lambda name: path.join(path.dirname(__file__, name))
+
+    
+def is_gbk(ch):
+    try: 
+        ch.encode('gbk')
+        return True
+    except:
+        return False
+    
+def filter_gbk(fname):
+    return ''.join([ch for ch in fname if is_gbk(ch)])
 
 def opti_img(img, mode, colors):
     if mode == 'quant':
         return imgyaso.pngquant_bts(img, colors)
     elif mode == 'grid':
         return imgyaso.grid_bts(img)
     elif mode == 'trunc':
@@ -53,13 +73,28 @@
         except KeyboardInterrupt as e:
             raise e
         except Exception as e:
             print(f'{url} retry {i}')
             if i == retry - 1: raise e
 
 def safe_mkdir(dir):
-    try: os.mkdir(dir)
+    try: os.makedirs(dir)
     except: pass
     
 def safe_rmdir(dir):
     try: shutil.rmtree(dir)
     except: pass
+
+def safe_remove(fname):
+    try: os.unlink(fname)
+    except: pass
+
+def anime4k_auto(img):
+    fname = path.join(tempfile.gettempdir(), uuid.uuid4().hex + '.png')
+    open(fname, 'wb').write(img)
+    subp.Popen(
+        ['wiki-tool', 'anime4k-auto', fname, '-G'], 
+        shell=True,
+    ).communicate()
+    img = open(fname, 'rb').read()
+    safe_remove(fname)
+    return img
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/zhihu_ques.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         {co}
     '''
     return {'title': au_name, 'content': co}
     
 def zhihu_ques(args):
     qid = args.qid
     cralwer_config['optiMode'] = args.opti_mode
-    
+    cralwer_config['imgSrc'] = ['data-original', 'src']
+
     url = f'https://www.zhihu.com/api/v4/questions/{qid}//answers?limit=20&include=content,voteup_count'
     j = request_retry('GET', url, headers=headers).json()
     title = '知乎问答：' + j['data'][0]['question']['title']
     co = f'''
         <blockquote>来源：<a href='https://www.zhihu.com/question/{qid}'>https://www.zhihu.com/question/{qid}</a></blockquote>
     '''
     articles = [{'title': title, 'content': co}]
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 = datetime.utcfromtimestamp(art['updated_time']).strftime('%Y-%m-%d') co =
 re.sub(r'.+?', '', art['content']) co = re.sub(r' src=".+?"', '', co) \
 .replace('data-actualsrc', 'src') co = f'''
      ä½èï¼{au_name}
      èµåæ°ï¼{vote}
      ç¼è¾äºï¼{upd_time}
 {co} ''' return {'title': au_name, 'content': co} def zhihu_ques(args): qid =
-args.qid cralwer_config['optiMode'] = args.opti_mode url = f'https://
-www.zhihu.com/api/v4/questions/{qid}//
+args.qid cralwer_config['optiMode'] = args.opti_mode cralwer_config['imgSrc'] =
+['data-original', 'src'] url = f'https://www.zhihu.com/api/v4/questions/{qid}//
 answers?limit=20&include=content,voteup_count' j = request_retry('GET', url,
 headers=headers).json() title = 'ç¥ä¹é®ç­ï¼' + j['data'][0]['question']
 ['title'] co = f'''
      æ¥æºï¼https://www.zhihu.com/question/{qid}
 ''' articles = [{'title': title, 'content': co}] imgs = {} while True: print
 (url) j = request_retry('GET', url, headers=headers).json() for art in j
 ['data']: art = get_content(art) art['content'] = process_img( art['content'],
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool/zhihu_ques_sele.py` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques_sele.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from EpubCrawler.config import config as cralwer_config
 from datetime import datetime
 from GenEpub import gen_epub
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from .util import *
 
-cralwer_config['optiMode'] = 'thres'
-cralwer_config['imgSrc'] = ['data-original', 'src']
-
 # 滚动到底
 def scroll_to_bottom(driver):
     driver.execute_script('''
         document.documentElement.scrollTop = 100000000
     ''')
     
 # 判断是否到底
@@ -87,15 +84,18 @@
             </blockquote>
             {co}
         '''
         articles.append({'title': au_name, 'content': co})
     return articles
 
 def zhihu_ques_sele(args):
+    cralwer_config['optiMode'] = 'thres'
+    cralwer_config['imgSrc'] = ['data-original', 'src']
     qid = args.qid
+    
     url = f'https://www.zhihu.com/question/{qid}'
     options = Options()
     options.add_argument('--headless')
     options.add_argument('--disable-gpu')
     options.add_argument('--log-level=3')
     options.add_argument(f'--user-agent={UA}')
     options.add_argument("--disable-blink-features=AutomationControlled")
```

#### html2text {}

```diff
@@ -1,48 +1,48 @@
 import re import sys import time import traceback from os import path from
 pyquery import PyQuery as pq from EpubCrawler.util import request_retry from
 EpubCrawler.img import process_img from EpubCrawler.config import config as
 cralwer_config from datetime import datetime from GenEpub import gen_epub from
 selenium import webdriver from selenium.webdriver.chrome.options import Options
-from .util import * cralwer_config['optiMode'] = 'thres' cralwer_config
-['imgSrc'] = ['data-original', 'src'] # æ»å¨å°åº def scroll_to_bottom
-(driver): driver.execute_script(''' document.documentElement.scrollTop =
-100000000 ''') # å¤æ­æ¯å¦å°åº def if_reach_bottom(driver): return
-driver.execute_script(''' return document.querySelector('.QuestionAnswers-
-answerButton') != null ''') # è·åæåä¸ä¸ª AID def get_last_aid(driver):
-return driver.execute_script(''' var ansLi = document.querySelectorAll
-('.AnswerItem') return (ansLi.length == 0)? '': ansLi[ansLi.length -
-1].getAttribute('name') ''') # è·å AID æ°é def get_aid_count(driver):
-return driver.execute_script(''' var ansLi = document.querySelectorAll
-('.AnswerItem') return ansLi.length ''') # è·ååç­æ°é def get_ans_count
-(driver): return driver.execute_script(''' var el = document.querySelector
-('h4.List-headerText') if (!el) return 0 var text = el.innerText.replace(',',
-'') var m = /\d+/.exec(text) if (!m) return 0 return Number.parseInt(m[0]) ''')
-# è·åæ´ä¸ªé¡µé¢ HTML def get_html(driver): return driver.execute_script
-(''' return document.documentElement.outerHTML ''') # è·åæç« åè¡¨ def
-get_articles(html, qid): rt = pq(html) rt.remove('noscript, .GifPlayer-icon, a
-svg') title = 'ç¥ä¹é®ç­ï¼' + fname_escape(rt('h1.QuestionHeader-title').eq
-(0).text()) co = f'''
+from .util import * # æ»å¨å°åº def scroll_to_bottom(driver):
+driver.execute_script(''' document.documentElement.scrollTop = 100000000 ''') #
+å¤æ­æ¯å¦å°åº def if_reach_bottom(driver): return driver.execute_script
+(''' return document.querySelector('.QuestionAnswers-answerButton') != null
+''') # è·åæåä¸ä¸ª AID def get_last_aid(driver): return
+driver.execute_script(''' var ansLi = document.querySelectorAll('.AnswerItem')
+return (ansLi.length == 0)? '': ansLi[ansLi.length - 1].getAttribute('name')
+''') # è·å AID æ°é def get_aid_count(driver): return
+driver.execute_script(''' var ansLi = document.querySelectorAll('.AnswerItem')
+return ansLi.length ''') # è·ååç­æ°é def get_ans_count(driver): return
+driver.execute_script(''' var el = document.querySelector('h4.List-headerText')
+if (!el) return 0 var text = el.innerText.replace(',', '') var m = /\d+/.exec
+(text) if (!m) return 0 return Number.parseInt(m[0]) ''') # è·åæ´ä¸ªé¡µé¢
+HTML def get_html(driver): return driver.execute_script(''' return
+document.documentElement.outerHTML ''') # è·åæç« åè¡¨ def get_articles
+(html, qid): rt = pq(html) rt.remove('noscript, .GifPlayer-icon, a svg') title
+= 'ç¥ä¹é®ç­ï¼' + fname_escape(rt('h1.QuestionHeader-title').eq(0).text())
+co = f'''
      æ¥æºï¼https://www.zhihu.com/question/{qid}
 ''' articles = [{'title': title, 'content': co}] el_ansLi = rt('.AnswerItem')
 for i in range(len(el_ansLi)): el = el_ansLi.eq(i) el_au = el.find('.UserLink-
 link') au_name = (el_au.text() or 'å¿åç¨æ·').strip() au_url = el_au.attr
 ('href') or '' el_time = el.find('.ContentItem-time>a') co_url = el_time.attr
 ('href') vote = el.find('.VoteButton--up').attr('aria-label').strip()[3:
 ] upd_time = el_time.text().strip()[4:] co = el.find('.RichText').html() co =
 f'''
      ä½èï¼{au_name}
      èµåæ°ï¼{vote}
      ç¼è¾äºï¼{upd_time}
 {co} ''' articles.append({'title': au_name, 'content': co}) return articles def
-zhihu_ques_sele(args): qid = args.qid url = f'https://www.zhihu.com/question/
-{qid}' options = Options() options.add_argument('--headless')
-options.add_argument('--disable-gpu') options.add_argument('--log-level=3')
-options.add_argument(f'--user-agent={UA}') options.add_argument("--disable-
-blink-features=AutomationControlled") driver = webdriver.Chrome
+zhihu_ques_sele(args): cralwer_config['optiMode'] = 'thres' cralwer_config
+['imgSrc'] = ['data-original', 'src'] qid = args.qid url = f'https://
+www.zhihu.com/question/{qid}' options = Options() options.add_argument('--
+headless') options.add_argument('--disable-gpu') options.add_argument('--log-
+level=3') options.add_argument(f'--user-agent={UA}') options.add_argument("--
+disable-blink-features=AutomationControlled") driver = webdriver.Chrome
 (options=options) driver.set_script_timeout(1000) # StealthJS stealth = open(d
 ('stealth.min.js')).read() driver.execute_cdp_cmd
 ("Page.addScriptToEvaluateOnNewDocument", { "source": stealth }) driver.get
 (url) # å³é­ç»å½å¯¹è¯æ¡ driver.execute_script(''' var cls_btn =
 document.querySelector('.Modal-closeButton') if (cls_btn) cls_btn.click() ''')
 ansCnt = get_ans_count(driver) # å¦ææ²¡æå°åºå°±ä¸ç´æ»å¨ while not
 if_reach_bottom(driver): try: cnt = get_aid_count(driver) print(f'reach bottom:
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/PKG-INFO` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.1.30.3
+Version: 2023.4.27.0
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
 Author: ApacheCN
 Author-email: apachecn@163.com
 License: UNKNOWN
 Description: # BookerDownloadTool
 Platform: UNKNOWN
```

### Comparing `BookerDownloadTool-2023.1.30.3/BookerDownloadTool.egg-info/SOURCES.txt` & `BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 README.md
 setup.py
 BookerDownloadTool/__init__.py
 BookerDownloadTool/__main__.py
 BookerDownloadTool/bili.py
+BookerDownloadTool/discuz.py
 BookerDownloadTool/dl_gh_book.py
+BookerDownloadTool/dmzj.py
 BookerDownloadTool/lightnovel.py
+BookerDownloadTool/nhentai.py
 BookerDownloadTool/stealth.min.js
 BookerDownloadTool/util.py
 BookerDownloadTool/zhihu_ques.py
 BookerDownloadTool/zhihu_ques_sele.py
 BookerDownloadTool.egg-info/PKG-INFO
 BookerDownloadTool.egg-info/SOURCES.txt
 BookerDownloadTool.egg-info/dependency_links.txt
```

### Comparing `BookerDownloadTool-2023.1.30.3/PKG-INFO` & `BookerDownloadTool-2023.4.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.1.30.3
+Version: 2023.4.27.0
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
 Author: ApacheCN
 Author-email: apachecn@163.com
 License: UNKNOWN
 Description: # BookerDownloadTool
 Platform: UNKNOWN
```

### Comparing `BookerDownloadTool-2023.1.30.3/setup.py` & `BookerDownloadTool-2023.4.27.0/setup.py`

 * *Files identical despite different names*

