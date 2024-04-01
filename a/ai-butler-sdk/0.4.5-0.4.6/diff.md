# Comparing `tmp/ai_butler_sdk-0.4.5.tar.gz` & `tmp/ai_butler_sdk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_butler_sdk-0.4.5.tar", max compression
+gzip compressed data, was "ai_butler_sdk-0.4.6.tar", max compression
```

## Comparing `ai_butler_sdk-0.4.5.tar` & `ai_butler_sdk-0.4.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2024-03-05 08:48:36.042873 ai_butler_sdk-0.4.5/ai_butler_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 01:59:14.986379 ai_butler_sdk-0.4.5/ai_butler_sdk/apis/__init__.py
--rw-r--r--   0        0        0     3154 2024-03-25 09:55:14.636724 ai_butler_sdk-0.4.5/ai_butler_sdk/apis/client.py
--rw-r--r--   0        0        0     1638 2024-03-26 07:50:09.843149 ai_butler_sdk-0.4.5/ai_butler_sdk/celery_app/__init__.py
--rw-r--r--   0        0        0     1155 2024-03-11 01:59:08.060645 ai_butler_sdk-0.4.5/ai_butler_sdk/celery_app/task_example.py
--rw-r--r--   0        0        0     5320 2024-03-26 05:42:18.476153 ai_butler_sdk-0.4.5/ai_butler_sdk/deploy_onnx.py
--rw-r--r--   0        0        0     1128 2024-03-26 03:22:01.404933 ai_butler_sdk-0.4.5/ai_butler_sdk/settings.py
--rw-r--r--   0        0        0     6051 2024-03-25 10:43:18.071678 ai_butler_sdk-0.4.5/ai_butler_sdk/train.py
--rw-r--r--   0        0        0     5303 2024-03-27 08:27:43.941506 ai_butler_sdk-0.4.5/ai_butler_sdk/utils.py
--rw-r--r--   0        0        0      783 2024-03-27 08:27:50.278494 ai_butler_sdk-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 ai_butler_sdk-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-03-05 08:48:36.042873 ai_butler_sdk-0.4.6/ai_butler_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 01:59:14.986379 ai_butler_sdk-0.4.6/ai_butler_sdk/apis/__init__.py
+-rw-r--r--   0        0        0     3154 2024-03-25 09:55:14.636724 ai_butler_sdk-0.4.6/ai_butler_sdk/apis/client.py
+-rw-r--r--   0        0        0     1638 2024-03-26 07:50:09.843149 ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/__init__.py
+-rw-r--r--   0        0        0     1213 2024-04-01 09:31:19.919697 ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/task_example.py
+-rw-r--r--   0        0        0     5410 2024-04-01 09:31:19.926210 ai_butler_sdk-0.4.6/ai_butler_sdk/deploy_onnx.py
+-rw-r--r--   0        0        0     1128 2024-03-26 03:22:01.404933 ai_butler_sdk-0.4.6/ai_butler_sdk/settings.py
+-rw-r--r--   0        0        0     6051 2024-03-25 10:43:18.071678 ai_butler_sdk-0.4.6/ai_butler_sdk/train.py
+-rw-r--r--   0        0        0     5303 2024-03-27 08:27:43.941506 ai_butler_sdk-0.4.6/ai_butler_sdk/utils.py
+-rw-r--r--   0        0        0      783 2024-04-01 09:31:28.021618 ai_butler_sdk-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 ai_butler_sdk-0.4.6/PKG-INFO
```

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/apis/client.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/apis/client.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/celery_app/__init__.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/celery_app/task_example.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/celery_app/task_example.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,11 +32,12 @@
         pretrain_model_weight_download_url,
     )
     mock_train()
 
 
 @celery_app.task
 def deploy_onnx_infer_by_train_task(
-    deploy_id: str, inner_token: str, train_result_url: str | None = None, is_gpu: bool = False
+    deploy_id: str, inner_token: str, train_result_url: str | None = None, is_gpu: bool = False,
+    service_type: str = "OBJECT_DETECTION"
 ):
-    deploy_onnx_infer = DeployOnnxInfer(deploy_id, inner_token, train_result_url, is_gpu)
+    deploy_onnx_infer = DeployOnnxInfer(deploy_id, inner_token, train_result_url, service_type, is_gpu)
     deploy_onnx_infer()
```

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/deploy_onnx.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/deploy_onnx.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 import traceback
 import random
 
 
 class DeployOnnxInfer:
     """部署onnx推理服务基类"""
 
-    def __init__(self, deploy_task_id, token, train_task_result_url, is_gpu=False, base_dir: str = ""):
+    def __init__(self, deploy_task_id, token, train_task_result_url, service_type, is_gpu=False, base_dir: str = ""):
         self.deploy_task_id = deploy_task_id
         self.token = token
+        self.service_type = service_type
         self.train_task_result_url = train_task_result_url
         self.onnx_weight_path = os.path.join(
             base_dir, f"output/deploy/{deploy_task_id}/{settings.DEPLOY_ONNX_WEIGHT_DIR}"
         )
         os.makedirs(self.onnx_weight_path, exist_ok=True)
         self.is_gpu = is_gpu
         if is_gpu:
@@ -80,15 +81,15 @@
         f"{settings.DEPLOY_TARGET_CONTAINER_WORKDIR}/{settings.DEPLOY_ONNX_WEIGHT_DIR}"
         bind_dir = os.path.join(settings.DEPLOY_TARGET_CONTAINER_WORKDIR, settings.DEPLOY_ONNX_WEIGHT_DIR)
         container = client.containers.run(
             image=self.docker_image_name,
             detach=True,  # 是否以后台模式运行
             volumes={os.path.join(settings.DEPLOY_HOST_DIR, self.onnx_weight_path): {"bind": bind_dir, "mode": "rw"}},
             ports={"8000/tcp": port},  # 端口映射，这里将容器的80端口映射到主机的8080端口
-            environment={"AUTHENTICATION_TOKEN": self.token, "IS_GPU": self.is_gpu},
+            environment={"AUTHENTICATION_TOKEN": self.token, "IS_GPU": self.is_gpu, "SERVICE_TYPE": self.service_type},
             name=container_name,  # 容器名称
         )
         container_id = container.id
         return container_id
 
     def __call__(self, *args, **kwargs):
         try:
```

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/settings.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/train.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/train.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.5/ai_butler_sdk/utils.py` & `ai_butler_sdk-0.4.6/ai_butler_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ai_butler_sdk-0.4.5/pyproject.toml` & `ai_butler_sdk-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   "UP",  # pyupgrade
 ]
 line-length = 120
 exclude = [".mypy_cache", ".*", "logs", "static", "migrations"]
 
 [tool.poetry]
 name = "ai-butler-sdk"
-version = "0.4.5"
+version = "0.4.6"
 description = "AI模型生产管理平台sdk"
 authors = ["王凡 <wangfan@keanbang.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 minio = "^7.2.5"
 httpx = "^0.27.0"
```

### Comparing `ai_butler_sdk-0.4.5/PKG-INFO` & `ai_butler_sdk-0.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-butler-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: AI模型生产管理平台sdk
 Author: 王凡
 Author-email: wangfan@keanbang.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

