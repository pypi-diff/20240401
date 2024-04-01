# Comparing `tmp/armasec-1.3.0.tar.gz` & `tmp/armasec-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armasec-1.3.0.tar", max compression
+gzip compressed data, was "armasec-1.4.0.tar", max compression
```

## Comparing `armasec-1.3.0.tar` & `armasec-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1078 2024-01-22 20:16:25.613894 armasec-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     2646 2024-01-22 20:16:25.613894 armasec-1.3.0/README.md
--rw-r--r--   0        0        0      423 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/__init__.py
--rw-r--r--   0        0        0     4225 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/armasec.py
--rw-r--r--   0        0        0     1231 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/exceptions.py
--rw-r--r--   0        0        0     3823 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/openid_config_loader.py
--rw-r--r--   0        0        0        0 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/py.typed
--rw-r--r--   0        0        0     9554 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/pytest_extension.py
--rw-r--r--   0        0        0      232 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/schemas/__init__.py
--rw-r--r--   0        0        0     2060 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/schemas/armasec_config.py
--rw-r--r--   0        0        0     1305 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/schemas/jwks.py
--rw-r--r--   0        0        0      637 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/schemas/openid_config.py
--rw-r--r--   0        0        0     6181 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/token_decoder.py
--rw-r--r--   0        0        0     3691 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/token_manager.py
--rw-r--r--   0        0        0     1053 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/token_payload.py
--rw-r--r--   0        0        0     9760 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/token_security.py
--rw-r--r--   0        0        0     1104 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec/utilities.py
--rw-r--r--   0        0        0     9093 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/auth.py
--rw-r--r--   0        0        0     3050 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/cache.py
--rw-r--r--   0        0        0     8270 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/client.py
--rw-r--r--   0        0        0     2279 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/config.py
--rw-r--r--   0        0        0     1523 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/exceptions.py
--rw-r--r--   0        0        0      756 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/format.py
--rw-r--r--   0        0        0      194 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/logging.py
--rw-r--r--   0        0        0     6113 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/main.py
--rw-r--r--   0        0        0      643 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/schemas.py
--rw-r--r--   0        0        0     3057 2024-01-22 20:16:25.613894 armasec-1.3.0/armasec_cli/time_loop.py
--rw-r--r--   0        0        0     2649 2024-01-22 20:16:25.633895 armasec-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 armasec-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-01 20:26:59.433843 armasec-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2646 2024-04-01 20:26:59.433843 armasec-1.4.0/README.md
+-rw-r--r--   0        0        0      423 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/__init__.py
+-rw-r--r--   0        0        0     4776 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/armasec.py
+-rw-r--r--   0        0        0     1369 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/exceptions.py
+-rw-r--r--   0        0        0     3823 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/openid_config_loader.py
+-rw-r--r--   0        0        0      280 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pluggable/__init__.py
+-rw-r--r--   0        0        0     1237 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pluggable/hookspecs.py
+-rw-r--r--   0        0        0        0 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/py.typed
+-rw-r--r--   0        0        0     9554 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pytest_extension.py
+-rw-r--r--   0        0        0      232 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/armasec_config.py
+-rw-r--r--   0        0        0     1305 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/jwks.py
+-rw-r--r--   0        0        0      637 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/openid_config.py
+-rw-r--r--   0        0        0     6249 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_decoder.py
+-rw-r--r--   0        0        0     3616 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_manager.py
+-rw-r--r--   0        0        0     1165 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_payload.py
+-rw-r--r--   0        0        0    10884 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_security.py
+-rw-r--r--   0        0        0     1105 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/utilities.py
+-rw-r--r--   0        0        0     9089 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/auth.py
+-rw-r--r--   0        0        0     3050 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/cache.py
+-rw-r--r--   0        0        0     8270 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/client.py
+-rw-r--r--   0        0        0     2277 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/config.py
+-rw-r--r--   0        0        0     1521 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/exceptions.py
+-rw-r--r--   0        0        0      756 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/format.py
+-rw-r--r--   0        0        0      194 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/logging.py
+-rw-r--r--   0        0        0     6113 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/main.py
+-rw-r--r--   0        0        0      642 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/schemas.py
+-rw-r--r--   0        0        0     3057 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/time_loop.py
+-rw-r--r--   0        0        0     2663 2024-04-01 20:26:59.461843 armasec-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 armasec-1.4.0/PKG-INFO
```

### Comparing `armasec-1.3.0/LICENSE.md` & `armasec-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/README.md` & `armasec-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec/armasec.py` & `armasec-1.4.0/armasec/armasec.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,48 +53,69 @@
         self.debug_exceptions = debug_exceptions
 
     @lru_cache(maxsize=128)
     def lockdown(
         self,
         *scopes: str,
         permission_mode: PermissionMode = PermissionMode.ALL,
+        skip_plugins: bool = False,
     ) -> TokenSecurity:
         """
         Initialize an instance of TokenSecurity to lockdown a route. Uses memoization to minimize
         the number of TokenSecurity instances initialized. Applies supplied permission_mode when
         checking token permssions against TokenSecurity scopes.
 
         Args:
             scopes: A list of scopes needed to access the endpoint.
             permissions_mode: If "ALL", all scopes listed are required for access. If "SOME", only
                 one of the scopes listed are required for access.
+            skip_plugins: If True, do not evaluate plugin validators.
         """
         return TokenSecurity(
             domain_configs=self.domain_configs,
             scopes=scopes,
             permission_mode=permission_mode,
             debug_logger=self.debug_logger,
             debug_exceptions=self.debug_exceptions,
+            skip_plugins=skip_plugins,
         )
 
