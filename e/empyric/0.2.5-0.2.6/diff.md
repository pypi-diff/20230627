# Comparing `tmp/empyric-0.2.5.tar.gz` & `tmp/empyric-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyric-0.2.5.tar", max compression
+gzip compressed data, was "empyric-0.2.6.tar", max compression
```

## Comparing `empyric-0.2.5.tar` & `empyric-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.5/LICENSE
--rw-r--r--   0        0        0     6412 2023-05-31 15:01:11.750049 empyric-0.2.5/README.md
--rw-r--r--   0        0        0     2312 2023-05-31 15:01:11.751075 empyric-0.2.5/empyric/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 14:57:14.109740 empyric-0.2.5/empyric/__main__.py
--rw-r--r--   0        0        0    38882 2023-06-04 21:44:41.067403 empyric-0.2.5/empyric/adapters.py
--rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.5/empyric/collection/__init__.py
--rw-r--r--   0        0        0     1686 2023-05-31 15:01:11.752149 empyric-0.2.5/empyric/collection/barometers.py
--rw-r--r--   0        0        0    10912 2023-05-31 15:01:11.752528 empyric-0.2.5/empyric/collection/controllers.py
--rw-r--r--   0        0        0     9778 2023-06-02 01:59:14.990281 empyric-0.2.5/empyric/collection/generators.py
--rw-r--r--   0        0        0     1182 2023-05-31 15:01:11.753110 empyric-0.2.5/empyric/collection/humans.py
--rw-r--r--   0        0        0    10753 2023-06-04 21:44:41.067911 empyric-0.2.5/empyric/collection/instrument.py
--rw-r--r--   0        0        0     3177 2023-05-31 15:01:11.753753 empyric-0.2.5/empyric/collection/io.py
--rw-r--r--   0        0        0    17628 2023-05-31 15:01:11.753942 empyric-0.2.5/empyric/collection/multimeters.py
--rw-r--r--   0        0        0    22234 2023-05-31 15:01:11.754634 empyric-0.2.5/empyric/collection/scopes.py
--rw-r--r--   0        0        0    28366 2023-06-04 21:44:41.068531 empyric-0.2.5/empyric/collection/sourcemeters.py
--rw-r--r--   0        0        0     3639 2023-05-31 15:01:11.755459 empyric-0.2.5/empyric/collection/spectrometers.py
--rw-r--r--   0        0        0     6525 2023-05-31 15:01:11.755664 empyric-0.2.5/empyric/collection/supplies.py
--rw-r--r--   0        0        0     2167 2023-05-31 15:01:11.755920 empyric-0.2.5/empyric/collection/thermometers.py
--rw-r--r--   0        0        0     9763 2023-05-31 15:01:11.756218 empyric-0.2.5/empyric/collection/virtual.py
--rw-r--r--   0        0        0    30073 2023-06-04 21:44:28.937395 empyric-0.2.5/empyric/experiment.py
--rw-r--r--   0        0        0    37351 2023-05-31 15:01:11.756847 empyric-0.2.5/empyric/graphics.py
--rw-r--r--   0        0        0      761 2023-05-31 15:01:11.757347 empyric-0.2.5/empyric/instruments.py
--rw-r--r--   0        0        0    32794 2023-06-05 18:09:48.183596 empyric-0.2.5/empyric/routines.py
--rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.5/empyric/runcard_schema.yaml
--rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.5/empyric/tests/__init__.py
--rw-r--r--   0        0        0     1420 2023-05-27 14:57:14.113113 empyric-0.2.5/empyric/tests/henon_runcard_example.yaml
--rw-r--r--   0        0        0      634 2023-05-31 15:01:11.758110 empyric-0.2.5/empyric/tests/test_adapter.py
--rw-r--r--   0        0        0     2122 2023-05-31 15:01:11.758329 empyric-0.2.5/empyric/tests/test_experiment.py
--rw-r--r--   0        0        0      638 2023-05-31 15:01:11.759672 empyric-0.2.5/empyric/tests/test_variable.py
--rw-r--r--   0        0        0     8112 2023-05-31 15:01:11.760402 empyric-0.2.5/empyric/tools.py
--rw-r--r--   0        0        0     6471 2023-06-02 01:59:14.991494 empyric-0.2.5/empyric/types.py
--rw-r--r--   0        0        0    15879 2023-05-31 15:01:11.761215 empyric-0.2.5/empyric/variables.py
--rw-r--r--   0        0        0      798 2023-06-05 18:16:02.594619 empyric-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7192 1970-01-01 00:00:00.000000 empyric-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.6/LICENSE
+-rw-r--r--   0        0        0     6412 2023-05-31 15:01:11.750049 empyric-0.2.6/README.md
+-rw-r--r--   0        0        0     2312 2023-05-31 15:01:11.751075 empyric-0.2.6/empyric/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:57:14.109740 empyric-0.2.6/empyric/__main__.py
+-rw-r--r--   0        0        0    39355 2023-06-25 22:05:57.941241 empyric-0.2.6/empyric/adapters.py
+-rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.6/empyric/collection/__init__.py
+-rw-r--r--   0        0        0     1686 2023-05-31 15:01:11.752149 empyric-0.2.6/empyric/collection/barometers.py
+-rw-r--r--   0        0        0    10912 2023-05-31 15:01:11.752528 empyric-0.2.6/empyric/collection/controllers.py
+-rw-r--r--   0        0        0     9776 2023-06-23 04:53:11.331739 empyric-0.2.6/empyric/collection/generators.py
+-rw-r--r--   0        0        0     1182 2023-05-31 15:01:11.753110 empyric-0.2.6/empyric/collection/humans.py
+-rw-r--r--   0        0        0    10752 2023-06-23 04:53:11.332174 empyric-0.2.6/empyric/collection/instrument.py
+-rw-r--r--   0        0        0     3177 2023-05-31 15:01:11.753753 empyric-0.2.6/empyric/collection/io.py
+-rw-r--r--   0        0        0    17628 2023-05-31 15:01:11.753942 empyric-0.2.6/empyric/collection/multimeters.py
+-rw-r--r--   0        0        0    25177 2023-06-25 22:05:57.941807 empyric-0.2.6/empyric/collection/scopes.py
+-rw-r--r--   0        0        0    28405 2023-06-23 04:53:11.333069 empyric-0.2.6/empyric/collection/sourcemeters.py
+-rw-r--r--   0        0        0     3639 2023-05-31 15:01:11.755459 empyric-0.2.6/empyric/collection/spectrometers.py
+-rw-r--r--   0        0        0     6525 2023-05-31 15:01:11.755664 empyric-0.2.6/empyric/collection/supplies.py
+-rw-r--r--   0        0        0     2167 2023-05-31 15:01:11.755920 empyric-0.2.6/empyric/collection/thermometers.py
+-rw-r--r--   0        0        0     9763 2023-05-31 15:01:11.756218 empyric-0.2.6/empyric/collection/virtual.py
+-rw-r--r--   0        0        0    30073 2023-06-04 21:44:28.937395 empyric-0.2.6/empyric/experiment.py
+-rw-r--r--   0        0        0    37351 2023-05-31 15:01:11.756847 empyric-0.2.6/empyric/graphics.py
+-rw-r--r--   0        0        0      761 2023-05-31 15:01:11.757347 empyric-0.2.6/empyric/instruments.py
+-rw-r--r--   0        0        0    35317 2023-06-27 04:25:04.163028 empyric-0.2.6/empyric/routines.py
+-rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.6/empyric/runcard_schema.yaml
+-rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.6/empyric/tests/__init__.py
+-rw-r--r--   0        0        0     1420 2023-05-27 14:57:14.113113 empyric-0.2.6/empyric/tests/henon_runcard_example.yaml
+-rw-r--r--   0        0        0      634 2023-05-31 15:01:11.758110 empyric-0.2.6/empyric/tests/test_adapter.py
+-rw-r--r--   0        0        0     2122 2023-05-31 15:01:11.758329 empyric-0.2.6/empyric/tests/test_experiment.py
+-rw-r--r--   0        0        0      638 2023-05-31 15:01:11.759672 empyric-0.2.6/empyric/tests/test_variable.py
+-rw-r--r--   0        0        0     8112 2023-05-31 15:01:11.760402 empyric-0.2.6/empyric/tools.py
+-rw-r--r--   0        0        0     6389 2023-06-23 04:53:11.333940 empyric-0.2.6/empyric/types.py
+-rw-r--r--   0        0        0    15879 2023-06-26 05:09:03.391752 empyric-0.2.6/empyric/variables.py
+-rw-r--r--   0        0        0      830 2023-06-27 04:26:13.474368 empyric-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7239 1970-01-01 00:00:00.000000 empyric-0.2.6/PKG-INFO
```

### Comparing `empyric-0.2.5/LICENSE` & `empyric-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/README.md` & `empyric-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/__init__.py` & `empyric-0.2.6/empyric/__init__.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/adapters.py` & `empyric-0.2.6/empyric/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -764,46 +764,64 @@
 
 
 class USB(Adapter):
     """
     Handles communications with pure USB instruments through PyVISA or USBTMC.
     """
 
