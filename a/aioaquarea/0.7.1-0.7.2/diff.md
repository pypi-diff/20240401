# Comparing `tmp/aioaquarea-0.7.1.tar.gz` & `tmp/aioaquarea-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioaquarea-0.7.1.tar", last modified: Fri Mar 29 23:47:06 2024, max compression
+gzip compressed data, was "aioaquarea-0.7.2.tar", last modified: Mon Apr  1 12:48:07 2024, max compression
```

## Comparing `aioaquarea-0.7.1.tar` & `aioaquarea-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:47:06.615593 aioaquarea-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-29 23:47:06.615593 aioaquarea-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:47:06.615593 aioaquarea-0.7.1/aioaquarea/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    39047 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/aioaquarea/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:47:06.615593 aioaquarea-0.7.1/aioaquarea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-29 23:47:06.000000 aioaquarea-0.7.1/aioaquarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-29 23:47:06.000000 aioaquarea-0.7.1/aioaquarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:47:06.000000 aioaquarea-0.7.1/aioaquarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-29 23:47:06.000000 aioaquarea-0.7.1/aioaquarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 23:47:06.000000 aioaquarea-0.7.1/aioaquarea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-29 23:47:02.000000 aioaquarea-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 23:47:06.615593 aioaquarea-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:48:07.941044 aioaquarea-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-01 12:48:07.941044 aioaquarea-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:48:07.937044 aioaquarea-0.7.2/aioaquarea/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40290 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/aioaquarea/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:48:07.937044 aioaquarea-0.7.2/aioaquarea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-01 12:48:07.000000 aioaquarea-0.7.2/aioaquarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 12:48:07.000000 aioaquarea-0.7.2/aioaquarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:48:07.000000 aioaquarea-0.7.2/aioaquarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 12:48:07.000000 aioaquarea-0.7.2/aioaquarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 12:48:07.000000 aioaquarea-0.7.2/aioaquarea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 12:48:01.000000 aioaquarea-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:48:07.941044 aioaquarea-0.7.2/setup.cfg
```

### Comparing `aioaquarea-0.7.1/LICENSE` & `aioaquarea-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/PKG-INFO` & `aioaquarea-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioaquarea
-Version: 0.7.1
+Version: 0.7.2
 Summary: Asynchronous library to control Panasonic Aquarea devices
 Author-email: "Carlos J. Aliaga" <dev@cjaliaga.net>
 License: MIT License
         
         Copyright (c) 2022 Carlos J. Aliaga
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aioaquarea-0.7.1/README.md` & `aioaquarea-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea/__init__.py` & `aioaquarea-0.7.2/aioaquarea/__init__.py`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea/const.py` & `aioaquarea-0.7.2/aioaquarea/const.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 AQUAREA_SERVICE_DEMO_BASE = "https://demo.aquarea-smart.panasonic.com/"
 AQUAREA_SERVICE_LOGIN = "remote/v1/api/auth/login"
 AQUAREA_SERVICE_DEVICES = "remote/v1/api/devices"
 AQUAREA_SERVICE_CONSUMPTION = "remote/v1/api/consumption"
 AQUAREA_SERVICE_CONTRACT = "remote/contract"
 AQUAREA_SERVICE_A2W_STATUS_DISPLAY = "remote/a2wStatusDisplay"
 AQUAREA_SERVICE_AUTH_CLIENT_ID = "vf2i6hW5hA2BB2BQGfTHXM4YFyW4I06K"
+AQUAREA_SERVICE_AUTH0_CLIENT = "eyJuYW1lIjoiYXV0aDAuanMtdWxwIiwidmVyc2lvbiI6IjkuMjMuMiJ9"
 
 PANASONIC = "Panasonic"
 
 
 class AquareaEnvironment(IntEnum):
     """Aquarea environment"""
```

