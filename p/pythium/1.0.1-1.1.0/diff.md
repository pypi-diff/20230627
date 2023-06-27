# Comparing `tmp/pythium-1.0.1.tar.gz` & `tmp/pythium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bo.liu/Work/pythium/dist/tmpn2lii5zx/pythium-1.0.1.tar", last modified: Wed Nov 16 06:18:05 2022, max compression
+gzip compressed data, was "/Users/bo.liu/Work/pythium/dist/tmpl5q0z6ew/pythium-1.1.0.tar", last modified: Tue Jun 27 05:14:25 2023, max compression
```

## Comparing `pythium-1.0.1.tar` & `pythium-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2022-11-16 06:18:05.207368 pythium-1.0.1/
--rw-r--r--   0 bo.liu     (505) staff       (20)     4540 2022-11-16 06:18:05.206966 pythium-1.0.1/PKG-INFO
--rw-r--r--   0 bo.liu     (505) staff       (20)     3031 2022-11-16 06:14:15.000000 pythium-1.0.1/README.md
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2022-11-16 06:18:05.203748 pythium-1.0.1/pythium/
--rw-r--r--   0 bo.liu     (505) staff       (20)      261 2022-11-16 06:09:03.000000 pythium-1.0.1/pythium/__init__.py
--rw-r--r--   0 bo.liu     (505) staff       (20)     7249 2022-11-16 06:09:03.000000 pythium-1.0.1/pythium/_impl.py
-drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2022-11-16 06:18:05.206479 pythium-1.0.1/pythium.egg-info/
--rw-r--r--   0 bo.liu     (505) staff       (20)     4540 2022-11-16 06:18:05.000000 pythium-1.0.1/pythium.egg-info/PKG-INFO
--rw-r--r--   0 bo.liu     (505) staff       (20)      239 2022-11-16 06:18:05.000000 pythium-1.0.1/pythium.egg-info/SOURCES.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        1 2022-11-16 06:18:05.000000 pythium-1.0.1/pythium.egg-info/dependency_links.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        1 2022-11-16 06:18:04.000000 pythium-1.0.1/pythium.egg-info/not-zip-safe
--rw-r--r--   0 bo.liu     (505) staff       (20)       42 2022-11-16 06:18:05.000000 pythium-1.0.1/pythium.egg-info/requires.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)        8 2022-11-16 06:18:05.000000 pythium-1.0.1/pythium.egg-info/top_level.txt
--rw-r--r--   0 bo.liu     (505) staff       (20)       38 2022-11-16 06:18:05.207477 pythium-1.0.1/setup.cfg
--rw-r--r--   0 bo.liu     (505) staff       (20)     1219 2022-11-16 06:17:42.000000 pythium-1.0.1/setup.py
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.656953 pythium-1.1.0/
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-06-27 05:14:25.656597 pythium-1.1.0/PKG-INFO
+-rw-r--r--   0 bo.liu     (505) staff       (20)     3036 2022-11-16 09:06:52.000000 pythium-1.1.0/README.md
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.653686 pythium-1.1.0/pythium/
+-rw-r--r--   0 bo.liu     (505) staff       (20)      359 2023-03-07 01:14:33.000000 pythium-1.1.0/pythium/__init__.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     5878 2023-03-08 06:11:02.000000 pythium-1.1.0/pythium/_impl.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     9748 2023-04-24 06:43:07.000000 pythium-1.1.0/pythium/actions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     5793 2022-12-12 07:51:54.000000 pythium-1.1.0/pythium/assertions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     3806 2023-03-08 09:25:12.000000 pythium-1.1.0/pythium/commands.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)      249 2022-01-21 07:11:16.000000 pythium-1.1.0/pythium/exceptions.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4007 2023-06-27 02:12:03.000000 pythium-1.1.0/pythium/http_session.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     8973 2023-06-27 00:56:23.000000 pythium-1.1.0/pythium/objects.py
+-rw-r--r--   0 bo.liu     (505) staff       (20)     2599 2022-12-12 01:49:47.000000 pythium-1.1.0/pythium/utils.py
+drwxr-xr-x   0 bo.liu     (505) staff       (20)        0 2023-06-27 05:14:25.656059 pythium-1.1.0/pythium.egg-info/
+-rw-r--r--   0 bo.liu     (505) staff       (20)     4553 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/PKG-INFO
+-rw-r--r--   0 bo.liu     (505) staff       (20)      382 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/SOURCES.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/dependency_links.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        1 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/not-zip-safe
+-rw-r--r--   0 bo.liu     (505) staff       (20)      119 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/requires.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)        8 2023-06-27 05:14:25.000000 pythium-1.1.0/pythium.egg-info/top_level.txt
+-rw-r--r--   0 bo.liu     (505) staff       (20)       38 2023-06-27 05:14:25.657079 pythium-1.1.0/setup.cfg
+-rw-r--r--   0 bo.liu     (505) staff       (20)     1339 2023-06-27 02:15:25.000000 pythium-1.1.0/setup.py
```

### Comparing `pythium-1.0.1/PKG-INFO` & `pythium-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythium
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python based Page Factory.
 Home-page: https://github.com/lucas234/pythium
 Author: lucas
 Author-email: ly_liubo@163.com
 License: MIT
