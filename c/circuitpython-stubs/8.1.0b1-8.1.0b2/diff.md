# Comparing `tmp/circuitpython-stubs-8.1.0b1.tar.gz` & `tmp/circuitpython-stubs-8.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.1.0b1.tar", last modified: Thu Mar 30 20:37:05 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.1.0b2.tar", last modified: Wed Apr 26 22:56:15 2023, max compression
```

## Comparing `circuitpython-stubs-8.1.0b1.tar` & `circuitpython-stubs-8.1.0b2.tar`

### file list

```diff
@@ -1,230 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.598649 circuitpython-stubs-8.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-30 20:37:05.598649 circuitpython-stubs-8.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.586649 circuitpython-stubs-8.1.0b1/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.598649 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-30 20:37:05.000000 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-03-30 20:37:05.000000 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:37:05.000000 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:37:05.000000 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-30 20:37:05.000000 circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    39554 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-30 20:37:02.000000 circuitpython-stubs-8.1.0b1/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.590649 circuitpython-stubs-8.1.0b1/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:37:05.598649 circuitpython-stubs-8.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-30 20:37:04.000000 circuitpython-stubs-8.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:37:05.594649 circuitpython-stubs-8.1.0b1/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-30 20:37:03.000000 circuitpython-stubs-8.1.0b1/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.912837 circuitpython-stubs-8.1.0b2/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-26 22:56:12.000000 circuitpython-stubs-8.1.0b2/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40051 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.916837 circuitpython-stubs-8.1.0b2/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:56:15.924837 circuitpython-stubs-8.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 22:56:15.000000 circuitpython-stubs-8.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 22:56:14.000000 circuitpython-stubs-8.1.0b2/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:15.920837 circuitpython-stubs-8.1.0b2/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-26 22:56:13.000000 circuitpython-stubs-8.1.0b2/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.1.0b1/README.rst` & `circuitpython-stubs-8.1.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/_bleio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/_eve/__init__.pyi` & `circuitpython-stubs-8.1.0b2/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/_pew/__init__.pyi` & `circuitpython-stubs-8.1.0b2/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.1.0b2/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/_stage/__init__.pyi` & `circuitpython-stubs-8.1.0b2/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.1.0b2/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.1.0b2/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.1.0b2/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/aesio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/alarm/__init__.pyi` & `circuitpython-stubs-8.1.0b2/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.1.0b2/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/alarm/time/__init__.pyi` & `circuitpython-stubs-8.1.0b2/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.1.0b2/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/analogbufio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/analogio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/atexit/__init__.pyi` & `circuitpython-stubs-8.1.0b2/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/audiobusio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/audiocore/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audiocore/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class RawSample:
     """A raw audio sample buffer in memory"""
 
     def __init__(
         self, buffer: ReadableBuffer, *, channel_count: int = 1, sample_rate: int = 8000
     ) -> None:
-        """Create a RawSample based on the given buffer of signed values. If channel_count is more than
+        """Create a RawSample based on the given buffer of values. If channel_count is more than
         1 then each channel's samples should alternate. In other words, for a two channel buffer, the
         first sample will be for channel 1, the second sample will be for channel two, the third for
         channel 1 and so on.
 
         :param ~circuitpython_typing.ReadableBuffer buffer: A buffer with samples
         :param int channel_count: The number of channels in the buffer
         :param int sample_rate: The desired playback sample rate
