# Comparing `tmp/leetpy-0.2.0.tar.gz` & `tmp/leetpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetpy-0.2.0.tar", last modified: Sat Mar 30 04:43:32 2024, max compression
+gzip compressed data, was "leetpy-0.2.1.tar", last modified: Mon Apr  1 18:40:51 2024, max compression
```

## Comparing `leetpy-0.2.0.tar` & `leetpy-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 04:43:32.557906 leetpy-0.2.0/
--rw-rw-rw-   0        0        0     1088 2024-02-27 09:00:16.000000 leetpy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3149 2024-03-30 04:43:32.556903 leetpy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2449 2024-03-30 04:41:01.000000 leetpy-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 04:43:32.547904 leetpy-0.2.0/leetpy/
--rw-rw-rw-   0        0        0      374 2024-03-29 20:08:51.000000 leetpy-0.2.0/leetpy/__init__.py
--rw-rw-rw-   0        0        0     6820 2024-03-29 14:14:55.000000 leetpy-0.2.0/leetpy/_reingold_tilford_algorithm.py
--rw-rw-rw-   0        0        0     2672 2024-03-29 14:57:57.000000 leetpy-0.2.0/leetpy/array_1d.py
--rw-rw-rw-   0        0        0     4993 2024-03-29 14:53:17.000000 leetpy-0.2.0/leetpy/array_2d.py
--rw-rw-rw-   0        0        0    19167 2024-03-30 04:28:04.000000 leetpy-0.2.0/leetpy/binary_tree.py
--rw-rw-rw-   0        0        0     8553 2024-03-29 14:47:45.000000 leetpy-0.2.0/leetpy/linked_list.py
-drwxrwxrwx   0        0        0        0 2024-03-30 04:43:32.554904 leetpy-0.2.0/leetpy.egg-info/
--rw-rw-rw-   0        0        0     3149 2024-03-30 04:43:31.000000 leetpy-0.2.0/leetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-03-30 04:43:32.000000 leetpy-0.2.0/leetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 04:43:32.000000 leetpy-0.2.0/leetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-30 04:43:32.000000 leetpy-0.2.0/leetpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 04:43:32.000000 leetpy-0.2.0/leetpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 04:43:32.557906 leetpy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1654 2024-03-30 04:42:20.000000 leetpy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.854921 leetpy-0.2.1/
+-rw-rw-rw-   0        0        0     1088 2024-02-27 09:00:16.000000 leetpy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4082 2024-04-01 18:40:51.853920 leetpy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2024-04-01 18:38:04.000000 leetpy-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.846920 leetpy-0.2.1/leetpy/
+-rw-rw-rw-   0        0        0      374 2024-03-29 20:08:51.000000 leetpy-0.2.1/leetpy/__init__.py
+-rw-rw-rw-   0        0        0     6820 2024-03-29 14:14:55.000000 leetpy-0.2.1/leetpy/_reingold_tilford_algorithm.py
+-rw-rw-rw-   0        0        0     2672 2024-03-29 14:57:57.000000 leetpy-0.2.1/leetpy/array_1d.py
+-rw-rw-rw-   0        0        0     4993 2024-03-30 08:21:13.000000 leetpy-0.2.1/leetpy/array_2d.py
+-rw-rw-rw-   0        0        0    26791 2024-03-31 13:14:22.000000 leetpy-0.2.1/leetpy/binary_tree.py
+-rw-rw-rw-   0        0        0     8553 2024-03-29 14:47:45.000000 leetpy-0.2.1/leetpy/linked_list.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:40:51.852920 leetpy-0.2.1/leetpy.egg-info/
+-rw-rw-rw-   0        0        0     4082 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 18:40:51.000000 leetpy-0.2.1/leetpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 18:40:51.854921 leetpy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2024-04-01 18:39:32.000000 leetpy-0.2.1/setup.py
```

### Comparing `leetpy-0.2.0/LICENSE` & `leetpy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.0/PKG-INFO` & `leetpy-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,71 @@
-Metadata-Version: 2.1
-Name: leetpy
-Version: 0.2.0
-Summary: You should solve DSA problems efficiently.
-Author: Aryan Pingle
-Author-email: realaryanpingle@gmail.com
-License: MIT
-Project-URL: Homepage, https://github.com/aryanpingle/LeetPy
-Project-URL: Source, https://github.com/aryanpingle/LeetPy
-Project-URL: Download, https://pypi.org/project/leetpy/#files
-Project-URL: Tracker, https://github.com/aryanpingle/LeetPy/issues
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![LeetPy Banner](https://raw.githubusercontent.com/aryanpingle/LeetPy/master/static/images/LeetPy%20Banner.png)](https://github.com/aryanpingle/LeetPy)
 
 > Debugging is twice as hard as writing the code in the first place.
 
 If you solve problems related to Data Structures & Algorithms (DSA), you know how frustrating it is to debug complex data structures like Binary Trees and Directed Graphs.
 
 **`LeetPy`** is a lightweight Python package that makes you more efficient when you solve DSA problems. It contains utility functions and algorithms that make debugging and testing *SO MUCH* easier. Here are some features:
 
 - **Several Data Structures**: Binary Trees, Linked Lists, 2-D Arrays, etc.
 - **Visualize Your Objects**: **`LeetPy`** provides convenient `print()` functions that show you what your structure looks like (all inside your terminal!).
 - **Save & Export**: Serialization and export functions help you save an exact copy of your structure, and give you the code to generate them from scratch.
 - **Flexibility**: Create your data structure *however* you want; **`LeetPy`**'s algorithms will always work correctly.
 
-## Usage & Examples
-
-Consider debugging the Binary Tree data structure:
-
-```python
-from leetpy import BinaryTree
-
-# from leetpy import TreeNode
-class TreeNode:
-    """A basic definition of a binary tree's node."""
-
-    def __init__(
-        self,
-        val: any = 0,
-        left: Optional["TreeNode"] = None,
-        right: Optional["TreeNode"] = None,
-    ):
-        self.val = val
-        self.left = left
-        self.right = right
-
-# Randomly generate the root of a binary tree
-root: TreeNode = BinaryTree.create(n=20, min_val=1, max_val=10)
-# Or, import it from a serialized array (like on Leetcode)
-root: TreeNode = BinaryTree.create_from_leetcode_array("[1,2,3,4,null,null,5]")
-
-# Count the number of nodes in the binary tree
-print(BinaryTree.count_nodes(root))
-# Print all the nodes of the binary tree
-for node in BinaryTree.travel_inorder(root):
-    print(node)
-# Visualize the structure of the binary tree
-BinaryTree.print_structure(root)
-```
-
-**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures.
-
 ## Installation
 
 To install the latest stable release, run:
 
 ```bash
 $ pip install leetpy
 ```
 
 To install from the latest GitHub commit:
 
 ```bash
 pip install git+https://github.com/aryanpingle/leetpy
 ```
 
+## Usage & Examples
+
+Here's a minimal use-case:
+
+```python
+# Create a random binary tree and visualize it
+
+from leetpy import BinaryTree
+
+root = BinaryTree.create(n=20)  # create a random binary tree with 20 nodes
+BinaryTree.print_structure(root)  # visualize the binary tree
+```
+
+And here's a complex one:
+
+```python
+# Suppose you want to 'save' 10 binary search trees (example: for testing purposes)
+# You would need some Python code that generates each tree exactly
+
+from leetpy import BinaryTree
+
+for i in range(1, 11):
+    # Generate a random binary search tree (BST) with 20 nodes
+    # Each node should have a value between 1 and 10 (inclusive)
+    root = BinaryTree.create(n=20, min_val=1, max_val=10, make_bst=True)
+    
+    # Get the python code that generates this exact BST
+    # Oh, and make each node an object of class "CustomNode"
+    # Oh, and keep indentation to 2 spaces
+    code += "\n" + BinaryTree.export_as_code(root, node_alias="CustomNode", indent=2)
+
+with open("testing.py", "w") as f:
+    f.write(code)
+```
+
+**`LeetPy`** offers a wide range of utility functions - for a wide range of data structures. Here's a comprehensive list of examples:
 
+|Example|Description|
+|---|---|
+|[Binary Tree Example 1](./examples/binary_tree/example_1.py)|Create a randomized binary tree with 20 nodes and visualize it.|
+|[Binary Tree Example 2](./examples/binary_tree/example_2.py)|Generate a file which contains code for creating randomized binary trees with some constraints (without dependending on the leetpy package).|
+|[Binary Tree Example 3](./examples/binary_tree/example_3.py)|Same as example 2, but with inlined generated code (reducing the number of generated lines).|
+|[Linked List Example 1](./examples/linked_list/example_1.py)|Create a randomized singly linked list with 20 nodes and visualize it.|
+|[Linked List Example 2](./examples/linked_list/example_2.py)|Create a randomized AND CYCLIC singly linked list with 20 UNIQUE nodes and visualize it.|
```

### Comparing `leetpy-0.2.0/leetpy/_reingold_tilford_algorithm.py` & `leetpy-0.2.1/leetpy/_reingold_tilford_algorithm.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.0/leetpy/array_1d.py` & `leetpy-0.2.1/leetpy/array_1d.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.0/leetpy/array_2d.py` & `leetpy-0.2.1/leetpy/array_2d.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.0/leetpy/linked_list.py` & `leetpy-0.2.1/leetpy/linked_list.py`

 * *Files identical despite different names*

### Comparing `leetpy-0.2.0/setup.py` & `leetpy-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("version.txt", "r") as f:
     version = f.read()
 
-version = "0.2.0"
+version = "0.2.1"
 
 # Validate the version name
 try:
     v = Version(version)
     rich_print(f"[bold cyan]{version}[/] [bold green]is a valid version name[/]")
 except:
     rich_print(f"[bold cyan]{version}[/] [bold red]is not a valid version name[/]")
```

