# Comparing `tmp/ld-as-framework-0.0.8.tar.gz` & `tmp/ld-as-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ld-as-framework-0.0.8.tar", last modified: Sat Mar 30 14:05:43 2024, max compression
+gzip compressed data, was "ld-as-framework-0.0.9.tar", last modified: Mon Apr  1 14:32:29 2024, max compression
```

## Comparing `ld-as-framework-0.0.8.tar` & `ld-as-framework-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.478292 ld-as-framework-0.0.8/
--rw-rw-rw-   0        0        0     1093 2024-03-27 12:05:50.000000 ld-as-framework-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      887 2024-03-30 14:05:43.477316 ld-as-framework-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      412 2024-03-27 12:05:50.000000 ld-as-framework-0.0.8/README.md
--rw-rw-rw-   0        0        0      640 2024-03-30 14:05:24.000000 ld-as-framework-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 14:05:43.478292 ld-as-framework-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.436179 ld-as-framework-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.438133 ld-as-framework-0.0.8/src/ld/
--rw-rw-rw-   0        0        0      176 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.446476 ld-as-framework-0.0.8/src/ld/android/
--rw-rw-rw-   0        0        0     7137 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/LDFramework.py
--rw-rw-rw-   0        0        0      721 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.452335 ld-as-framework-0.0.8/src/ld/android/action/
--rw-rw-rw-   0        0        0      366 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/action/ColorActionStrategy.py
--rw-rw-rw-   0        0        0     5141 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/action/CommonClass.py
--rw-rw-rw-   0        0        0      335 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/action/ImageActionStrategy.py
--rw-rw-rw-   0        0        0     1189 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/action/NodeActionStrategy.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.455264 ld-as-framework-0.0.8/src/ld/android/base/
--rw-rw-rw-   0        0        0     1885 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/base/BaseProperties.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.462103 ld-as-framework-0.0.8/src/ld/android/element/
--rw-rw-rw-   0        0        0     1776 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/element/Color.py
--rw-rw-rw-   0        0        0     1012 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/element/Image.py
--rw-rw-rw-   0        0        0     1537 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/android/element/Node.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.469504 ld-as-framework-0.0.8/src/ld/common/
--rw-rw-rw-   0        0        0     3058 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/common/ListUtil.py
--rw-rw-rw-   0        0        0      267 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/common/Logger.py
--rw-rw-rw-   0        0        0     6733 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/common/StrUtil.py
--rw-rw-rw-   0        0        0      777 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/common/TimeUtil.py
--rw-rw-rw-   0        0        0     3154 2024-03-30 14:05:27.000000 ld-as-framework-0.0.8/src/ld/common/TypeUtil.py
-drwxrwxrwx   0        0        0        0 2024-03-30 14:05:43.477316 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/
--rw-rw-rw-   0        0        0      887 2024-03-30 14:05:43.000000 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-03-30 14:05:43.000000 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 14:05:43.000000 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-30 14:05:43.000000 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2024-03-30 14:05:43.000000 ld-as-framework-0.0.8/src/ld_as_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.397571 ld-as-framework-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2024-03-27 06:20:53.000000 ld-as-framework-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      887 2024-04-01 14:32:29.396598 ld-as-framework-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-03-27 06:20:53.000000 ld-as-framework-0.0.9/README.md
+-rw-rw-rw-   0        0        0      640 2024-04-01 13:59:39.000000 ld-as-framework-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:32:29.397571 ld-as-framework-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.388811 ld-as-framework-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.389785 ld-as-framework-0.0.9/src/ld/
+-rw-rw-rw-   0        0        0      177 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.390758 ld-as-framework-0.0.9/src/ld/android/
+-rw-rw-rw-   0        0        0     7865 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/LDFramework.py
+-rw-rw-rw-   0        0        0      701 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.390758 ld-as-framework-0.0.9/src/ld/android/action/
+-rw-rw-rw-   0        0        0     7292 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/action/CommonClass.py
+-rw-rw-rw-   0        0        0     1086 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/action/NodeActionStrategy.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.391731 ld-as-framework-0.0.9/src/ld/android/base/
+-rw-rw-rw-   0        0        0     1229 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/base/BaseProperties.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.392705 ld-as-framework-0.0.9/src/ld/android/element/
+-rw-rw-rw-   0        0        0     1762 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/element/Color.py
+-rw-rw-rw-   0        0        0     2071 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/element/Image.py
+-rw-rw-rw-   0        0        0      439 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/element/Node.py
+-rw-rw-rw-   0        0        0     3211 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/android/element/Ocr.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.393679 ld-as-framework-0.0.9/src/ld/common/
+-rw-rw-rw-   0        0        0     3058 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/common/ListUtil.py
+-rw-rw-rw-   0        0        0      265 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/common/Logger.py
+-rw-rw-rw-   0        0        0     6733 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/common/StrUtil.py
+-rw-rw-rw-   0        0        0      777 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/common/TimeUtil.py
+-rw-rw-rw-   0        0        0     3154 2024-04-01 14:32:24.000000 ld-as-framework-0.0.9/src/ld/common/TypeUtil.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:32:29.395624 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/
+-rw-rw-rw-   0        0        0      887 2024-04-01 14:32:29.000000 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-01 14:32:29.000000 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:32:29.000000 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 14:32:29.000000 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2024-04-01 14:32:29.000000 ld-as-framework-0.0.9/src/ld_as_framework.egg-info/top_level.txt
```

### Comparing `ld-as-framework-0.0.8/LICENSE` & `ld-as-framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ld-as-framework-0.0.8/PKG-INFO` & `ld-as-framework-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ld-as-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: 零动AS插件提示包
 Author-email: 零动学院 <1132454419@qq.com>
 Project-URL: Homepage, https://www.yuque.com/xianle-skqwj/ld
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ld-as-framework-0.0.8/pyproject.toml` & `ld-as-framework-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ld-as-framework"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "零动学院", email = "1132454419@qq.com" },
 ]
 dependencies = ['ascript-tip']
 description = "零动AS插件提示包"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `ld-as-framework-0.0.8/src/ld/android/LDFramework.py` & `ld-as-framework-0.0.9/src/ld/android/LDFramework.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # encoding:utf-8
 import math
 
 import random
 
 import time
 
+from ascript.android.screen import Ocr
+
 from ascript.android import action
 
 from ascript.android.action import Path
 
 from functools import reduce
 
 from ascript.android.screen import CompareColors
 
 from .action.CommonClass import CommonAction
 
 from .base.BaseProperties import AScriptQueryElement, CommonResult
 
-from .element.Color import ColorQuery
-
-from .element.Image import ImageQuery
-
-from .action.ColorActionStrategy import ColorActionStrategy
-
-from .action.ImageActionStrategy import ImageActionStrategy
-
 from .action.NodeActionStrategy import NodeActionStrategy
 
 from typing import cast
 
 from .element.Node import NodeQuery
 
+from .element.Ocr import PaddleocrV2, PaddleocrV3, Tesseract
+
 from ..common.Logger import log_ld
 
 class LDFramework:
 
     """
     零动框架操作类
     """
@@ -52,17 +48,16 @@
 
     def element(self, *args: str) -> CommonAction:
         """
         获取元素的方法，可以利用获取的元素进行一系列操作
         :param args:元素特征信息
         :return:元素操作对象
         """
-            # 如果需要处理的元素是图片
-            # 如果需要处理的元素是颜色
             # 如果需要处理的元素是节点
+            # 图片和颜色都是统一点击坐标，没有独特的行为方式，所以无需使用别的策略
         pass
 
     def element_exist(self, *args: str) -> CommonAction:
         """
         判断元素是否存在，如果存在返回元素的链式操作对象，不存在返回false
         :param args:
         :return:
@@ -162,14 +157,23 @@
         :return:
         """
         pass
 
         def tmp(tmp_element: list):
             pass
 
+    def ocr_paddleocr_v2(rect, confidence=0.6, max_side_len=1200, precision=16, bitmap=None, file=None) -> str:
+        pass
+
+    def ocr_paddleocr_v3(rect, confidence=0.6, max_side_len=1200, precision=16, bitmap=None, file=None) -> str:
+        pass
+
+    def ocr_tesseract(rect, data_file=Ocr.Tess_CHI, split_level=Ocr.RIL_AUTO, white_list=None, black_list=None) -> str:
+        pass
+
 class 零动框架:
 
     def __init__(self, 特征库: dict):
         pass
 
     def 元素_操作(self, *args: str) -> CommonAction:
         """
@@ -253,7 +257,18 @@
     def 等待_比色成功(self, element: list, timeout=5) -> bool:
         """
         在时间内等待比色成功，在规定时间内仍然比色失败，则返回False
         :param element: 特征信息
         :param timeout: 等待时间
         :return:
         """
+        pass
+
+    def 文字识别_飞浆2(self, rect, confidence=0.6, max_side_len=1200, precision=16, bitmap=None, file=None) -> str:
+        pass
+
+    def 文字识别_飞浆3(self, rect, confidence=0.6, max_side_len=1200, precision=16, bitmap=None, file=None) -> str:
+        pass
+
+    def 文字识别_Tesseract(self, rect, data_file=Ocr.Tess_CHI, split_level=Ocr.RIL_AUTO, white_list=None,
+        pass
+
```

