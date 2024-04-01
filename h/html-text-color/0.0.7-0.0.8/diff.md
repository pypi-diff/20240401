# Comparing `tmp/html_text_color-0.0.7.tar.gz` & `tmp/html_text_color-0.0.8.tar.gz`

## Comparing `html_text_color-0.0.7.tar` & `html_text_color-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.7/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/__init__.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/create_colored.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.7/html_text_color/test.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_multiple.html
--rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_multiple.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_single.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_single.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_tokens.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.7/test_outputs/test_tokens.svg
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.7/LICENSE
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.7/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 html_text_color-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 html_text_color-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.8/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/__init__.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/create_colored.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/test.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_multiple.html
+-rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_multiple.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_single.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_single.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_tokens.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_tokens.svg
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.8/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 html_text_color-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 html_text_color-0.0.8/PKG-INFO
```

### Comparing `html_text_color-0.0.7/.github/workflows/publish_to_pypi.yml` & `html_text_color-0.0.8/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/html_text_color/create_colored.py` & `html_text_color-0.0.8/html_text_color/create_colored.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 from matplotlib import colormaps
 import re
 
 replacements = {"▁": " ", "<0x0A>": "<br/>", "Ġ": " ", "\n": "<br>"}
 stupid_color = re.compile(r"^[rgb]{,3}$")
 
 
-def process_color_nums(color_nums, normalize=True, color_order=None):
+def process_color_nums(color_nums, normalize=True, color_order=None, mn=None, mx=None):
     color_nums = np.array(color_nums)
     if color_nums.ndim == 1:
         color_nums = color_nums[:, None]
 
     if color_order is None:
         if color_nums.shape[1] == 1:
             color_order = "viridis"
         else:
             color_order = "rgb"
     assert color_nums.shape[1] <= 3, "color_nums must have 1-3 columns"
 
     if normalize:
-        color_nums = color_nums - color_nums.min(axis=0)
-        color_nums = (color_nums / np.clip(color_nums.max(axis=0), 1e-6, None)) * 255
+        color_nums = color_nums - (color_nums.min(axis=0) if mn is None else mn)
+        color_nums = (
+            color_nums
+            / np.clip(color_nums.max(axis=0) if mx is None else mx, 1e-6, None)
+        ) * 255
 
     color_nums = color_nums.astype(int)
 
     out = np.zeros((color_nums.shape[0], 3), dtype=int)
     if stupid_color.match(color_order):
         for i, d in enumerate("rgb"):
             if d in color_order and color_nums.shape[1] > color_order.index(d):
@@ -38,20 +41,27 @@
             out[i] = np.array(cmap(n)[:3]) * 255
     return out
 
 
 def from_text(tokens, color_nums, normalize=True, color_order=None, beautify=True):
     tokens = tokens.copy()
     if type(tokens[0]) == list:
+        mn = min(min(x) for x in color_nums)
+        mx = max(max(x) for x in color_nums)
         color_nums = [
-            process_color_nums(cn, normalize, color_order) for cn in color_nums
+            process_color_nums(cn, normalize, color_order, mn=mn, mx=mx)
+            for cn in color_nums
         ]
 
     else:
-        color_nums = process_color_nums(color_nums, normalize, color_order)
+        mn = min(color_nums)
+        mx = max(color_nums)
+        color_nums = process_color_nums(
+            color_nums, normalize, color_order, mn=mn, mx=mx
+        )
         color_nums = color_nums[None, ...]
         tokens = [tokens]
 
     if beautify:
         for i, ts in enumerate(tokens):
             for j, _t in enumerate(ts):
                 for old, new in replacements.items():
@@ -80,15 +90,15 @@
 
 
 def from_ids(
     ids,
     tokenizer,
     color_nums,
     normalize=True,
-    color_order="rgb",
+    color_order=None,
     beautify=True,
 ):
     if isinstance(ids[0], list):
         tokens = [tokenizer.convert_ids_to_tokens(i) for i in ids]
     else:
         tokens = tokenizer.convert_ids_to_tokens(ids)
     return from_text(tokens, color_nums, normalize, color_order, beautify)
```

### Comparing `html_text_color-0.0.7/html_text_color/test.py` & `html_text_color-0.0.8/html_text_color/test.py`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/test_outputs/test_multiple.html` & `html_text_color-0.0.8/test_outputs/test_multiple.html`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/test_outputs/test_multiple.svg` & `html_text_color-0.0.8/test_outputs/test_multiple.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/test_outputs/test_single.svg` & `html_text_color-0.0.8/test_outputs/test_single.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/test_outputs/test_tokens.svg` & `html_text_color-0.0.8/test_outputs/test_tokens.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/LICENSE` & `html_text_color-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/README.md` & `html_text_color-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/pyproject.toml` & `html_text_color-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.7/PKG-INFO` & `html_text_color-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: html_text_color
-Version: 0.0.7
+Version: 0.0.8
 Summary: Visualize number vector on text using colored html
 Author-email: Yannik Keller <yannik@kelnet.de>
 License: MIT License
 License-File: LICENSE
 Keywords: HTML,Language Model,color,text,visualization
 Requires-Python: >=3.6
 Requires-Dist: matplotlib
```

