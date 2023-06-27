# Comparing `tmp/login_gmail_selenium-1.1.9.tar.gz` & `tmp/login_gmail_selenium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\login_gmail_selenium-1.1.9.tar", last modified: Thu Jun 15 03:51:26 2023, max compression
+gzip compressed data, was "dist\login_gmail_selenium-1.2.0.tar", last modified: Tue Jun 27 08:07:57 2023, max compression
```

## Comparing `login_gmail_selenium-1.1.9.tar` & `login_gmail_selenium-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.250870 login_gmail_selenium-1.1.9/
--rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     2380 2023-06-15 03:51:26.249872 login_gmail_selenium-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-03-07 08:43:52.000000 login_gmail_selenium-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:25.943691 login_gmail_selenium-1.1.9/login_gmail_selenium/
--rw-rw-rw-   0        0        0       42 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.057386 login_gmail_selenium-1.1.9/login_gmail_selenium/common/
--rw-rw-rw-   0        0        0       24 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-06-14 09:30:06.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/constant.py
--rw-rw-rw-   0        0        0      628 2023-02-27 08:57:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/log.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.165100 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/
--rw-rw-rw-   0        0        0    38852 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/always_active.zip
--rw-rw-rw-   0        0        0     5260 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/fingerprint_defender.zip
--rw-rw-rw-   0        0        0   120399 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/spoof_timezone.zip
--rw-rw-rw-   0        0        0  5601639 2023-03-14 08:09:16.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/veepn.zip
--rw-rw-rw-   0        0        0    45183 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/webrtc_control.zip
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.227931 login_gmail_selenium-1.1.9/login_gmail_selenium/util/
--rw-rw-rw-   0        0        0       45 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/__init__.py
--rw-rw-rw-   0        0        0      706 2023-03-24 10:39:03.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/driver.py
--rw-rw-rw-   0        0        0     4719 2023-03-24 08:28:57.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/helper.py
--rw-rw-rw-   0        0        0    17155 2023-06-15 01:30:52.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/profile.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.016497 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 03:51:26.250870 login_gmail_selenium-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-06-15 03:51:23.000000 login_gmail_selenium-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.247879 login_gmail_selenium-1.1.9/test/
--rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.1.9/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:57.067986 login_gmail_selenium-1.2.0/
+-rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-06-27 08:07:57.066991 login_gmail_selenium-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2104 2023-06-27 07:43:39.000000 login_gmail_selenium-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:56.919384 login_gmail_selenium-1.2.0/login_gmail_selenium/
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:56.971244 login_gmail_selenium-1.2.0/login_gmail_selenium/common/
+-rw-rw-rw-   0        0        0       24 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/common/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/common/constant.py
+-rw-rw-rw-   0        0        0      628 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/common/log.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:57.057016 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/
+-rw-rw-rw-   0        0        0    38852 2023-06-27 08:04:25.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/always_active.zip
+-rw-rw-rw-   0        0        0     5260 2023-06-27 08:04:25.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/fingerprint_defender.zip
+-rw-rw-rw-   0        0        0   120399 2023-06-27 08:04:25.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/spoof_timezone.zip
+-rw-rw-rw-   0        0        0  5601639 2023-06-27 08:04:25.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/veepn.zip
+-rw-rw-rw-   0        0        0    45183 2023-06-27 08:04:25.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/extension/webrtc_control.zip
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:57.061005 login_gmail_selenium-1.2.0/login_gmail_selenium/util/
+-rw-rw-rw-   0        0        0       46 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/base_profile.py
+-rw-rw-rw-   0        0        0      706 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/driver.py
+-rw-rw-rw-   0        0        0     4723 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:57.064995 login_gmail_selenium-1.2.0/login_gmail_selenium/util/profiles/
+-rw-rw-rw-   0        0        0       73 2023-06-27 08:06:20.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/profiles/__init__.py
+-rw-rw-rw-   0        0        0     8899 2023-06-27 08:02:46.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/profiles/google_profile.py
+-rw-rw-rw-   0        0        0      479 2023-06-27 08:01:29.000000 login_gmail_selenium-1.2.0/login_gmail_selenium/util/profiles/profile.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:56.967290 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-06-27 08:07:56.000000 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2023-06-27 08:07:56.000000 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:07:56.000000 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-27 08:07:56.000000 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 08:07:56.000000 login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:07:57.067986 login_gmail_selenium-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-06-27 08:04:37.000000 login_gmail_selenium-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:07:57.065992 login_gmail_selenium-1.2.0/test/
+-rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.2.0/test/test.py
```

### Comparing `login_gmail_selenium-1.1.9/LICENSE` & `login_gmail_selenium-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/PKG-INFO` & `login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: login_gmail_selenium
-Version: 1.1.9
+Name: login-gmail-selenium
+Version: 1.2.0
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -32,17 +32,19 @@
 
 ## Usage
 ```pycon
 pip install login_gmail_selenium
 ```
 And then on example.py
 ```pycon
-from login_gmail_selenium.util.profile import ChromeProfile
+from login_gmail_selenium.util.profiles.profile import GoogleProfile
+from login_gmail_selenium.util.profiles.google_profile import Profile
 
-profile = ChromeProfile(email, password, backup_email)
+profile = GoogleProfile(email, password, backup_email)
+# profile = Profile(name_profile) If don't need login to google but save driver
 # To allow downloads add insecure=True to ChromeProfile
 # To handle false email with custom functions, use param false_email_callback
 driver = profile.retrieve_driver()
 profile.start()
 # Do whatever with driver afterward
 driver.get('https://www.google.com/')
 driver.quit()
@@ -52,14 +54,17 @@
 2. The temp folder's content will be generated by the library.
 Your folder should look like this
 ```cvs
 /temp
     /profiles
         /profile1
         /profile2
