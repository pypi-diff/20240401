# Comparing `tmp/cooking_with_gas-0.0.1-py3-none-any.whl.zip` & `tmp/cooking_with_gas-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3645 bytes, number of entries: 7
+Zip file size: 4052 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-01 17:40 cooking_with_gas/__init__.py
--rw-rw-rw-  2.0 fat     1126 b- defN 24-Apr-01 19:17 cooking_with_gas/gas.py
--rw-rw-rw-  2.0 fat     1076 b- defN 24-Apr-01 19:17 cooking_with_gas-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1946 b- defN 24-Apr-01 19:17 cooking_with_gas-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 19:17 cooking_with_gas-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-01 19:17 cooking_with_gas-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      594 b- defN 24-Apr-01 19:17 cooking_with_gas-0.0.1.dist-info/RECORD
-7 files, 4873 bytes uncompressed, 2581 bytes compressed:  47.0%
+-rw-rw-rw-  2.0 fat     3040 b- defN 24-Apr-01 19:48 cooking_with_gas/gas.py
+-rw-rw-rw-  2.0 fat     1076 b- defN 24-Apr-01 19:52 cooking_with_gas-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1946 b- defN 24-Apr-01 19:52 cooking_with_gas-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 19:52 cooking_with_gas-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-01 19:52 cooking_with_gas-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      594 b- defN 24-Apr-01 19:52 cooking_with_gas-0.0.2.dist-info/RECORD
+7 files, 6787 bytes uncompressed, 2988 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cooking_with_gas/__init__.py
 Comment: 
 
 Filename: cooking_with_gas/gas.py
 Comment: 
 
-Filename: cooking_with_gas-0.0.1.dist-info/LICENSE
+Filename: cooking_with_gas-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: cooking_with_gas-0.0.1.dist-info/METADATA
+Filename: cooking_with_gas-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cooking_with_gas-0.0.1.dist-info/WHEEL
+Filename: cooking_with_gas-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cooking_with_gas-0.0.1.dist-info/top_level.txt
+Filename: cooking_with_gas-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cooking_with_gas-0.0.1.dist-info/RECORD
+Filename: cooking_with_gas-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cooking_with_gas/gas.py

```diff
@@ -1,36 +1,102 @@
 import requests
 
+"""
+This module provides a class for interacting with Google Apps Script projects
+deployed as web apps. The class provides methods for sending GET and POST
+requests to the web app URL.
+
+Dependencies:
+    - requests
+
+
+"""
+
 
 class Gas:
+    """
+    A class to interact with Google Apps Script deployments.
+
+    This class provides methods to make GET and POST requests to a specified
+    Google Apps Script deployment.
+
+    Attributes:
+        _deployment_id (str): The deployment ID of the Google Apps Script.
+    """
+
     def __init__(self, deployment_id: str):
+        """
+        Initializes the Gas object with a deployment ID.
+
+        Args:
+            deployment_id (str): The deployment ID of the Google Apps Script.
+
+        Raises:
+            TypeError: If the deployment_id is not a string.
+        """
 
         if not isinstance(deployment_id, str):
             raise TypeError("Deployment ID must be a string")
 
         self._deployment_id = deployment_id
 
     def get_deployment_id(self) -> str:
+        """
+        Returns the deployment ID.
+
+        Returns:
+            str: The deployment ID.
+        """
         return self._deployment_id
 
     def get_url(self) -> str:
+        """
+        Constructs and returns the URL for the Google Apps Script deployment.
+
+        Returns:
+            str: The URL to access the Google Apps Script deployment.
+        """
         return f"https://script.google.com/macros/s/{self._deployment_id}/exec"
 
     def post(self, params: dict = None, data: dict = None) -> dict:
+        """
+        Sends a POST request to the Google Apps Script deployment.
 
+        Args:
+            params (dict, optional): URL parameters to be sent with the request.
+            data (dict, optional): Data to be sent in the JSON body of the request.
+
+        Returns:
+            dict: The JSON response from the Google Apps Script deployment.
+
+        Raises:
+            HTTPError: If the request did not succeed.
+        """
         # Send a POST request to the Google Apps Script URL
         response = requests.post(self.get_url(), params=params, json=data)
 
         # Raise an exception if the response is not successful
         response.raise_for_status()
 
         # return the JSON response
         return response.json()
 
     def get(self, params: dict = None) -> dict:
+        """
+        Sends a GET request to the Google Apps Script deployment.
+
+        Args:
+            params (dict, optional): URL parameters to be sent with the request.
+
+        Returns:
+            dict: The JSON response from the Google Apps Script deployment.
+
+        Raises:
+            HTTPError: If the request did not succeed.
+        """
         # Send a GET request to the Google Apps Script URL
         response = requests.get(self.get_url(), params=params)
 
         # Raise an exception if the response is not successful
         response.raise_for_status()
 
         return response.json()
```

## Comparing `cooking_with_gas-0.0.1.dist-info/LICENSE` & `cooking_with_gas-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cooking_with_gas-0.0.1.dist-info/METADATA` & `cooking_with_gas-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cooking-with-gas
-Version: 0.0.1
-Summary: A simple package to make it easier to use the Google Apps Script API.
+Version: 0.0.2
+Summary: A simple wrapper to make it easier to use the Google Apps Script API.
 Author-email: Harry Boyd <hboyd255@gmail.com>
 License: Copyright 2024 Harry Boyd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
```

## Comparing `cooking_with_gas-0.0.1.dist-info/RECORD` & `cooking_with_gas-0.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cooking_with_gas/__init__.py,sha256=okcPDmeNkYdBjLCYQ8gWjj_pXrRd_xXhN3gLMmaMK3g,22
-cooking_with_gas/gas.py,sha256=whzUoW_meH3Ml3MpCdxaPFgjT6n86s7BJDLhBYQcwmA,1126
-cooking_with_gas-0.0.1.dist-info/LICENSE,sha256=2Qo_c2dDoG_1Nd2gqFy3G3RyO-_RFgIBbEq0CDDMYAc,1076
-cooking_with_gas-0.0.1.dist-info/METADATA,sha256=4D8230Rmk7kvU1DVQ8QorNNCFO5FccRPLt1qC5xIsTg,1946
-cooking_with_gas-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cooking_with_gas-0.0.1.dist-info/top_level.txt,sha256=A46IjWcQ4AkkvIXG2EjOsH6A2qYQ0Q2LS6wfhkBeWQg,17
-cooking_with_gas-0.0.1.dist-info/RECORD,,
+cooking_with_gas/gas.py,sha256=RhvLHbfCtn3FiXd92yMo622NOAAlqMQ98Wavp5uem8c,3040
+cooking_with_gas-0.0.2.dist-info/LICENSE,sha256=2Qo_c2dDoG_1Nd2gqFy3G3RyO-_RFgIBbEq0CDDMYAc,1076
+cooking_with_gas-0.0.2.dist-info/METADATA,sha256=smETuu74jUvbDfcIpWgU1d_eApI2AlbNCugXnz9-AS0,1946
+cooking_with_gas-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cooking_with_gas-0.0.2.dist-info/top_level.txt,sha256=A46IjWcQ4AkkvIXG2EjOsH6A2qYQ0Q2LS6wfhkBeWQg,17
+cooking_with_gas-0.0.2.dist-info/RECORD,,
```