### Comparing `ld-as-framework-0.0.8/src/ld/android/action/NodeActionStrategy.py` & `ld-as-framework-0.0.9/src/ld/android/action/NodeActionStrategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # encoding:utf-8
 from time import sleep
 
-from ascript.android.node import Selector
-
 from .CommonClass import CommonAction, Method
 
-from ..element.Node import NodeQuery, ElementNode
+from ..element.Node import NodeQuery
 
 from ...common.Logger import log_ld
 
 class NodeActionStrategy(CommonAction):
 
     """
     节点操作对象
     """
     def __init__(self, selector: NodeQuery, eleName, framework):
         pass
 
-    def _find(self):
-        return self
-
     def _click_element(self, r=5):
         return self
 
     def long_click(self):
         """
         长安查询到的节点信息，如果没有查询到则不执行
         """
```

### Comparing `ld-as-framework-0.0.8/src/ld/android/base/BaseProperties.py` & `ld-as-framework-0.0.9/src/ld/android/base/BaseProperties.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,8 @@
 # encoding:utf-8
-from android.graphics import Point
-
-from ascript.android.node import Node
-
-from ...common.Logger import log_ld
-
 class Rect:
 
     """
     获取控件在屏幕中的位置
 
     left x坐标
 
@@ -18,71 +12,43 @@
 
     height 控件的高度
 
     centerX 控件的中心坐标X
 
     centerY 控件的中心坐标Y
     """
