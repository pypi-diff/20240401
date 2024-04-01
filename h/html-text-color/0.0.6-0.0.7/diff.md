# Comparing `tmp/html_text_color-0.0.6.tar.gz` & `tmp/html_text_color-0.0.7.tar.gz`

## Comparing `html_text_color-0.0.6.tar` & `html_text_color-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.6/html_text_color/__init__.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 html_text_color-0.0.6/html_text_color/create_colored.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.6/html_text_color/test.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_multiple.html
--rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_multiple.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_single.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_single.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_tokens.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.6/test_outputs/test_tokens.svg
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.6/LICENSE
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.6/README.md
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 html_text_color-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 html_text_color-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/__init__.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/create_colored.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/test.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_multiple.html
+-rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_multiple.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_single.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_single.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_tokens.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_tokens.svg
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.7/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 html_text_color-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 html_text_color-0.0.7/PKG-INFO
```

### Comparing `html_text_color-0.0.6/.github/workflows/publish_to_pypi.yml` & `html_text_color-0.0.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/html_text_color/create_colored.py` & `html_text_color-0.0.7/html_text_color/create_colored.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 from xml.etree import ElementTree as ET
 from xml.etree.ElementTree import ParseError
 import numpy as np
+from matplotlib import colormaps
+import re
 
 replacements = {"▁": " ", "<0x0A>": "<br/>", "Ġ": " ", "\n": "<br>"}
+stupid_color = re.compile(r"^[rgb]{,3}$")
 
 
-def process_color_nums(color_nums, normalize=True, color_order="rgb"):
+def process_color_nums(color_nums, normalize=True, color_order=None):
     color_nums = np.array(color_nums)
     if color_nums.ndim == 1:
         color_nums = color_nums[:, None]
 
+    if color_order is None:
+        if color_nums.shape[1] == 1:
+            color_order = "viridis"
+        else:
+            color_order = "rgb"
     assert color_nums.shape[1] <= 3, "color_nums must have 1-3 columns"
 
     if normalize:
         color_nums = color_nums - color_nums.min(axis=0)
         color_nums = (color_nums / np.clip(color_nums.max(axis=0), 1e-6, None)) * 255
 
     color_nums = color_nums.astype(int)
 
-    tmp = np.zeros((color_nums.shape[0], 3), dtype=int)
-    for i, d in enumerate("rgb"):
-        if d in color_order and color_nums.shape[1] > color_order.index(d):
-            tmp[:, i] = color_nums[:, color_order.index(d)]
-    return tmp
+    out = np.zeros((color_nums.shape[0], 3), dtype=int)
+    if stupid_color.match(color_order):
+        for i, d in enumerate("rgb"):
+            if d in color_order and color_nums.shape[1] > color_order.index(d):
+                out[:, i] = color_nums[:, color_order.index(d)]
+    else:
+        assert color_nums.shape[1] == 1, f"Invalid color_order {color_order}"
+        cmap = colormaps.get_cmap(color_order)
+        for i, n in enumerate(color_nums[:, 0]):
+            out[i] = np.array(cmap(n)[:3]) * 255
+    return out
 
 
-def from_text(tokens, color_nums, normalize=True, color_order="rgb", beautify=True):
+def from_text(tokens, color_nums, normalize=True, color_order=None, beautify=True):
     tokens = tokens.copy()
     if type(tokens[0]) == list:
         color_nums = [
             process_color_nums(cn, normalize, color_order) for cn in color_nums
         ]
 
     else:
@@ -45,14 +59,16 @@
 
     html = ET.Element("html")
     body = ET.Element("body")
     html.append(body)
     for tok_paragraph, col_paragraph in zip(tokens, color_nums):
         p = ET.Element("p")
         body.append(p)
+        hr = ET.Element("hr")
+        body.append(hr)
         for tok, col in zip(tok_paragraph, col_paragraph):
             try:
                 span = ET.fromstring(f"<span>{tok}</span>")
             except ParseError:
                 span = ET.Element("span")
                 span.text = tok
             span.attrib["style"] = (
```

### Comparing `html_text_color-0.0.6/html_text_color/test.py` & `html_text_color-0.0.7/html_text_color/test.py`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/test_outputs/test_multiple.html` & `html_text_color-0.0.7/test_outputs/test_multiple.html`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/test_outputs/test_multiple.svg` & `html_text_color-0.0.7/test_outputs/test_multiple.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/test_outputs/test_single.svg` & `html_text_color-0.0.7/test_outputs/test_single.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/test_outputs/test_tokens.svg` & `html_text_color-0.0.7/test_outputs/test_tokens.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/LICENSE` & `html_text_color-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/README.md` & `html_text_color-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.6/PKG-INFO` & `html_text_color-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: html_text_color
-Version: 0.0.6
+Version: 0.0.7
 Summary: Visualize number vector on text using colored html
 Author-email: Yannik Keller <yannik@kelnet.de>
 License: MIT License
 License-File: LICENSE
 Keywords: HTML,Language Model,color,text,visualization
 Requires-Python: >=3.6
+Requires-Dist: matplotlib
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # Visualize number vector on text using colored html
 ## Installation
 `pip install html-text-color`
```

