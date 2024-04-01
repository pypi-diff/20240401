# Comparing `tmp/graphpro-0.9.2.tar.gz` & `tmp/graphpro-0.9.3.tar.gz`

## Comparing `graphpro-0.9.2.tar` & `graphpro-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.9.2/pytest.ini
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 graphpro-0.9.2/readthedocs.yaml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 graphpro-0.9.2/requirements.txt
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 graphpro-0.9.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 graphpro-0.9.2/docs/conf.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 graphpro-0.9.2/docs/index.rst
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 graphpro-0.9.2/docs/install.rst
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 graphpro-0.9.2/docs/requirements.txt
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/annotations.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/collection.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/graph.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/graphgen.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/model.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 graphpro-0.9.2/src/graphpro/util/residues.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/graphpro/annotations_test.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/graphpro/collection_test.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/graphpro/graph_test.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/graphpro/graphgen_test.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/graphpro/model_test.py
--rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/testdata/5htc.pdb
--rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.9.2/test/testdata/hetnam.pdb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 graphpro-0.9.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 graphpro-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 graphpro-0.9.2/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 graphpro-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 graphpro-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.9.3/pytest.ini
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 graphpro-0.9.3/readthedocs.yaml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 graphpro-0.9.3/requirements.txt
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 graphpro-0.9.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 graphpro-0.9.3/docs/conf.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 graphpro-0.9.3/docs/index.rst
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 graphpro-0.9.3/docs/install.rst
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 graphpro-0.9.3/docs/requirements.txt
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/annotations.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/collection.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/graph.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/graphgen.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/model.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 graphpro-0.9.3/src/graphpro/util/residues.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/graphpro/annotations_test.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/graphpro/collection_test.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/graphpro/graph_test.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/graphpro/graphgen_test.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/graphpro/model_test.py
+-rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/testdata/5htc.pdb
+-rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.9.3/test/testdata/hetnam.pdb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 graphpro-0.9.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 graphpro-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 graphpro-0.9.3/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 graphpro-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 graphpro-0.9.3/PKG-INFO
```

### Comparing `graphpro-0.9.2/.github/workflows/python-app.yml` & `graphpro-0.9.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/docs/install.rst` & `graphpro-0.9.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/src/graphpro/annotations.py` & `graphpro-0.9.3/src/graphpro/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     def __init__(self):
         pass
 
     def generate(self, G: Graph, atom_group: AtomGroup):
         pass
 
     def encode(self) -> torch.tensor:
+        """ Encode the node property to a tensor
+
+            :returns a tensor the first dimension as number of nodes in the graph, 
+            and dtype float (to be able to cat to other node properties.)
+        """
         pass
 
 
 class ResidueType(NodeAnnotation):
     """ Generates a one letter annotation of the residue type and add this to the node
         with the specific `attr_name`
     """
@@ -34,8 +39,8 @@
         for res in atom_group.c_alphas_residues():
             node_id = G.get_node_by_resid(res['resid'])
             G.node_attr_add(node_id, self.attr_name, one_letter_res(res['resname']))
     
     def encode(self, G: Graph) -> torch.tensor:
         res_names = [G.node_attr(n)['resname'] for n in G.nodes()]
         res_ids = [self.res_letters.index(name) for name in res_names]
-        return F.one_hot(torch.tensor(res_ids, dtype=torch.int64), num_classes=len(self.res_letters))
+        return F.one_hot(torch.tensor(res_ids, dtype=torch.int64), num_classes=len(self.res_letters)).to(torch.float)
```

### Comparing `graphpro-0.9.2/src/graphpro/collection.py` & `graphpro-0.9.3/src/graphpro/collection.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/src/graphpro/graph.py` & `graphpro-0.9.3/src/graphpro/graph.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/src/graphpro/graphgen.py` & `graphpro-0.9.3/src/graphpro/graphgen.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/src/graphpro/model.py` & `graphpro-0.9.3/src/graphpro/model.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/src/graphpro/util/residues.py` & `graphpro-0.9.3/src/graphpro/util/residues.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/test/graphpro/annotations_test.py` & `graphpro-0.9.3/test/graphpro/annotations_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,8 +17,8 @@
     assert G.node_attr(0)['resname'] == 'M'
 
 def test_resname_encoded():
     G = md_analisys(u1).generate(ContactMap(cutoff=6), [ResidueType()])
     data = G.to_data(node_encoders=  [ResidueType()])
 
     assert data.x.size() == (214, 22)
-    assert data.x.dtype == torch.int64
+    assert data.x.dtype == torch.float
```

### Comparing `graphpro-0.9.2/test/graphpro/collection_test.py` & `graphpro-0.9.3/test/graphpro/collection_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/test/graphpro/graph_test.py` & `graphpro-0.9.3/test/graphpro/graph_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/test/graphpro/graphgen_test.py` & `graphpro-0.9.3/test/graphpro/graphgen_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/test/testdata/5htc.pdb` & `graphpro-0.9.3/test/testdata/5htc.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/test/testdata/hetnam.pdb` & `graphpro-0.9.3/test/testdata/hetnam.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/LICENSE.txt` & `graphpro-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/README.md` & `graphpro-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `graphpro-0.9.2/pyproject.toml` & `graphpro-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphpro"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="Pegerto Fernandez", email="pegerto@gmail.com" },
 ]
 description = "A python module to handle graph protein data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `graphpro-0.9.2/PKG-INFO` & `graphpro-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphpro
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python module to handle graph protein data
 Project-URL: Homepage, https://github.com/pegerto/graphpro
 Project-URL: Bug Tracker, https://github.com/pegerto/graphpro
 Author-email: Pegerto Fernandez <pegerto@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

