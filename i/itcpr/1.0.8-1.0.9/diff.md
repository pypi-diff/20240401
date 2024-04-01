# Comparing `tmp/itcpr-1.0.8.tar.gz` & `tmp/itcpr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itcpr-1.0.8.tar", last modified: Sun Feb 25 14:00:22 2024, max compression
+gzip compressed data, was "itcpr-1.0.9.tar", last modified: Mon Apr  1 11:55:32 2024, max compression
```

## Comparing `itcpr-1.0.8.tar` & `itcpr-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 14:00:22.569759 itcpr-1.0.8/
--rw-rw-rw-   0        0        0     1089 2021-10-13 04:00:06.000000 itcpr-1.0.8/LICENSE
--rw-rw-rw-   0        0        0        0 2021-10-13 04:00:06.000000 itcpr-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4323 2024-02-25 14:00:22.557482 itcpr-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3888 2024-02-20 04:00:10.000000 itcpr-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-02-25 14:00:22.569759 itcpr-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      703 2024-02-25 13:57:10.000000 itcpr-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-25 14:00:22.513393 itcpr-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-25 14:00:22.557482 itcpr-1.0.8/src/itcpr.egg-info/
--rw-rw-rw-   0        0        0     4323 2024-02-25 14:00:21.000000 itcpr-1.0.8/src/itcpr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-02-25 14:00:22.000000 itcpr-1.0.8/src/itcpr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 14:00:21.000000 itcpr-1.0.8/src/itcpr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-25 14:00:21.000000 itcpr-1.0.8/src/itcpr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7496 2024-02-25 13:57:00.000000 itcpr-1.0.8/src/spintronics.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:55:32.073324 itcpr-1.0.9/
+-rw-rw-rw-   0        0        0     1089 2021-10-13 04:00:06.000000 itcpr-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-10-13 04:00:06.000000 itcpr-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4323 2024-04-01 11:55:32.070325 itcpr-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3888 2024-02-20 04:00:10.000000 itcpr-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 11:55:32.073324 itcpr-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-04-01 11:54:36.000000 itcpr-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:55:31.991823 itcpr-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 11:55:32.067335 itcpr-1.0.9/src/itcpr.egg-info/
+-rw-rw-rw-   0        0        0     4323 2024-04-01 11:55:31.000000 itcpr-1.0.9/src/itcpr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-04-01 11:55:31.000000 itcpr-1.0.9/src/itcpr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 11:55:31.000000 itcpr-1.0.9/src/itcpr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 11:55:31.000000 itcpr-1.0.9/src/itcpr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7611 2024-04-01 11:54:19.000000 itcpr-1.0.9/src/spintronics.py
```

### Comparing `itcpr-1.0.8/LICENSE` & `itcpr-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `itcpr-1.0.8/PKG-INFO` & `itcpr-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itcpr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Your tools for ITCPR
 Home-page: https://github.com/ITCPR/itcpr-tools
 Author: Md. Abdus Sami Akanda
 Author-email: abdussamiakanda@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `itcpr-1.0.8/README.md` & `itcpr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `itcpr-1.0.8/setup.py` & `itcpr-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="itcpr",
-    version="1.0.8",
+    version="1.0.9",
     description="Your tools for ITCPR",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ITCPR/itcpr-tools",
     author="Md. Abdus Sami Akanda",
     author_email="abdussamiakanda@gmail.com",
     license="MIT",classifiers=[
```

### Comparing `itcpr-1.0.8/src/itcpr.egg-info/PKG-INFO` & `itcpr-1.0.9/src/itcpr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itcpr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Your tools for ITCPR
 Home-page: https://github.com/ITCPR/itcpr-tools
 Author: Md. Abdus Sami Akanda
 Author-email: abdussamiakanda@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `itcpr-1.0.8/src/spintronics.py` & `itcpr-1.0.9/src/spintronics.py`

 * *Files 7% similar despite different names*

```diff
@@ -162,22 +162,28 @@
                 file_path = os.path.join(root, file)
                 print(f"Deleting: {file_path}")
                 os.remove(file_path)  # Delete the file
                 deleted_files_count += 1
     
     print(f"Total .ovf files deleted: {deleted_files_count}")
 
+import subprocess
 
+def start_learing():
+    repo_urls = [
+        "https://github.com/ITCPR/learning.git",
+        "https://github.com/ITCPR/mumax3.git",
+        "https://github.com/ITCPR/python-codes.git"
+    ]
+    # Prompt the user for the third repository URL
+    third_repo_url = input("Please enter your name ID: ")
+    repo_urls.append("https://github.com/ITCPR/"+third_repo_url+".git")
     
-def help():
-    print("start() : builds necessary database for the package")
-    print("hello() : gets you started with the package")
-    print("about() : GRE basic informations")
-    print("new() : adds new word of GRE vocabulary")
-    print("meaning() : prints out the meaning of a given word")
-    print("set() : prints out all the words in a set")
-    print("flash() : flashcard of a set")
-    print("exam() : takes a random vocabulary quiz")
-    print("progress() : shows data about your preparation progress")
-    print("update() : updates database from the internet")
-    
+    for url in repo_urls:
+        try:
+            # Run the git clone command
+            subprocess.run(["git", "clone", url], check=True)
+            print(f"Successfully cloned {url}")
+        except subprocess.CalledProcessError as e:
+            print(f"Failed to clone {url}. Error: {e}")
+
```

