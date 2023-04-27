# Comparing `tmp/analysisbykwok-0.0.20.tar.gz` & `tmp/analysisbykwok-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.20.tar", last modified: Sat Apr 22 12:18:06 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.21.tar", last modified: Thu Apr 27 07:32:47 2023, max compression
```

## Comparing `analysisbykwok-0.0.20.tar` & `analysisbykwok-0.0.21.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.914706 analysisbykwok-0.0.20/
--rw-rw-rw-   0        0        0       62 2023-04-22 12:18:06.914706 analysisbykwok-0.0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.895002 analysisbykwok-0.0.20/analysisbykwok/
--rw-rw-rw-   0        0        0    17204 2023-04-22 12:08:05.000000 analysisbykwok-0.0.20/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-22 12:05:02.000000 analysisbykwok-0.0.20/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.913710 analysisbykwok-0.0.20/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2023-04-22 12:11:58.000000 analysisbykwok-0.0.20/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 12:18:06.915704 analysisbykwok-0.0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/
+-rw-rw-rw-   0        0        0       62 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/analysisbykwok/
+-rw-rw-rw-   0        0        0    17177 2023-04-27 07:29:35.000000 analysisbykwok-0.0.21/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-23 02:44:45.000000 analysisbykwok-0.0.21/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 07:32:47.000000 analysisbykwok-0.0.21/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-04-27 07:32:04.000000 analysisbykwok-0.0.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:32:47.068030 analysisbykwok-0.0.21/setup.cfg
```

### Comparing `analysisbykwok-0.0.20/analysisbykwok/__init__.py` & `analysisbykwok-0.0.21/analysisbykwok/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,19 +201,19 @@
                     )
         print('压缩成功，已经压缩到了文件夹:' + str(dir_) + '.zip')
     def ZipOut(dir, out):
         zf = zipfile.ZipFile(dir)
         os.chdir(out)
         ret = zf.extractall(path=out)  # 解压到指定目录
         print('解压成功')
-    def SendEmail(password, receivers, text, sub, filepath):
+    def SendEmail(name,password, receivers, text, sub, filepath):
         smtp_server = "smtp.qq.com"  # 发送邮箱服务器
         username = "yongxingkwok@foxmail.com"  # 用于发送邮箱的用户账号
         sender = 'yongxingkwok@foxmail.com'  # 发送者的邮箱
-        EMAIL_FROM_NAME = '郭永兴'  # 自定义发件人名称
+        EMAIL_FROM_NAME = name  # 自定义发件人名称
         time = datetime.datetime.today().strftime("%m-%d %H：%M")
         msg = MIMEMultipart()
         # 邮件正文
         msg.attach(MIMEText(str(text), 'plain', 'utf-8'))  # 文本内容换行\r\n
         msg['From'] = formataddr(pair=(EMAIL_FROM_NAME, sender))  # 自定义发件人的名称
         msg['To'] = ";".join(receivers)  # 发送给多个好友
         subject = str(sub).format(time)
@@ -318,28 +318,28 @@
             result2 = []
             for son1 in name:
                 result2.append(son1.replace('\'', '').replace('>', '').replace('<', ''))
             result = {}
             result['代码'] = result2
             result['名称'] = result1
             return result
-    def GetPlateInfo(PlateInfoName, url):
+    def GetPlateInfo(PlateInfoName, url,code):
         def FindCode(codes):
             result = []
             pro = ts.pro_api(ApiCode)
             data = pro.daily(ts_code='')
             data = data.sort_values(by='ts_code')
             data = data['ts_code'].T.values.tolist()
             for i in range(0, len(data)):
                 if data[i][:6] == codes:
                     result.append(data[i])
             return result
 
         a =function.GetPlateSon(PlateInfoName)
-        ApiCode=input('输入tushare的秘钥：')
+        ApiCode=code
         pro = ts.pro_api(ApiCode)
         print('正在下载' + str(PlateInfoName) + '板块的股票信息')
         for i in range(0, len(a['代码'])):
             code = FindCode(a['代码'][i])
             for son in code:
                 data = pro.daily(ts_code=son)
                 data.to_csv(r'{}\{}-{}.csv'.format(url, a['名称'][i], a['代码'][i]))
```

