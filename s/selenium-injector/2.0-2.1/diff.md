# Comparing `tmp/selenium_injector-2.0.tar.gz` & `tmp/selenium_injector-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_injector-2.0.tar", last modified: Tue Jun 20 13:09:52 2023, max compression
+gzip compressed data, was "dist\selenium_injector-2.1.tar", last modified: Tue Jun 27 08:06:16 2023, max compression
```

## Comparing `selenium_injector-2.0.tar` & `selenium_injector-2.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.0/LICENSE.md
--rw-rw-rw-   0        0        0      228 2023-06-20 11:58:10.000000 selenium_injector-2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4931 2023-06-20 13:09:52.000000 selenium_injector-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3625 2023-06-20 12:51:01.000000 selenium_injector-2.0/README.md
--rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.0/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.0/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-06-20 13:09:52.000000 selenium_injector-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1826 2023-06-20 11:40:08.000000 selenium_injector-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/
--rw-rw-rw-   0        0        0       21 2023-06-20 13:09:46.000000 selenium_injector-2.0/src/selenium_injector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/extension/
--rw-rw-rw-   0        0        0     3155 2023-06-20 10:48:36.000000 selenium_injector-2.0/src/selenium_injector/files/extension/background.js
--rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.0/src/selenium_injector/files/extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/js/
--rw-rw-rw-   0        0        0     6031 2023-06-20 13:01:28.000000 selenium_injector-2.0/src/selenium_injector/files/js/connection.js
--rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.0/src/selenium_injector/files/js/utils.js
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/
--rw-rw-rw-   0        0        0     9312 2023-06-20 13:05:57.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/background.js
--rw-rw-rw-   0        0        0        0 2023-04-06 20:20:08.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/content_helper.js
--rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/manifest.json
--rw-rw-rw-   0        0        0     6050 2023-06-17 13:56:27.000000 selenium_injector-2.0/src/selenium_injector/injector.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.0/src/selenium_injector/scripts/__init__.py
--rw-rw-rw-   0        0        0     6295 2023-06-20 11:35:20.000000 selenium_injector-2.0/src/selenium_injector/scripts/driverless.py
--rw-rw-rw-   0        0        0     1576 2023-06-20 10:58:22.000000 selenium_injector-2.0/src/selenium_injector/scripts/js.py
--rw-rw-rw-   0        0        0     1742 2023-06-20 11:34:48.000000 selenium_injector-2.0/src/selenium_injector/scripts/socket.py
--rw-rw-rw-   0        0        0     3804 2023-06-20 12:49:54.000000 selenium_injector-2.0/src/selenium_injector/scripts/sync_websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/utils/
--rw-rw-rw-   0        0        0       19 2022-11-24 10:40:41.000000 selenium_injector-2.0/src/selenium_injector/utils/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-06-20 11:35:20.000000 selenium_injector-2.0/src/selenium_injector/utils/utils.py
--rw-rw-rw-   0        0        0     1841 2023-06-20 13:00:41.000000 selenium_injector-2.0/src/selenium_injector/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/
--rw-rw-rw-   0        0        0     4931 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.1/LICENSE.md
+-rw-rw-rw-   0        0        0      228 2023-06-20 11:58:10.000000 selenium_injector-2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5124 2023-06-27 08:06:16.000000 selenium_injector-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3818 2023-06-26 17:27:31.000000 selenium_injector-2.1/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.1/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-06-27 08:06:16.000000 selenium_injector-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1826 2023-06-20 11:40:08.000000 selenium_injector-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/
+-rw-rw-rw-   0        0        0       21 2023-06-27 08:05:47.000000 selenium_injector-2.1/src/selenium_injector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/extension/
+-rw-rw-rw-   0        0        0     3032 2023-06-26 17:42:08.000000 selenium_injector-2.1/src/selenium_injector/files/extension/background.js
+-rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.1/src/selenium_injector/files/extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/js/
+-rw-rw-rw-   0        0        0     6058 2023-06-27 07:29:06.000000 selenium_injector-2.1/src/selenium_injector/files/js/connection.js
+-rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.1/src/selenium_injector/files/js/utils.js
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/
+-rw-rw-rw-   0        0        0     9216 2023-06-27 07:46:04.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/background.js
+-rw-rw-rw-   0        0        0     1924 2023-06-27 07:46:04.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/manifest.json
+-rw-rw-rw-   0        0        0     6050 2023-06-17 13:56:27.000000 selenium_injector-2.1/src/selenium_injector/injector.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.1/src/selenium_injector/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7438 2023-06-27 07:15:26.000000 selenium_injector-2.1/src/selenium_injector/scripts/injector.py
+-rw-rw-rw-   0        0        0     1576 2023-06-20 10:58:22.000000 selenium_injector-2.1/src/selenium_injector/scripts/js.py
+-rw-rw-rw-   0        0        0     1742 2023-06-20 11:34:48.000000 selenium_injector-2.1/src/selenium_injector/scripts/socket.py
+-rw-rw-rw-   0        0        0     3804 2023-06-20 12:49:54.000000 selenium_injector-2.1/src/selenium_injector/scripts/sync_websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:26:36.000000 selenium_injector-2.1/src/selenium_injector/utils/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-06-20 11:35:20.000000 selenium_injector-2.1/src/selenium_injector/utils/utils.py
+-rw-rw-rw-   0        0        0     2040 2023-06-26 16:52:11.000000 selenium_injector-2.1/src/selenium_injector/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/
+-rw-rw-rw-   0        0        0     5124 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/top_level.txt
```

### Comparing `selenium_injector-2.0/LICENSE.md` & `selenium_injector-2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/PKG-INFO` & `selenium_injector-2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_injector
-Version: 2.0
+Version: 2.1
 Summary: inject javascript into chrome
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -51,78 +51,84 @@
 
 ### Example scripts
 
 
 #### click on element
 ```python
 from selenium_injector.webdriver import Chrome
+
+# base driver to use
 # from selenium.webdriver import Chrome as base_driver
 from undetected_chromedriver import Chrome as base_driver
 
-driver = Chrome(base_driver=base_driver)
+driver = Chrome(base_drivers=(base_driver,))
 
 driver.get("https://www.wikipedia.org/")
-driver.driverless.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.driverless.tab_user)
+driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
-js = driver.driverless.socket.js
+js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
 try:
     prev_url = driver.current_url[:]
-    driver.driverless.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.driverless.tab_user, timeout=2)
+    driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
-    # noinspection PyUnboundLocalVariable
     if driver.current_url != prev_url:
-        pass
+        pass # new page loaded before send_response
     else:
         raise e
 
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 #### set proxy dynamically
 ```python
 from selenium_injector.webdriver import Chrome
 driver = Chrome()
 
