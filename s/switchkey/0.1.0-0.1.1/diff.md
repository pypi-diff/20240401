# Comparing `tmp/switchkey-0.1.0.tar.gz` & `tmp/switchkey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchkey-0.1.0.tar", max compression
+gzip compressed data, was "switchkey-0.1.1.tar", max compression
```

## Comparing `switchkey-0.1.0.tar` & `switchkey-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,19 @@
--rw-r--r--   0        0        0     3539 2024-03-30 14:45:21.749927 switchkey-0.1.0/README.md
--rw-r--r--   0        0        0      890 2024-03-30 14:47:15.406381 switchkey-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3214 2024-03-30 14:43:04.345522 switchkey-0.1.0/switchkey/api/request.py
--rw-r--r--   0        0        0     2282 2024-03-30 14:43:04.345522 switchkey-0.1.0/switchkey/api/response.py
--rw-r--r--   0        0        0     2046 2024-03-30 14:43:04.345522 switchkey-0.1.0/switchkey/api/routes.py
--rw-r--r--   0        0        0     8842 2024-03-30 14:43:04.345522 switchkey-0.1.0/switchkey/api/types.py
--rw-r--r--   0        0        0     7249 2024-03-30 14:43:04.349522 switchkey-0.1.0/switchkey/core/base.py
--rw-r--r--   0        0        0      214 2024-03-30 14:43:04.349522 switchkey-0.1.0/switchkey/core/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-30 14:42:23.785438 switchkey-0.1.0/switchkey/tests/__init__.py
--rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 switchkey-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3539 2024-03-30 14:45:21.749927 switchkey-0.1.1/README.md
+-rw-r--r--   0        0        0      822 2024-04-01 10:17:38.811202 switchkey-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3064 2024-04-01 10:07:13.365416 switchkey-0.1.1/switchkey/api/models/auth.py
+-rw-r--r--   0        0        0     5189 2024-03-31 23:48:02.093337 switchkey-0.1.1/switchkey/api/models/organization.py
+-rw-r--r--   0        0        0     3854 2024-03-31 23:47:08.153871 switchkey-0.1.1/switchkey/api/models/project.py
+-rw-r--r--   0        0        0      358 2024-03-31 23:46:57.232358 switchkey-0.1.1/switchkey/api/models/user.py
+-rw-r--r--   0        0        0     3625 2024-04-01 00:36:04.440726 switchkey-0.1.1/switchkey/api/request/request.py
+-rw-r--r--   0        0        0     1668 2024-04-01 00:37:34.082980 switchkey-0.1.1/switchkey/api/request/types.py
+-rw-r--r--   0        0        0     2659 2024-04-01 00:35:13.188508 switchkey-0.1.1/switchkey/api/response/response.py
+-rw-r--r--   0        0        0     5197 2024-04-01 01:42:13.528131 switchkey-0.1.1/switchkey/api/response/types.py
+-rw-r--r--   0        0        0     2051 2024-03-31 09:46:15.458637 switchkey-0.1.1/switchkey/api/routes.py
+-rw-r--r--   0        0        0     6495 2024-03-31 23:47:09.662080 switchkey-0.1.1/switchkey/api/types.py
+-rw-r--r--   0        0        0     5930 2024-04-01 10:13:56.877930 switchkey-0.1.1/switchkey/core/base.py
+-rw-r--r--   0        0        0      925 2024-04-01 10:04:08.230292 switchkey-0.1.1/switchkey/core/exceptions.py
+-rw-r--r--   0        0        0     4215 2024-04-01 01:25:39.056628 switchkey-0.1.1/switchkey/utils/config.py
+-rw-r--r--   0        0        0      703 2024-03-31 20:45:26.629894 switchkey-0.1.1/switchkey/utils/decorators.py
+-rw-r--r--   0        0        0      569 2024-04-01 01:02:43.547372 switchkey-0.1.1/switchkey/utils/logger.py
+-rw-r--r--   0        0        0     3529 2024-04-01 01:45:48.099007 switchkey-0.1.1/switchkey/utils/parser.py
+-rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 switchkey-0.1.1/PKG-INFO
```

### Comparing `switchkey-0.1.0/README.md` & `switchkey-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `switchkey-0.1.0/pyproject.toml` & `switchkey-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "switchkey"
-version = "0.1.0"
-description = "The SwitchKey Python client is a versatile tool for interacting with the SwitchKey feature management platform in Python applications. With this client, developers can easily integrate feature flags and toggle management capabilities into their Python projects. The client provides methods for connecting to SwitchKey environments, accessing user data, retrieving feature values, setting feature flags, and more. It simplifies the process of incorporating feature management functionality, enabling developers to efficiently control feature rollout and experimentation in their applications."
+version = "0.1.1"
+description = "The SwitchKey Python client enables seamless integration with the SwitchKey feature management platform in Python applications. Developers can effortlessly incorporate feature flags and toggle management into their projects, accessing user data, retrieving feature values, and setting feature flags with ease. This client streamlines the process of implementing feature management functionality, empowering developers to efficiently control feature rollout and experimentation in their applications."
 authors = ["Mahmoud Emad <mahmmoud.hassanein@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
+configparser = "^6.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `switchkey-0.1.0/switchkey/api/request.py` & `switchkey-0.1.1/switchkey/api/request/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Any, Dict
 import requests
