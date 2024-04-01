# Comparing `tmp/cgmetadata-0.1.4.tar.gz` & `tmp/cgmetadata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgmetadata-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cgmetadata-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cgmetadata-0.1.4.tar` & `cgmetadata-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      283 2024-04-01 06:13:10.491535 cgmetadata-0.1.4/.bumpversion.cfg
--rw-r--r--   0        0        0      210 2023-11-05 17:41:56.052872 cgmetadata-0.1.4/.gitignore
--rw-r--r--   0        0        0       45 2023-11-01 13:34:11.474743 cgmetadata-0.1.4/.isort.cfg
--rw-r--r--   0        0        0     1494 2023-11-07 14:52:11.477428 cgmetadata-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-10-29 14:57:39.312927 cgmetadata-0.1.4/LICENSE
--rw-r--r--   0        0        0     4432 2024-04-01 06:13:01.854760 cgmetadata-0.1.4/README.md
--rw-r--r--   0        0        0      735 2023-11-07 14:55:11.485102 cgmetadata-0.1.4/README_DEV.md
--rw-r--r--   0        0        0      622 2024-04-01 06:13:01.855887 cgmetadata-0.1.4/cgmetadata/__init__.py
--rw-r--r--   0        0        0       95 2023-11-06 05:19:42.688549 cgmetadata-0.1.4/cgmetadata/__main__.py
--rw-r--r--   0        0        0       50 2024-04-01 06:13:10.490940 cgmetadata-0.1.4/cgmetadata/_version.py
--rw-r--r--   0        0        0    11027 2024-04-01 06:13:01.857637 cgmetadata-0.1.4/cgmetadata/cgmetadata.py
--rw-r--r--   0        0        0    15061 2024-04-01 06:13:01.858544 cgmetadata-0.1.4/cgmetadata/classes.py
--rw-r--r--   0        0        0     5919 2024-04-01 06:13:01.859939 cgmetadata-0.1.4/cgmetadata/cli.py
--rw-r--r--   0        0        0      364 2024-04-01 06:13:01.860898 cgmetadata-0.1.4/cgmetadata/constants.py
--rw-r--r--   0        0        0     2225 2024-04-01 06:13:01.861688 cgmetadata-0.1.4/cgmetadata/iso6709.py
--rw-r--r--   0        0        0    10959 2024-04-01 06:13:01.862863 cgmetadata-0.1.4/cgmetadata/metadata.py
--rw-r--r--   0        0        0      479 2023-10-30 14:27:20.973589 cgmetadata-0.1.4/cgmetadata/types.py
--rw-r--r--   0        0        0     4206 2024-04-01 06:13:01.863628 cgmetadata-0.1.4/cgmetadata/utils.py
--rw-r--r--   0        0        0     3332 2024-04-01 06:13:01.864725 cgmetadata-0.1.4/cgmetadata/xmp.py
--rw-r--r--   0        0        0     1124 2023-11-08 14:42:20.048896 cgmetadata-0.1.4/docs/cli.md
--rw-r--r--   0        0        0     1127 2023-11-07 14:47:41.940223 cgmetadata-0.1.4/docs/index.md
--rw-r--r--   0        0        0       81 2023-11-05 15:02:59.157174 cgmetadata-0.1.4/docs/reference.md
--rw-r--r--   0        0        0      237 2023-11-07 14:46:36.075585 cgmetadata-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0     1101 2023-11-07 04:57:45.027909 cgmetadata-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 cgmetadata-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-04-01 15:16:15.140259 cgmetadata-0.1.5/.bumpversion.cfg
+-rw-r--r--   0        0        0      210 2023-11-05 17:41:56.052872 cgmetadata-0.1.5/.gitignore
+-rw-r--r--   0        0        0       45 2023-11-01 13:34:11.474743 cgmetadata-0.1.5/.isort.cfg
+-rw-r--r--   0        0        0     1494 2023-11-07 14:52:11.477428 cgmetadata-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-10-29 14:57:39.312927 cgmetadata-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5156 2024-04-01 15:15:19.440721 cgmetadata-0.1.5/README.md
+-rw-r--r--   0        0        0      735 2023-11-07 14:55:11.485102 cgmetadata-0.1.5/README_DEV.md
+-rw-r--r--   0        0        0      622 2024-04-01 06:13:01.855887 cgmetadata-0.1.5/cgmetadata/__init__.py
+-rw-r--r--   0        0        0       95 2023-11-06 05:19:42.688549 cgmetadata-0.1.5/cgmetadata/__main__.py
+-rw-r--r--   0        0        0       50 2024-04-01 15:16:15.139516 cgmetadata-0.1.5/cgmetadata/_version.py
+-rw-r--r--   0        0        0    11027 2024-04-01 06:13:01.857637 cgmetadata-0.1.5/cgmetadata/cgmetadata.py
+-rw-r--r--   0        0        0    15061 2024-04-01 06:13:01.858544 cgmetadata-0.1.5/cgmetadata/classes.py
+-rw-r--r--   0        0        0     5939 2024-04-01 15:01:07.390734 cgmetadata-0.1.5/cgmetadata/cli.py
+-rw-r--r--   0        0        0      364 2024-04-01 06:13:01.860898 cgmetadata-0.1.5/cgmetadata/constants.py
+-rw-r--r--   0        0        0     2225 2024-04-01 06:13:01.861688 cgmetadata-0.1.5/cgmetadata/iso6709.py
+-rw-r--r--   0        0        0    10959 2024-04-01 06:13:01.862863 cgmetadata-0.1.5/cgmetadata/metadata.py
+-rw-r--r--   0        0        0      479 2023-10-30 14:27:20.973589 cgmetadata-0.1.5/cgmetadata/types.py
+-rw-r--r--   0        0        0     4206 2024-04-01 06:13:01.863628 cgmetadata-0.1.5/cgmetadata/utils.py
+-rw-r--r--   0        0        0     3335 2024-04-01 15:07:18.298550 cgmetadata-0.1.5/cgmetadata/xmp.py
+-rw-r--r--   0        0        0     1152 2024-04-01 15:00:25.391002 cgmetadata-0.1.5/docs/cli.md
+-rw-r--r--   0        0        0     1127 2023-11-07 14:47:41.940223 cgmetadata-0.1.5/docs/index.md
+-rw-r--r--   0        0        0      263 2024-04-01 15:05:01.251538 cgmetadata-0.1.5/docs/reference.md
+-rw-r--r--   0        0        0      237 2023-11-07 14:46:36.075585 cgmetadata-0.1.5/mkdocs.yml
+-rw-r--r--   0        0        0     1101 2023-11-07 04:57:45.027909 cgmetadata-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 cgmetadata-0.1.5/PKG-INFO
```

### Comparing `cgmetadata-0.1.4/CHANGELOG.md` & `cgmetadata-0.1.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/LICENSE` & `cgmetadata-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/README.md` & `cgmetadata-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,42 @@
 >>> # read metadata from video file
 >>> md = VideoMetadata("test.MOV")
 >>> md.xmp.get("dc:subject")
 ['Coffee', 'Espresso']
 >>> 
 ```
 
+CGMetadata also include a utility function for reading an XMP file and returning a dictionary of metadata using native macOS APIs. This may be useful by itself as it doesn't require the use of external libraries or XML parsers.
+
+<!--
+Setup for doctest:
+
+```pycon
+>>> import shutil
+>>> import os
+>>> try:
+...     os.remove("test.xmp")
+... except Exception:
+...     pass
+...
+>>>  
+>>> cwd = os.getcwd()
+>>> _ = shutil.copy("tests/data/test.MOV.xmp", os.path.join(cwd, "test.xmp"))
+>>> 
+```
+-->
+
+```pycon
+>>> from cgmetadata import metadata_dictionary_from_xmp_packet
+>>> xmp_data = open("test.xmp").read()
+>>> metadata_dictionary_from_xmp_packet(xmp_data)
+{'dc:subject': ['Coffee', 'Espresso'], 'iio:hasXMP': 'True'}
+>>>
+```
+
 ## Installation
 
 ```bash
 pip install cgmetadata
 ```
 
 ## Documentation
```