-    def lockdown_all(self, *scopes: str) -> TokenSecurity:
+    def lockdown_all(
+        self,
+        *scopes: str,
+        skip_plugins: bool = False,
+    ) -> TokenSecurity:
         """
         Initialize an instance of TokenSecurity to lockdown a route. Uses memoization to minimize
         the number of TokenSecurity instances initialized. Requires all the scopes in the
         TokenSecurity instance to be included in the token permissions. This is just a wrapper
         around `lockdown()` with default permission_mode and is only included for symmetry.
 
         Args:
             scopes: A list of the scopes needed to access the endpoint. All are required.
+            skip_plugins: If True, do not evaluate plugin validators.
         """
-        return self.lockdown(*scopes, permission_mode=PermissionMode.ALL)
+        return self.lockdown(
+            *scopes,
+            permission_mode=PermissionMode.ALL,
+            skip_plugins=skip_plugins,
+        )
 
-    def lockdown_some(self, *scopes: str) -> TokenSecurity:
+    def lockdown_some(
+        self,
+        *scopes: str,
+        skip_plugins: bool = False,
+    ) -> TokenSecurity:
         """
         Initialize an instance of TokenSecurity to lockdown a route. Uses memoization to minimize
         the number of TokenSecurity instances initialized. Requires at least one permission in the
         token to match a scope attached to the TokenSecurity instance.
 
         Args:
             scopes: A list of the scopes needed to access the endpoint. Only one is required.
+            skip_plugins: If True, do not evaluate plugin validators.
         """
