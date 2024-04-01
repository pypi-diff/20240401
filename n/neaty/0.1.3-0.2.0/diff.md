# Comparing `tmp/neaty-0.1.3.tar.gz` & `tmp/neaty-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neaty-0.1.3.tar", last modified: Thu May 18 17:00:47 2023, max compression
+gzip compressed data, was "neaty-0.2.0.tar", last modified: Mon Apr  1 17:30:05 2024, max compression
```

## Comparing `neaty-0.1.3.tar` & `neaty-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      604 2023-05-18 17:00:47.977938 neaty-0.1.3/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)    11957 2023-05-18 17:00:47.821933 neaty-0.1.3/setup.py
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/src/
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/src/neaty/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      993 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/__init__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)      530 2023-05-18 17:00:47.077908 neaty-0.1.3/src/neaty/_meta.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     2588 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/log.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     7628 2023-05-18 15:00:46.615036 neaty-0.1.3/src/neaty/neaty.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/py.typed
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 17:30:05.601594 neaty-0.2.0/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    26338 2020-08-03 17:39:40.000000 neaty-0.2.0/LICENSE.md
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1211 2024-04-01 17:30:05.601594 neaty-0.2.0/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       55 2020-08-03 17:39:40.000000 neaty-0.2.0/README.md
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 17:30:05.601594 neaty-0.2.0/neaty.egg-info/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1211 2024-04-01 17:30:05.000000 neaty-0.2.0/neaty.egg-info/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      241 2024-04-01 17:30:05.000000 neaty-0.2.0/neaty.egg-info/SOURCES.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        1 2024-04-01 17:30:05.000000 neaty-0.2.0/neaty.egg-info/dependency_links.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        6 2024-04-01 17:30:05.000000 neaty-0.2.0/neaty.egg-info/top_level.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2024-04-01 17:30:05.601594 neaty-0.2.0/setup.cfg
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    12182 2024-04-01 17:30:00.000000 neaty-0.2.0/setup.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 17:30:05.601594 neaty-0.2.0/src/
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 17:30:05.601594 neaty-0.2.0/src/neaty/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      993 2023-03-07 15:22:03.000000 neaty-0.2.0/src/neaty/__init__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      530 2024-04-01 17:29:59.000000 neaty-0.2.0/src/neaty/_meta.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1131 2024-04-01 17:22:02.000000 neaty-0.2.0/src/neaty/log.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     7628 2023-05-18 15:00:46.000000 neaty-0.2.0/src/neaty/neaty.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:22:03.000000 neaty-0.2.0/src/neaty/py.typed
```

### Comparing `neaty-0.1.3/setup.py` & `neaty-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,36 +129,36 @@
     '__VDK_PYLIB_PKGMAP__',
 ]
 
 VDK_PYLIB_DEFAULT_PKGMAP = """
 neaty src/neaty py.typed
 """
 
-VDK_PYLIB_REQUIRES_PYSTUFF = [
-    '__VDK_PYLIB_REQUIRES_PYSTUFF__',
-]
-
 VDK_PYLIB_CLASSIFIERS_OVERRIDE = [
     '__VDK_PYLIB_CLASSIFIERS_OVERRIDE__',
 ]
 
 VDK_PYLIB_CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Natural Language :: English',
 ]
 
 VDK_PYLIB_PYTHON_GE = """
-3.9
+__VDK_PYLIB_PYTHON_GE__
 """
 
 VDK_PYLIB_PYTHON_LT = """
-3.11
+__VDK_PYLIB_PYTHON_LT__
 """
 
+VDK_PYPI_REQUIRES = [
+    '__VDK_PYPI_REQUIRES__',
+]
+
 MKIT_PROJ_LICENSE = """
 LGPLv2
 """
 
 
 class PackageMapItem:
 
@@ -264,20 +264,25 @@
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
     def __str__(self):
         return f"{self.x}.{self.y}"
 
+    def __eq__(self, othr):
+        return (self.x, self.y) == (othr.x, othr.y)
+
     def __lt__(self, othr):
         return (self.x, self.y) < (othr.x, othr.y)
 
     def range_to(self, othr):
         if othr < self:
             raise ValueError(f"impossible version range: {self} to {othr}")
