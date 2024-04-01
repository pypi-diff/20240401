# Comparing `tmp/streamlit-keyup-0.2.3.tar.gz` & `tmp/streamlit-keyup-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-keyup-0.2.3.tar", last modified: Wed Feb 14 22:37:57 2024, max compression
+gzip compressed data, was "streamlit-keyup-0.2.4.tar", last modified: Mon Apr  1 14:57:11 2024, max compression
```

## Comparing `streamlit-keyup-0.2.3.tar` & `streamlit-keyup-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:37:57.113726 streamlit-keyup-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-14 22:37:57.113726 streamlit-keyup-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 22:37:57.113726 streamlit-keyup-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:37:57.109727 streamlit-keyup-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:37:57.109727 streamlit-keyup-0.2.3/src/st_keyup/
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/src/st_keyup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:37:57.109727 streamlit-keyup-0.2.3/src/st_keyup/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/src/st_keyup/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/src/st_keyup/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/src/st_keyup/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-02-14 22:37:44.000000 streamlit-keyup-0.2.3/src/st_keyup/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:37:57.113726 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-14 22:37:57.000000 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-14 22:37:57.000000 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 22:37:57.000000 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 22:37:57.000000 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-14 22:37:57.000000 streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:57:11.367757 streamlit-keyup-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/src/st_keyup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/src/st_keyup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/src/st_keyup/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/src/st_keyup/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/src/st_keyup/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/src/st_keyup/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-01 14:57:03.000000 streamlit-keyup-0.2.4/src/st_keyup/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.363757 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 14:57:11.000000 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 14:57:11.000000 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:57:11.000000 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 14:57:11.000000 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 14:57:11.000000 streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/top_level.txt
```

### Comparing `streamlit-keyup-0.2.3/LICENSE` & `streamlit-keyup-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/PKG-INFO` & `streamlit-keyup-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-keyup
-Version: 0.2.3
+Version: 0.2.4
 Summary: Text input that renders on keyup
 Home-page: https://github.com/blackary/streamlit-keyup
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-keyup-0.2.3/README.md` & `streamlit-keyup-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/setup.py` & `streamlit-keyup-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-keyup",
-    version="0.2.3",
+    version="0.2.4",
     author="Zachary Blackwood",
     author_email="zachary@streamlit.io",
     description="Text input that renders on keyup",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blackary/streamlit-keyup",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `streamlit-keyup-0.2.3/src/st_keyup/__init__.py` & `streamlit-keyup-0.2.4/src/st_keyup/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/src/st_keyup/frontend/index.html` & `streamlit-keyup-0.2.4/src/st_keyup/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/src/st_keyup/frontend/main.js` & `streamlit-keyup-0.2.4/src/st_keyup/frontend/main.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -83,15 +83,16 @@
 
         if (debounce_time > 0) { // is false if debounce_time is 0 or undefined
             input.onkeyup = debounce(onKeyUp, debounce_time)
         } else {
             input.onkeyup = onKeyUp
         }
 
+        // Render with the correct height
+        Streamlit.setFrameHeight(73)
+
         window.rendered = true
     }
 }
 
 Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender)
-Streamlit.setComponentReady()
-// Render with the correct height
-Streamlit.setFrameHeight(73)
+Streamlit.setComponentReady()
```

### Comparing `streamlit-keyup-0.2.3/src/st_keyup/frontend/streamlit-component-lib.js` & `streamlit-keyup-0.2.4/src/st_keyup/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/src/st_keyup/frontend/style.css` & `streamlit-keyup-0.2.4/src/st_keyup/frontend/style.css`

 * *Files identical despite different names*

### Comparing `streamlit-keyup-0.2.3/src/streamlit_keyup.egg-info/PKG-INFO` & `streamlit-keyup-0.2.4/src/streamlit_keyup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-keyup
-Version: 0.2.3
+Version: 0.2.4
 Summary: Text input that renders on keyup
 Home-page: https://github.com/blackary/streamlit-keyup
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