### Comparing `cgmetadata-0.1.4/README_DEV.md` & `cgmetadata-0.1.5/README_DEV.md`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/__init__.py` & `cgmetadata-0.1.5/cgmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/cgmetadata.py` & `cgmetadata-0.1.5/cgmetadata/cgmetadata.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/classes.py` & `cgmetadata-0.1.5/cgmetadata/classes.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/cli.py` & `cgmetadata-0.1.5/cgmetadata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 from ._version import __version__
 from .classes import ImageMetadata, VideoMetadata
 from .utils import is_image, is_video
 
 
 def main():
-    """Print metadata for image files."""
+    """Print metadata for image and video files."""
     arg_parser = argparse.ArgumentParser(
-        description="Print metadata for image files in various formats."
+        description="Print metadata for image and video files in various formats."
     )
     arg_parser.add_argument(
         "image", metavar="IMAGE_OR_VIDEO", help="path to image or video file"
     )
     arg_parser.add_argument(
         "--version", "-v", action="version", version="%(prog)s " + __version__
     )
```

### Comparing `cgmetadata-0.1.4/cgmetadata/iso6709.py` & `cgmetadata-0.1.5/cgmetadata/iso6709.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/metadata.py` & `cgmetadata-0.1.5/cgmetadata/metadata.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/utils.py` & `cgmetadata-0.1.5/cgmetadata/utils.py`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/cgmetadata/xmp.py` & `cgmetadata-0.1.5/cgmetadata/xmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     xmp: str | bytes | __NSCFData,
 ) -> dict[str, Any]:
     """Extract key-value pairs from an XMP packet.
 
     Args:
         xmp: str or bytes for XMP packet
 
-    Returns: dict with key/value pairs from the XMP packet
+    Returns: dict with key/value pairs from the XMP packet.
 
     Raises:
-        ValueError if XMP packet cannot be decoded
+        ValueError: if XMP packet cannot be decoded.
     """
     with objc.autorelease_pool():
         if isinstance(xmp, (bytes, __NSCFData)):
             xmp = xmp.decode("utf-8")
         xmp = single_quotes_to_double_quotes(xmp)
         xmp = strip_xmp_packet(xmp)
         xmp = xmp.encode("utf-8")
```

