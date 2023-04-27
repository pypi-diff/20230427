# Comparing `tmp/visualtest_python-1.2.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 28537 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1129 b- defN 23-Apr-06 21:42 sbvt/__init__.py
--rw-r--r--  2.0 unx     9191 b- defN 23-Mar-23 22:50 sbvt/api.py
--rw-r--r--  2.0 unx    35553 b- defN 23-Apr-04 15:23 sbvt/browser-safari-bug-test.py
--rw-r--r--  2.0 unx    33376 b- defN 23-Apr-06 21:42 sbvt/browser.py
--rw-r--r--  2.0 unx     5981 b- defN 22-Sep-08 16:30 sbvt/imagetools.py
--rw-r--r--  2.0 unx      548 b- defN 22-Sep-08 16:30 sbvt/timer.py
--rw-r--r--  2.0 unx    10962 b- defN 23-Apr-06 21:41 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-06 21:49 visualtest_python-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Apr-06 21:49 visualtest_python-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 21:49 visualtest_python-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-06 21:49 visualtest_python-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      958 b- defN 23-Apr-06 21:49 visualtest_python-1.2.0.dist-info/RECORD
-12 files, 102744 bytes uncompressed, 26941 bytes compressed:  73.8%
+Zip file size: 20518 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1129 b- defN 23-Apr-26 16:58 sbvt/__init__.py
+-rw-r--r--  2.0 unx     9114 b- defN 23-Apr-26 16:54 sbvt/api.py
+-rw-r--r--  2.0 unx    34618 b- defN 23-Apr-26 16:54 sbvt/browser.py
+-rw-r--r--  2.0 unx     5981 b- defN 22-Sep-26 14:39 sbvt/imagetools.py
+-rw-r--r--  2.0 unx      548 b- defN 22-Sep-26 14:39 sbvt/timer.py
+-rw-r--r--  2.0 unx    11181 b- defN 23-Apr-26 16:54 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      869 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/RECORD
+11 files, 68486 bytes uncompressed, 19060 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: sbvt/__init__.py
 Comment: 
 
 Filename: sbvt/api.py
 Comment: 
 
-Filename: sbvt/browser-safari-bug-test.py
-Comment: 
-
 Filename: sbvt/browser.py
 Comment: 
 
 Filename: sbvt/imagetools.py
 Comment: 
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.2.0.dist-info/LICENSE
+Filename: visualtest_python-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.2.0.dist-info/METADATA
+Filename: visualtest_python-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.2.0.dist-info/WHEEL
+Filename: visualtest_python-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.2.0.dist-info/top_level.txt
+Filename: visualtest_python-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.2.0.dist-info/RECORD
+Filename: visualtest_python-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,14 +1,14 @@
 import logging
 import os.path
 
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 
 logPath = 'logs'
 if not os.path.exists(logPath):
     os.makedirs(logPath)
 
 # By generating a new logger as 'vt' we don't affect global logging from other packages
 # Each logger created in our package should be a child by prefacing with 'vt.childname'
```

## sbvt/api.py

```diff
@@ -157,27 +157,22 @@
         if response.status_code in range(200, 300):
             return result
         else:
             log.error(f'Failed to upload image. HTTP Response: {response.json()}')
             raise Exception(f'Failed to upload image. HTTP Response: {response.json()}')
 
     @staticmethod
-    def getToolkit(script=None):
-        global url
-        if script == 'userAgent':
-            url = f'{cdnUrl}/user-agent.min.js'
-            response = api.get(url)
-            return response.text
-        elif script == 'domCapture':
-            url = f'{cdnUrl}/dom-capture.min.js'
+    def getToolkit(scriptName=None):
+        if scriptName in ['user-agent','dom-capture','freeze-page','chrome-os-version']:
+            url = f'{cdnUrl}/{scriptName}.min.js'
             response = api.get(url)
             return response.text
         else:
-            log.error(f'Failed to grab the {script} CDN image.')
-            raise Exception(f'Failed to grab the {script} CDN image.')
+            log.error(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
+            raise Exception(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
 
     @staticmethod
     def printReport():
 
         for testRun in Api.testRuns:
             if not testRun["testRunId"]:  # logic to check if the users tests failed before a 'saveImage'
                 continue
```

## sbvt/browser.py

```diff
@@ -37,17 +37,18 @@
         if not driver.session_id:
             raise Exception('driver argument does not have a session_id!')
 
         if not driver.capabilities:
             raise Exception('driver argument does not have capabilities!')
 
         # setup api
-        self._userAgentScript = Api.getToolkit(script='userAgent')
-        self._domCaptureScript = Api.getToolkit(script='domCapture')
-
+        self._userAgentScript = Api.getToolkit('user-agent')
+        self._domCaptureScript = Api.getToolkit('dom-capture')
+        self._freezePageScript = Api.getToolkit('freeze-page')
+        self._chromeOsVersion = Api.getToolkit('chrome-os-version')
         self._api = Api()
         log.info(f'Capabilities from driver: {driver.capabilities}')
         self._driver = driver
         self._userAgentInfo = self.getNavigatorUserAgentData(self._driver)
         self._deviceInfo = self._api.getDeviceInfo(self._userAgentInfo, driver.capabilities)
         log.info(f'Final device info: {self._deviceInfo}')
 
@@ -115,19 +116,20 @@
             raise Exception(f'MAX_TIME_MIN must be between 0 and 10 minutes')
         self._MAX_TIME_MIN = minutes
 
     def getNavigatorUserAgentData(self, driver):
         """ Using a custom predefined script, get info from browser's navigator.userAgent """
         agent = driver.execute_script(f'return {self._userAgentScript};')
         log.info(f'Browser info interpreted from navigator.userAgent: {agent}')
-
-        # ensure is dictionary
-        if type(agent) is not dict:
-            log.info(f'navigator.userAgent was not a dictionary, the value was: {agent}')
-            agent = {}
+        if 'browserName' in agent and agent['browserName'] in ['chrome','edge','opera','samsunginternet']:
+            log.info(f'getting osVersion for chrome-based browser')
+            osVersion = driver.execute_async_script(self._chromeOsVersion)
+            if osVersion:
+                agent['osVersion'] = osVersion
+            log.info(f'osVersion for chrome-based browser: {agent["osVersion"]}')
 
         return agent
 
     def captureDom(self, driver, path, type=""):
         """ Using a custom predefined script, capture the webpage's DOM element information """
         domString = driver.execute_script(f'return {self._domCaptureScript};')
 
@@ -146,14 +148,17 @@
     def _findElement(self, cssSelector):
         return self._driver.find_element(By.CSS_SELECTOR, cssSelector)
     
     def _injectIgnoreElements(self, ignoreElements):
         script = 'window.sbvt = { ignoreElements: %s }' % json.dumps(ignoreElements)
         self._driver.execute_script(script)
 
+    def _freezePage(self):
+        self._driver.execute_script(f'return {self._freezePageScript};')
+
     def _getPageDimensions(self):
         script = """
             return JSON.stringify({
                 "document": {
                     "height": document.documentElement.clientHeight,
                     "width": document.documentElement.clientWidth
                 },
@@ -163,15 +168,15 @@
                 },
                 "windowInner": {
                     "height": window.innerHeight,
                     "width":  window.innerWidth
                 },
                 "fullpage": {
                     "height": Math.max(window.document.body.offsetHeight,window.document.body.scrollHeight, window.document.documentElement.offsetHeight, window.document.documentElement.scrollHeight),
-                    "width": Math.max(window.document.body.offsetWidth,window.document.body.scrollWidth, window.document.documentElement.offsetWidth, window.document.documentElement.scrollWidth)
+                    "width": Math.max(window.document.body.offsetWidth, window.document.documentElement.offsetWidth)
                 },
                 "devicePixelRatio": window.devicePixelRatio,
                 "initialScroll": {
                     x: window.scrollX, 
                     y: window.scrollY
                 }
             })
@@ -390,15 +395,15 @@
         try:
             shutil.rmtree(self.tmpDir)
             log.info(f'Deleted tmp images directory: {self.tmpDir}')
             self.tmpDir = None
         except OSError as e:
             log.warning(f'Error deleting tmp directory: {e.filename} - {e.strerror}.')
 
-    def takeFullpageScreenshot(self, path: str, lazyload=None):
+    def takeFullpageScreenshot(self, path: str, options):
         """
         Will take a fullpage screenshot and place the image at the path provided. \n
         Note this places a temporary folder at the current directory with the name sbTemp-{time}
         Args:
             path (str): the directory for where to save the image
             lazyload (int): if set, will scroll the page to load any content first and wait the number of milliseconds provided between each scroll
         """
@@ -438,14 +443,21 @@
             # take the selenium screenshot as final fullpage
             log.info(f'Taking single screenshot for single page')
 
             pageStopWatch = StopWatch()
             pageStopWatch.start()
             totalPageTime = 0
 
+            # freezePage script
+            if 'freezePage' in options:
+                if options['freezePage']:
+                    self._freezePage()
+            else:
+                self._freezePage()
+
             file = os.path.join(self.tmpDir, f'0.png')
             self._driver.save_screenshot(file)
 
             if self._cropEachBottom:
                 file = ImageTools.cropBottom(file, self._cropEachBottom)
 
             if self._cropEachTop:
@@ -467,16 +479,24 @@
         else:
 
             # scroll browser back to initial position
             log.info(f'PREP: Scrolling to top of page')
             self._driver.execute_script('window.scrollTo(0,0)')
 
             # handle lazy-loaded content if setting provided
-            if lazyload != None:
-                self._loadLazyContent(totalPages, lazyload)
+            if 'lazyload' in options:
+                if options['lazyload'] is not None:
+                    self._loadLazyContent(totalPages, options['lazyload'])
+
+            # freezePage script
+            if 'freezePage' in options:
+                if options['freezePage']:
+                    self._freezePage()
+            else:
+                self._freezePage()
 
             # to hide bottom fixed elements, this is a trick that works on most modern browsers
             log.info(f'PREP: Hiding bottom fixed elements: document.body.style.transform="translateY(0)"')
             self._driver.execute_script(f'document.body.style.transform="translateY(0)"')
             time.sleep(0.5) #some browsers need a little time to apply (Safari)
 
             done = False
@@ -637,35 +657,42 @@
 
         # delete the temp screenshot images used to build fullpage
         if not self._debugImages:
             self._deleteTmpDir()
 
         return result
 
-    def takeElementScreenshot(self, element, path):
+    def takeElementScreenshot(self, path, options):
         """
         Will take an element screenshot and place the image at the path provided. \n
         Args:
             element (WebElement): The reference to the Selenium WebElement to capture a screenshot of
             path (str): the directory for where to save the image
         """
         # measure how long it takes
         self.watch = StopWatch()
         self.watch.start()
 
         # create tmp directory for storing images that will be stitched together
         self._createTmpDir(os.path.dirname(path), 'element')
 
+        # freezePage script
+        if 'freezePage' in options:
+            if options['freezePage']:
+                self._freezePage()
+        else:
+            self._freezePage()
+
         # update the dimensions of the browser window and webpage
         self._getPageDimensions()
 
         # selenium.webdriver.firefox.webelement.FirefoxWebElement
-        log.debug(f'type of element is {type(element)}')
+        log.debug(f'type of element is {type(options["element"])}')
         log.info(f'Taking element screenshot of element')
-        element.screenshot(path)
+        options["element"].screenshot(path)
 
         # capture dom AFTER creating screenshot
         self.dom = self.captureDom(self._driver, path, 'element')
 
         # validate final fullpage image dimensions
         imageWidth, imageHeight = ImageTools.getImageSize(path)
 
@@ -684,29 +711,36 @@
         result['dom'] = self.dom #add dom after logging result
 
         if not self._debugImages:
             self._deleteTmpDir()
 
         return result
 
-    def takeViewportScreenshot(self, path):
+    def takeViewportScreenshot(self, path, options):
         """
         Will take a screenshot of the browser viewport and place the image at the path provided. \n
         Args:
             path (str): the directory for where to save the image
         """
         log.info(f'Taking screenshot of viewport')
 
         # measure how long it takes
         self.watch = StopWatch()
         self.watch.start()
 
         # create tmp directory for storing images that will be stitched together
         self._createTmpDir(os.path.dirname(path), 'viewport')
 
+        # freezePage script
+        if 'freezePage' in options:
+            if options['freezePage']:
+                self._freezePage()
+        else:
+            self._freezePage()
+
         # get initial page state for returning to later (must do before hiding scrollbar)
         self._getInitialPageState()
 
         # hide scroll bar for accurate dimensions
         hideScrollBarResult = self._driver.execute_script('return document.body.style.overflow="hidden";')
         log.info(f'PREP: Hide scrollbar result: {hideScrollBarResult}')
```

## sbvt/visualtest.py

```diff
@@ -219,48 +219,54 @@
                     elementsNotFound.append(cssSelector)
             
             if len(elementsNotFound) > 0:
                 raise Exception(f'Some ignoreElements were not found on the page: {",".join(elementsNotFound)}')
             else:
                 self.browser._injectIgnoreElements(options['ignoreElements'])
 
+        if 'freezePage' in options:
+            if not isinstance(options['freezePage'], bool):
+                raise Exception(f'freezePage must be of type "bool"')
+
         if 'element' in options:
-            result = self.browser.takeElementScreenshot(options['element'], filePath)
+            screenshotResult = self.browser.takeElementScreenshot(filePath, options)
             imageType = 'element'
         elif 'viewport' in options and options['viewport'] == True:
-            result = self.browser.takeViewportScreenshot(filePath)
+            result = self.browser.takeViewportScreenshot(filePath, options)
             imageType = 'viewport'
         else:
             if 'lazyload' in options:
                 if type(options['lazyload']) != int or options['lazyload'] < 0 or options['lazyload'] > 10000:
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
-                result = self.browser.takeFullpageScreenshot(filePath, options['lazyload'])
-            else:
-                result = self.browser.takeFullpageScreenshot(filePath)
+
+            screenshotResult = self.browser.takeFullpageScreenshot(filePath, options)
             imageType = 'fullpage'
         
         # save image to server
         imageData = {
             'sessionId': self._sessionId,
             'imageName': name,
             'imageType': imageType,
             'imageExt': 'png',
             'testUrl': self.browser._driver.current_url,
             'viewportWidth': self.browser.viewportWidth,
             'viewportHeight': self.browser.viewportHeight,
-            'imageWidth': result['imageSize']['width'],
-            'imageHeight': result['imageSize']['height'],
+            'imageWidth': screenshotResult['imageSize']['width'],
+            'imageHeight': screenshotResult['imageSize']['height'],
             'dom': json.dumps(self.browser.dom),
             'ignoredElements': json.dumps(self.browser.dom['ignoredElementsData'])
         }
         imageData.update(self.browser._deviceInfo) # required information about device/os/browser
 
         # these two are informational and just used to store - not required
         imageData.update({'driverCapabilities': json.dumps(self.browser.capabilities)})
         imageData.update({'userAgentInfo': json.dumps(self.browser._userAgentInfo)})
 
         # post the image, creating testrun if new
-        self._api.saveImage(self._settings['testRunName'], imageData, filePath)
+        imageApiResult = self._api.saveImage(self._settings['testRunName'], imageData, filePath)
 
-        return result
+        return {
+            'screenshotResult': screenshotResult,
+            'imageApiResult': imageApiResult,
+        }
```

## Comparing `visualtest_python-1.2.0.dist-info/LICENSE` & `visualtest_python-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.2.0.dist-info/METADATA` & `visualtest_python-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `visualtest_python-1.2.0.dist-info/RECORD` & `visualtest_python-1.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-sbvt/__init__.py,sha256=O1nvWpg3l7hxGYGbMZ_NPAvVfdM2vf4kwyuDK32YLmU,1129
-sbvt/api.py,sha256=q9VDvuoozKhDfK7AW3GF_qSrgBWS8XGJ4mc4Sy1GZpc,9191
-sbvt/browser-safari-bug-test.py,sha256=fBvEvdCCfydxstaz90RSpINg2KNBepseRbdObDtuGVo,35553
-sbvt/browser.py,sha256=_IAJSWUA4LW9jwJSeZtBjSMAz1WtL6GYW5fvI0I5WdE,33376
+sbvt/__init__.py,sha256=2r35CuXc9Fnkdlc1BrxcY70WQUsZCxgtgYChni57Wp4,1129
+sbvt/api.py,sha256=BS6nFHtzhfKmYAYcJXvYHmsAlAibNgTRUe4s4Hg8Eyw,9114
+sbvt/browser.py,sha256=IrA2nBhsxk5MODqsFCj51Mx3yOySY74jaoWZ5SPnC9s,34618
 sbvt/imagetools.py,sha256=6z4MA2Wfet8jMlTlKTU68JXSADXNj78fOXQhl7f_ONQ,5981
 sbvt/timer.py,sha256=ciQJQUYSTChdIbsLiYiEzPa6yw8YwSqaeWc7DU4gSrE,548
-sbvt/visualtest.py,sha256=2KrDPx_pOYSl1AEn8dkFhvYpIU10oI4EKzDLNk6nVHY,10962
-visualtest_python-1.2.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
-visualtest_python-1.2.0.dist-info/METADATA,sha256=Ax3iZfKsb9if7s1Tbs8PeUr3lukrfG_u5Cy1JOWLfKA,3876
-visualtest_python-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visualtest_python-1.2.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
-visualtest_python-1.2.0.dist-info/RECORD,,
+sbvt/visualtest.py,sha256=shoeT1Z1aWYZ_WztlX_H1Pw8e6stsZBwt3N_NF15qFc,11181
+visualtest_python-1.3.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
+visualtest_python-1.3.0.dist-info/METADATA,sha256=MsEPiwlbBJTQk1I6Qkrj_2b15BXk60eWu65oTq5oZg8,3876
+visualtest_python-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+visualtest_python-1.3.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
+visualtest_python-1.3.0.dist-info/RECORD,,
```

