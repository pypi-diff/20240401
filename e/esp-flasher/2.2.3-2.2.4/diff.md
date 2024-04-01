# Comparing `tmp/esp_flasher-2.2.3.tar.gz` & `tmp/esp_flasher-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp_flasher-2.2.3.tar", last modified: Sun Dec 17 12:11:15 2023, max compression
+gzip compressed data, was "esp_flasher-2.2.4.tar", last modified: Mon Apr  1 11:41:28 2024, max compression
```

## Comparing `esp_flasher-2.2.3.tar` & `esp_flasher-2.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:11:15.043413 esp_flasher-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-17 12:11:15.039413 esp_flasher-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:11:15.039413 esp_flasher-2.2.3/esp_flasher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   273167 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/esp_flasher/own_esptool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:11:15.039413 esp_flasher-2.2.3/esp_flasher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 12:11:14.000000 esp_flasher-2.2.3/esp_flasher.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-17 12:11:15.000000 esp_flasher-2.2.3/esp_flasher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 12:11:15.043413 esp_flasher-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-12-17 12:10:23.000000 esp_flasher-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:41:28.417315 esp_flasher-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 11:41:28.417315 esp_flasher-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:41:28.417315 esp_flasher-2.2.4/esp_flasher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   274083 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/esp_flasher/own_esptool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:41:28.417315 esp_flasher-2.2.4/esp_flasher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 11:41:28.000000 esp_flasher-2.2.4/esp_flasher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:41:28.421316 esp_flasher-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-01 11:40:42.000000 esp_flasher-2.2.4/setup.py
```

### Comparing `esp_flasher-2.2.3/LICENSE` & `esp_flasher-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esp_flasher-2.2.3/PKG-INFO` & `esp_flasher-2.2.4/esp_flasher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: esp_flasher
-Version: 2.2.3
+Name: esp-flasher
+Version: 2.2.4
 Summary: ESP8266/ESP32 Tasmota firmware flasher for ESP
 Home-page: https://github.com/Jason2866/ESP_Flasher
 Author: Jason2866
 Author-email: obermeier.johann@googlemail.com
 License: MIT
 Keywords: home,automation
 Platform: any
```

### Comparing `esp_flasher-2.2.3/README.md` & `esp_flasher-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `esp_flasher-2.2.3/esp_flasher/__main__.py` & `esp_flasher-2.2.4/esp_flasher/__main__.py`

 * *Files identical despite different names*

### Comparing `esp_flasher-2.2.3/esp_flasher/common.py` & `esp_flasher-2.2.4/esp_flasher/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 def read_chip_info(chip):
     mac = ":".join(f"{x:02X}" for x in read_chip_property(chip.read_mac))
     if isinstance(chip, esptool.ESP32ROM):
         model = read_chip_property(chip.get_chip_description)
         features = read_chip_property(chip.get_chip_features)
         num_cores = 2 if "Dual Core" in features else 1
         frequency = next((x for x in ("160MHz", "240MHz") if x in features), "80MHz")
-        has_bluetooth = "BT" in features or "BT 5" in features
+        has_bluetooth = "BLE" in features or "BT" in features or "BT 5" in features
         has_embedded_flash = "Embedded Flash" in features
         has_factory_calibrated_adc = "VRef calibration in efuse" in features
         return ESP32ChipInfo(
             model,
             mac,
             num_cores,
             frequency,
```

### Comparing `esp_flasher-2.2.3/esp_flasher/const.py` & `esp_flasher-2.2.4/esp_flasher/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 
 ESP32_DEFAULT_OTA_DATA = (
     "https://raw.githubusercontent.com/Jason2866/ESP_Flasher/factory/"
     "partitions/boot_app0.bin"
 )
 ESP32_DEFAULT_BOOTLOADER_FORMAT = (
     "https://raw.githubusercontent.com/Jason2866/ESP_Flasher/factory/"
```

### Comparing `esp_flasher-2.2.3/esp_flasher/gui.py` & `esp_flasher-2.2.4/esp_flasher/gui.py`

 * *Files identical despite different names*

### Comparing `esp_flasher-2.2.3/esp_flasher/helpers.py` & `esp_flasher-2.2.4/esp_flasher/helpers.py`

 * *Files identical despite different names*

### Comparing `esp_flasher-2.2.3/esp_flasher/own_esptool.py` & `esp_flasher-2.2.4/esp_flasher/own_esptool.py`

 * *Files 2% similar despite different names*

```diff
@@ -2232,15 +2232,15 @@
 
     def get_chip_description(self):
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return "%s (revision v%d.%d)" % (self.CHIP_NAME, major_rev, minor_rev)
 
     def get_chip_features(self):
-        return ["WiFi", "BT"]
+        return ["WiFi", "BLE"]
 
     def get_crystal_freq(self):
         # ESP32S3 XTAL is fixed to 40MHz
         return 40
 
     def get_flash_crypt_config(self):
         return None  # doesn't exist on ESP32-S3
@@ -2344,16 +2344,16 @@
     SPI_USR2_OFFS   = 0x20
     SPI_MOSI_DLEN_OFFS = 0x24
     SPI_MISO_DLEN_OFFS = 0x28
     SPI_W0_OFFS = 0x58
 
     BOOTLOADER_FLASH_OFFSET = 0x0
 
-    # Magic value for ESP32C3 eco 1+2 and ESP32C3 eco3 respectivly
-    CHIP_DETECT_MAGIC_VALUE = [0x6921506f, 0x1b31506f]
+    # Magic values for ESP32-C3 eco 1+2, eco 3, eco 6, and eco 7 respectively
+    CHIP_DETECT_MAGIC_VALUE = [0x6921506f, 0x1b31506f, 0x4881606f, 0x4361606f]
 
     UART_DATE_REG_ADDR = 0x60000000 + 0x7c
 
     EFUSE_BASE = 0x60008800
     EFUSE_BLOCK1_ADDR = EFUSE_BASE + 0x044
     MAC_EFUSE_REG  = EFUSE_BASE + 0x044
 
@@ -2417,15 +2417,15 @@
             0: "ESP32-C3",
         }.get(self.get_pkg_version(), "unknown ESP32-C3")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return "%s (revision v%d.%d)" % (chip_name, major_rev, minor_rev)
 
     def get_chip_features(self):
-        return ["Wi-Fi", "BT"]
+        return ["Wi-Fi", "BLE"]
 
     def get_crystal_freq(self):
         # ESP32C3 XTAL is fixed to 40MHz
         return 40
 
     def override_vddsdio(self, new_voltage):
         raise NotImplementedInROMError("VDD_SDIO overrides are not supported for ESP32-C3")
@@ -2753,15 +2753,15 @@
             1: "ESP32-C2",
         }.get(self.get_pkg_version(), "unknown ESP32-C2")
         major_rev = self.get_major_chip_version()
         minor_rev = self.get_minor_chip_version()
         return f"{chip_name} (revision v{major_rev}.{minor_rev})"
 
     def get_chip_features(self):
