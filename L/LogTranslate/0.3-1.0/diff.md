# Comparing `tmp/LogTranslate-0.3.tar.gz` & `tmp/LogTranslate-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-0.3.tar", last modified: Mon Jun 26 17:16:51 2023, max compression
+gzip compressed data, was "LogTranslate-1.0.tar", last modified: Tue Jun 27 15:21:01 2023, max compression
```

## Comparing `LogTranslate-0.3.tar` & `LogTranslate-1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:51.653275 LogTranslate-0.3/
--rw-rw-rw-   0        0        0     1079 2023-06-26 15:57:52.000000 LogTranslate-0.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:51.653275 LogTranslate-0.3/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0      618 2023-06-26 17:16:51.000000 LogTranslate-0.3/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-06-26 17:16:51.000000 LogTranslate-0.3/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:16:51.000000 LogTranslate-0.3/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-26 17:16:51.000000 LogTranslate-0.3/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-06-26 17:16:51.653275 LogTranslate-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2331 2023-06-26 16:22:25.000000 LogTranslate-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:51.653275 LogTranslate-0.3/log_translate/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:36:52.000000 LogTranslate-0.3/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:16:51.653275 LogTranslate-0.3/log_translate/business/
--rw-rw-rw-   0        0        0      610 2023-06-26 17:16:39.000000 LogTranslate-0.3/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0     3848 2023-06-26 17:16:39.000000 LogTranslate-0.3/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-26 17:16:39.000000 LogTranslate-0.3/log_translate/config_demo.py
--rw-rw-rw-   0        0        0     1266 2023-06-26 15:04:12.000000 LogTranslate-0.3/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-26 15:04:11.000000 LogTranslate-0.3/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4362 2023-06-26 17:16:39.000000 LogTranslate-0.3/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3004 2023-06-26 17:16:39.000000 LogTranslate-0.3/log_translate/read_log_file.py
--rw-rw-rw-   0        0        0     5447 2023-06-26 17:11:51.000000 LogTranslate-0.3/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     5599 2023-06-26 17:11:51.000000 LogTranslate-0.3/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-26 16:22:25.000000 LogTranslate-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 17:16:51.653275 LogTranslate-0.3/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-06-26 17:16:39.000000 LogTranslate-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:21:01.808447 LogTranslate-1.0/
+-rw-rw-rw-   0        0        0     1059 2023-06-26 17:21:40.000000 LogTranslate-1.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 15:21:01.791438 LogTranslate-1.0/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-06-27 15:21:01.000000 LogTranslate-1.0/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-06-27 15:21:01.000000 LogTranslate-1.0/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:21:01.000000 LogTranslate-1.0/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 15:21:01.000000 LogTranslate-1.0/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 15:21:01.000000 LogTranslate-1.0/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3172 2023-06-27 15:21:01.808447 LogTranslate-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2379 2023-06-27 14:49:49.000000 LogTranslate-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:21:01.803436 LogTranslate-1.0/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-27 08:16:54.000000 LogTranslate-1.0/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:21:01.806446 LogTranslate-1.0/log_translate/business/
+-rw-rw-rw-   0        0        0      636 2023-06-27 14:14:13.000000 LogTranslate-1.0/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 08:17:11.000000 LogTranslate-1.0/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-06-27 11:40:54.000000 LogTranslate-1.0/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      324 2023-06-27 11:40:54.000000 LogTranslate-1.0/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1294 2023-06-27 14:36:30.000000 LogTranslate-1.0/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       10 2023-06-26 17:21:40.000000 LogTranslate-1.0/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4236 2023-06-27 11:40:54.000000 LogTranslate-1.0/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3080 2023-06-27 15:20:40.000000 LogTranslate-1.0/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:21:01.807450 LogTranslate-1.0/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-27 14:36:27.000000 LogTranslate-1.0/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     6371 2023-06-27 15:14:55.000000 LogTranslate-1.0/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7708 2023-06-27 15:19:20.000000 LogTranslate-1.0/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      379 2023-06-26 17:21:40.000000 LogTranslate-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:21:01.809448 LogTranslate-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-06-27 15:20:59.000000 LogTranslate-1.0/setup.py
```

### Comparing `LogTranslate-0.3/LICENSE.txt` & `LogTranslate-1.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 贇
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 贇
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `LogTranslate-0.3/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.0/LogTranslate.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 LogTranslate.egg-info/PKG-INFO
 LogTranslate.egg-info/SOURCES.txt
 LogTranslate.egg-info/dependency_links.txt
+LogTranslate.egg-info/requires.txt
 LogTranslate.egg-info/top_level.txt
 log_translate/__init__.py
-log_translate/config_demo.py
+log_translate/config_default.py
 log_translate/data_struct.py
 log_translate/gloable.py
 log_translate/log_translator.py
 log_translate/read_log_file.py
 log_translate/ui_pyqt6.py
 log_translate/ui_pyside2.py
 log_translate/business/AndroidCrashPattern_translator.py
+log_translate/business/__init__.py
 log_translate/business/bluetooth_translator.py
-log_translate/business/AndroidCrashPattern_translator.py
-log_translate/business/bluetooth_translator.py
+log_translate/res/log_logo.ico
```

