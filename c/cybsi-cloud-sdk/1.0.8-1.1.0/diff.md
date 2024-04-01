# Comparing `tmp/cybsi_cloud_sdk-1.0.8.tar.gz` & `tmp/cybsi_cloud_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybsi_cloud_sdk-1.0.8.tar", max compression
+gzip compressed data, was "cybsi_cloud_sdk-1.1.0.tar", max compression
```

## Comparing `cybsi_cloud_sdk-1.0.8.tar` & `cybsi_cloud_sdk-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,40 @@
--rw-r--r--   0        0        0    10142 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/LICENSE
--rw-r--r--   0        0        0      626 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/README.md
--rw-r--r--   0        0        0      151 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/__init__.py
--rw-r--r--   0        0        0      195 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/__version__.py
--rw-r--r--   0        0        0      405 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/__init__.py
--rw-r--r--   0        0        0     1362 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/api.py
--rw-r--r--   0        0        0      426 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/__init__.py
--rw-r--r--   0        0        0      412 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/api.py
--rw-r--r--   0        0        0     8370 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/api_key.py
--rw-r--r--   0        0        0     1551 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/permission.py
--rw-r--r--   0        0        0     2159 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/resource.py
--rw-r--r--   0        0        0      821 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/token.py
--rw-r--r--   0        0        0     3764 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/client.py
--rw-r--r--   0        0        0     5631 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/client_config.py
--rw-r--r--   0        0        0      829 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/enum.py
--rw-r--r--   0        0        0     7971 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/error.py
--rw-r--r--   0        0        0      257 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/__init__.py
--rw-r--r--   0        0        0     2046 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/base.py
--rw-r--r--   0        0        0     6864 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/connector.py
--rw-r--r--   0        0        0      870 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/time.py
--rw-r--r--   0        0        0      595 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/__init__.py
--rw-r--r--   0        0        0     1200 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/api.py
--rw-r--r--   0        0        0     9771 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/collection.py
--rw-r--r--   0        0        0    15218 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/objects.py
--rw-r--r--   0        0        0     8513 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/schemas.py
--rw-r--r--   0        0        0     4302 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/pagination.py
--rw-r--r--   0        0        0      520 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/cloud/view.py
--rw-r--r--   0        0        0        0 2023-12-06 10:27:42.172896 cybsi_cloud_sdk-1.0.8/cybsi/py.typed
--rw-r--r--   0        0        0     1163 2023-12-06 10:27:42.176896 cybsi_cloud_sdk-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/LICENSE
+-rw-r--r--   0        0        0      626 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0      151 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/__version__.py
+-rw-r--r--   0        0        0      405 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/__init__.py
+-rw-r--r--   0        0        0     1362 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/api.py
+-rw-r--r--   0        0        0      539 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/__init__.py
+-rw-r--r--   0        0        0      412 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api.py
+-rw-r--r--   0        0        0     8864 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api_key.py
+-rw-r--r--   0        0        0     1814 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/limits.py
+-rw-r--r--   0        0        0     1551 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/permission.py
+-rw-r--r--   0        0        0     2159 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/resource.py
+-rw-r--r--   0        0        0      821 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/token.py
+-rw-r--r--   0        0        0     4393 2024-04-01 09:50:59.042470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/client.py
+-rw-r--r--   0        0        0     5631 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/client_config.py
+-rw-r--r--   0        0        0      829 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/enum.py
+-rw-r--r--   0        0        0     9679 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/error.py
+-rw-r--r--   0        0        0      306 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/files/__init__.py
+-rw-r--r--   0        0        0    23274 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/files/files.py
+-rw-r--r--   0        0        0      541 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/api.py
+-rw-r--r--   0        0        0     8823 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/schemas.py
+-rw-r--r--   0        0        0     7897 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/task_queue.py
+-rw-r--r--   0        0        0     7492 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/insight/tasks.py
+-rw-r--r--   0        0        0      257 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/base.py
+-rw-r--r--   0        0        0     8226 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/buffer.py
+-rw-r--r--   0        0        0     7192 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/connector.py
+-rw-r--r--   0        0        0     1755 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/multipart.py
+-rw-r--r--   0        0        0      870 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/time.py
+-rw-r--r--   0        0        0      595 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/api.py
+-rw-r--r--   0        0        0     9771 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/collection.py
+-rw-r--r--   0        0        0    15217 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/objects.py
+-rw-r--r--   0        0        0     8513 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/schemas.py
+-rw-r--r--   0        0        0     4302 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/pagination.py
+-rw-r--r--   0        0        0      520 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/cloud/view.py
+-rw-r--r--   0        0        0        0 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/cybsi/py.typed
+-rw-r--r--   0        0        0     1163 2024-04-01 09:50:59.046470 cybsi_cloud_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.1.0/PKG-INFO
```

### Comparing `cybsi_cloud_sdk-1.0.8/LICENSE` & `cybsi_cloud_sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/README.md` & `cybsi_cloud_sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/api.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/api_key.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/api_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     JsonObject,
     JsonObjectForm,
     JsonObjectView,
     parse_rfc3339_timestamp,
     rfc3339_timestamp,
 )
 from ..pagination import Cursor, Page
