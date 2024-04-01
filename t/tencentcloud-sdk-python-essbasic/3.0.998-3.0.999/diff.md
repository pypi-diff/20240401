# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.998.tar", last modified: Fri Oct 13 00:28:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.999.tar", last modified: Mon Oct 16 00:27:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.998.tar` & `tencentcloud-sdk-python-essbasic-3.0.999.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505009 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)    17658 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    78004 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      733 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1082 2023-10-13 00:28:08.000000 tencentcloud-sdk-python-essbasic-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505344 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    17658 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    78004 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      733 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-10-16 00:27:26.000000 tencentcloud-sdk-python-essbasic-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7147,14 +7147,21 @@
         :type ComponentPosX: float
         :param _ComponentPosY: 参数控件Y位置，单位px
         :type ComponentPosY: float
         :param _ComponentExtra: 扩展参数：
 为JSON格式。
 不同类型的控件会有部分非通用参数
 
+ComponentType为TEXT、MULTI_LINE_TEXT时，支持以下参数：
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+4 FontColor：字符串类型，格式为RGB颜色数字
+参数样例：    "ComponentExtra": "{\"FontColor\":\"255,0,0\",\"FontSize\":12}"
+
 TEXT/MULTI_LINE_TEXT控件可以指定
 1 Font：目前只支持黑体、宋体
 2 FontSize： 范围12-72
 3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
 例如：{"FontSize":12}
 
 ComponentType为FILL_IMAGE时，支持以下参数：
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.999/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.999/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.998/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.999/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-essbasic',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Essbasic SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

