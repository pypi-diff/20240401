# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.998.tar", last modified: Fri Oct 13 00:20:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.999.tar", last modified: Mon Oct 16 00:20:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.998.tar` & `tencentcloud-sdk-python-batch-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)    31661 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   301995 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1076 2023-10-13 00:20:58.000000 tencentcloud-sdk-python-batch-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    31661 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302061 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-10-16 00:20:14.000000 tencentcloud-sdk-python-batch-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1584,17 +1584,17 @@
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeleteWithInstance: bool
         :param _SnapshotId: 数据盘快照ID。选择的数据盘快照大小需小于数据盘大小。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotId: str
         :param _Encrypt: 数据盘是加密。取值范围：
-<li>TRUE：加密
-<li>FALSE：不加密<br>
-默认取值：FALSE<br>
+<li>true：加密
+<li>false：不加密<br>
+默认取值：false<br>
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Encrypt: bool
         :param _KmsKeyId: 自定义CMK对应的ID，取值为UUID或者类似kms-abcd1234。用于加密云盘。
 
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -7762,15 +7762,15 @@
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
@@ -7795,15 +7795,16 @@
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
@@ -9412,15 +9413,15 @@
 
     def __init__(self):
         r"""
         :param _VpcId: 私有网络ID，形如`vpc-xxx`。有效的VpcId可通过登录[控制台](https://console.cloud.tencent.com/vpc/vpc?rid=1)查询；也可以调用接口 [DescribeVpcEx](/document/api/215/1372) ，从接口返回中的`unVpcId`字段获取。若在创建子机时VpcId与SubnetId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type VpcId: str
         :param _SubnetId: 私有网络子网ID，形如`subnet-xxx`。有效的私有网络子网ID可通过登录[控制台](https://console.cloud.tencent.com/vpc/subnet?rid=1)查询；也可以调用接口  [DescribeSubnets](/document/api/215/15784) ，从接口返回中的`unSubnetId`字段获取。若在创建子机时SubnetId与VpcId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type SubnetId: str
-        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>TRUE：表示用作公网网关<br><li>FALSE：表示不作为公网网关<br><br>默认取值：FALSE。
+        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>true：表示用作公网网关<br><li>false：表示不作为公网网关<br><br>默认取值：false。
         :type AsVpcGateway: bool
         :param _PrivateIpAddresses: 私有网络子网 IP 数组，在创建实例、修改实例vpc属性操作中可使用此参数。当前仅批量创建多台实例时支持传入相同子网的多个 IP。
         :type PrivateIpAddresses: list of str
         :param _Ipv6AddressCount: 为弹性网卡指定随机生成的 IPv6 地址数量。
         :type Ipv6AddressCount: int
         """
         self._VpcId = None
```

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.998/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-batch-3.0.999/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.999/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.998/README.rst` & `tencentcloud-sdk-python-batch-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.998/setup.py` & `tencentcloud-sdk-python-batch-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-batch',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Batch SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

