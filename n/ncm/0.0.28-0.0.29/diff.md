# Comparing `tmp/ncm-0.0.28.tar.gz` & `tmp/ncm-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.28.tar", last modified: Tue Nov 15 20:01:36 2022, max compression
+gzip compressed data, was "ncm-0.0.29.tar", last modified: Mon Apr  1 16:34:15 2024, max compression
```

## Comparing `ncm-0.0.28.tar` & `ncm-0.0.29.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nathanwiens   (501) staff       (20)        0 2022-11-15 20:01:36.210624 ncm-0.0.28/
--rw-r--r--   0 nathanwiens   (501) staff       (20)     1083 2022-10-24 18:22:09.000000 ncm-0.0.28/LICENSE
--rw-r--r--   0 nathanwiens   (501) staff       (20)     1882 2022-11-15 20:01:36.210371 ncm-0.0.28/PKG-INFO
--rw-r--r--   0 nathanwiens   (501) staff       (20)     1569 2022-10-24 18:22:09.000000 ncm-0.0.28/README.md
-drwxr-xr-x   0 nathanwiens   (501) staff       (20)        0 2022-11-15 20:01:36.207454 ncm-0.0.28/ncm/
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)        0 2020-05-07 17:44:40.000000 ncm-0.0.28/ncm/__init__.py
--rw-r--r--   0 nathanwiens   (501) staff       (20)    83084 2022-11-15 19:59:44.000000 ncm-0.0.28/ncm/ncm.py
-drwxr-xr-x   0 nathanwiens   (501) staff       (20)        0 2022-11-15 20:01:36.210002 ncm-0.0.28/ncm.egg-info/
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)     1882 2022-11-15 20:01:36.000000 ncm-0.0.28/ncm.egg-info/PKG-INFO
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)      187 2022-11-15 20:01:36.000000 ncm-0.0.28/ncm.egg-info/SOURCES.txt
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)        1 2022-11-15 20:01:36.000000 ncm-0.0.28/ncm.egg-info/dependency_links.txt
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)       17 2022-11-15 20:01:36.000000 ncm-0.0.28/ncm.egg-info/requires.txt
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)        4 2022-11-15 20:01:36.000000 ncm-0.0.28/ncm.egg-info/top_level.txt
--rw-r--r--   0 nathanwiens   (501) staff       (20)       38 2022-11-15 20:01:36.210704 ncm-0.0.28/setup.cfg
--rwxr-xr-x   0 nathanwiens   (501) staff       (20)      578 2022-11-15 20:00:27.000000 ncm-0.0.28/setup.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.946784 ncm-0.0.29/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.29/LICENSE
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2304 2024-04-01 16:34:15.946784 ncm-0.0.29/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.29/README.md
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.945784 ncm-0.0.29/ncm/
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.29/ncm/__init__.py
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   149446 2024-04-01 16:31:07.000000 ncm-0.0.29/ncm/ncm.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.946784 ncm-0.0.29/ncm.egg-info/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2304 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/requires.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/top_level.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-01 16:34:15.946784 ncm-0.0.29/setup.cfg
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      590 2024-04-01 16:32:08.000000 ncm-0.0.29/setup.py
```

### Comparing `ncm-0.0.28/LICENSE` & `ncm-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.28/PKG-INFO` & `ncm-0.0.29/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1
-Name: ncm
-Version: 0.0.28
-Summary: Python client library for Cradlepoint NCM API
-Home-page: https://github.com/nathanwiens/ncm
-Author: Nathan Wiens - Cradlepoint
-Author-email: nathan.wiens@cradlepoint.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cradlepoint NCM SDK
-This is a Python client library for Cradlepoint NCM API
+This is a Python client library for Cradlepoint NCM API (both v2 and v3)
 
 INSTALL AND RUN INSTRUCTIONS
 
 1. Install the ncm pip package, or copy the ncm.py file into your working directory:
     ```
     pip3 install ncm
     ```
 
-2. Set NCM API Keys. API Keys must be passed as a dictionary:
+2. Set NCM API v2 Keys. API Keys must be passed as a dictionary:
     ```
     api_keys = {
         'X-CP-API-ID': 'aaaa',
         'X-CP-API-KEY': 'bbbb',
         'X-ECM-API-ID': 'cccc',
         'X-ECM-API-KEY': 'dddd'
     }
     ```
+    For API v3 Key it can be included in the same dictionary as token (optional):
+    ```
+    api_keys = {
+        'X-CP-API-ID': 'aaaa',
+        'X-CP-API-KEY': 'bbbb',
+        'X-ECM-API-ID': 'cccc',
+        'X-ECM-API-KEY': 'dddd',
+        "token": 'eeee'
+    }
+    ```
+    Note: if only using v3, just include the token in the dictionary.
 
 3. Import the module and create an instance of the NcmClient object:
    
    If using pip:
     ```
     from ncm import ncm
     n = ncm.NcmClient(api_keys=api_keys)
```

### Comparing `ncm-0.0.28/ncm/ncm.py` & `ncm-0.0.29/ncm/ncm.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 """
 
 from requests import Session
 from requests.adapters import HTTPAdapter
 from http import HTTPStatus
 from urllib3.util.retry import Retry
 from datetime import datetime, timedelta
+import sys
 import os
 import json
 
 
 def __is_json(test_json):
     """
     Checks if a string is a valid json object
@@ -62,109 +63,127 @@
     try:
         json.loads(test_json)
     except ValueError:
         return False
     return True
 
 
-class NcmClient:
-    """
-    This NCM Client class provides functions for interacting with =
-    the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
-    found at: https://developer.cradlepoint.com
-    """
-
+class BaseNcmClient:
     def __init__(self,
-                 api_keys=None,
                  log_events=True,
+                 logger=None,
                  retries=5,
                  retry_backoff_factor=2,
                  retry_on=None,
-                 base_url=os.environ.get(
-                     'CP_BASE_URL', 'https://www.cradlepointecm.com/api/v2')
-                 ):
+                 base_url=None):
         """
         Constructor. Sets up and opens request session.