-driver.driverless.proxy.set(host="example_host.com", port=143, password="password", username="user-1")
+driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
-driver.driverless.proxy.clear()
+driver.injector.proxy.clear()
 driver.quit()
 ```
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
 - [ ] Add MV2 extension
   - [ ] change headers
 - [ ] add events
+  - [ ] make protocoll use `UUIDS`'s
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
-  - [x] manage locatiom api leak
+  - [x] manage location api leak
   - [ ] proxy per request
 - [ ] add `chrome.scripting` support
 - [ ] add automation tools
-  - [ ] click
+  - [x] click
   - [ ] send_keys
   - [ ] find_element
-    - [ ] by XPATH
+    - [x] by XPATH
+- [ ] undetectability
+  - [x] make tab scripts private
+  - [x] support base_driver argument
+  - [ ] make `/files/js/utils.js` private
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_injector-2.0/README.md` & `selenium_injector-2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,78 +21,84 @@
 
 ### Example scripts
 
 
 #### click on element
 ```python
 from selenium_injector.webdriver import Chrome
+
+# base driver to use
 # from selenium.webdriver import Chrome as base_driver
 from undetected_chromedriver import Chrome as base_driver
 
-driver = Chrome(base_driver=base_driver)
+driver = Chrome(base_drivers=(base_driver,))
 
 driver.get("https://www.wikipedia.org/")