-    def __init__(self, rect=None, left=None, top=None, width=None, height=None, centerX=None, centerY=None):
+    def __init__(self, left=None, top=None, width=None, height=None, centerX=None, centerY=None):
         self.left = left
         self.top = top
         self.width = width
         self.height = height
         self.centerX = centerX
         self.centerY = centerY
         pass
 
 class CommonResult:
 
     """
     查询元素的公共返回体
     """
-    def __init__(self, source_target, framework, find_range: [int, int, int, int] = None):
+    def __init__(self, source_target, rect: Rect):
         """
         调用获取元素方法后拿到的返回结果，经过统一包装
         :param source_target: 查询后的源对象
-        :param framework: 框架引用
-        :param find_range: 查询范围（节点没有）
-        """
-        pass
-
-    def _deal_color(self):
-        """
-        处理颜色对象的方法
-        """
-        pass
-
-    def _deal_node(self):
-        """
-        处理节点对象的方法
-        """
-        pass
-
-    def _deal_image(self):
-        """
-        处理图片对象的方法
-        :return:
-        """
-        pass
-
-    def click(self, r):
-        """
-        点击元素所在坐标
-        :param r: 随机偏移
-        :return:
+        :param rect: 查询后得到的坐标信息对象，要自行包装
         """
         pass
 
 class AScriptQueryElement:
 
     """
     AS元素查询父类，所有的元素查询都需要继承该类
     """
     def __init__(self):
         pass
 
-    def _find_element(self, eleName):
+    def _find_element(self, eleName) -> CommonResult:
         pass
 
-    def _find_all_element(self, eleName):
+    def _find_all_element(self, eleName) -> list:
         pass
```

### Comparing `ld-as-framework-0.0.8/src/ld/android/element/Color.py` & `ld-as-framework-0.0.9/src/ld/android/element/Color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding:utf-8
 from ascript.android.screen import FindColors
 
 from ...common.Logger import log_ld
 
-from ..base.BaseProperties import AScriptQueryElement, CommonResult
+from ..base.BaseProperties import AScriptQueryElement, CommonResult, Rect
 
 class ColorQuery(AScriptQueryElement):
 
     def __init__(self, colors: str):
         # 必填，颜色特征点, 通常用图色助手获取
         # 非必填，圈定屏幕范围
         # 必填，找色结果间距 默认:5像素 ,如果返回的结果,多个点位的像素值 在5像素内重合.则只保留一个
@@ -44,18 +44,16 @@
         """
         相似度, 取值范围0-1，1为100%匹配 默认:0.9
         :param diff: 相似度，取值范围0-1
         :return:
         """
         return self
 
-    def _find_element(self, eleName):
+    def _build_result(self, ele_target):
         pass
 
-    def _find_all_element(self, eleName):
+    def _find_element(self, eleName):
         pass
 
-class ElementColor(CommonResult):
-
-    def click(self, r):
+    def _find_all_element(self, eleName):
         pass
