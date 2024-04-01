# Comparing `tmp/helm-hawk-0.0.0.tar.gz` & `tmp/helm-hawk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helm-hawk-0.0.0.tar", last modified: Tue Mar 26 18:13:05 2024, max compression
+gzip compressed data, was "helm-hawk-0.0.1.tar", last modified: Mon Apr  1 12:20:27 2024, max compression
```

## Comparing `helm-hawk-0.0.0.tar` & `helm-hawk-0.0.1.tar`

### file list

```diff
@@ -1,48 +1,66 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.327029 helm-hawk-0.0.0/
--rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-03-26 18:13:05.327029 helm-hawk-0.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4168 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/diff/
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/diff/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/diff/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)      112 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/diff/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/diff/commands/diff_revision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1142 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/diff/commands/diff_upgrade.py
--rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/diff/diff.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/get/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/get/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/get/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/get/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      924 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/get/commands/get_values.py
--rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/get/get.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/history/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/history/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      682 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/history/history.py
--rw-r--r--   0 vsts      (1001) docker     (127)      850 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/rollback/
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/rollback/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/rollback/rollback.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/status/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/status/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1526 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/status/status.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/uninstall/
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/uninstall/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/uninstall/uninstall.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.323028 helm-hawk-0.0.0/cli/upgrade/
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/upgrade/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/upgrade/upgrade.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.327029 helm-hawk-0.0.0/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8822 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/utils/helm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1376 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/cli/utils/kubectl.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 18:13:05.327029 helm-hawk-0.0.0/helm_hawk.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      802 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-03-26 18:13:05.000000 helm-hawk-0.0.0/helm_hawk.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-03-26 18:13:05.327029 helm-hawk-0.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-03-26 18:12:51.000000 helm-hawk-0.0.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4168 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/diff/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/diff/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      112 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/diff_revision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1142 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/diff_upgrade.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/diff.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/get/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/get/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      924 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/commands/get_values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/get.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/history/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/history/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      682 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/history/history.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/list/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/list/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/list/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1114 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/pull/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/pull/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/pull/pull.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/repo/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/repo/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      142 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      369 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/remove.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/update.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1048 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/repo.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/rollback/
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/rollback/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/rollback/rollback.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/status/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/status/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1526 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/status/status.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/template/
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/template/template.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/uninstall/
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/uninstall/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/uninstall/uninstall.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/upgrade/
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/upgrade/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/upgrade/upgrade.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11955 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/helm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1376 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/kubectl.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/helm_hawk.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1103 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-01 12:20:27.914774 helm-hawk-0.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/setup.py
```

### Comparing `helm-hawk-0.0.0/PKG-INFO` & `helm-hawk-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helm-hawk
-Version: 0.0.0
+Version: 0.0.1
 Author: Ankit Singh
 Author-email: as8356047@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `helm-hawk-0.0.0/README.md` & `helm-hawk-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/diff/commands/diff_revision.py` & `helm-hawk-0.0.1/cli/diff/commands/diff_revision.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/diff/commands/diff_upgrade.py` & `helm-hawk-0.0.1/cli/diff/commands/diff_upgrade.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/get/commands/get_values.py` & `helm-hawk-0.0.1/cli/get/commands/get_values.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/history/history.py` & `helm-hawk-0.0.1/cli/history/history.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/rollback/rollback.py` & `helm-hawk-0.0.1/cli/rollback/rollback.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/status/status.py` & `helm-hawk-0.0.1/cli/status/status.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/uninstall/uninstall.py` & `helm-hawk-0.0.1/cli/uninstall/uninstall.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/upgrade/upgrade.py` & `helm-hawk-0.0.1/cli/upgrade/upgrade.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/cli/utils/helm.py` & `helm-hawk-0.0.1/cli/utils/helm.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,75 @@
     def extend_context_and_namespace(self,command:list)-> list:
             if self.context: 
                 command.extend([ "--kube-context" ,self.context])
             if  self.namespace: 
                 command.extend(["--namespace" ,self.namespace])
             return command
 
+    def helm_list(self,all,all_namespaces) -> str:
+        try: 
+            helm_list_command=["helm","ls"]
+            if all: helm_list_command.extend(["-a"])
+            if all_namespaces: helm_list_command.extend(["-A"])
+            helm_list_output=subprocess.run(helm_list_command,capture_output=True,text=True,check=True)
+            return helm_list_output.stdout
+        except subprocess.CalledProcessError as e:
+            return Fore.RED + e.stderr
+
+    def pull(self,chart_name,version,username,password,untar,repo,pass_credentials):
+        try:
+            helm_pull_command= ["helm", "pull",chart_name]
+            if version: helm_pull_command.extend( [ "--version", version])
+            if username and password: helm_pull_command.extend(['--username',username,'--password',password])
+            if untar : helm_pull_command.extend(['--untar'])
+            if repo: helm_pull_command.extend(['--repo',repo])
+            if pass_credentials: helm_pull_command.extend(['--pass-credentials'])
+
+            helm_pull_output=subprocess.run(helm_pull_command, capture_output=True, text=True,check=True)
+        
+            output=helm_pull_output.stderr if helm_pull_output.stderr else helm_pull_output.stdout
+            return output
+        except subprocess.CalledProcessError as e:
+            return Fore.RED + e.stderr
+
+    def repo_add(self,name,url,pass_credentials,username,password):
+        try:
+            helm_repo_add_command= ["helm","repo","add",name,url]
+            if username and password: helm_repo_add_command.extend(['--username',username,'--password',password])
+            if pass_credentials: helm_repo_add_command.extend(['--pass-credentials'])
+            helm_repo_add_output=subprocess.run(helm_repo_add_command,capture_output=True,text=True,check=True)
+
+            return helm_repo_add_output.stdout
+        except subprocess.CalledProcessError as e:
+            return Fore.RED + e.stderr
+    def repo_list(self,output):
+        try:
+            helm_repo_list_command=["helm","repo","list"]
+            if output: helm_repo_list_command.extend(['-o',output])
+            helm_repo_list_output=subprocess.run(helm_repo_list_command, capture_output=True,text=True,check=True)
+            return helm_repo_list_output.stdout
+        except subprocess.CalledProcessError as e:
+            return Fore.RED + e.stderr
+
+    def repo_update(self,repo):
+        try: 
+            helm_repo_update_command=["helm","repo","update",*repo]
+            helm_repo_update_output = subprocess.run(helm_repo_update_command,capture_output=True,text=True,check=True)
+            return helm_repo_update_output.stdout
+        except subprocess.CalledProcessError as e:
+            return  Fore.RED + e.stderr
+
+    def repo_remove(self,repo):
+        try: 
+            helm_repo_reomove_command=["helm","repo","remove",*repo]
+            helm_repo_remove_output = subprocess.run(helm_repo_reomove_command,capture_output=True,text=True,check=True)
+            return helm_repo_remove_output.stdout
+        except subprocess.CalledProcessError as e:
+            return  Fore.RED + e.stderr
+  
     def get_values(self,**kwargs):
         try:
             release_name=kwargs.get("release_name")
             revision=kwargs.get("revision")
             if not revision:
                 values_command = ["helm", "get" ,"values",release_name]
             else:
@@ -94,15 +155,15 @@
         try:
             value_files=self.parse_values_command(values)
             helm_template_command = ['helm', 'template', release_name, chart_path, *value_files]
             helm_template_command=self.extend_context_and_namespace(helm_template_command)
             helm_template_output = subprocess.run(helm_template_command, capture_output=True, text=True, check=True)
             return helm_template_output.stdout
         except subprocess.CalledProcessError as e:
-            print(e.stderr)
+            print(Fore.RED + e.stderr)
     
     def diff(self,release_name,chart_path,values)->str:
         '''This outputs your diff using kubectl'''
         try:
 
             kubectl=Kubectl(context=self.context,namespace=self.namespace)
             template=self.helm_template(release_name,chart_path,values)
```

### Comparing `helm-hawk-0.0.0/cli/utils/kubectl.py` & `helm-hawk-0.0.1/cli/utils/kubectl.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.0/helm_hawk.egg-info/PKG-INFO` & `helm-hawk-0.0.1/helm_hawk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helm-hawk
-Version: 0.0.0
+Version: 0.0.1
 Author: Ankit Singh
 Author-email: as8356047@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `helm-hawk-0.0.0/setup.py` & `helm-hawk-0.0.1/setup.py`

 * *Files identical despite different names*