+from .limits import RequestLimitForm, RequestLimitView
 from .permission import ResourcePermissionForm, ResourcePermissionView
 from .token import TokenView
 
 logger = logging.getLogger(__name__)
 
 
 class APIKeyAuth(httpx.Auth):
@@ -192,28 +193,32 @@
     This is the form you need to fill to generate API-Key.
 
     Args:
         permissions: List of permissions.
         expires_at: Expiration date.
             The API-Key is automatically disabled after the expiration date.
         description: API-Key description.
+        request_limits: List of API-Key request limits.
     """
 
     def __init__(
         self,
         permissions: Iterable[ResourcePermissionForm],
         *,
+        request_limits: Optional[Iterable[RequestLimitForm]] = None,
         expires_at: Optional[datetime] = None,
         description: Optional[str] = None,
     ):
         super().__init__()
         if expires_at is not None:
             self._data["expiresAt"] = rfc3339_timestamp(expires_at)
         if description is not None:
             self._data["description"] = description
+        if request_limits is not None:
+            self._data["requestLimits"] = [limit.json() for limit in request_limits]
         self._data["permissions"] = [perm.json() for perm in permissions]
 
 
 class APIKeyRegistrationView(JsonObjectView):
     """API-Key view."""
 
     @property
@@ -264,7 +269,12 @@
         """API-Key revoked flag."""
         return self._get("revoked")
 
     @property
     def permissions(self) -> List[ResourcePermissionView]:
         """List of permissions."""
         return [ResourcePermissionView(perm) for perm in self._get("permissions")]
+
+    @property
+    def request_limits(self) -> List[RequestLimitView]:
+        """List of request limits."""
+        return [RequestLimitView(limit) for limit in self._get("requestLimits")]
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/permission.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/permission.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/resource.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/resource.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/auth/token.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/auth/token.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/client.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .auth import APIKeyAuth, AuthAPI
 from .client_config import Config
+from .files import FilesAPI, FilesAsyncAPI
+from .insight.api import InsightAPI, InsightAsyncAPI
 from .internal import AsyncHTTPConnector, HTTPConnector
 from .iocean import IOCeanAPI, IOCeanAsyncAPI
 
 
 class Client:
     """The main entry point for all actions with Cybsi Cloud REST API.
 
@@ -73,14 +75,24 @@
         return AuthAPI(self._connector)
 
     @property
     def iocean(self) -> IOCeanAPI:
         """IOCean API handle."""
         return IOCeanAPI(self._connector)
 
