# Comparing `tmp/litio-1.5.2.tar.gz` & `tmp/litio-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litio-1.5.2.tar", last modified: Wed Jan 10 17:42:11 2024, max compression
+gzip compressed data, was "litio-1.6.0.tar", last modified: Mon Apr  1 18:45:15 2024, max compression
```

## Comparing `litio-1.5.2.tar` & `litio-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.339559 litio-1.5.2/
--rw-r--r--   0 lizard    (1000) lizard    (1000)    35149 2023-11-22 01:38:02.000000 litio-1.5.2/LICENSE
--rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-01-10 17:42:11.336225 litio-1.5.2/PKG-INFO
--rw-r--r--   0 lizard    (1000) lizard    (1000)     8664 2023-12-06 04:50:28.000000 litio-1.5.2/README.md
--rw-r--r--   0 lizard    (1000) lizard    (1000)       38 2024-01-10 17:42:11.339559 litio-1.5.2/setup.cfg
--rw-r--r--   0 lizard    (1000) lizard    (1000)     1299 2024-01-10 17:40:10.000000 litio-1.5.2/setup.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.312892 litio-1.5.2/src/
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.319559 litio-1.5.2/src/litio/
--rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-22 01:38:02.000000 litio-1.5.2/src/litio/__init__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)       48 2023-11-22 01:38:02.000000 litio-1.5.2/src/litio/__main__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     1942 2024-01-10 17:39:41.000000 litio-1.5.2/src/litio/litio.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.332892 litio-1.5.2/src/litio/utils/
--rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-28 17:23:46.000000 litio-1.5.2/src/litio/utils/__init__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     4555 2023-12-05 21:12:45.000000 litio-1.5.2/src/litio/utils/ai.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)       21 2024-01-10 17:40:03.000000 litio-1.5.2/src/litio/utils/info.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     5989 2023-12-05 21:12:45.000000 litio-1.5.2/src/litio/utils/litio.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     6001 2024-01-10 17:40:56.000000 litio-1.5.2/src/litio/utils/modules.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     4892 2023-12-05 21:12:45.000000 litio-1.5.2/src/litio/utils/output.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     6860 2023-12-05 21:12:45.000000 litio-1.5.2/src/litio/utils/tester.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     2559 2023-12-05 21:12:45.000000 litio-1.5.2/src/litio/utils/utils.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.336225 litio-1.5.2/src/litio.egg-info/
--rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/PKG-INFO
--rw-r--r--   0 lizard    (1000) lizard    (1000)      523 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/SOURCES.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)        1 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/dependency_links.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)       46 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/entry_points.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)       80 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/requires.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)        6 2024-01-10 17:42:11.000000 litio-1.5.2/src/litio.egg-info/top_level.txt
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-01-10 17:42:11.336225 litio-1.5.2/tests/
--rw-r--r--   0 lizard    (1000) lizard    (1000)      680 2023-11-30 21:17:37.000000 litio-1.5.2/tests/test1.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)      235 2023-11-28 19:46:57.000000 litio-1.5.2/tests/tests2.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.712181 litio-1.6.0/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)    35149 2023-11-22 01:38:02.000000 litio-1.6.0/LICENSE
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-01 18:45:15.708847 litio-1.6.0/PKG-INFO
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     8664 2023-12-06 04:50:28.000000 litio-1.6.0/README.md
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       38 2024-04-01 18:45:15.712181 litio-1.6.0/setup.cfg
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     1299 2024-04-01 18:27:55.000000 litio-1.6.0/setup.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.652181 litio-1.6.0/src/
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.675514 litio-1.6.0/src/litio/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-22 01:38:02.000000 litio-1.6.0/src/litio/__init__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       48 2023-11-22 01:38:02.000000 litio-1.6.0/src/litio/__main__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     1967 2024-04-01 18:44:03.000000 litio-1.6.0/src/litio/litio.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.702181 litio-1.6.0/src/litio/utils/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-28 17:23:46.000000 litio-1.6.0/src/litio/utils/__init__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     4555 2024-04-01 02:55:37.000000 litio-1.6.0/src/litio/utils/ai.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       21 2024-04-01 18:27:47.000000 litio-1.6.0/src/litio/utils/info.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     5931 2024-04-01 18:21:43.000000 litio-1.6.0/src/litio/utils/litio.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     8335 2024-04-01 18:15:08.000000 litio-1.6.0/src/litio/utils/modules.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     4892 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/output.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     6860 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/tester.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     2559 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/utils.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.705514 litio-1.6.0/src/litio.egg-info/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/PKG-INFO
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      523 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/SOURCES.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        1 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/dependency_links.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       46 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/entry_points.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       80 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/requires.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        6 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/top_level.txt
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.705514 litio-1.6.0/tests/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      680 2023-11-30 21:17:37.000000 litio-1.6.0/tests/test1.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      235 2023-11-28 19:46:57.000000 litio-1.6.0/tests/tests2.py
```

### Comparing `litio-1.5.2/LICENSE` & `litio-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/PKG-INFO` & `litio-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litio
-Version: 1.5.2
+Version: 1.6.0
 Summary: A simple tool for testing
 Home-page: https://github.com/lizardwine/litio
 Author: Lizardwine
 Author-email: lizardwine@hotmail.com
 License: GPL v3.0
 Project-URL: Bug Tracker, https://github.com/lizardwine/litio/issues
 Keywords: testing,tester