-driver.driverless.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.driverless.tab_user)
+driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
-js = driver.driverless.socket.js
+js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
 try:
     prev_url = driver.current_url[:]
-    driver.driverless.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.driverless.tab_user, timeout=2)
+    driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
-    # noinspection PyUnboundLocalVariable
     if driver.current_url != prev_url:
-        pass
+        pass # new page loaded before send_response
     else:
         raise e
 
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 #### set proxy dynamically
 ```python
 from selenium_injector.webdriver import Chrome
 driver = Chrome()
 
-driver.driverless.proxy.set(host="example_host.com", port=143, password="password", username="user-1")
+driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
-driver.driverless.proxy.clear()
+driver.injector.proxy.clear()
 driver.quit()
 ```
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
 - [ ] Add MV2 extension
   - [ ] change headers
 - [ ] add events
+  - [ ] make protocoll use `UUIDS`'s
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
-  - [x] manage locatiom api leak
+  - [x] manage location api leak
   - [ ] proxy per request
 - [ ] add `chrome.scripting` support
 - [ ] add automation tools
-  - [ ] click
+  - [x] click
   - [ ] send_keys
   - [ ] find_element
-    - [ ] by XPATH
+    - [x] by XPATH
+- [ ] undetectability
+  - [x] make tab scripts private
+  - [x] support base_driver argument
+  - [ ] make `/files/js/utils.js` private
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_injector-2.0/build_upload.md` & `selenium_injector-2.1/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/setup.py` & `selenium_injector-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/files/extension/background.js` & `selenium_injector-2.1/src/selenium_injector/files/extension/background.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -29,27 +29,18 @@
         }
     }, 25000);
 }
 
 // chrome extension libs
 
 globalThis.proxy = {}
+proxy.credentials = {}
 
-proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true, bypass_list = ["localhost"]) {
-    proxy.config = {
-        mode: "fixed_servers",
-        rules: {
-            singleProxy: {
-                scheme: scheme,
-                host: host,
-                port: port
-            },
-            bypassList: bypass_list
-        }
-    };
+proxy.set = function(config, patch_webrtc = true, patch_location = true) {
+    proxy.config = config
     chrome.proxy.settings.set({
         value: proxy.config,
         scope: "regular"
     }, function() {});
     if (patch_webrtc) {
         webrtc_leak.disable();
     };
@@ -74,14 +65,20 @@
         contentsettings.set_location("allow")
     }
     delete(proxy.config)
 }
 
 
 proxy.set_auth = function(username, password, urls = ["<all_urls>"]) {
+    proxy.credentials = {
+        "password": password,
+        "username": username,
+        "urls": urls
+    };
+
     proxy.auth_call = function(details) {
         return {
             authCredentials: {
                 username: username,
                 password: password
             }
         };
@@ -91,14 +88,15 @@
             urls: urls
         },
         ['blocking']
     );
 }
 
 proxy.clear_auth = function(urls = ["<all_urls>"]) {
+    proxy.credentials = {};
     chrome.webRequest.onAuthRequired.removeListener(
         proxy.auth_call, {
             urls: urls
         },
         ['blocking']);
     delete(proxy.auth_call)
 }
```

### Comparing `selenium_injector-2.0/src/selenium_injector/files/extension/manifest.json` & `selenium_injector-2.1/src/selenium_injector/files/extension/manifest.json`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/files/js/connection.js` & `selenium_injector-2.1/src/selenium_injector/files/js/connection.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -49,14 +49,15 @@
     handler(request) {
         var request = JSON.parse(request);
         console.log({
             "request": request
         })
         this.not_return = request["not_return"]
         this.status = 200
+        var e = undefined
         try {
             var result = this.eval(request)
         } catch (e) {
             var result = {
                 "message": e.message,
                 "stack": e.stack
             };
```

