# Comparing `tmp/paperplotlib-0.0.1.tar.gz` & `tmp/paperplotlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperplotlib-0.0.1.tar", max compression
+gzip compressed data, was "paperplotlib-0.0.2.tar", max compression
```

## Comparing `paperplotlib-0.0.1.tar` & `paperplotlib-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-03-24 12:11:55.505650 paperplotlib-0.0.1/LICENSE
--rw-r--r--   0        0        0       90 2024-03-31 09:00:50.490081 paperplotlib-0.0.1/paperplotlib/__init__.py
--rw-r--r--   0        0        0      582 2024-03-31 13:28:42.095294 paperplotlib-0.0.1/paperplotlib/bar_graph.py
--rw-r--r--   0        0        0      654 2024-03-31 13:45:26.164686 paperplotlib-0.0.1/paperplotlib/color.css
--rw-r--r--   0        0        0     1061 2024-03-31 13:44:29.622325 paperplotlib-0.0.1/paperplotlib/color.py
--rw-r--r--   0        0        0      410 2024-03-24 12:37:00.984651 paperplotlib-0.0.1/paperplotlib/display.py
--rw-r--r--   0        0        0      963 2024-03-31 13:07:46.133903 paperplotlib-0.0.1/paperplotlib/graph.py
--rw-r--r--   0        0        0      114 2024-03-26 11:56:54.539725 paperplotlib-0.0.1/paperplotlib/line_graph.py
--rw-r--r--   0        0        0      463 2024-03-31 14:00:07.894325 paperplotlib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1085 2024-03-31 08:51:20.330642 paperplotlib-0.0.1/README.md
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 paperplotlib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-24 12:11:55.505650 paperplotlib-0.0.2/LICENSE
+-rw-r--r--   0        0        0       90 2024-03-31 09:00:50.490081 paperplotlib-0.0.2/paperplotlib/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-01 13:21:16.836152 paperplotlib-0.0.2/paperplotlib/bar_graph.py
+-rw-r--r--   0        0        0      518 2024-04-01 13:22:28.733641 paperplotlib-0.0.2/paperplotlib/color.css
+-rw-r--r--   0        0        0     2849 2024-04-01 13:19:56.767956 paperplotlib-0.0.2/paperplotlib/color.py
+-rw-r--r--   0        0        0     2664 2024-04-01 13:04:44.432619 paperplotlib-0.0.2/paperplotlib/graph.py
+-rw-r--r--   0        0        0      114 2024-03-26 11:56:54.539725 paperplotlib-0.0.2/paperplotlib/line_graph.py
+-rw-r--r--   0        0        0      502 2024-04-01 13:57:08.467884 paperplotlib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1425 2024-04-01 13:53:07.741280 paperplotlib-0.0.2/README.md
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 paperplotlib-0.0.2/PKG-INFO
```

### Comparing `paperplotlib-0.0.1/LICENSE` & `paperplotlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paperplotlib-0.0.1/README.md` & `paperplotlib-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # paperplotlib
 
+> 本项目还处于早期开发阶段, 欢迎反馈建议
+
 paperplotlib 是基于 matplotlib 的论文实验数据绘图库, 意在快速绘制论文实验结果部分中常见的柱状图/折线图
 
 本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对简洁的 API 调用
 
