# Comparing `tmp/RobokitRS-1.0.1.8-py3-none-any.whl.zip` & `tmp/RobokitRS-1.0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12484 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat    76554 b- defN 22-Jun-20 03:17 RobokitRS/RobokitRS.py
--rw-rw-rw-  2.0 fat     3408 b- defN 22-Mar-11 05:16 RobokitRS/RobokitRS_config.py
+Zip file size: 12582 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat    77418 b- defN 22-Jun-22 06:41 RobokitRS/RobokitRS.py
+-rw-rw-rw-  2.0 fat     3424 b- defN 22-Jun-22 06:19 RobokitRS/RobokitRS_config.py
 -rw-rw-rw-  2.0 fat       21 b- defN 22-Mar-21 00:38 RobokitRS/__init__.py
 -rw-rw-rw-  2.0 fat     1110 b- defN 22-Jun-20 03:17 RobokitRS/pins/pins.config
--rw-rw-rw-  2.0 fat      680 b- defN 22-Jun-20 03:20 RobokitRS-1.0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-20 03:20 RobokitRS-1.0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 22-Jun-20 03:20 RobokitRS-1.0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      638 b- defN 22-Jun-20 03:20 RobokitRS-1.0.1.8.dist-info/RECORD
-8 files, 82513 bytes uncompressed, 11370 bytes compressed:  86.2%
+-rw-rw-rw-  2.0 fat      720 b- defN 22-Jun-22 06:52 RobokitRS-1.0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-22 06:52 RobokitRS-1.0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 22-Jun-22 06:52 RobokitRS-1.0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      638 b- defN 22-Jun-22 06:52 RobokitRS-1.0.1.9.dist-info/RECORD
+8 files, 83433 bytes uncompressed, 11468 bytes compressed:  86.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: RobokitRS/__init__.py
 Comment: 
 
 Filename: RobokitRS/pins/pins.config
 Comment: 
 
-Filename: RobokitRS-1.0.1.8.dist-info/METADATA
+Filename: RobokitRS-1.0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: RobokitRS-1.0.1.8.dist-info/WHEEL
+Filename: RobokitRS-1.0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: RobokitRS-1.0.1.8.dist-info/top_level.txt
+Filename: RobokitRS-1.0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: RobokitRS-1.0.1.8.dist-info/RECORD
+Filename: RobokitRS-1.0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RobokitRS/RobokitRS.py

