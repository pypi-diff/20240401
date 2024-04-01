# Comparing `tmp/vcx_py-1.1.1.tar.gz` & `tmp/vcx_py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcx_py-1.1.1.tar", last modified: Thu Mar 28 19:43:05 2024, max compression
+gzip compressed data, was "vcx_py-1.1.2.tar", last modified: Mon Apr  1 13:21:21 2024, max compression
```

## Comparing `vcx_py-1.1.1.tar` & `vcx_py-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-03-28 19:43:05.498797 vcx_py-1.1.1/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.1.1/LICENSE
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-03-28 19:43:05.498797 vcx_py-1.1.1/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3936 2024-03-22 20:52:38.000000 vcx_py-1.1.1/README.md
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-03-28 19:43:05.498797 vcx_py-1.1.1/setup.cfg
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-03-28 19:42:56.000000 vcx_py-1.1.1/setup.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-03-28 19:43:05.498797 vcx_py-1.1.1/vcx_py/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      792 2024-03-18 23:09:16.000000 vcx_py-1.1.1/vcx_py/__init__.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     9862 2024-03-28 19:41:48.000000 vcx_py-1.1.1/vcx_py/client.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2365 2024-03-21 19:20:57.000000 vcx_py-1.1.1/vcx_py/constants.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.1.1/vcx_py/schema.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3065 2024-03-28 19:39:06.000000 vcx_py-1.1.1/vcx_py/utils.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-03-28 19:43:05.498797 vcx_py-1.1.1/vcx_py.egg-info/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-03-28 19:43:05.000000 vcx_py-1.1.1/vcx_py.egg-info/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-03-28 19:43:05.000000 vcx_py-1.1.1/vcx_py.egg-info/SOURCES.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-03-28 19:43:05.000000 vcx_py-1.1.1/vcx_py.egg-info/dependency_links.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-03-28 19:43:05.000000 vcx_py-1.1.1/vcx_py.egg-info/top_level.txt
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:21:21.050702 vcx_py-1.1.2/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.1.2/LICENSE
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-04-01 13:21:21.050702 vcx_py-1.1.2/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3936 2024-03-22 20:52:38.000000 vcx_py-1.1.2/README.md
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-04-01 13:21:21.050702 vcx_py-1.1.2/setup.cfg
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-04-01 13:20:59.000000 vcx_py-1.1.2/setup.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:21:21.030701 vcx_py-1.1.2/vcx_py/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      792 2024-03-18 23:09:16.000000 vcx_py-1.1.2/vcx_py/__init__.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)    10437 2024-04-01 13:20:10.000000 vcx_py-1.1.2/vcx_py/client.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2365 2024-03-21 19:20:57.000000 vcx_py-1.1.2/vcx_py/constants.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.1.2/vcx_py/schema.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3065 2024-03-28 19:39:06.000000 vcx_py-1.1.2/vcx_py/utils.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:21:21.050702 vcx_py-1.1.2/vcx_py.egg-info/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-04-01 13:21:20.000000 vcx_py-1.1.2/vcx_py.egg-info/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-04-01 13:21:20.000000 vcx_py-1.1.2/vcx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-04-01 13:21:20.000000 vcx_py-1.1.2/vcx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-04-01 13:21:20.000000 vcx_py-1.1.2/vcx_py.egg-info/top_level.txt
```

### Comparing `vcx_py-1.1.1/LICENSE` & `vcx_py-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/PKG-INFO` & `vcx_py-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcx_py
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple python client for the VirgoCX API
 Home-page: https://www.github.com/aarjaneiro/vcx_py
 Author: Aaron Janeiro Stone
 Author-email: aaron@thequant.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vcx_py-1.1.1/README.md` & `vcx_py-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/setup.py` & `vcx_py-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from setuptools import setup
 
 setup(
     name='vcx_py',
-    version='1.1.1',
+    version='1.1.2',
     packages=['vcx_py'],
     license='MIT',
     author='Aaron Janeiro Stone',
     author_email='aaron@thequant.ca',
     description='A simple python client for the VirgoCX API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `vcx_py-1.1.1/vcx_py/__init__.py` & `vcx_py-1.1.2/vcx_py/__init__.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/vcx_py/client.py` & `vcx_py-1.1.2/vcx_py/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,17 @@
         non-limit buy orders (otherwise `qty` is required).
         """
         if isinstance(category, OrderType):
             category = category.value
         if isinstance(direction, OrderDirection):
             direction = direction.value
 
+        if qty is None and total is None:
+            raise ValueError("Either quantity or total is required")
+
         # Handle conversions
         if category == OrderType.LIMIT:
             if price is None:
                 raise ValueError("Price is required for limit orders")
             if qty is None:
                 if not handle_conversions:
                     raise ValueError("Quantity is required for limit orders")
@@ -150,14 +153,23 @@
                     raise ValueError("Total is required for non-limit buy orders")
                 else:
                     market_price = kwargs.get("market_price", None)
                     if market_price is None:
                         market_price = self.__extract_market_price__(direction, symbol)
                     total = qty * market_price
                     qty = None
+            elif qty is None:
+                if not handle_conversions:
+                    raise ValueError("Quantity is required for non-limit sell orders")
+                else:
+                    market_price = kwargs.get("market_price", None)
+                    if market_price is None:
+                        market_price = self.__extract_market_price__(direction, symbol)
+                    qty = total / market_price
+                    total = None
 
         payload = {"apiKey": self._api_key(), "symbol": symbol, "category": category, "type": direction,
                    "country": 1}
 
         with VirgoCXClient.STATIC_LOCK:
             if symbol in VirgoCXClient.FMT_DATA:
                 fmt_data = VirgoCXClient.FMT_DATA[symbol]
```

### Comparing `vcx_py-1.1.1/vcx_py/constants.py` & `vcx_py-1.1.2/vcx_py/constants.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/vcx_py/schema.py` & `vcx_py-1.1.2/vcx_py/schema.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/vcx_py/utils.py` & `vcx_py-1.1.2/vcx_py/utils.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.1/vcx_py.egg-info/PKG-INFO` & `vcx_py-1.1.2/vcx_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcx_py
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple python client for the VirgoCX API
 Home-page: https://www.github.com/aarjaneiro/vcx_py
 Author: Aaron Janeiro Stone
 Author-email: aaron@thequant.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

