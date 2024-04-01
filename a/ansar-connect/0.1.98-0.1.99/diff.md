# Comparing `tmp/ansar-connect-0.1.98.tar.gz` & `tmp/ansar-connect-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.98.tar", last modified: Wed Mar 20 23:18:37 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.99.tar", last modified: Wed Mar 20 23:50:38 2024, max compression
```

## Comparing `ansar-connect-0.1.98.tar` & `ansar-connect-0.1.99.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.810039 ansar-connect-0.1.98/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.98/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2673 2024-03-20 23:18:37.810039 ansar-connect-0.1.98/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.98/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-08 02:51:46.000000 ansar-connect-0.1.98/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-03-20 23:18:37.810039 ansar-connect-0.1.98/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2262 2024-03-08 02:51:56.000000 ansar-connect-0.1.98/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.806039 ansar-connect-0.1.98/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.806039 ansar-connect-0.1.98/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.806039 ansar-connect-0.1.98/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12318 2024-03-17 14:02:14.000000 ansar-connect-0.1.98/src/ansar/command/ansar_cloud.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14130 2024-03-18 06:24:39.000000 ansar-connect-0.1.98/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12527 2024-03-18 00:43:30.000000 ansar-connect-0.1.98/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.98/src/ansar/command/fixed_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8682 2024-03-18 00:43:30.000000 ansar-connect-0.1.98/src/ansar/command/product_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.810039 ansar-connect-0.1.98/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2974 2024-03-20 23:18:19.000000 ansar-connect-0.1.98/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13223 2024-03-17 14:04:50.000000 ansar-connect-0.1.98/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    74889 2024-03-20 23:17:52.000000 ansar-connect-0.1.98/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5943 2024-03-18 00:43:30.000000 ansar-connect-0.1.98/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8143 2024-03-18 20:45:59.000000 ansar-connect-0.1.98/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.98/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21086 2024-03-08 13:33:32.000000 ansar-connect-0.1.98/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.98/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    35011 2024-03-17 14:05:23.000000 ansar-connect-0.1.98/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.98/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    18159 2024-03-18 22:03:04.000000 ansar-connect-0.1.98/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2122 2024-03-05 18:55:10.000000 ansar-connect-0.1.98/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    35756 2024-02-09 05:51:14.000000 ansar-connect-0.1.98/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1864 2024-03-07 06:20:08.000000 ansar-connect-0.1.98/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.98/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5599 2024-03-18 02:37:23.000000 ansar-connect-0.1.98/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:18:37.810039 ansar-connect-0.1.98/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2673 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      960 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      251 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-03-20 23:18:37.000000 ansar-connect-0.1.98/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.99/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2673 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.99/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-08 02:51:46.000000 ansar-connect-0.1.99/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2262 2024-03-08 02:51:56.000000 ansar-connect-0.1.99/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.099109 ansar-connect-0.1.99/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.099109 ansar-connect-0.1.99/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12318 2024-03-17 14:02:14.000000 ansar-connect-0.1.99/src/ansar/command/ansar_cloud.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14130 2024-03-18 06:24:39.000000 ansar-connect-0.1.99/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12527 2024-03-18 00:43:30.000000 ansar-connect-0.1.99/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.99/src/ansar/command/fixed_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8682 2024-03-18 00:43:30.000000 ansar-connect-0.1.99/src/ansar/command/product_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2974 2024-03-20 23:50:34.000000 ansar-connect-0.1.99/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13223 2024-03-17 14:04:50.000000 ansar-connect-0.1.99/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    74547 2024-03-20 23:49:44.000000 ansar-connect-0.1.99/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5943 2024-03-18 00:43:30.000000 ansar-connect-0.1.99/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8143 2024-03-18 20:45:59.000000 ansar-connect-0.1.99/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.99/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21086 2024-03-08 13:33:32.000000 ansar-connect-0.1.99/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.99/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    35011 2024-03-17 14:05:23.000000 ansar-connect-0.1.99/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.99/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    18159 2024-03-18 22:03:04.000000 ansar-connect-0.1.99/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2122 2024-03-05 18:55:10.000000 ansar-connect-0.1.99/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    35756 2024-02-09 05:51:14.000000 ansar-connect-0.1.99/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1864 2024-03-07 06:20:08.000000 ansar-connect-0.1.99/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.99/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5599 2024-03-18 02:37:23.000000 ansar-connect-0.1.99/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-20 23:50:38.103109 ansar-connect-0.1.99/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2673 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      960 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      251 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-03-20 23:50:38.000000 ansar-connect-0.1.99/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.98/LICENSE` & `ansar-connect-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/PKG-INFO` & `ansar-connect-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.98
+Version: 0.1.99
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.98/README.md` & `ansar-connect-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/pyproject.toml` & `ansar-connect-0.1.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/setup.py` & `ansar-connect-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/command/ansar_cloud.py` & `ansar-connect-0.1.99/src/ansar/command/ansar_cloud.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.99/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.99/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/command/fixed_directory.py` & `ansar-connect-0.1.99/src/ansar/command/fixed_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/command/product_directory.py` & `ansar-connect-0.1.99/src/ansar/command/product_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/__init__.py` & `ansar-connect-0.1.99/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 31a4ad19770eee935c41df422eecec2b265b5a9e
-Version: 0.1.97 (2024-03-21@12:18:19+NZDT)
+Commit: 73185415c2c3f1687d6c1a6e2711fb98a0ec636e
+Version: 0.1.98 (2024-03-21@12:50:34+NZDT)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.98/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.99/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/directory.py` & `ansar-connect-0.1.99/src/ansar/connect/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1183,32 +1183,25 @@
 		return CLEARING
 	self.close_route()
 
 	self.forward(Dropped(), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 def PublisherLoop_CLEARING_Completed(self, message):
-	self.trace(f'[1] {self.created_session}, {self.return_address}, {self.created_session}')
-	self.trace(f'[2] {self.value}, {self.publisher_address}, {self.origin_address}')
-	self.trace(f'[3] {self.publisher_address}, {self.origin_address}')
-
 	if self.created_session is None or self.return_address != self.created_session:
-		self.trace(f'[4]')
 		return CLEARING
-	self.trace(f'[5]')
+
 	self.create_session = None
 	self.close_route()
 
 	if self.closing:
-		self.trace(f'[6]')
 		self.forward(Cleared(self.value), self.publisher_address, self.origin_address)
 	else:
-		self.trace(f'[7]')
 		self.forward(Dropped(), self.publisher_address, self.origin_address)
-	self.trace(f'[8]')
+
 	self.complete(ar.Aborted())
 
 PUBLISHER_LOOP_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	LOOPED: (
```

### Comparing `ansar-connect-0.1.98/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.99/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.99/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/grouping.py` & `ansar-connect-0.1.99/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/networking.py` & `ansar-connect-0.1.99/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.99/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/node.py` & `ansar-connect-0.1.99/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.99/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/procedure.py` & `ansar-connect-0.1.99/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/product.py` & `ansar-connect-0.1.99/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/socketry.py` & `ansar-connect-0.1.99/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/standard.py` & `ansar-connect-0.1.99/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/transporting.py` & `ansar-connect-0.1.99/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar/connect/wan.py` & `ansar-connect-0.1.99/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.98/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.99/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.98
+Version: 0.1.99
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.98/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.99/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