+    @property
+    def insight(self) -> InsightAPI:
+        """Insight API handle."""
+        return InsightAPI(self._connector)
+
+    @property
+    def files(self) -> FilesAPI:
+        """Files API handle."""
+        return FilesAPI(self._connector)
+
 
 class AsyncClient:
     """The asynchronous analog of :class:`Client`.
 
     As you can see, the asynchronous client has fewer features than synchronous one.
     This is because we don't simply copy-paste features,
     but provide them only when they're actually useful in asynchronous applications.
@@ -116,7 +128,17 @@
         """Close client and release connections."""
         await self._connector.aclose()
 
     @property
     def iocean(self) -> IOCeanAsyncAPI:
         """IOCean asynchronous API handle."""
         return IOCeanAsyncAPI(self._connector)
+
+    @property
+    def insight(self) -> InsightAsyncAPI:
+        """Insight asynchronous API handle."""
+        return InsightAsyncAPI(self._connector)
+
+    @property
+    def files(self) -> FilesAsyncAPI:
+        """Files API handle."""
+        return FilesAsyncAPI(self._connector)
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/client_config.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/client_config.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/enum.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/enum.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/error.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,94 +85,123 @@
     """
 
     BadRequest = "BadRequest"
     InvalidData = "InvalidData"
     InvalidPathArgument = "InvalidPathArgument"
     InvalidQueryArgument = "InvalidQueryArgument"
 
-    def __init__(self, content: JsonObject) -> None:
-        super().__init__(400, content, header="invalid request")
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(400, resp.json(), header="invalid request")
 
 
 class UnauthorizedError(APIError):
     """Client lacks valid authentication credentials. Retry will never work."""
 
     Unauthorized = "Unauthorized"
 
-    def __init__(self, content: JsonObject) -> None:
-        super().__init__(401, content, header="operation not authorized")
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(401, resp.json(), header="operation not authorized")
 
 
 class ForbiddenError(APIError):
     """Operation was forbidden. Retry will not work unless system is reconfigured."""
 
-    def __init__(self, content: JsonObject) -> None:
-        super().__init__(403, content, header="operation forbidden")
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(403, resp.json(), header="operation forbidden")
 
     @property
     def code(self) -> "ForbiddenErrorCodes":
         """Error code."""
         return ForbiddenErrorCodes(self._view.code)
 
 
 class NotFoundError(APIError):
     """Requested resource not found. Retry will never work."""
 
-    def __init__(self, content: JsonObject) -> None:
+    def __init__(self, resp: httpx.Response) -> None:
         super().__init__(404, {}, header="resource not found", suffix="")
 
 
 class ConflictError(APIError):
     """Resource already exists. Retry will never work."""
 
-    def __init__(self, content: JsonObject) -> None:
-        super().__init__(409, content, header="resource already exists")
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(409, resp.json(), header="resource already exists")
 
     @property
     def code(self) -> "ConflictErrorCodes":
         """Error code."""
         return ConflictErrorCodes(self._view.code)
 
 
 class ResourceModifiedError(APIError):
     """Resource was modified since last read. **Retry is a must**.
 
     Read the updated resource from API, and apply your modifications again.
     """
 
-    def __init__(self, content: JsonObject) -> None:
+    def __init__(self, resp: httpx.Response) -> None:
         super().__init__(
-            412, content, header="resource was modified since last read", suffix=""
+            412, resp.json(), header="resource was modified since last read", suffix=""
         )
 
 
 class RequestEntityTooLargeError(APIError):
     """Request content is too large."""
 
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(
+            413, resp.json(), header="request content is too large", suffix=""
+        )
+
+
+class RangeNotSatisfiableError(APIError):
     def __init__(self, content: JsonObject) -> None:
-        super().__init__(413, content, header="request content is too large", suffix="")
+        super().__init__(416, content, header="range is not satisfiable", suffix="")
 
 
 class SemanticError(APIError):
     """Semantic error. Retry will not work (almost always).
 
     Request syntax was valid, but system business rules forbid the request.
 
     For example, we're trying to unpack an artifact, but the artifact is not an archive.
     """
 
-    def __init__(self, content: JsonObject) -> None:
-        super().__init__(422, content, header="semantic error")
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(422, resp.json(), header="semantic error")
 
     @property
     def code(self) -> "SemanticErrorCodes":
         """Error code."""
         return SemanticErrorCodes(self._view.code)
 
 
