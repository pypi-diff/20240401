# Comparing `tmp/ollama_downloads-0.1.0.tar.gz` & `tmp/ollama_downloads-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_downloads-0.1.0.tar", max compression
+gzip compressed data, was "ollama_downloads-0.1.1.tar", max compression
```

## Comparing `ollama_downloads-0.1.0.tar` & `ollama_downloads-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-03-27 21:11:16.291574 ollama_downloads-0.1.0/LICENSE
--rw-r--r--   0        0        0      716 2024-03-30 16:37:59.617465 ollama_downloads-0.1.0/README.md
--rw-r--r--   0        0        0      496 2024-03-30 17:20:11.548719 ollama_downloads-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 19:16:18.538261 ollama_downloads-0.1.0/src/ollama_downloads/__init__.py
--rw-r--r--   0        0        0     4309 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_all.txt
--rw-r--r--   0        0        0     6400 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_all_downloaded.txt
--rw-r--r--   0        0        0      996 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_big.txt
--rw-r--r--   0        0        0     1099 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_codes.txt
--rw-r--r--   0        0        0      393 2024-03-30 04:37:32.711660 ollama_downloads-0.1.0/src/ollama_downloads/models/models_few.txt
--rw-r--r--   0        0        0      103 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_math.txt
--rw-r--r--   0        0        0      102 2024-03-30 16:45:53.862099 ollama_downloads-0.1.0/src/ollama_downloads/models/models_one.txt
--rw-r--r--   0        0        0      201 2024-03-30 16:47:39.437394 ollama_downloads-0.1.0/src/ollama_downloads/models/models_sql.txt
--rwxr-xr-x   0        0        0     9530 2024-03-30 04:17:18.010618 ollama_downloads-0.1.0/src/ollama_downloads/ollama_downloads_process.py
--rwxr-xr-x   0        0        0     8685 2024-03-30 02:25:52.565254 ollama_downloads-0.1.0/src/ollama_downloads/ollama_downloads_process.py.1
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 ollama_downloads-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-27 21:11:16.291574 ollama_downloads-0.1.1/LICENSE
+-rw-r--r--   0        0        0      716 2024-03-30 16:37:59.617465 ollama_downloads-0.1.1/README.md
+-rw-r--r--   0        0        0      981 2024-04-01 21:48:44.255748 ollama_downloads-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-27 19:16:18.538261 ollama_downloads-0.1.1/src/ollama_downloads/__init__.py
+-rwxr-xr-x   0        0        0     9763 2024-04-01 21:41:13.183990 ollama_downloads-0.1.1/src/ollama_downloads/ollama_downloads_process.py
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 ollama_downloads-0.1.1/PKG-INFO
```

### Comparing `ollama_downloads-0.1.0/LICENSE` & `ollama_downloads-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_downloads-0.1.0/README.md` & `ollama_downloads-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ollama_downloads-0.1.0/src/ollama_downloads/ollama_downloads_process.py` & `ollama_downloads-0.1.1/src/ollama_downloads/ollama_downloads_process.py`

 * *Files 15% similar despite different names*

```diff
@@ -176,28 +176,33 @@
         for fname in ["models_all_downloaded.txt", "models_big.txt", "models_all.txt", "models_codes.txt", "models_sql.txt", "models_math.txt",]:
             self._load_file(fname)
 
     @clock
     def _save_file(self, fname, fdata):
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
         dirpath = os.path.dirname(os.path.abspath(__file__))
-        print(f"{name_} dirpath {dirpath}")
+        # Package root is located at 2 levels up
+        dirpath = os.path.join(dirpath, "../..")
         fname = os.path.join(dirpath, self.options["models_dir"], fname)
         print(f"{name_} fname {fname}")
+        print(f"{name_} fname {fname}")
         with open(fname, "w") as fp:
             json.dump(fdata, fp, indent=4)
 
     @clock
     def _load_file(self, fname):
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
         print(f"{name_} fname {fname}")
         dirpath = os.path.dirname(os.path.abspath(__file__))
+        # Package root is located at 2 levels up
+        dirpath = os.path.join(dirpath, "../..")
         print(f"{name_} dirpath {dirpath}")
         fname = os.path.join(dirpath, self.options["models_dir"], fname)
         print(f"{name_} fname {fname}")
+        print(f"{name_} fname {fname}")
         with open(fname, "r") as fp:
             data = json.load(fp)
             printit(f"{fname} data", data)
             printit(f"{fname} data type", type(data))
 
 
 def Options():
@@ -211,8 +216,8 @@
     return args
 
 
 if __name__ == "__main__":
     options = Options()
     printit("options", options)
     ollama_models = OllamaModels(options)
-    ollama_models.download_models()
+    ollama_models.download_models()
```

### Comparing `ollama_downloads-0.1.0/PKG-INFO` & `ollama_downloads-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-downloads
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Kenneth Wong
 Author-email: kennethwork101@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

