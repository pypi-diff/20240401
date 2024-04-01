# Comparing `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1120.tar.gz` & `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1120.tar", last modified: Sun Mar 31 20:28:35 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1121.tar", last modified: Mon Apr  1 20:31:57 2024, max compression
```

## Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120.tar` & `tencentcloud-sdk-python-cdwdoris-3.0.1121.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/
--rw-r--r--   0 root         (0) root         (0)      703 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   124055 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16479 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1083 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/setup.py
--rw-r--r--   0 root         (0) root         (0)      752 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      550 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-31 20:28:34.000000 tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/
+-rw-r--r--   0 root         (0) root         (0)      703 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   129648 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16479 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/setup.py
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 20:31:57.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-01 20:31:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1120
+Version: 3.0.1121
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/errorcodes.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/models.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,28 +407,34 @@
         :param _HaType: 高可用类型：
 0：非高可用（只有1个FE，FeSpec.CreateInstanceSpec.Count=1），
 1：读高可用（至少需部署3个FE，FeSpec.CreateInstanceSpec.Count>=3，且为奇数），
 2：读写高可用（至少需部署5个FE，FeSpec.CreateInstanceSpec.Count>=5，且为奇数）。
         :type HaType: int
         :param _CaseSensitive: 表名大小写是否敏感，0：敏感；1：不敏感，以小写进行比较；2：不敏感，表名改为以小写存储
         :type CaseSensitive: int
+        :param _EnableMultiZones: 是否开启多可用区
+        :type EnableMultiZones: bool
+        :param _UserMultiZoneInfos: 开启多可用区后，用户的所有可用区和子网信息
+        :type UserMultiZoneInfos: :class:`tencentcloud.cdwdoris.v20211228.models.NetworkInfo`
         """
         self._Zone = None
         self._FeSpec = None
         self._BeSpec = None
         self._HaFlag = None
         self._UserVPCId = None
         self._UserSubnetId = None
         self._ProductVersion = None
         self._ChargeProperties = None
         self._InstanceName = None
         self._DorisUserPwd = None
         self._Tags = None
         self._HaType = None
         self._CaseSensitive = None
+        self._EnableMultiZones = None
+        self._UserMultiZoneInfos = None
 
     @property
     def Zone(self):
         return self._Zone
 
     @Zone.setter
     def Zone(self, Zone):
@@ -526,14 +532,30 @@
     def CaseSensitive(self):
         return self._CaseSensitive
 
     @CaseSensitive.setter
     def CaseSensitive(self, CaseSensitive):
         self._CaseSensitive = CaseSensitive
 
+    @property
+    def EnableMultiZones(self):
+        return self._EnableMultiZones
+
+    @EnableMultiZones.setter
+    def EnableMultiZones(self, EnableMultiZones):
+        self._EnableMultiZones = EnableMultiZones
+
+    @property
+    def UserMultiZoneInfos(self):
+        return self._UserMultiZoneInfos
+
+    @UserMultiZoneInfos.setter
+    def UserMultiZoneInfos(self, UserMultiZoneInfos):
+        self._UserMultiZoneInfos = UserMultiZoneInfos
+
 
     def _deserialize(self, params):
         self._Zone = params.get("Zone")
         if params.get("FeSpec") is not None:
             self._FeSpec = CreateInstanceSpec()
             self._FeSpec._deserialize(params.get("FeSpec"))
         if params.get("BeSpec") is not None:
@@ -552,14 +574,18 @@
             self._Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self._Tags.append(obj)
         self._HaType = params.get("HaType")
         self._CaseSensitive = params.get("CaseSensitive")
+        self._EnableMultiZones = params.get("EnableMultiZones")
+        if params.get("UserMultiZoneInfos") is not None:
+            self._UserMultiZoneInfos = NetworkInfo()
+            self._UserMultiZoneInfos._deserialize(params.get("UserMultiZoneInfos"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2662,14 +2688,20 @@
         :type CaseSensitive: int
         :param _IsWhiteSGs: 用户是否可以绑定安全组
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsWhiteSGs: bool
         :param _BindSGs: 已绑定的安全组信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type BindSGs: list of str
+        :param _EnableMultiZones: 是否为多可用区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnableMultiZones: bool
+        :param _UserNetworkInfos: 用户可用区和子网信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserNetworkInfos: str
         """
         self._InstanceId = None
         self._InstanceName = None
         self._Status = None
         self._Version = None
         self._Region = None
         self._Zone = None
@@ -2706,14 +2738,16 @@
         self._IfExistCatalog = None
         self._Characteristic = None
         self._RestartTimeout = None
         self._GraceShutdownWaitSeconds = None
         self._CaseSensitive = None
         self._IsWhiteSGs = None
         self._BindSGs = None
+        self._EnableMultiZones = None
+        self._UserNetworkInfos = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -3055,14 +3089,30 @@
     def BindSGs(self):
         return self._BindSGs
 
     @BindSGs.setter
     def BindSGs(self, BindSGs):
         self._BindSGs = BindSGs
 
+    @property
+    def EnableMultiZones(self):
+        return self._EnableMultiZones
+
+    @EnableMultiZones.setter
+    def EnableMultiZones(self, EnableMultiZones):
+        self._EnableMultiZones = EnableMultiZones
+
+    @property
+    def UserNetworkInfos(self):
+        return self._UserNetworkInfos
+
+    @UserNetworkInfos.setter
+    def UserNetworkInfos(self, UserNetworkInfos):
+        self._UserNetworkInfos = UserNetworkInfos
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._InstanceName = params.get("InstanceName")
         self._Status = params.get("Status")
         self._Version = params.get("Version")
         self._Region = params.get("Region")
@@ -3109,14 +3159,16 @@
         self._IfExistCatalog = params.get("IfExistCatalog")
         self._Characteristic = params.get("Characteristic")
         self._RestartTimeout = params.get("RestartTimeout")
         self._GraceShutdownWaitSeconds = params.get("GraceShutdownWaitSeconds")
         self._CaseSensitive = params.get("CaseSensitive")
         self._IsWhiteSGs = params.get("IsWhiteSGs")
         self._BindSGs = params.get("BindSGs")
+        self._EnableMultiZones = params.get("EnableMultiZones")
+        self._UserNetworkInfos = params.get("UserNetworkInfos")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3346,30 +3398,110 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class NetworkInfo(AbstractModel):
+    """网络信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Zone: 可用区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Zone: str
+        :param _SubnetId: 子网id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param _SubnetIpNum: 当前子网可用ip数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetIpNum: int
+        """
+        self._Zone = None
+        self._SubnetId = None
+        self._SubnetIpNum = None
+
+    @property
+    def Zone(self):
+        return self._Zone
+
+    @Zone.setter
+    def Zone(self, Zone):
+        self._Zone = Zone
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+    @property
+    def SubnetIpNum(self):
+        return self._SubnetIpNum
+
+    @SubnetIpNum.setter
+    def SubnetIpNum(self, SubnetIpNum):
+        self._SubnetIpNum = SubnetIpNum
+
+
+    def _deserialize(self, params):
+        self._Zone = params.get("Zone")
+        self._SubnetId = params.get("SubnetId")
+        self._SubnetIpNum = params.get("SubnetIpNum")
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
 class NodeInfo(AbstractModel):
     """NodeInfo
 
     """
 
     def __init__(self):
         r"""
         :param _Ip: 用户IP
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ip: str
         :param _Status: 节点状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
+        :param _NodeName: 节点角色名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeName: str
+        :param _ComponentName: 组件名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentName: str
+        :param _NodeRole: 节点角色
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeRole: str
+        :param _LastRestartTime: 节点上次重启的时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastRestartTime: str
+        :param _Zone: 节点所在可用区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Zone: str
         """
         self._Ip = None
         self._Status = None
+        self._NodeName = None
+        self._ComponentName = None
+        self._NodeRole = None
+        self._LastRestartTime = None
+        self._Zone = None
 
     @property
     def Ip(self):
         return self._Ip
 
     @Ip.setter
     def Ip(self, Ip):
@@ -3379,18 +3511,63 @@
     def Status(self):
         return self._Status
 
     @Status.setter
     def Status(self, Status):
         self._Status = Status
 
+    @property
+    def NodeName(self):
+        return self._NodeName
+
+    @NodeName.setter
+    def NodeName(self, NodeName):
+        self._NodeName = NodeName
+
+    @property
+    def ComponentName(self):
+        return self._ComponentName
+
+    @ComponentName.setter
+    def ComponentName(self, ComponentName):
+        self._ComponentName = ComponentName
+
+    @property
+    def NodeRole(self):
+        return self._NodeRole
+
+    @NodeRole.setter
+    def NodeRole(self, NodeRole):
+        self._NodeRole = NodeRole
+
+    @property
+    def LastRestartTime(self):
+        return self._LastRestartTime
+
+    @LastRestartTime.setter
+    def LastRestartTime(self, LastRestartTime):
+        self._LastRestartTime = LastRestartTime
+
+    @property
+    def Zone(self):
+        return self._Zone
+
+    @Zone.setter
+    def Zone(self, Zone):
+        self._Zone = Zone
+
 
     def _deserialize(self, params):
         self._Ip = params.get("Ip")
         self._Status = params.get("Status")
+        self._NodeName = params.get("NodeName")
+        self._ComponentName = params.get("ComponentName")
+        self._NodeRole = params.get("NodeRole")
+        self._LastRestartTime = params.get("LastRestartTime")
+        self._Zone = params.get("Zone")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1120'
+__version__ = '3.0.1121'
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/setup.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwdoris',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1120"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1121"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwdoris SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/README.rst` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1120
+Version: 3.0.1121
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1120/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwdoris-3.0.1121/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