-        return self.lockdown(*scopes, permission_mode=PermissionMode.SOME)
+        return self.lockdown(
+            *scopes,
+            permission_mode=PermissionMode.SOME,
+            skip_plugins=skip_plugins,
+        )
```

### Comparing `armasec-1.3.0/armasec/exceptions.py` & `armasec-1.4.0/armasec/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,40 +7,44 @@
     A custom exception class used for checking conditions and handling other exceptions.
 
     Attributes:
         status_code: The HTTP status code indicated by the error. Set to 400.
     """
 
     status_code: int = starlette.status.HTTP_400_BAD_REQUEST
+    detail: str = "Bad request"
 
 
 class AuthenticationError(ArmasecError):
     """
     Indicates a failure to authenticate and decode jwt.
 
     Attributes:
         status_code: The HTTP status code indicated by the error. Set to 401.
     """
 
     status_code: int = starlette.status.HTTP_401_UNAUTHORIZED
+    detail: str = "Not authenticated"
 
 
 class AuthorizationError(ArmasecError):
     """
     Indicates that the provided claims don't match the claims required for a protected endpoint.
 
     Attributes:
         status_code: The HTTP status code indicated by the error. Set to 403.
     """
 
     status_code: int = starlette.status.HTTP_403_FORBIDDEN
+    detail: str = "Not authorized"
 
 
 class PayloadMappingError(ArmasecError):
     """
     Indicates that the configured payload_claim_mapping did not match a path in the token.
 
     Attributes:
         status_code: The HTTP status code indicated by the error. Set to 500.
     """
 
     status_code: int = starlette.status.HTTP_500_INTERNAL_SERVER_ERROR
+    detail: str = "Server error"
```

### Comparing `armasec-1.3.0/armasec/openid_config_loader.py` & `armasec-1.4.0/armasec/openid_config_loader.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec/pytest_extension.py` & `armasec-1.4.0/armasec/pytest_extension.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec/schemas/armasec_config.py` & `armasec-1.4.0/armasec/schemas/armasec_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,27 @@
         description=snick.unwrap(
             """
             If falsey, use ``http`` when pulling openid config from the OIDC server
             instead of ``https`` (the default).
             """,
         ),
     )
-    match_keys: Dict[
-        str, Union[str, List[Any], Dict[Any, Any], Set[Any], bool, int, float]
-    ] = Field(
-        dict(),
-        description=snick.unwrap(
-            """
+    match_keys: Dict[str, Union[str, List[Any], Dict[Any, Any], Set[Any], bool, int, float]] = (
+        Field(
+            dict(),
+            description=snick.unwrap(
+                """
             Dictionary of key-value pair to match in the token when decoding it. It will
             raise 403 in case the input key-value pair cannot be found in the token.
             """
-        ),
+            ),
+        )
     )
     payload_claim_mapping: Optional[Dict[str, Any]] = Field(
         None,
         description=snick.unwrap(
             """
             Optional mappings that are applied to map claims to top-level properties of
             TokenPayload. See docs for `TokenDecoder` for more info.
             """
-        )
+        ),
     )
```

### Comparing `armasec-1.3.0/armasec/schemas/jwks.py` & `armasec-1.4.0/armasec/schemas/jwks.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec/schemas/openid_config.py` & `armasec-1.4.0/armasec/schemas/openid_config.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec/token_decoder.py` & `armasec-1.4.0/armasec/token_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module provides an abstract base class for algorithmic token decoders
 """
+
 from __future__ import annotations
 
 from functools import partial
 from typing import Callable
 
 import jmespath
 import buzz
@@ -44,15 +45,15 @@
                                      decode method. For example, one can ignore token expiration by
                                      setting this to `{ "verify_exp": False }`
             payload_claim_mapping:   Optional mappings that are applied to map claims to top-level
                                      attribute of TokenPayload using a dict format of:
 
                                      ```
                                      {
-                                         "top_level+attribute": "decoded.token.JMESPath"
+                                         "top_level_attribute": "decoded.token.JMESPath"
                                      }
                                      ```
                                      The values _must_ be a valid JMESPath.
 
                                      Consider this example:
 
                                      ```
@@ -126,21 +127,24 @@
             )
             self.debug_logger(f"Raw payload dictionary is {payload_dict}")
 
         with PayloadMappingError.handle_errors(
             "Failed to map decoded token to payload",
             do_except=partial(log_error, self.debug_logger),
         ):
-            for (payload_key, token_jmespath) in self.payload_claim_mapping.items():
+            for payload_key, token_jmespath in self.payload_claim_mapping.items():
                 mapped_value = jmespath.search(token_jmespath, payload_dict)
                 buzz.require_condition(
                     mapped_value is not None,
                     f"No matching values found for claim mapping {token_jmespath} -> {payload_key}",
                     raise_exc_class=KeyError,
                 )
                 payload_dict[payload_key] = mapped_value
             self.debug_logger(f"Mapped payload dictionary is {payload_dict}")
 
             self.debug_logger("Attempting to convert to TokenPayload")
-            token_payload = TokenPayload(**payload_dict)
+            token_payload = TokenPayload(
+                **payload_dict,
+                original_token=token,
+            )
             self.debug_logger(f"Built token_payload as {token_payload}")
             return token_payload
```

### Comparing `armasec-1.3.0/armasec/token_manager.py` & `armasec-1.4.0/armasec/token_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
             auth_str,
             f"Could not find auth header at {self.header_key}",
         )
         auth_str = str(auth_str)
 
         self.debug_logger("Attempting to get authorization scheme")
         (scheme, token) = get_authorization_scheme_param(auth_str)
-        self.debug_logger(f"Auth scheme is {scheme} and token is {token}")
         AuthenticationError.require_condition(
             scheme and token,
             f"Could not extract scheme ('{self.auth_scheme}') from token '{token}'",
         )
         AuthenticationError.require_condition(
             scheme.lower() == self.auth_scheme,
             f"Invalid auth scheme '{scheme}': expected '{self.auth_scheme}'",
```

### Comparing `armasec-1.3.0/armasec/token_security.py` & `armasec-1.4.0/armasec/token_security.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from fastapi.security.api_key import APIKeyBase
 from pydantic import BaseModel
 from snick import unwrap
 from starlette.requests import Request
 
 from armasec.exceptions import AuthenticationError, AuthorizationError
 from armasec.openid_config_loader import OpenidConfigLoader
+from armasec.pluggable import plugin_manager
 from armasec.schemas import DomainConfig
 from armasec.token_decoder import TokenDecoder
 from armasec.token_manager import TokenManager
 from armasec.token_payload import TokenPayload
 from armasec.utilities import noop
 
 
@@ -63,33 +64,36 @@
     def __init__(
         self,
         domain_configs: List[DomainConfig],
         scopes: Optional[Iterable[str]] = None,
         permission_mode: PermissionMode = PermissionMode.ALL,
         debug_logger: Optional[Callable[..., None]] = None,
         debug_exceptions: bool = False,
+        skip_plugins: bool = False,
     ):
         """
         Initializes the TokenSecurity instance.
 
         Args:
             domain_configs:   List of domain configuration to authenticate the tokens against.
             scopes:           Optional permissions scopes that should be checked
             permission_mode:  The PermissionMode to apply in the protected route.
             debug_logger:     A callable, that if provided, will allow debug logging. Should be
                               passed as a logger method like `logger.debug`
             debug_exceptions: If True, raise original exceptions. Should only be used in a testing
                               or debugging context.
