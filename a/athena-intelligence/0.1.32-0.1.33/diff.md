# Comparing `tmp/athena_intelligence-0.1.32.tar.gz` & `tmp/athena_intelligence-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.32.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.33.tar", max compression
```

## Comparing `athena_intelligence-0.1.32.tar` & `athena_intelligence-0.1.33.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     4235 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/README.md
--rw-r--r--   0        0        0      435 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/pyproject.toml
--rw-r--r--   0        0        0      905 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/__init__.py
--rw-r--r--   0        0        0     4806 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/base_client.py
--rw-r--r--   0        0        0     3576 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12215 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-14 18:41:27.955577 athena_intelligence-0.1.32/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/snippet/client.py
--rw-r--r--   0        0        0      918 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/dataset.py
--rw-r--r--   0        0        0      989 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     1979 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/status_enum.py
--rw-r--r--   0        0        0     1277 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/tools.py
--rw-r--r--   0        0        0      992 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-14 18:41:27.959577 athena_intelligence-0.1.32/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/README.md
+-rw-r--r--   0        0        0      435 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0      905 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/base_client.py
+-rw-r--r--   0        0        0     3576 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/snippet/client.py
+-rw-r--r--   0        0        0      918 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/dataset.py
+-rw-r--r--   0        0        0      989 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2390 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0     1277 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/tools.py
+-rw-r--r--   0        0        0      992 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.33/PKG-INFO
```

### Comparing `athena_intelligence-0.1.32/README.md` & `athena_intelligence-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/__init__.py` & `athena_intelligence-0.1.33/src/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/base_client.py` & `athena_intelligence-0.1.33/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/client.py` & `athena_intelligence-0.1.33/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/__init__.py` & `athena_intelligence-0.1.33/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.33/src/athena/core/client_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.32",
+            "X-Fern-SDK-Version": "0.1.33",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.32/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.33/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/file.py` & `athena_intelligence-0.1.33/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/http_client.py` & `athena_intelligence-0.1.33/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.33/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/core/request_options.py` & `athena_intelligence-0.1.33/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/dataset/client.py` & `athena_intelligence-0.1.33/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/message/client.py` & `athena_intelligence-0.1.33/src/athena/message/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.message.submit(
             content="visit www.athenaintelligence.ai and summarize the website in one paragraph",
-            model=Model.GPT_3_5_TURBO,
-            tools=[Tools.SEARCH, Tools.BROWSE, Tools.SEARCH],
+            model=Model.GPT_35_TURBO,
+            tools=[Tools.SEARCH, Tools.BROWSE],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"content": content}
         if model is not OMIT:
             _request["model"] = model
         if tools is not OMIT:
             _request["tools"] = tools
@@ -189,16 +189,16 @@
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.message.submit(
             content="visit www.athenaintelligence.ai and summarize the website in one paragraph",
-            model=Model.GPT_3_5_TURBO,
-            tools=[Tools.SEARCH, Tools.BROWSE, Tools.SEARCH],
+            model=Model.GPT_35_TURBO,
+            tools=[Tools.SEARCH, Tools.BROWSE],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"content": content}
         if model is not OMIT:
             _request["model"] = model
         if tools is not OMIT:
             _request["tools"] = tools
```

### Comparing `athena_intelligence-0.1.32/src/athena/polling_message_client.py` & `athena_intelligence-0.1.33/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/query/client.py` & `athena_intelligence-0.1.33/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/report/client.py` & `athena_intelligence-0.1.33/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/snippet/client.py` & `athena_intelligence-0.1.33/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/__init__.py` & `athena_intelligence-0.1.33/src/athena/types/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/dataset.py` & `athena_intelligence-0.1.33/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.33/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.33/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.33/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/message_out.py` & `athena_intelligence-0.1.33/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.33/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/model.py` & `athena_intelligence-0.1.33/src/athena/types/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,26 +16,30 @@
     GPT_4 = "gpt-4"
     MIXTRAL_SMALL_8_X_7_B_0211 = "mixtral-small-8x7b-0211"
     MISTRAL_LARGE_0224 = "mistral-large-0224"
     LLAMA_V_270_B_CHAT = "llama-v2-70b-chat"
     CLAUDE_3_OPUS_20240229 = "claude-3-opus-20240229"
     CLAUDE_3_SONNET_20240229 = "claude-3-sonnet-20240229"
     CLAUDE_3_HAIKU_20240307 = "claude-3-haiku-20240307"
+    GOOGLE_GEMINI_10_PRO_LATEST = "google-gemini-1.0-pro-latest"
+    DATABRICKS_DBRX = "databricks-dbrx"
 
     def visit(
         self,
         gpt_35_turbo: typing.Callable[[], T_Result],
         gpt_4_turbo_preview: typing.Callable[[], T_Result],
         gpt_4: typing.Callable[[], T_Result],
         mixtral_small_8_x_7_b_0211: typing.Callable[[], T_Result],
         mistral_large_0224: typing.Callable[[], T_Result],
         llama_v_270_b_chat: typing.Callable[[], T_Result],
         claude_3_opus_20240229: typing.Callable[[], T_Result],
         claude_3_sonnet_20240229: typing.Callable[[], T_Result],
         claude_3_haiku_20240307: typing.Callable[[], T_Result],
+        google_gemini_10_pro_latest: typing.Callable[[], T_Result],
+        databricks_dbrx: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is Model.GPT_35_TURBO:
             return gpt_35_turbo()
         if self is Model.GPT_4_TURBO_PREVIEW:
             return gpt_4_turbo_preview()
         if self is Model.GPT_4:
             return gpt_4()
@@ -47,7 +51,11 @@
             return llama_v_270_b_chat()
         if self is Model.CLAUDE_3_OPUS_20240229:
             return claude_3_opus_20240229()
         if self is Model.CLAUDE_3_SONNET_20240229:
             return claude_3_sonnet_20240229()
         if self is Model.CLAUDE_3_HAIKU_20240307:
             return claude_3_haiku_20240307()
+        if self is Model.GOOGLE_GEMINI_10_PRO_LATEST:
+            return google_gemini_10_pro_latest()
+        if self is Model.DATABRICKS_DBRX:
+            return databricks_dbrx()
```

### Comparing `athena_intelligence-0.1.32/src/athena/types/report.py` & `athena_intelligence-0.1.33/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/snippet.py` & `athena_intelligence-0.1.33/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/sql_results.py` & `athena_intelligence-0.1.33/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/status_enum.py` & `athena_intelligence-0.1.33/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/tools.py` & `athena_intelligence-0.1.33/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/src/athena/types/validation_error.py` & `athena_intelligence-0.1.33/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.32/PKG-INFO` & `athena_intelligence-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.32
+Version: 0.1.33
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