-        :param api_keys: Dictionary of API credentials.
-          Optional, but must be set before calling functions.
-        :type api_keys: dict
         :param retries: number of retries on failure. Optional.
         :param retry_backoff_factor: backoff time multiplier for retries.
           Optional.
         :param retry_on: types of errors on which automatic retry will occur.
           Optional.
         :param base_url: # base url for calls. Configurable for testing.
           Optional.
         """
         if retry_on is None:
             retry_on = [
                 HTTPStatus.REQUEST_TIMEOUT,
                 HTTPStatus.GATEWAY_TIMEOUT,
                 HTTPStatus.SERVICE_UNAVAILABLE
             ]
-        if api_keys is None:
-            api_keys = {}
-        self.logEvents = log_events
-        self.base_url = base_url
+        self.log_events = log_events
+        self.logger = logger
         self.session = Session()
         self.adapter = HTTPAdapter(
             max_retries=Retry(total=retries,
                               backoff_factor=retry_backoff_factor,
                               status_forcelist=retry_on,
                               redirect=3
                               )
         )
+        self.base_url = base_url
         self.session.mount(self.base_url, self.adapter)
-        if api_keys:
-            if self.__validate_api_keys(api_keys):
-                self.session.headers.update(api_keys)
-        self.session.headers.update({
-            'Content-Type': 'application/json'
-        })
+    
+    def log(self, level, message):
+        """
+        Logs messages if self.logEvents is True.
+        """
+        if self.log_events:
+            if self.logger:
+                log_level = getattr(self.logger, level)
+                log_level(message)
+            else:
+                print(f"{level}: {message}", file=sys.stderr) 
 
-    def __return_handler(self, status_code, returntext, obj_type):
+    def _return_handler(self, status_code, returntext, obj_type):
         """
         Prints returned HTTP request information if self.logEvents is True.
         """
         if str(status_code) == '200':
-            if self.logEvents:
-                print('{0} Operation Successful\n'.format(str(obj_type)))
-            return None
+            return f'{obj_type} operation successful.'
         elif str(status_code) == '201':
-            if self.logEvents:
-                print('{0} Added Successfully\n'.format(str(obj_type)))
-            return None
+            self.log('info', '{0} created Successfully'.format(str(obj_type)))
+            return returntext
         elif str(status_code) == '202':
-            if self.logEvents:
-                print('{0} Added Successfully\n'.format(str(obj_type)))
-            return None
+            self.log('info', '{0} accepted Successfully'.format(str(obj_type)))
+            return returntext
         elif str(status_code) == '204':
-            if self.logEvents:
-                print('{0} Deleted Successfully\n'.format(str(obj_type)))
-            return None
+            self.log('info', '{0} deleted Successfully'.format(str(obj_type)))
+            return returntext
         elif str(status_code) == '400':
-            if self.logEvents:
-                print('Bad Request\n')
-            return None
+            self.log('error', 'Bad Request')
+            return f'ERROR: {status_code}: {returntext}'
         elif str(status_code) == '401':
-            if self.logEvents:
-                print('Unauthorized Access\n')
-            return returntext
+            self.log('error', 'Unauthorized Access')
+            return f'ERROR: {status_code}: {returntext}'
         elif str(status_code) == '404':
-            if self.logEvents:
-                print('Resource Not Found\n')
-            return returntext
+            self.log('error', 'Resource Not Found\n')
+            return f'ERROR: {status_code}: {returntext}'
         elif str(status_code) == '500':
-            if self.logEvents:
-                print('HTTP 500 - Server Error\n')
-            return returntext
+            self.log('error', 'HTTP 500 - Server Error\n')
+            return f'ERROR: {status_code}: {returntext}'
         else:
-            print('HTTP Status Code: {0} - No returned data\n'.format(
-                str(status_code)))
+            self.log('info', f'HTTP Status Code: {status_code} - {returntext}\n')
+
+
+class NcmClientv2(BaseNcmClient):
+    def __init__(self,
+                 api_keys=None,
+                 log_events=True,
+                 logger=None,
+                 retries=5,
+                 retry_backoff_factor=2,
+                 retry_on=None,
+                 base_url=None):
+        base_url = base_url or os.environ.get("CP_BASE_URL", "https://www.cradlepointecm.com/api/v2")
+        super().__init__(log_events=log_events, logger=logger, retries=retries, retry_backoff_factor=retry_backoff_factor, retry_on=retry_on, base_url=base_url)
+        if api_keys:
+            if self.__validate_api_keys(api_keys):
+                self.session.headers.update(api_keys)
+        self.session.headers.update({
+            'Content-Type': 'application/json'
+        })
+    
+    def __validate_api_keys(self, api_keys):
+        """
+        Checks NCM API Keys are a dictionary containing all necessary keys
+        :param api_keys: Dictionary of API credentials. Optional.
+        :type api_keys: dict
+        :return: True if valid
+        """
+        if not isinstance(api_keys, dict):
+            raise TypeError("API Keys must be passed as a dictionary")
+
+        for key in ('X-CP-API-ID', 'X-CP-API-KEY', 'X-ECM-API-ID', 'X-ECM-API-KEY'):
+            if not api_keys.get(key):
+                raise KeyError(f"{key} missing. Please ensure all API Keys are present.")
 
+        return True
+    
     def __get_json(self, get_url, call_type, params=None):
         """
         Returns full paginated results, and handles chunking "__in" params
         in groups of 100.
         """
         results = []
         __in_keys = 0
@@ -198,28 +217,28 @@
                         chunk_str = ','.join(map(str, chunk))
                         params.update({key: chunk_str})
                         url = get_url
                         while url and (len(results) < limit):
                             ncm = self.session.get(url, params=params)
                             if not (200 <= ncm.status_code < 300):
                                 break
-                            self.__return_handler(ncm.status_code,
+                            self._return_handler(ncm.status_code,
                                                   ncm.json()['data'],
                                                   call_type)
                             url = ncm.json()['meta']['next']
                             for d in ncm.json()['data']:
                                 results.append(d)
 
         if __in_keys == 0:
             url = get_url
             while url and (len(results) < limit):
                 ncm = self.session.get(url, params=params)
                 if not (200 <= ncm.status_code < 300):
                     break
-                self.__return_handler(ncm.status_code, ncm.json()['data'],
+                self._return_handler(ncm.status_code, ncm.json()['data'],
                                       call_type)
                 url = ncm.json()['meta']['next']
                 for d in ncm.json()['data']:
                     results.append(d)
         return results
 
     def __parse_kwargs(self, kwargs, allowed_params):
@@ -231,39 +250,20 @@
         if 'limit' not in params:
             params.update({'limit': '500'})
 
         bad_params = {k: v for (k, v) in kwargs.items() if
                       k not in allowed_params}
         if len(bad_params) > 0:
             raise ValueError("Invalid parameters: {}".format(bad_params))
-
-        if 'X-CP-API-ID' not in self.session.headers:
-            raise KeyError(
-                "X-CP-API-ID missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-CP-API-KEY' not in self.session.headers:
-            raise KeyError(
-                "X-CP-API-KEY missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-ECM-API-ID' not in self.session.headers:
-            raise KeyError(
-                "X-ECM-API-ID missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-ECM-API-KEY' not in self.session.headers:
-            raise KeyError(
-                "X-ECM-API-KEY missing. "
-                "Please ensure all API Keys are present.")
+        
+        self.__validate_api_keys(dict(self.session.headers)) 
 
         return params
 
-    @staticmethod
-    def __chunk_param(param):
+    def __chunk_param(self, param):
         """
         Chunks parameters into groups of 100 per Cradlepoint limit.
         Iterate through chunks with a for loop.
         """
         n = 100
 
         if type(param) is str:
@@ -273,46 +273,14 @@
         else:
             raise TypeError("Invalid param format. Must be str or list.")
 
         """Yield successive n-sized chunks from lst."""
         for i in range(0, len(param_list), n):
             yield param_list[i:i + n]
 
-    @staticmethod
-    def __validate_api_keys(api_keys):
-        """
-        Checks NCM API Keys are a dictionary containing all necessary keys
-        :param api_keys: Dictionary of API credentials. Optional.
-        :type api_keys: dict
-        :return: True if valid
-        """
-        if type(api_keys) is not dict:
-            raise TypeError("API Keys must be passed as a dictionary")
-
-        if 'X-CP-API-ID' not in api_keys:
-            raise KeyError(
-                "X-CP-API-ID missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-CP-API-KEY' not in api_keys:
-            raise KeyError(
-                "X-CP-API-KEY missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-ECM-API-ID' not in api_keys:
-            raise KeyError(
-                "X-ECM-API-ID missing. "
-                "Please ensure all API Keys are present.")
-
-        if 'X-ECM-API-KEY' not in api_keys:
-            raise KeyError(
-                "X-ECM-API-KEY missing. "
-                "Please ensure all API Keys are present.")
-        return True
-
     def set_api_keys(self, api_keys):
         """
         Sets NCM API Keys for session.
         :param api_keys: Dictionary of API credentials. Optional.
         :type api_keys: dict
         """
         if self.__validate_api_keys(api_keys):
@@ -365,15 +333,15 @@
 
         post_data = {
             'account': '/api/v1/accounts/{}/'.format(str(parent_account_id)),
             'name': str(subaccount_name)
         }
 
         ncm = self.session.post(post_url, data=json.dumps(post_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def create_subaccount_by_parent_name(self, parent_account_name,
                                          subaccount_name):
         """
         This operation creates a new subaccount.
         :param parent_account_name: Name of parent account.
