# Comparing `tmp/visualtest_python-1.4.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20358 bytes, number of entries: 11
--rw-r--r--  2.0 unx      121 b- defN 23-Jun-01 20:43 sbvt/__init__.py
--rw-r--r--  2.0 unx     8453 b- defN 23-May-26 19:46 sbvt/api.py
--rw-r--r--  2.0 unx    35100 b- defN 23-Jun-01 20:43 sbvt/browser.py
--rw-r--r--  2.0 unx     6269 b- defN 23-Jun-01 20:43 sbvt/imagetools.py
--rw-r--r--  2.0 unx      548 b- defN 23-May-08 21:54 sbvt/timer.py
--rw-r--r--  2.0 unx    14314 b- defN 23-Jun-01 20:43 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/RECORD
-11 files, 70719 bytes uncompressed, 18900 bytes compressed:  73.3%
+Zip file size: 20477 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-27 15:00 sbvt/__init__.py
+-rw-r--r--  2.0 unx     6904 b- defN 23-Jun-27 14:39 sbvt/api.py
+-rw-r--r--  2.0 unx    35671 b- defN 23-Jun-20 12:05 sbvt/browser.py
+-rw-r--r--  2.0 unx     6269 b- defN 23-Jun-09 14:01 sbvt/imagetools.py
+-rw-r--r--  2.0 unx      548 b- defN 23-May-11 09:06 sbvt/timer.py
+-rw-r--r--  2.0 unx    15818 b- defN 23-Jun-27 14:39 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/RECORD
+11 files, 71245 bytes uncompressed, 19019 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.4.0.dist-info/LICENSE
+Filename: visualtest_python-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.4.0.dist-info/METADATA
+Filename: visualtest_python-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.4.0.dist-info/WHEEL
+Filename: visualtest_python-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.4.0.dist-info/top_level.txt
+Filename: visualtest_python-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.4.0.dist-info/RECORD
+Filename: visualtest_python-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,4 +1,4 @@
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.4.0'
+__version__ = '1.5.0'
```

## sbvt/api.py

```diff
@@ -160,43 +160,20 @@
             url = f'{Api.cdnUrl}/{scriptName}.min.js'
             response = api.get(url)
             return response.text
         else:
             log.error(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
             raise Exception(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
 
-    def printReport(self):
-
-        url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images'
-        response = api.get(url).json()
-        imageCount = response["page"]["totalItems"]
-        print(f'View your {imageCount} {"capture" if imageCount == 1 else "captures"} here: ' + Fore.BLUE + f'{Api.webUrl}/projects/{response["items"][0]["projectId"]}/testruns/{response["items"][0]["testRunId"]}/comparisons'+ Style.RESET_ALL)
-
-        comparisonUrl = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}?expand=comparison-totals'
-        comparisons = {"complete": 0}
-        maxLoops = 20
-        countLoops = 0
-        while comparisons["complete"] != imageCount and countLoops <= maxLoops:
+    def getTestRunResult(self, timeout=3):
+        if not self.testRun:
+            raise Exception("Cannot run get testrun result without first taking a capture()")
+        i = 0
+        comparisons = { 'pending': 1 }
+        while comparisons['pending'] > 0 and i < timeout * 4 * 60:
+            url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}?expand=comparison-totals'
+            response = api.get(url).json()
+            comparisons = response['comparisons']
+            i = i + 1
             time.sleep(0.25)