-Description: #### Pyium 
+Description: #### Pythium 
         ***
         Python based Page Factory design pattern test library, similar to Java's Page Factory pattern, 
         designed to reduce code redundancy, easy to use, are very descriptive， make the code more 
         readable and understandable and with a high degree of scalability.
         
         - Supports locate element with annotation
         - Supports multiple positioning methods for the same element
@@ -69,15 +69,15 @@
         
         if __name__ == '__main__':
             from selenium import webdriver
         
             driver = webdriver.Chrome()
             login = LoginPage(driver)
             # no @property
-            login.search_input.click()
+            login.search_input().click()
             # with @property
             login.search_input_with_property.click()
             # for dynamical locator
             login.dynamical_locator(2, 3, 4, 5).click()
             # for list WebElement
             print(len(login.list_web_elements()))
         ```
@@ -88,14 +88,15 @@
         
         example: `@find_all(by(css=".icon-logo1"), by(id="icon"))` 
         
         first will find element `by(css=".icon-logo1")`, if found, return `WebElement`; 
         
         if not found, will find element `by(id="icon")`, if found, return `WebElement`, if not found, will raise `Exception`.
          
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pythium-1.0.1/README.md` & `pythium-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#### Pyium 
+#### Pythium 
 ***
 Python based Page Factory design pattern test library, similar to Java's Page Factory pattern, 
 designed to reduce code redundancy, easy to use, are very descriptive， make the code more 
 readable and understandable and with a high degree of scalability.
 
 - Supports locate element with annotation
 - Supports multiple positioning methods for the same element
@@ -61,15 +61,15 @@
 
 if __name__ == '__main__':
     from selenium import webdriver
 
     driver = webdriver.Chrome()
     login = LoginPage(driver)
     # no @property
-    login.search_input.click()
+    login.search_input().click()
     # with @property
     login.search_input_with_property.click()
     # for dynamical locator
     login.dynamical_locator(2, 3, 4, 5).click()
     # for list WebElement
     print(len(login.list_web_elements()))
 ```
@@ -79,8 +79,8 @@
 given that at least one criteria match. it uses an OR conditional relationship between the multiple `@xxx_find_by`.
 
 example: `@find_all(by(css=".icon-logo1"), by(id="icon"))` 
 
 first will find element `by(css=".icon-logo1")`, if found, return `WebElement`; 
 
 if not found, will find element `by(id="icon")`, if found, return `WebElement`, if not found, will raise `Exception`.
- 
+
```

### Comparing `pythium-1.0.1/pythium/_impl.py` & `pythium-1.1.0/pythium/_impl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,96 @@
 # @Project: pythium
 # @Author：Lucas Liu
 # @Time: 2022/10/28 9:15 AM
