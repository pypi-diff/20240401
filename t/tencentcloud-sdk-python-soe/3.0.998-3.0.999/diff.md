# Comparing `tmp/tencentcloud-sdk-python-soe-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-soe-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.998.tar", last modified: Fri Oct 13 00:35:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.999.tar", last modified: Mon Oct 16 00:34:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-soe-3.0.998.tar` & `tencentcloud-sdk-python-soe-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67959 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)     5919 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/soe_client.py
--rw-r--r--   0 root         (0) root         (0)    14811 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:35:05.000000 tencentcloud-sdk-python-soe-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68696 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/soe_client.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:34:15.000000 tencentcloud-sdk-python-soe-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-soe-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-soe-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/models.py` & `tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1363,14 +1363,16 @@
         :type IsQuery: int
         :param _TextMode: 输入文本模式
 0: 普通文本（默认）
 1：[音素结构](https://cloud.tencent.com/document/product/884/33698)文本
         :type TextMode: int
         :param _Keyword: 主题词和关键词
         :type Keyword: str
+        :param _COSBucketURL: 音频存储路径，支持通过子路径指定文件夹名称
+        :type COSBucketURL: str
         """
         self._SeqId = None
         self._IsEnd = None
         self._VoiceFileType = None
         self._VoiceEncodeType = None
         self._UserVoiceData = None
         self._SessionId = None
@@ -1382,14 +1384,15 @@
         self._StorageMode = None
         self._SentenceInfoEnabled = None
         self._ServerType = None
         self._IsAsync = None
         self._IsQuery = None
         self._TextMode = None
         self._Keyword = None
+        self._COSBucketURL = None
 
     @property
     def SeqId(self):
         return self._SeqId
 
     @SeqId.setter
     def SeqId(self, SeqId):
@@ -1473,18 +1476,22 @@
 
     @SoeAppId.setter
     def SoeAppId(self, SoeAppId):
         self._SoeAppId = SoeAppId
 
     @property
     def StorageMode(self):
+        warnings.warn("parameter `StorageMode` is deprecated", DeprecationWarning) 
+
         return self._StorageMode
 
     @StorageMode.setter
     def StorageMode(self, StorageMode):
+        warnings.warn("parameter `StorageMode` is deprecated", DeprecationWarning) 
+
         self._StorageMode = StorageMode
 
     @property
     def SentenceInfoEnabled(self):
         return self._SentenceInfoEnabled
 
     @SentenceInfoEnabled.setter
@@ -1527,14 +1534,22 @@
     def Keyword(self):
         return self._Keyword
 
     @Keyword.setter
     def Keyword(self, Keyword):
         self._Keyword = Keyword
 
+    @property
+    def COSBucketURL(self):
+        return self._COSBucketURL
+
+    @COSBucketURL.setter
+    def COSBucketURL(self, COSBucketURL):
+        self._COSBucketURL = COSBucketURL
+
 
     def _deserialize(self, params):
         self._SeqId = params.get("SeqId")
         self._IsEnd = params.get("IsEnd")
         self._VoiceFileType = params.get("VoiceFileType")
         self._VoiceEncodeType = params.get("VoiceEncodeType")
         self._UserVoiceData = params.get("UserVoiceData")
@@ -1547,14 +1562,15 @@
         self._StorageMode = params.get("StorageMode")
         self._SentenceInfoEnabled = params.get("SentenceInfoEnabled")
         self._ServerType = params.get("ServerType")
         self._IsAsync = params.get("IsAsync")
         self._IsQuery = params.get("IsQuery")
         self._TextMode = params.get("TextMode")
         self._Keyword = params.get("Keyword")
+        self._COSBucketURL = params.get("COSBucketURL")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1650,18 +1666,22 @@
 
     @SessionId.setter
     def SessionId(self, SessionId):
         self._SessionId = SessionId
 
     @property
     def AudioUrl(self):
+        warnings.warn("parameter `AudioUrl` is deprecated", DeprecationWarning) 
+
         return self._AudioUrl
 
     @AudioUrl.setter
     def AudioUrl(self, AudioUrl):
+        warnings.warn("parameter `AudioUrl` is deprecated", DeprecationWarning) 
+
         self._AudioUrl = AudioUrl
 
     @property
     def SentenceInfoSet(self):
         return self._SentenceInfoSet
 
     @SentenceInfoSet.setter
```

### Comparing `tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/soe_client.py` & `tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/soe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.998/tencentcloud/soe/v20180724/errorcodes.py` & `tencentcloud-sdk-python-soe-3.0.999/tencentcloud/soe/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.998/tencentcloud_sdk_python_soe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.999/tencentcloud_sdk_python_soe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.999/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.998/README.rst` & `tencentcloud-sdk-python-soe-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.998/setup.py` & `tencentcloud-sdk-python-soe-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-soe',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Soe SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

