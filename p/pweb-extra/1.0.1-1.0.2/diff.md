# Comparing `tmp/pweb-extra-1.0.1.tar.gz` & `tmp/pweb-extra-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pweb-extra-1.0.1.tar", last modified: Mon Apr  1 07:25:29 2024, max compression
+gzip compressed data, was "pweb-extra-1.0.2.tar", last modified: Mon Apr  1 13:00:32 2024, max compression
```

## Comparing `pweb-extra-1.0.1.tar` & `pweb-extra-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.813469 pweb-extra-1.0.1/
--rw-rw-rw-   0        0        0    11549 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2039 2024-04-01 07:25:29.811440 pweb-extra-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.761896 pweb-extra-1.0.1/pweb_extra/
--rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/pweb_extra/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.791475 pweb-extra-1.0.1/pweb_extra/barqr/
--rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/pweb_extra/barqr/__init__.py
--rw-rw-rw-   0        0        0     1140 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/pweb_extra/barqr/barcode_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.794435 pweb-extra-1.0.1/pweb_extra/document/
--rw-rw-rw-   0        0        0        0 2024-04-01 06:21:56.000000 pweb-extra-1.0.1/pweb_extra/document/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-04-01 07:23:05.000000 pweb-extra-1.0.1/pweb_extra/document/pweb_pdf.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.807437 pweb-extra-1.0.1/pweb_extra/pws/
--rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.1/pweb_extra/pws/__init__.py
--rw-rw-rw-   0        0        0     3222 2024-03-28 05:12:33.000000 pweb-extra-1.0.1/pweb_extra/pws/pweb_socket.py
--rw-rw-rw-   0        0        0      338 2024-04-01 04:59:16.000000 pweb-extra-1.0.1/pweb_extra/pws/pweb_socket_conf.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:25:29.809441 pweb-extra-1.0.1/pweb_extra.egg-info/
--rw-rw-rw-   0        0        0     2039 2024-04-01 07:25:29.000000 pweb-extra-1.0.1/pweb_extra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-04-01 07:25:29.000000 pweb-extra-1.0.1/pweb_extra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:25:29.000000 pweb-extra-1.0.1/pweb_extra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-23 14:48:18.000000 pweb-extra-1.0.1/pweb_extra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2024-04-01 07:25:29.000000 pweb-extra-1.0.1/pweb_extra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 07:25:29.000000 pweb-extra-1.0.1/pweb_extra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 07:25:29.814438 pweb-extra-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-03-30 00:30:41.000000 pweb-extra-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.916712 pweb-extra-1.0.2/
+-rw-rw-rw-   0        0        0    11549 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2039 2024-04-01 13:00:32.913714 pweb-extra-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.835655 pweb-extra-1.0.2/pweb_extra/
+-rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/pweb_extra/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.890716 pweb-extra-1.0.2/pweb_extra/barqr/
+-rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/pweb_extra/barqr/__init__.py
+-rw-rw-rw-   0        0        0     1140 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/pweb_extra/barqr/barcode_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.893683 pweb-extra-1.0.2/pweb_extra/document/
+-rw-rw-rw-   0        0        0        0 2024-04-01 06:21:56.000000 pweb-extra-1.0.2/pweb_extra/document/__init__.py
+-rw-rw-rw-   0        0        0     1899 2024-04-01 12:58:57.000000 pweb-extra-1.0.2/pweb_extra/document/pweb_pdf.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.910740 pweb-extra-1.0.2/pweb_extra/pws/
+-rw-rw-rw-   0        0        0        0 2024-03-23 14:48:11.000000 pweb-extra-1.0.2/pweb_extra/pws/__init__.py
+-rw-rw-rw-   0        0        0     3222 2024-03-28 05:12:33.000000 pweb-extra-1.0.2/pweb_extra/pws/pweb_socket.py
+-rw-rw-rw-   0        0        0      338 2024-04-01 04:59:16.000000 pweb-extra-1.0.2/pweb_extra/pws/pweb_socket_conf.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:00:32.912711 pweb-extra-1.0.2/pweb_extra.egg-info/
+-rw-rw-rw-   0        0        0     2039 2024-04-01 13:00:32.000000 pweb-extra-1.0.2/pweb_extra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-04-01 13:00:32.000000 pweb-extra-1.0.2/pweb_extra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:00:32.000000 pweb-extra-1.0.2/pweb_extra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-23 14:48:18.000000 pweb-extra-1.0.2/pweb_extra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       87 2024-04-01 13:00:32.000000 pweb-extra-1.0.2/pweb_extra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 13:00:32.000000 pweb-extra-1.0.2/pweb_extra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:00:32.916712 pweb-extra-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-04-01 12:59:41.000000 pweb-extra-1.0.2/setup.py
```

### Comparing `pweb-extra-1.0.1/LICENSE` & `pweb-extra-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pweb-extra-1.0.1/PKG-INFO` & `pweb-extra-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pweb-extra
-Version: 1.0.1
+Version: 1.0.2
 Summary: PWeb Extra help to email, task scheduling and various external operation.
 Home-page: https://github.com/banglafighter/pweb-extra
 Author: Problem Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pweb-extra-1.0.1/README.md` & `pweb-extra-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pweb-extra-1.0.1/pweb_extra/barqr/barcode_generator.py` & `pweb-extra-1.0.2/pweb_extra/barqr/barcode_generator.py`

 * *Files identical despite different names*

### Comparing `pweb-extra-1.0.1/pweb_extra/document/pweb_pdf.py` & `pweb-extra-1.0.2/pweb_extra/document/pweb_pdf.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,39 +10,42 @@
             html_content: str = None,
             html_file_path: str = None,
             pdf_store_path: str = None,
             url: str = None,
             css: str = None,
             css_file_path: str = None,
             css_url: str = None,