-    timeout = 0.5
-
     # Get USB library
     if importlib.util.find_spec("pyvisa"):
         lib = "pyvisa"
     elif importlib.util.find_spec("usbtmc"):
         lib = "usbtmc"
     else:
         lib = None
 
     no_lib_msg = "No USB library was found! " "Please install either PyVISA or USBTMC."
 
+    _timeout = 0.5
+
+    @property
+    def timeout(self):
+        return self._timeout
+
+    @timeout.setter
+    def timeout(self, timeout):
+        if self.backend is not None:
+            if self.lib == "usbtmc":
+                self.backend.timeout = timeout
+            elif self.lib == "pyvisa":
+                self.backend.timeout = 1000 * timeout
+
+        self._timeout = timeout
+
     def connect(self):
         serial_number = str(self.instrument.address)
 
         if self.lib == "pyvisa":
             visa = importlib.import_module("pyvisa")
 
             manager = visa.ResourceManager()
 
             for address in manager.list_resources():
                 if serial_number in address:
                     self.backend = manager.open_resource(
-                        address, open_timeout=self.timeout
+                        address, open_timeout=1000 * self.timeout
                     )
-                    self.backend.timeout = self.timeout
+
+                    # PyVISA timeout is in milliseconds
+                    self.backend.timeout = 1000 * self.timeout
 
         elif self.lib == "usbtmc":
             usbtmc = importlib.import_module("usbtmc")
 
             self.backend = usbtmc.Instrument("USB::" + serial_number + "::INSTR")
 
+            self.backend.timeout = self.timeout
+
         else:
             raise AdapterError(f"invalid library specification, {self.lib}")
 
         self.connected = True
 
     def _write(self, message):
         self.backend.write(message)
@@ -1050,18 +1068,20 @@
     else:
         lib = None
 
     @property
     def busy(self):
         if self._protocol == "Serial":
             return bool(
-                sum([
-                    adapter._busy for adapter in
-                    Modbus._serial_adapters.get(self.port, [])
-                ])
+                sum(
+                    [
+                        adapter._busy
+                        for adapter in Modbus._serial_adapters.get(self.port, [])
+                    ]
+                )
             )
         else:
             return self._busy
 
     @busy.setter
     def busy(self, busy):
         self._busy = busy