### Comparing `cgmetadata-0.1.4/docs/cli.md` & `cgmetadata-0.1.5/docs/cli.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Command Line Interface
 
 The package will install a small command line utility, `cgmd`, which prints
 metadata for an image file in tabular, JSON, CSV, TSV, or XMP formats.
 The CLI can also be used by executing `python3 -m cgmetadata`.
 
 ```
-usage: cgmd [-h] [--version] [--csv] [--tsv] [--json] [--xmp] [--indent INDENT] [--no-header] IMAGE
+usage: cgmd [-h] [--version] [--csv] [--tsv] [--json] [--xmp] [--indent INDENT] [--no-header] IMAGE_OR_VIDEO
 
-Print metadata for image files in various formats.
+Print metadata for image and video files in various formats.
 
 positional arguments:
-  IMAGE                 path to image file
+  IMAGE_OR_VIDEO        path to image or video file
 
 options:
   -h, --help            show this help message and exit
   --version, -v         show program's version number and exit
   --csv, -c             output as comma separated values (CSV); see also --no-header
   --tsv, -t             output as tab separated values (TSV); see also --no-header
   --json, -j            output as JSON; see also --indent
```

### Comparing `cgmetadata-0.1.4/docs/index.md` & `cgmetadata-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/pyproject.toml` & `cgmetadata-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cgmetadata-0.1.4/PKG-INFO` & `cgmetadata-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgmetadata
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use native Core Graphics / ImageIO API on macOS to access and change image metadata
 Author-email: Rhet Turnbull <rturnbull+git@gmail.com>
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pyobjc-core>=9.2
 Requires-Dist: pyobjc-framework-Contacts>=9.2
@@ -107,14 +107,42 @@
 >>> # read metadata from video file
 >>> md = VideoMetadata("test.MOV")
 >>> md.xmp.get("dc:subject")
 ['Coffee', 'Espresso']
 >>> 
 ```
 
+CGMetadata also include a utility function for reading an XMP file and returning a dictionary of metadata using native macOS APIs. This may be useful by itself as it doesn't require the use of external libraries or XML parsers.
+
+<!--
+Setup for doctest:
+
+```pycon
+>>> import shutil
+>>> import os
+>>> try:
+...     os.remove("test.xmp")
+... except Exception:
+...     pass
+...
+>>>  
+>>> cwd = os.getcwd()
+>>> _ = shutil.copy("tests/data/test.MOV.xmp", os.path.join(cwd, "test.xmp"))
+>>> 
+```
+-->
+
+```pycon
+>>> from cgmetadata import metadata_dictionary_from_xmp_packet
+>>> xmp_data = open("test.xmp").read()
+>>> metadata_dictionary_from_xmp_packet(xmp_data)
+{'dc:subject': ['Coffee', 'Espresso'], 'iio:hasXMP': 'True'}
+>>>
+```
+
 ## Installation
 
 ```bash
 pip install cgmetadata
 ```
 
 ## Documentation
```

