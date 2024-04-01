# Comparing `tmp/p621-0.0.1.tar.gz` & `tmp/p621-0.1.0.tar.gz`

## Comparing `p621-0.0.1.tar` & `p621-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 p621-0.0.1/.pypirc
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 p621-0.0.1/src/p621/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 p621-0.0.1/src/p621/requests.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 p621-0.0.1/src/p621/posts/__init__.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 p621-0.0.1/src/p621/posts/classes.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 p621-0.0.1/src/p621/posts/interactions.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 p621-0.0.1/.gitignore
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 p621-0.0.1/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 p621-0.0.1/README.md
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 p621-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 p621-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 p621-0.1.0/.pypirc
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/requests.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/classes.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/interactions.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 p621-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 p621-0.1.0/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 p621-0.1.0/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 p621-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 p621-0.1.0/PKG-INFO
```

### Comparing `p621-0.0.1/src/p621/posts/classes.py` & `p621-0.1.0/src/p621/posts/classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         self.copyrights: list[str] = tags['copyright']
         self.characters: list[str] = tags['character']
         self.species: list[str] = tags['species']
         self.invalid: list[str] = tags['invalid']
         self.meta: list[str] = tags['meta']
         self.lore: list[str] = tags['lore']
 
+    def dump(self) -> list[str]:
+        return self.general + self.artists + self.copyrights + self.characters + self.species + self.invalid + self.meta + self.lore
+
 
 class Post:
     def __init__(self, post: dict) -> None:
         self.id: int = post['id']
         self.description: str = post['description']
 
         self.created_at: str = post['created_at']
@@ -65,8 +68,23 @@
 
         self.pools: list[str] = post['pools']
 
         self.parent: int = post['relationships']['parent_id']
         self.children: list[str] = post['relationships']['children']
 
         self.approver_id: int = post['approver_id']
-        self.uploader_id: int = post['uploader_id']
+        self.uploader_id: int = post['uploader_id']
+
+    def download(self, path: str = None) -> None:
+        import urllib.request
+
+        target: str = str(self.id) + '.' + self.file.extension
+        if path:
+            target = path + '/' + target
+
+        url: str = self.file.url
+        urllib.request.urlretrieve(url, target)
+
+    def open(self) -> None:
+        import webbrowser
+        url: str = 'https://e621.net/posts/' + str(self.id)
+        webbrowser.open(url)
```

### Comparing `p621-0.0.1/LICENSE` & `p621-0.1.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 MIT License
 
+Copyright (c) 2024 IdEatSomeFish
+
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

