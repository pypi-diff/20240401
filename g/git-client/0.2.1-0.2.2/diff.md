# Comparing `tmp/git-client-0.2.1.tar.gz` & `tmp/git-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-client-0.2.1.tar", last modified: Mon Jan 13 20:13:55 2020, max compression
+gzip compressed data, was "git-client-0.2.2.tar", last modified: Mon Apr  1 16:39:54 2024, max compression
```

## Comparing `git-client-0.2.1.tar` & `git-client-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 neolaura   (501) staff       (20)        0 2020-01-13 20:13:55.000000 git-client-0.2.1/
--rw-r--r--   0 neolaura   (501) staff       (20)     1552 2020-01-13 20:13:55.000000 git-client-0.2.1/PKG-INFO
--rw-r--r--   0 neolaura   (501) staff       (20)      939 2019-08-16 22:20:22.000000 git-client-0.2.1/README.md
-drwxr-xr-x   0 neolaura   (501) staff       (20)        0 2020-01-13 20:13:55.000000 git-client-0.2.1/git_client.egg-info/
--rw-r--r--   0 neolaura   (501) staff       (20)     1552 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/PKG-INFO
--rw-r--r--   0 neolaura   (501) staff       (20)      284 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/SOURCES.txt
--rw-r--r--   0 neolaura   (501) staff       (20)        1 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/dependency_links.txt
--rw-r--r--   0 neolaura   (501) staff       (20)       44 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/entry_points.txt
--rw-r--r--   0 neolaura   (501) staff       (20)       40 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/requires.txt
--rw-r--r--   0 neolaura   (501) staff       (20)       10 2020-01-13 20:13:54.000000 git-client-0.2.1/git_client.egg-info/top_level.txt
-drwxr-xr-x   0 neolaura   (501) staff       (20)        0 2020-01-13 20:13:55.000000 git-client-0.2.1/gitclient/
--rw-r--r--   0 neolaura   (501) staff       (20)        0 2019-07-29 15:29:57.000000 git-client-0.2.1/gitclient/__init__.py
--rwxr-xr-x   0 neolaura   (501) staff       (20)     3330 2019-08-16 16:37:32.000000 git-client-0.2.1/gitclient/ignore.py
--rwxr-xr-x   0 neolaura   (501) staff       (20)     6824 2020-01-13 20:13:30.000000 git-client-0.2.1/gitclient/main.py
--rw-r--r--   0 neolaura   (501) staff       (20)       38 2020-01-13 20:13:55.000000 git-client-0.2.1/setup.cfg
--rw-r--r--   0 neolaura   (501) staff       (20)      811 2020-01-13 20:13:17.000000 git-client-0.2.1/setup.py
+drwxr-xr-x   0 shindagger   (501) staff       (20)        0 2024-04-01 16:39:54.627589 git-client-0.2.2/
+-rw-r--r--   0 shindagger   (501) staff       (20)     1074 2022-05-06 18:47:59.000000 git-client-0.2.2/LICENSE
+-rw-r--r--   0 shindagger   (501) staff       (20)     1366 2024-04-01 16:39:54.627408 git-client-0.2.2/PKG-INFO
+-rw-r--r--   0 shindagger   (501) staff       (20)      939 2022-05-06 18:47:59.000000 git-client-0.2.2/README.md
+drwxr-xr-x   0 shindagger   (501) staff       (20)        0 2024-04-01 16:39:54.626298 git-client-0.2.2/git_client.egg-info/
+-rw-r--r--   0 shindagger   (501) staff       (20)     1366 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/PKG-INFO
+-rw-r--r--   0 shindagger   (501) staff       (20)      292 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shindagger   (501) staff       (20)        1 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shindagger   (501) staff       (20)       43 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/entry_points.txt
+-rw-r--r--   0 shindagger   (501) staff       (20)       40 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/requires.txt
+-rw-r--r--   0 shindagger   (501) staff       (20)       10 2024-04-01 16:39:54.000000 git-client-0.2.2/git_client.egg-info/top_level.txt
+drwxr-xr-x   0 shindagger   (501) staff       (20)        0 2024-04-01 16:39:54.626996 git-client-0.2.2/gitclient/
+-rw-r--r--   0 shindagger   (501) staff       (20)        0 2022-05-06 18:48:00.000000 git-client-0.2.2/gitclient/__init__.py
+-rwxr-xr-x   0 shindagger   (501) staff       (20)     3330 2022-05-06 18:48:00.000000 git-client-0.2.2/gitclient/ignore.py
+-rwxr-xr-x   0 shindagger   (501) staff       (20)     6847 2024-04-01 16:16:06.000000 git-client-0.2.2/gitclient/main.py
+-rw-r--r--   0 shindagger   (501) staff       (20)       38 2024-04-01 16:39:54.627643 git-client-0.2.2/setup.cfg
+-rw-r--r--   0 shindagger   (501) staff       (20)      811 2024-04-01 16:16:25.000000 git-client-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `git-client-0.2.1/PKG-INFO` & `git-client-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: git-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: gc is a command line helper client for using git.
 Home-page: https://gitlab.com/shindagger/git-client
 Author: Andy Klier
 Author-email: andyklier@gmail.com
-License: UNKNOWN
-Description: # gc  
-          
-        `gc` is a simple command line helper client for git.  
-          
-        Obviously git has a lot of functionality in the CLI already. Not seeking to re-invent any wheels, `gc` can simplify commits and pushes, add or remove files from .gitignore, and maybe one day help with merge fixes.  
-          
-        ### usage  
-          
-        `$ gc "subject for a git commit"`  
-          
-        **Commit local git repo with message "subject for a git commit", add or rm files, and push changes.** You will be prompted to add a body message (skip with 'n'), and you will see a list of untracked, modified, or deleted files. Simply unselect any files you DON'T want to add or rm.  
-          
-        `$ gc -I`  
-          
-        **show .gitignore for current project and exit**  
-          
-        `$ gc -i config.ini terraform.tfvars`  
-          
-        **add `config.ini` and `terraform.tfvars` to project's .gitignore.** If a file exists already, it will be deleted, but you will be prompted first (unless you provide the [-y] or [--yes] flag).  
-          
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gc  
+  
+`gc` is a simple command line helper client for git.  
+  
+Obviously git has a lot of functionality in the CLI already. Not seeking to re-invent any wheels, `gc` can simplify commits and pushes, add or remove files from .gitignore, and maybe one day help with merge fixes.  
+  
+### usage  
+  
+`$ gc "subject for a git commit"`  
+  
+**Commit local git repo with message "subject for a git commit", add or rm files, and push changes.** You will be prompted to add a body message (skip with 'n'), and you will see a list of untracked, modified, or deleted files. Simply unselect any files you DON'T want to add or rm.  
+  
+`$ gc -I`  
+  
+**show .gitignore for current project and exit**  
+  
+`$ gc -i config.ini terraform.tfvars`  
+  
+**add `config.ini` and `terraform.tfvars` to project's .gitignore.** If a file exists already, it will be deleted, but you will be prompted first (unless you provide the [-y] or [--yes] flag).  
+
```

