# Comparing `tmp/m3u8-4.0.0.tar.gz` & `tmp/m3u8-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u8-4.0.0.tar", last modified: Tue Dec 12 23:16:33 2023, max compression
+gzip compressed data, was "m3u8-4.1.0.tar", last modified: Mon Apr  1 17:41:15 2024, max compression
```

## Comparing `m3u8-4.0.0.tar` & `m3u8-4.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2023-12-12 23:16:33.344994 m3u8-4.0.0/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-12-29 01:47:32.000000 m3u8-4.0.0/LICENSE
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2022-12-29 01:47:32.000000 m3u8-4.0.0/MANIFEST.in
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15735 2023-12-12 23:16:33.344740 m3u8-4.0.0/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15465 2023-07-25 22:57:47.000000 m3u8-4.0.0/README.rst
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2023-12-12 23:16:33.342951 m3u8-4.0.0/m3u8/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2525 2023-12-12 23:06:49.000000 m3u8-4.0.0/m3u8/__init__.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1023 2023-05-11 22:24:51.000000 m3u8-4.0.0/m3u8/httpclient.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1369 2023-12-12 23:06:49.000000 m3u8-4.0.0/m3u8/mixins.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    53969 2023-12-12 23:06:49.000000 m3u8-4.0.0/m3u8/model.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    22773 2023-12-12 23:06:49.000000 m3u8-4.0.0/m3u8/parser.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1750 2023-12-12 23:06:49.000000 m3u8-4.0.0/m3u8/protocol.py
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2023-12-12 23:16:33.343765 m3u8-4.0.0/m3u8.egg-info/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15735 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      441 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/SOURCES.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/dependency_links.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/not-zip-safe
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       61 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/requires.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2023-12-12 23:16:33.000000 m3u8-4.0.0/m3u8.egg-info/top_level.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       58 2023-12-12 23:06:49.000000 m3u8-4.0.0/requirements.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2023-12-12 23:16:33.345038 m3u8-4.0.0/setup.cfg
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      655 2023-12-12 23:11:18.000000 m3u8-4.0.0/setup.py
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2023-12-12 23:16:33.344462 m3u8-4.0.0/tests/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     6149 2023-12-12 23:06:49.000000 m3u8-4.0.0/tests/test_loader.py
--rwxr-xr-x   0 mauricio.antunes   (501) staff       (20)    49093 2023-12-12 23:06:49.000000 m3u8-4.0.0/tests/test_model.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    36766 2023-12-12 23:06:49.000000 m3u8-4.0.0/tests/test_parser.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1073 2023-12-12 23:06:49.000000 m3u8-4.0.0/tests/test_strict_validations.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    13995 2023-12-12 23:06:49.000000 m3u8-4.0.0/tests/test_variant_m3u8.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.522981 m3u8-4.1.0/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-12-29 01:47:32.000000 m3u8-4.1.0/LICENSE
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2022-12-29 01:47:32.000000 m3u8-4.1.0/MANIFEST.in
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15662 2024-04-01 17:41:15.522656 m3u8-4.1.0/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15465 2023-07-25 22:57:47.000000 m3u8-4.1.0/README.rst
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.519748 m3u8-4.1.0/m3u8/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2525 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/__init__.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1023 2023-05-11 22:24:51.000000 m3u8-4.1.0/m3u8/httpclient.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1369 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/mixins.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    53969 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/model.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    23156 2024-04-01 17:38:58.000000 m3u8-4.1.0/m3u8/parser.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1750 2023-12-12 23:06:49.000000 m3u8-4.1.0/m3u8/protocol.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.521018 m3u8-4.1.0/m3u8.egg-info/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15662 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      441 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/SOURCES.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/dependency_links.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/not-zip-safe
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       61 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/requires.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2024-04-01 17:41:15.000000 m3u8-4.1.0/m3u8.egg-info/top_level.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       58 2023-12-12 23:06:49.000000 m3u8-4.1.0/requirements.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2024-04-01 17:41:15.523083 m3u8-4.1.0/setup.cfg
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      655 2024-04-01 17:39:10.000000 m3u8-4.1.0/setup.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2024-04-01 17:41:15.522344 m3u8-4.1.0/tests/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     6149 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_loader.py
+-rwxr-xr-x   0 mauricio.antunes   (501) staff       (20)    49520 2024-04-01 17:38:58.000000 m3u8-4.1.0/tests/test_model.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    36766 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_parser.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1073 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_strict_validations.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    13995 2023-12-12 23:06:49.000000 m3u8-4.1.0/tests/test_variant_m3u8.py
```

### Comparing `m3u8-4.0.0/LICENSE` & `m3u8-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/PKG-INFO` & `m3u8-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: m3u8
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python m3u8 parser
 Home-page: https://github.com/globocom/m3u8
 Author: Globo.com
 License: MIT
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: backports-datetime-fromisoformat; python_version < "3.11"
 
 .. image:: https://github.com/globocom/m3u8/actions/workflows/main.yml/badge.svg
 
 .. image:: https://badge.fury.io/py/m3u8.svg
     :target: https://badge.fury.io/py/m3u8
 
 m3u8