-from appium.webdriver.common.appiumby import AppiumBy
-from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from functools import wraps
-from selenium.webdriver.remote.webdriver import WebDriver
 from appium.webdriver.webdriver import WebDriver as MobileDriver
-from typing import Union, List, Callable, Any
+from typing import Union, Callable, Any
 import inspect
 from abc import abstractmethod
+from selenium.webdriver.remote.webdriver import WebDriver
+from typing import List
 from selenium.webdriver.remote.webelement import WebElement
 from appium.webdriver.webelement import WebElement as MobileElement
-
-
-_LOCATORS = {
-            # selenium locators
-            'css': By.CSS_SELECTOR,
-            'id_': By.ID,
-            'name': By.NAME,
-            'xpath': By.XPATH,
-            'link_text': By.LINK_TEXT,
-            'partial_link_text': By.PARTIAL_LINK_TEXT,
-            'tag_name': By.TAG_NAME,
-            'class_name': By.CLASS_NAME,
-            # appium locators
-            "ios_predicate": AppiumBy.IOS_PREDICATE,
-            "ios_uiautomation": AppiumBy.IOS_UIAUTOMATION,
-            "ios_class_chain": AppiumBy.IOS_CLASS_CHAIN,
-            "android_uiautomator": AppiumBy.ANDROID_UIAUTOMATOR,
-            "android_viewtag": AppiumBy.ANDROID_VIEWTAG,
-            "android_data_matcher": AppiumBy.ANDROID_DATA_MATCHER,
-            "android_view_matcher": AppiumBy.ANDROID_VIEW_MATCHER,
-            # Deprecated
-            "windows_ui_automation": AppiumBy.WINDOWS_UI_AUTOMATION,
-            "accessibility_id": AppiumBy.ACCESSIBILITY_ID,
-            "image": AppiumBy.IMAGE,
-            "custom": AppiumBy.CUSTOM,
-            }
-
-
-def _get_kwargs():
-    frame = inspect.currentframe().f_back
-    keys, _, _, values = inspect.getargvalues(frame)
-    kwargs = {}
-    for key in keys:
-        if key != 'self':
-            kwargs[key] = values[key]
-    return kwargs
-
-
-def _valid_locator(_kwargs):
-    if len(_kwargs) != 1:
-        raise Exception("Only support one locate strategy, please have a check!")
-    (k, v), = _kwargs.items()
-    if k not in _LOCATORS.keys():
-        raise Exception(f"NotSupport({k}='{v}'), Only support the following locators: {list(_LOCATORS.keys())}")
-    locator = (_LOCATORS[k], v)
-    return locator
-
-
-def _get_func_kwargs(args_, kwargs_, func):
-    default_kwargs = inspect.signature(func).parameters
-    keys = list(default_kwargs.keys())[1:]
-    if len(args_) == len(keys):
-        return dict(zip(list(keys), args_))
-    if len(kwargs_) == len(keys):
-        return kwargs_
-    default_keys = keys[len(args_):]
-    default_keys = [i for i in default_keys if i not in kwargs_]
-    new_kwargs_ = dict(zip(list(keys), args_))
-    for key in default_keys:
-        new_kwargs_[key] = default_kwargs.get(key).default
-    kwargs_.update(new_kwargs_)
-    return kwargs_
+from pythium.objects import Element, Elements
+from pythium.actions import Actions
+from pythium.utils import Utils
+from pythium.assertions import PageAssertions
+from pythium.http_session import HttpSession
 
 
 def _handle_return_type(return_type, driver: WebDriver, locator):
     if return_type in [List[WebElement], List[MobileElement]]:
-        return driver.find_elements(*locator)
+        return driver.find_elements(*locator[0])
     elif return_type in [WebElement, MobileElement]:
-        return driver.find_element(*locator)
+        return driver.find_element(*locator[0])
+    elif issubclass(return_type, Element) or issubclass(return_type, Elements):
+        return return_type(**locator[1], driver=driver)
     else:
-        raise Exception("Only support the WebElement and [WebElement]!")
+        raise Exception("Only support the WebElement, [WebElement], Element and Elements!")
 
 
 def find_by(id_=None, css=None, name=None, xpath=None, partial_link_text=None,
             link_text=None, class_name=None, tag_name=None) -> Callable[[], Any]:
     """ find webElement by locator(selenium)"""
-    _locators = {k: v for k, v in _get_kwargs().items() if v}
-    _by, value = _valid_locator(_locators)
+    _locators = {k: v for k, v in Utils.get_kwargs().items() if v}
+    _by, value, key = Utils.valid_locator(_locators)
 
     def decorator(func):
         @wraps(func)
         def wrapped_func(*args, **kwargs):
-            func_kwargs = _get_func_kwargs(args[1:], kwargs, func)
-            locator = (_by, value.format(**func_kwargs))
-            browser_name = args[0].driver.capabilities.get('browserName')
-            device_name = args[0].driver.capabilities.get('deviceName')
-            browsers = ['chrome', 'firefox', 'safari', 'ie', 'edge', 'opera']
-            if not device_name and browser_name.lower() in browsers:
-                args[0].locators[func.__name__] = locator
+            func_kwargs = Utils.get_func_kwargs(args[1:], kwargs, func)
+            locator = (_by, value.format(**func_kwargs)), {key: value}
+            if args[0].action.is_web_platform:
+                args[0].locators[func.__name__] = locator[0]
                 return_type = inspect.signature(func).return_annotation
                 return _handle_return_type(return_type, args[0].driver, locator)
             else:
                 return func(*args, **kwargs)
         return wrapped_func
     return decorator
 
 
-def _find_by(platform):
-    def __find_by(id_=None, css=None, name=None, xpath=None, partial_link_text=None,
-                  link_text=None, class_name=None, tag_name=None, ios_predicate=None,
-                  android_uiautomator=None, android_viewtag=None, android_data_matcher=None,
-                  android_view_matcher=None, windows_ui_automation=None, accessibility_id=None,
-                  ios_uiautomation=None, ios_class_chain=None, image=None, custom=None) -> Callable[[], Any]:
+def _appium_find_by(platform):
+    def _find_by(id_=None, css=None, name=None, xpath=None, partial_link_text=None,
+                 link_text=None, class_name=None, tag_name=None, ios_predicate=None,
+                 android_uiautomator=None, android_viewtag=None, android_data_matcher=None,
+                 android_view_matcher=None, windows_ui_automation=None, accessibility_id=None,
+                 ios_uiautomation=None, ios_class_chain=None, image=None, custom=None) -> Callable[[], Any]:
         """ find mobileElement by locator(appium)"""
-        _locators = {k: v for k, v in _get_kwargs().items() if v}
-        locator = _valid_locator(_locators)
+        _locators = {k: v for k, v in Utils.get_kwargs().items() if v}
+        _by, value, key = Utils.valid_locator(_locators)
 
         def decorator(func):
             @wraps(func)
             def wrapped_func(*args, **kwargs):
-                platform_name = args[0].driver.capabilities.get('platformName')
-                if platform_name.lower() == platform.lower():
-                    args[0].locators[func.__name__] = locator
-                    return args[0].driver.find_element(*locator)
+                func_kwargs = Utils.get_func_kwargs(args[1:], kwargs, func)
+                locator = (_by, value.format(**func_kwargs)), {key: value}
+                if args[0].action.is_platform(platform):
+                    args[0].locators[func.__name__] = locator[0]
+                    return_type = inspect.signature(func).return_annotation
+                    return _handle_return_type(return_type, args[0].driver, locator)
                 else:
                     return func(*args, **kwargs)
             return wrapped_func
         return decorator