### Comparing `selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/background.js` & `selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/background.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,27 +29,18 @@
         }
     }, 25000);
 }
 
 // chrome extension libs
 
 globalThis.proxy = {}
+proxy.credentials = {}
 
-proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true, bypass_list = ["localhost"]) {
-    proxy.config = {
-        mode: "fixed_servers",
-        rules: {
-            singleProxy: {
-                scheme: scheme,
-                host: host,
-                port: port
-            },
-            bypassList: bypass_list
-        }
-    };
+proxy.set = function(config, patch_webrtc = true, patch_location = true) {
+    proxy.config = config
     chrome.proxy.settings.set({
         value: proxy.config,
         scope: "regular"
     }, function() {});
     if (patch_webrtc) {
         webrtc_leak.disable();
     };
@@ -74,14 +65,20 @@
         contentsettings.set_location("allow")
     }
     delete(proxy.config)
 }
 
 
 proxy.set_auth = function(username, password, urls = ["<all_urls>"]) {
+    proxy.credentials = {
+        "password": password,
+        "username": username,
+        "urls": urls
+    };
+
     proxy.auth_call = function(details) {
         return {
             authCredentials: {
                 username: username,
                 password: password
             }
         };
@@ -91,14 +88,15 @@
             urls: urls
         },
         ['blocking']
     );
 }
 
 proxy.clear_auth = function(urls = ["<all_urls>"]) {
+    proxy.credentials = {};
     chrome.webRequest.onAuthRequired.removeListener(
         proxy.auth_call, {
             urls: urls
         },
         ['blocking']);
     delete(proxy.auth_call)
 }
@@ -181,14 +179,15 @@
     handler(request) {
         var request = JSON.parse(request);
         console.log({
             "request": request
         })
         this.not_return = request["not_return"]
         this.status = 200
+        var e = undefined
         try {
             var result = this.eval(request)
         } catch (e) {
             var result = {
                 "message": e.message,
                 "stack": e.stack
             };
@@ -363,9 +362,9 @@
             case "!=":
                 return a != b;
         }
         throw new Error("Can't apply operator " + op);
     }
 
 } //end connector class
-var connection = new connector("localhost", 53576, "selenium-injector-mv3")
+var connection = new connector("localhost", 55065, "selenium-injector-mv3")
 connection.connect();