```diff
@@ -1517,14 +1517,15 @@
             self.__pixel_led_init(pin, 1)
             ledData = RGBLedData()
             ledData.pinNumber = pin
             ledData.red = 0
             ledData.green = 0
             ledData.blue = 0
             ledData.brightness = 100
+            ledData.isOn = False
             self.__led_data_dict[pin] = ledData
 
         self.__pin_data_dict[pin].mode = mode
         protocol = ProtocolData()
         protocol.data = [ 0xF4, pin, mode.value ]
         self.__protocol_buf.append(protocol)
 
@@ -1717,15 +1718,16 @@
             self.set_pin_mode(pin, Modes.RGBLED)
 
         self.__led_data_dict[pin].red = red 
         self.__led_data_dict[pin].green = green
         self.__led_data_dict[pin].blue = blue
         self.__led_data_dict[pin].prevBrightness = self.__led_data_dict[pin].brightness
 
-        self.set_rgb_led_on(pin)
+        if self.__led_data_dict[pin].isOn is True:
+            self.set_rgb_led_on(pin)
 
     def set_rgb_led_brightness(self, pin:int=LED_PIN, brightness:int=100):
         """
         RGB LED set brightness function.
 
         Parameters
         --------
@@ -1740,16 +1742,24 @@
         if pin > 13 or pin < 2:
             print('Pin value error. Pin value must be between 2 and 13')
             return
         if brightness > 100 or brightness < 0:
             print('Brightness value error. Brightness value must be between 0 and 100')
             return
 
+        if pin in self.__led_data_dict:
+            if self.__led_data_dict[pin].brightness == self.__led_data_dict[pin].prevBrightness:
+                return
+        else:
+            self.set_pin_mode(pin, Modes.RGBLED)
+
         self.__led_data_dict[pin].brightness = brightness
-        self.set_rgb_led_on(pin)
+
+        if self.__led_data_dict[pin].isOn is True:
+            self.set_rgb_led_on(pin)
 
     def change_rgb_led_brightness(self, pin:int=LED_PIN, brightness:int=10):
         """
         RGB LED change brightness function.
 
         Parameters
         --------
@@ -1759,39 +1769,56 @@
         brightness
             The relative brightness value of RGB LED
         """
 
         if pin > 13 or pin < 2:
             print('Pin value error. Pin value must be between 2 and 13')
             return
+
+        if pin in self.__led_data_dict:
+            pass
+        else:
+            self.set_pin_mode(pin, Modes.RGBLED)
         
         self.__led_data_dict[pin].brightness += brightness
 
         if self.__led_data_dict[pin].brightness < 0:
             self.__led_data_dict[pin].brightness = 0
         if self.__led_data_dict[pin].brightness > 100:
             self.__led_data_dict[pin].brightness = 100
 
-        self.set_rgb_led_on(pin)
+        if self.__led_data_dict[pin].isOn is True:
+            self.set_rgb_led_on(pin)
 
     def set_rgb_led_on(self,pin:int=LED_PIN):
         """
         RGB LED set color function.
 
         Parameters
         --------
         pin
             Pin number of RGB LED
             (min : 2, max : 13)
         """
+
+        if pin in self.__led_data_dict:
+            pass
+        else:
+            self.set_pin_mode(pin, Modes.RGBLED)
+        
         colorRate = min( MAXRATE, max(0, MAXRATE * (self.__led_data_dict[pin].brightness * ALPHARATIO * 0.01)))
         r = round(self.__led_data_dict[pin].red * colorRate)
         g = round(self.__led_data_dict[pin].green * colorRate)
         b = round(self.__led_data_dict[pin].blue * colorRate)
 
+        if (r == 0) and (g == 0) and (b == 0):
+            self.__led_data_dict[pin].isOn = False
+        else:
+            self.__led_data_dict[pin].isOn = True
+
         protocol = ProtocolData()
         protocol.data.append(self.__START_SYSEX)
         protocol.data.append(0x00)
         protocol.data.append(0x07)
         protocol.data.append(0x06)
         protocol.data.append( int(pin << 1 | 1) )
         protocol.data.append(0x01)
@@ -1865,27 +1892,27 @@
         protocol.data.append(int(duration % 128))
         protocol.data.append(int(duration / 128))
         protocol.data.append(self.__END_SYSEX)
         protocol.delay = duration * 0.001
         self.__protocol_buf.append(protocol)
     
     def tone_do(self, pin:int = BUZZER_PIN, duration = 1000):
-        self.tone(pin, 73, duration)
+        self.tone(pin, 72, duration)
     def tone_re(self, pin:int = BUZZER_PIN, duration = 1000):
         self.tone(pin, 74, duration)
     def tone_mi(self, pin:int = BUZZER_PIN, duration = 1000):
         self.tone(pin, 76, duration)
     def tone_fa(self, pin:int = BUZZER_PIN, duration = 1000):
         self.tone(pin, 77, duration)
     def tone_sol(self, pin:int = BUZZER_PIN, duration = 1000):
         self.tone(pin, 79, duration)
     def tone_la(self, pin:int = BUZZER_PIN, duration = 1000):
-        self.tone(pin, 83, duration)
+        self.tone(pin, 81, duration)
     def tone_si(self, pin:int = BUZZER_PIN, duration = 1000):
-        self.tone(pin, 84, duration)
+        self.tone(pin, 83, duration)
     
     def melody_poweron(self):
         self.tone_with_delay(BUZZER_PIN,75,170)
         self.tone_with_delay(BUZZER_PIN,78,204)
         self.tone_with_delay(BUZZER_PIN,82,255)
         self.tone_with_delay(BUZZER_PIN,85,291)
```

## RobokitRS/RobokitRS_config.py

```diff
@@ -14,14 +14,15 @@
 class RGBLedData():
   pinNumber = 0
   red = 0
   green = 0
   blue = 0
   brightness = 100
   prevBrightness = 0
+  isOn = False
 
 class ProtocolData():
   def __init__(self) -> None:
     self.data = []
     self.delay = 0.0
 
 class GyroData():
```

## Comparing `RobokitRS-1.0.1.8.dist-info/METADATA` & `RobokitRS-1.0.1.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: RobokitRS
-Version: 1.0.1.8
-Summary: Python library for RobokitRS
+Version: 1.0.1.9
+Summary: UNKNOWN
 Home-page: https://eng.roborobo.co.kr/main
 Author: Roborobo
 Author-email: roborobolab@gmail.com
 License: MIT
 Download-URL: https://github.com/RoboroboLab/RobokitRS/archive/master.tar.gz
 Keywords: RobokitRS,roborobo
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3
+Description-Content-Type: text/markdown
 Requires-Dist: pyserial
 
-UNKNOWN
+Python library for RobokitRS
```

