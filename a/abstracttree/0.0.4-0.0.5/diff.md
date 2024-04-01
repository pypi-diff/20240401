# Comparing `tmp/abstracttree-0.0.4-py3-none-any.whl.zip` & `tmp/abstracttree-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 21230 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      732 b- defN 24-Feb-26 15:48 abstracttree/__init__.py
+Zip file size: 22933 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      826 b- defN 24-Mar-30 17:08 abstracttree/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 24-Mar-30 16:36 abstracttree/binarytree.py
 -rw-rw-rw-  2.0 fat    10020 b- defN 24-Feb-07 14:48 abstracttree/conversions.py
--rw-rw-rw-  2.0 fat    17386 b- defN 24-Feb-23 23:59 abstracttree/export.py
--rw-rw-rw-  2.0 fat     1609 b- defN 24-Feb-26 16:17 abstracttree/heaptree.py
--rw-rw-rw-  2.0 fat     2559 b- defN 24-Feb-01 13:24 abstracttree/predicates.py
--rw-rw-rw-  2.0 fat     3854 b- defN 24-Feb-26 18:26 abstracttree/route.py
--rw-rw-rw-  2.0 fat    10141 b- defN 24-Feb-19 19:10 abstracttree/treeclasses.py
--rw-rw-rw-  2.0 fat    11548 b- defN 24-Feb-26 18:27 abstracttree-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6749 b- defN 24-Feb-26 18:27 abstracttree-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-26 18:27 abstracttree-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-26 18:27 abstracttree-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      984 b- defN 24-Feb-26 18:27 abstracttree-0.0.4.dist-info/RECORD
-12 files, 65687 bytes uncompressed, 19586 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat    17887 b- defN 24-Mar-30 16:36 abstracttree/export.py
+-rw-rw-rw-  2.0 fat     1986 b- defN 24-Mar-30 16:36 abstracttree/heaptree.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 24-Mar-30 16:37 abstracttree/predicates.py
+-rw-rw-rw-  2.0 fat     4302 b- defN 24-Feb-29 12:54 abstracttree/route.py
+-rw-rw-rw-  2.0 fat    10394 b- defN 24-Mar-30 16:36 abstracttree/treeclasses.py
+-rw-rw-rw-  2.0 fat    11548 b- defN 24-Apr-01 19:40 abstracttree-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8152 b- defN 24-Apr-01 19:40 abstracttree-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 19:40 abstracttree-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-01 19:40 abstracttree-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1067 b- defN 24-Apr-01 19:40 abstracttree-0.0.5.dist-info/RECORD
+13 files, 71958 bytes uncompressed, 21161 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: abstracttree/__init__.py
 Comment: 
 
+Filename: abstracttree/binarytree.py
+Comment: 
+
 Filename: abstracttree/conversions.py
 Comment: 
 
 Filename: abstracttree/export.py
 Comment: 
 
 Filename: abstracttree/heaptree.py
@@ -15,23 +18,23 @@
 
 Filename: abstracttree/route.py
 Comment: 
 
 Filename: abstracttree/treeclasses.py
 Comment: 
 
-Filename: abstracttree-0.0.4.dist-info/LICENSE
+Filename: abstracttree-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: abstracttree-0.0.4.dist-info/METADATA
+Filename: abstracttree-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: abstracttree-0.0.4.dist-info/WHEEL
+Filename: abstracttree-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: abstracttree-0.0.4.dist-info/top_level.txt
+Filename: abstracttree-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: abstracttree-0.0.4.dist-info/RECORD
+Filename: abstracttree-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstracttree/__init__.py

```diff
@@ -1,13 +1,15 @@
 __all__ = [
     "Tree",
     "DownTree",
     "UpTree",
-    "MutableDownTree",
     "MutableTree",
+    "MutableDownTree",
+    "BinaryTree",
+    "BinaryDownTree",
     "astree",
     "print_tree",
     "plot_tree",
     "to_string",
     "to_image",
     "to_dot",
     "to_mermaid",
@@ -16,16 +18,17 @@
     "RemoveDuplicates",
     "PreventCycles",
     "MaxDepth",
     "HeapTree",
     "Route",
 ]
 
+from .binarytree import BinaryTree, BinaryDownTree
 from .conversions import astree
 from .export import print_tree, plot_tree, to_image, to_dot, to_mermaid, to_string, to_pillow, \
     to_latex
 from .heaptree import HeapTree
 from .predicates import RemoveDuplicates, PreventCycles, MaxDepth
 from .route import Route
 from .treeclasses import Tree, DownTree, UpTree, MutableDownTree, MutableTree
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## abstracttree/export.py

```diff
@@ -450,14 +450,29 @@
     file.write("\n")
     for back in range(depth, 0, -1):
         file.write(back * indent + "}\n")
 
     file.write(r"\end{tikzpicture}")
 
 