-        return ["Wi-Fi", "BT"]
+        return ["Wi-Fi", "BLE"]
 
     def get_minor_chip_version(self):
         num_word = 1
         return (self.read_reg(self.EFUSE_BLOCK2_ADDR + (4 * num_word)) >> 16) & 0xF
 
     def get_major_chip_version(self):
         num_word = 1
@@ -5466,283 +5466,291 @@
 qFIFn0wnXlwk3mS40efw0bGLR3Ivs4gBwB/78MMBg8uWQJEVcpMMsAuGsz3mqrjW7yCzVNXz6wDpg4tzQoTYDH8eJHKMgfJ8a+/EPnbdz7ujAO+R/u6n82IFt0lrNU2zNJmkmfmleXu++sV7OI7Nw7o4L/ja6c4l\
 ubj7xp4VLsXFck9Uwh8OoUEtJhi2dMtvyXasmuX2G9Wt2AZKb3rhNlvWchWrbUDU1Ta8FygKXsu1xeAj4qlLxYlO2+i84zUuaOz+4xekRmnQipOEavbSfrt8RDLnN3cDcBotv2hJR81YISfcgEJ7cPpN4xnp/mtm\
 vKzxb+Kk/uNzr3fJ1jch0ycSCDU7NyhJh+bSa3TmVpltfPWpwP7uxsKDClBoG/DFrmTtkuK+BZL02n3vs3dS1e4D+nSPgKx6e7s3t3+tFBp8nYBlxybq2Hr9+7E7d5LrDbdy615/3fs97rWTXjvttSe9dtZrV71M\
 Rj+z0ekf+I1OT/8qcH169eXSf+hHX9OOP5GHruOp63is355c055e086ubJ9f0Xp7RatzTfjGdnVle3XV3rn286n7dvJJODr/hHX3IW+vkQI9yHUPkv4d8boz3pbfuOk3OsPe8Rudqyg7FkqHIL3/ZiLrwVn02lWv\
 3SQbdon+E3fxf1sK/F4p8XulyO+VMr9XCl3X/sSPVi7gaXfgFHceBQrFZbEXIMh9gBIZtDttk467dKW7bP36xnIyjVWaZb/9P7DMz0g=\
 """)))
 ESP32ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
+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\
 """)))
 ESP32S2ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
+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\
 """)))
 ESP32S3ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
+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\
 """)))
 ESP32C3ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
