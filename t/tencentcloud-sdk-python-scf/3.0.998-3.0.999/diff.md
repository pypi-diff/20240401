# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.998.tar", last modified: Fri Oct 13 00:34:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.999.tar", last modified: Mon Oct 16 00:33:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.998.tar` & `tencentcloud-sdk-python-scf-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    44580 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   322466 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    32699 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:34:29.000000 tencentcloud-sdk-python-scf-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    44580 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   322505 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    32699 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:33:46.000000 tencentcloud-sdk-python-scf-3.0.999/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:33:45.000000 tencentcloud-sdk-python-scf-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-scf-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1516,15 +1516,15 @@
 
     def __init__(self):
         r"""
         :param _FunctionName: 新建触发器绑定的函数名称
         :type FunctionName: str
         :param _TriggerName: 新建触发器名称。如果是定时触发器，名称支持英文字母、数字、连接符和下划线，最长100个字符；如果是cos触发器，需要是对应cos存储桶适用于XML API的访问域名(例如:5401-5ff414-12345.cos.ap-shanghai.myqcloud.com);如果是其他触发器，见具体触发器绑定参数的说明
         :type TriggerName: str
-        :param _Type: 触发器类型，目前支持 cos 、cmq、 timer、 ckafka、apigw类型。创建 cls 触发器请参考[CLS 创建投递 SCF 任务](https://cloud.tencent.com/document/product/614/61096)。
+        :param _Type: 触发器类型，目前支持 cos 、cmq、 timer、 ckafka、apigw类型。创建函数URL请在此填写 http 。创建 cls 触发器请参考[CLS 创建投递 SCF 任务](https://cloud.tencent.com/document/product/614/61096)。
         :type Type: str
         :param _TriggerDesc: 触发器对应的参数，可见具体[触发器描述说明](https://cloud.tencent.com/document/product/583/39901)
         :type TriggerDesc: str
         :param _Namespace: 函数的命名空间
         :type Namespace: str
         :param _Qualifier: 函数的版本，默认为 $LATEST，建议填写 [$DEFAULT](https://cloud.tencent.com/document/product/583/36149#.E9.BB.98.E8.AE.A4.E5.88.AB.E5.90.8D)方便后续进行版本的灰度发布。
         :type Qualifier: str
```

### Comparing `tencentcloud-sdk-python-scf-3.0.998/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.999/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.999/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.998/README.rst` & `tencentcloud-sdk-python-scf-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.998/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.999/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.998/setup.py` & `tencentcloud-sdk-python-scf-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-scf',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Scf SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