+            resource_root_path: str = None,
             encoding=None,
             content_zoom: float = 1,
             font_config=FontConfiguration(),
             embed_css=False,
             media_type='print'):
 
         # Started Main Coding
         if not html_content and not html_file_path and not url:
             raise PPyCException("Content not found")
 
         # Configuring HTML Content
         html_object = HTML(
+            base_url=resource_root_path,
             string=html_content,
             filename=html_file_path,
             url=url,
             media_type=media_type,
             encoding=encoding
         )
 
         # Configuring CSS
         stylesheets = None
         css_font_conf = None
         if css_url or css or css_file_path:
             css_font_conf = font_config
             stylesheets = [CSS(
+                base_url=resource_root_path,
                 string=css,
                 filename=css_file_path,
                 url=css_url,
                 font_config=css_font_conf,
                 media_type=media_type,
                 encoding=encoding
             )]
```

### Comparing `pweb-extra-1.0.1/pweb_extra/pws/pweb_socket.py` & `pweb-extra-1.0.2/pweb_extra/pws/pweb_socket.py`

 * *Files identical despite different names*

### Comparing `pweb-extra-1.0.1/pweb_extra.egg-info/PKG-INFO` & `pweb-extra-1.0.2/pweb_extra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pweb-extra
-Version: 1.0.1
+Version: 1.0.2
 Summary: PWeb Extra help to email, task scheduling and various external operation.
 Home-page: https://github.com/banglafighter/pweb-extra
 Author: Problem Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pweb-extra-1.0.1/setup.py` & `pweb-extra-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return dependency
 
     return dependency + ["ppy-common", "ppy-file-text"]
 
 
 setup(
     name='pweb-extra',
-    version='1.0.1',
+    version='1.0.2',
     url='https://github.com/banglafighter/pweb-extra',
     license='Apache 2.0',
     author='Problem Fighter',
     author_email='banglafighter.com@gmail.com',
     description='PWeb Extra help to email, task scheduling and various external operation.',
     long_description=README,
     long_description_content_type='text/markdown',
```