```

### Comparing `circuitpython-stubs-8.1.0b1/audioio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/audiomixer/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/audiomp3/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/bitbangio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.1.0b2/bitmaptools/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -269,7 +269,48 @@
 
     :param bitmap dest_bitmap: Destination bitmap.  It must have a value_count of 2 or 65536.  The stored values are 0 and the maximum pixel value.
     :param bitmap source_bitmap: Source bitmap that contains the graphical region to be dithered.  It must have a value_count of 65536.
     :param colorspace: The colorspace of the image.  The supported colorspaces are ``RGB565``, ``BGR565``, ``RGB565_SWAPPED``, and ``BGR565_SWAPPED``
     :param algorithm: The dither algorithm to use, one of the `DitherAlgorithm` values.
     """
     ...
+
+def draw_circle(
+    dest_bitmap: displayio.Bitmap, x: int, y: int, radius: int, value: int
+) -> None:
+    """Draws a circle into a bitmap specified using a center (x0,y0) and radius r.
+
+    :param bitmap dest_bitmap: Destination bitmap that will be written into
+    :param int x: x-pixel position of the circle's center
+    :param int y: y-pixel position of the circle's center
+    :param int radius: circle's radius
+    :param int value: Bitmap palette index that will be written into the
+           circle in the destination bitmap
+
+    .. code-block:: Python
+
+       import board
+       import displayio
+       import bitmaptools
+
+       display = board.DISPLAY
+       main_group = displayio.Group()
+       display.root_group = main_group
+
+       palette = displayio.Palette(2)
+       palette[0] = 0xffffff
+       palette[1] = 0x440044
+
+       bmp = displayio.Bitmap(128,128, 2)
+       bmp.fill(0)
+
+       bitmaptools.circle(64,64, 32, 1)
+
+       tilegrid = displayio.TileGrid(bitmap=bmp, pixel_shader=palette)
+       main_group.append(tilegrid)
+
+       while True:
+           pass
+
+    """
+
+    ...
```

### Comparing `circuitpython-stubs-8.1.0b1/bitops/__init__.pyi` & `circuitpython-stubs-8.1.0b2/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/board/__init__.pyi` & `circuitpython-stubs-8.1.0b2/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/busio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/camera/__init__.pyi` & `circuitpython-stubs-8.1.0b2/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/canio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ./microcontroller/__init__.pyi
 ./msgpack/__init__.pyi
 ./neopixel_write/__init__.pyi
 ./nvm/__init__.pyi
 ./onewireio/__init__.pyi
 ./os/__init__.pyi
 ./paralleldisplay/__init__.pyi
+./picodvi/__init__.pyi
 ./ps2io/__init__.pyi
 ./pulseio/__init__.pyi
 ./pwmio/__init__.pyi
 ./qrio/__init__.pyi
 ./rainbowio/__init__.pyi
 ./random/__init__.pyi
 ./rgbmatrix/__init__.pyi
@@ -172,14 +173,15 @@
 memorymonitor/__init__.pyi
 microcontroller/__init__.pyi
 msgpack/__init__.pyi
 neopixel_write/__init__.pyi
 nvm/__init__.pyi
 onewireio/__init__.pyi
 paralleldisplay/__init__.pyi
+picodvi/__init__.pyi
 ps2io/__init__.pyi
 pulseio/__init__.pyi
 pwmio/__init__.pyi
 qrio/__init__.pyi
 rainbowio/__init__.pyi
 rgbmatrix/__init__.pyi
 rotaryio/__init__.pyi
```

### Comparing `circuitpython-stubs-8.1.0b1/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.1.0b2/circuitpython_stubs.egg-info/top_level.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 memorymonitor-stubs
 microcontroller-stubs
 msgpack-stubs
 neopixel_write-stubs
 nvm-stubs
 onewireio-stubs
 paralleldisplay-stubs
+picodvi-stubs
 ps2io-stubs
 pulseio-stubs
 pwmio-stubs
 qrio-stubs
 rainbowio-stubs
 rgbmatrix-stubs
 rotaryio-stubs
```

### Comparing `circuitpython-stubs-8.1.0b1/countio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/cyw43/__init__.pyi` & `circuitpython-stubs-8.1.0b2/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/digitalio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/displayio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/displayio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 import typing
 from typing import Optional, Tuple, Union
 
 import busio
 import circuitpython_typing
 import microcontroller
-import paralleldisplay
 import vectorio
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
+CIRCUITPYTHON_TERMINAL: Group
+"""The `displayio.Group` that is the displayed serial terminal (REPL)."""
+
+import paralleldisplay
+
 def release_displays() -> None:
     """Releases any actively used displays so their buses and pins can be used again. This will also
     release the builtin display on boards that have one. You will need to reinitialize it yourself
     afterwards. This may take seconds to complete if an active EPaperDisplay is refreshing.
 
     Use this once in your code.py if you initialize a display. Place it right before the
     initialization so the display is active as long as possible."""
@@ -318,15 +322,16 @@
     """Gets the height of the board"""
     rotation: int
     """The rotation of the display as an int in degrees."""
     bus: _DisplayBus
     """The bus being used by the display"""
     root_group: Group
     """The root group on the display.