+class TooManyRequestsError(APIError):
+    """Too many requests error.
+
+    Retry request after some time.
+    """
+
+    def __init__(self, resp: httpx.Response) -> None:
+        super().__init__(429, resp.json(), header="too many requests error")
+        retry_after = resp.headers.get("Retry-After")
+        self._retry_after = int(retry_after) if retry_after is not None else None
+
+    @property
+    def code(self) -> "TooManyRequestsErrorCodes":
+        """Error code."""
+        return TooManyRequestsErrorCodes(self._view.code)
+
+    @property
+    def retry_after(self) -> Optional[int]:
+        """Period in seconds after which request could be repeated."""
+        return self._retry_after
+
+
 @document_enum
 class ForbiddenErrorCodes(CybsiAPIEnum):
     """Possible error codes of :class:`ForbiddenError`."""
 
     MissingPermissions = "MissingPermissions"
     """Authenticated but not authorized to perform operation."""
     Forbidden = "Forbidden"
@@ -195,26 +224,52 @@
 
     ResourceNotFound = "ResourceNotFound"
     """Cloud resource not found."""
     InvalidSchemaID = "InvalidSchemaID"
     """schemaID parameter can't be changed."""
     SchemaNotFound = "SchemaNotFound"
     """The specified schema is not found"""
+    InvalidRequestLimit = "InvalidRequestLimit"
+    """The specified request limit cannot be set."""
+    LimitSetConflict = "LimitSetConflict"
+    """The limit set has conflicts."""
 
     # Objects
     InvalidKeyFormat = "InvalidKeyFormat"
     """Object key has invalid format."""
     InvalidKeySet = "InvalidKeySet"
     """Object has invalid key set."""
     KeySetConflict = "KeySetConflict"
     """Object key intersects with another one."""
     SchemaCheckFail = "SchemaCheckFail"
     """Object validation by schema failed."""
     CursorOutOfRange = "CursorOutOfRange"
     """Cursor for collection changes is obsolete."""
+    InvalidFilePart = "InvalidFilePart"
+    """File part is invalid"""
+    MissingFilePart = "MissingFilePart"
+    """File part is missing"""
+
+    # Filebox
+    FileNotFound = "FileNotFound"
+    """File not found."""
+
+    # Tasks
+    TaskNotFound = "TaskNotFound"
+    """Task not found."""
+    InvalidState = "InvalidState"
+    """Invalid task state."""
+
+
+@document_enum
+class TooManyRequestsErrorCodes(CybsiAPIEnum):
+    """Too many requests error codes."""
+
+    LimitExceeded = "LimitExceeded"
+    """Request limit exceeded."""
 
 
 class ErrorView(dict):
     """Error returned by Cybsi Cloud API."""
 
     @property
     def code(self) -> str:
@@ -261,20 +316,22 @@
     400: InvalidRequestError,
     401: UnauthorizedError,
     403: ForbiddenError,
     404: NotFoundError,
     409: ConflictError,
     412: ResourceModifiedError,
     413: RequestEntityTooLargeError,
+    416: RangeNotSatisfiableError,
     422: SemanticError,
+    429: TooManyRequestsError,
 }
 
 
 def _raise_cybsi_error(resp: httpx.Response) -> None:
     err_cls = _error_mapping.get(resp.status_code, None)
     if err_cls is not None:
-        raise err_cls(resp.json())
+        raise err_cls(resp)
 
     raise CybsiError(
         f"unexpected response status code: {resp.status_code}. "
         f"Request body: {resp.text}"
     )
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/base.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/base.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/connector.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 import httpx
 
 from cybsi.__version__ import __version__
 
 from ..api import Tag
 from ..error import CybsiError, _raise_cybsi_error
+from ..internal.multipart import apply_async_multipart_stream
 
 _BASIC_HEADERS = {
     "User-Agent": f"cybsi-cloud-client/v{__version__}",
     "X-Api-Version": "1",
 }
 
 _IF_MATCH_HEADER = "If-Match"
 
