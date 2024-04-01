# Comparing `tmp/xia-framework-0.0.8.tar.gz` & `tmp/xia-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-framework-0.0.8.tar", last modified: Sun Mar 31 16:56:29 2024, max compression
+gzip compressed data, was "xia-framework-0.0.9.tar", last modified: Sun Mar 31 17:09:48 2024, max compression
```

## Comparing `xia-framework-0.0.8.tar` & `xia-framework-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:56:29.603267 xia-framework-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 16:56:20.000000 xia-framework-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 16:56:29.000000 xia-framework-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-31 16:56:29.603267 xia-framework-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 16:56:20.000000 xia-framework-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 16:56:29.603267 xia-framework-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 16:56:20.000000 xia-framework-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:56:29.603267 xia-framework-0.0.8/xia_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-31 16:56:20.000000 xia-framework-0.0.8/xia_framework/realm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:56:29.603267 xia-framework-0.0.8/xia_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-31 16:56:29.000000 xia-framework-0.0.8/xia_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-31 16:56:29.000000 xia-framework-0.0.8/xia_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:56:29.000000 xia-framework-0.0.8/xia_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 16:56:29.000000 xia-framework-0.0.8/xia_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 16:56:29.000000 xia-framework-0.0.8/xia_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:09:48.429932 xia-framework-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 17:09:40.000000 xia-framework-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 17:09:48.000000 xia-framework-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-31 17:09:48.429932 xia-framework-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 17:09:40.000000 xia-framework-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 17:09:48.429932 xia-framework-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 17:09:40.000000 xia-framework-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:09:48.429932 xia-framework-0.0.9/xia_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-31 17:09:40.000000 xia-framework-0.0.9/xia_framework/realm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:09:48.429932 xia-framework-0.0.9/xia_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-31 17:09:48.000000 xia-framework-0.0.9/xia_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-31 17:09:48.000000 xia-framework-0.0.9/xia_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 17:09:48.000000 xia-framework-0.0.9/xia_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 17:09:48.000000 xia-framework-0.0.9/xia_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 17:09:48.000000 xia-framework-0.0.9/xia_framework.egg-info/top_level.txt
```

### Comparing `xia-framework-0.0.8/LICENSE` & `xia-framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-framework-0.0.8/setup.py` & `xia-framework-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xia-framework-0.0.8/xia_framework/application.py` & `xia-framework-0.0.9/xia_framework/application.py`

 * *Files identical despite different names*

### Comparing `xia-framework-0.0.8/xia_framework/cosmos.py` & `xia-framework-0.0.9/xia_framework/cosmos.py`

 * *Files identical despite different names*

### Comparing `xia-framework-0.0.8/xia_framework/foundation.py` & `xia-framework-0.0.9/xia_framework/foundation.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,28 +76,14 @@
         else:
             module_dict[module_name] = {"package": package, "class": module_class}
             print(f"Module {module_name} Registered")
 
         with open(self.module_yaml, 'w') as file:
             yaml.dump(module_dict, file, default_flow_style=False, sort_keys=False)
 
-    def update_requirements(self):
-        needed_packages = self.get_needed_packages()
-
-        requirements_content = "\n".join(needed_packages.values())
-        with open(self.requirements_txt, 'w') as file:
-            file.write(requirements_content)
-
-    def install_requirements(self):
-        with open(self.landscape_yaml, 'r') as file:
-            landscape_dict = yaml.safe_load(file) or {}
-        pip_index_url = landscape_dict["settings"].get("pip_index_url", "https://pypi.org/simple")
-        subprocess.run(['pip', 'install', '-r', self.requirements_txt,
-                        f"--index-url={pip_index_url}"], check=True)
-
     @classmethod
     def _fill_full_dependencies(cls, module_dict: dict):
         counter = 1  # Trigger the first iteration
         while counter > 0:
             counter = 0
             for module_name, module_config in module_dict.items():
                 for dependency in module_config["_dependencies"]:
```

### Comparing `xia-framework-0.0.8/xia_framework/framework.py` & `xia-framework-0.0.9/xia_framework/framework.py`

 * *Files 26% similar despite different names*

```diff
@@ -48,14 +48,28 @@
                     else:
                         package_address = f"git+https://{git_https_url}/{package_name}#egg={package_name}"
                 else:
                     package_address = f"{package_name}=={package_version}" if package_version else package_name
                 package_addresses[package_name] = package_address
         return package_addresses
 
+    def update_requirements(self):
+        needed_packages = self.get_needed_packages()
+
+        requirements_content = "\n".join(needed_packages.values())
+        with open(self.requirements_txt, 'w') as file:
+            file.write(requirements_content)
+
+    def install_requirements(self):
+        with open(self.landscape_yaml, 'r') as file:
+            landscape_dict = yaml.safe_load(file) or {}
+        pip_index_url = landscape_dict["settings"].get("pip_index_url", "https://pypi.org/simple")
+        subprocess.run(['pip', 'install', '-r', self.requirements_txt,
+                        f"--index-url={pip_index_url}"], check=True)
+
     def terraform_init(self, env: str):
         with open(self.landscape_yaml, 'r') as file:
             landscape_dict = yaml.safe_load(file) or {}
         current_settings = landscape_dict.get("settings", {})
         bucket_name = current_settings["cosmos_name"]
         # bucket_name = current_settings["realm_name"] + "_" + current_settings["foundation_name"]
         tf_init_cmd = (f'terraform -chdir=iac/environments/{env} init '
```