-    If the root group is set to ``None``, the default CircuitPython terminal will be shown.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
     """
     def fill_row(self, y: int, buffer: WriteableBuffer) -> WriteableBuffer:
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data
         """
@@ -370,14 +375,15 @@
         busy_state: bool = True,
         seconds_per_frame: float = 180,
         always_toggle_chip_select: bool = False,
         grayscale: bool = False,
         advanced_color_epaper: bool = False,
         two_byte_sequence_length: bool = False,
         start_up_time: float = 0,
+        address_little_endian: bool = False,
     ) -> None:
         """Create a EPaperDisplay object on the given display bus (`displayio.FourWire` or `paralleldisplay.ParallelBus`).
 
         The ``start_sequence`` and ``stop_sequence`` are bitpacked to minimize the ram impact. Every
         command begins with a command byte followed by a byte to determine the parameter count and
         delay. When the top bit of the second byte is 1 (0x80), a delay will occur after the command
         parameters are sent. The remaining 7 bits are the parameter count excluding any delay
@@ -411,14 +417,15 @@
         :param bool busy_state: State of the busy pin when the display is busy
         :param float seconds_per_frame: Minimum number of seconds between screen refreshes
         :param bool always_toggle_chip_select: When True, chip select is toggled every byte
         :param bool grayscale: When true, the color ram is the low bit of 2-bit grayscale
         :param bool advanced_color_epaper: When true, the display is a 7-color advanced color epaper (ACeP)
         :param bool two_byte_sequence_length: When true, use two bytes to define sequence length
         :param float start_up_time: Time to wait after reset before sending commands
+        :param bool address_little_endian: Send the least significant byte (not bit) of multi-byte addresses first. Ignored when ram is addressed with one byte
         """
         ...
     def show(self, group: Group) -> None:
         """
         .. note:: `show()` is deprecated and will be removed in CircuitPython 9.0.0.
           Use ``.root_group = group`` instead.
 
@@ -448,15 +455,16 @@
     rotation: int
     """The rotation of the display as an int in degrees."""
     bus: _DisplayBus
     """The bus being used by the display"""
 
     root_group: Group
     """The root group on the epaper display.
