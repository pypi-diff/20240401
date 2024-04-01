# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.998.tar", last modified: Fri Oct 13 00:30:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.999.tar", last modified: Mon Oct 16 00:29:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)   368411 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)    20522 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    84131 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      583 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1088 2023-10-13 00:30:24.000000 tencentcloud-sdk-python-iotexplorer-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   373823 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)    20522 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    85058 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      583 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-10-16 00:29:29.000000 tencentcloud-sdk-python-iotexplorer-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7965,14 +7965,180 @@
             for item in params.get("Positions"):
                 obj = PositionItem()
                 obj._deserialize(item)
                 self._Positions.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class GetDeviceSumStatisticsRequest(AbstractModel):
+    """GetDeviceSumStatistics请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProductIds: 产品id列表，长度为0则拉取项目内全部产品
+        :type ProductIds: list of str
+        """
+        self._ProjectId = None
+        self._ProductIds = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProductIds(self):
+        return self._ProductIds
+
+    @ProductIds.setter
+    def ProductIds(self, ProductIds):
+        self._ProductIds = ProductIds
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._ProductIds = params.get("ProductIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GetDeviceSumStatisticsResponse(AbstractModel):
+    """GetDeviceSumStatistics返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ActivationCount: 激活设备总数
+        :type ActivationCount: int
+        :param _OnlineCount: 在线设备总数
+        :type OnlineCount: int
+        :param _ActivationBeforeDay: 前一天激活设备数
+        :type ActivationBeforeDay: int
+        :param _ActiveBeforeDay: 前一天活跃设备数
+        :type ActiveBeforeDay: int
+        :param _ActivationWeekDayCount: 前一周激活设备数
+        :type ActivationWeekDayCount: int
+        :param _ActiveWeekDayCount: 前一周活跃设备数
+        :type ActiveWeekDayCount: int
+        :param _ActivationBeforeWeekDayCount: 上一周激活设备数
+        :type ActivationBeforeWeekDayCount: int
+        :param _ActiveBeforeWeekDayCount: 上一周活跃设备数
+        :type ActiveBeforeWeekDayCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ActivationCount = None
+        self._OnlineCount = None
+        self._ActivationBeforeDay = None
+        self._ActiveBeforeDay = None
+        self._ActivationWeekDayCount = None
+        self._ActiveWeekDayCount = None
+        self._ActivationBeforeWeekDayCount = None
+        self._ActiveBeforeWeekDayCount = None
+        self._RequestId = None
+
+    @property
+    def ActivationCount(self):
+        return self._ActivationCount
+
+    @ActivationCount.setter
+    def ActivationCount(self, ActivationCount):
+        self._ActivationCount = ActivationCount
+
+    @property
+    def OnlineCount(self):
+        return self._OnlineCount
+
+    @OnlineCount.setter
+    def OnlineCount(self, OnlineCount):
+        self._OnlineCount = OnlineCount
+
+    @property
+    def ActivationBeforeDay(self):
+        return self._ActivationBeforeDay
+
+    @ActivationBeforeDay.setter
+    def ActivationBeforeDay(self, ActivationBeforeDay):
+        self._ActivationBeforeDay = ActivationBeforeDay
+
+    @property
+    def ActiveBeforeDay(self):
+        return self._ActiveBeforeDay
+
+    @ActiveBeforeDay.setter
+    def ActiveBeforeDay(self, ActiveBeforeDay):
+        self._ActiveBeforeDay = ActiveBeforeDay
+
+    @property
+    def ActivationWeekDayCount(self):
+        return self._ActivationWeekDayCount
+
+    @ActivationWeekDayCount.setter
+    def ActivationWeekDayCount(self, ActivationWeekDayCount):
+        self._ActivationWeekDayCount = ActivationWeekDayCount
+
+    @property
+    def ActiveWeekDayCount(self):
+        return self._ActiveWeekDayCount
+
+    @ActiveWeekDayCount.setter
+    def ActiveWeekDayCount(self, ActiveWeekDayCount):
+        self._ActiveWeekDayCount = ActiveWeekDayCount
+
+    @property
+    def ActivationBeforeWeekDayCount(self):
+        return self._ActivationBeforeWeekDayCount
+
+    @ActivationBeforeWeekDayCount.setter
+    def ActivationBeforeWeekDayCount(self, ActivationBeforeWeekDayCount):
+        self._ActivationBeforeWeekDayCount = ActivationBeforeWeekDayCount
+
+    @property
+    def ActiveBeforeWeekDayCount(self):
+        return self._ActiveBeforeWeekDayCount
+
+    @ActiveBeforeWeekDayCount.setter
+    def ActiveBeforeWeekDayCount(self, ActiveBeforeWeekDayCount):
+        self._ActiveBeforeWeekDayCount = ActiveBeforeWeekDayCount
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._ActivationCount = params.get("ActivationCount")
+        self._OnlineCount = params.get("OnlineCount")
+        self._ActivationBeforeDay = params.get("ActivationBeforeDay")
+        self._ActiveBeforeDay = params.get("ActiveBeforeDay")
+        self._ActivationWeekDayCount = params.get("ActivationWeekDayCount")
+        self._ActiveWeekDayCount = params.get("ActiveWeekDayCount")
+        self._ActivationBeforeWeekDayCount = params.get("ActivationBeforeWeekDayCount")
+        self._ActiveBeforeWeekDayCount = params.get("ActiveBeforeWeekDayCount")
+        self._RequestId = params.get("RequestId")
+
+
 class GetFamilyDeviceUserListRequest(AbstractModel):
     """GetFamilyDeviceUserList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1356,14 +1356,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def GetDeviceSumStatistics(self, request):
+        """拉取设备统计汇总数据
+
+        :param request: Request instance for GetDeviceSumStatistics.
+        :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceSumStatisticsRequest`
+        :rtype: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceSumStatisticsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GetDeviceSumStatistics", params, headers=headers)
+            response = json.loads(body)
+            model = models.GetDeviceSumStatisticsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def GetFamilyDeviceUserList(self, request):
         """用于获取设备绑定的用户列表
 
         :param request: Request instance for GetFamilyDeviceUserList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetFamilyDeviceUserListRequest`
         :rtype: :class:`tencentcloud.iotexplorer.v20190423.models.GetFamilyDeviceUserListResponse`
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.999/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.999/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.998/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.999/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-iotexplorer',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Iotexplorer SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