+            skip_plugins:     If True, do not evaluate plugin validators.
         """
         self.domain_configs = domain_configs
         self.scopes = scopes
         self.permission_mode = permission_mode
 
         self.debug_logger = debug_logger if debug_logger else noop
         self.debug_exceptions = debug_exceptions
+        self.skip_plugins = skip_plugins
 
         # Settings needed for FastAPI's APIKeyBase
         self.model: APIKey = APIKey(
             **{"in": APIKeyIn.header},  # type: ignore[arg-type]
             name=TokenManager.header_key,
             description=self.__class__.__doc__,
         )
@@ -118,66 +122,84 @@
             )
         except Exception as err:
             if self.debug_exceptions:
                 raise err
             else:
                 raise HTTPException(
                     status_code=getattr(err, "status_code", status.HTTP_401_UNAUTHORIZED),
-                    detail="Not authenticated",
+                    detail=getattr(err, "detail", "Not authenticated"),
                     headers={"WWW-Authenticate": "Bearer"},
                 )
 
-        if not self.scopes:
-            return token_payload
+        if self.scopes:
+            token_permissions = set(token_payload.permissions)
+            my_permissions = set(self.scopes)
 
-        token_permissions = set(token_payload.permissions)
-        my_permissions = set(self.scopes)
-
-        self.debug_logger(
-            unwrap(
-                f"""
-                Checking my permissions {my_permissions} against token_permissions
-                {token_permissions} using PermissionMode {self.permission_mode}
-                """
-            )
-        )
-        try:
-            if self.permission_mode == PermissionMode.ALL:
-                message = unwrap(
+            self.debug_logger(
+                unwrap(
                     f"""