@@ -1075,40 +1095,34 @@
         if re.match("\d+\.\d+\.\d+\.\d+", address[0]):
             # Modbus TCP
             self._protocol = "TCP"
 
             if len(address) == 1:
                 address.append(502)  # standard Modbus TCP port
 
-            self.backend = client.ModbusTcpClient(
-                host=address[0],
-                port=int(address[1])
-            )
+            self.backend = client.ModbusTcpClient(host=address[0], port=int(address[1]))
 
         else:
             # Modbus Serial
             self._protocol = "Serial"
 
             if len(address) == 1:
-
                 # assume slave id is zero if not specified
                 port, slave_id = address[0], 0
 
             else:
                 port, slave_id = address
 
             if port in Modbus._serial_adapters:
-
                 Modbus._serial_adapters[port].append(self)
 
                 # use existing backend
                 self.backend = Modbus._serial_adapters[port].backend
 
             else:
-
                 Modbus._serial_adapters[port] = [self]
 
                 self.backend = client.ModbusSerialClient(
                     address=port,
                     baudrate=self.baud_rate,
                     bytesize=self.byte_size,
                     parity=self.parity,
@@ -1140,16 +1154,15 @@
         values = np.array([values]).flatten()
 
         if func_code not in [5, 15, 6, 16]:
             raise ValueError(f"invalid Modbus function code {func_code}")
 
         if _type and _type not in self.types:
             raise TypeError(
-                "invalid _type argument; must be one of:\n"
-                + ", ".join(self.types)
+                "invalid _type argument; must be one of:\n" + ", ".join(self.types)
             )
 
         if "5" in str(func_code):
             # Write coils
 
             bool_values = [bool(value) for value in values]
```

### Comparing `empyric-0.2.5/empyric/collection/barometers.py` & `empyric-0.2.6/empyric/collection/barometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/controllers.py` & `empyric-0.2.6/empyric/collection/controllers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/generators.py` & `empyric-0.2.6/empyric/collection/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
         "channel 2 low level",
         "channel 1 frequency",
         "channel 2 frequency",
         "channel 1 pulse width",
         "channel 2 pulse width",
         "channel 1 pulse delay",
         "channel 2 pulse delay",
-        'channel 1 invert',
-        'channel 2 invert',
-        'equal phase'
+        "channel 1 invert",
+        "channel 2 invert",
+        "equal phase",
     )
 
     wave_forms = ("SINE", "SQUARE", "RAMP", "PULSE", "NOISE", "ARB", "DC", "PRBS", "IQ")
 
     def _set_channel_n_output(self, n, output: Toggle, load: String, polarity: String):
         self.write(f"C{n}:OUTP {output},LOAD,{load},PLRT,{polarity}")
 
@@ -96,27 +96,25 @@
         values = response[1::2]
 
         waveform_dict = {key: value for key, value in zip(keys, values)}
 
         return waveform_dict
 
     def _set_channel_n_invert(self, n, state: Toggle):
-
         if state == ON:
-            self.write('C%d:INVT ON' % n)
+            self.write("C%d:INVT ON" % n)
         elif state == OFF:
-            self.write('C%d:INVT OFF' % n)
+            self.write("C%d:INVT OFF" % n)
 
     def _get_channel_n_invert(self, n):
+        response = self.query("C%d:INVT?" % n)
 
-        response = self.query('C%d:INVT?' % n)
-
-        if 'ON' in response:
+        if "ON" in response:
             return ON
-        if 'OFF' in response:
+        if "OFF" in response:
             return OFF
 
     # Output
     @setter
     def set_channel_1_output(self, output: Toggle):
         _, load, polarity = self._get_channel_n_output(1)
 
@@ -316,10 +314,9 @@
     @getter
     def get_channel_2_invert(self) -> Toggle:
         return self._get_channel_n_invert(2)
 
     # Equalize phase of both channels
     @setter
     def set_equal_phase(self, state: Toggle):
-
         if state == ON:
-            self.write('EQPHASE')
+            self.write("EQPHASE")
```

### Comparing `empyric-0.2.5/empyric/collection/humans.py` & `empyric-0.2.6/empyric/collection/humans.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/instrument.py` & `empyric-0.2.6/empyric/collection/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             # The knob attribute is set to the returned value of the method, or
             # the value argument if the returned value is None
             if returned_value is not None:
                 self.__setattr__(knob, recast(returned_value, to=dtype))
             else:
                 self.__setattr__(knob, recast(value, to=dtype))
         finally:
-
             self.lock.release()
 
     return wrapped_method
 
 
 def getter(method):
     """
```

### Comparing `empyric-0.2.5/empyric/collection/io.py` & `empyric-0.2.6/empyric/collection/io.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/multimeters.py` & `empyric-0.2.6/empyric/collection/multimeters.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/scopes.py` & `empyric-0.2.6/empyric/collection/scopes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import struct
 from empyric.tools import find_nearest
 from empyric.adapters import *
 from empyric.collection.instrument import *
 from empyric.types import Float, Array, Integer, String
 
 
-class TekScope(Instrument):
+class TekTDSScope(Instrument):
     """
     Tektronix oscillscope of the TDS200, TDS1000/2000, TDS1000B/2000B,
-    TPS2000 series
+    TPS2000 series.
 