+eNq9Wgtz1EYS/ivGTiCQVG60q9ckwV5jrxcbTCAFcUGWi6UZieAEH3aWYCrsf7/5uns0I+FdKnVVVymylubRPT3dX7/0961Fc7W49d1GfWt3fpUkm/Mrk950/xvNr1Tuft2/uijcQ3qK8Vmx716WO/MrW7o/aoym\
+fnSMP+SfcjPMZH6lk/lVWfNv4/apR5NNt4Ue7Tt6CoOOUulml6WbnWBJMn43v2ozN9zysHbrrAUpXpIk8jf+qdNHzGbpyFfa/dLbI7BZHBKzOE/1E04mh2pwTCObELenyxd0gIX7j5g36iFeuKc23ZlfOubdy3Y0\
+qfe3HJkSi5J7bns72sehDjcdQZVVg/M4nm75Ha851tK9dTs1jvNEu31aN2LcEepWpFnwUuV41akTWAUChXtKnPSbjEfLbIb/QQrgDfNp5MOzwI3KZoZF0+S0anGAZ8uiU2rZzb3Hyz35Ws0vd7E9WMj4DhUmakdU\
+u5cm4VNBlnosAnaLwKT70wqTuuSptG8WjuUZ9EutW7p8JsRscf1iMBWW1sU7iG1nlzUDO5E0MLHyalztmKlQJpV+T0tkdjHDHbohqJBXrJKfbT7jh979eXaTXNTF2wtp9BYUXNjnm97iaZW/UGxcyMY6eeX5ENIp\
+hNc4aiTsgv8gq+NrEXYrLMQRYSDEex54r4tcjrjisPSQH7iHHORarxpbvI+hfUShrH/AsZjCDR5p9QkrME4P6bSGjLxn3bKljbdshE827MLZCczw4wNHwzJk0G5tUawY8JvLtXu0sqBS+/22IqGMisiiStGqMX73\
+lmJ75QkxDzlPAx1oTal7JxoS1TtLIc0UJhEPnlJ4Tsye29ny7kNhBRwuGLLo4rXYIyPPEdkY37kWmh07BN9mfk7Ak04LLbZgZwGjeRv3m+wb6Dixhh1SwBnkXDLNOmWMchAB6hl00OwXTIuQRfGu0EHj7VUDL2US\
+iVsQu81FosrZUonDFzdFJuRPoJZiTbq8R7eyOxPnwSgGiL5q9MQr/tZXX4hTMCyt4GBw5YcDL+PdR+QGvizEC5hm549wHpUJIGs5lCn5GYpbqg33oDwgY/Y04GM9mrHwyH6LjW1xULqIVWAm/iefXEMUsAn50Klo\
+y+kqTsSc7DgT8PeOqueQdoPbNB5MvPZ67Cm9GmWzLd65KQJvUG4Tozkd+xV8WMHuFMZkZKSFJ7bfsVAgJfzWpHHuHybXWzzABrNbwAfGMP+YHcTQPPwd0t2tthDy+RidSXjAN37EHNK16aE5OGrtmDklsG54ABbG\
+1nYbMlU3WcGT8XP21iQgc988Y5Xgx33zbxYCnGWd3SV4uD+5CcwFI+yjVupWkwwcDg4N6fMpJySbOS2cTxjj3F5zYnS+z5s7/ZmzfEQdXKyCkMVFKz3VeJ29QcgxgLRVykaRHeQJhAQZsu3RxPGaUNyQ8R9KrQNM\
+k+G+EX5o+KPIt3UYPd+TAAUz1Uymj7zVQAIErQcUC1QX7u/6CVsNqSdmZICY8pHsnXfRyVULxtrlX2GkzXcueLXVgk2GL+pagPZH+bDDT05vL6fx3ER8MsvvlYRqeGF6GxBab/I9kVqmq2UPDITGVZZC0kh2Ph7x\
+/q30BptH4JJG4xn/bcSfU9wyhoPPGaVVFJNxrGZYdW0a7VgILo/NO0E79QaxDoVFMnFFxD9QiH64i4CkChFuHPdNi/BsKA70Mn/eD5w5SKTYuuat2uYiWmxpnEPXFbnPHb6OWoRXEzuG71avP54YiBcCBZ7p8Q6A\
+GgSzCxCqHwlYWqhw9hp/LcCGBU5ppCzZz4yrxJAEnqUgVluxpHXSYfiCzy54QGkCBYOyivEcx9JAouzbdfo24fX9nf2OKjsLsSdtX8124aZT9grvRH0y1jWwqmP7ji6CxrWEGQLOupAovksBBosBzh3pbt6dz2NX\
+ksGVmoT8NTk8wrE6iLKtJmdAy2r/CGhZHd5xt6Gro/lllN5VlAOZP3Fwb1KvH4mJwNlnR+sgXt6Nr0H5xva2ubluG1yRegR/RCqa7j5heGTRgkr+LLKKLu/CuWxyIZrn7usRJPgT4g6nb3b8b1Y2SsjaTbgux4at\
+jwCOLlG2sChjETHXZ9DUc6/H74MYe3BebItCGlFIuuNtn7NKGNB2rvlblivyFPrNOfI32ThSBcXe1YcNXUkA9qu214u/kSSgzF4ZoMOJF5FdfpBKAEUIPcUVADVVbF1jntj4ssNqqqdYvvxbKJnvWe1pdyOZjY7k\
+JtSG1NlMaibSiLa7OF628QZDhtE9/3RsPh7PF4Y9X4UtxqgnwL6RGZI6Z2LaADEEoLUuNlkVsTFlHWtVkdKREUdH9Is8tkVIi5Faoswq3SU23uO1IKuuJhJ8sTX9DFzq0X70GdrQlMiUnnFiCVUwtH7/w0uc6tjR\
+p7ulOFfV65WEDD1dSiA3niZiobksS34wPwazgqtpRhy0tBTgDfP6QuQSI7Pokq2kTAABVGIL7DX4zqDd5MwQT2ecPupkJsk3XqTiuSP0jQgP0fj/jb6nIHNxV8C3GT+5+0wPbZZtuUmGNr79Gatq808g/PHZUwj1\
+6RGigur5nRdQshfz818w+ODsIQYfHh1j8Ph2FReTTnYPwcdFuLu2yyqmgswNX6Q1UtioGBQoh20Yue2IY6Xu74pCDlqLOY2oJpQJa5uKD9ZgPN/mSSvVHZW32sVPiAJtVMikkNjl5/txTB3VZLss2Txcvg9Y0xY7\
+kjxw4iaBBmEakg0KhY1Xmgl7hpXXgSKRy4BYb3Ud9kq8OgkXKtE3AnZz4fYUMa0tH/sCFb0/D6xiD9JRqRckwcAWWxteawpJL8rWl0TzftgKE0tGgQgtq8O2/u4NEdflXlTNKFWcZ4wHFGoJygdVt6DPoYZXUxHN\
+r/fCSSSwHnOwCMG1ze73GJn+BiO90NVY6ilFFP9LZe/GK/K1kEXb1QKxZTmRevgg429oqvbcfyC2n+T9ejit0JQ9GnqHNE91VS5zOgXxkqGgzKbT6Xrfa1thK0OdXCUHoXDLePq5DRo16EzIdfCmAVFWp9hqfUWl\
+9XfJJTzzK1WeMskda8nRJdhCauC1u0ym610KDmqodhvXLwDofrtOVSiubHc7YYVyGoFRnA1wje2Id7s8Wx95lo1YTi0uFwUTXUkXpZDCRsnuFHdF7+vwvqQakQO/hdR0IW9IhpoDY0nba+41YCqoNTIO9Y3nK8LK\
+Y2pRJL40/IQehW+V38ajbkNNiol8HwrqpvhaCjeS1PpE3imH4cw2XotTlrUHpL1thusqQ/CSTO9D+E/yf0bmFVLAwizE8tJhx6K16TB5bbLoFQWlwH/iRCe7fO0r7IRshSKC6RpPYZPQKZvPZ4NMYNQHZ6dvc7q6\
+hSin9lfHV3UszPTv19FAN6nx3SWKJQ/EtzVdCfhhcEdUJ2v5CFX5wSv+exEctcEOBAJL3gMRVV38xZh6HmIa8hBo6dRdzrsnPBSDuojkDq0vcdCdEZnX7KdbE7tEyS5irkpLx2KWzlcxdIDLvY6bpCvejaJ2WtJZ\
+AHzWvo8zEo44LtJn+XEedJJ6hu/SdxzwkVRddOuD31TaU9kP/o3hN7VNn+cSQTZ8CU01tNTDmaGu08iZLOb+xSfHxFYAzpe1WSJ3adqpn9a5vLKKUnzyh0kIdTW6H+XIF873cTa3uo6buj6bIPxFFKFnbwUOIRwn\
+F8OI6S2aYmjFUcoQ7GpfWScb09BXONJE3f3BC88y5muuGw12ORVSPtDCVoRT0h2ANlP623NRb8epL8jfxh83CM+ywDKzhAusbbCrygRYoueU++x8kFec1JHRCfxQl6pgblrxrCXUpKWy5B+bHG+RezHLpQ/7zeSY\
+A9YaCq6lkEs6Se7pjzBRLJkIA7XtxzCGFriRsv5qWfyO2jjAG1UzLrl9ds0Z1iRnvMYmUqZbt6ZSr5+Ajk8q0THn4PKG5Emlh6lmAEi+HU3BtEXPif6i7hPdE1ZrWd36rw2ycDVKnvnqXo642THcYBQ26HrNtUg+\
+oUJEJZjQeBIPxN339g+3Ddtuqb23glQavJ0n5RyVOWOloXqMd/l15ByvpxuXEUeBCXi/Vm+x8rI4t76Qyo1v/XmfwcNCtqtnDPyxiUKrcD2Czq13deo+eJwFlCeBNOYgoDfj2y+x934Q+aOhC+cZv2MGvoMoXvJr\
+3uVvkfxgTSNCwaU2aeA58V84QACZeKqmU5cDyTsS8caFtMcaDpMoIeqJjE0Yz9agaYtuuJefE4V07HjuEiSrXtQzimK7OrpbL/VExvP44vOgNOsVfp1RPke92QQ0lHZ07b0XqaxlmKY4PihxFaIK+r5EwpirOt1r\
+3kvnkZo8lLU2jBP4HXKHNrahdvZMXMhwBc0gg9n7dLCV5Tb9lRrXkv8BPu0aJ2DUicTlNqiuV19fzFHiYaHE1sxCjkiBfd1p6/Il1rxnGLL6/v4quhM4tHL/KRWHJ/4wJuS93C6/Byoz4aldRr2vRpRqJKqJhhX0\
+yvpPk3BJkG6d9TGnYBZs82mEzbpGurV1x6ebW1+xP1bqmBWiHH/pi3MeAqj3n3GNlWrSAbZRTzVfiiqN57cOqYnbiohzL/JY3vKxBNnw+KtDn0odEJD4KByRdu0Nlns+r/v35r9tsAqHqbrDWM6iET2PBxZPdfpE\
+cnv/kYPKDlgCdXujJ0nJgix9hPSF8JlII7rrWhPCOA4WQp9+x2mIfOiSxj2hbYijg1bqgRcsBbIIgJLBoFbRyq6+v0FfepW+WGRCkCvNN93IRxHi80z6fZy/US61CQov2T1fr9Mb90J0RJUj6h+m1H+hMHhTnLtU\
+wenLAQLGCYo6aSKZd79Nrx2Q/kLWfR6cGRTI5O+4gGxKrC/zKOvy/vp6Prevb9VTqRC5GX0U2fiPGg1fqEWxrO5qMrsykq5GFqXuapLpookyuuwiktIghvwcThv1be+rSijfg6jZriKzJHGcSGhO6Uvhv+eRT7S6\
+HnpcaBpLaoOX9IGL+KXVruNfUZ1aba+aefq1aGX6P/qwWAXa4k3Y0WSfKq2AdKQSlQAmFIe+XEgY4f22FQBWHXI5NQ7gjLrLyLrKQISWTw2S2GCc8uwKYFuPHvRB6ANJYkqpAvqaujdkr5IIJOoQhF2KRVpKUe6H\
+O2zMZFu6kvisVcI7mGDLAcrl/Xswne9YdePgsK43Z6P78gERVbuoUZJ95DCpy+MrUSkpfQXFlux9pTV8MyyGUo2q8B35kyjYKTnFE124FPFaFibXjLelwD462WLjaWQRNSeRqKI2n0nhFjrflUiLcAotauDxoKII\
+X0vKptQLSQdJTj92n+++oRULFiIhA/ppiD6a8Y9vcUzDUYeq4+bMWwE9SSXLjIx32X0DKp9oddVfKy5Xe8Uy0twSJ0+KpKQoboQTinUl7tRRZ9Q7jkqHyDX2/rRZHtb1lL/9FMRWg5R8+hxjtV6nGIh0Xkdf90bZ\
+dCNVSHJuZV9hQ7NjPfIwGPLK/0i0PuKUtbJM1m/btNwea/PHLXpT+dMD9Kby5zfRm8pfAGfhjPIHLbpT+cMD3FB+PF907alb32zQ9/q//rmoLvHVfqKKIk2SMlVupDlfXH7oXo6zMnUvbbWo6PN+CG4iCuDEeE6f\
+29P9lpPf+IearXhPQOb+esw/l/MF3rYjniaDH/lpkwdr1Xt0l0wUmuspkYuiAQcnbsEGP1Ql/6I/qZp4HVWPLktp9GIMl0jf2Nuq9+If//yMfcNuZZ/MLZFhLHKV5KlO8uV/AaGtV00=\
 """)))
 ESP32C6ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-eNq9Wm1zFDcS/ivGTnDgUkTa3XlRALMGr9c2mEAKQkE2CTMajQ9f8MXOcjEV9r+fnu7WSjP2Lrm6uvtg77xI6lar++m3+XN77i7n299u1Nu7s0utN2eXdnTT/xvMLlXuf/1fXcwuW/+n1FsMmeJyNLssR+PZZVP6\
-MbWMGYUxQx5Bf8oPsn6k0X5Kzb/Oj64H4809fzvY84QVXnqSpR9dln60xhQ9/OBXzfzrll8bP69pmBqmaC3XzN1T5rf05Cvjf+npkX/or+bEMHZWfY89yvYcNmxlFeZ/8YZ2MMcUcG/VEzyYywbb2YXfgH/eDsb1\
-3pYnVeKxfnjoeRvsYWOHm56oyqrenjxf22HRa7a28E/9Ss5zr41fp/VvrN9G3YpEC56qPLtm5IVWgUDh77Q/BJfx2zKb4h8kAd4wnt58fBm5UdnUsnhcTrPm+7hvWHxKLZZjH/L0QL5Ws4tdLA8WMj5HhYHGEzX+\
-odW8K4jTDEXGfhKY9JeNMGlKHkrrZnFbgcEwtfFTFy+FWFNcPxlMxal1kYHB8S5rB1Yqs4l/XgWFrh7YiZAl5S5ovAz1NxYb9VMV1CgoV8n3TT7lm875BXZ1LhoTjIe0egtKLuzzSW/xsCocKBYuZGGjTyIrRHoE\
-4TkxwUHBwiXjC8cSOK4wFxuFnRD7eWSfLDSXmat3TffB8HHOug1qssULWlpQlKsJN9gik7rBb1rzipUZkoCkWktG37F2WbJJl3TCMBt6wab96bEn0TCC0GJeGtsr3oTFRQUCjDVNIRv3s7YS4QyKxLhKUbAhfh8t\
-xAzLV8Q7RD6JZKBDpelsqE/TPFgIZaYwjiwEQstbbR/5dRteuy+piM50+nKOJuACQdARGRufvJEXS2YI1O3sjBBoNCn8AAvraaY9wAZJvWeh7CRirDACrkHIJdOsRwxWHitIkR6A+72CaRHEKF7ViGqR4RoApwwi\
-YeuoliRP5Y2qxOaLXGRC/gVGI2Zlyod0JrtT8SQMZ4DrS2fGQf23vvpCPIRlsI/eBgd+2HM5wZckLuHLQsRq3YNf435UJshsZFOYjntoLa5J9QcBnDFhErGyHkxZfmTLxcaOOCxTJEowFW+Uj68hCwSFhGhftOJk\
-FS8b/kYNM3ECwWF1HNNudKFlAJWguh0M0iTlLSbhisgYNNumqE5bPoEvK9izwpKsvGnhlZtvWSCQEH5rUjj/h8H1Fr9ga9kt4AtTuH/GjqJvHeEI6ehWGwi5fyjEVEIFPvAj5pCOzPStwVNrh8wpgbbj1WFgbGy3\
-IFN1k/VbD1+z1yYB2QP7EqcQbvfszywEOM06u0/YcICohCDXsedeeZwUGqSOB5uG9HmXY5LNjDYzGzPA+bVmxOhsjxf3yjNjkxB18DELQhcftXRU4132HqFHD8+uZ21MWOFFMWEaZNeDsWdUU/CQ8YVS66DSZgX8\
-uM1iSLc8wTJB6Gb0iEVtXXEym79NgqOCV/Q4KiDDYLpgz9yCchvgZyg2gYeuZ1fDFfAbmH0vhLxaXkzSsVr8LovnRGQFA7B/VZC2Oi/iwcalG4kE1zLWDxThvqsYG3YjpkY/iI8sPYqLO8PHkEZ+ooA1L9g6CKCI\
-SzQ0hKO/FbnEbbadWgysJr4sy81IsrAyLyD1CikFhW+jY78DR2FCdg5C9VPBmQYRYfYOV3Ow0cDEDQL/7Ac+YGJIYjdGCz+4Yk0xeql2c96+mBJF2hRMySyGQmzLwIizO/x4lXOw6pv+ymFFlZ3G2I2Wr6a7OIgR\
-A+oHsfKMTQysmkTvVXIQ9N6IgxZcM8WQXyyj6N5k4NqS9HLc7XXair+v4X+sJh9HeksQUEc5ttX4FChT7R0BZarD2/4oTHU0u0jSo4pyCPs7dh3SmHdPGRWBLGV2tA4aJeo216CjazrL3Fy/jLeC7adAF1LQ0e7z\
-xAgykMlfJvlYkriQdWb6XFTPH9hTiPB7AItXuGb4M2sbJTXtJmDfs9LUR5j6BrZYQ0sRatan2MpZUOQ/oih158h2RCOtaCQd8k7I+8SFtku3dodlWw/kN+eIWWVZoguKPVNwucvUGgasdtbJ7u0G3p5YYMOrIJ9m\
-8VFSafKrHZ0dSepSpYY15IEuJO7rzgqRn3aLP4WYvctKTwSspAMmEZoQ7DPARlIzHSe67uNfWSaYC5nF8v77Y/vpeDa37D8qLDFEQo7o2DwQfc7EsAFhcC+1KTZZF7EwReuf0UUCb6wFd0e/yAVbxILwMrV4xmq0\
-S5z8gccCraYaS+DCFvUDgKlD/uk68giku1nuS07IoAqW5u99/AkbO/b06YQpRlT1+k2RsaPSQUHQcKLFSsk4n9+z30Wzgq9xAy5LtBQZ9RPjQoSS4rKoU1NJno3dV2II7DP4zKDa5M0QiGYcKRg9lYw141oP8pIU\
-exPCfSz+/2Mv6b86vy8A7IbP7wNtTN9s2Zyd7pv5zmfN6+IKlD87fQHZvjh6DVG/vv0GivZmdvYjXj4+fYKXT46O8fL4VpUWZV7tHoKR83iErYTp7DKAi47Ps7FSFKgYHigFdIzgDd6PkuuK4g6aizFO1BMKhbmu\
-4tDe4X2+w4PWWVylzjWFoXp1cBnyMwpQt5jpVlLauhN58q+WAgjiS6vbq8FmlWmJwri2iay7fouKUFM+iyUZKtMkfgBRE+mX5MhaxhGuqq2NkGiHOmAetW85bBCnp5UgkDFlCKM56HrOTHPRordmErFfqSypJF1c\
-VqsqqhKFVYJdaL4m02/4YFo3uYs3k7/DoD4YvKvTIli3gHXjhPwiNt8mhS/FqBbKwHEWMehouAlbMbKBJsu7lWAj/omqsuR4M6mPJiJQ+u1kmpayLFUgJ5M1WNsGq83kgdL7oXYZEHH9AtXVMr0cVVg3oME6aA58\
-eM2C7pflL/CFkyBtkt05ZFBdSe3WMFdRqnQixlB0kxRNwV6720YJhNIQIUOIz0Npyg864zO8OF1D0wgZ79nPJPMH06XUdClDL9ksEXXR8zo+L6nY4VFoLoVJSA9+g6rdQ9Y2xGwonmMoaDl5Xw274xWB1jHV3HWo\
-bz6nW2FZ5bdwa9pYXGEid2OF2BZ/kwqEVFoRcxKKaJqbd+dil2UtJ2Mf7YCFCdWIJweQ+of8P6NxgmyssHPRsVE/m6xM3s8mjU4eUaHO3YfXaVAyDTZ8vcqT2pN7Xqf1Lun9zGbTXlgukOYEKb2iofBRiPO3Jhwb\
-H9OxsNM9Wx+YozXiQquE4rp9cTBuWcZ8EotGVOxpeQdV+TEo/B8iN+rp7AvElbwGohuqeAJ1zmJ8UUqBqq6X2ecj4SFpryjhmsqKuXgiOjIi846dJYrvwexaiQ06XJUNbauWbZWrWaLOQHsdS3pZhhpYRh/HghcT\
-8NfNHtn1+T36eXkP4ocooT1BNaUR1uh7H6TnBgH7iDMEpNSGwxJ8CyBuX99b5BLSOT4JV/VN9XCK2KAt7nibxdh/8fYxEECgi1icZbHcp2Fvw7ClayurJOMOLlPF8NMgSCgHoQK8xx0KV/8meAdgY3QrWGOKtqPa\
-c0iKAaUhz4dZpiGh7WlONGhZwpN25Tofh6NQ/r2FixsEOllEClrEi7eK2l/ZCBx0P+IOL2dBJ5wGkWkIRlA3pGA+WjHRslywYVn96ya3Bgn87WIRAmU7fsmxXg01NFI2pEr5kObFgWJvRBi42nzqLqKkgny9FHA0\
-H1CGBbyiysQlqs/OmWOOPuU5jZay1ro5Ss2fg07IwdCk5Tz6hmQWIbtt+7DBhQQmMpVAkJocdEKYagSH2tDhzuK5KLkP5+ayAdfV+2sM4hrL9mYtktecvYvR2kDlsTjjPgk67QdwxdlqOqPojAId70qsdDOR3gY2\
-wlbWEE1rboOob6jHlHqLNZdlufWFVDlChynAOr/GOCcWrCILYWtWJ2HKKK2lhs4N6ccBeJxGIKYzdXY/Aiyjz4+pf32cuIy+k+UR/8AI9N2Ln/gxr/KniL03h5RK84m6PPKspTCFNkXdCHK7pbrsi3eRvENJ8xeV\
-cBcaQh2RiTWj42P3BNxJfgMShXSGeOwCtbCqE5QMktCrTs42SF3L+zw9+DwqzecUfpVFlqpBcdZ2cJDKzuRSoK/UAMskYo4aXCVev0esXI3cGHDKiUydRYUJSkPuSXyHs6w6DRp+IT+iGLte6sjiJ8z5yMbfNAd7\
-6+g+hTfee4EmdcgpShChCkP4YMY+BKGpsIXWCLSItMmx26VqPSSElgUONHQevIBQwW2uRSV3TdjJJ0wnunUzJFgwTSepFnX4sevhlwyNqfVRdzeThKvtwOVbaQICeGqisx2abhgZejws/VT0YvRUUx9+FRt1FHt6\
-Yw6xKr7WqYPRcJPiXecU51LKHWFj1XJjjYmd7nrYszpNJyQpbuhnq2xfmi3tjY5cxXIagsgvkp6i9B2DodPZW8/GXJig32F4ow5FRlF6Gyw90vu654bKpRsa9t4YlUwbhtBngz7tKYcx1Q0xoHSLjGTBtRV8G91N\
-8xtKNzZB4Sf279er98ZxjE3o0y1qe42oYUDx4SbPpuKdE+1A8qvGqOyOtHxW1O3HGo9kP5KTOovehMxBf2DltCXml3mSmARveT2fh9f3ZCnOQR2KvoRz4Us2y0fpETUWc0sEGY3sc7WxH7Bh1G42d0nek50nguoF\
-cZ/HyrLzNR2qT49jRStk5WSfJJFXUwEV8knh0w35FCc4qDottAwl7MVDKoKJb1jFUqVMUlpVOyvlnoli5v+lH0m1AGkZgtZaghibXVVdQe1EMSqBT6gPfVGnuULCK/8TTR+BVBvJAbVsdZ9xdpWZCK0QnuvUbLwK\
-7Qp8N2J4mr4DfGwlIJdiWKgBB3NmxXzPuxSXfCFG2VCCcBDP0NnxjnTSCHI5xIIV8qefs4uDh8gPv2Xt5d19hyeb08FBIYIaiQmU2SdJbBgoz0SbpCiUVtTX6YhSRb8cqMr42Uo5eJXEGiWVK4IaXIhYGxYi/bY7\
-7NTqwastthsnk6iPVpPN+TRFKnxQ92VpsAh7MHL4AQsqiq2NJEtKvZEsrI31goYiWPWeJs1ZgAQM9KkDAHb43W/wQZYrVqpOewm/CebJt7FlRoZ7X9JVemTTymcjKYZ05Cizsknnv41xPAhVAaUo3GxFhVxUpzIN\
-N4uroQAtVsZ5nZ2bqxi2GqM2e1A9WpfCSdSBpmc/lXXJRz7G9hbN/xrqbIRp30g2TC26BRMMC1YtZ49t/qxF9yR/sY/uSf76Jron+RugK7xQ/rhF/yR/so9SVH48my8bKNtfb9Bn2r/8Pq8u8LG2VuVAD9VoOPBv\
-3Nn84uPy4UBrPGyqeUVfdUsqoOj0d6h2iujQR3vh0uXxacXnzTXlPLmhHqfc0CeE/mI/eV+mg9tquSJ9dlvSzZ1kRPKYmnc8/Oe17N2W30CeNIkvb8qrp+z++0v4ZxfhMk+GtNWyM3Dn+sf/0xtq0turb76+jttt\
-OdSODoxyMzCDxb8B397NZQ==\
+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\
+PFn+C4psGGw=\
 """)))
 ESP32H2ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