+    /blank_profiles
+        /blank_profiles1
+        /blank_profiles2
 /extension
     /custom_extension
         extension1.zip
         extension2.crx
 example.py
 ```
```

### Comparing `login_gmail_selenium-1.1.9/README.md` & `login_gmail_selenium-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 
 ## Usage
 ```pycon
 pip install login_gmail_selenium
 ```
 And then on example.py
 ```pycon
-from login_gmail_selenium.util.profile import ChromeProfile
+from login_gmail_selenium.util.profiles.profile import GoogleProfile
+from login_gmail_selenium.util.profiles.google_profile import Profile
 
-profile = ChromeProfile(email, password, backup_email)
+profile = GoogleProfile(email, password, backup_email)
+# profile = Profile(name_profile) If don't need login to google but save driver
 # To allow downloads add insecure=True to ChromeProfile
 # To handle false email with custom functions, use param false_email_callback
 driver = profile.retrieve_driver()
 profile.start()
 # Do whatever with driver afterward
 driver.get('https://www.google.com/')
 driver.quit()
@@ -37,14 +39,17 @@
 2. The temp folder's content will be generated by the library.
 Your folder should look like this
 ```cvs
 /temp
     /profiles
         /profile1
         /profile2
+    /blank_profiles
+        /blank_profiles1
+        /blank_profiles2
 /extension
     /custom_extension
         extension1.zip
         extension2.crx
 example.py
 ```
```

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/common/constant.py` & `login_gmail_selenium-1.2.0/login_gmail_selenium/common/constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 WIDE_WAIT = [1, 10]
 PASTE_PERCENTAGE = 50
 DISK_SPACE = 80.0
 CHANGED_PASSWORD_SEPARATOR = '::::'
 PASSWORD_LENGTH = 25
 ACCOUNT_DISABLED_MESSAGE = 'Account disabled'
 ACCOUNT_VERIFICATION_MESSAGE = 'Account required verification steps'
-ACCOUNT_REQUIRED_CAPTCHA = 'Account required captcha'
+ACCOUNT_REQUIRED_CAPTCHA_MESSAGE = 'Account required captcha'
 ACCOUNT_REJECTED_MESSAGE = 'Account rejected because of suspicious action'
+ACCOUNT_PASSWORD_CHANGED_MESSAGE = 'Password changed'
 
 
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except (Exception, SyntaxError):
         base_path = os.path.abspath(".")
@@ -35,12 +36,13 @@
 
 
 # NOTE: Configuration
 CWD = resource_path("")
 TEMP_FOLDER = resource_path("temp")
 os.makedirs(TEMP_FOLDER, exist_ok=True)
 LOG_FILE = os.path.join(TEMP_FOLDER, 'output.log')
-PROFILE_FOLDER = os.path.join(TEMP_FOLDER, 'profiles')
+PROFILE_GOOGLE_FOLDER = os.path.join(TEMP_FOLDER, 'profiles')
+BLANK_PROFILE_FOLDER = os.path.join(TEMP_FOLDER, 'blank_profiles')
 PATCHED_DRIVER = os.path.join(TEMP_FOLDER, 'chromedriver.exe')
 CHANGED_EMAILS_FILE = os.path.join(TEMP_FOLDER, 'changed_emails.log')
 FALSE_EMAIL_FILE = os.path.join(TEMP_FOLDER, 'false_email.log')
 PROXY_FOLDER = os.path.join(TEMP_FOLDER, 'proxy')