```

### Comparing `litio-1.5.2/README.md` & `litio-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/setup.py` & `litio-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/lizardwine/litio',
     project_urls={
         "Bug Tracker": "https://github.com/lizardwine/litio/issues",
     },
     license='GPL v3.0',
-    version='1.5.2',
+    version='1.6.0',
     keywords=['testing', 'tester'],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
```

### Comparing `litio-1.5.2/src/litio/litio.py` & `litio-1.6.0/src/litio/litio.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,20 @@
     from utils import modules, info
 except ModuleNotFoundError:
     from .utils import modules, info
 
 
 def litio():
     parser = argparse.ArgumentParser(description='A command line function tester')
-    if not os.path.exists('./litio.yml'):
-        print(f"Litio v{info.__version__}")
-        print("No config file 'litio.yml' found")
-        exit(1)
-    
-    data = open('./litio.yml', "r").read()
-    data = yaml.safe_load(data)
+    data = {
+        'safe-mode': False
+    }
+    if os.path.exists('./litio.yml'):
+        data = open('./litio.yml', "r").read()
+        data = yaml.safe_load(data)
     
     modules_info = modules.load_modules(data.get('safe-mode'))
     def get_module(module_name, info=False):
         if info:
             return modules_info[module_name]
         return modules_info['utils']['Kwargs'](**modules_info[module_name])
     
@@ -40,12 +39,15 @@
             if option.get('aliases'):
                 option.pop('aliases')
             option.pop('option')
             sub_parser.add_argument(*flags_or_name, **option)
         sub_parser.set_defaults(func=sub_command['controller'])
     
     args = parser.parse_args()
+    if args.__dict__.get('func') is None:
+        parser.print_help()
+        exit(0)    
     args.func(args, get_module)
     exit(0)
 
 if __name__ == '__main__':
     litio()