-                    Token permissions {token_permissions} missing some required permissions
-                    {my_permissions - token_permissions}
+                    Checking my permissions {my_permissions} against token_permissions
+                    {token_permissions} using PermissionMode {self.permission_mode}
                     """
                 )
-                self.debug_logger(message)
-                AuthorizationError.require_condition(
-                    my_permissions - token_permissions == set(),
-                    message,
-                )
-            elif self.permission_mode == PermissionMode.SOME:
-                message = unwrap(
-                    f"""
-                    Token permissions {token_permissions} missing at least one required permissions
-                    {my_permissions}
-                    """
-                )
-                self.debug_logger(message)
-                AuthorizationError.require_condition(token_permissions & my_permissions, message)
-            else:
-                raise AuthorizationError(f"Unknown permission_mode: {self.permission_mode}")
-
-        except Exception as err:
-            if self.debug_exceptions:
-                raise err
-            else:
-                raise HTTPException(
-                    status_code=getattr(err, "status_code", status.HTTP_403_FORBIDDEN),
-                    detail="Not authorized",
-                    headers={"WWW-Authenticate": "Bearer"},
+            )
+            try:
+                if self.permission_mode == PermissionMode.ALL:
+                    message = unwrap(
+                        f"""
+                        Token permissions {token_permissions} missing some required permissions
+                        {my_permissions - token_permissions}
+                        """
+                    )
+                    AuthorizationError.require_condition(
+                        my_permissions - token_permissions == set(),
+                        message,
+                    )
+                elif self.permission_mode == PermissionMode.SOME:
+                    message = unwrap(
+                        f"""
+                        Token permissions {token_permissions} missing at least
+                        one required permissions
+                        {my_permissions}
+                        """
+                    )
+                    AuthorizationError.require_condition(
+                        token_permissions & my_permissions,
+                        message,
+                    )
+                else:
+                    raise AuthorizationError(f"Unknown permission_mode: {self.permission_mode}")
+
+            except Exception as err:
+                if self.debug_exceptions:
+                    raise err
+                else:
+                    raise HTTPException(
+                        status_code=getattr(err, "status_code", status.HTTP_403_FORBIDDEN),
+                        detail=getattr(err, "detail", "Not authorized"),
+                        headers={"WWW-Authenticate": "Bearer"},
+                    )
+
+        if not self.skip_plugins:
+            self.debug_logger("Applying plugin checks")
+            try:
+                plugin_manager.hook.armasec_plugin_check(
+                    request=request,
+                    token_payload=token_payload,
+                    debug_logger=self.debug_logger,
                 )
+            except Exception as err:
+                if self.debug_exceptions:
+                    raise err
+                else:
+                    raise HTTPException(
+                        status_code=getattr(err, "status_code", status.HTTP_403_FORBIDDEN),
+                        detail=getattr(err, "detail", "Not authorized"),
+                        headers={"WWW-Authenticate": "Bearer"},
+                    )
 
         return token_payload
 
     def _load_all_managers(self) -> None:
         if len(self.managers) == 0:
             for domain_config in self.domain_configs:
                 try:
```

### Comparing `armasec-1.3.0/armasec/utilities.py` & `armasec-1.4.0/armasec/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides some utility functions.
 """
+
 from traceback import format_tb
 from typing import Callable
 
 from buzz import DoExceptParams
 from snick import dedent
```

### Comparing `armasec-1.3.0/armasec_cli/auth.py` & `armasec-1.4.0/armasec_cli/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from armasec_cli.config import OidcProvider
 from armasec_cli.schemas import Persona, CliContext
 from armasec_cli.format import terminal_message
 from armasec_cli.time_loop import TimeLoop
 
 
 def extract_persona(token_set: TokenSet | None = None):