```

### Comparing `selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/manifest.json` & `selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/manifest.json`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/injector.py` & `selenium_injector-2.1/src/selenium_injector/injector.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/scripts/driverless.py` & `selenium_injector-2.1/src/selenium_injector/scripts/injector.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,40 @@
         self.user = user
 
     def check_cmd(self, value, values):
         if value not in values:
             raise ValueError("Expected " + str(values) + " , but got" + str(value))
 
 
-class Driverless:
-    def __init__(self, port: int = None, host: str = None, user="selenium-injector-mv3"):
+class Injector:
+    def __init__(self, port: int = None, host: str = None, user="selenium-injector-mv3", temp_dir: str = None):
         from selenium_injector.scripts.socket import socket
         from selenium_injector.utils.utils import read, write, sel_injector_path, random_port
 
         if not host:
             host = "localhost"
         if not port:
             port = random_port(host=host)
 
         self.user = user
 
-        self.config = f"""
+        config = f"""
         var connection = new connector("{host}", {port}, "{self.user}")
         connection.connect();
         """
-        self.path = sel_injector_path() + "files/tmp/injector_extension"
+        if temp_dir:
+            self.path = temp_dir + "/injector_extension"
+        else:
+            self.path = sel_injector_path() + "files/tmp/injector_extension"
 
-        self.background_js = read("files/extension/background.js")
+        background_js = read("files/extension/background.js")
+        manifest_json = read("files/extension/manifest.json")
         self.connection_js = read("files/js/connection.js")
-        write(self.path + "/background.js", self.background_js + self.connection_js + self.config, sel_root=False)
+        write(self.path + "/background.js", background_js + self.connection_js + config, sel_root=False)
+        write(self.path + "/manifest.json", manifest_json, sel_root=False)
 
         self.socket = socket()
         self.socket.start(port=port, host=host)
         self.stop = self.socket.stop
         self.exec = self.socket.exec
         self.exec_command = self.socket.exec_command
 
@@ -40,55 +45,75 @@
         self.proxy = self.proxy(socket=self.socket, user=self.user)
         self.webrtc_leak = self.webrtc_leak(socket=self.socket, user=self.user)
         self.contentsettings = self.contentsettings(socket=self.socket, user=self.user)
         self.tabs = self.tabs(socket=self.socket, user=self.user)
 
     @property
     def page_source(self):
-        return self.socket.exec(self.socket.js.types.path("document.documentElement.outerHTML"), user="tab-0")["result"][0]
+        return \
+            self.socket.exec(self.socket.js.types.path("document.documentElement.outerHTML"), user="tab-0")["result"][0]
 
     class proxy(base_driver):
         def __init__(self, socket, user):
             self.supported_schemes = ["http", "https", "socks4", "socks5"]
             super().__init__(socket, user=user)
 
         @property
         def rules(self):
             try:
-                return self.socket.exec_command("proxy.get",user=self.user)["result"][0]["value"]["rules"]
+                return self.socket.exec_command("proxy.get", user=self.user)["result"][0]["value"]["rules"]
             except KeyError:
                 return None
 
         @property
         def mode(self):
-            return self.socket.exec_command("proxy.get",user=self.user)["result"][0]["value"]["mode"]
+            return self.socket.exec_command("proxy.get", user=self.user)["result"][0]["value"]["mode"]
+
+        @property
+        def auth(self):
+            return self.socket.exec(self.socket.js.types.path("proxy.credentials"))["result"][0]
+
+        def set(self, config, patch_webrtc: bool = True, patch_location: bool = True):
+            self.socket.exec_command("proxy.set", [config, patch_webrtc, patch_location],
+                                     timeout=10, user=self.user)
 
         # noinspection PyDefaultArgument
-        def set(self, host: str, port: int, scheme: str = "http", patch_webrtc: bool = True,
-                patch_location: bool = True, bypass_list: list = ["localhost"],
-                username: str = None, password: str = None,
-                timeout=10):
+        def set_single(self, host: str, port: int, scheme: str = "http", bypass_list=["localhost", "127.0.0.1"], patch_webrtc: bool = True,
+                       patch_location: bool = True,
+                       username: str = None, password: str = None,
+                       timeout=10):
 
             self.check_cmd(scheme, self.supported_schemes)
             # auth
             if username and password:
-                timeout = int(timeout / 2)
+                timeout = int(timeout / 3)
+                if self.auth:
+                    self.clear_auth(timeout=timeout)
                 self.set_auth(username=username, password=password, timeout=timeout)
             elif username or password:
                 raise ValueError("For authentification, username and password need to get specified, only got one")
 
-            self.socket.exec_command("proxy.set", [scheme, host, port, patch_webrtc, patch_location, bypass_list],
-                                     timeout=10, user=self.user)
+            config = {"mode": "fixed_servers", "rules": {
+                "singleProxy": {"host": host, "port": port, "scheme": scheme},
+                "bypassList": bypass_list
+            }}
+
+            self.set(config=config, patch_webrtc=patch_webrtc, patch_location=patch_location)
 
         # noinspection PyDefaultArgument
         def set_auth(self, username: str, password: str, urls=["<all_urls>"], timeout=10):
             self.socket.exec_command("proxy.set_auth", [username, password, urls], timeout=timeout, user=self.user)
 
+        # noinspection PyDefaultArgument
+        def clear_auth(self,urls=["<all_urls>"], timeout=10):
+            self.socket.exec_command("proxy.clear_auth", [urls], timeout=timeout, user=self.user)
+
         def clear(self, clear_webrtc=True, clear_location=True, timeout=10):
-            self.socket.exec_command("proxy.clear", [clear_webrtc, clear_location], timeout=timeout, user=self.user)
+            self.socket.exec_command("proxy.clear", [clear_webrtc, clear_location], timeout=int(timeout/2), user=self.user)
+            self.clear_auth(timeout=int(timeout/2))
 
     class webrtc_leak(base_driver):
         def __init__(self, socket, user):
             self.supported_values = ["default", "default_public_and_private_interfaces",
                                      "default_public_interface_only", "disable_non_proxied_udp"]
             super().__init__(socket, user)
```