+# Optional integration with PrettyPrint
+try:
+    from PrettyPrint import PrettyPrintTree as _PPTree
+
+    # This calls astree more often than necessary but preserves signature of func
+    pprint_tree = _PPTree(get_children=lambda t: astree(t).children,
+                          get_val=lambda t: str(astree(t)))
+
+except ImportError:
+    _PPTree = None
+
+    def pprint_tree(_, *_args, **_kwargs):
+        raise ImportError("Install PrettyPrint from pypi by `pip install PrettyPrint`")
+
+
 def _latex_options(node, options):
     output = []
     for option in options:
         if callable(option):
             output.append(str(option(node)))
         else:
             output.append(str(option))
```

## abstracttree/heaptree.py

```diff
@@ -1,13 +1,14 @@
 from typing import Collection, Optional
 
-from .treeclasses import Tree, TNode
+from .binarytree import BinaryTree
+from .treeclasses import TNode
 
 
-class HeapTree(Tree):
+class HeapTree(BinaryTree):
     """Provides a tree interface to a heap.
 
     Mainly useful for visualisation purposes.
     >>> from abstracttree import print_tree
     >>> import heapq
     >>> tree = HeapTree()
     >>> for n in range(5, 0, -1):
@@ -46,14 +47,26 @@
     @property
     def children(self: TNode) -> Collection[TNode]:
         return [HeapTree(self.heap, i)
                 for i in range(2 * self.index + 1, 2 * self.index + 3)
                 if i < len(self.heap)]
 
     @property
+    def left_child(self) -> Optional[TNode]:
+        i = 2 * self.index + 1
+        if i < len(self.heap):
+            return HeapTree(self.heap, i)
+
+    @property
+    def right_child(self) -> Optional[TNode]:
+        i = 2 * self.index + 2
+        if i < len(self.heap):
+            return HeapTree(self.heap, i)
+
+    @property
     def parent(self: TNode) -> Optional[TNode]:
         n = self.index
         if n != 0:
             return HeapTree(self.heap, (n - 1) // 2)
         else:
             return None
```

## abstracttree/route.py

```diff
@@ -105,22 +105,35 @@
         for i, j in itertools.pairwise(indices):
             path_i, path_j = self._apaths[i:j + 1]
             c = self._route._common2(i, j)
             yield from path_i[:c:-1] + path_j[c:-1]
         if path_j:
             yield path_j[-1]
 
+    def __reversed__(self):
+        indices = range(len(self._apaths))
+        path_i = None
+        for j, i in itertools.pairwise(indices[::-1]):
+            path_i, path_j = self._apaths[i:j + 1]
+            c = self._route._common2(i, j)
+            yield from path_j[:c:-1] + path_i[c:-1]
+        if path_i:
+            yield path_i[-1]
+
     def __len__(self):
         s = 1
         indices = range(len(self._apaths))
         for i, j in itertools.pairwise(indices):
             p1, p2 = self._apaths[i:j + 1]
             s += len(p1) + len(p2) - 2 * self._route._common2(i, j) - 2
         return s
 
 
 class EdgesView(RouteView):
     def __iter__(self):
         return itertools.pairwise(self._route.nodes)
 
+    def __reversed__(self):
+        return itertools.pairwise(reversed(self._route.nodes))
+
     def __len__(self):
         return len(self._route.nodes) - 1
```

## abstracttree/treeclasses.py

```diff
@@ -319,14 +319,21 @@
 
     def __iter__(self):
         level = [self.tree]
         while level:
             yield iter(level)
             level = [child for node in level for child in node.children]
 
+    def zigzag(self):
+        """Traverse the levels in zigzag-order."""
+        level = [self.tree]
+        while level:
+            yield iter(level)
+            level = [child for node in reversed(level) for child in reversed(node.children)]
+
     def count(self):
         return 1 + max(it.depth for (_, it) in self.tree.nodes.preorder())
 
 
 class SiblingsView(TreeView):
     __slots__ = "node"
```

## Comparing `abstracttree-0.0.4.dist-info/LICENSE` & `abstracttree-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abstracttree-0.0.4.dist-info/METADATA` & `abstracttree-0.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: abstracttree
-Version: 0.0.4
+Version: 0.0.5
 Summary: Abstract base classes for tree data structures
-Home-page: https://github.com/lverweijen/abstracttree
-Author: lverweijen
-Author-email: lauwerund@gmail.com
+Author-email: lverweijen <lauwerund@gmail.com>
 License: Apache License 2.0
-Keywords: tree,datastructure,graphviz,mermaid,abc,visualization
+Project-URL: Homepage, https://github.com/lverweijen/abstracttree
+Project-URL: Repository, https://github.com/lverweijen/abstracttree
+Project-URL: Issues, https://github.com/lverweijen/abstracttree/issues
+Project-URL: Changelog, https://github.com/lverweijen/abstracttree/blob/main/changes.md
+Keywords: tree,datastructure,hierarchy,taxonomy,newick,graphviz,mermaid
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Provides-Extra: pillow
-Requires-Dist: Pillow >=5.0 ; extra == 'pillow'
+Provides-Extra: export
+Requires-Dist: Pillow >=5.0 ; extra == 'export'
+Requires-Dist: matplotlib >=3.0 ; extra == 'export'
 
 This Python package contains a few abstract base classes for tree data structures.
 Trees are very common data structure that represents a hierarchy of common nodes.
 This package defines abstract base classes for these data structure in order to make code reusable.
 
 ## Abstract base classes ##
 
@@ -42,35 +45,42 @@
 Tree[Tree];
 MutableTree[MutableTree];
 DownTree[DownTree];
 Tree[Tree];
 MutableTree[MutableTree];
 MutableDownTree[MutableDownTree];
 MutableTree[MutableTree];
+BinaryDownTree[BinaryDownTree]
+BinaryTree[BinaryTree]
 AbstractTree-->UpTree;
 UpTree-->Tree;
 Tree-->MutableTree;
 AbstractTree-->DownTree;
 DownTree-->Tree;
 DownTree-->MutableDownTree;
 MutableDownTree-->MutableTree;
+DownTree-->BinaryDownTree
+BinaryDownTree-->BinaryTree
+Tree-->BinaryTree
 ```
 
 Downtrees are trees that have links to their direct children.
 Uptrees are trees that link to their parent.
 A Tree has links in both directions.
 
-| ABC               | Inherits from             | Abstract Methods                | Mixin Methods                                                        |
-|-------------------|---------------------------|---------------------------------|----------------------------------------------------------------------|
-| `AbstractTree`    |                           |                                 | `nid`, `eqv()`                                                                      |
-| `UpTree`          | `AbstractTree`            | `parent`                        | `root`, `is_root`, `ancestors`, `path`                               |
-| `DownTree`        | `AbstractTree`            | `children`                      | `nodes`, `descendants`, `leaves`, `levels`, `is_leaf`, `transform()` |
-| `Tree`            | `UpTree`, `DownTree`      |                                 | `siblings`                                                           |
-| `MutableDownTree` | `DownTree`                | `add_child()`, `remove_child()` | `add_children()`                                                     |
-| `MutableTree`     | `Tree`, `MutableDownTree` |                                 | `detach()`                                                           |
+| ABC               | Inherits from               | Abstract Methods                  | Mixin Methods                                                                                                                        |
+|-------------------|-----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
+| `AbstractTree`    |                             |                                   | `nid`, `eqv()`                                                                                                                       |
+| `UpTree`          | `AbstractTree`              | `parent`                          | `root`, `is_root`, `ancestors`, `path`                                                                                               |
+| `DownTree`        | `AbstractTree`              | `children`                        | `nodes`, `descendants`, `leaves`, `levels`, `is_leaf`, `transform()`, `nodes.preorder()`, `nodes.postorder()`, `nodes.levelorder()`  |
+| `Tree`            | `UpTree`, `DownTree`        |                                   | `siblings`                                                                                                                           |
+| `MutableDownTree` | `DownTree`                  | `add_child()`, `remove_child()`   | `add_children()`                                                                                                                     |
+| `MutableTree`     | `Tree`, `MutableDownTree`   |                                   | `detach()`                                                                                                                           |
+| `BinaryDownTree`  | `DownTree`                  | `left_child`, `right_child`       | `children`, `nodes.inorder()`, `descendants.inorder()`                                                                               |
+| `BinaryTree`      | `BinaryDownTree`, `Tree`    |                                   |                                                                                                                                      |
 
 In your own code, you can inherit from these trees.
 For example, if your tree only has links to children:
 
 ```python
 import abstracttree
 from abstracttree import print_tree
```