### Comparing `git-client-0.2.1/README.md` & `git-client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `git-client-0.2.1/git_client.egg-info/PKG-INFO` & `git-client-0.2.2/git_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: git-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: gc is a command line helper client for using git.
 Home-page: https://gitlab.com/shindagger/git-client
 Author: Andy Klier
 Author-email: andyklier@gmail.com
-License: UNKNOWN
-Description: # gc  
-          
-        `gc` is a simple command line helper client for git.  
-          
-        Obviously git has a lot of functionality in the CLI already. Not seeking to re-invent any wheels, `gc` can simplify commits and pushes, add or remove files from .gitignore, and maybe one day help with merge fixes.  
-          
-        ### usage  
-          
-        `$ gc "subject for a git commit"`  
-          
-        **Commit local git repo with message "subject for a git commit", add or rm files, and push changes.** You will be prompted to add a body message (skip with 'n'), and you will see a list of untracked, modified, or deleted files. Simply unselect any files you DON'T want to add or rm.  
-          
-        `$ gc -I`  
-          
-        **show .gitignore for current project and exit**  
-          
-        `$ gc -i config.ini terraform.tfvars`  
-          
-        **add `config.ini` and `terraform.tfvars` to project's .gitignore.** If a file exists already, it will be deleted, but you will be prompted first (unless you provide the [-y] or [--yes] flag).  
-          
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gc  
+  
+`gc` is a simple command line helper client for git.  
+  
+Obviously git has a lot of functionality in the CLI already. Not seeking to re-invent any wheels, `gc` can simplify commits and pushes, add or remove files from .gitignore, and maybe one day help with merge fixes.  
+  
+### usage  
+  
+`$ gc "subject for a git commit"`  
+  
+**Commit local git repo with message "subject for a git commit", add or rm files, and push changes.** You will be prompted to add a body message (skip with 'n'), and you will see a list of untracked, modified, or deleted files. Simply unselect any files you DON'T want to add or rm.  
+  
+`$ gc -I`  
+  
+**show .gitignore for current project and exit**  
+  
+`$ gc -i config.ini terraform.tfvars`  
+  
+**add `config.ini` and `terraform.tfvars` to project's .gitignore.** If a file exists already, it will be deleted, but you will be prompted first (unless you provide the [-y] or [--yes] flag).  
+
```

### Comparing `git-client-0.2.1/gitclient/ignore.py` & `git-client-0.2.2/gitclient/ignore.py`

 * *Files identical despite different names*

### Comparing `git-client-0.2.1/gitclient/main.py` & `git-client-0.2.2/gitclient/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 """ simple git commits """
 
 import argparse
 from argparse import RawTextHelpFormatter
+import json
 import sys
 import os
 import subprocess
 import signal
 import time
 import inquirer
 import pkg_resources
@@ -135,19 +136,19 @@
                     choices=sani_tracked,
                     default=sani_tracked,
                 )]  
                 answers = inquirer.prompt(questions)  # returns a dict
                 ufs = answers['untracked or modified files']
                 for uf in ufs:
                     if uf in sani_deleted:
-                        print(cs("git rm "+uf, "red"))
-                        subprocess.call("git rm "+uf, shell=True, stdout=subprocess.PIPE)
+                        print(cs(f"git rm {uf}", "red"))
+                        subprocess.call("git rm '{uf}'", shell=True, stdout=subprocess.PIPE)
                     else:
-                        print(cs("git add "+uf, "green"))
-                        subprocess.call("git add "+uf, shell=True, stdout=subprocess.PIPE)
+                        print(cs(f"git add {uf}", "green"))
+                        subprocess.call(f"git add '{uf}'", shell=True, stdout=subprocess.PIPE)
                 print()
             else:
                 print(cs("  No untracked or modified files.", "grey"))
             print("Committing...")
             time.sleep(1)
             #print(fullcmd)
             os.system(fullcmd)
```

### Comparing `git-client-0.2.1/setup.py` & `git-client-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="git-client",
-    version="0.2.1",
+    version="0.2.2",
     author="Andy Klier",
     author_email="andyklier@gmail.com",
     description="gc is a command line helper client for using git.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/shindagger/git-client",
     packages=['gitclient'],
```