-
     if token_set is None:
         token_set = load_tokens_from_cache()
 
     try:
         identity_data = validate_token_and_extract_identity(token_set)
     except ExpiredSignatureError:
         Abort.require_condition(
@@ -67,15 +66,15 @@
 
     with Abort.handle_errors(
         """
         There was an unknown error while validating the access token.
 
         Please try logging in again.
         """,
-        ignore_exc_class=ExpiredSignatureError,     # Will be handled in calling context
+        ignore_exc_class=ExpiredSignatureError,  # Will be handled in calling context
         raise_kwargs=dict(
             subject="Invalid access token",
             log_message="Unknown error while validating access access token",
         ),
     ):
         token_data = jwt.decode(
             token_set.access_token,
```

### Comparing `armasec-1.3.0/armasec_cli/cache.py` & `armasec-1.4.0/armasec_cli/cache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from armasec_cli.schemas import TokenSet
 from armasec_cli.exceptions import Abort
 from armasec_cli.config import cache_dir
 
 
 def init_cache(func):
-
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             cache_dir.mkdir(exist_ok=True, parents=True)
             token_dir = cache_dir / "token"
             token_dir.mkdir(exist_ok=True)
             info_file = cache_dir / "info.txt"
@@ -27,14 +26,15 @@
 
                 Please check your home directory permissions and try again.
                 """,
                 subject="Non-writable cache dir",
                 log_message="Non-writable cache dir",
             )
         return func(*args, **kwargs)
+
     return wrapper
 
 
 def _get_token_paths() -> tuple[Path, Path]:
     token_dir = cache_dir / "token"
     access_token_path: Path = token_dir / "access.token"
     refresh_token_path: Path = token_dir / "refresh.token"
```

### Comparing `armasec-1.3.0/armasec_cli/client.py` & `armasec-1.4.0/armasec_cli/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     base_url = f"{protocol}://{settings.oidc_domain}"
     logger.debug(f"Creating client with base URL {base_url}")
     return httpx.Client(
         base_url=base_url,
         headers={"content-type": "application/x-www-form-urlencoded"},
     )
 
-def attach_client(func):
 
+def attach_client(func):
     @wraps(func)
     def wrapper(ctx: typer.Context, *args, **kwargs):
-
         if ctx.obj.settings is None:
             raise Abort(
                 """
                 Cannot attach client before settings!
 
                 Check the order of the decorators and make sure settings are attached
                 first.
@@ -39,14 +38,15 @@
                 subject="Attaching out of order",
                 log_message="Attaching out of order",
             )
 
         logger.debug("Binding client to CLI context")
         ctx.obj.client = build_client(ctx.obj.settings)
         return func(ctx, *args, **kwargs)
+
     return wrapper
 
 
 def _deserialize_request_model(
     request_model: pydantic.BaseModel,
     request_kwargs: dict[str, Any],
     abort_message: str,
```

### Comparing `armasec-1.3.0/armasec_cli/config.py` & `armasec-1.4.0/armasec_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 class OidcProvider(AutoNameEnum):
     AUTH0 = auto()
     KEYCLOAK = auto()
 
 
-
 class Settings(BaseModel):
     oidc_domain: str
     oidc_audience: str
     oidc_client_id: str
     oidc_use_https: bool = True
     oidc_max_poll_time: int = 5 * 60  # 5 minutes
     oidc_provider: OidcProvider = OidcProvider.KEYCLOAK
@@ -44,18 +43,16 @@
             ),
             subject="Configuration Error",
             log_message="Configuration error",
         )
 
 
 def attach_settings(func):
-
     @wraps(func)
     def wrapper(ctx: typer.Context, *args, **kwargs):
-
         try:
             logger.debug(f"Loading settings from {settings_path}")
             settings_values = json.loads(settings_path.read_text())
         except FileNotFoundError:
             raise Abort(
                 f"""
                 No settings file found at {settings_path}!
@@ -64,14 +61,15 @@
                 """,
                 subject="Settings file missing!",
                 log_message="Settings file missing!",
             )
         logger.debug("Binding settings to CLI context")
         ctx.obj.settings = init_settings(**settings_values)
         return func(ctx, *args, **kwargs)
+
     return wrapper
 
 
 def dump_settings(settings: Settings):
     logger.debug(f"Saving settings to {settings_path}")
     settings_values = json.dumps(settings.dict())
     settings_path.write_text(settings_values)
```

### Comparing `armasec-1.3.0/armasec_cli/exceptions.py` & `armasec-1.4.0/armasec_cli/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import typer
 from loguru import logger
 from rich import traceback
 from rich.console import Console
 from rich.panel import Panel
 
 
-
 # Enables prettified traceback printing via rich
 traceback.install()
 
 
 class ArmasecCliError(buzz.Buzz):
     pass
 
@@ -33,15 +32,14 @@
         self.log_message = log_message
         self.warn_only = warn_only
         (_, self.original_error, __) = exc_info()
         super().__init__(message, *args, **kwargs)
 
 
 def handle_abort(func):
-
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             func(*args, **kwargs)
         except Abort as err:
             if not err.warn_only:
                 if err.log_message is not None:
```

### Comparing `armasec-1.3.0/armasec_cli/format.py` & `armasec-1.4.0/armasec_cli/format.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/armasec_cli/main.py` & `armasec-1.4.0/armasec_cli/main.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
         )
         raise typer.Exit()
 
     init_logs(verbose=verbose)
     ctx.obj = CliContext()
 
 
-
 @app.command()
 @handle_abort
 @init_cache
 @attach_settings
 @attach_client
 def login(ctx: typer.Context):
     token_set: TokenSet = fetch_auth_tokens(ctx.obj)
     persona: Persona = extract_persona(token_set)
     terminal_message(
         f"User was logged in with email '{persona.identity_data.email}'",
         subject="Logged in!",
     )
 
+
 @app.command()
 @handle_abort
 @init_cache
 def logout():
     """
     Logs out of the jobbergate-cli. Clears the saved user credentials.
     """
```

### Comparing `armasec-1.3.0/armasec_cli/schemas.py` & `armasec-1.4.0/armasec_cli/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TokenSet(BaseModel):
     access_token: str
     refresh_token: Optional[str] = None
 
 
 class IdentityData(BaseModel):
     client_id: str
-    email: Optional[str] =  None
+    email: Optional[str] = None
 
 
 class Persona(BaseModel):
     token_set: TokenSet
     identity_data: IdentityData
```

### Comparing `armasec-1.3.0/armasec_cli/time_loop.py` & `armasec-1.4.0/armasec_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `armasec-1.3.0/pyproject.toml` & `armasec-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "armasec"
-version = "1.3.0"
+version = "1.4.0"
 description = "Injectable FastAPI auth via OIDC"
 authors = ["Omnivector Engineering Team <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/omnivector-solutions/armasec"
 repository = "https://github.com/omnivector-solutions/armasec"
 documentation = "https://omnivector-solutions.github.io/armasec"
@@ -36,14 +36,15 @@
 # These are needed for the "cli" extra
 typer = {version = "^0.9.0", optional = true}
 loguru = {version = "^0.5.3", optional = true}
 rich = {version = "^13.5.2", optional = true}
 pendulum = {version = "^3.0.0", optional = true}
 pyperclip = {version = "^1.8.2", optional = true}
 jmespath = "^1.0.1"
+pluggy = "^1.4.0"
 
 [tool.poetry.extras]
 cli = ["typer", "loguru", "rich", "pendulum", "pyperclip"]
 
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=7,<9"
@@ -59,15 +60,15 @@
 Sphinx = "^4"
 grip = "^4.6.1"
 mkdocs-material = "^9.1.21"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 pygments = "^2.16.1"
 plummet = {extras = ["time-machine"], version = "^1.2.1"}
 pytest-mock = "^3.11.1"
-ruff = "^0.0.286"
+ruff = "^0.3"
 types-jmespath = "^1.0.2.7"
 
 
 [tool.poetry.scripts]
 armasec = {callable = "armasec_cli.main:app", extras = ["cli"]}
 
 [tool.poetry.plugins.pytest11]
```

### Comparing `armasec-1.3.0/PKG-INFO` & `armasec-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armasec
-Version: 1.3.0
+Version: 1.4.0
 Summary: Injectable FastAPI auth via OIDC
 Home-page: https://github.com/omnivector-solutions/armasec
 License: MIT
 Author: Omnivector Engineering Team
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Provides-Extra: cli
 Requires-Dist: auto-name-enum (>=2,<3)
 Requires-Dist: fastapi (>=0.68)
 Requires-Dist: httpx (>=0,<1)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0) ; extra == "cli"
 Requires-Dist: pendulum (>=3.0.0,<4.0.0) ; extra == "cli"
+Requires-Dist: pluggy (>=1.4.0,<2.0.0)
 Requires-Dist: py-buzz (>=4.1,<5.0)
 Requires-Dist: pydantic (<2.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0) ; extra == "cli"
 Requires-Dist: pytest (>=6,<8)
 Requires-Dist: python-jose[cryptography] (>=3.2,<4.0)
 Requires-Dist: respx (>=0,<1)
 Requires-Dist: rich (>=13.5.2,<14.0.0) ; extra == "cli"
```