+apply_async_multipart_stream()
+
 
 class HTTPConnector:
     """Connector performing round trips to Cybsi Cloud."""
 
     def __init__(
         self,
         base_url: str,
@@ -77,14 +80,17 @@
         return self._do("PUT", path, json=json, **kwargs)
 
     def do_delete(
         self, path: str, params: Optional[dict] = None, **kwargs
     ) -> httpx.Response:
         return self._do("DELETE", path, params=params, **kwargs)
 
+    def do_head(self, path: str, **kwargs) -> httpx.Response:
+        return self._do("HEAD", path, **kwargs)
+
     def _do(self, method: str, path: str, stream=False, **kwargs):
         """Do HTTP request.
 
         Args:
             method: HTTP method i.e GET, POST, PUT.
             path: URL path.
             kwargs: Any kwargs supported by httpx.Request.
@@ -177,14 +183,17 @@
         return await self._do("PUT", path, json=json, **kwargs)
 
     async def do_delete(
         self, path: str, params: Optional[dict] = None, **kwargs
     ) -> httpx.Response:
         return await self._do("DELETE", path, params=params, **kwargs)
 
+    async def do_head(self, path: str, **kwargs) -> httpx.Response:
+        return await self._do("HEAD", path, **kwargs)
+
     async def _do(self, method: str, path: str, stream=False, **kwargs):
         """Do HTTP request.
 
         Args:
             method: HTTP method i.e GET, POST, PUT.
             path: URL path.
             kwargs: Any kwargs supported by httpx.Request.
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/internal/time.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/internal/time.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/__init__.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     CollectionCommonView,
     CollectionRegistrationView,
     CollectionView,
 )
 from .objects import (
     ObjectAPI,
     ObjectsAsyncAPI,
-    ObjectKeyType,
-    ObjectType,
-    ObjectView,
     ObjectKeyView,
+    ObjectView,
     ObjectChangeView,
+    ObjectKeyType,
+    ObjectType,
     ObjectOperation,
 )
 from .schemas import (
     SchemaAPI,
     SchemaAsyncAPI,
     SchemaView,
     SchemaCommonView,
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/api.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/collection.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/collection.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/objects.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import httpx
 from enum_tools import document_enum
 
 from ..enum import CybsiAPIEnum
 from ..internal import BaseAPI, BaseAsyncAPI, JsonObject, JsonObjectView
 from ..pagination import AsyncPage, Cursor, Page
 
+_PATH = "/iocean/collections/{}/objects"
+
 
 @document_enum
 class ObjectKeyType(CybsiAPIEnum):
     """Object key type."""
 
     MD5Hash = "MD5Hash"
     SHA1Hash = "SHA1Hash"
@@ -30,17 +32,14 @@
     File = "File"
     DomainName = "DomainName"
     URL = "URL"
     IPAddress = "IPAddress"
     IPNetwork = "IPNetwork"
 
 
-_PATH = "/iocean/collections/{}/objects"
-
-
 @document_enum
 class ObjectOperation(CybsiAPIEnum):
     """Object change operation."""
 
     Add = "Add"
     """Object was added to collection."""
     Remove = "Remove"
```

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/iocean/schemas.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/iocean/schemas.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/pagination.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/pagination.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/cybsi/cloud/view.py` & `cybsi_cloud_sdk-1.1.0/cybsi/cloud/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.0.8/pyproject.toml` & `cybsi_cloud_sdk-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybsi-cloud-sdk"
-version = "1.0.8"
+version = "1.1.0"
 description = "Cybsi Cloud development kit"
 authors = ["Cybsi Cloud developers"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "cybsi" },
 ]
@@ -32,15 +32,15 @@
 [tool.isort]
 profile = "black"
 extend_skip = ["__init__.py"]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "1.0.8"
+current = "1.1.0"
 
 regex = '''
   ^
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `cybsi_cloud_sdk-1.0.8/PKG-INFO` & `cybsi_cloud_sdk-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybsi-cloud-sdk
-Version: 1.0.8
+Version: 1.1.0
 Summary: Cybsi Cloud development kit
 License: Apache-2.0
 Author: Cybsi Cloud developers
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

