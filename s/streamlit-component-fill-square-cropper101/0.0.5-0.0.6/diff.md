# Comparing `tmp/streamlit_component_fill_square_cropper101-0.0.5.tar.gz` & `tmp/streamlit_component_fill_square_cropper101-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_component_fill_square_cropper101-0.0.5.tar", last modified: Sun Mar 31 17:50:34 2024, max compression
+gzip compressed data, was "streamlit_component_fill_square_cropper101-0.0.6.tar", last modified: Mon Apr  1 14:25:38 2024, max compression
```

## Comparing `streamlit_component_fill_square_cropper101-0.0.5.tar` & `streamlit_component_fill_square_cropper101-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 17:50:34.136972 streamlit_component_fill_square_cropper101-0.0.5/
--rw-rw-rw-   0        0        0       79 2024-03-31 14:07:08.000000 streamlit_component_fill_square_cropper101-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1010 2024-03-31 17:50:34.134125 streamlit_component_fill_square_cropper101-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      533 2024-03-30 19:17:45.000000 streamlit_component_fill_square_cropper101-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 17:50:34.137604 streamlit_component_fill_square_cropper101-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1111 2024-03-31 17:38:45.000000 streamlit_component_fill_square_cropper101-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 17:50:34.075642 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101/
--rw-rw-rw-   0        0        0      745 2024-03-31 16:43:26.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101/__init__ - Copy.py
--rw-rw-rw-   0        0        0     2304 2024-03-31 17:44:06.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101/__init__.py
--rw-rw-rw-   0        0        0     1442 2024-03-28 17:18:21.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101/fill_square_cropper.py
-drwxrwxrwx   0        0        0        0 2024-03-31 17:50:34.130456 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-03-31 17:50:33.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-03-31 17:50:34.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 17:50:33.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-31 17:50:33.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2024-03-31 17:50:33.000000 streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:25:38.530356 streamlit_component_fill_square_cropper101-0.0.6/
+-rw-rw-rw-   0        0        0       79 2024-03-31 14:07:08.000000 streamlit_component_fill_square_cropper101-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1325 2024-04-01 14:25:38.528773 streamlit_component_fill_square_cropper101-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2024-04-01 14:17:56.000000 streamlit_component_fill_square_cropper101-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:25:38.532027 streamlit_component_fill_square_cropper101-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2024-04-01 14:24:37.000000 streamlit_component_fill_square_cropper101-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:25:38.495090 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101/
+-rw-rw-rw-   0        0        0     2324 2024-03-31 20:46:47.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:25:38.526675 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-04-01 14:25:38.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-04-01 14:25:38.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:25:38.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-01 14:25:38.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2024-04-01 14:25:38.000000 streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/top_level.txt
```

### Comparing `streamlit_component_fill_square_cropper101-0.0.5/PKG-INFO` & `streamlit_component_fill_square_cropper101-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 Metadata-Version: 2.1
 Name: streamlit_component_fill_square_cropper101
-Version: 0.0.5
+Version: 0.0.6
 Summary: streamlit_component_fill_square_cropper, adds a filler when needed of the avg color pixel.
 Home-page: https://github.com/webdevserv/streamlit_component_fill_square_cropper101
 Author: Idoia Lertxundi
 Author-email: idoiagoikoa@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
 Requires-Dist: numpy
 Requires-Dist: streamlit
 