+        if othr == self:
+            yield self
         for rx in range(self.x, othr.x+1):
             for ry in range(self.y, othr.y):
                 yield self.__class__(rx, ry)
 
     def as_classifier(self):
         return f'Programming Language :: Python :: {self.x}.{self.y}'
 
@@ -288,19 +293,19 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
     ]
 
     @classmethod
     def from_macros(cls):
         ver_ge_txt = vdk_cleanup(VDK_PYLIB_PYTHON_GE) or '3.0'
-        ver_lt_txt = vdk_cleanup(VDK_PYLIB_PYTHON_LT) or '3.12'
+        ver_lt_txt = vdk_cleanup(VDK_PYLIB_PYTHON_LT) or '3.13'
         ver_ge = VersionNumber.from_text(ver_ge_txt)
         ver_lt = VersionNumber.from_text(ver_lt_txt)
         return cls(
-            versions=ver_ge.range_to(ver_lt)
+            versions=list(ver_ge.range_to(ver_lt))
         )
 
     def __init__(self, versions):
         self.versions = versions
 
     @property
     def classifiers(self):
@@ -333,23 +338,26 @@
 
 def vdk_packageinfo():
     pmap = PackageMap.from_macros()
     pmeta = PackageMeta.from_macros()
     return pmap.as_dict() | pmeta.as_dict()
 
 
+VDK_PACKAGEINFO = vdk_packageinfo()
+
 setup(
     description='neaty - Neaty logger',
     license='LGPLv2',
     long_description=vdk_cleanup(VDK_PYLIB_DESCRIPTION),
+    long_description_content_type='text/markdown',
     maintainer_email='Alois Mahdal <netvor+neaty@vornet.cz>',
     name='neaty',
-    packages=vdk_packageinfo()['packages'],
-    package_dir=vdk_packageinfo()['package_dir'],
-    package_data=vdk_packageinfo()['package_data'],
+    packages=VDK_PACKAGEINFO['packages'],
+    package_dir=VDK_PACKAGEINFO['package_dir'],
+    package_data=VDK_PACKAGEINFO['package_data'],
     url='https://gitlab.com/vornet/python/python-neaty',
-    requires=vdk_cleanup(VDK_PYLIB_REQUIRES_PYSTUFF),
-    version='0.1.3',
-    classifiers=vdk_packageinfo()['classifiers'],
+    requires=vdk_cleanup(VDK_PYPI_REQUIRES),
+    version='0.2.0',
+    classifiers=VDK_PACKAGEINFO['classifiers'],
 )
 
-# setup.py built with MKit 0.0.60 and vdk-pylib-0.0.31
+# setup.py built with MKit 0.1.3 and vdk-pylib-0.1.1
```

### Comparing `neaty-0.1.3/src/neaty/__init__.py` & `neaty-0.2.0/src/neaty/__init__.py`

 * *Files identical despite different names*

### Comparing `neaty-0.1.3/src/neaty/_meta.py` & `neaty-0.2.0/src/neaty/_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CODENAME: str = """
 
 """.strip()
 
 GIT_LASTHASH: str = """
-52283d543c687ff829df4f67d811682336e43ce9
+7e4f3d20a07b2f425fe0584284e3808d20599f3e
 """.strip()
 
 GIT_LASTSUMMARY: str = """
-Bump version to 0.1.3
+Bump version to 0.2.0
 """.strip()
 
 LICENSE: str = """
 LGPLv2
 """.strip()
 
 MAINTAINER: str = """
@@ -31,9 +31,9 @@
 """.strip()
 
 VCS_BROWSER: str = """
 https://gitlab.com/vornet/python/python-neaty
 """.strip()
 
 VERSION: str = """
-0.1.3
+0.2.0
 """.strip()
```

### Comparing `neaty-0.1.3/src/neaty/neaty.py` & `neaty-0.2.0/src/neaty/neaty.py`

 * *Files identical despite different names*