### Comparing `selenium_injector-2.0/src/selenium_injector/scripts/js.py` & `selenium_injector-2.1/src/selenium_injector/scripts/js.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/scripts/socket.py` & `selenium_injector-2.1/src/selenium_injector/scripts/socket.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/scripts/sync_websocket.py` & `selenium_injector-2.1/src/selenium_injector/scripts/sync_websocket.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector/utils/utils.py` & `selenium_injector-2.1/src/selenium_injector/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.0/src/selenium_injector.egg-info/PKG-INFO` & `selenium_injector-2.1/src/selenium_injector.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-injector
-Version: 2.0
+Version: 2.1
 Summary: inject javascript into chrome
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -51,78 +51,84 @@
 
 ### Example scripts
 
 
 #### click on element
 ```python
 from selenium_injector.webdriver import Chrome
+
+# base driver to use
 # from selenium.webdriver import Chrome as base_driver
 from undetected_chromedriver import Chrome as base_driver
 
-driver = Chrome(base_driver=base_driver)
+driver = Chrome(base_drivers=(base_driver,))
 
 driver.get("https://www.wikipedia.org/")
-driver.driverless.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.driverless.tab_user)
+driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
-js = driver.driverless.socket.js
+js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
 try:
     prev_url = driver.current_url[:]
-    driver.driverless.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.driverless.tab_user, timeout=2)
+    driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
-    # noinspection PyUnboundLocalVariable
     if driver.current_url != prev_url:
-        pass
+        pass # new page loaded before send_response
     else:
         raise e
 
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 #### set proxy dynamically
 ```python
 from selenium_injector.webdriver import Chrome
 driver = Chrome()
 
-driver.driverless.proxy.set(host="example_host.com", port=143, password="password", username="user-1")
+driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
-driver.driverless.proxy.clear()
+driver.injector.proxy.clear()
 driver.quit()
 ```
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
 - [ ] Add MV2 extension
   - [ ] change headers
 - [ ] add events
+  - [ ] make protocoll use `UUIDS`'s
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
-  - [x] manage locatiom api leak
+  - [x] manage location api leak
   - [ ] proxy per request
 - [ ] add `chrome.scripting` support
 - [ ] add automation tools
-  - [ ] click
+  - [x] click
   - [ ] send_keys
   - [ ] find_element
-    - [ ] by XPATH
+    - [x] by XPATH
+- [ ] undetectability
+  - [x] make tab scripts private
+  - [x] support base_driver argument
+  - [ ] make `/files/js/utils.js` private
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_injector-2.0/src/selenium_injector.egg-info/SOURCES.txt` & `selenium_injector-2.1/src/selenium_injector.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 src/selenium_injector.egg-info/requires.txt
 src/selenium_injector.egg-info/top_level.txt
 src/selenium_injector/files/extension/background.js
 src/selenium_injector/files/extension/manifest.json
 src/selenium_injector/files/js/connection.js
 src/selenium_injector/files/js/utils.js
 src/selenium_injector/files/tmp/injector_extension/background.js
-src/selenium_injector/files/tmp/injector_extension/content_helper.js
 src/selenium_injector/files/tmp/injector_extension/manifest.json
 src/selenium_injector/scripts/__init__.py
-src/selenium_injector/scripts/driverless.py
+src/selenium_injector/scripts/injector.py
 src/selenium_injector/scripts/js.py
 src/selenium_injector/scripts/socket.py
 src/selenium_injector/scripts/sync_websocket.py
 src/selenium_injector/utils/__init__.py
 src/selenium_injector/utils/utils.py
```