-    NOT TESTED
+    Although there are up to four channels, the constructor checks the model
+    number for the actual number of supported channels. With the 2-channel
+    models, any methods relating to channels 3 or 4 will take no action.
+
+    2-Channel models: TXX1001, TXX1002, TXX1012, TXX2002, TXX2012, TXX2022
+
+    4-channel models: TXX2004, TXX2014
     """
 
     name = "TekScope"
 
-    supported_adapters = ((USB, {"timeout": 10}),)  # acquisitions can take a long time
+    supported_adapters = ((USB, {"timeout": 10}),)
 
     knobs = (
         "horz scale",
         "horz position",
         "ch1 scale",
         "ch1 position",
         "ch2 scale",
@@ -34,91 +40,205 @@
     meters = (
         "channel 1",
         "channel 2",
         "channel 3",
         "channel 4",
     )
 
+    channels = 0
+
+    two_channel_models = [1001, 1002, 1012, 2002, 2012, 2022]
+    four_channel_models = [2004, 2014]
+
+    def __init__(self, *args, **kwargs):
+        # Check for number of channels before standard initialization
+        adapter = USB(Instrument(args[0]))
+
+        self.model = int(re.search("\d\d\d\d", adapter.query("*IDN?"))[0])
+
+        adapter.disconnect()
+
+        if self.model in self.two_channel_models:
+            self.channels = 2
+        elif self.model in self.four_channel_models:
+            self.channels = 4
+
+        super().__init__(*args, **kwargs)
+
+    # Horizontal
+
     @setter
     def set_horz_scale(self, scale: Float):
         self.write("HOR:SCA %.3e" % scale)
 
+    @getter
+    def get_horz_scale(self) -> Float:
+        return float(self.query("HOR:SCA?"))
+
     @setter
     def set_horz_position(self, position: Float):
         self.write("HOR:POS %.3e" % position)
 
-    @setter
-    def set_ch1_scale(self, scale: Float):
-        self.write("CH1:SCA %.3e" % scale)
+    @getter
+    def get_horz_position(self) -> Float:
+        return float(self.query("HOR:POS?"))
 
-    @setter
-    def set_ch2_scale(self, scale: Float):
-        self.write("CH1:SCA %.3e" % scale)
+    # Channel 1
 
     @setter
-    def set_ch3_scale(self, scale: Float):
+    def set_ch1_scale(self, scale: Float):
         self.write("CH1:SCA %.3e" % scale)
 
-    @setter
-    def set_ch4_scale(self, scale: Float):
-        self.write("CH1:SCA %.3e" % scale)
+    @getter
+    def get_ch1_scale(self) -> Float:
+        return float(self.query("CH1:SCA?"))
 
     @setter
     def set_ch1_position(self, position: Float):
         self.write("CH1:POS %.3e" % position)
 
+    @getter
+    def get_ch1_position(self) -> Float:
+        return float(self.query("CH1:POS?"))
+
+    @measurer
+    def measure_channel_1(self) -> Array:
+        return self._measure_channel(1)
+
+    # Channel 2
+
+    @setter
+    def set_ch2_scale(self, scale: Float):
+        self.write("CH2:SCA %.3e" % scale)
+
+    @getter
+    def get_ch2_scale(self) -> Float:
+        return float(self.query("CH2:SCA?"))
+
     @setter
     def set_ch2_position(self, position: Float):
-        self.write("CH1:POS %.3e" % position)
+        self.write("CH2:POS %.3e" % position)
+
+    @getter
+    def get_ch2_position(self) -> Float:
+        return float(self.query("CH2:POS?"))
+
+    @measurer
+    def measure_channel_2(self) -> Array:
+        return self._measure_channel(2)
+
+    # Channel 3
+
+    @setter
+    def set_ch3_scale(self, scale: Float):
+        if self.channels > 2:
+            self.write("CH3:SCA %.3e" % scale)
+        else:
+            return np.nan
+
+    @getter
+    def get_ch3_scale(self) -> Float:
+        if self.channels > 2:
+            return float(self.query("CH3:SCA?"))
+        else:
+            return np.nan
 
     @setter
     def set_ch3_position(self, position: Float):
-        self.write("CH1:POS %.3e" % position)
+        if self.channels > 2:
+            self.write("CH3:POS %.3e" % position)
+        else:
+            return np.nan
+
+    @getter
+    def get_ch3_position(self) -> Float:
+        if self.channels > 2:
+            return float(self.query("CH3:POS?"))
+        else:
+            return np.nan
+
+    @measurer
+    def measure_channel_3(self) -> Array:
+        if self.channels > 2:
+            return self._measure_channel(3)
+        else:
+            return [np.nan]
+
+    # Channel 4
+
+    @setter
+    def set_ch4_scale(self, scale: Float):
+        if self.channels > 2:
+            self.write("CH4:SCA %.3e" % scale)
+        else:
+            return np.nan
+
+    @getter
+    def get_ch4_scale(self) -> Float:
+        if self.channels > 2:
+            return float(self.query("CH4:SCA?"))
+        else:
+            return np.nan
 
     @setter
     def set_ch4_position(self, position: Float):
-        self.write("CH1:POS %.3e" % position)
+        if self.channels > 2:
+            self.write("CH4:POS %.3e" % position)
+        else:
+            return np.nan
+
+    @getter
+    def get_ch4_position(self) -> Float:
+        if self.channels > 2:
+            return float(self.query("CH4:POS?"))
+        else:
+            return np.nan
+
+    @measurer
+    def measure_channel_4(self) -> Array:
+        if self.channels > 2:
+            return self._measure_channel(4)
+        else:
+            return [np.nan]
+
+    # Trigger
 
     @setter
     def set_trigger_level(self, level: Float):
         self.write("TRIG:MAI:LEV %.3e" % level)
 
-    def _measure_channel(self, channel):
+    @getter
+    def get_trigger_level(self) -> Float:
+        return float(self.query("TRIG:MAI:LEV?"))
+
+    def _measure_channel(self, n):
         self.write("DAT:ENC ASCI")  # ensure ASCII encoding of data
-        self.write("DAT:SOU CH%d" % channel)  # switch to channel 1
+        self.write("DAT:SOU CH%d" % n)  # switch to channel n
 
         scale_factor = float(self.query("WFMPRE:YMULT?"))
         zero = float(self.query("WFMPRE:YZERO?"))
         offset = float(self.query("WFMPRE:YOFF?"))
 
         self.write("ACQ:STATE RUN")  # acquire the waveform
 
         while int(self.query("BUSY?")):
-            time.sleep(1)  # wait for acquisition to complete
+            time.sleep(0.25)  # wait for acquisition to complete
 
-        str_data = self.query("CURVE?").split(" ")[1].split(",")
-        return np.array(
-            [(float(datum) - offset) * scale_factor + zero for datum in str_data]
-        )
+        normal_timeout = self.adapter.timeout
+        self.adapter.timeout = 60
 
-    @measurer
-    def measure_channel_1(self) -> Array:
-        return self._measure_channel(1)
+        response = self.query("CURVE?")
 
-    @measurer
-    def measure_channel_2(self) -> Array:
-        return self._measure_channel(2)
+        str_data = response.split(",")
 
-    @measurer
-    def measure_channel_3(self) -> Array:
-        return self._measure_channel(3)
+        self.adapter.timeout = normal_timeout
 
-    @measurer
-    def measure_channel_4(self) -> Array:
-        return self._measure_channel(4)
+        return np.array(
+            [(float(datum) - offset) * scale_factor + zero for datum in str_data]
+        )
 
 
 class MulticompProScope(Instrument):
     """
     Multicomp Pro PC Oscilloscope.
 
     NOT TESTED