### Comparing `aioaquarea-0.7.1/aioaquarea/core.py` & `aioaquarea-0.7.2/aioaquarea/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import urllib.parse
 import html
 
 import aiohttp
 
 from .const import (
     AQUAREA_SERVICE_A2W_STATUS_DISPLAY,
+    AQUAREA_SERVICE_AUTH0_CLIENT,
     AQUAREA_SERVICE_BASE,
     AQUAREA_SERVICE_CONSUMPTION,
     AQUAREA_SERVICE_CONTRACT,
     AQUAREA_SERVICE_DEMO_BASE,
     AQUAREA_SERVICE_DEVICES,
     AQUAREA_SERVICE_LOGIN,
     AQUAREA_SERVICE_AUTH_CLIENT_ID,
@@ -215,15 +216,15 @@
 
         resp = await self._sess.request(method, url, **kwargs)
 
         if resp.content_type == "application/json":
             data = await resp.json()
 
             # let's check for access token and expiration time
-            if self._access_token and "accessToken" in data:
+            if self._access_token and self.__contains_valid_token(data):
                 self._access_token = data["accessToken"]["token"]
                 self._token_expiration = dt.datetime.strptime(
                     data["accessToken"]["expires"], "%Y-%m-%dT%H:%M:%S%z"
                 )
 
             # Aquarea returns a 200 even if the request failed, we need to check the message property to see if it's an error
             # Some errors just require to login again, so we raise a AuthenticationError in those known cases
@@ -235,14 +236,22 @@
                     if error.error_code in list(AuthenticationErrorCodes):
                         raise AuthenticationError(error.error_code, error.error_message)
 
                     raise ApiError(error.error_code, error.error_message)
 
         return resp
 
+    def __contains_valid_token(self, data: dict) -> bool:
+        """Check if the data contains a valid token."""
+        return (
+            "accessToken" in data
+            and "token" in data["accessToken"]
+            and "expires" in data["accessToken"]
+        )
+
     async def look_for_errors(
         self, data: dict
     ) -> list[FaultError]:
         """Look for errors in the response and return them as a list of FaultError objects."""
         if not isinstance(data, dict):
             return []
 
@@ -256,30 +265,30 @@
         intent = dt.datetime.now()
         await self._login_lock.acquire()
         try:
             if self._last_login > intent:
                 return
 
             if self._environment is AquareaEnvironment.DEMO:
-                await self._login_demo()
+                await self.__login_demo()
             else:
-                await self._login_production()
-
+                await self.__login_production()
+                
             self._last_login = dt.datetime.now()
 
         finally:
             self._login_lock.release()
 
-    async def _login_demo(self) -> None:
+    async def __login_demo(self) -> None:
         _ = await self.request("GET", "", referer=self._base_url)
         self._token_expiration = dt.datetime.astimezone(
             dt.datetime.utcnow(), tz=dt.timezone.utc
         ) + dt.timedelta(days=1)
 
-    async def _login_production(self) -> None:
+    async def __login_production(self) -> None:
         response: aiohttp.ClientResponse = await self.request(
             "POST",
             AQUAREA_SERVICE_LOGIN,
             referer=self._base_url,
             headers={
                 "popup-screen-id": "1001",
                 "Registration-Id": "",
@@ -300,14 +309,20 @@
             "GET",
             external_url="https://authglb.digital.panasonic.com/authorize",
             referer=self._base_url,
             params=query_params,
             allow_redirects=False)
 
         location = response.headers.get("Location")
+
+        # We might be already on the last step of the login process if we're refreshing the token
+        if self.__is_final_step(location):
+            return await self.__complete_login(location)
+        
+        # We continue with the login process
         parsed_url = urllib.parse.urlparse(location)
 
         # Extract the value of the 'state' query parameter
         query_params2 = urllib.parse.parse_qs(parsed_url.query)
         state_value = query_params2.get('state', [None])[0]
 
         response: aiohttp.ClientResponse = await self.request(
@@ -346,15 +361,15 @@
 
         response: aiohttp.ClientResponse = await self.request(
             "POST",
             external_url="https://authglb.digital.panasonic.com/usernamepassword/login",
             referer=f"https://authglb.digital.panasonic.com/login?{urllib.parse.urlencode(query_params)}",
             content_type="application/json; charset=UTF-8",
             headers={
-                "Auth0-Client": "eyJuYW1lIjoiYXV0aDAuanMtdWxwIiwidmVyc2lvbiI6IjkuMjMuMiJ9"
+                "Auth0-Client": AQUAREA_SERVICE_AUTH0_CLIENT,
             },
             allow_redirects=False,
             json=data,
             throw_on_error=False)
 
         if not response.ok and response.content_type == "application/json":
             data = await response.json()
@@ -391,27 +406,40 @@
             "GET",
             external_url=f"https://authglb.digital.panasonic.com{location}",
             referer=self._base_url,
             allow_redirects=False)
 
         location = response.headers.get("Location") 
 
+        if self.__is_final_step(location):
+            return await self.__complete_login(location)
+        
+        raise AuthenticationError(AuthenticationErrorCodes.INVALID_USERNAME_OR_PASSWORD, "Invalid username or password")
+
+    async def __complete_login(self, location: str) -> None:
+        """Complete the login process."""
+        
         response: aiohttp.ClientResponse = await self.request(
             "GET",
             external_url=location,
             referer=self._base_url,
             allow_redirects=False)
         
         self._access_token = response.cookies.get("accessToken").value
         self._token_expiration = None
 
         self._logger.info(
             f"Login successful for {self.username}. Access Token Expiration: {self._token_expiration}"
         )
 
+    def __is_final_step(self, location: str) -> bool:
+        """Check if the location is the final step of the login process."""
+        parsed = urllib.parse.urlparse(location)
+        return parsed.hostname == "aquarea-smart.panasonic.com" and parsed.path == "/authorizationCallback" and "code" in urllib.parse.parse_qs(parsed.query)
+
     @auth_required
     async def get_devices(self, include_long_id=False) -> list[DeviceInfo]:
         """Get list of devices and its configuration, without status."""
         response = await self.request("GET", AQUAREA_SERVICE_DEVICES)
         data = await response.json()
 
         if not isinstance(data, dict):
```

### Comparing `aioaquarea-0.7.1/aioaquarea/data.py` & `aioaquarea-0.7.2/aioaquarea/data.py`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea/errors.py` & `aioaquarea-0.7.2/aioaquarea/errors.py`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea/statistics.py` & `aioaquarea-0.7.2/aioaquarea/statistics.py`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea/util.py` & `aioaquarea-0.7.2/aioaquarea/util.py`

 * *Files identical despite different names*

### Comparing `aioaquarea-0.7.1/aioaquarea.egg-info/PKG-INFO` & `aioaquarea-0.7.2/aioaquarea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioaquarea
-Version: 0.7.1
+Version: 0.7.2
 Summary: Asynchronous library to control Panasonic Aquarea devices
 Author-email: "Carlos J. Aliaga" <dev@cjaliaga.net>
 License: MIT License
         
         Copyright (c) 2022 Carlos J. Aliaga
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aioaquarea-0.7.1/pyproject.toml` & `aioaquarea-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioaquarea"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Carlos J. Aliaga", email="dev@cjaliaga.net" },
 ]
 description = "Asynchronous library to control Panasonic Aquarea devices"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

