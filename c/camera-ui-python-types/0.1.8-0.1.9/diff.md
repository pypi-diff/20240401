# Comparing `tmp/camera-ui-python-types-0.1.8.tar.gz` & `tmp/camera-ui-python-types-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camera-ui-python-types-0.1.8.tar", last modified: Wed Mar 20 19:36:43 2024, max compression
+gzip compressed data, was "camera-ui-python-types-0.1.9.tar", last modified: Wed Mar 20 22:30:51 2024, max compression
```

## Comparing `camera-ui-python-types-0.1.8.tar` & `camera-ui-python-types-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 19:36:43.833196 camera-ui-python-types-0.1.8/
--rw-r--r--   0 seydx      (501) staff       (20)      486 2024-03-20 19:36:43.832990 camera-ui-python-types-0.1.8/PKG-INFO
--rw-r--r--   0 seydx      (501) staff       (20)       26 2024-03-19 11:41:30.000000 camera-ui-python-types-0.1.8/README.md
-drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 19:36:43.832259 camera-ui-python-types-0.1.8/camera_ui_python_types/
--rw-r--r--   0 seydx      (501) staff       (20)    14517 2024-03-20 19:04:57.000000 camera-ui-python-types-0.1.8/camera_ui_python_types/__init__.py
-drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 19:36:43.832743 camera-ui-python-types-0.1.8/camera_ui_python_types.egg-info/
--rw-r--r--   0 seydx      (501) staff       (20)      486 2024-03-20 19:36:43.000000 camera-ui-python-types-0.1.8/camera_ui_python_types.egg-info/PKG-INFO
--rw-r--r--   0 seydx      (501) staff       (20)      237 2024-03-20 19:36:43.000000 camera-ui-python-types-0.1.8/camera_ui_python_types.egg-info/SOURCES.txt
--rw-r--r--   0 seydx      (501) staff       (20)        1 2024-03-20 19:36:43.000000 camera-ui-python-types-0.1.8/camera_ui_python_types.egg-info/dependency_links.txt
--rw-r--r--   0 seydx      (501) staff       (20)       23 2024-03-20 19:36:43.000000 camera-ui-python-types-0.1.8/camera_ui_python_types.egg-info/top_level.txt
--rw-r--r--   0 seydx      (501) staff       (20)       38 2024-03-20 19:36:43.833233 camera-ui-python-types-0.1.8/setup.cfg
--rw-r--r--   0 seydx      (501) staff       (20)      685 2024-03-20 19:36:41.000000 camera-ui-python-types-0.1.8/setup.py
+drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 22:30:51.546627 camera-ui-python-types-0.1.9/
+-rw-r--r--   0 seydx      (501) staff       (20)      486 2024-03-20 22:30:51.546414 camera-ui-python-types-0.1.9/PKG-INFO
+-rw-r--r--   0 seydx      (501) staff       (20)       26 2024-03-19 11:41:30.000000 camera-ui-python-types-0.1.9/README.md
+drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 22:30:51.545531 camera-ui-python-types-0.1.9/camera_ui_python_types/
+-rw-r--r--   0 seydx      (501) staff       (20)    14513 2024-03-20 22:30:31.000000 camera-ui-python-types-0.1.9/camera_ui_python_types/__init__.py
+drwxr-xr-x   0 seydx      (501) staff       (20)        0 2024-03-20 22:30:51.546185 camera-ui-python-types-0.1.9/camera_ui_python_types.egg-info/
+-rw-r--r--   0 seydx      (501) staff       (20)      486 2024-03-20 22:30:51.000000 camera-ui-python-types-0.1.9/camera_ui_python_types.egg-info/PKG-INFO
+-rw-r--r--   0 seydx      (501) staff       (20)      237 2024-03-20 22:30:51.000000 camera-ui-python-types-0.1.9/camera_ui_python_types.egg-info/SOURCES.txt
+-rw-r--r--   0 seydx      (501) staff       (20)        1 2024-03-20 22:30:51.000000 camera-ui-python-types-0.1.9/camera_ui_python_types.egg-info/dependency_links.txt
+-rw-r--r--   0 seydx      (501) staff       (20)       23 2024-03-20 22:30:51.000000 camera-ui-python-types-0.1.9/camera_ui_python_types.egg-info/top_level.txt
+-rw-r--r--   0 seydx      (501) staff       (20)       38 2024-03-20 22:30:51.546677 camera-ui-python-types-0.1.9/setup.cfg
+-rw-r--r--   0 seydx      (501) staff       (20)      685 2024-03-20 22:30:48.000000 camera-ui-python-types-0.1.9/setup.py
```

### Comparing `camera-ui-python-types-0.1.8/camera_ui_python_types/__init__.py` & `camera-ui-python-types-0.1.9/camera_ui_python_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -556,9 +556,9 @@
     @abstractmethod
     async def on_form_submit(self, action_id: str, payload: Any) -> Optional[dict]:
         pass
 
     @abstractmethod
     def configure_cameras(
         self, cameras: List[Any]
-    ) -> None:  # todo: replace Any with Camera Device
+    ) -> None:  # todo: replace with Camera Device
         pass
```

### Comparing `camera-ui-python-types-0.1.8/setup.py` & `camera-ui-python-types-0.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="camera-ui-python-types",
-    version="0.1.8",
+    version="0.1.9",
     description="camera.ui python types",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/seydx/camera.ui",
     author="seydx",
     author_email="dev@seydx.com",
     maintainer="seydx",
```

