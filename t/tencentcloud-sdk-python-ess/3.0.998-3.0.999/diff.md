# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.998.tar", last modified: Fri Oct 13 00:28:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.999.tar", last modified: Mon Oct 16 00:27:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.998.tar` & `tencentcloud-sdk-python-ess-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   601905 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)   116342 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24653 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:28:02.000000 tencentcloud-sdk-python-ess-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   602461 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)   116342 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24792 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:27:20.000000 tencentcloud-sdk-python-ess-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.998/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.999/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1609,14 +1609,28 @@
         :type ComponentName: str
         :param _ComponentRequired: 是否必选，默认为false-非必选
         :type ComponentRequired: bool
         :param _ComponentRecipientId: 控件关联的参与方ID，对应Recipient结构体中的RecipientId
         :type ComponentRecipientId: str
         :param _ComponentExtra: 扩展参数：
 为JSON格式。
+不同类型的控件会有部分非通用参数
+
+ComponentType为TEXT、MULTI_LINE_TEXT时，支持以下参数：
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+4 FontColor：字符串类型，格式为RGB颜色数字
+参数样例：    "ComponentExtra": "{\"FontColor\":\"255,0,0\",\"FontSize\":12}"
+
+TEXT/MULTI_LINE_TEXT控件可以指定
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+例如：{"FontSize":12}
 
 ComponentType为FILL_IMAGE时，支持以下参数：
 NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
 FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
 
 ComponentType为SIGN_SIGNATURE类型可以控制签署方式
 {“ComponentTypeLimit”: [“xxx”]}
@@ -1631,19 +1645,19 @@
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+参数样例： "ComponentExtra": "{"Format":“yyyy m d”,"FontSize":12,"Gaps":"2,2", "FontAlign":"Right"}"
 
 ComponentType为SIGN_SEAL类型时，支持以下参数：
 1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
-参数样例："ComponentExtra":"{\"PageRanges\":[{\"BeginPage\":1,\"EndPage\":-1}]}"
+参数样例： "ComponentExtra":"{"PageRange":[{"BeginPage":1,"EndPage":-1}]}"
         :type ComponentExtra: str
         :param _IsFormType: 是否是表单域类型，默认false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param _ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
```

### Comparing `tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.998/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.999/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 # 签署流程已有关联文档，请检查参数修改后重试。
 FAILEDOPERATION_FLOWHASDOCUMENT = 'FailedOperation.FlowHasDocument'
 
 # 流程未找到关联的电子文件信息，请检查操作步骤，检查参数，并在修改后重试。
 FAILEDOPERATION_FLOWHASNODOCUMENT = 'FailedOperation.FlowHasNoDocument'
 
+# 身份信息校验不通过，请确认后重试。
+FAILEDOPERATION_IDCARDNUMBERCHECKFAILED = 'FailedOperation.IdCardNumberCheckFailed'
+
 # 当前无可用的许可
 FAILEDOPERATION_LICENSENOQUOTA = 'FailedOperation.LicenseNoQuota'
 
 # 签署审核未通过，请先完成审核。
 FAILEDOPERATION_NOSIGNREVIEWPASS = 'FailedOperation.NoSignReviewPass'
 
 # 此合同流程不支持审批
```

### Comparing `tencentcloud-sdk-python-ess-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.999/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.998/README.rst` & `tencentcloud-sdk-python-ess-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.998/setup.py` & `tencentcloud-sdk-python-ess-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ess',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ess SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