-一些绘制的示例代码和结果图见: [paperplotlib 示例]()
+一些绘制的示例代码和结果图见: [paperplotlib 示例](https://luzhixing12345.github.io/paperplotlib/articles/md-docs/使用示例/)
 
-## 安装与使用
+## 安装
 
 ```bash
 pip install paperplotlib
 ```
 
+## 快速开始
+
 ```python
 import paperplotlib as ppl
+import numpy as np
 
-x = [2, 4, 8, 16, 32]
-y = [0.1, 0.5, 0.7, 0.9, 1.0]
+# 随机生成一个 5 x 7 的数据
+a = 5
+b = 7
+y = np.random.randint(10, 100, size=(a, b))
+
+group_names = [f"group {i}" for i in range(a)]
+column_names = [f"column {i}" for i in range(b)]
 
 graph = ppl.BarGraph()
-graph.plot(x, y)
+graph.plot_2d(y, group_names, column_names)
 graph.x_label = "The number of data"
 graph.y_label = "Throughput (Mbps)"
-
-graph.save("test.png")
+graph.save()
 ```
 
-![](./test.png)
+![](./images/paperplotlib/result.png)
 
 使用文档: [paperplotlib document](https://luzhixing12345.github.io/paperplotlib/)
 
 ## 参考
 
 - [matplotlib](https://matplotlib.org/stable/users/index.html)
 - [matplotlib.pyplot的使用总结大全](https://www.zhihu.com/tardis/zm/art/139052035?source_id=1003)
 - [matplotlib.pyplot常用函数讲解大全(一)](https://zhuanlan.zhihu.com/p/139475633)
-- [matplotlib.pyplot常用函数讲解大全(二)](https://zhuanlan.zhihu.com/p/139946399)
+- [matplotlib.pyplot常用函数讲解大全(二)](https://zhuanlan.zhihu.com/p/139946399)
```

### Comparing `paperplotlib-0.0.1/PKG-INFO` & `paperplotlib-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 Metadata-Version: 2.1
 Name: paperplotlib
-Version: 0.0.1
-Summary: 1
+Version: 0.0.2
+Summary: 论文实验数据绘图
 Home-page: https://github.com/luzhixing12345/paperplotlib
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Project-URL: Documentation, https://luzhixing12345.github.io/paperplotlib/
 Project-URL: Repository, https://github.com/luzhixing12345/paperplotlib
 Description-Content-Type: text/markdown
 
 # paperplotlib
 
+> 本项目还处于早期开发阶段, 欢迎反馈建议
+
 paperplotlib 是基于 matplotlib 的论文实验数据绘图库, 意在快速绘制论文实验结果部分中常见的柱状图/折线图
 
 本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对简洁的 API 调用
 
-一些绘制的示例代码和结果图见: [paperplotlib 示例]()
+一些绘制的示例代码和结果图见: [paperplotlib 示例](https://luzhixing12345.github.io/paperplotlib/articles/md-docs/使用示例/)
 
-## 安装与使用
+## 安装
 
 ```bash
 pip install paperplotlib
 ```
 
+## 快速开始
+
 ```python
 import paperplotlib as ppl
+import numpy as np
+
+# 随机生成一个 5 x 7 的数据
+a = 5
+b = 7
+y = np.random.randint(10, 100, size=(a, b))
 
-x = [2, 4, 8, 16, 32]
-y = [0.1, 0.5, 0.7, 0.9, 1.0]
+group_names = [f"group {i}" for i in range(a)]
+column_names = [f"column {i}" for i in range(b)]
 
 graph = ppl.BarGraph()
-graph.plot(x, y)
+graph.plot_2d(y, group_names, column_names)
 graph.x_label = "The number of data"
 graph.y_label = "Throughput (Mbps)"
-
-graph.save("test.png")
+graph.save()
 ```
 
-![](./test.png)
+![](./images/paperplotlib/result.png)
 
 使用文档: [paperplotlib document](https://luzhixing12345.github.io/paperplotlib/)
 
 ## 参考
 
 - [matplotlib](https://matplotlib.org/stable/users/index.html)
 - [matplotlib.pyplot的使用总结大全](https://www.zhihu.com/tardis/zm/art/139052035?source_id=1003)
 - [matplotlib.pyplot常用函数讲解大全(一)](https://zhuanlan.zhihu.com/p/139475633)
 - [matplotlib.pyplot常用函数讲解大全(二)](https://zhuanlan.zhihu.com/p/139946399)
+
```