```

### Comparing `litio-1.5.2/src/litio/utils/ai.py` & `litio-1.6.0/src/litio/utils/ai.py`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/src/litio/utils/litio.py` & `litio-1.6.0/src/litio/utils/litio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import rich, yaml, os
 
 def run(args, get_module):
     if not os.path.exists('litio.yml'):
-        rich.print(f"[bold red]Config file \"[bold yellow]litio.yml[/bold yellow]\" does not exist[/bold red]")
+        print("❌ No config file 'litio.yml' found")
         exit(1)
     data = open('./litio.yml','r').read()
     data = yaml.safe_load(data)
     tests_output_args = get_module('utils').OutputArgs(title=data["name"])
     for test, test_data in data["tests"].items():
         path = test_data['path']
         tests_output_args.add_group({
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litio-1.5.2/src/litio/utils/modules.py` & `litio-1.6.0/src/litio/utils/modules.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 import os, argparse, importlib, subprocess
 from git import Repo
-
+import json
 from . import litio, info, output, utils, tester, ai
+import tarfile
+
 
+def uncompress(source, dest):
+    with tarfile.open(source, "r:gz") as tar:
+        tar.extractall(path=dest)
 
 def purge_dir(dir):
     if not os.path.exists(dir):
         return
     for f in os.listdir(dir):
         if os.path.isdir(os.path.join(dir, f)):
             purge_dir(os.path.join(dir, f))
             os.rmdir(os.path.join(dir, f))
         else:
             os.remove(os.path.join(dir, f))
 
+def prepare_for_install():
+    if not os.path.exists(f'./litio'):
+        os.mkdir(f'./litio')
+    if not os.path.exists(f'./litio/modules'):
+        os.mkdir(f'./litio/modules')
+    if not os.path.exists(f'./litio/modules/.dev'):
+        os.mkdir(f'./litio/modules/.dev')
+
 def install_module(args, get_module):
     module = args.module
     version = None
+    if module.endswith('.tar.gz'):
+        prepare_for_install()
+        name = ".".join(module.split(".")[:-2])
+        name = name.split("/")[-1]
+        print("Installing module from tarball")
+        uncompress(module, f'./litio/modules/.dev/{name}')
+        print(f"Module {name} installed successfully")
+        return
+        
     if '@' in module:
         module, version = module.split('@')
-    if not os.path.exists(f'./litio'):
-        os.mkdir(f'./litio')
-    if not os.path.exists(f'./litio/modules'):
-        os.mkdir(f'./litio/modules')
+    prepare_for_install()
     if args.upgrade and os.path.exists(f'./litio/modules/{module}'):
         purge_dir(f'./litio/modules/{module}')
         os.rmdir(f'./litio/modules/{module}')
     if os.path.exists(f'./litio/modules/{module}'):
         print(f"Module {module} already installed")
         return
     if not os.path.exists(f'./litio/modules/{module.split("/")[0]}'):
@@ -59,24 +78,60 @@
         print(f"Module {args.module} not installed")
         return
     
     purge_dir(f'./litio/modules/{args.module}')
     os.rmdir(f'./litio/modules/{args.module}')
     print(f"Module {args.module} removed successfully")
 
+def pack_module(args, get_module):
+    required_files = ["litio.py", "litio.json"]
+    for file in required_files:
+        if not os.path.exists(file):
+            print(f"Required file {file} not found")
+            return
+    ignore = ["dist"]
+    if os.path.exists('./.litioignore'):
+        ignore += open('./.litioignore', 'r').read().splitlines()
+    package_data = json.load(open('./litio.json', 'r'))
+    if not package_data.get('name'):
+        print('Missing name in litio.json')
+        return
+    if not package_data.get('version'):
+        print('Missing version in litio.json')
+        return
+    if not os.path.exists('./dist/'):
+        os.mkdir('./dist/')
+    else:
+        purge_dir('./dist/')
+    tar = tarfile.open(f'./dist/{package_data["name"]}-{package_data["version"]}.tar.gz', 'w:gz')
+    for file in os.listdir('./'):
+        if file in ignore and not file in required_files:
+            continue
+        tar.add(file)
+    tar.close()
+    print("Module packed successfully")
+
 options = {
     'version': {
         'option': '--version',
         'aliases': ['-v'],
         'action': 'version',
         'version':'%(prog)s v{}'.format(info.__version__)
     }
 }
 
 sub_commands = {
+    'pack': {
+        'command': 'pack',
+        'help': 'pack a litio module',
+        'controller': pack_module,
+        'options': {
+            
+        }
+    },
     'run': {
         'command': 'run',
         'help': 'run a litio test',
         'controller': litio.run,
         'options': {
             'verbose': {
                 'option': '--verbose',
@@ -168,17 +223,27 @@
         'fix_bug': ai.fix_bug
         
     }
 }
 def load_modules(safe_mode):
     if not os.path.exists('./litio/modules') or safe_mode:
         return modules_info
-    for author in os.listdir(f'./litio/modules'):
+    modules = os.listdir(f'./litio/modules')
+    modules = [module for module in modules if module != ".dev"]
+    for author in modules:
         for module in os.listdir(f'./litio/modules/{author}'):
             if not os.path.exists(f'./litio/modules/{author}/{module}/litio.py'):
                 continue
             spec = importlib.util.spec_from_file_location(f'{author}-{module}', f'./litio/modules/{author}/{module}/litio.py')
             modulelib = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(modulelib)
             for key, value in modulelib.litio.items():
                 modules_info[key].update(value)
+    for module in os.listdir('./litio/modules/.dev'):
+        if not os.path.exists(f'./litio/modules/.dev/{module}/litio.py'):
+            continue
+        spec = importlib.util.spec_from_file_location(f'.dev-{module}', f'./litio/modules/.dev/{module}/litio.py')
+        modulelib = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(modulelib)
+        for key, value in modulelib.litio.items():
+            modules_info[key].update(value)
     return modules_info
```

### Comparing `litio-1.5.2/src/litio/utils/output.py` & `litio-1.6.0/src/litio/utils/output.py`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/src/litio/utils/tester.py` & `litio-1.6.0/src/litio/utils/tester.py`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/src/litio/utils/utils.py` & `litio-1.6.0/src/litio/utils/utils.py`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/src/litio.egg-info/PKG-INFO` & `litio-1.6.0/src/litio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litio
-Version: 1.5.2
+Version: 1.6.0
 Summary: A simple tool for testing
 Home-page: https://github.com/lizardwine/litio
 Author: Lizardwine
 Author-email: lizardwine@hotmail.com
 License: GPL v3.0
 Project-URL: Bug Tracker, https://github.com/lizardwine/litio/issues
 Keywords: testing,tester
```

### Comparing `litio-1.5.2/src/litio.egg-info/SOURCES.txt` & `litio-1.6.0/src/litio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litio-1.5.2/tests/test1.py` & `litio-1.6.0/tests/test1.py`

 * *Files identical despite different names*