-XMbtthxqTwfGKsnTbPVvMfzUqA==\
+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\
++hfcvBvW\
 """)))
 ESP32C2ROM.STUB_CODE = eval(zlib.decompress(base64.b64decode(b"""
-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\
+eNqtWgt3EzcW/ishaUOh3XZkz0MCNrHBiWOScEoPLEvqlM5oZljYki2pWZJDvb999d17ZWkc23QfJ8exZ0bSvbqP7z40n27PmqvZ7Xtb1e3pVaKmV8p9qsL9xif5+cn0yubTK92fXpXGfdPdx+6mLibuf7m/i/8/\
+uH+pe+JG2mbb/bOySEqLzM/cuv3pzP25S/c4OcENd9Wm+9PL6VXjbra9QTXacWQ0JqmHbvm6N3Lr9CbbjmCSlY58z33cWK0HxNNtv6Lqf3ArZO6i5VGmmLu7bqXGca6MW6d1T6zbQtUSM7JB93G8mnToCINA4a6U\
+dtMyfqqzMf5BCuAN4+nJ9fPATZKNLYumyWnW7BDXNYsuSeaLsQ95uidfJdPLIZYHC+5+A5Yw0Diixt20incFWZq+CNhNApPuZy1MGs1Dad0sbMsz6KfWbur8uRCri9WTwVSYWhVOsLbaH7JlYCVIgwaWwlBe7tsD\
+oZxjykeaIqML/lRudgIr8ral+brOx3zRUaHnWOViMT2hpcCa04TpyQ5Y2Ts8rPQ6xcKFLGzU68AKkU4hv8ZRI3kX/MPZctCM57jEXGzUFMJ+Htivilw2un7LdJ3zp4KeVevNZIdXs7SaGFftL7A/pnOLn7TmBRsz\
+xAAxtfCx3mDIbsv6kiXreMlGuK1r8FlMb5NL/n7saLg7upLV2qJY88AvLibAKsd6BRkmr7cTiaZXRN6lxcL6+H40Fz/UL4h5CPwg0IEFadPZ0TJRsz8X0kxhEPHgKYVrZR+5lWtefVlYtDTAKi0YvsgCjFgA4Rkh\
+ndgT4I9oLtgB9PXs9IJAKD0o3AALv6jHYkipX8aRUyMLY58KzCYpoA1y1kyzShmvHFzAfDIYox0VTItQJuFVYYnW+64BdsogEregd5uLRBPnVBqbL3ZFJrVmdzLiVkY/JK0MgTmKsdghGuD6qjEDb/47X30hAcLy\
+rpw4t0cw1BFUPtmktS7cwgkSQdjeMu4YGWY1bwDWS4ifCJTLaEujg0qV+CfPey1CdzeaXhdvZRmB+Lb5DMkIGGuaTRougu3sRuCU33WzIBpRfkVYbJk7I5YQ5NYRGdg/8BFTwNTZlGOhZpUug/vKHRPwNR/e77LH\
+2QaXcIEZbOoNfl0KKKX8acsFaMGMC2wqe8xIWwNk2Wyv6pI93Ii1wQSBzjCZitcjr4MIzC6ofcsETLFGtqAaU8b23rpLQVtatBwP77hZEEr2ev4h+BWCUGuCu/pPSeEg4icIjqaUK6YIQUzVGQc4mbqe92Rb0gLl\
+lFaZfajyALeqSCzl4C40XY6mFxP45Mv2DMI8m0SpDFE19jfeOKccb55wwIDcNZQBSqvNdOAtPAqeMKqm7qyx69dYsR8AnK6eAE1IuOnwZWxxsKr8OfKm9+/JfpAStsj46r8g6P0kcERxZxtJiSNW9x3XtTpDylXB\
+ogD6/bdsVo1YJSVcJsirY+G9b1kiVU++c45JgAyCrdXiOMJGXzubbewLBiGd1fNZZDhdm2eHW2U422tFtoUn80+ypr0fWaKVwGn4YUygS7DiHTTeo9SEp4vhkfEvrlTv1H46nc7sewlD/WvE9nnGLgk2EUaUnmTn\
+pOqcZrsbmzehxKXhr8bYDxMGkEocpDRDt0irPka307t0D64r5koGlnaoPtlksRxh6n7HaJ9zfkLKTSlaXp8jhT51XPQlYuKTVJuW/hmz5yx+h6aKxzQkoj8p+ySYVyORAZkOYoCzmaUcsQhw5xGpLiXVxA2kmq2W\
+bDhlmnAaii5uYplx5mHUmG9CPG3KoVnAbBmJlsHtvwazDogxruH21iow+4hIeD+GsxZEbHZ/2SM3aTS/gX3f330GI3k2vXgJVidvgQjl48fHeHh89wQPT6YXp5DI+WmEiL4KjarJp0ocxzb7v8SCkLpuHV/If23p\
+SztMOAiVVtUbs/yoDCi29hDBr02cPY6ljM0HK4ii+kJqRQkRrXewjhMSfD+TAtIXu52idhhKb+urEZ8/ecP0aZ9Lz3ZE8EVgDEmxjSvCgg2NUwWkXVbSBTyBfen6HouDrCbjigWoADe21Q4/4MxtCPs0can4PePd\
+clrtFUiKW59Z77JmbDqWFgOr+zFzuAgNnTTaI49ssmwYzgGJnKXfGcnShua+5IqfBGSPrAOZ1ifSdmR/EqDoIc3bo7LiaCA4ZptNOOPUWVUrgi6kz7sckGymNHE6WEDJlBidjgSzW7qRLsyh7o3Q9qh6k6V+R13n\
+77hzURUvhhNo4n0wC9gvN00O9oT1XCKsJHClJHCQOOX/jSR1eJ5Gv0tKc2kuxgAiYTiAUMxtShYFIrjNN6fOJeWtY1L+jfI4iex2UW+XlmMDVkEpVGYIq+rgb1JuczQXnF2U7N2K+9brPQLpLXFrLR6c6YHva+FX\
+og6XmKm6zY0kkf6WYyU7oOWMzwnXRzUVdc6m0/FNAK2WHYL2WlBFNGXH3IRlqhSZEj5p/QruigS0uCYBv4fXlGAZpDP+8TmmK9xHnwPhShXdck1RQtoOWy/HUGdSwutLCV/nVsVj3t3l281USy9ww59KdXuElD5V\
+bHbs0qW0IQvxas3OV7dyvwr3NQGks/qZNEIg+1ZJd60v1UvFzToMBbVGnlPCEY1PyElOx5LbEeTmT+nS+Ms7uDRtAGQmcj9UZbb4OoRjSLc2Ej4Uzc27c7FLXYny7KM9sDBEWqEOjlgrRu39Z2ReA6YL+y/f9/pj\
+pfeAK9du3b3J701UpVMvYUOJDdRGp0sjbagIMHyX1Xc4oITiHT+1xuuKdTMXo+wq1NUd6L82vh9L6c+hoFizaJSchOhCUaHlbLDU194LPoqkqHF8KEmj5jWQNFbFPxnWLqIMX0J25ZNHpR8JD1EPNxGuKfvIJSck\
+JRGZN4zI6PB5Xwwqi7jSNW2rkW3p9SxR+7FdxZJaxKueZSdrGI7E7t3veuSdfV00pNKV6l/14PTBwYNgp9SFn1BS7qWeqJGPnQCN9ssH/tLSti4fPH0gebRi/TR22WsnY0v9W7gvxl6zUBCfgAmqCJkdC+vPNMz6\
+YYuApMso9ZYoAqv0PV+DDqLu+fRxxEbSVL8KNGLTG2QzkDSmZnipKZhhosooYI9QgmlZGZlX0272Fl33U59G3sGPWwREWUAPWsoJugzOUdoAJnQNwK58pfma8z3yHAENashi98Y0fGXVL9t8JkFRws7nvhCxg3NO\
+MiqYJuVmSpLsPs0LA8UHiRoAtv69u0gi6efa6k6X5wjELWMSn4x8do7BHPWW59RK2nfr57B4tUbZYgQh6IDI0txbvp4TV2mX0YQbdJSmoKdqAWvUXSXNYCqZkHRpCeyzoI9Erllfz5EzmJsL9MMCi0OVSiSvqP2h\
+xZEbT+JYonZnfSXSY1bD+qmsn4Zo5Nd3gcS+YfNA5ePJe/43EJNUwZ9yuaR2h22TpbbzhXR6EoRtJLse2BOf/SfipdQoX4qSVkXZSxo3m32JRy50BM7GAYpJfY09DBDLSPNjHFOPo6CxHFh5xN8xAsd7xTnf5lU+\
+SbthaU4jomglInmelT+4g2Vngt3NwjIO+QZJNpOWNhTYMLrA3XVHZOytuK4tzh9geF5+ThRSRPJYtPjqspOL9KKMq4o06qWu5HkeqzsPprLZttn/IH+qR4PPXqOHbAPOybFG7eNHNrrDvXWlVnlVk8uBqeThV1X6\
+qPkoZXCCTiTVvg2DAb6X+cJZjKUzmbFA/PIMGkEO8ujmw1am1+krOn15ykpH4VW363Y9+Ci5WBYs1lstxUKpLBpp+tR2HCXKaQTw6mR+jjkfGa/r6mi0jiisAOWCHj3DWRzCFW/GSjep8Gc+D0FoLGy1c9mRbJzM\
+qSdGaYdsUbU/a4eSKtpZF2MEP+vmZsbLVkZWBVTg0mtnGwdS4sdGeqT9Lydd96cjrIzDrm070PwzO1epuHxP8P4AjXPY0oq0cy/9WPSViB5b7H/l50gV6dDEZ7tUY3qv5bOfN10t+rO6uod9lYt91bwijrT6S26v\
+kieSCRXh0C7JDlkYVXtrFXDXdLr+RWBVSY9k0WIkpHFMzIQF+u6n4ayR0vF+R4BbLEA6AjNLUU8LdDXSRuo8NEk00zeQii16kUFLLEtsSEbllI50WcibBgC29H5cXX0tbfokPeekYg2evApZEJep6LWldORCSdg2\
+zyb9tNLUohctBqhRUyV1TbeDZBygnpGvX3DWhgeE7eoDN7Otxnydh8aCB801fP64uotEyRVSlNrKaQ81oy0r1AG7GB1lr0N5kq7FmTPuClTNdNZEDYrsfSSlpVxxM14PTjpvDMH4jn3fNMA3+SfJ4sVYQIWCoj+f\
+llcOfISsoq4ORX1qc/Sl61qEdvQqUGuSk6hTnuxtGnkkb0ak/2MsYxP4ThpTgBhftGQ3jVZQOzKJUuATvNCbQ4rVVJp773gtb2P4Rp9Oq6j6TdfS8Km/ih3FGc1QYDvzrkbvOR1bOQ+R3pnv2XoHZlO8ZnlJLnAp\
+blhT8XEUdNfYwZ6cDzHUUnIHv2s5O7k8eohq+R7bK2/wH5ixPe4dSTebOmUN1fC/S+PDl9llaFGpRXP+4HOmMVluHiY6dNZ170WU42hujonqL4VcLcdc+G73OMhWvRc77CuNTKIOdkV+5ooh6WpQDpNEDX3ZghGt\
+e/cvKYc38qZPkpxh++f8Rs87GjZjmZH3o9mNfKPpD35FsLScZyRVIJYUv0aZZUuqhvnMFy8wyQnBoqMqHFX+qNTyADJ1ieyN78UDJhthhlJbSXdx01uQjw9VlKjGIZ8Wk0CLHSyK6tVZi7mJXqsHb+WbjMGchugS\
+V8X+RSsKXuVGbraKP4g1ZSKNRSomQbXNv2+fwd6fHeLIPX+5ewatn4H2j3h83J7g8ckh2MxPp7PFmcDtb7bozc1Xv83KS7y/qZKiSJXSaeKeNBezy+vFzX4/Sd3NupyV/kVPRBL2LHpHSw++mc7oncoU3z9MLyiV\
+afD9C19Ql4J753T7Cd82GhP+6p85E4kvSbT0siZA5QYdMSkaQNHA/XrobyDiyaN8ermYWRMm0wAsbok3eveUyKQ37/0/fl16ohGp3jIjt0XIsU6SnslMkc//DdOgaK8=\
 """)))
 
 
 def _main():
     try:
         main()
     except FatalError as e:
         print('\nA fatal error occurred: %s' % e)
         sys.exit(2)
 
 
 if __name__ == '__main__':
     _main()
+
+
```

### Comparing `esp_flasher-2.2.3/esp_flasher.egg-info/PKG-INFO` & `esp_flasher-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: esp-flasher
-Version: 2.2.3
+Name: esp_flasher
+Version: 2.2.4
 Summary: ESP8266/ESP32 Tasmota firmware flasher for ESP
 Home-page: https://github.com/Jason2866/ESP_Flasher
 Author: Jason2866
 Author-email: obermeier.johann@googlemail.com
 License: MIT
 Keywords: home,automation
 Platform: any
```

### Comparing `esp_flasher-2.2.3/setup.py` & `esp_flasher-2.2.4/setup.py`

 * *Files identical despite different names*

