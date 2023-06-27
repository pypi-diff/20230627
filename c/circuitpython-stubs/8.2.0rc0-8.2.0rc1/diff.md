# Comparing `tmp/circuitpython-stubs-8.2.0rc0.tar.gz` & `tmp/circuitpython-stubs-8.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.2.0rc0.tar", last modified: Fri Jun 23 18:32:31 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.0rc1.tar", last modified: Tue Jun 27 17:31:04 2023, max compression
```

## Comparing `circuitpython-stubs-8.2.0rc0.tar` & `circuitpython-stubs-8.2.0rc1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-23 18:32:31.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.2.0rc0/README.rst` & `circuitpython-stubs-8.2.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/_eve/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/_pew/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/_stage/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/aesio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/alarm/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/analogio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/atexit/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audioio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/bitops/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/board/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/busio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/camera/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/canio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/countio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/displayio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/espidf/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/espnow/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/espulp/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/fontio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/getpass/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/gifio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/gnss/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/keypad/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/math/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/mdns/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/nvm/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/os/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/qrio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/random/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/rtc/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/samd/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/setup.py` & `circuitpython-stubs-8.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ssl/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/storage/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/struct/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/synthio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/time/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/touchio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/traceback/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/wifi/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc0/zlib/__init__.pyi` & `circuitpython-stubs-8.2.0rc1/zlib/__init__.pyi`

 * *Files identical despite different names*

