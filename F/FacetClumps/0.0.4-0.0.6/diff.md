# Comparing `tmp/FacetClumps-0.0.4.tar.gz` & `tmp/FacetClumps-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FacetClumps-0.0.4.tar", last modified: Fri May  5 16:27:08 2023, max compression
+gzip compressed data, was "dist\FacetClumps-0.0.6.tar", last modified: Mon Apr  1 13:06:16 2024, max compression
```

## Comparing `FacetClumps-0.0.4.tar` & `FacetClumps-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.958453 FacetClumps-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.915564 FacetClumps-0.0.4/FacetClumps/
--rw-rw-rw-   0        0        0      743 2023-05-05 15:06:54.000000 FacetClumps-0.0.4/FacetClumps/Detect_FacetClumps.py
--rw-rw-rw-   0        0        0      639 2023-01-28 03:02:47.000000 FacetClumps-0.0.4/FacetClumps/Detect_Files.py
--rw-rw-rw-   0        0        0     9276 2023-05-05 14:27:26.000000 FacetClumps-0.0.4/FacetClumps/Detect_Files_Funs.py
--rw-rw-rw-   0        0        0    21417 2023-05-05 16:26:42.000000 FacetClumps-0.0.4/FacetClumps/FacetClumps_2D_Funs.py
--rw-rw-rw-   0        0        0    26590 2023-05-05 14:32:47.000000 FacetClumps-0.0.4/FacetClumps/FacetClumps_3D_Funs.py
--rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.4/FacetClumps/Test_File.py
--rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.4/FacetClumps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.945487 FacetClumps-0.0.4/FacetClumps.egg-info/
--rw-rw-rw-   0        0        0      197 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.955462 FacetClumps-0.0.4/FacetClumps_Code/
--rw-rw-rw-   0        0        0      639 2023-01-28 03:02:47.000000 FacetClumps-0.0.4/FacetClumps_Code/Detect_Files.py
--rw-rw-rw-   0        0        0    21494 2023-03-02 01:54:55.000000 FacetClumps-0.0.4/FacetClumps_Code/FacetClumps_2D_Funs.py
--rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.4/FacetClumps_Code/Test_File.py
--rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.4/FacetClumps_Code/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-05 16:27:08.957455 FacetClumps-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-02-28 04:15:08.000000 FacetClumps-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 16:27:08.958453 FacetClumps-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-05-05 14:45:15.000000 FacetClumps-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:06:16.525303 FacetClumps-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:06:16.517303 FacetClumps-0.0.6/FacetClumps/
+-rw-rw-rw-   0        0        0      743 2023-05-05 15:06:54.000000 FacetClumps-0.0.6/FacetClumps/Detect_FacetClumps.py
+-rw-rw-rw-   0        0        0      639 2023-01-28 03:02:47.000000 FacetClumps-0.0.6/FacetClumps/Detect_Files.py
+-rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.6/FacetClumps/Test_File.py
+-rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.6/FacetClumps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:06:16.521303 FacetClumps-0.0.6/FacetClumps.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-01 13:06:16.000000 FacetClumps-0.0.6/FacetClumps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-01 13:06:16.000000 FacetClumps-0.0.6/FacetClumps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:06:16.000000 FacetClumps-0.0.6/FacetClumps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 13:06:16.000000 FacetClumps-0.0.6/FacetClumps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      182 2024-04-01 13:06:16.521303 FacetClumps-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-02-28 04:15:08.000000 FacetClumps-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:06:16.525303 FacetClumps-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1314 2024-04-01 13:05:55.000000 FacetClumps-0.0.6/setup.py
```

### Comparing `FacetClumps-0.0.4/FacetClumps/Detect_FacetClumps.py` & `FacetClumps-0.0.6/FacetClumps/Detect_FacetClumps.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.0.4/FacetClumps/Detect_Files.py` & `FacetClumps-0.0.6/FacetClumps/Detect_Files.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.0.4/setup.py` & `FacetClumps-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FacetClumps',  # 包名
-    version='0.0.4',  # 版本 0.3, 0.0.3
-    description="FacetClumps: A molecular cloud clump detection algorithm based on Facet model",  # 包简介
+    version='0.0.6',  # 版本 0.3, 0.0.4
+    description="FacetClumps: A Facet-based Molecular Clump Detection Algorithm",  # 包简介
     # long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     # include_package_data=True,  # 是否允许上传资源文件
     author='Jiang Yu',  # 作者
     author_email="yujiang@pmo.ac.cn",  # 作者邮件
     # maintainer='',  # 维护者
     # maintainer_email="yujiang@pmo.ac.cn",  # 维护者邮件
     # license='MIT License',  # 协议
```

