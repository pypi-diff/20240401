# Comparing `tmp/tencentcloud-sdk-python-cr-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-cr-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.998.tar", last modified: Fri Oct 13 00:25:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.999.tar", last modified: Mon Oct 16 00:24:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cr-3.0.998.tar` & `tencentcloud-sdk-python-cr-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136120 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)    26131 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/cr_client.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1070 2023-10-13 00:25:10.000000 tencentcloud-sdk-python-cr-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136120 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)    26131 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/cr_client.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:24:23.000000 tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-10-16 00:24:22.000000 tencentcloud-sdk-python-cr-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/models.py` & `tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/cr_client.py` & `tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/cr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.998/tencentcloud/cr/v20180321/errorcodes.py` & `tencentcloud-sdk-python-cr-3.0.999/tencentcloud/cr/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cr-3.0.999/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.998'
+__version__ = '3.0.999'
```

### Comparing `tencentcloud-sdk-python-cr-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.999/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.998/README.rst` & `tencentcloud-sdk-python-cr-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.998/tencentcloud_sdk_python_cr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.999/tencentcloud_sdk_python_cr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.998/setup.py` & `tencentcloud-sdk-python-cr-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cr',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