-    If the root group is set to ``None``, the default CircuitPython terminal will be shown.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
     """
 
 class FourWire:
     """Manage updating a display over SPI four wire protocol in the background while Python code runs.
     It doesn't handle display initialization."""
 
     def __init__(
```

### Comparing `circuitpython-stubs-8.1.0b1/dualbank/__init__.pyi` & `circuitpython-stubs-8.1.0b2/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/espcamera/__init__.pyi` & `circuitpython-stubs-8.1.0b2/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/espidf/__init__.pyi` & `circuitpython-stubs-8.1.0b2/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/espnow/__init__.pyi` & `circuitpython-stubs-8.1.0b2/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/espulp/__init__.pyi` & `circuitpython-stubs-8.1.0b2/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/floppyio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/fontio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/framebufferio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/framebufferio/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -73,8 +73,11 @@
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data
         """
         ...
     root_group: displayio.Group
-    """The root group on the display."""
+    """The root group on the display.
+    If the root group is set to `displayio.CIRCUITPYTHON_TERMINAL`, the default CircuitPython terminal will be shown.
+    If the root group is set to ``None``, no output will be shown.
+    """
```

### Comparing `circuitpython-stubs-8.1.0b1/frequencyio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/getpass/__init__.pyi` & `circuitpython-stubs-8.1.0b2/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/gifio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/gifio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Access GIF-format images
 """
 
 from __future__ import annotations
 
 import typing
-from typing import Union
+from typing import Optional, Union
 
 import displayio
 from circuitpython_typing import ReadableBuffer
 
 class GifWriter:
     def __init__(
         self,
@@ -137,14 +137,16 @@
         ...
     width: int
     """Width of the gif. (read only)"""
     height: int
     """Height of the gif. (read only)"""
     bitmap: displayio.Bitmap
     """The bitmap used to hold the current frame."""
+    palette: Optional[displayio.Palette]
+    """The palette for the current frame if it exists."""
     def next_frame(self) -> float:
         """Loads the next frame. Returns expected delay before the next frame in seconds."""
     duration: float
     """Returns the total duration of the GIF in seconds. (read only)"""
     frame_count: int
     """Returns the number of frames in the GIF. (read only)"""
     min_delay: float
```

### Comparing `circuitpython-stubs-8.1.0b1/gnss/__init__.pyi` & `circuitpython-stubs-8.1.0b2/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/hashlib/__init__.pyi` & `circuitpython-stubs-8.1.0b2/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.1.0b2/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/imagecapture/__init__.pyi` & `circuitpython-stubs-8.1.0b2/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ipaddress/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.1.0b2/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/keypad/__init__.pyi` & `circuitpython-stubs-8.1.0b2/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/math/__init__.pyi` & `circuitpython-stubs-8.1.0b2/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/mdns/__init__.pyi` & `circuitpython-stubs-8.1.0b2/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/memorymap/__init__.pyi` & `circuitpython-stubs-8.1.0b2/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.1.0b2/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/microcontroller/__init__.pyi` & `circuitpython-stubs-8.1.0b2/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/msgpack/__init__.pyi` & `circuitpython-stubs-8.1.0b2/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.1.0b2/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/nvm/__init__.pyi` & `circuitpython-stubs-8.1.0b2/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/onewireio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/onewireio/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Low-level bit primitives for Maxim (formerly Dallas Semi) one-wire protocol.
 
-   Protocol definition is here: https://www.maximintegrated.com/en/app-notes/index.mvp/id/126"""
+   Protocol definition is here: https://www.analog.com/en/technical-articles/1wire-communication-through-software.html"""
 
 from __future__ import annotations
 
 import microcontroller
 
 class OneWire:
     def __init__(self, pin: microcontroller.Pin) -> None:
```

### Comparing `circuitpython-stubs-8.1.0b1/os/__init__.pyi` & `circuitpython-stubs-8.1.0b2/os/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """Sync all filesystems."""
     ...
 
 def urandom(size: int) -> str:
     """Returns a string of *size* random bytes based on a hardware True Random
     Number Generator. When not available, it will raise a NotImplementedError.
 
-    **Limitations:** Not yet available on nRF. Not available on SAMD21 due to lack of hardware.
+    **Limitations:** Not available on SAMD21 due to lack of hardware.
     """
     ...
 
 def utime(path: str, times: Tuple[int, int]) -> None:
     """Change the timestamp of a file."""
     ...
```

### Comparing `circuitpython-stubs-8.1.0b1/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.1.0b2/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ps2io/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/pulseio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/pwmio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/qrio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/random/__init__.pyi` & `circuitpython-stubs-8.1.0b2/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.1.0b2/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/rotaryio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/rp2pio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/rtc/__init__.pyi` & `circuitpython-stubs-8.1.0b2/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/samd/__init__.pyi` & `circuitpython-stubs-8.1.0b2/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/sdcardio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/sdioio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/setup.py` & `circuitpython-stubs-8.1.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.1.0b2/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/socketpool/__init__.pyi` & `circuitpython-stubs-8.1.0b2/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ssl/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/storage/__init__.pyi` & `circuitpython-stubs-8.1.0b2/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/struct/__init__.pyi` & `circuitpython-stubs-8.1.0b2/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/supervisor/__init__.pyi` & `circuitpython-stubs-8.1.0b2/supervisor/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,18 @@
     """Whether CircuitPython may autoreload based on workflow writes to the filesystem."""
 
     ble_workflow: bool
     """Enable/Disable ble workflow until a reset. This prevents BLE advertising outside of the VM and
     the services used for it."""
 
     next_stack_limit: int
-    """The size of the stack for the next vm run. If its too large, the default will be used."""
+    """The size of the stack for the next vm run. If its too large, the default will be used.
 
+    **Limitations**: Stack size is fixed at startup on the ``espressif`` port; setting this will have no effect.
+    """
     rgb_status_brightness: int
     """Set brightness of status RGB LED from 0-255. This will take effect
     after the current code finishes and the status LED is used to show
     the finish state."""
 
 class SafeModeReason:
     """The reason that CircuitPython went into safe mode.
```

### Comparing `circuitpython-stubs-8.1.0b1/terminalio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/time/__init__.pyi` & `circuitpython-stubs-8.1.0b2/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/touchio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/traceback/__init__.pyi` & `circuitpython-stubs-8.1.0b2/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.1.0b2/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/usb/core/__init__.pyi` & `circuitpython-stubs-8.1.0b2/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.1.0b2/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/usb_hid/__init__.pyi` & `circuitpython-stubs-8.1.0b2/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/usb_host/__init__.pyi` & `circuitpython-stubs-8.1.0b2/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/usb_midi/__init__.pyi` & `circuitpython-stubs-8.1.0b2/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/vectorio/__init__.pyi` & `circuitpython-stubs-8.1.0b2/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/watchdog/__init__.pyi` & `circuitpython-stubs-8.1.0b2/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.1.0b1/wifi/__init__.pyi` & `circuitpython-stubs-8.1.0b2/wifi/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -156,74 +156,84 @@
         ssid: Union[str | ReadableBuffer],
         password: Union[str | ReadableBuffer] = b"",
         *,
         channel: int = 1,
         authmode: Optional[AuthMode] = None,
         max_connections: Optional[int] = 4,
     ) -> None:
-        """Starts an Access Point with the specified ssid and password.
+        """Starts running an access point with the specified ssid and password.
 
         If ``channel`` is given, the access point will use that channel unless
         a station is already operating on a different channel.
 
         If ``authmode`` is not None, the access point will use that Authentication
         mode. If a non-empty password is given, ``authmode`` must not be ``OPEN``.
         If ``authmode`` is not given or is None,
         ``OPEN`` will be used when the password is the empty string,
         otherwise ``authmode`` will be ``WPA_WPA2_PSK``.
 
+        The length of ``password`` must be 8-63 characters if it is ASCII,
+        or exactly 64 hexadecimal characters if it is the hex form of the 256-bit key.
+
         If ``max_connections`` is given, the access point will allow up to
         that number of stations to connect."""
         ...
     def stop_ap(self) -> None:
-        """Stops the Access Point."""
+        """Stops the access point."""
         ...
+    ap_active: bool
+    """True if running as an access point. (read-only)"""
     def connect(
         self,
         ssid: Union[str | ReadableBuffer],
         password: Union[str | ReadableBuffer] = b"",
         *,
         channel: int = 0,
         bssid: Optional[Union[str | ReadableBuffer]] = None,
         timeout: Optional[float] = None,
     ) -> None:
         """Connects to the given ssid and waits for an ip address. Reconnections are handled
         automatically once one connection succeeds.
 
+        The length of ``password`` must be 0 if there is no password, 8-63 characters if it is ASCII,
+        or exactly 64 hexadecimal characters if it is the hex form of the 256-bit key.
+
         By default, this will scan all channels and connect to the access point (AP) with the
         given ``ssid`` and greatest signal strength (rssi).
 
         If ``channel`` is non-zero, the scan will begin with the given channel and connect to
         the first AP with the given ``ssid``. This can speed up the connection time
         significantly because a full scan doesn't occur.
 
         If ``bssid`` is given and not None, the scan will start at the first channel or the one given and
         connect to the AP with the given ``bssid`` and ``ssid``."""
         ...
+    connected: bool
+    """True if connected to an access point (read-only)."""
     ipv4_gateway: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station gateway when connected to an access point. None otherwise."""
+    """IP v4 Address of the station gateway when connected to an access point. None otherwise. (read-only)"""
     ipv4_gateway_ap: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the access point gateway, when enabled. None otherwise."""
+    """IP v4 Address of the access point gateway, when enabled. None otherwise. (read-only)"""
     ipv4_subnet: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station subnet when connected to an access point. None otherwise."""
+    """IP v4 Address of the station subnet when connected to an access point. None otherwise. (read-only)"""
     ipv4_subnet_ap: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the access point subnet, when enabled. None otherwise."""
+    """IP v4 Address of the access point subnet, when enabled. None otherwise. (read-only)"""
     def set_ipv4_address(
         self,
         *,
         ipv4: ipaddress.IPv4Address,
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
         Setting the address manually will stop the DHCP client."""
         ...
     ipv4_address: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the station when connected to an access point. None otherwise."""
+    """IP v4 Address of the station when connected to an access point. None otherwise. (read-only)"""
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point, when enabled. None otherwise."""
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
     def start_dhcp(self) -> None:
```

### Comparing `circuitpython-stubs-8.1.0b1/zlib/__init__.pyi` & `circuitpython-stubs-8.1.0b2/zlib/__init__.pyi`

 * *Files identical despite different names*