-from switchkey.api.response import SwitchKeyResponse
+from switchkey.api.response.response import SwitchKeyResponse
 from enum import Enum
 
 
 class SwitchKeyRequestMethod(Enum):
     POST = "POST"
     GET = "GET"
     PUT = "PUT"
@@ -15,45 +15,52 @@
 class SwitchKeyRequest:
     """
     Make an HTTP request to the specified URL using the provided method.
 
     Args:
         url (str): The URL to make the request to.
         method (SwitchKeyRequestMethod): The HTTP method to use for the request.
+        headers (Dict[str, str]): Additional headers for the request.
 
     Returns:
         SwitchKeyResponse: An object containing the response from the request.
 
     Raises:
         ValueError: If an invalid method is provided.
     """
 
     @staticmethod
     def call(
         url: str,
         method: SwitchKeyRequestMethod,
-        data: Dict[str, Any] = {}
+        data: Dict[str, Any] = {},
+        token: str | None = None,
     ) -> SwitchKeyResponse:
         try:
+            headers = {}
+            if token:
+                headers["Authorization"] = f"Bearer {token}"
+
             if method == SwitchKeyRequestMethod.GET:
                 response = requests.get(url)
             elif method == SwitchKeyRequestMethod.POST:
-                response = requests.post(url, json=data)
+                response = requests.post(url, json=data, headers=headers)
             elif method == SwitchKeyRequestMethod.PUT:
-                response = requests.put(url, json=data)
+                response = requests.put(url, json=data, headers=headers)
             elif method == SwitchKeyRequestMethod.DELETE:
-                response = requests.delete(url)
+                response = requests.delete(url, headers=headers)
             else:
                 raise ValueError("Invalid method provided.")
 
             response_content = response.content.decode()
-            
+
             # Check if response content is not valid JSON.
             if response_content.startswith("<!DOCTYPE html>"):
