# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.998.tar", last modified: Fri Oct 13 00:27:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.999.tar", last modified: Mon Oct 16 00:27:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.998.tar` & `tencentcloud-sdk-python-emr-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    31934 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   467608 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)    14648 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:27:51.000000 tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:27:50.000000 tencentcloud-sdk-python-emr-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    32872 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   477110 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)    14890 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:27:07.000000 tencentcloud-sdk-python-emr-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/emr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeAutoScaleRecords(self, request):
+        """获取集群的自动扩缩容的详细记录
+
+        :param request: Request instance for DescribeAutoScaleRecords.
+        :type request: :class:`tencentcloud.emr.v20190103.models.DescribeAutoScaleRecordsRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeAutoScaleRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAutoScaleRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAutoScaleRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeClusterNodes(self, request):
         """查询集群节点信息
 
         :param request: Request instance for DescribeClusterNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeClusterNodesRequest`
         :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeClusterNodesResponse`
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,169 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AutoScaleRecord(AbstractModel):
+    """弹性扩缩容记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _StrategyName: 扩缩容规则名。
+        :type StrategyName: str
+        :param _ScaleAction: "SCALE_OUT"和"SCALE_IN"，分别表示扩容和缩容。
+        :type ScaleAction: str
+        :param _ActionStatus: 取值为"SUCCESS","FAILED","PART_SUCCESS","IN_PROCESS"，分别表示成功、失败、部分成功和流程中。
+        :type ActionStatus: str
+        :param _ActionTime: 流程触发时间。
+        :type ActionTime: str
+        :param _ScaleInfo: 扩缩容相关描述信息。
+        :type ScaleInfo: str
+        :param _ExpectScaleNum: 只在ScaleAction为SCALE_OUT时有效。
+        :type ExpectScaleNum: int
+        :param _EndTime: 流程结束时间。
+        :type EndTime: str
+        :param _StrategyType: 策略类型，按负载或者按时间，1表示负载伸缩，2表示时间伸缩
+        :type StrategyType: int
+        :param _SpecInfo: 扩容时所使用规格信息。
+        :type SpecInfo: str
+        :param _CompensateFlag: 补偿扩容，0表示不开启，1表示开启
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CompensateFlag: int
+        :param _CompensateCount: 补偿次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CompensateCount: int
+        """
+        self._StrategyName = None
+        self._ScaleAction = None
+        self._ActionStatus = None
+        self._ActionTime = None
+        self._ScaleInfo = None
+        self._ExpectScaleNum = None
+        self._EndTime = None
+        self._StrategyType = None
+        self._SpecInfo = None
+        self._CompensateFlag = None
+        self._CompensateCount = None
+
+    @property
+    def StrategyName(self):
+        return self._StrategyName
+
+    @StrategyName.setter
+    def StrategyName(self, StrategyName):
+        self._StrategyName = StrategyName
+
+    @property
+    def ScaleAction(self):
+        return self._ScaleAction
+
+    @ScaleAction.setter
+    def ScaleAction(self, ScaleAction):
+        self._ScaleAction = ScaleAction
+
+    @property
+    def ActionStatus(self):
+        return self._ActionStatus
+
+    @ActionStatus.setter
+    def ActionStatus(self, ActionStatus):
+        self._ActionStatus = ActionStatus
+
+    @property
+    def ActionTime(self):
+        return self._ActionTime
+
+    @ActionTime.setter
+    def ActionTime(self, ActionTime):
+        self._ActionTime = ActionTime
+
+    @property
+    def ScaleInfo(self):
+        return self._ScaleInfo
+
+    @ScaleInfo.setter
+    def ScaleInfo(self, ScaleInfo):
+        self._ScaleInfo = ScaleInfo
+
+    @property
+    def ExpectScaleNum(self):
+        return self._ExpectScaleNum
+
+    @ExpectScaleNum.setter
+    def ExpectScaleNum(self, ExpectScaleNum):
+        self._ExpectScaleNum = ExpectScaleNum
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def StrategyType(self):
+        return self._StrategyType
+
+    @StrategyType.setter
+    def StrategyType(self, StrategyType):
+        self._StrategyType = StrategyType
+
+    @property
+    def SpecInfo(self):
+        return self._SpecInfo
+
+    @SpecInfo.setter
+    def SpecInfo(self, SpecInfo):
+        self._SpecInfo = SpecInfo
+
+    @property
+    def CompensateFlag(self):
+        return self._CompensateFlag
+
+    @CompensateFlag.setter
+    def CompensateFlag(self, CompensateFlag):
+        self._CompensateFlag = CompensateFlag
+
+    @property
+    def CompensateCount(self):
+        return self._CompensateCount
+
+    @CompensateCount.setter
+    def CompensateCount(self, CompensateCount):
+        self._CompensateCount = CompensateCount
+
+
+    def _deserialize(self, params):
+        self._StrategyName = params.get("StrategyName")
+        self._ScaleAction = params.get("ScaleAction")
+        self._ActionStatus = params.get("ActionStatus")
+        self._ActionTime = params.get("ActionTime")
+        self._ScaleInfo = params.get("ScaleInfo")
+        self._ExpectScaleNum = params.get("ExpectScaleNum")
+        self._EndTime = params.get("EndTime")
+        self._StrategyType = params.get("StrategyType")
+        self._SpecInfo = params.get("SpecInfo")
+        self._CompensateFlag = params.get("CompensateFlag")
+        self._CompensateCount = params.get("CompensateCount")
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
 class BootstrapAction(AbstractModel):
     """引导脚本
 
     """
 
     def __init__(self):
         r"""
@@ -2924,14 +3079,142 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeAutoScaleRecordsRequest(AbstractModel):
+    """DescribeAutoScaleRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _Filters: 记录过滤参数，目前仅能为“StartTime”,“EndTime”和“StrategyName”。StartTime和EndTime支持2006-01-02 15:04:05 或者2006/01/02 15:04:05的时间格式
+        :type Filters: list of KeyValue
+        :param _Offset: 分页参数。
+        :type Offset: int
+        :param _Limit: 分页参数。最大支持100
+        :type Limit: int
+        """
+        self._InstanceId = None
+        self._Filters = None
+        self._Offset = None
+        self._Limit = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = KeyValue()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
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
+class DescribeAutoScaleRecordsResponse(AbstractModel):
+    """DescribeAutoScaleRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总扩缩容记录数。
+        :type TotalCount: int
+        :param _RecordList: 记录列表。
+        :type RecordList: list of AutoScaleRecord
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._RecordList = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def RecordList(self):
+        return self._RecordList
+
+    @RecordList.setter
+    def RecordList(self, RecordList):
+        self._RecordList = RecordList
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("RecordList") is not None:
+            self._RecordList = []
+            for item in params.get("RecordList"):
+                obj = AutoScaleRecord()
+                obj._deserialize(item)
+                self._RecordList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeClusterNodesRequest(AbstractModel):
     """DescribeClusterNodes请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7861,14 +8144,61 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class KeyValue(AbstractModel):
+    """键值对，主要用来做Filter
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Key: 键
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Key: str
+        :param _Value: 值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        """
+        self._Key = None
+        self._Value = None
+
+    @property
+    def Key(self):
+        return self._Key
+
+    @Key.setter
+    def Key(self, Key):
+        self._Key = Key
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+
+    def _deserialize(self, params):
+        self._Key = params.get("Key")
+        self._Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class LoginSettings(AbstractModel):
     """登录设置
 
     """
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.999/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,17 @@
 
 # CustomConfig参数值无效。
 INVALIDPARAMETER_INVALIDEXTENDFIELD = 'InvalidParameter.InvalidExtendField'
 
 # 无效的任务失败处理策略。
 INVALIDPARAMETER_INVALIDFAILUREPOLICY = 'InvalidParameter.InvalidFailurePolicy'
 
+# 无效过滤参数。
+INVALIDPARAMETER_INVALIDFILTERKEY = 'InvalidParameter.InvalidFilterKey'
+
 # 无效参数，EMR实例不符合要求。
 INVALIDPARAMETER_INVALIDINSTANCE = 'InvalidParameter.InvalidInstance'
 
 # 不合法的实例计费模式。
 INVALIDPARAMETER_INVALIDINSTANCECHARGETYPE = 'InvalidParameter.InvalidInstanceChargeType'
 
 # 无效的集群名称。
@@ -283,14 +286,17 @@
 
 # 软件名无效。
 INVALIDPARAMETER_INVALIDSOFTWARENAME = 'InvalidParameter.InvalidSoftWareName'
 
 # 软件版本无效。
 INVALIDPARAMETER_INVALIDSOFTWAREVERSION = 'InvalidParameter.InvalidSoftWareVersion'
 
+# invalid Parameter StartTime or EndTime.参数无效
+INVALIDPARAMETER_INVALIDSTARTTIMEORENDTIME = 'InvalidParameter.InvalidStartTimeOrEndTime'
+
 # 无效的子网ID。
 INVALIDPARAMETER_INVALIDSUBNETID = 'InvalidParameter.InvalidSubnetId'
 
 # 无效的高可用参数。
 INVALIDPARAMETER_INVALIDSUPPORTHA = 'InvalidParameter.InvalidSupportHA'
 
 # 参数错误。
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.999/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/README.rst` & `tencentcloud-sdk-python-emr-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.998/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.999/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.998/setup.py` & `tencentcloud-sdk-python-emr-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-emr',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Emr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