-# Streamlit - Component Square Fill Cropper Component
+# Streamlit Component Fill Square Cropper101  
+Streamlit Component Squares image with the adequate color filler  
+![Alt Text](https://github.com/webdevserv/streamlit_component_fill_square_cropper101/blob/f6772817321ed43baa7f238f53f6b3613700597a/images/add.JPG)  
 
-Streamlit Component Squares image with the adecuate color filler
-
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://webdevserv-portfolio-idoia-icodeidoia-portfolio-9kblei.streamlit.app/a_LIVE_Square_Filler_app)
+Demo: [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://webdevserv-portfolio-idoia-icodeidoia-portfolio-9kblei.streamlit.app/a_LIVE_Square_Filler_app)  
 
 # installation
 
-pip install streamlit-component-square-fill-cropper1-webdevserv
+pip install streamlit-component-fill-square-cropper101
+
+# running locally
+
+streamlit run app.py  
+or  
+streamlit run app.py --server.enableXsrfProtection false  
 
+#temporarily disable XSRF protection, which might be causing the 403.  
 
 # use
 
-import streamlit as st
-from streamlit_component_square_fill_cropper1_webdevserv import square_fill_cropper as scropper
+import streamlit as st  
+
+
+from streamlit_component_fill_square_cropper101 import square_fill_cropper
```

### Comparing `streamlit_component_fill_square_cropper101-0.0.5/setup.py` & `streamlit_component_fill_square_cropper101-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     :return: content of README.md
     """
     return open(join(dirname(__file__), "README.md")).read()
 
 
 setuptools.setup(
     name="streamlit_component_fill_square_cropper101",
-    version="0.0.5",
+    version="0.0.6",
     author="Idoia Lertxundi",
     author_email='idoiagoikoa@gmail.com',
     description="streamlit_component_fill_square_cropper, adds a filler when needed of the avg color pixel.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/webdevserv/streamlit_component_fill_square_cropper101",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101/__init__.py` & `streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 import requests
 from io import BytesIO
 
 _RELEASE = True
 
 if not _RELEASE:
     _component_func = components.declare_component(
-        "streamlit_component_square_filler_cropper101",
+        "streamlit_component_fill_square_cropper101",
         url="http://localhost:8501",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
-    _component_func = components.declare_component("streamlit_component_square_filler_cropper101", path=build_dir)
+    _component_func  = components.declare_component("streamlit_component_fill_square_cropper101", path=build_dir)
 
 if not _RELEASE:
-    _component_func = components.declare_component(
-        "st_img_label",
+    component = components.declare_component(
+        "streamlit_component_fill_square_cropper101",
         url="http://localhost:8501",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
-    _component_func = components.declare_component("streamlit_component_square_filler_cropper101", path=build_dir)
+    _component_func  = components.declare_component("streamlit_component_fill_square_cropper101", path=build_dir)
 
 
 def fill_square_cropper(img: Image.Image):
     imgsz = [img.height, img.width]
 
     original_size = imgsz
```

### Comparing `streamlit_component_fill_square_cropper101-0.0.5/streamlit_component_fill_square_cropper101.egg-info/PKG-INFO` & `streamlit_component_fill_square_cropper101-0.0.6/streamlit_component_fill_square_cropper101.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 Metadata-Version: 2.1
 Name: streamlit_component_fill_square_cropper101
-Version: 0.0.5
+Version: 0.0.6
 Summary: streamlit_component_fill_square_cropper, adds a filler when needed of the avg color pixel.
 Home-page: https://github.com/webdevserv/streamlit_component_fill_square_cropper101
 Author: Idoia Lertxundi
 Author-email: idoiagoikoa@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
 Requires-Dist: numpy
 Requires-Dist: streamlit
 
-# Streamlit - Component Square Fill Cropper Component
+# Streamlit Component Fill Square Cropper101  
+Streamlit Component Squares image with the adequate color filler  
+![Alt Text](https://github.com/webdevserv/streamlit_component_fill_square_cropper101/blob/f6772817321ed43baa7f238f53f6b3613700597a/images/add.JPG)  
 
-Streamlit Component Squares image with the adecuate color filler
-
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://webdevserv-portfolio-idoia-icodeidoia-portfolio-9kblei.streamlit.app/a_LIVE_Square_Filler_app)
+Demo: [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://webdevserv-portfolio-idoia-icodeidoia-portfolio-9kblei.streamlit.app/a_LIVE_Square_Filler_app)  
 
 # installation
 
-pip install streamlit-component-square-fill-cropper1-webdevserv
+pip install streamlit-component-fill-square-cropper101
+
+# running locally
+
+streamlit run app.py  
+or  
+streamlit run app.py --server.enableXsrfProtection false  
 
+#temporarily disable XSRF protection, which might be causing the 403.  
 
 # use
 
-import streamlit as st
-from streamlit_component_square_fill_cropper1_webdevserv import square_fill_cropper as scropper
+import streamlit as st  
+
+
+from streamlit_component_fill_square_cropper101 import square_fill_cropper
```