-    return __find_by
+    return _find_by
 
 
-ios_find_by = _find_by(platform="ios")
-android_find_by = _find_by(platform="android")
+ios_find_by = _appium_find_by('ios')
+android_find_by = _appium_find_by('android')
 
 
 def by(id_=None, css=None, name=None, xpath=None, partial_link_text=None,
        link_text=None, class_name=None, tag_name=None, image=None, custom=None,
        android_uiautomator=None, android_viewtag=None, android_data_matcher=None,
        android_view_matcher=None, windows_ui_automation=None, accessibility_id=None,
        ios_uiautomation=None, ios_class_chain=None, ios_predicate=None):
-    _locators = {k: v for k, v in _get_kwargs().items() if v}
-    _valid_locator(_locators)
+    _locators = {k: v for k, v in Utils.get_kwargs().items() if v}
+    Utils.valid_locator(_locators)
     return _locators
 
 
 def _find_all(by_: Union[find_by, ios_find_by, android_find_by]):
     def __find_all(*strategies: by):
         """ find webElement by chain"""
         def decorator(func):
@@ -174,16 +117,35 @@
 android_find_all = _find_all(android_find_by)
 
 
 class Page:
     def __init__(self, driver_: Union[MobileDriver, WebDriver]):
         self.driver = driver_
         self.locators = {}
+        self.action = Actions(self.driver)
+
+    @abstractmethod
+    def _is_loaded(self):
+        pass
 
     def goto(self, url):
         self.driver.get(url)
         return self
 
-    @abstractmethod
-    def _is_loaded(self):
-        pass
+    def open_deeplink(self, link, ios_bundle_id=None):
+        self.action.open_deep_link(link, ios_bundle_id)
+        return self
+
+    @property
+    def expect(self) -> PageAssertions:
+        return PageAssertions(self.driver)
+
+    @property
+    def request(self):
+        session = HttpSession()
+        session.cookies.update(self._get_cookies())
+        return session
+
+    def _get_cookies(self) -> dict:
+        cookies = {cookie['name']: cookie['value'] for cookie in self.driver.get_cookies()}
+        return cookies
```

### Comparing `pythium-1.0.1/pythium.egg-info/PKG-INFO` & `pythium-1.1.0/pythium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythium
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python based Page Factory.
 Home-page: https://github.com/lucas234/pythium
 Author: lucas
 Author-email: ly_liubo@163.com
 License: MIT
-Description: #### Pyium 
+Description: #### Pythium 
         ***
         Python based Page Factory design pattern test library, similar to Java's Page Factory pattern, 
         designed to reduce code redundancy, easy to use, are very descriptive， make the code more 
         readable and understandable and with a high degree of scalability.
         
         - Supports locate element with annotation
         - Supports multiple positioning methods for the same element
@@ -69,15 +69,15 @@
         
         if __name__ == '__main__':
             from selenium import webdriver
         
             driver = webdriver.Chrome()
             login = LoginPage(driver)
             # no @property
-            login.search_input.click()
+            login.search_input().click()
             # with @property
             login.search_input_with_property.click()
             # for dynamical locator
             login.dynamical_locator(2, 3, 4, 5).click()
             # for list WebElement
             print(len(login.list_web_elements()))
         ```
@@ -88,14 +88,15 @@
         
         example: `@find_all(by(css=".icon-logo1"), by(id="icon"))` 
         
         first will find element `by(css=".icon-logo1")`, if found, return `WebElement`; 
         
         if not found, will find element `by(id="icon")`, if found, return `WebElement`, if not found, will raise `Exception`.
          
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pythium-1.0.1/setup.py` & `pythium-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythium",
-    version="1.0.1",
+    version="1.1.0",
     author="lucas",
     author_email="ly_liubo@163.com",
     description="Python based Page Factory.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lucas234/pythium",
     zip_safe=False,
     license='MIT',
     install_requires=[
         'selenium==4.1',
         'Appium-Python-Client==2.7.1',
+        'retrying==1.3.4',
+        'requests==2.31.0',
+        'allure-python-commons==2.9.43',
+        'loguru==0.5.3'
     ],
     packages=['pythium'],
     python_requires=">=3",
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
```

