# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.998.tar", last modified: Fri Oct 13 00:38:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.999.tar", last modified: Mon Oct 16 00:37:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.998.tar` & `tencentcloud-sdk-python-tke-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1119118 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)    19924 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   199717 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:38:48.000000 tencentcloud-sdk-python-tke-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1119184 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)    19924 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   199717 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:37:55.000000 tencentcloud-sdk-python-tke-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -34414,15 +34414,15 @@
 class RunAutomationServiceEnabled(AbstractModel):
     """描述了 “云自动化助手” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>TRUE：表示开启云自动化助手服务<br><li>FALSE：表示不开启云自动化助手服务<br><br>默认取值：FALSE。
+        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>true：表示开启云自动化助手服务<br><li>false：表示不开启云自动化助手服务<br><br>默认取值：false。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -34509,15 +34509,16 @@
 class RunMonitorServiceEnabled(AbstractModel):
     """描述了 “云监控” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>TRUE：表示开启云监控服务<br><li>FALSE：表示不开启云监控服务<br><br>默认取值：TRUE。
+        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>true：表示开启云监控服务<br><li>false：表示不开启云监控服务<br><br>默认取值：true。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
```

### Comparing `tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.998/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.999/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.999/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.998/README.rst` & `tencentcloud-sdk-python-tke-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.998/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.999/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.998/setup.py` & `tencentcloud-sdk-python-tke-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

