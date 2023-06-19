# Comparing `tmp/lps22hh-0.3.0.tar.gz` & `tmp/lps22hh-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lps22hh-0.3.0.tar", last modified: Fri May 19 12:42:56 2023, max compression
+gzip compressed data, was "lps22hh-0.4.0.tar", last modified: Mon Jun 19 07:22:51 2023, max compression
```

## Comparing `lps22hh-0.3.0.tar` & `lps22hh-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:42:56.841566 lps22hh-0.3.0/
--rw-r--r--   0 chris      (501) staff       (20)     1072 2023-05-19 06:32:49.000000 lps22hh-0.3.0/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:42:56.841169 lps22hh-0.3.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1912 2023-05-19 12:40:55.000000 lps22hh-0.3.0/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:42:56.835143 lps22hh-0.3.0/lps22hh/
--rw-r--r--   0 chris      (501) staff       (20)       28 2023-05-19 12:40:05.000000 lps22hh-0.3.0/lps22hh/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    11086 2023-05-19 12:40:05.000000 lps22hh-0.3.0/lps22hh/lps22hh.py
--rw-r--r--   0 chris      (501) staff       (20)     2081 2023-05-19 09:44:38.000000 lps22hh-0.3.0/lps22hh/register.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:42:56.840362 lps22hh-0.3.0/lps22hh.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:42:56.000000 lps22hh-0.3.0/lps22hh.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      209 2023-05-19 12:42:56.000000 lps22hh-0.3.0/lps22hh.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-19 12:42:56.000000 lps22hh-0.3.0/lps22hh.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-19 12:42:56.000000 lps22hh-0.3.0/lps22hh.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-19 12:42:56.841695 lps22hh-0.3.0/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      980 2023-05-19 12:41:23.000000 lps22hh-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:22:51.490737 lps22hh-0.4.0/
+-rw-rw-rw-   0        0        0     1072 2023-05-19 06:32:49.000000 lps22hh-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4288 2023-06-19 07:22:51.489754 lps22hh-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2266 2023-06-19 07:15:36.000000 lps22hh-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 07:22:51.467683 lps22hh-0.4.0/lps22hh/
+-rw-rw-rw-   0        0        0       28 2023-05-19 12:40:05.000000 lps22hh-0.4.0/lps22hh/__init__.py
+-rw-rw-rw-   0        0        0    11078 2023-05-31 10:30:52.000000 lps22hh-0.4.0/lps22hh/lps22hh.py
+-rw-rw-rw-   0        0        0     2081 2023-05-31 10:29:53.000000 lps22hh-0.4.0/lps22hh/register.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:22:51.475685 lps22hh-0.4.0/lps22hh.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-06-19 07:22:51.000000 lps22hh-0.4.0/lps22hh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-19 07:22:51.000000 lps22hh-0.4.0/lps22hh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:22:51.000000 lps22hh-0.4.0/lps22hh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 07:22:51.000000 lps22hh-0.4.0/lps22hh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      772 2023-06-19 07:22:31.000000 lps22hh-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:22:51.490737 lps22hh-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 07:22:51.487759 lps22hh-0.4.0/tests/
+-rw-rw-rw-   0        0        0     3304 2023-06-19 06:58:27.000000 lps22hh-0.4.0/tests/tests.py
```

### Comparing `lps22hh-0.3.0/LICENSE` & `lps22hh-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lps22hh-0.3.0/PKG-INFO` & `lps22hh-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,65 @@
-Metadata-Version: 2.1
-Name: lps22hh
-Version: 0.3.0
-Summary: Raspberry Pi Pico Micropyhton library to interact with the ST LPS22HH Barometric pressure sensor
-Home-page: https://github.com/cbraissant/lps22hh_pico_driver
-Author: Chris Braissant
-Author-email: chrisbraissant@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Embedded Systems
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LPS22HH Pico Driver
-
-Micropython library for the ST LPS22HH pressure sensor
-
-## Overview
-The LPS22HH sensor is a high-resolution digital output pressure sensor manufactured by STMicroelectronics.
-This driver enables seamless integration of the LPS22HH sensor with the Raspberry Pi Pico.
-
-## Features
-- Interface to communicate with the LPS22HH pressure sensor.
-- Reading of pressure and temperature values
-- Configuration of registers via dedicated functions
-- Communication via SPI (I2C not implemented yet)
-- Designed to be compatible with the Raspberry Pi Pico running on Micropython. Other boards not tested
-
-## Installation
-```bash
-pip install lps22hh
-```
-
-## Getting Started
-```python
-from machine import SPI, Pin
-from lps22hh import LPS22HH
-
-# Create a new SPI device, and assign the pins corresponding to your device
-cs_pin = Pin(1, Pin.OUT)
-spi = SPI(0, baudrate=1000000, firstbit=SPI.MSB, sck=Pin(2), mosi=Pin(3), miso=Pin(0))
-
-# Create a new instance of the LPS22HH sensor
-sensor = LPS22HH(spi, cs_pin)
-
-# By default, the device is in power-down mode and the ODR need to be changed
-# for the device to take continuous measurements
-sensor.data_rate = 200
-
-# The Block Data Update (BDU) is used to inhibit the update of the output
-# registers until all output registers parts are read, to avoids reading values
-# from different sample times
-sensor.block_data_update = 1
-
-while True:
-    if sensor.new_pressure_data:
-        print(sensor.pressure)
-```
-
-## TODO
-- [ ] FIFO functionalities
-- [ ] Interrupts
-- [ ] I2C, I3C communications
-
-## Contributing
-Contributions to this project are welcome. If you find any issues, have suggestions for improvements, or want to add new features, feel free to open an issue or submit a pull request.
-
-## License
-This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code in accordance with the terms of the license.
+# LPS22HH Pico Driver
+Micropython library for the ST LPS22HH and the LPS27HH pressure sensor
+
+## Overview
+The LPS22HH and LPS27HH sensors are high-resolution digital output pressure sensors manufactured by STMicroelectronics.
+This driver enables seamless integration of the sensors with the Raspberry Pi Pico.
+
+## Features
+- Interface to communicate with the LPS22HH and LPS27HH pressure sensor.
+- Reading of pressure and temperature values
+- Configuration of registers via dedicated functions
+- Communication via SPI (I2C not implemented yet)
+- Designed to be compatible with the Raspberry Pi Pico running on Micropython. Other boards not tested
+
+## Installation
+Use `pip` (see [Python Package Index ](https://pypi.org/))
+
+```bash
+> pip install lps22hh
+```
+
+or 
+
+Use `mip` (see MicroPython [Package management](https://docs.micropython.org/en/latest/reference/packages.html)):
+
+```bash
+> mpremote mip install github:cbraissant/lps22hh-pico-driver
+```
+
+## Getting Started
+```python
+from machine import SPI, Pin
+from lps22hh import LPS22HH
+
+# Create a new SPI device, and assign the pins corresponding to your device
+cs_pin = Pin(1, Pin.OUT)
+spi = SPI(0, baudrate=1000000, firstbit=SPI.MSB, sck=Pin(2), mosi=Pin(3), miso=Pin(0))
+
+# Create a new instance of the LPS22HH sensor
+sensor = LPS22HH(spi, cs_pin)
+
+# By default, the device is in power-down mode and the ODR need to be changed
+# for the device to take continuous measurements
+sensor.data_rate = 200
+
+# The Block Data Update (BDU) is used to inhibit the update of the output
+# registers until all output registers parts are read, to avoids reading values
+# from different sample times
+sensor.block_data_update = 1
+
+while True:
+    if sensor.new_pressure_data:
+        print(sensor.pressure)
+```
+
+## TODO
+- [ ] FIFO functionalities
+- [ ] Interrupts
+- [ ] I2C, I3C communications
+
+## Contributing
+Contributions to this project are welcome. If you find any issues, have suggestions for improvements, or want to add new features, feel free to open an issue or submit a pull request.
+
+## License
+This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code in accordance with the terms of the license.
```

### Comparing `lps22hh-0.3.0/lps22hh/lps22hh.py` & `lps22hh-0.4.0/lps22hh/lps22hh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Author: Chris Braissant
 #
 # Driver for the ST LPS22HH:
 # High-performance MEMS nano pressure sensor:
 # 260-1260 hPa absolute digital output barometer
 
 from machine import SPI, Pin
-from lps22hh.register import Register, Bits
+from register import Register, Bits
 
 _INTERRUPT_CFG = 0x0B
 _THS_P_L = 0x0C
 _THS_P_H = 0x0D
 _IF_CTRL = 0x0E
 _WHO_AM_I = 0x0F
 _CTRL_REG1 = 0x10
```

### Comparing `lps22hh-0.3.0/lps22hh/register.py` & `lps22hh-0.4.0/lps22hh/register.py`

 * *Files identical despite different names*

