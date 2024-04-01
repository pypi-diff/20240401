# Comparing `tmp/loopia_update_ip-0.5.0.tar.gz` & `tmp/loopia_update_ip-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopia_update_ip-0.5.0.tar", last modified: Sun Mar 31 20:47:24 2024, max compression
+gzip compressed data, was "loopia_update_ip-0.5.1.tar", last modified: Mon Apr  1 19:14:31 2024, max compression
```

## Comparing `loopia_update_ip-0.5.0.tar` & `loopia_update_ip-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:47:24.796305 loopia_update_ip-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35171 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4346 2024-03-31 20:47:24.796305 loopia_update_ip-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3780 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:47:24.793305 loopia_update_ip-0.5.0/loopia_update_ip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:47:24.795305 loopia_update_ip-0.5.0/loopia_update_ip/lib/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/ExternalIPMonitor.py
--rw-rw-rw-   0 root         (0) root         (0)    18168 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/LoopiaAPI.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/Mailer.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/StreamToLogger.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/lib/get_external_ip.py
--rw-rw-rw-   0 root         (0) root         (0)     9510 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/loopia_update_ip/loopia_update_ip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:47:24.794305 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4346 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-31 20:47:24.000000 loopia_update_ip-0.5.0/loopia_update_ip.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 20:47:24.796305 loopia_update_ip-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-31 20:47:14.000000 loopia_update_ip-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:14:31.610538 loopia_update_ip-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35171 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4346 2024-04-01 19:14:31.610538 loopia_update_ip-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:14:31.608538 loopia_update_ip-0.5.1/loopia_update_ip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:14:31.610538 loopia_update_ip-0.5.1/loopia_update_ip/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/ExternalIPMonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18595 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/LoopiaAPI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/Mailer.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/StreamToLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/lib/get_external_ip.py
+-rw-rw-rw-   0 root         (0) root         (0)     9510 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/loopia_update_ip/loopia_update_ip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:14:31.609538 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4346 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-01 19:14:31.000000 loopia_update_ip-0.5.1/loopia_update_ip.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 19:14:31.610538 loopia_update_ip-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-01 19:14:21.000000 loopia_update_ip-0.5.1/setup.py
```

### Comparing `loopia_update_ip-0.5.0/LICENSE` & `loopia_update_ip-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loopia_update_ip-0.5.0/PKG-INFO` & `loopia_update_ip-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopia_update_ip
-Version: 0.5.0
+Version: 0.5.1
 Summary: Application to keep DNS records updated when external IP-address change using the Loopia-API for the domain provider Loopia
 Home-page: https://gitlab.com/loopia-update-ip
 Author: Niklas Melin
 Author-email: niklasme@pm.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loopia_update_ip-0.5.0/README.md` & `loopia_update_ip-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `loopia_update_ip-0.5.0/loopia_update_ip/lib/LoopiaAPI.py` & `loopia_update_ip-0.5.1/loopia_update_ip/lib/LoopiaAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,34 +358,44 @@
             if not response == 'OK':
                 print(f' ERROR: Subdomain {subdomain} could not be created for domain {self.domain}\n'
                       f' \t API-endpoint error: {response}')
                 return "ERROR"
             # Since just defined, no zone record exist!
             subdomain_records = []
 
-        if len(subdomain_records) >= 2:
-            print(' ERROR: Multiple DNS records defined which is not supported')
-            return ' ERROR: Multiple DNS records defined which is not supported'
+        # Check if an A-record exists
+        a_record = list()
+        if len(subdomain_records) >= 1:
+            # Loop through records and check if a record matches type A
+            for record in subdomain_records:
+                if record['type'] == 'A':
+                    a_record.append(record)
 
-        elif len(subdomain_records) == 1:
+        # Check if multiple A-records has been defined
+        if len(a_record) > 1:
+            print(' ERROR: Multiple A-records defined which is not supported, update canceled')
+            return ' ERROR: Multiple A-records defined which is not supported'
+
+        if len(a_record) == 1:
             # Replace IP address in zone record
             subdomain_record = subdomain_records[0]
             subdomain_record['rdata'] = ip
 
             # Update zone record with new IP address
             try:
                 response = self.client.updateZoneRecord(self.username,
                                                         self.password,
                                                         self.domain,
                                                         subdomain,
                                                         subdomain_record)
             except xmlrpc.client.Fault as error_msg:
                 return error_msg.faultString
 
-        elif len(subdomain_records) == 0:
+        # If now A-record exist, create a new one
+        elif len(subdomain_records) == 0 or len(a_record) == 0:
             subdomain_record = self.create_record_dict('A', ttl, 0, ip, 0)
 
             # Create zone record with IP address
             try:
                 response = self.client.addZoneRecord(self.username,
                                                      self.password,
                                                      self.domain,
```

### Comparing `loopia_update_ip-0.5.0/loopia_update_ip/lib/Mailer.py` & `loopia_update_ip-0.5.1/loopia_update_ip/lib/Mailer.py`

 * *Files identical despite different names*

### Comparing `loopia_update_ip-0.5.0/loopia_update_ip/loopia_update_ip.py` & `loopia_update_ip-0.5.1/loopia_update_ip/loopia_update_ip.py`

 * *Files identical despite different names*

### Comparing `loopia_update_ip-0.5.0/loopia_update_ip.egg-info/PKG-INFO` & `loopia_update_ip-0.5.1/loopia_update_ip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopia-update-ip
-Version: 0.5.0
+Version: 0.5.1
 Summary: Application to keep DNS records updated when external IP-address change using the Loopia-API for the domain provider Loopia
 Home-page: https://gitlab.com/loopia-update-ip
 Author: Niklas Melin
 Author-email: niklasme@pm.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loopia_update_ip-0.5.0/loopia_update_ip.egg-info/SOURCES.txt` & `loopia_update_ip-0.5.1/loopia_update_ip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopia_update_ip-0.5.0/setup.py` & `loopia_update_ip-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="loopia_update_ip",
-    version="0.5.0",
+    version="0.5.1",
     author="Niklas Melin",
     author_email="niklasme@pm.me",
     description="Application to keep DNS records updated when external "
                 "IP-address change using the Loopia-API for the domain provider Loopia",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/loopia-update-ip",
```