```

### Comparing `ld-as-framework-0.0.8/src/ld/android/element/Image.py` & `ld-as-framework-0.0.9/src/ld/android/element/Image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,88 @@
 # encoding:utf-8
 from ...common.Logger import log_ld
 
-from ..base.BaseProperties import AScriptQueryElement, CommonResult
+from ..base.BaseProperties import AScriptQueryElement, CommonResult, Rect
 
 from ascript.android.system import R
 
 from ascript.android.screen import FindImages
 
-class ImageQuery(AScriptQueryElement):
+class BaseImageQuery(AScriptQueryElement):
 
-    def __init__(self, mode="find"):
+    def __init__(self):
         # 局部图片名称或路径 当只填写图片名称时,将在res/img下找到该名称的图片
         # 非必填，圈定屏幕范围
         # 图片结果的可信度0-1之间, 1为100%匹配,低于该可信度的结果将被过滤掉 默认:0.9
         pass
 
+    def img(self, part_img: str):
+        return self
+
     def res(self, part_img: str):
         return self
 
     def sd(self, part_img: str):
         return self
 
     def rect(self, x, y, x1, y1):
         return self
 
     def confidence(self, confidence: float):
         return self
 
+    def _build_result(ele_target):
+        """
+        包装统一返回类
+        :param ele_target: 原始返回对象
+        """
+        pass
+
     def _find_element(self, eleName):
         pass
 
     def _find_all_element(self, eleName):
         pass
 
-class ElementImage(CommonResult):
+class ImageFindQuery(BaseImageQuery):
+
+    def __init__(self):
+        pass
+
+    def _find_all_element(self, eleName):
+        pass
+
+class ImageFindTemplateQuery(BaseImageQuery):
+
+    def __init__(self):
+        # 参数为False: 使用灰度图匹配
+        # 参数为True:使用原色图匹配.
+        pass
+
+    def rgb(self, rgb: bool = True):
+        return self
+
+    def _find_all_element(self, eleName):
+        # 查询所有也没有rgb
+        pass
+
+class ImageFindSiftQuery(BaseImageQuery):
+
+    def __init__(self):
+        # 参数为False: 使用灰度图匹配
+        # 参数为True:使用原色图匹配.
+        pass
+
+    def _find_all_element(self, eleName):
+        pass
+
+class ImageQuery:
+
+    def find() -> ImageFindQuery:
+        pass
+
+    def find_template() -> ImageFindTemplateQuery:
+        pass
 
-    def click(self, r):
+    def find_sift() -> ImageFindSiftQuery:
         pass
```

### Comparing `ld-as-framework-0.0.8/src/ld/common/ListUtil.py` & `ld-as-framework-0.0.9/src/ld/common/ListUtil.py`

 * *Files identical despite different names*

### Comparing `ld-as-framework-0.0.8/src/ld/common/StrUtil.py` & `ld-as-framework-0.0.9/src/ld/common/StrUtil.py`

 * *Files identical despite different names*

### Comparing `ld-as-framework-0.0.8/src/ld/common/TimeUtil.py` & `ld-as-framework-0.0.9/src/ld/common/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `ld-as-framework-0.0.8/src/ld/common/TypeUtil.py` & `ld-as-framework-0.0.9/src/ld/common/TypeUtil.py`

 * *Files identical despite different names*

### Comparing `ld-as-framework-0.0.8/src/ld_as_framework.egg-info/PKG-INFO` & `ld-as-framework-0.0.9/src/ld_as_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ld-as-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: 零动AS插件提示包
 Author-email: 零动学院 <1132454419@qq.com>
 Project-URL: Homepage, https://www.yuque.com/xianle-skqwj/ld
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ld-as-framework-0.0.8/src/ld_as_framework.egg-info/SOURCES.txt` & `ld-as-framework-0.0.9/src/ld_as_framework.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 src/ld/__init__.py
 src/ld/android/LDFramework.py
 src/ld/android/__init__.py
-src/ld/android/action/ColorActionStrategy.py
 src/ld/android/action/CommonClass.py
-src/ld/android/action/ImageActionStrategy.py
 src/ld/android/action/NodeActionStrategy.py
 src/ld/android/base/BaseProperties.py
 src/ld/android/element/Color.py
 src/ld/android/element/Image.py
 src/ld/android/element/Node.py
+src/ld/android/element/Ocr.py
 src/ld/common/ListUtil.py
 src/ld/common/Logger.py
 src/ld/common/StrUtil.py
 src/ld/common/TimeUtil.py
 src/ld/common/TypeUtil.py
 src/ld_as_framework.egg-info/PKG-INFO
 src/ld_as_framework.egg-info/SOURCES.txt
```