```

### Comparing `empyric-0.2.5/empyric/collection/sourcemeters.py` & `empyric-0.2.6/empyric/collection/sourcemeters.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,14 @@
         if np.ndim(voltages) == 1:
             return np.array(voltages, dtype=float)  # --> self.fast_voltages
         else:
             raise ValueError(f"invalid fast voltages: {voltages}")
 
     @measurer
     def measure_fast_currents(self) -> Array:
-
         normal_timeout = self.adapter.timeout
         self.adapter.timeout = None  # measurements can take a while
 
         list_length = len(self.fast_voltages)
 
         if list_length == 0:
             raise ValueError(f"fast voltages for {self.name} have not been set")
@@ -649,25 +648,27 @@
 
         path = self.name + "-fast_iv_measurement.csv"
 
         list_length = len(self.fast_voltages)
 
         if list_length >= 100:
             sub_lists = [
-                self.fast_voltages[ # pylint: disable=unsubscriptable-object
+                self.fast_voltages[  # pylint: disable=unsubscriptable-object
                     i * 100 : (i + 1) * 100
                 ]
                 for i in range(list_length // 100)
             ]
         else:
             sub_lists = []
 
         if list_length % 100 > 0:
             sub_lists.append(
-                self.fast_voltages[-(list_length % 100) :] # pylint: disable=unsubscriptable-object
+                self.fast_voltages[
+                    -(list_length % 100) :
+                ]  # pylint: disable=unsubscriptable-object
             )
 
         current_list = []
 
         normal_timeout = self.adapter.timeout
         self.adapter.timeout = None  # the response times can be long
```

### Comparing `empyric-0.2.5/empyric/collection/spectrometers.py` & `empyric-0.2.6/empyric/collection/spectrometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/supplies.py` & `empyric-0.2.6/empyric/collection/supplies.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/thermometers.py` & `empyric-0.2.6/empyric/collection/thermometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/collection/virtual.py` & `empyric-0.2.6/empyric/collection/virtual.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/experiment.py` & `empyric-0.2.6/empyric/experiment.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/graphics.py` & `empyric-0.2.6/empyric/graphics.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/instruments.py` & `empyric-0.2.6/empyric/instruments.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/routines.py` & `empyric-0.2.6/empyric/routines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import importlib
 import numbers
 import socket
 import queue
 import threading
 import asyncio
 import time
+from typing import Union
+
 import select
 import functools
 
 import numpy as np
 import pandas as pd
 
+from bayes_opt import BayesianOptimization, UtilityFunction
+
 from empyric.tools import (
     convert_time,
     autobind_socket,
     read_from_socket,
     write_to_socket,
     get_ip_address,
 )
@@ -35,36 +39,73 @@
 
 class Routine:
     """
     A Routine periodically updates a set of `knobs` based on a given state of an
     experiment. The knobs argument should be a dictionary of the form
     {..., name: variable, ...}.
 
-    The optional `start` and `end` arguments indicate when the routine should
-    start and end. The default values are 0 and infinity, respectively. When
-    updating, the routine compares these values to the `Time` value of the
-    given state.
+    The optional `enable` argument should be a string corresponding to a key in whatever
+    object is being passed as the `state` argument to the `update` method. The
+    corresponding value should be boolean. When the enabling value is False, the
+    `update` method takes no action. Otherwise, the `update` method proceeds normally.
+
+    The optional `start`, `end` and `duration` arguments indicate when the routine
+    should start and end. The `start` argument can be a number in seconds or a string
+    with a number and units, e.g. "2 minutes", indicating when the routine starts, or it
+    can be set to 'on enable' such that the start time is set to the time at which it is
+    enabled (possibly repeatedly) and the end time is set to the start time plus
+    `_duration` on each call to the `update` method. One can specify either `end` or
+    `duration`, but not both; `end` is the absolute time at which the routine will end,
+    while `duration` is the length of time the routine will run for (end minus start).
 
-    All other arguments are fixed values or string dictionary keys,
-    corresponding to variables values of the controlling experiment.
+    All other arguments are fixed values or dictionary keys, corresponding to variable
+    values of the controlling experiment.
     """
 
     assert_control = True
 
+    _start_on_enable = False
+
+    _duration = 0.0
+
     def __init__(
-        self, knobs: dict, enable: String = None, start=0.0, end=np.inf, **kwargs
+        self,
+        knobs: dict,
+        enable: String = None,
+        start: Union[Float, String] = None,
+        end: Union[Float, String] = None,
+        duration: Union[Float, String] = None,
+        **kwargs,
     ):
         self.knobs = knobs
 
         for knob in self.knobs.values():
             knob._controller = None  # to control access to knob
 
         self.enable = enable
-        self.start = convert_time(start)
-        self.end = convert_time(end)
+
+        if start is not None:
+            if start == "on enable":
+                self.start = np.nan  # will be set when routine is enabled
+                self._start_on_enable = True
+            else:
+                self.start = convert_time(start)
+        else:
+            self.start = 0.0
+
+        if end is not None:
+            self.end = convert_time(end)
+            self._duration = self.end - self.start
+        elif duration is not None:
+            self.end = self.start + convert_time(duration)
+            self._duration = convert_time(duration)
+        else:
+            self.end = np.inf
+            self._duration = np.inf
+
         self.prepped = False
         self.finished = False
 
         for key, value in kwargs.items():
             self.__setattr__(key.replace(" ", "_"), value)
 
     @staticmethod
@@ -84,14 +125,19 @@
 
         @functools.wraps(update)
         def wrapped_update(self, state):
             if self.enable is not None and not state[self.enable]:
                 for name, knob in self.knobs.items():
                     if knob._controller == self:
                         knob._controller = None
+
+                if self._start_on_enable:
+                    self.start = np.nan
+                    self.end = np.nan
+
                 return
 
             elif state["Time"] < self.start:
                 if not self.prepped:
                     self.prep(state)
                     self.prepped = True
 
@@ -106,18 +152,21 @@
                     for name, knob in self.knobs.items():
                         if knob._controller == self:
                             knob._controller = None
 
                 return
 
             else:
-
                 if not self.prepped:
                     self.prep(state)
 
+                if self._start_on_enable and np.isnan(self.start):
+                    self.start = state["Time"]
+                    self.end = self.start + self._duration
+
                 for name, knob in self.knobs.items():
                     if knob._controller and knob._controller != self:
                         # take no action if another routine has control
                         return
                     elif self.assert_control:
                         # assert control if needed
                         knob._controller = self
@@ -302,15 +351,14 @@
         if "end" not in kwargs:
             self.end = np.max(self.times)
 
     @Routine.enabler
     def update(self, state):
         knobs_times_values = zip(self.knobs, self.times, self.values)
         for knob, times, values in knobs_times_values:
-
             if np.min(times) > state["Time"] or np.max(times) < state["Time"]:
                 continue
 
             j_last = np.argwhere(times <= state["Time"]).flatten()[-1]
             j_next = np.argwhere(times > state["Time"]).flatten()[0]
 
             last_time = times[j_last]
@@ -331,34 +379,31 @@
             value = last_value + (next_value - last_value) * (
                 state["Time"] - last_time
             ) / (next_time - last_time)
 
             self.knobs[knob].value = value
 
     def prep(self, state):
-
         # Validate values
         for knob, value_list in zip(self.knobs.keys(), self.values):
             for value in value_list:
-
                 is_number = isinstance(value, numbers.Number)
                 is_variable = value in list(state.keys())
 
                 if not is_number and not is_variable:
                     raise ValueError(
-                        f'value {value} given for knob {knob} in Timecourse '
-                        f'routine is invalid; value must be a numeric type or '
-                        f'the name of a variable in the updating state'
+                        f"value {value} given for knob {knob} in Timecourse "
+                        f"routine is invalid; value must be a numeric type or "
+                        f"the name of a variable in the updating state"
                     )
 
     def finish(self, state):
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
-
                 if isinstance(value, String) and value in state:
                     knob.value = state[value]
                 else:
                     knob.value = value
 
 
 class Sequence(Routine):
@@ -401,158 +446,158 @@
 
         self.iteration = (self.iteration + 1) % len(self.values[0])
 
     def finish(self, state):
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
-
                 if isinstance(value, String) and value in state:
                     knob.value = state[value]
                 else:
                     knob.value = value
 
 
-class Minimization(Routine):
+class Maximization(Routine):
     """
-    Minimize a `meter`(/expression) influenced by the set of `knobs`, using
-    simulated annealing.
+    Maximize a meter or expression influenced by the set of knobs.
+
+    This routine uses a `bayesian optimizer
+    <https://github.com/bayesian-optimization/BayesianOptimization>`_, which models
+    the relation between the knobs and the meter as a gaussian process.
+
+    The `bounds` parameter
+    provides the parameter space over which the knob values can be explored.
 
-    The `meter` argument is the expression or meter to be minimized. The
-    `max_deltas` argument is an optional list/array of same length as `knobs`
-    indicating the maximum change per step for each knob; if not specified,
-    defaults to a list of ones. The `T0` and `T1` argumnets are the initial and
-    final temperatures; if not specified, defaults to T0 = 0.0 and T1 = 0.0.
-    The `samples` argument determines the number of meter values to average
-    together for each step.
+    The `max_deltas` parameter is a value or 1-D array of values which are the
+    maximum change in a single step the knob(s) can take.
+
+    The `kappa` parameter determines how much time the algorithm spends
+    exploring the parameter space away from the maximum versus the parameter
+    space in the vicinity of the maximum. Higher `kappa` leads to more
+    exploration, lower `kappa` leads to more "exploitation" of the maximum.
     """
 
+    _sign = 1.0
+
+    _last_setting = -np.inf
+
     def __init__(
-        self, knobs: dict, meter, max_deltas=None, T0=0.0, T1=0.0, samples=1, **kwargs
+        self,
+        knobs: dict,
+        meter,
+        bounds,
+        max_deltas=None,
+        kappa=2.5,
+        settling_time: Union[Float, String] = 0.0,
+        **kwargs,
     ):
         Routine.__init__(self, knobs, **kwargs)
 
-        self.meter = meter
+        self.bounds = {
+            knob: subbounds
+            for knob, subbounds in zip(knobs, np.reshape(bounds, (len(knobs), -1)))
+        }
 
         if max_deltas:
-            self.max_deltas = np.array([max_deltas]).flatten()
+            if np.ndim(max_deltas) == 0:
+                self.max_deltas = np.array([max_deltas] * len(knobs))
+            elif np.ndim(max_deltas) == 1 and len(max_deltas) == len(knobs):
+                self.max_deltas = np.array(max_deltas)
+            else:
+                ValueError(
+                    f"Improperly specified max_deltas parameter {max_deltas} for "
+                    "optimization routine; must be either a single value or 1-D array "
+                    "with the same length as the knobs argument"
+                )
         else:
-            self.max_deltas = np.ones(len(self.knobs))
+            self.max_deltas = np.array([np.inf] * len(self.knobs))
 
-        self.T = T0
-        self.T0 = T0
-        self.T1 = T1
-        self.samples = samples
+        self.meter = meter
 
-        self.meter_values = []
         self.best_meter = None
         self.best_knobs = [None for _ in self.knobs]
 
-        self.revert = False  # going back?
-
-    @Routine.enabler
-    def update(self, state):
-        # Take no action if knobs values are undefined
-        if None in [state[knob] for knob in self.knobs] or np.nan in [
-            state[knob] for knob in self.knobs
-        ]:
-            return
+        self.optimizer = BayesianOptimization(
+            f=None,
+            verbose=0,
+            pbounds=self.bounds,
+            random_state=6174,
+            allow_duplicate_points=True,
+        )
 
-        if not self.prepped:
-            self.prep(state)
-            self.prepped = True
-
-        # Update temperature
-        self.T = self.T0 + (self.T1 - self.T0) * (state["Time"] - self.start) / (
-            self.end - self.start
+        self._kappa0 = kappa
+        self.util_func = UtilityFunction(
+            kappa=kappa,  # exploration vs. exploitation parameter
         )
 
-        # Get meter values
-        meter_value = state[self.meter]
+        self.settling_time = convert_time(settling_time)
 
-        # Check for valid new meter value
-        if meter_value is not None and meter_value != np.nan:
-            self.meter_values.append(meter_value)
-        else:
-            return
+    @Routine.enabler
+    def update(self, state):
+        non_numeric_knobs = [
+            not isinstance(state[knob], numbers.Number) for knob in self.knobs
+        ]
 
-        # Check if enough samples have been measured
-        if len(self.meter_values) <= self.samples:
+        if np.any(non_numeric_knobs):
+            # undefined state; take no action
             return
 
-        # Check if found (or returned to) minimum
-        if self.better(np.mean(self.meter_values)) or self.revert:
-            # Record this new (or past) optimal state
-            self.best_meter = np.mean(self.meter_values)
-            self.best_knobs = [state[knob] for knob in self.knobs]
-
-            # Generate and apply new knob settings
-            new_knobs = self.best_knobs + self.max_deltas * (
-                2 * np.random.rand(len(self.knobs)) - 1
-            )
-
-            for knob, new_value in zip(self.knobs.values(), new_knobs):
-                knob.value = new_value
-
-            self.meter_values = []
-            self.revert = False
+        if not isinstance(state[self.meter], numbers.Number):
+            # undefined target value; take no action
+            return
 
-        else:
-            for knob, best_val in zip(self.knobs.values(), self.best_knobs):
-                knob.value = best_val
+        if state["Time"] < self._last_setting + self.settling_time:
+            return
 
-            self.meter_values = []
-            self.revert = True
+        self.optimizer.register(
+            params={knob: state[knob] for knob in self.knobs},
+            target=self._sign * state[self.meter],
+        )
 
-    def better(self, meter_value):
-        if meter_value is None or meter_value == np.nan:
-            return False
+        suggestion = self.optimizer.suggest(self.util_func)
 
-        if self.best_meter is None or self.best_meter == np.nan:
-            return False
+        for i, (knob, value) in enumerate(suggestion.items()):
+            if value is None or not np.isfinite(value):
+                pass
+            elif np.abs(value - state[knob]) <= self.max_deltas[i]:
+                self.knobs[knob].value = value
+            else:
+                sign = (value - state[knob]) / np.abs(value - state[knob])
+                self.knobs[knob].value = state[knob] + sign * self.max_deltas[i]
 
-        change = meter_value - self.best_meter
+        self._last_setting = state["Time"]
 
-        if self.T > 0:
-            _rand = np.random.rand()
-            return (change < 0) or (np.exp(-change / self.T) > _rand)
-        else:
-            return change < 0
+        self.best_meter = self.optimizer.max["target"]
+        self.best_knobs = self.optimizer.max["params"]
 
-    def prep(self, state):
-        self.best_knobs = [state[knob] for knob in self.knobs]
-        self.best_meter = state[self.meter]
+        if np.isfinite(self.end):
+            kappa = self._kappa0 * (self.end - state["Time"]) / self._duration
+            self.util_func.kappa = kappa
 
     def finish(self, state):
-        for knob, best_val in zip(self.knobs.values(), self.best_knobs):
-            knob.value = best_val
-
-
-class Maximization(Minimization):
-    """
-    Maximize a `meter`/expression influenced by the set of knobs;
-    otherwise, works the same way as Minimize.
-    """
-
-    best_meter = -np.inf
-
-    def better(self, meter_value):
-        if meter_value is None or meter_value == np.nan:
-            return False
+        for i, (knob, value) in enumerate(self.best_knobs.items()):
+            if value is None or not np.isfinite(value):
+                print(f"Warning: No optimal value was found for {knob}")
+            if np.abs(value - state[knob]) <= self.max_deltas[i]:
+                self.knobs[knob].value = value
+            else:
+                print(
+                    f"Warning: optimal value for {knob} suggested by optimizer "
+                    f"is {value}, but applying this value would exceed the "
+                    f"max_delta parameter. Instead, {knob} will be set as "
+                    f"close as possible without exceeding this limit."
+                )
+                sign = (value - state[knob]) / np.abs(value - state[knob])
+                self.knobs[knob].value = state[knob] + sign * self.max_deltas[i]
 
-        if self.best_meter is None or self.best_meter == np.nan:
-            return False
 
-        change = meter_value - self.best_meter
+class Minimization(Maximization):
+    """Same as Maximization except that the sign of the meter is inverted"""
 
-        if self.T > 0:
-            _rand = np.random.rand()
-            return (change > 0) or (np.exp(change / self.T) > _rand)
-        else:
-            return change > 0
+    _sign = -1.0
 
 
 class SocketServer(Routine):
     """
     Server routine for transmitting data to other experiments, local or remote,
     using the socket interface.
```

### Comparing `empyric-0.2.5/empyric/runcard_schema.yaml` & `empyric-0.2.6/empyric/runcard_schema.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/tests/henon_runcard_example.yaml` & `empyric-0.2.6/empyric/tests/henon_runcard_example.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/tests/test_adapter.py` & `empyric-0.2.6/empyric/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/tests/test_experiment.py` & `empyric-0.2.6/empyric/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/tests/test_variable.py` & `empyric-0.2.6/empyric/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/tools.py` & `empyric-0.2.6/empyric/tools.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/empyric/types.py` & `empyric-0.2.6/empyric/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 class Type(ABC):
     """Abstract base class for all supported data types"""
 
     pass
 
 
 class Boolean(Type):
-    """Abstract base class for all boolean types; `bool` and `np.bool_` are
-    subclasses"""
+    """Abstract base class for `bool` and `numpy.bool_`"""
 
     pass
 
 
 Boolean.register(bool)
 Boolean.register(np.bool_)
 
@@ -65,51 +64,47 @@
 
 
 ON = Toggle("ON")
 OFF = Toggle("OFF")
 
 
 class Integer(Type):
-    """Abstract base class for all integer types; `int` and `np.integer` are
-    subclasses"""
+    """Abstract base class for `int` and `numpy.integer`"""
 
     pass
 
 
 Integer.register(int)
 Integer.register(np.integer)
 
 
 class Float(Type):
-    """Abstract base class for all float types; `float` and `np.floating` are
-    subclasses"""
+    """Abstract base class for `float` and `numpy.floating`"""
 
     pass
 
 
 Float.register(float)
 Float.register(np.floating)
 
 
 class String(Type):
-    """Abstract base class for all string types; `str` and `np.str_` are
-    subclasses"""
+    """Abstract base class for `str` and `numpy.str_`"""
 
     pass
 
 
 String.register(str)
 String.register(np.str_)
 
 
 class Array(Type):
     """
-    Abstract base class for all array-like types, essentially any commonly
-    used type that can be indexed; `list`, `tuple`, `numpy.ndarray`,
-    `pandas.Series` and `pandas.Dataframe` are subclasses
+    Abstract base class for `list`, `tuple`, `numpy.ndarray`, `pandas.Series`
+    and `pandas.Dataframe`
     """
 
     pass
 
 
 Array.register(list)
 Array.register(tuple)
@@ -125,14 +120,17 @@
 }
 
 
 def recast(value: Any, to: type = Type) -> Union[Type, None]:
     """
     Convert a value into the appropriate type for the information it contains.
 
+    If a subclass of `Type` is passed to the optional `to` keyword argument,
+    the value is reast to that type. Otherwise, recasting goes as follows.
+
     Booleans are converted into numpy booleans; integers are converted into
     64-bit numpy integers; floats are converted into 64-bit numpy floats.
 
     Array-like values are converted into the analogous numpy array.
 
     Strings are inspected to determine if they represent boolean or numerical
     values and, if so, recasts values to the appropriate types. If a string
@@ -153,15 +151,14 @@
     if to != Type:
         if value is None:
             return None
 
         for dtype in np.array([to], dtype=object).flatten():
             # Recast to desired type
             try:
-
                 if get_origin(dtype) is Union:
                     # Expand type unions
                     return recast(value, to=get_args(dtype))
 
                 if issubclass(dtype, Boolean):
                     return np.bool_(value)
                 elif issubclass(dtype, Toggle):
```

### Comparing `empyric-0.2.5/empyric/variables.py` & `empyric-0.2.6/empyric/variables.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.5/pyproject.toml` & `empyric-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empyric"
-version = "0.2.5"
+version = "0.2.6"
 description = "A package for experiment automation"
 authors = ["Daniel Merthe <dmerthe@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dmerthe/empyric"
 packages = [
     { include = "empyric"},
 ]
@@ -17,14 +17,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "1.24.3"
 scipy = "1.9.3"
 matplotlib = "3.6.2"
 pandas = "1.5.3"
 pykwalify = "1.8.0"
+bayesian-optimization = "1.4.3"
 "ruamel.yaml" = "0.17.21"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pylint = "*"
 black = "*"
```

### Comparing `empyric-0.2.5/PKG-INFO` & `empyric-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: empyric
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for experiment automation
 Home-page: https://github.com/dmerthe/empyric
 Author: Daniel Merthe
 Author-email: dmerthe@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bayesian-optimization (==1.4.3)
 Requires-Dist: matplotlib (==3.6.2)
 Requires-Dist: numpy (==1.24.3)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pykwalify (==1.8.0)
 Requires-Dist: ruamel.yaml (==0.17.21)
 Requires-Dist: scipy (==1.9.3)
 Project-URL: Repository, https://github.com/dmerthe/empyric
```