-               return SwitchKeyResponse(
+                print("response_content", response_content)
+                return SwitchKeyResponse(
                     status_code=response.status_code,
                     error_message="Response content is not valid json.",
                 )
 
             # Check if response content is empty
             if not response_content.strip():
                 return SwitchKeyResponse(
@@ -70,17 +77,21 @@
                     data=response_content.get("results"),
                 )
             elif response.status_code >= 400:
                 if response_content.get("detail") is None:
                     error_message = response_content.get("message")
                 else:
                     error_message = response_content.get("detail")
+
+                error = response_content.get("error")
+
                 return SwitchKeyResponse(
                     status_code=response.status_code,
                     error_message=error_message,
+                    error=error
                 )
             else:
                 return SwitchKeyResponse(
                     status_code=response.status_code,
                     error_message=response_content.get("detail"),
                 )
         except requests.exceptions.RequestException as e:
```

### Comparing `switchkey-0.1.0/switchkey/api/response.py` & `switchkey-0.1.1/switchkey/api/response/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,48 @@
+from typing import Any, Dict, List
+
+
 class SwitchKeyResponse:
     def __init__(
         self,
         status_code: int,
         data=None,
         error_message: str | None = None,
         message: str | None = None,
+        error: List[Dict[str, Any]] = None 
     ):
         """
         Initialize a SwitchKeyResponse object.
 
         Args:
             status_code (int): The HTTP status code of the response.
             data (Any, optional): The data returned in the response. Defaults to None.
             error_message (str | None, optional): The error message, if any. Defaults to None.
             message (str | None, optional): Additional message associated with the response. Defaults to None.
         """
         self.status_code = status_code
         self.data = data
         self.error_message = error_message
         self.message = message
+        self.error = error
 
     def __repr__(self):
         """
         Return a string representation of the SwitchKeyResponse object.
 
         Returns:
             str: String representation of the SwitchKeyResponse object.
         """
         is_error = self.error_message is None
         self.message = self.message if self.message is not None else None
         self.data = self.data if self.data is not None else None
         self.error_message = self.error_message if self.error_message is not None else None
+        self.error = self.error if self.error is not None else None
 
-        return f"SwitchKeyResponse(status_code={self.status_code}, data={self.data}, message={self.message}, error={is_error}, error_message={self.error_message})"
+        return f"SwitchKeyResponse(status_code={self.status_code}, data={self.data}, message={self.message}, is_error={is_error}, error_message={self.error_message}, error={self.error})"
 
     def get_error_message(self):
         """
         Get the error message associated with the response.
 
         Returns:
             str | None: Error message if present, otherwise None.
@@ -65,7 +71,16 @@
         """
         Get the HTTP status code of the response.
 
         Returns:
             int: HTTP status code.
         """
         return self.status_code
+
+    def get_error(self):
+        """
+        Get the HTTP error of the response.
+
+        Returns:
+            Dict[str, Any]: HTTP error.
+        """
+        return self.error
```

### Comparing `switchkey-0.1.0/switchkey/api/routes.py` & `switchkey-0.1.1/switchkey/api/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     SIGNUP = "http://127.0.0.1:8000/api/auth/signup/"
     LOGIN = "http://127.0.0.1:8000/api/auth/login/"
     USERS = "http://127.0.0.1:8000/api/auth/users/"
     
     # Endpoints with parameters
     ORGANIZATIONS_ID = "http://127.0.0.1:8000/api/organizations/{}/"
     ENVIRONMENTS_KEY = "http://127.0.0.1:8000/api/environments/key/{}/"
-    ENVIRONMENTS_SET = "http://127.0.0.1:8000/api/environments/key/{}/set/?user_id={}"
+    ENVIRONMENTS_SET = "http://127.0.0.1:8000/api/environments/key/{}/user/set/?user_id={}"
     ENVIRONMENTS_ID = "http://127.0.0.1:8000/api/environments/{}/"
     PROJECTS_ID = "http://127.0.0.1:8000/api/projects/{}/"
     GROUPS_ID = "http://127.0.0.1:8000/api/groups/{}/"
     USERS_ID = "http://127.0.0.1:8000/api/auth/users/{}/"
 
 class SwitchKeyRoutes:
     """Class to manage API routes."""
```

### Comparing `switchkey-0.1.0/switchkey/core/base.py` & `switchkey-0.1.1/switchkey/core/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from typing import Any, Dict, List
 from uuid import UUID
+from switchkey.api.models.auth import SwitchKeyAuth
+from switchkey.api.models.organization import SwitchKeyOrganization
+from switchkey.api.models.project import SwitchKeyProject
 from switchkey.api.types import (
     SwitchKeyEnvironmentType,
-    SwitchKeyProjectType,
-    SwitchKeyOrganizationType,
-    SwitchKeyUserType,
+    # SwitchKeyProjectType,
+    # SwitchKeyOrganizationResponseType,
+    # SwitchKeyUserType,
     SwitchKeyProjectUserType,
 )
-from switchkey.api.request import SwitchKeyRequest, SwitchKeyRequestMethod
-from switchkey.core.exceptions import FeatureNotEnabled as FeatureNotEnabledError
+from switchkey.api.request.request import SwitchKeyRequest, SwitchKeyRequestMethod
+from switchkey.core.exceptions import AuthenticationError, FeatureNotEnabled as FeatureNotEnabledError
 from switchkey.api.routes import SwitchKeyRoutes, EndPoints
+from switchkey.utils.config import SwitchKeyConfig
+from switchkey.utils.logger import SwitchKeyLogger
 
 
 class SwitchKeyBase(type):
     """
     Metaclass for the SwitchKey class hierarchy.
     """
 
@@ -32,177 +37,120 @@
         environment (SwitchKeyEnvironmentType): Environment object.
 
     Methods:
         connect() -> None: Connect to the SwitchKey environment.
         __parse_device(device_data: Dict[str, Any]) -> None: Parse device data.
         __parse_project_user(user_data: Dict[str, Any]) -> SwitchKeyProjectUserType: Parse project user data.
         __parse_user(user_data: Dict[str, Any]) -> SwitchKeyUserType | List[SwitchKeyUserType]: Parse user data.
-        __parse_organization(organization_data: Dict[str, Any]) -> SwitchKeyOrganizationType: Parse organization data.
+        __parse_organization(organization_data: Dict[str, Any]) -> SwitchKeyOrganizationResponseType: Parse organization data.
         __parse_project(project_data: Dict[str, Any]) -> SwitchKeyProjectType: Parse project data.
         __parse_environment() -> SwitchKeyEnvironmentType: Parse environment data.
     """
 
-    def __init__(self, environment_key: UUID) -> None:
+    def __init__(self, api_token: str | None = None) -> None:
         """
         Initialize the SwitchKey instance.
 
         Args:
-            environment_key (uuid): The key of the environment.
+            api_token (Bearer Token): User token required only if you are going to make create/update/delete requests.
         """
+        self.logger = SwitchKeyLogger.get_logger()
+        self.auth = SwitchKeyAuth()
 
-        self.FeatureNotEnabled = FeatureNotEnabledError
-        self.environment_key = environment_key
-        self.features = {}
-        self.__routes = SwitchKeyRoutes()
-        self.environment_data = None
-        self.environment = None
-    
-    def connect(self) -> None:
-        """
-        Connect to the SwitchKey environment.
-        """
-
-        environment = SwitchKeyRequest.call(
-            self.__routes.get_route(EndPoints.ENVIRONMENTS_KEY, self.environment_key),
-            SwitchKeyRequestMethod.GET,
-        )
-
-        if environment.error_message is not None:
-            raise ConnectionError(environment.error_message)
-
-        self.environment_data = environment.data
-        self.environment = self.__parse_environment()
-
-    def __parse_device(self, device_data: Dict[str, Any]) -> None:
-        """
-        Parse device data.
-
-        Args:
-            device_data (Dict[str, Any]): Device data to be parsed.
-        """
-
-        pass
-
-    def __parse_project_user(
-        self, user_data: Dict[str, Any]
-    ) -> List[SwitchKeyProjectUserType]:
-        """
-        Parse project user data.
-
-        Args:
-            user_data (Dict[str, Any]): Project user data to be parsed.
-
-        Returns:
-            List[SwitchKeyProjectUserType]: Parsed project user object.
-        """
-
-        users = []
-        for user in user_data:
-            users.append(
-                SwitchKeyProjectUserType(
-                    device=self.__parse_device(user),
-                    features=user.get("features"),
-                    id=user.get("id"),
-                    username=user.get("username"),
-                    environment_key=self.environment_key
-                )
-            )
-        return users
-
-    def __parse_user(
-        self, user_data: Dict[str, Any]
-    ) -> SwitchKeyUserType | List[SwitchKeyUserType]:
-        """
-        Parse user data.
-
-        Args:
-            user_data (Dict[str, Any]): User data to be parsed.
-
-        Returns:
-            SwitchKeyUserType | List[SwitchKeyUserType]: Parsed user object or list of parsed user objects.
-        """
-
-        if type(user_data) == list:
-            users: List[SwitchKeyUserType] = []
-            for user in user_data:
-                users.append(
-                    SwitchKeyUserType(
-                        background_color=user.get("background_color"),
-                        email=user.get("email"),
-                        first_name=user.get("first_name"),
-                        full_name=user.get("full_name"),
-                        is_active=user.get("is_active"),
-                        id=user.get("id"),
-                        joining_at=user.get("joining_at"),
-                        last_name=user.get("last_name"),
-                    )
-                )
+        if api_token is None:
+            self.config = SwitchKeyConfig()
+            if self.config.check():
+                self.logger.info("The config file exists, and api_token is loaded from the config file.")
+                self.api_token = self.config.load().access_token
         else:
-            return SwitchKeyUserType(
-                background_color=user_data.get("background_color"),
-                email=user_data.get("email"),
-                first_name=user_data.get("first_name"),
-                full_name=user_data.get("full_name"),
-                is_active=user_data.get("is_active"),
-                id=user_data.get("id"),
-                joining_at=user_data.get("joining_at"),
-                last_name=user_data.get("last_name"),
-            )
-
-    def __parse_organization(
-        self, organization_data: Dict[str, Any]
-    ) -> SwitchKeyOrganizationType:
-        """
-        Parse organization data.
-
-        Args:
-            organization_data (Dict[str, Any]): Organization data to be parsed.
-
-        Returns:
-            SwitchKeyOrganizationType: Parsed organization object.
-        """
-
-        return SwitchKeyOrganizationType(
-            id=organization_data.get("id"),
-            name=organization_data.get("name"),
-            created=organization_data.get("created"),
-            modified=organization_data.get("modified"),
-            members=self.__parse_user(organization_data.get("members")),
-            owner=self.__parse_user(organization_data.get("owner")),
-        )
-
-    def __parse_project(self, project_data: Dict[str, Any]) -> SwitchKeyProjectType:
-        """
-        Parse project data.
+            raise AuthenticationError("There are no tokens found in the config file, and none were specified when initializing an instance of the SwitchKey client. Please ensure that tokens are provided either in the config file or passed during initialization.")
 
-        Args:
-            project_data (Dict[str, Any]): Project data to be parsed.
-
-        Returns:
-            SwitchKeyProjectType: Parsed project object.
-        """
-
-        return SwitchKeyProjectType(
-            id=project_data.get("id"),
-            name=project_data.get("name"),
-            created=project_data.get("created"),
-            modified=project_data.get("modified"),
-            organization=self.__parse_organization(project_data.get("organization")),
-        )
-
-    def __parse_environment(self) -> SwitchKeyEnvironmentType:
-        """
-        Parse environment data.
-
-        Returns:
-            SwitchKeyEnvironmentType: Parsed environment object.
-        """
-
-        return SwitchKeyEnvironmentType(
-            created=self.environment_data.get("created"),
-            id=self.environment_data.get("id"),
-            project=self.__parse_project(self.environment_data.get("project")),
-            environment_key=self.environment_data.get("environment_key"),
-            modified=self.environment_data.get("modified"),
-            name=self.environment_data.get("name"),
-            users=self.__parse_project_user(self.environment_data.get("users")),
-        )
+        self.api_token = api_token
+        self.organization = SwitchKeyOrganization(api_token = self.api_token)
+        self.project = SwitchKeyProject(api_token = self.api_token)
+
+        # self.FeatureNotEnabled = FeatureNotEnabledError
+        # self.features = {}
+        # self.__routes = SwitchKeyRoutes()
+        # self.environment_data = None
+        # self.environment = None
+    
+    # def connect(self, environment_key: UUID) -> None:
+    #     """
+    #     Connect to the SwitchKey environment.
+
+    #     Args:
+    #         environment_key (UUID): The key of the environment to connect to.
+
+    #     Raises:
+    #         ConnectionError: If there is an error message in the response.
+
+    #     Returns:
+    #         None
+    #     """
+    #     self.environment_key = environment_key
+
+    #     environment = SwitchKeyRequest.call(
+    #         self.__routes.get_route(EndPoints.ENVIRONMENTS_KEY, self.environment_key),
+    #         SwitchKeyRequestMethod.GET,
+    #     )
+
+    #     if environment.error_message:
+    #         raise ConnectionError(environment.error_message)
+
+    #     self.environment_data = environment.data
+    #     self.environment = self.__parse_environment()
+
+    # def __parse_device(self, device_data: Dict[str, Any]) -> None:
+    #     """
+    #     Parse device data.
+
+    #     Args:
+    #         device_data (Dict[str, Any]): Device data to be parsed.
+    #     """
+
+    #     pass
+
+    # def __parse_project_user(
+    #     self, user_data: Dict[str, Any]
+    # ) -> List[SwitchKeyProjectUserType]:
+    #     """
+    #     Parse project user data.
+
+    #     Args:
+    #         user_data (Dict[str, Any]): Project user data to be parsed.
+
+    #     Returns:
+    #         List[SwitchKeyProjectUserType]: Parsed project user object.
+    #     """
+
+    #     users = []
+    #     for user in user_data:
+    #         users.append(
+    #             SwitchKeyProjectUserType(
+    #                 device=self.__parse_device(user),
+    #                 features=user.get("features"),
+    #                 id=user.get("id"),
+    #                 username=user.get("username"),
+    #                 environment_key=self.environment_key
+    #             )
+    #         )
+    #     return users
+
+
+    # def __parse_environment(self) -> SwitchKeyEnvironmentType:
+    #     """
+    #     Parse environment data.
+
+    #     Returns:
+    #         SwitchKeyEnvironmentType: Parsed environment object.
+    #     """
+
+    #     return SwitchKeyEnvironmentType(
+    #         created=self.environment_data.get("created"),
+    #         id=self.environment_data.get("id"),
+    #         project=self.__parse_project(self.environment_data.get("project")),
+    #         environment_key=self.environment_data.get("environment_key"),
+    #         modified=self.environment_data.get("modified"),
+    #         name=self.environment_data.get("name"),
+    #         users=self.__parse_project_user(self.environment_data.get("users")),
+    #     )
```

### Comparing `switchkey-0.1.0/PKG-INFO` & `switchkey-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: switchkey
-Version: 0.1.0
-Summary: The SwitchKey Python client is a versatile tool for interacting with the SwitchKey feature management platform in Python applications. With this client, developers can easily integrate feature flags and toggle management capabilities into their Python projects. The client provides methods for connecting to SwitchKey environments, accessing user data, retrieving feature values, setting feature flags, and more. It simplifies the process of incorporating feature management functionality, enabling developers to efficiently control feature rollout and experimentation in their applications.
+Version: 0.1.1
+Summary: The SwitchKey Python client enables seamless integration with the SwitchKey feature management platform in Python applications. Developers can effortlessly incorporate feature flags and toggle management into their projects, accessing user data, retrieving feature values, and setting feature flags with ease. This client streamlines the process of implementing feature management functionality, empowering developers to efficiently control feature rollout and experimentation in their applications.
 Author: Mahmoud Emad
 Author-email: mahmmoud.hassanein@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: configparser (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SwitchKey Python Client
 
 ## Introduction
```