```

### Comparing `m3u8-4.0.0/README.rst` & `m3u8-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8/__init__.py` & `m3u8-4.1.0/m3u8/__init__.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8/httpclient.py` & `m3u8-4.1.0/m3u8/httpclient.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8/mixins.py` & `m3u8-4.1.0/m3u8/mixins.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8/model.py` & `m3u8-4.1.0/m3u8/model.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8/parser.py` & `m3u8-4.1.0/m3u8/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,14 +460,25 @@
 
 
 def _parse_cueout_cont(line, state):
     elements = line.split(":", 1)
     if len(elements) != 2:
         return
 
+    # EXT-X-CUE-OUT-CONT:2.436/120 style
+    res = re.match(
+        r"^[-+]?([0-9]+(\.[0-9]+)?|\.[0-9]+)/[-+]?([0-9]+(\.[0-9]+)?|\.[0-9]+)$",
+        elements[1]
+    )
+    if res:
+        state["current_cue_out_elapsedtime"] = res.group(1)
+        state["current_cue_out_duration"] = res.group(3)
+        return
+
+    # EXT-X-CUE-OUT-CONT:ElapsedTime=10,Duration=60,SCTE35=... style
     cue_info = _parse_attribute_list(
         protocol.ext_x_cue_out_cont,
         line,
         remove_quotes_parser("duration", "elapsedtime", "scte35"),
     )
 
     duration = cue_info.get("duration")
```

### Comparing `m3u8-4.0.0/m3u8/protocol.py` & `m3u8-4.1.0/m3u8/protocol.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/m3u8.egg-info/PKG-INFO` & `m3u8-4.1.0/m3u8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: m3u8
-Version: 4.0.0
+Version: 4.1.0
 Summary: Python m3u8 parser
 Home-page: https://github.com/globocom/m3u8
 Author: Globo.com
 License: MIT
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: backports-datetime-fromisoformat; python_version < "3.11"
 
 .. image:: https://github.com/globocom/m3u8/actions/workflows/main.yml/badge.svg
 
 .. image:: https://badge.fury.io/py/m3u8.svg
     :target: https://badge.fury.io/py/m3u8
 
 m3u8
```

### Comparing `m3u8-4.0.0/setup.py` & `m3u8-4.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_reqs = [
     req for req in open(abspath(join(dirname(__file__), "requirements.txt")))
 ]
 
 setup(
     name="m3u8",
     author="Globo.com",
-    version="4.0.0",
+    version="4.1.0",
     license="MIT",
     zip_safe=False,
     include_package_data=True,
     install_requires=install_reqs,
     packages=["m3u8"],
     url="https://github.com/globocom/m3u8",
     description="Python m3u8 parser",
```

### Comparing `m3u8-4.0.0/tests/test_loader.py` & `m3u8-4.1.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/tests/test_model.py` & `m3u8-4.1.0/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,28 @@
     assert segments[4].cue_out is True
     assert segments[9].cue_out is False
     assert (
         segments[4].scte35 == "/DAlAAAAAAAAAP/wFAUAAAABf+//wpiQkv4ARKogAAEBAQAAQ6sodg=="
     )
 
 
+def test_segment_cue_out_cont_alt():
+    obj = m3u8.M3U8(playlists.CUE_OUT_CONT_ALT_PLAYLIST)
+    segments = obj.segments
+
+    assert segments[1].scte35_elapsedtime == '2'
+    assert segments[1].scte35_duration == '120'
+
+    assert segments[2].scte35_elapsedtime == '8'
+    assert segments[2].scte35_duration == '120.0'
+
+    assert segments[3].scte35_elapsedtime == '14.001'
+    assert segments[3].scte35_duration == '120.0'
+
+
 def test_segment_envivio_scte35_attribute():
     obj = m3u8.M3U8(playlists.CUE_OUT_ENVIVIO_PLAYLIST)
     segments = obj.segments
     assert segments[3].cue_out is True
     assert (
         segments[4].scte35 == "/DAlAAAENOOQAP/wFAUBAABrf+//N25XDf4B9p/gAAEBAQAAxKni9A=="
     )
```

### Comparing `m3u8-4.0.0/tests/test_parser.py` & `m3u8-4.1.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/tests/test_strict_validations.py` & `m3u8-4.1.0/tests/test_strict_validations.py`

 * *Files identical despite different names*

### Comparing `m3u8-4.0.0/tests/test_variant_m3u8.py` & `m3u8-4.1.0/tests/test_variant_m3u8.py`

 * *Files identical despite different names*