### Comparing `LogTranslate-0.3/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.0/log_translate/business/bluetooth_translator.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from log_translate.data_struct import Log, Level
-from log_translate.log_translator import *
-
-
-class SecTagDemoTranslator(SecStrTagTranslator):
-    def __init__(self):
-        super().__init__("DFJ",
-                         lambda string: re.search(r"(?P<tag>.*?) *:(?P<msg>.*)", string),
-                         [
-                             SysLogTranslator({
-                                 "sec_tag": self.new_tag
-                             })
-                         ])
-
-    def new_tag(self, tag, msg):
-        return Log(translated=msg)
-
-
-class BluetoothTranslator(TagStrTranslator):
-    def __init__(self):
-        super().__init__({
-            "BluetoothAdapter": bluetooth_adapter,
-            "BluetoothGatt": bluetooth_gatt,
-            "bt_rfcomm": bt_rfcomm,
-            "WS_BT_BluetoothPairingRequest": bluetooth_pairing_request,
-            "ActivityTaskManager": bluetooth_pairing_dialog
-        })
-
-
-code_state = {
-    "10": "手机系统蓝牙 已关闭",
-    "12": "手机系统蓝牙 已打开",
-    "OFF": "手机系统蓝牙 已关闭",
-    "ON": "手机系统蓝牙 已打开"
-}
-
-
-def bluetooth_pairing_dialog(msg):
-    # ActivityTaskManager: Displayed com.oplus.wirelesssettings/com.android.settings.bluetooth.BluetoothPairingDialog
-    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
-    if "BluetoothPairingDialog" in msg:
-        result = re.search("Displayed.*BluetoothPairingDialog", msg)
-        if result:
-            return Log(translated=" ----------------------- 配对PIN码弹窗弹出 ----------------------- ")
-    return None
-
-
-def bluetooth_pairing_request(msg):
-    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
-    if "PAIRING_REQUEST" in msg:
-        return Log(translated=" ----------------------- 设备请求配对 ----------------------- ")
-    return None
-
-
-def bt_rfcomm(msg):
-    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
-    if "port_rfc_closed" in msg:
-        result = re.search(".*: (ON|OFF)", msg)
-        if result:
-            if result.group(1) in code_state:
-                return Log(translated=">>>>>>>>>>  %s  <<<<<<<< " % (code_state[result.group(1)]), level=Level.i)
-
-    return None
-
-
-def bluetooth_adapter(msg):
-    if "isLeEnabled" in msg:
-        result = re.search(".*: (ON|OFF)", msg)
-        if result:
-            if result.group(1) in code_state:
-                return Log(translated=">>>>>>>>>>  %s  <<<<<<<< " % (code_state[result.group(1)]), level=Level.i)
-
-    return None
-
-
-# noinspection PyTypeChecker
-def bluetooth_gatt(msg: object) -> object:
-    if "cancelOpen()" in msg:
-        result = re.search("device: (.*?)", msg)
-        return Log(translated=">>>>>>>>>>  gatt 手机主动断开连接 %s  <<<<<<<< " % (result.group(1)), level=Level.w)
-    if "close()" in msg:
-        return Log(translated=">>>>>>>>>>  gatt 手机主动关闭连接  <<<<<<<< ", level=Level.w)
-    if "connect()" in msg:
-        # connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false
-        result = re.search("device: (.*?),", msg)
-        return Log(translated=">>>>>>>>>>  gatt 发起设备连接 %s  <<<<<<<< " % (result.group(1)), level=Level.w)
-    return None
-
-
-if __name__ == '__main__':
-    result = re.search("device: (.*?),", "connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false")
-    print(result.group(1))
-    result = re.search("(?<=\*).*", "onReCreateBond: 24:*:35:06")
-
-    # (?<=A).+?(?=B) 匹配规则A和B之间的元素 不包括A和B
-    #
-    print(result.group())
+from log_translate.data_struct import Log, Level
+from log_translate.log_translator import *
+
+
+class SecTagDemoTranslator(SecStrTagTranslator):
+    def __init__(self):
+        super().__init__("DFJ",
+                         lambda string: re.search(r"(?P<tag>.*?) *:(?P<msg>.*)", string),
+                         [
+                             SysLogTranslator({
+                                 "sec_tag": self.new_tag
+                             })
+                         ])
+
+    def new_tag(self, tag, msg):
+        return Log(translated=msg)
+
+
+class BluetoothTranslator(TagStrTranslator):
+    def __init__(self):
+        super().__init__({
+            "BluetoothAdapter": bluetooth_adapter,
+            "BluetoothGatt": bluetooth_gatt,
+            "bt_rfcomm": bt_rfcomm,
+            "WS_BT_BluetoothPairingRequest": bluetooth_pairing_request,
+            "ActivityTaskManager": bluetooth_pairing_dialog
+        })
+
+
+code_state = {
+    "10": "手机系统蓝牙 已关闭",
+    "12": "手机系统蓝牙 已打开",
+    "OFF": "手机系统蓝牙 已关闭",
+    "ON": "手机系统蓝牙 已打开"
+}
+
+
+def bluetooth_pairing_dialog(msg):
+    # ActivityTaskManager: Displayed com.oplus.wirelesssettings/com.android.settings.bluetooth.BluetoothPairingDialog
+    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
+    if "BluetoothPairingDialog" in msg:
+        result = re.search("Displayed.*BluetoothPairingDialog", msg)
+        if result:
+            return Log(translated=" ----------------------- 配对PIN码弹窗弹出 ----------------------- ")
+    return None
+
+
+def bluetooth_pairing_request(msg):
+    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
+    if "PAIRING_REQUEST" in msg:
+        return Log(translated=" ----------------------- 设备请求配对 ----------------------- ")
+    return None
+
+
+def bt_rfcomm(msg):
+    # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
+    if "port_rfc_closed" in msg:
+        result = re.search(".*: (ON|OFF)", msg)
+        if result:
+            if result.group(1) in code_state:
+                return Log(translated=">>>>>>>>>>  %s  <<<<<<<< " % (code_state[result.group(1)]), level=Level.i)
+
+    return None
+
+
+def bluetooth_adapter(msg):
+    if "isLeEnabled" in msg:
+        result = re.search(".*: (ON|OFF)", msg)
+        if result:
+            if result.group(1) in code_state:
+                return Log(translated=">>>>>>>>>>  %s  <<<<<<<< " % (code_state[result.group(1)]), level=Level.i)
+
+    return None
+
+
+# noinspection PyTypeChecker
+def bluetooth_gatt(msg: object) -> object:
+    if "cancelOpen()" in msg:
+        result = re.search("device: (.*?)", msg)
+        return Log(translated=">>>>>>>>>>  gatt 手机主动断开连接 %s  <<<<<<<< " % (result.group(1)), level=Level.w)
+    if "close()" in msg:
+        return Log(translated=">>>>>>>>>>  gatt 手机主动关闭连接  <<<<<<<< ", level=Level.w)
+    if "connect()" in msg:
+        # connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false
+        result = re.search("device: (.*?),", msg)
+        return Log(translated=">>>>>>>>>>  gatt 发起设备连接 %s  <<<<<<<< " % (result.group(1)), level=Level.w)
+    return None
+
+
+if __name__ == '__main__':
+    result = re.search("device: (.*?),", "connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false")
+    print(result.group(1))
+    result = re.search("(?<=\*).*", "onReCreateBond: 24:*:35:06")
+
+    # (?<=A).+?(?=B) 匹配规则A和B之间的元素 不包括A和B
+    #
+    print(result.group())
```

### Comparing `LogTranslate-0.3/log_translate/log_translator.py` & `LogTranslate-1.0/log_translate/log_translator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import re
-from abc import abstractmethod
-
-from log_translate.gloable import pids
-
-
-# 通过正则表达式匹配tag解析
-# :param pattern_translators 是数据[tag,fun(tag, msg)] fun参数必须是(tag, msg)
-class TagPatternTranslator(object):
-    def __init__(self, pattern_translators):
-        self.pattern_translators = pattern_translators
-
-    def translate(self, tag, msg):
-        for pattern in self.pattern_translators:
-            match = re.compile(pattern, re.IGNORECASE).match(tag)
-            if match:
-                translator = self.pattern_translators[pattern]
-                if callable(translator):
-                    return translator(tag, msg)
-                else:
-                    return translator.translate(tag, msg)
-        return None
-
-
-# 字符串匹配tag  例子参考 BluetoothTranslator
-# :param str_translators是数组[tag, fun(msg)] fun方法参数是 (msg)
-class TagStrTranslator(object):
-    def __init__(self, str_translators):
-        self.str_translators = str_translators
-
-    def translate(self, tag, msg):
-        if tag in self.str_translators:
-            translator = self.str_translators[tag]
-            if callable(translator):
-                return translator(msg)
-            else:
-                return translator.translate(msg)
-        return None
-
-
-class SecStrTagTranslator(TagStrTranslator):
-    """
-    :param father表示上一级tag
-    :param tag_from_str_fun 从字符串解析tag的方法
-    :param tag_translators 用来解析二级tag的translator 是个数组必须是TagStrTranslator|TagPatternTranslator
-    """
-
-    def __init__(self, father, tag_from_str_fun, tag_translators):
-        super().__init__({
-            father: self.translate_new_tag
-        })
-        self.tag_from_str_fun = tag_from_str_fun
-        self.tag_translators = tag_translators
-
-    def translate_new_tag(self, msg):
-        log = self.tag_from_str_fun(msg)
-        if log:
-            sec_tag = log.group("tag")
-            sec_msg = log.group("msg")
-            for translator in self.tag_translators:
-                result = translator.translate(sec_tag, sec_msg)
-                if result:
-                    return result
-        return None
-
-
-class StringTranslator(object):
-    def __init__(self, tag_translators=None):
-        # 这里是 TagStrTranslator
-        if tag_translators is None:
-            tag_translators = []
-        self.tag_translators = tag_translators
-
-    def translate(self, string):
-        # 系统日志
-        # 03-21 21:31:45.534 12980 15281 I ActivityManager   : START 0 ooooo:
-        log = self.tag_from_str(string)
-        if log:
-            tag = log.group("tag")
-            msg = log.group("msg")
-            time = log.group("time")
-            try:
-                pid = log.group("pid")
-            except:
-                pid = "0000"
-            for translator in self.tag_translators:
-                show = translator.translate(tag, msg)
-                if show:
-                    show.time = time
-                    show.oring = msg
-                    show.process = pid
-                    if pids.count(pid) == 0:
-                        pids.append(pid)
-                    return show
-        return None
-
-    @abstractmethod
-    def tag_from_str(self, string):
-        pass
-
-
-class SysLogTranslator(StringTranslator):
-    def tag_from_str(self, string):
-        # 04-29 10:01:16.788935  1848  2303 D OGG_Detector: D:done mCurrStatus: 0
-        return re.search(r"(?P<time>\d+.*\.\d{3,}) +(?P<pid>\d+).* [A-Z] (?P<tag>.*?) *:(?P<msg>.*)", string)
-
-
-class LogcatTranslator(StringTranslator):
-
-    def tag_from_str(self, string):
-        pass
-
-
-if __name__ == '__main__':
-    result = re.search("device: (.*?),", "connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false")
-    print(result.group(1))
-    result = re.search("(?<=\*).*", "onReCreateBond: 24:*:35:06")
-
-    # (?<=A).+?(?=B) 匹配规则A和B之间的元素 不包括A和B
-    #
-    print(result.group())
-
-    str = "04-29 10:01:16.788935  1848  2303 D OGG_Detector: D:done mCurrStatus: 0"
-    f = re.search(r"(?P<time>\d+.*\.\d{3,}) +(?P<pid>\d+).* [A-Z] (?P<tag>.*?) *:(?P<msg>.*)", str)
-    print(f.group("pid"))
-    print(f.group("tag"))
+import re
+from abc import abstractmethod
+
+from log_translate.gloable import pids
+
+
+# 通过正则表达式匹配tag解析
+# :param pattern_translators 是数据[tag,fun(tag, msg)] fun参数必须是(tag, msg)
+class TagPatternTranslator(object):
+    def __init__(self, pattern_translators):
+        self.pattern_translators = pattern_translators
+
+    def translate(self, tag, msg):
+        for pattern in self.pattern_translators:
+            match = re.compile(pattern, re.IGNORECASE).match(tag)
+            if match:
+                translator = self.pattern_translators[pattern]
+                if callable(translator):
+                    return translator(tag, msg)
+                else:
+                    return translator.translate(tag, msg)
+        return None
+
+
+# 字符串匹配tag  例子参考 BluetoothTranslator
+# :param str_translators是数组[tag, fun(msg)] fun方法参数是 (msg)
+class TagStrTranslator(object):
+    def __init__(self, str_translators):
+        self.str_translators = str_translators
+
+    def translate(self, tag, msg):
+        if tag in self.str_translators:
+            translator = self.str_translators[tag]
+            if callable(translator):
+                return translator(msg)
+            else:
+                return translator.translate(msg)
+        return None
+
+
+class SecStrTagTranslator(TagStrTranslator):
+    """
+    :param father表示上一级tag
+    :param tag_from_str_fun 从字符串解析tag的方法
+    :param tag_translators 用来解析二级tag的translator 是个数组必须是TagStrTranslator|TagPatternTranslator
+    """
+
+    def __init__(self, father, tag_from_str_fun, tag_translators):
+        super().__init__({
+            father: self.translate_new_tag
+        })
+        self.tag_from_str_fun = tag_from_str_fun
+        self.tag_translators = tag_translators
+
+    def translate_new_tag(self, msg):
+        log = self.tag_from_str_fun(msg)
+        if log:
+            sec_tag = log.group("tag")
+            sec_msg = log.group("msg")
+            for translator in self.tag_translators:
+                result = translator.translate(sec_tag, sec_msg)
+                if result:
+                    return result
+        return None
+
+
+class StringTranslator(object):
+    def __init__(self, tag_translators=None):
+        # 这里是 TagStrTranslator
+        if tag_translators is None:
+            tag_translators = []
+        self.tag_translators = tag_translators
+
+    def translate(self, string):
+        # 系统日志
+        # 03-21 21:31:45.534 12980 15281 I ActivityManager   : START 0 ooooo:
+        log = self.tag_from_str(string)
+        if log:
+            tag = log.group("tag")
+            msg = log.group("msg")
+            time = log.group("time")
+            try:
+                pid = log.group("pid")
+            except:
+                pid = "0000"
+            for translator in self.tag_translators:
+                show = translator.translate(tag, msg)
+                if show:
+                    show.time = time
+                    show.oring = msg
+                    show.process = pid
+                    if pids.count(pid) == 0:
+                        pids.append(pid)
+                    return show
+        return None
+
+    @abstractmethod
+    def tag_from_str(self, string):
+        pass
+
+
+class SysLogTranslator(StringTranslator):
+    def tag_from_str(self, string):
+        # 04-29 10:01:16.788935  1848  2303 D OGG_Detector: D:done mCurrStatus: 0
+        return re.search(r"(?P<time>\d+.*\.\d{3,}) +(?P<pid>\d+).* [A-Z] (?P<tag>.*?) *:(?P<msg>.*)", string)
+
+
+class LogcatTranslator(StringTranslator):
+
+    def tag_from_str(self, string):
+        pass
+
+
+if __name__ == '__main__':
+    result = re.search("device: (.*?),", "connect() - device: 34:47:9A:31:52:CF, auto: false, eattSupport: false")
+    print(result.group(1))
+    result = re.search("(?<=\*).*", "onReCreateBond: 24:*:35:06")
+
+    # (?<=A).+?(?=B) 匹配规则A和B之间的元素 不包括A和B
+    #
+    print(result.group())
+
+    str = "04-29 10:01:16.788935  1848  2303 D OGG_Detector: D:done mCurrStatus: 0"
+    f = re.search(r"(?P<time>\d+.*\.\d{3,}) +(?P<pid>\d+).* [A-Z] (?P<tag>.*?) *:(?P<msg>.*)", str)
+    print(f.group("pid"))
+    print(f.group("tag"))
```