```

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/common/log.py` & `login_gmail_selenium-1.2.0/login_gmail_selenium/common/log.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/always_active.zip` & `login_gmail_selenium-1.2.0/login_gmail_selenium/extension/always_active.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/fingerprint_defender.zip` & `login_gmail_selenium-1.2.0/login_gmail_selenium/extension/fingerprint_defender.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/spoof_timezone.zip` & `login_gmail_selenium-1.2.0/login_gmail_selenium/extension/spoof_timezone.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/veepn.zip` & `login_gmail_selenium-1.2.0/login_gmail_selenium/extension/veepn.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/webrtc_control.zip` & `login_gmail_selenium-1.2.0/login_gmail_selenium/extension/webrtc_control.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/util/driver.py` & `login_gmail_selenium-1.2.0/login_gmail_selenium/util/driver.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium/util/helper.py` & `login_gmail_selenium-1.2.0/login_gmail_selenium/util/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import random
 import math
 import os
-import login_gmail_selenium.common.constant as Constant
-from selenium.webdriver.common.keys import Keys
-from selenium.common.exceptions import TimeoutException, NoSuchElementException
-from selenium.webdriver.common.by import By
-from time import sleep
+import random
+import secrets
+import string
 from random import randint, uniform
+from time import sleep
+
 import selenium.webdriver.support.expected_conditions as EC
+from selenium.common.exceptions import TimeoutException, NoSuchElementException
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import WebDriverWait
-import secrets
-import string
+
+import login_gmail_selenium.common.constant as Constant
 
 
 def sleep_for(period):
     sleep(randint(period[0], period[1]))
 
 
 def type_text(driver, text, xpath, custom_enter=None, paste_text=Constant.PASTE_PERCENTAGE, loading=False,
```

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/PKG-INFO` & `login_gmail_selenium-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: login-gmail-selenium
-Version: 1.1.9
+Name: login_gmail_selenium
+Version: 1.2.0
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -32,17 +32,19 @@
 
 ## Usage
 ```pycon
 pip install login_gmail_selenium
 ```
 And then on example.py
 ```pycon
-from login_gmail_selenium.util.profile import ChromeProfile
+from login_gmail_selenium.util.profiles.profile import GoogleProfile
+from login_gmail_selenium.util.profiles.google_profile import Profile
 
-profile = ChromeProfile(email, password, backup_email)
+profile = GoogleProfile(email, password, backup_email)
+# profile = Profile(name_profile) If don't need login to google but save driver
 # To allow downloads add insecure=True to ChromeProfile
 # To handle false email with custom functions, use param false_email_callback
 driver = profile.retrieve_driver()
 profile.start()
 # Do whatever with driver afterward
 driver.get('https://www.google.com/')
 driver.quit()
@@ -52,14 +54,17 @@
 2. The temp folder's content will be generated by the library.
 Your folder should look like this
 ```cvs
 /temp
     /profiles
         /profile1
         /profile2
+    /blank_profiles
+        /blank_profiles1
+        /blank_profiles2
 /extension
     /custom_extension
         extension1.zip
         extension2.crx
 example.py
 ```
```

### Comparing `login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/SOURCES.txt` & `login_gmail_selenium-1.2.0/login_gmail_selenium.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,11 +12,14 @@
 login_gmail_selenium/common/log.py
 login_gmail_selenium/extension/always_active.zip
 login_gmail_selenium/extension/fingerprint_defender.zip
 login_gmail_selenium/extension/spoof_timezone.zip
 login_gmail_selenium/extension/veepn.zip
 login_gmail_selenium/extension/webrtc_control.zip
 login_gmail_selenium/util/__init__.py
+login_gmail_selenium/util/base_profile.py
 login_gmail_selenium/util/driver.py
 login_gmail_selenium/util/helper.py
-login_gmail_selenium/util/profile.py
+login_gmail_selenium/util/profiles/__init__.py
+login_gmail_selenium/util/profiles/google_profile.py
+login_gmail_selenium/util/profiles/profile.py
 test/test.py
```

### Comparing `login_gmail_selenium-1.1.9/setup.py` & `login_gmail_selenium-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r', encoding='utf-16') as f:
     requirements = [line.rstrip('\n') for line in f]
 
 setuptools.setup(
     name="login_gmail_selenium",
-    version="1.1.9",
+    version="1.2.0",
     author="Minh Hoang",
     author_email="ngminhhoang1412@gmail.com",
     description="A python package for login google by selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ngminhhoang1412/LoginGmailSelenium",
     include_package_data=True,
```

### Comparing `login_gmail_selenium-1.1.9/test/test.py` & `login_gmail_selenium-1.2.0/test/test.py`

 * *Files identical despite different names*