@@ -394,15 +362,15 @@
         put_url = '{0}/accounts/{1}/'.format(self.base_url, str(subaccount_id))
 
         put_data = {
             "name": str(new_subaccount_name)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def rename_subaccount_by_name(self, subaccount_name, new_subaccount_name):
         """
         This operation renames a subaccount
         :param subaccount_name: Name of subaccount to rename
         :param new_subaccount_name: New name for subaccount
@@ -417,15 +385,15 @@
         :param subaccount_id: ID of subaccount to delete
         :return:
         """
         call_type = 'Subaccount'
         post_url = '{0}/accounts/{1}'.format(self.base_url, subaccount_id)
 
         ncm = self.session.delete(post_url)
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def delete_subaccount_by_name(self, subaccount_name):
         """
         This operation deletes a subaccount
         :param subaccount_name: Name of subaccount to delete
         :return:
@@ -522,15 +490,15 @@
         :return:
         """
         call_type = 'Configuration Manager'
         put_url = '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                            config_man_id)
 
         ncm = self.session.put(put_url, json=config_man_json)
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def patch_configuration_managers(self, router_id, config_man_json):
         """
         This method patches an configuration_managers for associated id.
         :param router_id: ID of router to update
         :param config_man_json: JSON of the "configuration" field of the
@@ -551,15 +519,15 @@
         payload = config_man_json
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
 
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def put_configuration_managers(self, router_id, configman_json):
         """
         This method overwrites the configuration for a router with id.
         :param router_id: ID of router to update
         :param configman_json: JSON of the "configuration" field of the
@@ -579,15 +547,15 @@
 
         payload = configman_json
 
         ncm = self.session.put(
             '{0}/configuration_managers/{1}/?fields=configuration'.format(
                 self.base_url, str(configman_id)),
             json=payload)  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def patch_group_configuration(self, group_id, config_json):
         """
         This method patches an configuration_managers for associated id.
         :param group_id: ID of group to update
         :param config_json: JSON of the "configuration" field of the
@@ -597,15 +565,15 @@
         call_type = 'Configuration Manager'
 
         payload = config_json
 
         ncm = self.session.patch(
             '{0}/groups/{1}/'.format(self.base_url, str(group_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def copy_router_configuration(self, src_router_id, dst_router_id):
         """
         Copies the Configuration Manager config of one router to another.
         This function will not copy any passwords as they are encrypted.
         :param src_router_id: Router ID to copy from
@@ -624,15 +592,15 @@
         dst_config_man_id = \
             self.get_configuration_managers(router=dst_router_id)[0]['id']
 
         put_url = '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                            dst_config_man_id)
 
         ncm = self.session.patch(put_url, data=src_config)
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def resume_updates_for_router(self, router_id):
         """
         This method will resume updates for a router in Sync Suspended state.
         :param router_id: ID of router to update
         :return:
@@ -647,15 +615,15 @@
         configman_id = response['data'][0]['id']
         payload = {"suspended": False}
 
         ncm = self.session.put(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(configman_id)),
             json=payload)
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def get_device_app_bindings(self, **kwargs):
         """
         This method gives device app binding information for all device
         app bindings associated with the account.
         :param kwargs: A set of zero or more allowed parameters
@@ -843,15 +811,15 @@
             'name': str(group_name),
             'product': str(
                 self.get_product_by_name(product_name)['resource_url']),
             'target_firmware': str(firmware['resource_url'])
         }
 
         ncm = self.session.post(post_url, data=json.dumps(post_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def create_group_by_parent_name(self, parent_account_name, group_name,
                                     product_name, firmware_version):
         """
         This operation creates a new group.
         :param parent_account_name: Name of parent account
@@ -878,15 +846,15 @@
         put_url = '{0}/groups/{1}/'.format(self.base_url, group_id)
 
         put_data = {
             "name": str(new_group_name)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def rename_group_by_name(self, existing_group_name, new_group_name):
         """
         This operation renames a group by specifying name.
         :param existing_group_name: Name of the group to rename
         :param new_group_name: New name for the group.
@@ -901,15 +869,15 @@
         :param group_id: ID of the group to delete
         :return:
         """
         call_type = 'Group'
         post_url = '{0}/groups/{1}/'.format(self.base_url, group_id)
 
         ncm = self.session.delete(post_url)
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def delete_group_by_name(self, group_name):
         """
         This operation deletes a group by specifying Name.
         :param group_name: Name of the group to delete
         :return:
@@ -1012,15 +980,15 @@
             'longitude': longitude,
             'method': 'manual',
             'router': 'https://www.cradlepointecm.com/api/v2/routers/{}/'
                 .format(str(router_id))
         }
 
         ncm = self.session.post(post_url, data=json.dumps(post_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def delete_location_for_router(self, router_id):
         """
         This operation deletes the location for a router by ID.
         :param router_id: ID of router for which to remove location.
         :return:
@@ -1030,15 +998,15 @@
         locations = self.get_locations(router=router_id)
         if locations:
             location_id = locations[0]['id']
 
             post_url = '{0}/locations/{1}/'.format(self.base_url, location_id)
 
             ncm = self.session.delete(post_url)
-            result = self.__return_handler(ncm.status_code, ncm.text,
+            result = self._return_handler(ncm.status_code, ncm.text,
                                            call_type)
             return result
         else:
             return "NO LOCATION FOUND"
 
     def get_net_device_health(self, **kwargs):
         """
@@ -1239,15 +1207,15 @@
         post_url = '{0}/reboot_activity/'.format(self.base_url)
 
         post_data = {
             'router': '{0}/routers/{1}/'.format(self.base_url, str(router_id))
         }
 
         ncm = self.session.post(post_url, data=json.dumps(post_data))
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def reboot_group(self, group_id):
         """
         This operation reboots all routers in a group.
         :param group_id: ID of group to reboot
         :return:
@@ -1256,15 +1224,15 @@
         post_url = '{0}/reboot_activity/'.format(self.base_url)
 
         post_data = {
             'group': '{0}/groups/{1}/'.format(self.base_url, str(group_id))
         }
 
         ncm = self.session.post(post_url, data=json.dumps(post_data))
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def get_router_alerts(self, **kwargs):
         """
         This method provides a history of device alerts. To receive device
         alerts, you must enable them through the ECM UI: Alerts -> Settings.
         The info section of the alert is firmware dependent and
@@ -1549,15 +1517,15 @@
         put_url = '{0}/routers/{1}/'.format(self.base_url, router_id)
 
         put_data = {
             'name': str(new_router_name)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def rename_router_by_name(self, existing_router_name, new_router_name):
         """
         This operation renames a router by name.
         :param existing_router_name: Name of router to rename
         :param new_router_name: New name for router
@@ -1580,15 +1548,15 @@
 
         put_data = {
             "group": 'https://www.cradlepointecm.com/api/v2/groups/{}/'.format(
                 group_id)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def remove_router_from_group(self, router_id=None, router_name=None):
         """
         This operation removes a router from its group.
         Either the ID or the name must be specified.
         :param router_id: ID of router to move.
@@ -1605,18 +1573,17 @@
 
         put_data = {
             "group": None
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
         if ncm.status_code == 201 or ncm.status_code == 202:
-            if self.logEvents:
-                print('Router Modified Successfully\n')
+            self.log('info', 'Router Modified Successfully')
             return None
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def assign_router_to_account(self, router_id, account_id):
         """
         This operation assigns a router to an account.
         :param router_id: ID of router to move.
         :param account_id: ID of destination account.
@@ -1629,28 +1596,28 @@
         put_data = {
             "account":
                 'https://www.cradlepointecm.com/api/v2/accounts/{}/'.format(
                     account_id)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def delete_router_by_id(self, router_id):
         """
         This operation deletes a router by ID.
         :param router_id: ID of router to delete.
         :return:
         """
         call_type = 'Router'
         post_url = '{0}/routers/{1}/'.format(self.base_url, router_id)
 
         ncm = self.session.delete(post_url)
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def delete_router_by_name(self, router_name):
         """
         This operation deletes a router by name.
         :param router_name: Name of router to delete
         :return:
@@ -1810,15 +1777,15 @@
                 ]
             }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def set_custom1(self, router_id, text):
         """
         This method updates the Custom1 field in NCM for a given router id.
         :param router_id: ID of router to update.
         :param text: The text to set for the field
@@ -1829,15 +1796,15 @@
         put_url = '{0}/routers/{1}/'.format(self.base_url, str(router_id))
 
         put_data = {
             "custom1": str(text)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def set_custom2(self, router_id, text):
         """
         This method updates the Custom2 field in NCM for a given router id.
         :param router_id: ID of router to update.
         :param text: The text to set for the field
@@ -1848,15 +1815,15 @@
         put_url = '{0}/routers/{1}/'.format(self.base_url, str(router_id))
 
         put_data = {
             "custom2": str(text)
         }
 
         ncm = self.session.put(put_url, data=json.dumps(put_data))
-        result = self.__return_handler(ncm.status_code, ncm.json(), call_type)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def set_admin_password(self, router_id: int, new_password: str):
         """
         This method sets the local admin password for a router.
         :param router_id: ID of router to update
         :param new_password: Cleartext password to assign
@@ -1888,15 +1855,15 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def set_router_name(self, router_id: int, new_router_name: str):
         """
         This method sets the local admin password for a router.
         :param router_id: ID of router to update
         :param new_router_name: Name/System ID to set
@@ -1924,15 +1891,15 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def set_router_description(self, router_id: int, new_router_description: str):
         """
         This method sets the local admin password for a router.
         :param router_id: ID of router to update
         :param new_router_description: Description string to set
@@ -1960,15 +1927,15 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def set_router_asset_id(self, router_id: int, new_router_asset_id: str):
         """
         This method sets the local admin password for a router.
         :param router_id: ID of router to update
         :param new_router_asset_id: Asset ID string to set
@@ -1996,15 +1963,15 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def set_ethernet_wan_ip(self, router_id: int, new_wan_ip: str,
                             new_netmask: str = None, new_gateway: str = None):
         """
         This method sets the Ethernet WAN IP Address for a given router id.
         :param router_id: ID of router to update
@@ -2049,15 +2016,15 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
     def add_custom_apn(self, router_id: int, new_carrier: str, new_apn: str):
         """
         This method adds a new APN to the Advanced APN configuration
         :param router_id: ID of router to update
         :param new_carrier: Home Carrier / PLMN
@@ -2099,9 +2066,1807 @@
             ]
         }
 
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
-        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
+        return result
+
+class NcmClientv3(BaseNcmClient):
+    """
+    This NCM Client class provides functions for interacting with =
+    the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
+    found at: https://developer.cradlepoint.com
+    """
+
+    def __init__(self,
+                 api_key=None,
+                 log_events=False,
+                 logger=None,
+                 retries=5,
+                 retry_backoff_factor=2,
+                 retry_on=None,
+                 base_url=None):
+        """
+        Constructor. Sets up and opens request session.
+        :param api_key: API Bearer token (without the "Bearer" text).
+          Optional, but must be set before calling functions.
+        :type api_key: str
+        :param log_events: if True, HTTP status info will be printed. False by default
+        :type log_events: bool
+        :param retries: number of retries on failure. Optional.
+        :param retry_backoff_factor: backoff time multiplier for retries.
+          Optional.
+        :param retry_on: types of errors on which automatic retry will occur.
+          Optional.
+        :param base_url: # base url for calls. Configurable for testing.
+          Optional.
+        """
+        base_url = base_url or os.environ.get("CP_BASE_URL_V3", "https://api.cradlepointecm.com/api/v3")
+        super().__init__(log_events, logger, retries, retry_backoff_factor, retry_on, base_url)
+        if api_key:
+            token = {'Authorization': f'Bearer {api_key}'}
+            self.session.headers.update(token)
+        self.session.headers.update({
+            'Content-Type': 'application/vnd.api+json',
+            'Accept': 'application/vnd.api+json'
+        })
+
+    def __get_json(self, get_url, call_type, params=None):
+        """
+        Returns full paginated results
+        """
+        results = []
+
+        if params is not None and "limit" in params:
+            limit = params['limit']
+            if limit == 0:
+                limit = 1000000
+            if params['limit'] > 50 or params['limit'] == 0:
+                params['page[size]'] = 50
+            else:
+                params['page[size]'] = params['limit']
+        else:
+            limit = 50
+
+        url = get_url
+
+        while url and (len(results) < limit):
+            ncm = self.session.get(url, params=params)
+            if not (200 <= ncm.status_code < 300):
+                return self._return_handler(ncm.status_code, ncm.json(), call_type)
+            data = ncm.json()['data']
+            if isinstance(data, list):
+                self._return_handler(ncm.status_code, data, call_type)
+                for d in data:
+                    results.append(d)
+            else:
+                results.append(data)
+            if "links" in ncm.json():
+                url = ncm.json()['links']['next']
+            else:
+                url = None
+
+        if params is not None and "filter[fields]" in params.keys():
+            data = []
+            fields = params['filter[fields]'].split(",")
+            for result in results:
+                items = {}
+                for k, v in result['attributes'].items():
+                    if k in fields:
+                        items[k] = v
+                data.append(items)
+            return data
+
+        return results
+
+
+    def __parse_kwargs(self, kwargs, allowed_params):
+        """
+        Checks for invalid parameters and missing API Keys, and handles "filter" fields
+        """
+
+        bad_params = {k: v for (k, v) in kwargs.items() if
+                      k not in allowed_params if ("search" not in k and "filter" not in k and "sort" not in k)}
+        if len(bad_params) > 0:
+            raise ValueError("Invalid parameters: {}".format(bad_params))
+
+        if 'Authorization' not in self.session.headers:
+            raise KeyError(
+                "API key missing. "
+                "Please set API key before making API calls.")
+
+        params = {}
+
+        for key, val in kwargs.items():
+            if "search" in key or "filter" in key or "sort" in key or "limit" in key:
+                params[key] = val
+
+            elif "__" in key:
+                split_key = key.split("__")
+                params[f'filter[{split_key[0]}][{split_key[1]}]'] = val
+            else:
+                params[f'filter[{key}]'] = val
+
+        return params
+
+    def __parse_search_kwargs(self, kwargs, allowed_params):
+        """
+        Checks for invalid parameters and missing API Keys, and handles "search" fields
+        """
+
+        bad_params = {k: v for (k, v) in kwargs.items() if
+                      k not in allowed_params if ("search" not in k and "filter" not in k and "sort" not in k)}
+        if len(bad_params) > 0:
+            raise ValueError("Invalid parameters: {}".format(bad_params))
+
+        if 'Authorization' not in self.session.headers:
+            raise KeyError(
+                "API key missing. "
+                "Please set API key before making API calls.")
+
+        params = {}
+
+        for key, val in kwargs.items():
+            if "filter" in key or "sort" in key or "limit" in key:
+                params[key] = val
+            elif "fields" in key:
+                params[f'filter[{key}]'] = val
+            else:
+                if "search" not in key:
+                    params[f'search[{key}]'] = val
+
+        return params
+
+    def __parse_put_kwargs(self, kwargs, allowed_params):
+        """
+        Checks for invalid parameters and missing API Keys, and handles "filter" fields
+        """
+
+        bad_params = {k: v for (k, v) in kwargs.items() if
+                      k not in allowed_params if ("search" not in k and "filter" not in k and "sort" not in k)}
+        if len(bad_params) > 0:
+            raise ValueError("Invalid parameters: {}".format(bad_params))
+
+        if 'Authorization' not in self.session.headers:
+            raise KeyError(
+                "API key missing. "
+                "Please set API key before making API calls.")
+
+        return kwargs
+
+    def set_api_key(self, api_key):
+        """
+        Sets NCM API Keys for session.
+        :param api_key: API Bearer token (without the "Bearer" prefix).
+        :type api_key: str
+        """
+        if api_key:
+            token = {'Authorization': f'Bearer {api_key}'}
+            self.session.headers.update(token)
+        return
+
+    def get_users(self, **kwargs):
+        """
+        Returns users with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of users with details.
+        """
+        call_type = 'Users'
+        get_url = f'{self.base_url}/beta/users'
+
+        allowed_params = ['email',
+                          'email__not',
+                          'first_name',
+                          'first_name__ne',
+                          'id',
+                          'is_active__ne',
+                          'last_login',
+                          'last_login__lt',
+                          'last_login__lte',
+                          'last_login__gt',
+                          'last_login__gte',
+                          'last_login__ne',
+                          'last_name',
+                          'last_name__ne',
+                          'pending_email',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+
+    def create_user(self, email, first_name, last_name, **kwargs):
+        """
+        Creates a user.
+        :param email: Email address
+        :type email: str
+        :param first_name: First name
+        :type first_name: str
+        :param last_name: Last name
+        :type last_name: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: User creation result.
+        """
+        call_type = 'User'
+        post_url = f'{self.base_url}/beta/users'
+
+        allowed_params = ['is_active',
+                          'last_login',
+                          'pending_email']
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        params['email'] = email
+        params['first_name'] = first_name
+        params['last_name'] = last_name
+
+        """GET TENANT ID"""
+        t = self.get_subscriptions(limit=1)
+
+        data = {
+            "data": {
+                "type": "users",
+                "attributes": params,
+                "relationships": {
+                    "tenant": {
+                        "data": [t[0]['relationships']['tenants']['data']]
+                    }
+                }
+            }
+        }
+
+        ncm = self.session.post(post_url, data=json.dumps(data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
+
+    def update_user(self, email, **kwargs):
+        """
+        Updates a user's date.
+        :param email: Email address
+        :type email: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: User update result.
+        """
+        call_type = 'Users'
+
+        user = self.get_users(email=email)[0]
+        user.pop('links')
+
+        put_url = f'{self.base_url}/beta/users/{user["id"]}'
+
+        allowed_params = ['first_name',
+                          'last_name',
+                          'is_active',
+                          'user_id',
+                          'last_login',
+                          'pending_email']
+        params = self.__parse_kwargs(kwargs, allowed_params)
+
+        for k, v in params.items():
+            user['attributes'][k] = v
+
+        user = {"data": user}
+
+        ncm = self.session.put(put_url, data=json.dumps(user))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def delete_user(self, email, **kwargs):
+        """
+        Updates a user's date.
+        :param email: Email address
+        :type email: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: None unless error.
+        """
+        call_type = 'Users'
+
+        user = self.get_users(email=email)[0]
+        user.pop('links')
+
+        delete_url = f'{self.base_url}/beta/users/{user["id"]}'
+
+        ncm = self.session.delete(delete_url)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
+        return result
+
+    def get_asset_endpoints(self, **kwargs):
+        """
+        Returns assets with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of asset endpoints (routers) with details.
+        """
+        call_type = 'Asset Endpoints'
+        get_url = f'{self.base_url}/asset_endpoints'
+
+        allowed_params = ['id',
+                          'hardware_series',
+                          'hardware_series_key',
+                          'mac_address',
+                          'serial_number',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_subscriptions(self, **kwargs):
+        """
+        Returns subscriptions with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of subscriptions with details.
+        """
+        call_type = 'Subscriptions'
+        get_url = f'{self.base_url}/subscriptions'
+
+        allowed_params = ['end_time',
+                          'end_time__lt',
+                          'end_time__lte',
+                          'end_time__gt',
+                          'end_time__gte',
+                          'end_time__ne',
+                          'id',
+                          'name',
+                          'quantity',
+                          'start_time',
+                          'start_time__lt',
+                          'start_time__lte',
+                          'start_time__gt',
+                          'start_time__gte',
+                          'start_time__ne',
+                          'tenant',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if kwargs.get('search'):
+            params = self.__parse_search_kwargs(kwargs, allowed_params)
+        else:
+            params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_networks(self, **kwargs):
+        """
+        Returns information about your private cellular networks.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of PCNs with details.
+        """
+        call_type = 'Private Cellular Networks'
+        get_url = f'{self.base_url}/beta/private_cellular_networks'
+
+        allowed_params = ['core_ip',
+                          'created_at',
+                          'created_at__lt',
+                          'created_at__lte',
+                          'created_at__gt',
+                          'created_at__gte',
+                          'created_at__ne',
+                          'ha_enabled',
+                          'id',
+                          'mobility_gateways',
+                          'mobility_gateway_virtual_ip',
+                          'name',
+                          'state',
+                          'status',
+                          'tac',
+                          'type',
+                          'updated_at',
+                          'updated_at__lt',
+                          'updated_at__lte',
+                          'updated_at__gt',
+                          'updated_at__gte',
+                          'updated_at__ne',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_network(self, network_id, **kwargs):
+        """
+        Returns information about a private cellular network.
+        :param network_id: ID of the private_cellular_networks record
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: An individual PCN network with details.
+        """
+        call_type = 'Private Cellular Networks'
+        get_url = f'{self.base_url}/beta/private_cellular_networks/{network_id}'
+
+        allowed_params = ['name',
+                          'segw_ip',
+                          'ha_enabled',
+                          'mobility_gateway_virtual_ip',
+                          'state',
+                          'status',
+                          'tac',
+                          'created_at',
+                          'updated_at',
+                          'fields']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def update_private_cellular_network(self, id=None, name=None, **kwargs):
+        """
+        Make changes to a private cellular network.
+        :param id: PCN network ID. Specify either this or name.
+        :type id: str
+        :param name: PCN network name
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: PCN update result.
+        """
+        call_type = 'Private Cellular Network'
+
+        if not id and not name:
+            return "ERROR: no network specified. Must specify either network_id or network_name"
+
+        if id:
+            net = self.get_private_cellular_networks(id=id)[0]
+        elif name:
+            net = self.get_private_cellular_networks(name=name)[0]
+
+        if name:
+            kwargs['name'] = name
+
+        net.pop('links')
+
+        put_url = f'{self.base_url}/beta/private_cellular_networks/{net["id"]}'
+
+        allowed_params = ['core_ip',
+                          'ha_enabled',
+                          'id',
+                          'mobility_gateways',
+                          'mobility_gateway_virtual_ip',
+                          'name',
+                          'state',
+                          'status',
+                          'tac',
+                          'type']
+        params = self.__parse_put_kwargs(kwargs, allowed_params)
+
+        for k, v in params.items():
+            net['attributes'][k] = v
+
+        data = {"data": net}
+
+        ncm = self.session.put(put_url, data=json.dumps(data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def create_private_cellular_network(self, name, core_ip, ha_enabled=False, mobility_gateway_virtual_ip=None, mobility_gateways=None):
+        """
+        Make changes to a private cellular network.
+        :param name: Name of the networks.
+        :type name: str
+        :param core_ip: IP address to reach core network.
+        :type core_ip: str
+        :param ha_enabled: High availability (HA) of network.
+        :type ha_enabled: bool
+        :param mobility_gateway_virtual_ip: Virtual IP address to reach core when HA is enabled. Nullable.
+        :type mobility_gateway_virtual_ip: str
+        :param mobility_gateways: Comma separated list of private_cellular_cores IDs to add as mobility gateways. Nullable.
+        :type mobility_gateways: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Create PCN result..
+        """
+        call_type = 'Private Cellular Network'
+
+        post_url = f'{self.base_url}/beta/private_cellular_networks'
+
+        data = {
+            "data": {
+                "type": "private_cellular_networks",
+                "attributes": {
+                    "name": name,
+                    "core_ip": core_ip,
+                    "ha_enabled": ha_enabled,
+                    "mobility_gateway_virtual_ip": mobility_gateway_virtual_ip
+                }
+            }
+        }
+
+        if mobility_gateways:
+            relationships = {
+                "mobility_gateways": {
+                    "data": []
+                }
+            }
+            gateways = mobility_gateways.split(",")
+
+            for gateway in gateways:
+                relationships['mobility_gateways']['data'].append({"type": "private_cellular_cores", "id": gateway})
+
+            data['data']['relationships'] = relationships
+
+        ncm = self.session.post(post_url, data=json.dumps(data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def delete_private_cellular_network(self, id):
+        """
+        Returns information about a private cellular network.
+        :param id: ID of the private_cellular_networks record
+        :type id: str
+        :return: None unless error.
+        """
+        # TODO support deletion by network name
+        call_type = 'Private Cellular Network'
+        delete_url = f'{self.base_url}/beta/private_cellular_networks/{id}'
+
+        ncm = self.session.delete(delete_url)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
+        return result
+
+    def get_private_cellular_cores(self, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of Mobility Gateways with details.
+        """
+        call_type = 'Private Cellular Cores'
+        get_url = f'{self.base_url}/beta/private_cellular_cores'
+
+        allowed_params = ['created_at',
+                          'id',
+                          'management_ip',
+                          'network',
+                          'router',
+                          'status',
+                          'type',
+                          'updated_at',
+                          'url',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_core(self, core_id, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param core_id: ID of the private_cellular_cores record
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: An individual Mobility Gateway with details.
+        """
+        call_type = 'Private Cellular Core'
+        get_url = f'{self.base_url}/beta/private_cellular_cores/{core_id}'
+
+        allowed_params = ['created_at',
+                          'id',
+                          'management_ip',
+                          'network',
+                          'router',
+                          'status',
+                          'type',
+                          'updated_at',
+                          'url',
+                          'fields',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_radios(self, **kwargs):
+        """
+        Returns information about a private cellular radio.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of Cellular APs with details.
+        """
+        call_type = 'Private Cellular Radios'
+        get_url = f'{self.base_url}/beta/private_cellular_radios'
+
+        allowed_params = ['admin_state',
+                          'antenna_azimuth',
+                          'antenna_beamwidth',
+                          'antenna_downtilt',
+                          'antenna_gain',
+                          'bandwidth',
+                          'category',
+                          'cpi_id',
+                          'cpi_name',
+                          'cpi_signature',
+                          'created_at',
+                          'description',
+                          'fccid',
+                          'height',
+                          'height_type',
+                          'id',
+                          'indoor_deployment',
+                          'latitude',
+                          'location',
+                          'longitude',
+                          'mac',
+                          'name',
+                          'network',
+                          'serial_number',
+                          'tdd_mode',
+                          'tx_power',
+                          'type',
+                          'updated_at',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_radio(self, id, **kwargs):
+        """
+        Returns information about a private cellular radio.
+        :param id: ID of the private_cellular_radios record
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: An individual Cellular AP with details.
+        """
+        call_type = 'Private Cellular Radios'
+        get_url = f'{self.base_url}/beta/private_cellular_radios/{id}'
+
+        allowed_params = ['admin_state',
+                          'antenna_azimuth',
+                          'antenna_beamwidth',
+                          'antenna_downtilt',
+                          'antenna_gain',
+                          'bandwidth',
+                          'category',
+                          'cpi_id',
+                          'cpi_name',
+                          'cpi_signature',
+                          'created_at',
+                          'description',
+                          'fccid',
+                          'height',
+                          'height_type',
+                          'id',
+                          'indoor_deployment',
+                          'latitude',
+                          'location',
+                          'longitude',
+                          'mac',
+                          'name',
+                          'network',
+                          'serial_number',
+                          'tdd_mode',
+                          'tx_power',
+                          'type',
+                          'updated_at',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def update_private_cellular_radio(self, id=None, name=None, **kwargs):
+        """
+        Updates a Cellular AP's data.
+        :param id: ID of the private_cellular_radio record. Must specify this or name.
+        :type id: str
+        :param name: Name of the Cellular AP. Must specify this or id.
+        type id: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Update Cellular AP results.
+        """
+        call_type = 'Private Cellular Radio'
+
+        if id:
+            radio = self.get_private_cellular_radios(id=id)[0]
+        elif name:
+            radio = self.get_private_cellular_radios(name=name)[0]
+        else:
+            return "ERROR: Must specify either ID or name"
+
+        if name:
+            kwargs['name'] = name
+
+        put_url = f'{self.base_url}/beta/private_cellular_radios/{radio["id"]}'
+
+        if "network" in kwargs.keys():
+            relationships = {
+                "network": {
+                    "data": {
+                        "type": "private_cellular_networks",
+                        "id": kwargs['network']
+                    }
+                }
+            }
+            kwargs.pop("network")
+
+            radio['data']['relationships'] = relationships
+
+        if "location" in kwargs.keys():
+            location = {
+                "data": {
+                    "type": "private_cellular_radio_groups",
+                    "id": kwargs['location']
+                }
+            }
+            kwargs.pop("location")
+            radio['data']['location'] = location
+
+        allowed_params = ['admin_state',
+                          'antenna_azimuth',
+                          'antenna_beamwidth',
+                          'antenna_downtilt',
+                          'antenna_gain',
+                          'bandwidth',
+                          'category',
+                          'cpi_id',
+                          'cpi_name',
+                          'cpi_signature',
+                          'created_at',
+                          'description',
+                          'fccid',
+                          'height',
+                          'height_type',
+                          'id',
+                          'indoor_deployment',
+                          'latitude',
+                          'location',
+                          'longitude',
+                          'mac',
+                          'name',
+                          'network',
+                          'serial_number',
+                          'tdd_mode',
+                          'tx_power']
+        params = self.__parse_put_kwargs(kwargs, allowed_params)
+
+        for k, v in params.items():
+            radio['attributes'][k] = v
+
+        radio = {"data": radio}
+
+        ncm = self.session.put(put_url, data=json.dumps(radio))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def get_private_cellular_radio_groups(self, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of Cellular AP Groups with details.
+        """
+        call_type = 'Private Cellular Radio Groups'
+        get_url = f'{self.base_url}/beta/private_cellular_radio_groups'
+
+        allowed_params = ['created_at',
+                          'created_at__lt',
+                          'created_at__lte',
+                          'created_at__gt',
+                          'created_at__gte',
+                          'created_at__ne',
+                          'description',
+                          'id',
+                          'name',
+                          'network',
+                          'type',
+                          'updated_at',
+                          'updated_at__lt',
+                          'updated_at__lte',
+                          'updated_at__gt',
+                          'updated_at__gte',
+                          'updated_at__ne',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_radio_group(self, group_id, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param group_id: ID of the private_cellular_radio_groups record
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: An individual Cellular AP Group with details.
+        """
+        call_type = 'Private Cellular Radio Group'
+        get_url = f'{self.base_url}/beta/private_cellular_radio_groups/{group_id}'
+
+        allowed_params = ['created_at',
+                          'description',
+                          'id',
+                          'name',
+                          'network',
+                          'type',
+                          'updated_at',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def update_private_cellular_radio_group(self, id=None, name=None, **kwargs):
+        """
+        Updates a Radio Group.
+        :param id: ID of the private_cellular_radio_groups record. Must specify this or name.
+        :type id: str
+        :param name: Name of the Radio Group. Must specify this or id.
+        type name: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Update Cellular AP Group results.
+        """
+        call_type = 'Private Cellular Radio Group'
+
+        if id:
+            group = self.get_private_cellular_radio_groups(id=id)[0]
+        elif name:
+            group = self.get_private_cellular_radio_groups(name=name)[0]
+        else:
+            return "ERROR: Must specify either ID or name"
+
+        if name:
+            kwargs['name'] = name
+
+        put_url = f'{self.base_url}/beta/private_cellular_sims/{group["id"]}'
+
+        if "network" in kwargs.keys():
+            relationships = {
+                "network": {
+                    "data": {
+                        "type": "private_cellular_networks",
+                        "id": kwargs['network']
+                    }
+                }
+            }
+            kwargs.pop("network")
+
+            group['data']['relationships'] = relationships
+
+        allowed_params = ['name',
+                          'description']
+        params = self.__parse_put_kwargs(kwargs, allowed_params)
+
+        for k, v in params.items():
+            group['attributes'][k] = v
+
+        group = {"data": group}
+
+        ncm = self.session.put(put_url, data=json.dumps(group))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def create_private_cellular_radio_group(self, name, description, network=None):
+        """
+        Creates a Radio Group.
+        :param name: Name of the Radio Group.
+        type name: str
+        :param description: Description of the Radio Group.
+        :type description: str
+        param network: ID of the private_cellular_network to belong to. Optional.
+        :type network: str
+        :return: Create Private Cellular Radio Group results.
+        """
+        call_type = 'Private Cellular Radio Group'
+
+        post_url = f'{self.base_url}/beta/private_cellular_radio_groups'
+
+        group = {
+            "data": {
+                "type": "private_cellular_radio_groups",
+                "attributes": {
+                    "name": name,
+                    "description": description
+                }
+            }
+        }
+
+        if network:
+            relationships = {
+                "network": {
+                    "data": {
+                        "type": "private_cellular_networks",
+                        "id": network
+                    }
+                }
+            }
+
+            group['data']['relationships'] = relationships
+
+        ncm = self.session.post(post_url, data=json.dumps(group))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def delete_private_cellular_radio_group(self, id):
+        """
+        Deletes a private_cellular_radio_group record.
+        :param id: ID of the private_cellular_radio_group record
+        :type id: str
+        :return: None unless error.
+        """
+        #TODO support deletion by group name
+        call_type = 'Private Cellular Radio Group'
+        delete_url = f'{self.base_url}/beta/private_cellular_radio_group/{id}'
+
+        ncm = self.session.delete(delete_url)
+        result = self._return_handler(ncm.status_code, ncm.text, call_type)
+        return result
+
+    def get_private_cellular_sims(self, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of PCN SIMs with details.
+        """
+        call_type = 'Private Cellular SIMs'
+        get_url = f'{self.base_url}/beta/private_cellular_sims'
+
+        allowed_params = ['created_at',
+                          'created_at__lt',
+                          'created_at__lte',
+                          'created_at__gt',
+                          'created_at__gte',
+                          'created_at__ne',
+                          'iccid',
+                          'id',
+                          'imsi',
+                          'last_contact_at',
+                          'last_contact_at__lt',
+                          'last_contact_at__lte',
+                          'last_contact_at__gt',
+                          'last_contact_at__gte',
+                          'last_contact_at__ne',
+                          'name',
+                          'network',
+                          'state',
+                          'state_updated_at',
+                          'state_updated_at__lt',
+                          'state_updated_at__lte',
+                          'state_updated_at__gt',
+                          'state_updated_at__gte',
+                          'state_updated_at__ne',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_sim(self, id, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param sim_id: ID of the private_cellular_sims record
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: An individual PCN SIM with details.
+        """
+        call_type = 'Private Cellular SIMs'
+        get_url = f'{self.base_url}/beta/private_cellular_sims/{id}'
+
+        allowed_params = ['created_at',
+                          'iccid',
+                          'id',
+                          'imsi',
+                          'last_contact_at',
+                          'name',
+                          'network',
+                          'state',
+                          'state_updated_at',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def update_private_cellular_sim(self, id=None, iccid=None, imsi=None, **kwargs):
+        """
+        Updates a SIM's data.
+        :param id: ID of the private_cellular_sim record. Must specify ID, ICCID, or IMSI.
+        :type id: str
+        :param iccid: ICCID. Must specify ID, ICCID, or IMSI.
+        :type id: str
+        :param imsi: IMSI. Must specify ID, ICCID, or IMSI.
+        :type id: str
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Update PCN SIM results.
+        """
+        call_type = 'Private Cellular SIM'
+
+        if id:
+            sim = self.get_private_cellular_sims(id=id)[0]
+        elif iccid:
+            sim = self.get_private_cellular_sims(iccid=iccid)[0]
+        elif imsi:
+            sim = self.get_private_cellular_sims(imsi=imsi)[0]
+        else:
+            return "ERROR: Must specify either ID, ICCID, or IMSI"
+
+        put_url = f'{self.base_url}/beta/private_cellular_sims/{sim["id"]}'
+
+        if "network" in kwargs.keys():
+            relationships = {
+                "network": {
+                    "data": {
+                        "type": "private_cellular_networks",
+                        "id": kwargs['network']
+                    }
+                }
+            }
+            kwargs.pop("network")
+
+            sim['data']['relationships'] = relationships
+
+        allowed_params = ['name',
+                          'state']
+        params = self.__parse_put_kwargs(kwargs, allowed_params)
+
+        for k, v in params.items():
+            sim['attributes'][k] = v
+
+        sim = {"data": sim}
+
+        ncm = self.session.put(put_url, data=json.dumps(sim))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def get_private_cellular_radio_statuses(self, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Cellular radio status for all cellular radios.
+        """
+        call_type = 'Private Cellular Radio Statuses'
+        get_url = f'{self.base_url}/beta/private_cellular_radio_statuses'
+
+        allowed_params = ['admin_state',
+                          'boot_time',
+                          'cbrs_sas_status',
+                          'cell',
+                          'connected_ues',
+                          'ethernet_status',
+                          'id',
+                          'ipsec_status',
+                          'ipv4_address',
+                          'last_update_time',
+                          'online_status',
+                          'operational_status',
+                          'operating_tx_power',
+                          's1_status',
+                          'time_synchronization',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_private_cellular_radio_status(self, status_id, **kwargs):
+        """
+        Returns information about a private cellular core.
+        :param status_id: ID of the private_cellular_radio_statuses resource
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Cellular radio status for an individual radio.
+        """
+        call_type = 'Private Cellular Radio Status'
+        get_url = f'{self.base_url}/beta/private_cellular_radio_statuses/{status_id}'
+
+        allowed_params = ['admin_state',
+                          'boot_time',
+                          'cbrs_sas_status',
+                          'cell',
+                          'connected_ues',
+                          'ethernet_status',
+                          'id',
+                          'ipsec_status',
+                          'ipv4_address',
+                          'last_update_time',
+                          'online_status',
+                          'operational_status',
+                          'operating_tx_power',
+                          's1_status',
+                          'time_synchronization',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+
+    def get_public_sim_mgmt_assets(self, **kwargs):
+        """
+        Returns information about SIM asset resources in your NetCloud Manager account.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: SIM asset resources.
+        """
+        call_type = 'Private Cellular Radio Status'
+        get_url = f'{self.base_url}/beta/public_sim_mgmt_assets'
+
+        allowed_params = ['assigned_imei',
+                          'carrier',
+                          'detected_imei',
+                          'device_status',
+                          'iccid',
+                          'is_licensed'
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+    def get_public_sim_mgmt_rate_plans(self, **kwargs):
+        """
+        Returns information about rate plan resources associated with the SIM assets in your NetCloud Manager account.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: Rate plans for SIM assets.
+        """
+        call_type = 'Private Cellular Radio Status'
+        get_url = f'{self.base_url}/beta/public_sim_mgmt_assets'
+
+        allowed_params = ['carrier',
+                          'name',
+                          'status',
+                          'fields',
+                          'limit',
+                          'sort']
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        results = self.__get_json(get_url, call_type, params=params)
+        return results
+
+
+    def get_exchange_sites(self, **kwargs):
+        """
+        Returns exchange sites.
+        :param kwargs: A set of zero or more allowed parameters
+        in the allowed_params list.
+        :return: A list of exchange sites or a single site if site_id is provided.
+        """
+        call_type = 'Exchange Sites'
+        get_url = f'{self.base_url}/beta/exchange_sites'
+
+        if 'site_id' in kwargs:
+            get_url += f'/{kwargs["site_id"]}'
+            response = self.__get_json(get_url, call_type)
+            return response
+
+        allowed_params = ['exchange_network',
+                        'name',
+                        'fields',
+                        'limit',
+                        'sort']
+
+        params = None
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+
+        response = self.__get_json(get_url, call_type, params=params)
+        return response
+
+    def create_exchange_site(self, name, exchange_network_id, router_id, local_domain=None, primary_dns=None, secondary_dns=None, lan_as_dns=False):
+        """
+        Creates an exchange site.
+        :param name: Name of the exchange site.
+        :type name: str
+        :param primary_dns: Primary DNS of the exchange site.
+        :type primary_dns: str
+        :param secondary_dns: Secondary DNS of the exchange site.
+        :type secondary_dns: str
+        :param lan_as_dns: Whether LAN is used as DNS.
+        :type lan_as_dns: bool
+        :param local_domain: Local domain of the exchange site.
+        :type local_domain: str
+        :param exchange_network_id: ID of the exchange network.
+        :type exchange_network_id: str
+        :param router_id: ID of the endpoint.
+        :type router_id: str
+        :return: The response from the POST request.
+        """
+        call_type = 'Create Exchange Site'
+
+        post_url = f'{self.base_url}/beta/exchange_sites'
+
+        data = {
+            "data": {
+                "type": "exchange_user_managed_sites",
+                "attributes": {
+                    "name": name,
+                    "primary_dns": primary_dns,
+                    "secondary_dns": secondary_dns,
+                    "lan_as_dns": lan_as_dns,
+                    "local_domain": local_domain
+                },
+                "relationships": {
+                    "exchange_network": {
+                        "data": {
+                            "id": exchange_network_id,
+                            "type": "exchange_networks"
+                        }
+                    },
+                    "endpoints": {
+                        "data": [
+                            {
+                                "id": router_id,
+                                "type": "endpoints"
+                            }
+                        ]
+                    }
+                }
+            }
+        }
+
+        ncm = self.session.post(post_url, data=json.dumps(data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        if ncm.status_code == 201:
+            return ncm.json()['data']
+        else:
+            return result
+
+    def update_exchange_site(self, site_id, **kwargs):
+        """
+        Updates an exchange site.
+        :param site_id: ID of the exchange site to update.
+        :type site_id: str
+        :param kwargs: Keyword arguments for the attributes and relationships of the exchange site.
+        :return: The response from the PUT request.
+        """
+        call_type = 'Update Exchange Site'
+        put_url = f'{self.base_url}/beta/exchange_sites/{site_id}'
+
+        allowed_params = ['name', 'primary_dns', 'secondary_dns', 'lan_as_dns', 'local_domain']
+
+        current_site = self.get_exchange_sites(site_id=site_id)[0]
+        exchange_network_id = current_site['relationships']['exchange_network']['data']['id']
+        router_id = current_site['relationships']['endpoints']['data'][0]['id']
+        attributes = current_site['attributes']
+
+        for key, value in kwargs.items():
+            if key in allowed_params:
+                attributes['key'] = value
+
+        ncm = self.session.put(put_url, data=json.dumps({
+            "data": {
+                "type": "exchange_user_managed_sites",
+                "id": site_id,
+                "attributes": attributes,
+                "relationships": {
+                    "exchange_network": {
+                        "data": {
+                            "type": "exchange_networks",
+                            "id": exchange_network_id
+                        }
+                    },
+                    "endpoints": {
+                        "data": [{
+                            "type": "routers",
+                            "id": router_id
+                        }]
+                    }
+                }
+            }
+        }))
+
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def delete_exchange_site(self, site_id):
+        """
+        Deletes an exchange site.
+        :param site_id: ID of the exchange site to delete.
+        :type site_id: str
+        :return: The response from the DELETE request.
+        """
+        call_type = 'Delete Exchange Site'
+        delete_url = f'{self.base_url}/beta/exchange_sites{site_id}'
+
+        ncm = self.session.delete(delete_url)
+        result = self._return_handler(ncm.status_code, ncm, call_type)
+        return result
+
+    def get_exchange_resources(self, exchange_network=None, exchange_site=None, **kwargs):
+        """
+        Returns exchange sites.
+        :param kwargs: A set of zero or more allowed parameters
+        in the allowed_params list.
+        :return: A list of exchange sites or a single site if site_id is provided.
+        """
+        call_type = 'Exchange Resources'
+        get_url = f'{self.base_url}/beta/exchange_resources'
+
+        params = {}
+
+        allowed_params = ['exchange_network',
+                          'name',
+                          'id',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if kwargs:
+            if "search" not in kwargs.keys():
+                params = self.__parse_kwargs(kwargs, allowed_params)
+            else:
+                if kwargs['search']:
+                    params = self.__parse_search_kwargs(kwargs, allowed_params)
+                else:
+                    params = self.__parse_kwargs(kwargs, allowed_params)
+
+        if exchange_site:
+            params['filter[exchange_site]'] = exchange_site
+        elif exchange_network:
+            params['filter[exchange_network]'] = exchange_network
+
+        response = self.__get_json(get_url, call_type, params=params)
+        return response
+
+    def create_exchange_resource(self, site_id, resource_name, resource_type, **kwargs):
+        """
+        Creates an exchange site.
+        :param site_id: NCX Site ID to add the resource to.
+        :type site_id: str
+        :param resource_name: Name for the new resource
+        :type resource_type: str
+        :param resource_type: exchange_fqdn_resources, exchange_wildcard_fqdn_resources, or exchange_ipsubnet_resources
+        :type resource_type: str
+
+        :return: The response from the POST request.
+        """
+        call_type = 'Create Exchange Site Resource'
+
+        post_url = f'{self.base_url}/beta/exchange_resources'
+        allowed_params = ['name',
+                          'protocols',
+                          'tags',
+                          'domain',
+                          'ip',
+                          'static_prime_ip',
+                          'port_ranges',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        attributes = {key: value for key, value in kwargs.items() if key in allowed_params}
+        attributes['name'] = resource_name
+
+        data = {
+            "data": {
+                "type": resource_type,
+                "attributes": attributes,
+                "relationships": {
+                    "exchange_site": {
+                        "data": {
+                            "id": site_id,
+                            "type": "exchange_sites"
+                        }
+                    }
+                }
+            }
+        }
+
+        ncm = self.session.post(post_url, data=json.dumps(data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        if ncm.status_code == 201:
+            return ncm.json()['data']
+        else:
+            return result
+
+    def update_exchange_resource(self, resource_id, exchange_network=None, exchange_site=None, **kwargs):
+        """
+        Updates an exchange site.
+        :param resource_id: ID of the exchange resource to update.
+        :type resource_id: str
+        :param kwargs: Keyword arguments for the attributes and relationships of the exchange site.
+        :return: The response from the PUT request.
+        """
+        call_type = 'Update Exchange Site'
+        put_url = f'{self.base_url}/beta/exchange_resources/{resource_id}'
+
+        allowed_params = ['name',
+                          'protocols',
+                          'tags',
+                          'domain',
+                          'ip',
+                          'static_prime_ip',
+                          'port_ranges']
+
+        if exchange_site:
+            current_resource = self.get_exchange_resources(exchange_site=exchange_site, id=resource_id)[0]
+        elif exchange_network:
+            current_resource = self.get_exchange_resources(exchange_network=exchange_network, id=resource_id)[0]
+
+        exchange_site_id = current_resource['relationships']['exchange_site']['data']['id']
+        attributes = current_resource['attributes']
+
+        for key, value in kwargs.items():
+            if key in allowed_params:
+                attributes['key'] = value
+
+        ncm = self.session.put(put_url, data=json.dumps({
+            "data": {
+                "type": current_resource['type'],
+                "id": resource_id,
+                "attributes": attributes,
+                "relationships": {
+                    "exchange_site": {
+                        "data": {
+                            "type": "exchange_sites",
+                            "id": exchange_site_id
+                        }
+                    }
+                }
+            }
+        }))
+
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def delete_exchange_resource(self, resource_id):
+        """
+        Deletes an exchange resource.
+        :param resource_id: ID of the exchange resource to delete.
+        :type resource_id: str
+        :return: The response from the DELETE request.
+        """
+        call_type = 'Delete Exchange Site'
+        delete_url = f'{self.base_url}/beta/exchange_resources{resource_id}'
+
+        ncm = self.session.delete(delete_url)
+        result = self._return_handler(ncm.status_code, ncm, call_type)
+        return result
+
+'''
+    def get_group_modem_upgrade_jobs(self, **kwargs):
+        """
+        Returns users with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of users with details.
+        """
+        call_type = 'Group Modem Upgrades'
+        get_url = f'{self.base_url}/beta/group_modem_upgrade_jobs'
+
+        allowed_params = ['id',
+                          'group_id',
+                          'module_id',
+                          'carrier_id',
+                          'overwrite',
+                          'active_only',
+                          'upgrade_only',
+                          'batch_size',
+                          'created_at',
+                          'created_at__lt',
+                          'created_at__lte',
+                          'created_at__gt',
+                          'created_at__gte',
+                          'created_at__ne',
+                          'updated_at',
+                          'updated_at__lt',
+                          'updated_at__lte',
+                          'updated_at__gt',
+                          'updated_at__gte',
+                          'updated_at__ne',
+                          'available_version',
+                          'modem_count',
+                          'success_count',
+                          'failed_count',
+                          'statuscarrier_name',
+                          'module_name',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+
+    def get_group_modem_upgrade_job(self, job_id, **kwargs):
+        """
+        Returns users with details.
+        :param job_id: The ID of the job
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of users with details.
+        """
+        call_type = 'Group Modem Upgrades'
+        get_url = f'{self.base_url}/beta/group_modem_upgrade_jobs/{job_id}'
+
+        allowed_params = ['id',
+                          'group_id',
+                          'module_id',
+                          'carrier_id',
+                          'overwrite',
+                          'active_only',
+                          'upgrade_only',
+                          'batch_size',
+                          'created_at',
+                          'updated_at',
+                          'available_version',
+                          'modem_count',
+                          'success_count',
+                          'failed_count',
+                          'statuscarrier_name',
+                          'module_name',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+
+    def get_group_modem_upgrade_summary(self, **kwargs):
+        """
+        Returns users with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of users with details.
+        """
+        call_type = 'Group Modem Upgrades'
+        get_url = f'{self.base_url}/beta/group_modem_upgrade_jobs'
+
+        allowed_params = ['group_id',
+                          'module_id',
+                          'module_name',
+                          'upgradable_modems',
+                          'up_to_date_modems',
+                          'summary_data',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+
+    def get_group_modem_upgrade_device_summary(self, **kwargs):
+        """
+        Returns users with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of users with details.
+        """
+        call_type = 'Group Modem Upgrades'
+        get_url = f'{self.base_url}/beta/group_modem_upgrade_jobs'
+
+        allowed_params = ['group_id',
+                          'module_id',
+                          'carrier_id',
+                          'overwrite',
+                          'active_only',
+                          'upgrade_only',
+                          'router_name',
+                          'net_device_name',
+                          'current_version',
+                          'type',
+                          'fields',
+                          'limit',
+                          'sort']
+
+        if "search" not in kwargs.keys():
+            params = self.__parse_kwargs(kwargs, allowed_params)
+        else:
+            if kwargs['search']:
+                params = self.__parse_search_kwargs(kwargs, allowed_params)
+            else:
+                params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+'''
+
+class NcmClient:
+    """
+    This NCM Client class provides functions for interacting with =
+    the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
+    found at: https://developer.cradlepoint.com
+    """
+
+    def __init__(self, 
+              api_keys=None,
+              api_key=None,
+              log_events=True,
+              logger=None,
+              retries=5,
+              retry_backoff_factor=2,
+              retry_on=None,
+              base_url=None,
+              base_url_v3=None):
+        """
+        :param api_keys: Dictionary of API credentials (apiv2).
+            Optional, but must be set before calling functions.
+        :type api_keys: dict
+        :param api_key: API key for apiv3.
+            Optional, but must be set before calling functions.
+        :type api_key: str
+        """
+        api_keys = api_keys or {}
+        apiv3_key = api_keys.pop('token', None) or api_key
+        self.v2 = None
+        self.v3 = None
+        if api_keys:
+            self.v2 = NcmClientv2(api_keys=api_keys, 
+                                  log_events=log_events,
+                                  logger=logger,
+                                  retries=retries, 
+                                  retry_backoff_factor=retry_backoff_factor, 
+                                  retry_on=retry_on, 
+                                  base_url=base_url)
+        if apiv3_key:
+            base_url = base_url_v3 if api_keys else base_url
+            self.v3 = NcmClientv3(api_key=apiv3_key, 
+                                  log_events=log_events, 
+                                  logger=logger,
+                                  retries=retries, 
+                                  retry_backoff_factor=retry_backoff_factor, 
+                                  retry_on=retry_on, 
+                                  base_url=base_url)
+        
+    def __getattribute__(self, name):
+        try:
+            return super().__getattribute__(name)
+        except AttributeError:
+            # Prioritize v3 over v2
+            if self.v3 and hasattr(self.v3, name):
+                return getattr(self.v3, name)
+            if self.v2 and hasattr(self.v2, name):
+                return getattr(self.v2, name)
+            raise
```

### Comparing `ncm-0.0.28/ncm.egg-info/PKG-INFO` & `ncm-0.0.29/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.28
+Version: 0.0.29
 Summary: Python client library for Cradlepoint NCM API
-Home-page: https://github.com/nathanwiens/ncm
+Home-page: https://github.com/cradlepoint/api-samples/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 # Cradlepoint NCM SDK
-This is a Python client library for Cradlepoint NCM API
+This is a Python client library for Cradlepoint NCM API (both v2 and v3)
 
 INSTALL AND RUN INSTRUCTIONS
 
 1. Install the ncm pip package, or copy the ncm.py file into your working directory:
     ```
     pip3 install ncm
     ```
 
-2. Set NCM API Keys. API Keys must be passed as a dictionary:
+2. Set NCM API v2 Keys. API Keys must be passed as a dictionary:
     ```
     api_keys = {
         'X-CP-API-ID': 'aaaa',
         'X-CP-API-KEY': 'bbbb',
         'X-ECM-API-ID': 'cccc',
         'X-ECM-API-KEY': 'dddd'
     }
     ```
+    For API v3 Key it can be included in the same dictionary as token (optional):
+    ```
+    api_keys = {
+        'X-CP-API-ID': 'aaaa',
+        'X-CP-API-KEY': 'bbbb',
+        'X-ECM-API-ID': 'cccc',
+        'X-ECM-API-KEY': 'dddd',
+        "token": 'eeee'
+    }
+    ```
+    Note: if only using v3, just include the token in the dictionary.
 
 3. Import the module and create an instance of the NcmClient object:
    
    If using pip:
     ```
     from ncm import ncm
     n = ncm.NcmClient(api_keys=api_keys)
```

### Comparing `ncm-0.0.28/setup.py` & `ncm-0.0.29/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.28",
+    version="0.0.29",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/nathanwiens/ncm",
+    url="https://github.com/cradlepoint/api-samples/ncm",
     packages=find_packages(),
     python_requires='>=3.6',
     install_requires=[
         'requests',
         'urllib3'
     ]
 )
```