-            log.info(f'imageCount: {imageCount} != comparisonTotal: {comparisons["complete"]} -- mismatch... running again for testRun {self.testRun} countLoops: {countLoops}')
-            comparisonResult = api.get(comparisonUrl).json()
-            comparisons = comparisonResult["comparisons"]
-            countLoops += 1
-
-        try:
-            # print(f'Comparisons: {str(comparisons)}')
-            new = comparisons["status"]["new_image"]
-            failed = comparisons["status"]["unreviewed"]
-            passed = comparisons["status"]["passed"]
-
-            if new:
-                print(Style.BRIGHT + Fore.YELLOW + f'\t{new} new base {"image" if new == 1 else "images"}' + Style.RESET_ALL)
-            if failed:
-                print(Style.BRIGHT + Fore.RED + f'\t{failed} image comparison {"failure" if failed == 1 else "failures"} to review' + Style.RESET_ALL)
-            if passed:
-                print(Style.RESET_ALL + Style.BRIGHT + Fore.GREEN + f'\t{passed} image comparisons passed' + Style.RESET_ALL)
-            if comparisons["complete"] != imageCount:
-                print(Style.BRIGHT + Fore.MAGENTA + f'\tTimed out getting comparisons results' + Style.RESET_ALL)
-        except Exception as e:
-            print(Style.BRIGHT + Fore.MAGENTA + f'\tError getting comparisons results: {str(e)}' + Style.RESET_ALL)
-
+        return comparisons
```

## sbvt/browser.py

```diff
@@ -399,15 +399,15 @@
             lazyload (int): if set, will scroll the page to load any content first and wait the number of milliseconds provided between each scroll
         """
         imageBinary = bytearray()  # New empty byte array
 
         if self._deviceInfo['osName'] == 'ios':
             raise Exception('iOS devices do no currently support fullpage screenshots.')
 
-        log.info(f'Taking full page screenshot at URL: {self._driver.current_url}')
+        log.info(f'Taking full page for image name "{name}" screenshot at URL: {self._driver.current_url}')
 
         # limit how long we let a screenshot run
         self.fullpageStopWatch = StopWatch()
         self.fullpageStopWatch.start()
 
         # create images directory for debug
         debugImageDir = None
@@ -517,29 +517,33 @@
                 # don't scroll for first pageIndex
                 if pageIndex > 0:
 
                     # scroll and check scrolled correctly
                     scrolled = self._scrollPage(pageIndex)
 
                     # check if the page height changed
-                    if self._fullpageHeightChanged():
+                    if self._scrollMethod == 'JS_SCROLL' and self._fullpageHeightChanged():
                         newTotalPages = self._getNumberOfPagesToScroll()
                         if newTotalPages > totalPages:
                             totalPages = newTotalPages
                             log.info(f'Total pages is now {totalPages}')
                             # if grew, scroll again to same position to ensure 
                             # handles infinite-scroll or lazy loaded content
                             self._scrollPage(pageIndex)
 
                 # check if we should stop scrolling due to a limit
                 hitLimit, reasonStopped = self._checkScrollingLimits(pageIndex, totalPages)
 
                 # take the selenium screenshot
-                viewportImage = self._driver.get_screenshot_as_png()
-
+                if self._deviceInfo["browserName"].capitalize() == 'Safari':
+                    screenshotElement = self._driver.find_element(By.TAG_NAME, 'body')
+                    viewportImage = screenshotElement.screenshot_as_png
+                else:
+                    viewportImage = self._driver.get_screenshot_as_png()
+                
                 if self._debug:
                     debugImageName = f'{pageIndex}.png'
                     debugImagePath = os.path.join(debugImageDir, debugImageName)
                     with open(debugImagePath, 'wb') as outfile:
                         outfile.write(viewportImage)
                         outfile.close()
 
@@ -662,14 +666,15 @@
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
         result['imageBinary'] = imageBinary
 
         return result
 
+
     def takeElementScreenshot(self, options):
         """
         Will take an element screenshot and place the image at the path provided. \n
         Args:
             element (WebElement): The reference to the Selenium WebElement to capture a screenshot of
             path (str): the directory for where to save the image
         """
@@ -747,15 +752,19 @@
         # hide scroll bar for accurate dimensions
         hideScrollBarResult = self._driver.execute_script('return document.body.style.overflow="hidden";')
         log.info(f'PREP: Hide scrollbar result: {hideScrollBarResult}')
 
         # update the dimensions of the browser window and webpage
         self._getPageDimensions()
 
-        imageBinary = self._driver.get_screenshot_as_png()
+        if self._deviceInfo["browserName"].capitalize() == 'Safari':
+            screenshotElement = self._driver.find_element(By.TAG_NAME, 'body')
+            imageBinary = screenshotElement.screenshot_as_png
+        else:
+            imageBinary = self._driver.get_screenshot_as_png()
 
         if self._cropEachBottom:
             imageBinary = ImageTools.cropBottom(imageBinary, self._cropEachBottom)
 
         if self._cropEachTop:
             imageBinary = ImageTools.cropTop(imageBinary, self._cropEachTop)
 
@@ -789,7 +798,9 @@
             'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
         result['imageBinary'] = imageBinary
         return result
+
+
```

## sbvt/visualtest.py

```diff
@@ -2,14 +2,15 @@
 import os
 import logging
 import time
 
 from .browser import Browser
 from .imagetools import ImageTools
 from .api import Api
+from colorama import Fore, Style
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
 
 class VisualTest:
     """
     Class for SmartBear VisualTest
 
@@ -272,22 +273,24 @@
             else:
                 raise Exception(f'comparisonMode value should be "detailed" or "layout" mode.')
 
         if 'element' in options:
             screenshotResult = self.browser.takeElementScreenshot(options)
             imageType = 'element'
         elif 'viewport' in options and options['viewport'] == True:
+
             screenshotResult = self.browser.takeViewportScreenshot(options)
             imageType = 'viewport'
         else:
             if 'lazyload' in options:
                 if type(options['lazyload']) != int or options['lazyload'] < 0 or options['lazyload'] > 10000:
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
 
             screenshotResult = self.browser.takeFullpageScreenshot(name, options)
+
             imageType = 'fullpage'
         
         # save image to server
         imageData = {
             'sessionId': self._sessionId,
             'imageName': name,
             'imageType': imageType,
@@ -339,8 +342,35 @@
 
         return {
             'screenshotResult': screenshotResult,
             'imageApiResult': imageApiResult,
         }
 
     def printReport(self):
-        return self._api.printReport()
+        
+        comparisons = self._api.getTestRunResult()
+        imageCount = comparisons["total"]
+        print(f'View your {imageCount} {"capture" if imageCount == 1 else "captures"} here: ' + Fore.BLUE + self._api.testRun['appUrl'] + Style.RESET_ALL)
+
+        try:
+            # print(f'Comparisons: {str(comparisons)}')
+            new = comparisons["status"]["new_image"]
+            failed = comparisons["status"]["unreviewed"]
+            passed = comparisons["status"]["passed"]
+
+            if new:
+                print(Style.BRIGHT + Fore.YELLOW + f'\t{new} new base {"image" if new == 1 else "images"}' + Style.RESET_ALL)
+            if failed:
+                print(Style.BRIGHT + Fore.RED + f'\t{failed} image comparison {"failure" if failed == 1 else "failures"} to review' + Style.RESET_ALL)
+            if passed:
+                print(Style.RESET_ALL + Style.BRIGHT + Fore.GREEN + f'\t{passed} image comparisons passed' + Style.RESET_ALL)
+            if comparisons["complete"] != imageCount:
+                print(Style.BRIGHT + Fore.MAGENTA + f'\tTimed out getting comparisons results' + Style.RESET_ALL)
+        except Exception as e:
+            print(Style.BRIGHT + Fore.MAGENTA + f'\tError getting comparisons results: {str(e)}' + Style.RESET_ALL)
+
+    def getTestRunResult(self):
+        comparisons = self._api.getTestRunResult()
+        return {
+            'passed' : comparisons['aggregate']['passed'], 
+            'failed' : comparisons['aggregate']['failed']
+            }
```

## Comparing `visualtest_python-1.4.0.dist-info/LICENSE` & `visualtest_python-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.4.0.dist-info/METADATA` & `visualtest_python-1.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `visualtest_python-1.4.0.dist-info/RECORD` & `visualtest_python-1.5.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-sbvt/__init__.py,sha256=aKQW8BR2G4m8PNJa8IYmZay5M8P1VJ-bKTVjp-c5Rbc,121
-sbvt/api.py,sha256=2F2qgGLUDfQnnc58wwWgpmpgVcZLGIm1AsONKqLz4aQ,8453
-sbvt/browser.py,sha256=5MJ5s-A5JxGMRKknuOyXpCctXG39k13ENmtLWZblW4Y,35100
+sbvt/__init__.py,sha256=2agJBIkgnUZoVKzrVT7YbSxxBBFkmliHMzytcRVm2L0,121
+sbvt/api.py,sha256=8oFBLbYAKU0PbgJ0781gUYjOTE5fFRvQlJryty1UwDs,6904
+sbvt/browser.py,sha256=YGJOpBltpK_WAuUrYlhjVaF_cy2of_oTEmvBfZXY3Bo,35671
 sbvt/imagetools.py,sha256=rZjArTuJkuSZOeuGWccRwyBsBxJMdvaWRwTxZuh0O-g,6269
 sbvt/timer.py,sha256=ciQJQUYSTChdIbsLiYiEzPa6yw8YwSqaeWc7DU4gSrE,548
-sbvt/visualtest.py,sha256=ZChEY5bB8DMQ_H18KbDvBFuwWjrck8lZPnP9Q3OjvcA,14314
-visualtest_python-1.4.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
-visualtest_python-1.4.0.dist-info/METADATA,sha256=3Ly0oSBbnNNpnpNCAS_i556FpXrLcQZelheA5bNDxco,3876
-visualtest_python-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visualtest_python-1.4.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
-visualtest_python-1.4.0.dist-info/RECORD,,
+sbvt/visualtest.py,sha256=SJPv8oWIb30q1bp5jj5NtoXNohPcWOTnfqHLLCZ5Qz4,15818
+visualtest_python-1.5.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
+visualtest_python-1.5.0.dist-info/METADATA,sha256=Z8dzV5_sjkXT7Cvox2WkdxzTd_Y5l4OS7BKeHbnoFeM,3876
+visualtest_python-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+visualtest_python-1.5.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
+visualtest_python-1.5.0.dist-info/RECORD,,
```

