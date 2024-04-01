# Comparing `tmp/fado-2.1.2.tar.gz` & `tmp/fado-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fado-2.1.2.tar", max compression
+gzip compressed data, was "fado-2.2.0.tar", max compression
```

## Comparing `fado-2.1.2.tar` & `fado-2.2.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1587 2023-03-26 14:46:07.054413 fado-2.1.2/FAdo/__init__.py
--rw-r--r--   0        0        0     2069 2023-04-06 07:40:03.282453 fado-2.1.2/FAdo/automata_grammar.lark
--rw-r--r--   0        0        0    21249 2023-01-06 09:39:16.942907 fado-2.1.2/FAdo/cfg.py
--rw-r--r--   0        0        0    39132 2023-01-06 09:39:16.943239 fado-2.1.2/FAdo/codes.py
--rw-r--r--   0        0        0    17630 2023-01-06 09:38:40.155195 fado-2.1.2/FAdo/comboperations.py
--rw-r--r--   0        0        0    24810 2023-04-06 07:36:31.364197 fado-2.1.2/FAdo/common.py
--rw-r--r--   0        0        0    39059 2023-01-06 09:38:40.155618 fado-2.1.2/FAdo/conversions.py
--rw-r--r--   0        0        0   217634 2023-04-06 07:45:15.888846 fado-2.1.2/FAdo/fa.py
--rw-r--r--   0        0        0     1120 2023-01-06 09:37:44.494862 fado-2.1.2/FAdo/families.py
--rw-r--r--   0        0        0    20747 2023-04-06 07:40:03.282738 fado-2.1.2/FAdo/fio.py
--rw-r--r--   0        0        0    46442 2023-01-30 10:18:37.272680 fado-2.1.2/FAdo/fl.py
--rw-r--r--   0        0        0     5034 2023-01-06 09:37:44.496073 fado-2.1.2/FAdo/graphs.py
--rw-r--r--   0        0        0    12885 2023-04-03 20:40:37.314906 fado-2.1.2/FAdo/prax.py
--rw-r--r--   0        0        0   179231 2023-01-30 10:19:43.217240 fado-2.1.2/FAdo/reex.py
--rw-r--r--   0        0        0     1620 2023-01-06 09:39:16.946414 fado-2.1.2/FAdo/regexp_grammar.lark
--rw-r--r--   0        0        0    10645 2023-01-06 09:38:40.158702 fado-2.1.2/FAdo/rndadfa.py
--rw-r--r--   0        0        0     5584 2023-01-06 09:37:44.498441 fado-2.1.2/FAdo/rndfap.py
--rw-r--r--   0        0        0    16941 2023-01-06 09:39:01.226047 fado-2.1.2/FAdo/ska.py
--rw-r--r--   0        0        0     1932 2023-01-06 09:37:44.499818 fado-2.1.2/FAdo/smwc.py
--rw-r--r--   0        0        0     3616 2023-04-03 20:40:37.169177 fado-2.1.2/FAdo/ssemigroup.py
--rw-r--r--   0        0        0    22725 2023-01-06 09:37:44.500079 fado-2.1.2/FAdo/sst.py
--rw-r--r--   0        0        0     5559 2023-01-06 09:38:40.160286 fado-2.1.2/FAdo/tfa.py
--rw-r--r--   0        0        0    46337 2023-01-06 09:39:16.946537 fado-2.1.2/FAdo/transducers.py
--rw-r--r--   0        0        0     3676 2023-01-06 09:38:40.160870 fado-2.1.2/FAdo/unionFind.py
--rw-r--r--   0        0        0    59804 2023-01-30 10:19:43.217485 fado-2.1.2/FAdo/witness.py
--rw-r--r--   0        0        0     3093 2023-01-06 09:38:40.164173 fado-2.1.2/README.rst
--rw-r--r--   0        0        0     1959 2023-04-06 07:34:50.924451 fado-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 fado-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2226 2024-04-01 18:17:56.743307 fado-2.2.0/FAdo/__init__.py
+-rw-r--r--   0        0        0     2069 2023-04-06 08:38:09.592232 fado-2.2.0/FAdo/automata_grammar.lark
+-rw-r--r--   0        0        0    21249 2023-01-06 09:39:16.942907 fado-2.2.0/FAdo/cfg.py
+-rw-r--r--   0        0        0    39132 2024-02-12 14:29:32.700684 fado-2.2.0/FAdo/codes.py
+-rw-r--r--   0        0        0    17630 2023-01-06 09:38:40.155195 fado-2.2.0/FAdo/comboperations.py
+-rw-r--r--   0        0        0    29227 2024-04-01 18:52:05.496164 fado-2.2.0/FAdo/common.py
+-rw-r--r--   0        0        0    39048 2024-04-01 18:17:56.744163 fado-2.2.0/FAdo/conversions.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:55:35.801787 fado-2.2.0/FAdo/dfa_minimization.pyx
+-rw-r--r--   0        0        0   222251 2024-04-01 18:37:28.913327 fado-2.2.0/FAdo/fa.py
+-rw-r--r--   0        0        0     1120 2023-01-06 09:37:44.494862 fado-2.2.0/FAdo/families.py
+-rw-r--r--   0        0        0    20747 2023-04-06 08:38:09.593414 fado-2.2.0/FAdo/fio.py
+-rw-r--r--   0        0        0    64374 2024-04-01 18:38:28.215690 fado-2.2.0/FAdo/fl.py
+-rw-r--r--   0        0        0     5034 2023-01-06 09:37:44.496073 fado-2.2.0/FAdo/graphs.py
+-rw-r--r--   0        0        0     3329 2024-04-01 18:17:56.745011 fado-2.2.0/FAdo/ordered.py
+-rw-r--r--   0        0        0    12885 2024-02-12 14:29:16.122784 fado-2.2.0/FAdo/prax.py
+-rw-r--r--   0        0        0   179231 2024-02-12 14:29:16.123181 fado-2.2.0/FAdo/reex.py
+-rw-r--r--   0        0        0     1620 2023-01-06 09:39:16.946414 fado-2.2.0/FAdo/regexp_grammar.lark
+-rw-r--r--   0        0        0    12463 2024-02-12 17:27:04.919321 fado-2.2.0/FAdo/rndadfa.py
+-rw-r--r--   0        0        0     5584 2023-01-06 09:37:44.498441 fado-2.2.0/FAdo/rndfap.py
+-rw-r--r--   0        0        0    16941 2023-01-06 09:39:01.226047 fado-2.2.0/FAdo/ska.py
+-rw-r--r--   0        0        0     1932 2023-01-06 09:37:44.499818 fado-2.2.0/FAdo/smwc.py
+-rw-r--r--   0        0        0     3616 2023-04-06 08:38:09.593687 fado-2.2.0/FAdo/ssemigroup.py
+-rw-r--r--   0        0        0    22725 2023-01-06 09:37:44.500079 fado-2.2.0/FAdo/sst.py
+-rw-r--r--   0        0        0     5559 2023-01-06 09:38:40.160286 fado-2.2.0/FAdo/tfa.py
+-rw-r--r--   0        0        0    46337 2024-02-12 14:29:16.123925 fado-2.2.0/FAdo/transducers.py
+-rw-r--r--   0        0        0     3676 2023-01-06 09:38:40.160870 fado-2.2.0/FAdo/unionFind.py
+-rw-r--r--   0        0        0    60763 2024-04-01 18:17:56.745206 fado-2.2.0/FAdo/witness.py
+-rw-r--r--   0        0        0     3895 2024-04-01 18:17:56.745911 fado-2.2.0/README.rst
+-rw-r--r--   0        0        0     2192 2024-04-01 18:50:46.639291 fado-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 fado-2.2.0/PKG-INFO
```

### Comparing `fado-2.1.2/FAdo/__init__.py` & `fado-2.2.0/FAdo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # coding=utf-8
 """ FAdo initialization"""
-#  Copyright (c) 2022. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#  Copyright (c) 2022-2024. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 #  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 #  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 
-version="2.0.4"
+version="2.1.3"
 __all__=["fa","reex","common","cfg","fl","comboperations","ska","conversions","codes","transducers",
-         "rndfap","rndadfa","fio","prax","ssemigroup"]
+         "rndfap","rndadfa","fio","prax","ssemigroup","witness"]
 __package__="FAdo"
```

### Comparing `fado-2.1.2/FAdo/automata_grammar.lark` & `fado-2.2.0/FAdo/automata_grammar.lark`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/cfg.py` & `fado-2.2.0/FAdo/cfg.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/codes.py` & `fado-2.2.0/FAdo/codes.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/comboperations.py` & `fado-2.2.0/FAdo/comboperations.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/common.py` & `fado-2.2.0/FAdo/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,40 @@
    or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
    for more details.
 
    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    675 Mass Ave, Cambridge, MA 02139, USA."""
 
+#  Copyright (c) 2023-2024. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+
 import os
 import random
 from copy import deepcopy
 from abc import abstractmethod
 import functools
 import tempfile
 import subprocess
@@ -44,15 +70,15 @@
     PyPy = False
 
 try:
     from IPython.display import display, SVG  # , get_ipython
 except ImportError:
     pass
 
-FAdoVersion = "2.1.2"
+FAdoVersion = ("2.2.0")
 __version__ = FAdoVersion
 
 
 def run_from_ipython_notebook():
     try:
         cfg = get_ipython().config
         if 'IPKernelApp' in cfg:
@@ -180,14 +206,18 @@
     pass
 
 
 class FAdoNotImplemented(FAdoError):
     pass
 
 
+class FASiseMismatch(FAdoError):
+    pass
+
+
 class DFASyntaticError(DFAerror):
     def __init__(self, line):
         self.line = line
 
 
 class DFAstateUnknown(DFAerror):
     def __init__(self, stidx):
@@ -293,14 +323,19 @@
         return "Transducer Error"
 
 
 class SSError(FAdoError):
     pass
 
 
+class ParRangError(FAdoError):
+    def __str__(self):
+        return "Parameter out of range"
+
+
 class SSMissAlphabet(SSError):
     def __str__(self):
         return "Missing alphabet"
 
 
 class SSBadTransition(SSError):
     def __str__(self):
@@ -1065,7 +1100,83 @@
 def zeta(s: int | float, t=100) -> float | complex:
     """Implementation of Riemman's zeta function"""
     if s == 1:
         return complex("inf")
     term = (1 / 2 ** (n + 1) * sum((-1) ** k * binom(n, k) * (k + 1) ** -s
                                    for k in range(n + 1)) for n in count(0))
     return sum(islice(term, t)) / (1 - 2 ** (1 - s))
+
+
+def inBase(n: int, base: int, tail=None) -> list:
+    """ Writes the representation of a non-null natural in a base.
+
+    Args:
+        n: number to conver
+        base: base to use
+    Returns: list of integers
+
+    .. versionadded:: 2.1.3    """
+    assert n >= 0
+    if tail is None:
+        if n == 0:
+            return [0]
+        tail = []
+    if n == 0:
+        return tail
+    r = n % base
+    return inBase((n-r)//base, base, [r]+tail)
+
+
+def pad(n: int, nu: list)->list :
+    """ Pads the given list nu to have the appropriate number of leading 0 up to size n
+
+    Args:
+        n: number of algarisms
+        nu: list"""
+    l = len(nu)
+    return [0 for _i in range(n-l)] + nu
+
+
+def fromBase(n: list, b: int) ->int:
+    """Converts a number n in base b into an integer
+
+    Args:
+        n (list): number to convert
+        b (int): base used
+
+    Returns: int
+    .. versionadded: 2.1.3"""
+    p = 1
+    v =0
+    n.reverse()
+    for i in n:
+        v += p * i
+        p *= b
+    return v
+
+
+def padList(l: list, size: int) -> list:
+    """ Pads the list l, with zeros, up to the size size
+
+    Args:
+        l (list): the list to pad
+        size (int): the desired size
+
+    Returns:
+        list: the resulting list
+
+    .. versionadded:: 2.1.3"""
+    if len(l) == size: return l
+    return [0 for i in range(size - len(l))] + l
+
+
+def unifSzSubset(max: int) -> int:
+    """ Returns a size uniformly distributed for a variable that behaves like a subset of a max element set.
+
+    Args:
+        max (int): max size to accept
+    Returns:
+        int: the size
+
+    .. versionadded:: 2.1.3"""
+    n = random.randint(1,2**(max)-1)
+    return len(bin(n))-2
```

### Comparing `fado-2.1.2/FAdo/conversions.py` & `fado-2.2.0/FAdo/conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 from . import reex
 import itertools
 
 
 def FA2GFA(aut):
     """ Creates a GFA equivalent to NFA
 
-    :arg aut: the automaton
-    :type aut: OFA
-    :returns: a GFA deep copy
-    :rtype: GFA """
+    Args:
+        aut (OFA): the automaton
+    Returns:
+        GFA: deep copy"""
     gfa = GFA()
     gfa.setSigma(aut.Sigma)
     if isinstance(aut, NFA):
         # this should be optimized
         fa = aut._toNFASingleInitial()
         gfa.Initial = uSet(fa.Initial)
         gfa.States = fa.States[:]
@@ -65,31 +65,32 @@
         raise TypeError()
 
 
 def FAallRegExps(aut):
     """Evaluates the alphabetic length of the equivalent regular expression using every possible order of state
     elimination.
 
-    :arg aut: the automaton
-    :type aut: OFA
-    :rtype: list of tuples (int, list of states)"""
+    Args:
+        aut (OFA): the automaton
+    Returns:
+        listo of tuples: list of tuples (int, list of states)"""
     new = aut.dup()
     new.trim()
     gfa = FA2GFA(new)
     for order in itertools.permutations(list(range(len(gfa.States)))):
         return FA2regexpSEO(aut, copy(list(order))).alphabeticLength(), order
 
 
 def cutPoints(aut):
     """Set of FA's cut points
 
-    :arg aut: the automaton
-    :type aut: OFA
-    :returns: set of states
-    :rtype: set of int"""
+    Args:
+        aut (OFA): the automaton
+    Returns:
+        set of states: """
     gfa = FA2GFA(aut)
     gfa.normalize()
     # make gfa a graph instead of a digraph
     new_edges = []
     for a in gfa.delta:
         for b in gfa.delta[a]:
             new_edges.append((a, b))
```

### Comparing `fado-2.1.2/FAdo/fa.py` & `fado-2.2.0/FAdo/fa.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,28 @@
    or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
    for more details.
 
    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    675 Mass Ave, Cambridge, MA 02139, USA."""
 
+#  Copyright (c) 2024. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+
 from copy import copy
 from functools import cmp_to_key
 from collections import deque
 import deprecation
 import typing
 
 #import FAdo.fa
@@ -76,15 +90,15 @@
             str: line to add to the dot file."""
         return "\"{0:s}\" -> \"{1:s}\" [label = \"{2:s}\"];{3:s} ".format(st1, st2, lbl1, sep)
 
     def dotFormat(self, size="20,20", filename=None, direction="LR", strict=False, maxlblsz=6, sep="\n") -> str:
         """ A dot representation
 
         Args:
-            direction (str): direction of drawing - "LR" or "RL"
+            direction (str): direction of drawdrawing - "LR" or "RL"
             size (str): size of image
             filename (str): Name of the output file
             sep (str): line separator
             maxlblsz (int): max size of labels before getting removed
             strict (bool): use limitations of label sizes
         Returns:
             str: the dot representation
@@ -192,14 +206,46 @@
 
     def __len__(self):
         """Size: number of states
 
         :rtype: int"""
         return len(self.States)
 
+    def eliminateStout(self, st):
+        """Eliminate all transitions outgoing from a given state
+
+        Args:
+            st (int): the state index to lose all outgoing transitions
+
+        .. attention::
+           performs in place alteration of the automata
+
+        .. versionadded:: 0.9.6"""
+        if st in list(self.delta.keys()):
+            del (self.delta[st])
+        return self
+
+    def dup(self):
+        """ Duplicate OFA
+
+        Returns:
+            OFA: duplicate object"""
+        return deepcopy(self)
+
+    def changeSigma(self, subst: dict):
+        """ Change the alphabet of an automaton by means of a sunstitution subst
+
+        Args:
+            subst (dict): substitution
+        Raises:
+            FASiseMismatch: if substitution has a size different from existing alphabet"""
+        if len(subst) != len(self.Sigma):
+            raise FASiseMismatch("")
+        #todo: complete the code that cannot be inplementes in this class
+        pass
     def stateAlphabet(self, sti: int) -> list:
         """Active alphabet for this state
 
         Args:
             sti (int): state
         Returns:
             list:"""
@@ -890,14 +936,34 @@
                     ci = -1
                 else:
                     ci = sig.index(c)
                 for j in forceIterable(self.delta[i][c]):
                     dt.append((i, ci, j))
         return tags, self.States, sig, dt, initial, final
 
+    def quotient(self, other):
+        """ Returns the quotient (NFA) of a language by another language, both given by FA.
+
+        Args:
+            other (OFA):  the language to be quotient by
+        Returns:
+            NFA: the quotient
+
+        .. versionadded: 2.1.5"""
+        autp = self.product(other)
+        aut = self.toNFA()
+        l = set()
+        for f,s in autp.States:
+            if s in other.States:
+                i = other.States.index(s)
+                if i in other.Final and f in aut.States:
+                    l.add(aut.States.index(f))
+        aut.setInitial(l)
+        return aut
+
     def trim(self):
         """Removes the states that do not lead to a final state, or, inclusively,
             that can't be reached from the initial state. Only useful states
             remain.
 
         Returns:
             FA:
@@ -998,36 +1064,14 @@
            self loops are taken in consideration"""
         visited = []
         lst = []
         for s in range(len(self.States)):
             self._topoSort(s, visited, lst)
         return lst
 
-    def eliminateStout(self, st):
-        """Eliminate all transitions outgoing from a given state
-
-        Args:
-            st (int): the state index to lose all outgoing transitions
-
-        .. attention::
-           performs in place alteration of the automata
-
-        .. versionadded:: 0.9.6"""
-        if st in list(self.delta.keys()):
-            del (self.delta[st])
-        return self
-
-    def dup(self):
-        """ Duplicate OFA
-
-        Returns:
-            OFA: duplicate object"""
-        return deepcopy(self)
-
-
 class NFA(OFA):
     """Class for Non-deterministic Finite Automata (epsilon-transitions allowed).
 
     :ivar list States: set of states.
     :ivar set sigma: alphabet set.
     :ivar set Initial: initial state indexes.
     :ivar set Final: set of final states indexes.
@@ -3132,14 +3176,36 @@
         if sti1 not in self.delta:
             self.delta[sti1] = {sym: sti2}
         else:
             if sym in self.delta[sti1] and self.delta[sti1][sym] is not sti2:
                 raise DFAnotNFA("extra transition from ({0:>s}, {1:>s})".format(str(sti1), sym))
             self.delta[sti1][sym] = sti2
 
+    def addTransitionIfNeeded(self, sti1: int, sym, sti2: int) -> int:
+        """ Adds a new transition from sti1 to sti2 consuming symbol sym, creating states if needed
+
+        Args:
+            sti1 (int): state index of departure
+            sti2 (int): state index of arrival
+            sym (Any): symbol consumed
+        Returns:
+            int: the destination state
+        Raises:
+            DFAnotNFA: if one tries to add a non-deterministic transition"""
+        if sti1 not in self.delta:
+            sti2 = self.addState()
+            self.delta[sti1]={sym: sti2}
+            return sti2
+        elif sym not in self.delta[sti1]:
+            sti2 = self.addState()
+            self.delta[sti1][sym] = sti2
+            return sti2
+        else:
+            return self.delta[sti1][sym]
+
     def delTransition(self, sti1, sym, sti2, _no_check=False):
         """Remove a transition if existing and perform cleanup on the transition function's internal data structure.
 
         Args:
             sti1 (int): state index of departure
             sym (Any): symbol consumed
             sti2 (int): state index of arrival
@@ -3305,15 +3371,15 @@
         if not self.Final.isdisjoint(ini):
             d.addFinal(0)
         index = 0
         while True:
             slist = l_states[index]
             si = d.stateIndex(slist)
             for s in self.Sigma:
-                stl = set([self.evalSymbol(s1, s) for s1 in slist if s in self.delta[s1]])
+                stl = set([self.evalSymbol(s1, s) for s1 in slist if (not (self.finalP(s1) and s1 not in self.delta)) and s in self.delta[s1]])
                 if not stl:
                     continue
                 if stl not in l_states:
                     l_states.append(stl)
                     foo = d.addState(stl)
                     if not self.Final.isdisjoint(stl):
                         d.addFinal(foo)
@@ -4283,15 +4349,15 @@
                     if r1 != r2:
                         sets.union(r1, r2)
                         stack.append((r1, r2))
             if equiv:
                 return False
         return True
 
-    def minimalIncremental(self, minimal_test=False):
+    def minimalIncremental(self, minimal_test=False, one_cicle=False):
         """Minimizes the DFA with an incremental method using the Union-Find algorithm and Memoized non-equivalence
         intermediate results
 
         :param bool minimal_test: starts by verifying that the automaton is not minimal?
         :returns: equivalent minimal DFA
         :rtype: DFA
 
@@ -4941,15 +5007,15 @@
         :rtype: bool"""
         if self.delta_inv is None:
             self._compute_delta_inv()
         for c in self.delta_inv.get(st, {}):
             l = self.delta_inv[st][c]
             if len(l) > 1:
                 todo = [st]
-                done = set([])
+                done = set()
                 while todo:
                     s = todo.pop()
                     done.add(s)
                     for d in self.delta.get(s, {}):
                         j = self.delta[s][d]
                         if j in l:
                             return False
@@ -5622,14 +5688,31 @@
             final.add(dicti[i])
         self.Final = final
         states = list(range(len(self.States)))
         for i in range(len(self.States)):
             states[dicti[i]] = self.States[i]
         self.States = states
 
+    def hxState(self, st: int) -> str:
+        """ A hash value for the transition of a state. The automaton needs to be complete.
+
+        :param int st: the state
+        :rtype: str"""
+        if self.finalP(st):
+            s = "F"
+        else:
+            s = ""
+        for c in self.Sigma:
+            st1 = self.delta[st][c]
+            if st1 == st:
+                s += "A"
+            else:
+                s += str(st1)
+        return s
+
     def witnessDiff(self, other):
         """ Returns a witness for the difference of two DFAs and:
 
         +---+------------------------------------------------------+
         | 0 | if the witness belongs to the **other** language     |
         +---+------------------------------------------------------+
         | 1 | if the witness belongs to the **self** language      |
@@ -6517,7 +6600,37 @@
 
 def _initPool() -> tuple:
     """Initialize pool structure
 
     :return: pool and done objects
     :rtype: tuple"""
     return set(), set()
+
+def reduce_size(aut: DFA, maxIter=None) -> DFA:
+    """ A smaller (if possible) DFA. To use with huge automata.
+
+    :param DFA aut: the aoutomata to reduce
+    :param int maxIter: the maxiimum number of iterations before return
+    :rtype: DFA"""
+    aut.complete()
+    if maxIter is None:
+        maxIter = len(aut.States)
+    it = 0
+    while True:
+        sz0 = len(aut)
+        hx, clusters = dict(), dict()
+        for s in aut.stateIndexes():
+            h = aut.hxState(s)
+            if h in hx:
+                clusters[h] = clusters.get(h, [hx[h]]) + [s]
+            else:
+                hx[h] = s
+        it += 1
+        sz1 = 0
+        if len(clusters):
+            ls = [clusters[i] for i in clusters]
+            aut.joinStates(ls)
+            aut.complete()
+            sz1 = len(aut)
+        if sz1 >= sz0 or it >= maxIter:
+            break
+    return aut
```

### Comparing `fado-2.1.2/FAdo/families.py` & `fado-2.2.0/FAdo/families.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/fio.py` & `fado-2.2.0/FAdo/fio.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/fl.py` & `fado-2.2.0/FAdo/fl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 """Finite languages and related automata manipulation
 
 Finite languages manipulation
 
-.. *Authors:* Rogério Reis & Nelma Moreira
+.. *Authors:* Rogério Reis, Nelma Moreira & Guilherme Duarte
 
 .. *This is part of FAdo project*   https://fado.dcc.fc.up.pt
 
-.. *Version:* 1.3.3
-
 .. *Copyright*: 1999-2022 Rogério Reis & Nelma Moreira {rvr,nam}@dcc.fc.up.pt
 
 .. This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.
 
@@ -21,18 +19,72 @@
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.
 
    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA."""
 
+#  Copyright (c) 2023-2024. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+
 from . import fa
-from copy import copy
+import copy
 from . common import *
 import random
+from bitarray import bitarray, frozenbitarray
+from bitarray.util import ba2int
+from itertools import product
+from z3 import *
 
 
 class FL(object):
     """Finite Language Class
 
     :var Words: the elements of the language
     :var Sigma: the alphabet"""
@@ -56,43 +108,50 @@
         l = l[:-1] + "}, {"
         for i in self.Sigma:
             l += str(i)+","
         l = l[:-1] + "})"
         return l
 
     def __repr__(self):
-        return "FL%s" % self.__str__()
+        return "FL%blksz" % self.__str__()
 
     def __len__(self):
         return len(self.Words)
 
     def __contains__(self, item):
         return item in self.Words
 
     def union(self, other):
         """union of FL:   a | b
 
-        :param FL other: right hand operand
-        :rtype: FL
-        :raises FAdoGeneralError: if both arguments are not FL"""
+        Args:
+            other (FL): right hand operand
+        Returns:
+            FL: result of the union
+        Raises:
+            FAdoGeneralError: if both arguments are not FL"""
         return self.__or__(other)
 
     def __or__(self, other):
         if type(other) != type(self):
             raise FAdoGeneralError("Incompatible objects")
         new = FL()
         new.Sigma = self.Sigma | other.Sigma
         new.Words = self.Words | other.Words
         return new
 
     def intersection(self, other):
         """Intersection of FL: a & b
 
-        :param FL other: right hand operand
-        :raises FAdoGeneralError: if both arguments are not FL"""
+        Args:
+            other (FL): left hand operand
+        Returns:
+            FL: result of the operation
+        Raises:
+            FAdoGeneralError: if both arguments are not FL"""
         return self.__and__(other)
 
     def __iter__(self):
         return iter(self.Words)
 
     def __and__(self, other):
         if type(other) != type(self):
@@ -101,68 +160,77 @@
         new.Sigma = self.Sigma | other.Sigma
         new.Words = self.Words & other.Words
         return new
 
     def diff(self, other):
         """Difference of FL: a - b
 
-        :param FL other: right hand operand
-        :rtype: FL
-        :raises FAdoGeneralError: if both arguments are not FL"""
+        Args:
+            other (FL): left hand operand
+        Returns:
+            FL: result of the operation
+        Raises:
+            FAdoGeneralError: if both arguments are not FL"""
         return self.__sub__(other)
 
     def __sub__(self, other):
         if type(other) != type(self):
             raise FAdoGeneralError("Incompatible objects")
         new = FL()
         new.Sigma = self.Sigma | other.Sigma
         new.Words = self.Words - other.Words
         return new
 
     def setSigma(self, Sigma, Strict=False):
         """Sets the alphabet of a FL
 
-        :param set Sigma: alphabet
-        :param bool Strict: behaviour
+        Args:
+            Sigma (string): alphabet
+            Strict (bool): behaviour
 
         .. attention::
            Unless Strict flag is set to True, alphabet can only be enlarged.  The resulting alphabet is  in fact the
            union of the former alphabet with the new one. If flag is set to True, the alphabet is simply replaced."""
         if Strict:
             self.Sigma = Sigma
         else:
             self.Sigma = self.Sigma.union(Sigma)
 
     def addWords(self, wList):
         """Adds a list of words to a FL
 
-        :param list wList: words to add"""
+        Args:
+            wList (list): words to be added"""
         self.Words |= set(wList)
         for w in wList:
             if w.epsilonP():
                 continue
             for c in w:
                 self.Sigma.add(c)
 
     def addWord(self, word):
         """Adds a word to a FL
-        :type word: Word
-        :rtype: FL"""
+
+        Args:
+            word (string): word to be added
+        Returns:
+            FL: """
         if word in self:
             return
         self.Words.add(word)
         if not word.epsilonP():
             for c in word:
                 self.Sigma.add(c)
 
     def suffixClosedP(self):
         """Tests if a language is suffix closed
 
-        :rtype: bool"""
-        wrds = list(copy(self.Words))
+        Returns:
+            bool: True if language is suffix closed"""
+        wrds = list(copy.copy(self.Words))
         if Epsilon not in wrds:
             return False
         else:
             wrds.remove(Epsilon)
         wrds.sort(lambda x, y: len(x) - len(y))
         while wrds:
             w = wrds.pop()
@@ -173,17 +241,18 @@
                     if w1 in wrds:
                         wrds.remove(w1)
         return True
 
     def filter(self, automata):
         """Separates a language in two other using a DFA of NFA as a filter
 
-        :param DFA|NFA automata: the automata to be used as a filter
-        :returns: the accepted/unaccepted pair of languages
-        :rtype: tuple of FL"""
+        Args:
+            automata (dict): the automata to be used as a filter
+        Returns:
+            tuple of FL: the accepted/unaccepted pair of languages"""
         a, b = (FL(), FL())
         a.setSigma(self.Sigma)
         b.setSigma(self.Sigma)
         for w in self.Words:
             if automata.evalWord(w):
                 a.addWords([w])
             else:
@@ -191,15 +260,15 @@
         return a, b
 
     def MADFA(self):
         """Generates the minimal acyclical DFA using specialized algorithm
 
         .. versionadded:: 1.3.3
 
-        .. seealso:: Incremental Construction of Minimal Acyclic Finite-State Automata, J.Daciuk, s.Mihov, B.Watson and r.E.Watson
+        .. seealso:: Incremental Construction of Minimal Acyclic Finite-State Automata, J.Daciuk, blksz.Mihov, B.Watson and r.E.Watson
 
         :rtype: ADFA"""
         if self.Words == FL([Epsilon]).Words:
             aut = ADFA()
             i = aut.addState()
             aut.setInitial(i)
             aut.addFinal(i)
@@ -220,18 +289,18 @@
         aut._replace_or_register(i, register)
         aut.Minimal = True
         return aut
 
     def trieFA(self):
         """Generates the trie automaton that recognises this language
 
-        :returns: the trie automaton
-        :rtype: ADFA"""
+        Returns:
+            ADFA: the trie automaton"""
         new = ADFA()
-        new.setSigma(copy(self.Sigma))
+        new.setSigma(copy.copy(self.Sigma))
         i = new.addState()
         new.setInitial(i)
         for w in self.Words:
             if w.epsilonP():
                 new.addFinal(i)
             else:
                 s = i
@@ -244,35 +313,38 @@
                         s = new.delta[s][c]
                 new.addFinal(s)
         return new
 
     def toDFA(self):
         """ Generates a DFA recognizing the language
 
-        :rtype: ADFA
+        Returns:
+            ADFA: the DFA
 
         .. versionadded:: 1.2"""
         return self.trieFA()
 
     def toNFA(self):
         """Generates a NFA recognizing the language
 
-        :rtype: ANFA
+        Returns:
+            ANFA:
 
         .. versionadded:: 1.2"""
         return self.toDFA().toANFA()
 
     # noinspection PyUnboundLocalVariable
     def multiLineAutomaton(self):
         """Generates the trivial linear ANFA equivalent to this language
-    
-        :rtype: ANFA"""
+
+        Returns:
+            ANFA: the trivial linear ANFA"""
         new = ANFA()
         s1 = None
-        new.setSigma(copy(self.Sigma))
+        new.setSigma(copy.copy(self.Sigma))
         for w in self.Words:
             s = new.addState()
             new.addInitial(s)
             for c in w:
                 s1 = new.addState()
                 new.addTransition(s, c, s1)
                 s = s1
@@ -287,17 +359,17 @@
 
     def __init__(self):
         super(DFCA, self).__init__()
         self.length = None
 
     @property
     def length(self):
-        """
-        :return: size of the longest word
-        :rtype: int"""
+        """ The length of the longest word
+        Returns:
+            int: the length of the longest word"""
         return self.length
 
     @length.setter
     def length(self, value):
         """Setter
         :param int value: size"""
         self.length = value
@@ -320,25 +392,27 @@
         self.Initial = None
         self.States = []
         self.Final = set()
 
     @abstractmethod
     def addState(self, _):
         """
-        :rtype: int"""
+        Returns:
+            int: """
         pass
 
     @abstractmethod
     def finalP(self, _):
         pass
 
     def setDeadState(self, sti):
         """Identifies the dead state
 
-        :param int sti: index of the dead state
+        Args:
+            sti (string): index of the dead state
 
         .. attention::
            nothing is done to ensure that the state given is legitimate
 
         .. note::
            without dead state identified, most of the methods for acyclic automata can not be applied"""
         self.Dead = sti
@@ -349,17 +423,17 @@
             _ = self.Dead
         except AttributeError:
             x = self.addState(DeadName)
             self.setDeadState(x)
 
     def ordered(self):
         """Orders states names in its topological order
-    
-        :returns: ordered list of state indexes
-        :rtype: list of int
+
+        Returns:
+            list of int: ordered list of state indexes
 
         .. note::
            one could use the FA.toposort() method, but special care must be taken with the dead state for the
            algorithms related with cover automata."""
 
         def _dealS(st1):
             if st1 not in torder:
@@ -380,16 +454,16 @@
             st = queue.pop()
             _dealS(st)
         torder.append(dead)
         return torder
 
     def _getRdelta(self):
         """
-        :returns: pair, map of number of sons map, of reverse conectivity
-        :rtype: dict"""
+        Returns:
+            dict: pair, map of number of sons map, of reverse conectivity"""
         done = set()
         deltaC, rdelta = {}, {}
         notDone = set(forceIterable(self.Initial))
         while notDone:
             sts = uSet(notDone)
             done.add(sts)
             l = set()
@@ -405,34 +479,34 @@
             if s not in rdelta:
                 rdelta[s] = set()
         return deltaC, rdelta
 
     def directRank(self):
         """Compute rank function
 
-        :return: ranf map
-        :rtype: dict"""
+        Returns:
+            dict: rank map"""
         r, _ = self.evalRank()
         n = {}
         for x in r:
             for i in r[x]:
                 n[i] = x
         return n
 
     def evalRank(self):
         """Evaluates the rank map of a automaton
 
-        :return: pair of sets of states by rank map, reverse delta accessability map
-        :rtype: tuple"""
+        Returns:
+            tuple: pair of sets of states by rank map, reverse delta accessability map"""
         (deltaC, rdelta) = self._getRdelta()
         rank, deltai = {}, {}
         for s in range(len(self.States)):
             deltai.setdefault(deltaC[s], set([])).add(s)
         i = -1
-        notDone = copy(list(range(len(self.States))))
+        notDone = list(range(len(self.States)))
         deltaC[self.Dead] = 0
         deltai[1].remove(self.Dead)
         deltai[0] = {self.Dead}
         rdelta[self.Dead].remove(self.Dead)
         while notDone:
             rank[i] = deepcopy(deltai[0])
             deltai[0] = set()
@@ -445,17 +519,16 @@
                 notDone.remove(s)
             i += 1
         return rank, rdelta
 
     def getLeaves(self):
         """The set of leaves, i.e. final states for last symbols of language words
 
-        :return: set of leaves
-        :rtype: set"""
-
+        Returns:
+            set: A set of leaves"""
         # noinspection PyUnresolvedReferences
         def _last(s1):
             queue, done = {s1}, set()
             while queue:
                 q = queue.pop()
                 done.add(q)
                 for k in self.delta.get(q, {}):
@@ -482,21 +555,21 @@
     """
     def __init__(self):
         fa.DFA.__init__(self)
         AFA.__init__(self)
         self.Minimal = False
 
     def __repr__(self):
-        return 'ADFA({0:s})'.format(self.__str__())
+        return 'ADFA({0:blksz})'.format(self.__str__())
 
     def complete(self, dead=None):
         """Make the ADFA complete
 
-        :param int dead: a state to be identified as dead state if one was not identified yet
-        :rtype: ADFA
+        Args:
+            dead (int, optional): a state to be identified as dead state if one was not identified yet
 
         .. attention::
            The object is modified in place
 
         .. versionchanged:: 1.3.3"""
         if dead is not None:
             self.Dead = dead
@@ -515,30 +588,33 @@
                     self.addTransition(st, k, self.Dead)
         self.Minimal = False
         return self
 
     def dup(self):
         """Duplicate the basic structure into a new ADFA. Basically a copy.deep.
 
-        :rtype: ADFA"""
-        return deepcopy(self)
+        Returns:
+            ADFA: """
+        return copy.deepcopy(self)
 
     def __invert__(self):
         """ Complement of a ADFA is a DFA
 
-        :return:DFA
-        """
+        Returns:
+            DFA: """
         aut = self.forceToDFA()
         return ~aut
 
     def minimalP(self, method=None):
         """Tests if the DFA is minimal
 
-        :param method: minimization algorithm (here void)
-        :rtype: bool
+        Args:
+            method (str): minimization algorithm (here void)
+        Returns:
+            bool:
 
         .. versionchanged:: 1.3.3"""
         if self.Minimal:
             return True
         foo = self.minimal()
         if self.completeP():
             foo.complete()
@@ -546,58 +622,60 @@
         if answ:
             self.Minimal = True
         return answ
 
     def forceToDFA(self):
         """ Conversion to DFA
 
-        :rtype: DFA"""
+        Returns:
+            DFA: """
         new = fa.DFA()
-        new.States = deepcopy(self.States)
-        new.Sigma = deepcopy(self.Sigma)
+        new.States = copy.deepcopy(self.States)
+        new.Sigma = copy.deepcopy(self.Sigma)
         new.Initial = self.Initial
-        new.Final = copy(self.Final)
+        new.Final = copy.copy(self.Final)
         for s in self.delta:
             for c in self.delta[s]:
                 new.addTransition(s, c, self.delta[s][c])
         return new
 
     def forceToDFCA(self):
         """ Conversion to DFCA
 
-        :rtype: DFA"""
+        Returns:
+            DFA: """
         return self.forceToDFA()
 
     def wordGenerator(self):
         """Creates a random word generator
 
-        :return: the random word generator
-        :rtype: RndWGen
+        Returns:
+            RndWGen: the random word generator
 
         .. versionadded:: 1.2"""
         return RndWGen(self)
 
     def possibleToReverse(self):
         """Tests if language is reversible
 
         .. versionadded:: 1.3.3"""
         return True
 
     def minimal(self):
         """Finds the minimal equivalent ADFA
 
-        .. seealso:: [TCS 92 pp 181-189] Minimisation of acyclic deterministic automata in linear time, Dominique Revuz
+        Returns:
+            DFA: the minimal equivalent ADFA
 
-        .. versionchanged:: 1.3.3
+        .. seealso:: [TCS 92 pp 181-189] Minimisation of acyclic deterministic automata in linear time, Dominique Revuz
 
-        :returns: the minimal equivalent ADFA
-        :rtype: ADFA"""
+        .. versionchanged:: 1.3.3 """
 
         def _getListDelta(ss):
-            """returns [([sons,final?],s) for s in ss].sort"""
+            """returns [([sons,final?],blksz) for blksz in ss].sort"""
             l = []
             for s in ss:
                 dl = [new.delta[s][k] for k in new.Sigma]
                 dl.append(s in new.Final)
                 l.append((dl, s))
             l.sort()
             return l
@@ -608,15 +686,15 @@
                 for k in new.delta[s]:
                     if new.delta[s][k] == r2:
                         new.delta[s][k] = r1
             toBeDeleted.append(r2)
 
         if len(self.States) == 1:
             return self
-        new = deepcopy(self)
+        new = copy.deepcopy(self)
         new.trim()
         new.complete()
         if new.Dead is None:
             deadName = None
         else:
             deadName = new.States[new.Dead]
         rank, rdelta = new.evalRank()
@@ -638,24 +716,27 @@
             new.Dead = new.stateIndex(deadName)
         new.Minimal = True
         return new
 
     def minReversible(self):
         """Returns the minimal reversible equivalent automaton
 
-        :rtype: ADFA"""
+        Returns:
+            ADFA: """
         new = self.dup()
         new.evalRank()
 
     def statePairEquiv(self, s1, s2):
         """Tests if two states of a ADFA are equivalent
 
-        :param int s1: state1
-        :param int s2: state2
-        :rtype: bool
+        Args:
+            s1 (int): state1
+            s2 (int): state2
+        Returns:
+            bool:
 
         .. versionadded:: 1.3.3"""
         if not self.same_nullability(s1, s2):
             return False
         else:
             return self.delta.get(s1, {}) == self.delta.get(s2, {})
 
@@ -674,28 +755,31 @@
             self.addTransition(s1, c, s2)
             s1 = s2
         self.addFinal(s1)
 
     def _last_child(self, s):
         """to be used by xxx of FL.MADFA
 
-        :param int s: state index
-        :returns: pair state index / symbol
+        Args:
+            s (int): state index
+        Returns:
+            tuple: pair state index / symbol
 
         .. versionadded:: 1.3.3"""
         for c in sorted(list(self.Sigma)).__reversed__():
             if c in self.delta.get(s, {}):
                 return self.delta[s][c], c
         raise FAdoGeneralError("Something unexpected in _last_child({:d})".format(s))
 
     def _replace_or_register(self, s, r):
         """to be used by xxx of FL.MADFA
 
-        :param int s: state
-        :param Set r: register (inherited from context)
+        Args:
+            s (int): state index
+            r (set): register (inherited from context)
 
         .. versionadded:: 1.3.3"""
         (child, c) = self._last_child(s)
         if self.delta.get(child, {}):
             self._replace_or_register(child, r)
         for q in r:
             if self.statePairEquiv(q, child):
@@ -703,48 +787,50 @@
                 self.deleteState(child)
                 return
         r.add(child)
 
     def _common_prefix(self, wrd):
         """The longest prefix of w that can be read in the ADFA and the correspondent state
 
-        :param Word wrd: word"""
+        Args:
+            wrd (Word): the word """
         pref = Word()
         q = self.Initial
         for s in wrd:
             if s in self.delta.get(q, {}):
                 pref.append(s)
                 q = self.delta[q][s]
             else:
                 break
         return pref, q
 
     def _addWordToMinimal(self, w):
         """Incremental minimization algorithm
 
-        :param Word w: word
+        Args:
+            w (Word): the word
 
         .. attention:: in place transformation
 
         .. versionadded:: 1.3.3
 
-        .. seealso:: Incremental Construction of Minimal Acyclic Finite-State Automata, J.Daciuk, s.Mihov,
+        .. seealso:: Incremental Construction of Minimal Acyclic Finite-State Automata, J.Daciuk, blksz.Mihov,
                      B.Watson and r.E.Watson"""
 
         def _transverseNonConfluence(wrd):
             inCount = dict()
             for s in range(len(self.States)):
                 for c in self.delta.get(s, {}):
                     for s1 in self.delta[s][c]:
                         inCount[s1] = inCount.get(s1, 0) + 1
             q1 = self.Initial
             visited1 = [q1]
             for ii, sym in enumerate(wrd):
                 if sym not in self.delta.get(q1, {}) or inCount[self.delta[q1][sym]] > 1:
-                    # here there was a reference to s self.delta.get(s, {}) that must be wrong!
+                    # here there was a reference to blksz self.delta.get(blksz, {}) that must be wrong!
                     return q1, ii
                 q1 = self.delta[q1][sym]
                 visited1.append(q1)
 
         def _cloneConfluence(st, wrd, ind):
             q1 = st
             for ii, sym in enumerate(wrd[ind:]):
@@ -787,16 +873,19 @@
         q, i = _cloneConfluence(q, w, i)
         _addSuffix(q, w[i:])
         if j < len(w):
             self.delta[f][w[j]] = _replOrReg(self.delta[f][w[j]], w[j+1:])
 
     def dissMin(self, witnesses=None):
         """Evaluates the minimal dissimilarity language
-        :param dict witnesses: optional witness dictionay
-        :rtype: FL
+
+        Args:
+            witnesses (dict): optional witness dictionay
+        Returns:
+            FL:
 
         .. versionadded:: 1.2.1"""
         new = self.minimal()
         sz = len(new.States)
         todo = [(i, j) for i in range(sz) for j in range(i)]
         mD = FL(Sigma=new.Sigma)
         lvl = new.level()
@@ -825,15 +914,16 @@
                     Li.append((i, j))
             delFromList(todo, Li)
         return mD
 
     def diss(self):
         """ Evaluates the dissimilarity language
 
-        :rtype: FL
+        Returns:
+            FL:
 
         .. versionadded:: 1.2.1"""
         new = self.minimal()
         n = len(new.States)
         mD = FL(Sigma=new.Sigma)
         lvl = new.level()
         rnk = new.directRank()
@@ -855,16 +945,16 @@
                         skip = True
                         break
         return mD
 
     def level(self):
         """Computes the level  for each state
 
-        :returns: levels of states
-        :rtype: dict
+        Returns:
+            dict: levels of states
 
         .. versionadded:: 0.9.8"""
         lvl = {}
         done, alvl = set(), [self.Initial]
         l = 0
         while alvl:
             nlvl = set()
@@ -872,26 +962,27 @@
                 lvl[i] = l
                 done.add(i)
                 for c in self.delta[i]:
                     j = self.delta[i][c]
                     if j not in done and j not in alvl:
                         nlvl.add(j)
             l += 1
-            alvl = copy(nlvl)
+            alvl = copy.copy(nlvl)
         return lvl
 
     def _gap(self, l, lvl):
         """Computes the gap value for each pair of states.
 
         The automata is supposed to have its states named numerically in such way that the initial is zero
 
-        :param int l: length of the longest word
-        :param dict lvl: level of each state
-        :returns: gap function
-        :rtype: dict"""
+        Args:
+            l (int): length of the longest word
+            lvl (dict): level of each state
+        Returns:
+            dict: gap function """
         def _range(r, s):
             return l - max(lvl[r], lvl[s])
         gp = {}
         n = len(self.States) - 1
         for i in range(n):
             gp[(self.stateIndex(i), self.stateIndex(n))] = l
         if lvl[self.stateIndex(n)] <= l:
@@ -916,15 +1007,16 @@
                             gp[(self.stateIndex(i), self.stateIndex(j))] = min(gp[(self.stateIndex(i),
                                                                                    self.stateIndex(j))], g + 1)
         return gp
 
     def minDFCA(self):
         """Generates a minimal deterministic cover automata from a DFA
 
-        :rtype: DFCA
+        Returns:
+            DCFA:
 
         .. versionadded:: 0.9.8
 
         .. seealso::
             Cezar Campeanu, Andrei Päun, and Sheng Yu, An efficient algorithm for constructing minimal cover
             automata for finite languages, IJFCS"""
         new = self.dup().minimal()
@@ -971,30 +1063,32 @@
         except AttributeError:
             pass
         return self
 
     def toANFA(self):
         """Converts the ADFA in a equivalent ANFA
 
-        :rtype: ANFA"""
+        Returns:
+            ANFA:"""
         new = ANFA()
-        new.setSigma(copy(self.Sigma))
-        new.States = copy(self.States)
+        new.setSigma(copy.copy(self.Sigma))
+        new.States = copy.copy(self.States)
         for s in range(len(self.States)):
             for k in self.delta.get(s, {}):
                 new.addTransition(s, k, self.delta[s][k])
         new.addInitial(self.Initial)
         for s in self.Final:
             new.addFinal(s)
         return new
 
     def toNFA(self):
         """Converts the ADFA in a equivalent NFA
 
-        :rtype: ANFA
+        Returns:
+            ANFA:
 
         .. versionadded:: 1.2"""
         return self.toANFA()
 
 
 class RndWGen(object):
     """Word random generator class
@@ -1074,16 +1168,17 @@
             for k in l:
                 self.addTransition(s, k, stf)
             self.delFinal(s)
 
     def mergeStates(self, s1, s2):
         """Merge state s2 into state s1
 
-        :param int s1: state
-        :param int s2: state
+        Args:
+            s1 (int): state index
+            s2 (int): state index
 
         .. note::
            no attempt is made to check if the merging preserves the language of teh automaton
 
         .. attention:: the object is modified in place"""
         (_, rdelta) = self._getRdelta()
         for s in rdelta[s2]:
@@ -1111,28 +1206,31 @@
                 s = self.stateIndex(l.pop())
                 self.mergeStates(s0, s)
 
     def mergeInitial(self):
         """Merge initial states
 
         .. attention:: object is modified in place"""
-        l = copy(self.Initial)
+        l = copy.copy(self.Initial)
         s0 = self.stateIndex(l.pop())
         while l:
             s = self.stateIndex(l.pop())
             self.mergeStates(s0, s)
 
 
-def sigmaInitialSegment(Sigma, l, exact=False):
+def sigmaInitialSegment(Sigma: list, l: int, exact=False) -> ADFA:
     """Generates the ADFA recognizing Sigma^i for i<=l
-    :param set Sigma: the alphabet
-    :param int l: length
-    :param bool exact: only the words with exactly that length?
-    :returns: the automaton
-    :rtype: ADFA"""
+
+    Args:
+        Sigma (list): the alphabet
+        l (int): length
+        exact (bool): only the words with exactly that length?
+    Returns:
+        ADFA: the automaton
+    """
     new = ADFA()
     new.setSigma(Sigma)
     s = new.addState()
     if not exact:
         new.addFinal(s)
     new.setInitial(s)
     for i in range(l):
@@ -1144,28 +1242,30 @@
         s = s1
     return new
 
 
 # noinspection PyUnboundLocalVariable
 def genRndTrieBalanced(maxL, Sigma, safe=True):
     """Generates a random trie automaton for a binary language of balanced words of a given leght for max word
-    :param int maxL: length of the max word
-    :param set Sigma: alphabet to be used
-    :param bool safe: should a word of size maxl be present in every language?
-    :return: the generated trie automaton
-    :rtype: ADFA"""
+
+    Args:
+        maxL (int): the length of the max word
+        Sigma (set): the alphabet to be used
+        safe (bool): should a word of size maxl be present in every language?
+    Returns:
+        ADFA: the generated trie automaton """
 
     def _genEnsurance(m, alphabet):
         l = len(alphabet)
         fair = m / l
         if m % l == 0:
             odd = 0
         else:
             odd = 1
-        pool = copy(alphabet)
+        pool = copy.copy(alphabet)
         c = {}
         sl = []
         while len(sl) < m:
             s1 = random.choice(pool)
             c[s1] = c.get(s1, 0) + 1
             if c[s1] == fair + odd:
                 pool.remove(s1)
@@ -1224,25 +1324,26 @@
     return trie
 
 
 # noinspection PyUnboundLocalVariable
 def genRndTrieUnbalanced(maxL, Sigma, ratio, safe=True):
     """Generates a random trie automaton for a binary language of balanced words of a given length for max word
 
-    :param int maxL: length of the max word
-    :param set Sigma: alphabet to be used
-    :param int ratio: the ratio of the unbalance
-    :param bool safe: should a word of size maxl be present in every language?
-    :return: the generated trie automaton
-    :rtype: ADFA"""
+    Args:
+        maxL (int): length of the max word
+        Sigma (set): alphabet to be used
+        ratio (int): the ratio of the unbalance
+        safe (bool): should a word of size maxl be present in every language?
+    Returns:
+        ADFA: the generated trie automaton """
 
     def _genEnsurance(m, alphabet):
         chief = uSet(alphabet)
         fair = m / (ratio + 1)
-        pool = list(copy(alphabet))
+        pool = list(copy.copy(alphabet))
         c = {}
         sl = []
         while len(sl) < m:
             s1 = random.choice(pool)
             c[s1] = c.get(s1, 0) + 1
             if len(sl) - c.get(chief, 0) == fair:
                 pool = [chief]
@@ -1299,19 +1400,21 @@
         trie.delFinal(s)
     return trie
 
 
 # noinspection PyUnboundLocalVariable
 def genRandomTrie(maxL, Sigma, safe=True):
     """Generates a random trie automaton for a finite language with a given length for max word
-    :param int maxL: length of the max word
-    :param set Sigma: alphabet to be used
-    :param bool safe: should a word of size maxl be present in every language?
-    :return: the generated trie automaton
-    :rtype: ADFA"""
+
+    Args:
+        maxL (int): length of the max word
+        Sigma (set): alphabet to be used
+        safe (bool): should a word of size maxl be present in every language?
+    Returns:
+        ADFA: the generated trie automaton """
 
     def _genEnsurance(m, alphabet):
         l = len(alphabet)
         sl = list(alphabet)
         return [sl[random.randint(0, l - 1)] for _ in range(m)]
 
     # noinspection PyUnboundLocalVariable
@@ -1355,20 +1458,22 @@
     return trie
 
 
 # noinspection PyUnboundLocalVariable
 def genRndTriePrefix(maxL, Sigma, ClosedP=False, safe=True):
     """Generates a random trie automaton for a finite (either prefix free or prefix closed) language with a given
     length for max word
-    :param int maxL: length of the max word
-    :param set Sigma: alphabet to be used
-    :param bool ClosedP: should it be a prefix closed language?
-    :param bool safe: should a word of size maxl be present in every language?
-    :return: the generated trie automaton
-    :rtype: ADFA"""
+
+    Args:
+        maxL (int): length of the max word
+        Sigma (set): alphabet to be used
+        ClosedP (bool): should it be a prefix closed language?
+        safe (bool): should a word of size maxl be present in every language?
+    Returns:
+        ADFA: the generated trie automaton """
 
     def _genEnsurance(m, alphabet):
         l = len(alphabet)
         sl = list(alphabet)
         return [sl[random.randint(0, l - 1)] for _ in range(m)]
 
     def _descend(s1, ens, saf, m):
@@ -1425,42 +1530,45 @@
     _descend(s, ensurance, safe, maxL)
     return trie
 
 
 def DFAtoADFA(aut):
     """Transforms an acyclic DFA into a ADFA
 
-    :param DFA aut: the automaton to be transformed
-    :raises notAcyclic: if the DFA is not acyclic
-    :returns: the converted automaton
-    :rtype: ADFA"""
-    new = deepcopy(aut)
+    Args:
+        aut (DFA): the automaton to be transformed
+    Returns:
+        ADFA: the converted automaton
+    Raises:
+        notAcyclic: if the DFA is not acyclic """
+    new = copy.deepcopy(aut)
     new.trim()
     if not new.acyclicP(True):
         raise notAcyclic()
     afa = ADFA()
-    afa.States = copy(new.States)
-    afa.Sigma = copy(new.Sigma)
+    afa.States = copy.copy(new.States)
+    afa.Sigma = copy.copy(new.Sigma)
     afa.Initial = new.Initial
-    afa.delta = copy(new.delta)
-    afa.Final = copy(new.Final)
+    afa.delta = copy.copy(new.delta)
+    afa.Final = copy.copy(new.Final)
     afa.complete()
     return afa
 
 
 def stringToADFA(s):
     """Convert a canonical string representation of a ADFA to a ADFA
-    :param list s: the string in its canonical order
-    :returns: the ADFA
-    :rtype: ADFA
+
+    Args:
+        s (str): the string in its canonical order
+    Returns:
+        ADFA: the ADFA
 
     .. seealso::
         Marco Almeida, Nelma Moreira, and Rogério Reis. Exact generation of minimal acyclic deterministic finite
-        automata. International Journal of Foundations of Computer Science, 19(4):751-765, August 2008.
-    """
+        automata. International Journal of Foundations of Computer Science, 19(4):751-765, August 2008. """
     k = len(s[0]) - 1
     new = ADFA()
     new.setSigma([str(c) for c in range(k)])
     for st, sts in enumerate(s):
         new.addState(str(st))
         for c, s1 in enumerate(sts[:-1]):
             new.addTransition(st, str(c), s1)
@@ -1475,23 +1583,26 @@
 def dfa_block(m, sigma=["a", "b"]):
     return sigmaInitialSegment(sigma, m, True)
 
 
 def dfa_maxlen(m, sigma=["a", "b"]):
     return sigmaInitialSegment(sigma, m)
 
-def coBlockDFA(a, n):
-    """
-    :param DFA a: automaton accepting fixed length words
-    :param int n: length of words accepted, n > 0
-    :rtype DFA: accepts the words of length n not accepted by a
+def coBlockDFA(a: fa.DFA, n: int) -> fa.DFA:
     """
+    Args:
+        a (DFA): automaton accepting fixed length words
+        n (int): length of words accepted, n > 0
+    Returns:
+        DFA: accepts the words of length n not accepted by a
+
+    .. versionadded:: 2.1.2 """
 
     def _addStates(a, n, k):
-        # Invoked using k s.t. k-1 = 1st level of a state with a missing transition
+        # Invoked using k blksz.t. k-1 = 1st level of a state with a missing transition
         # then new states added at levels k,...,n and new transitions from each
         # new state to the new one of the next level using all symbols as labels
         if k > n:
             return
         newst = {}
         for i in range(k, n+1):
             newst[i] = a.addState()
@@ -1524,12 +1635,365 @@
         sss = ssq
     return coa.trim()
 
 
 def blockUniversalP(a, n):
     """
     Args:
-         a (NFA): block NFA (= NFA accepting only words of same length)
+         a (NFA): blksz NFA (= NFA accepting only words of same length)
          n (int): length of accepted words
     Returns:
-        bool: whether a is block universal (accepts all words of length n)"""
+        bool: whether a is blksz universal (accepts all words of length n)
+
+    .. versionadded: 2.1.2"""
     return coBlockDFA(a.toDFA(), n).emptyP()
+
+
+class BitString(object):
+    """ Class to represent the bitstring of a block language
+
+    :var blocksize: the size of the block
+    :var alphsize: the size of the alphabet
+    :var bst: the bitstring representation of the language
+
+    .. versionadded: 2.1.3
+    """
+    def __init__(self,blksz, alphsize, bst=None):
+        self.blocksize = blksz
+        self.alphsize = alphsize
+        if bst is not None:
+            self.bst = bitarray(bst)
+        else:
+            self.bst = bitarray(alphsize**blksz)
+
+
+    def strb(self):
+        return "".join([str(self.bst[i]) for i in range(len(self.bst))])
+
+    def minDFA(self):
+        def _nonnullname(n):
+            for i in n:
+                if i != "0":
+                    return True
+            return False
+
+        def _partName(n, k, c):
+            p = len(n) // k
+            return n[p*c:p*(c+1)]
+
+        lastDone = False
+        whole = self.strb()
+        aut = fa.DFA()
+        todo, done = set(), set()
+        idx = idx = aut.addState(whole)
+        aut.setInitial(idx)
+        todo.add(idx)
+        while todo:
+            idx = todo.pop()
+            done.add(idx)
+            for c in range(self.alphsize):
+                n = _partName(aut.States[idx], self.alphsize, c)
+                if _nonnullname(n):
+                    id1 = aut.stateIndex(n, True)
+                    if len(n) == 1:
+                        if not lastDone:
+                            aut.setFinal([id1])
+                            lastDone = True
+                    elif id1 not in done:
+                        todo.add(id1)
+                    aut.addTransition(idx, str(c), id1)
+        return aut
+
+        si = aut.addState(self.strb())
+        aut.setInitial(si)
+
+    def minNFA(self):
+        aut = ANFA()
+        sti1 = aut.addState('final')
+        aut.addFinal(sti1)
+        m = {frozenbitarray('1'): sti1}
+        d= {frozenbitarray('1'): {frozenbitarray('1')}}
+        PreviousStatesID = {frozenbitarray('0'), frozenbitarray('1')}
+        for ri in range(1, self.blocksize + 1):
+            idsize = self.alphsize ** ri
+            states_id = [self.bst[k * idsize: (k + 1) * idsize] for k in range(self.alphsize ** self.blocksize // idsize)]
+            states_id = {y for y in [frozenbitarray(x) for x in states_id] if y.any()}
+            left = 0
+            right = len(states_id)
+            coverSize = -1
+            coverModel = None
+            while left <= right:
+                mid = (left + right) // 2
+                r = _coverOfSizeN(states_id, PreviousStatesID, mid, self.alphsize, idsize)
+                if r:
+                    coverSize = mid
+                    coverModel = r
+                    right = mid - 1
+                else:
+                    left = mid + 1
+            if coverSize == -1:
+                raise NFAerror(
+                    f'no cover found for StatesID: {states_id}, PreviousStatesID: {PreviousStatesID}')
+            cover = coverModel[0]
+            statesCover = coverModel[1]
+            for StateID in cover:
+                if ri < self.blocksize:
+                    sti1 = aut.addState()
+                else:
+                    sti1 = aut.addState('start')
+                    aut.setInitial({sti1})
+                m[StateID] = sti1
+                ImageIDsize = idsize // self.alphsize
+                ImagesStateID = [StateID[k * ImageIDsize: (k + 1) * ImageIDsize] for k in range(self.alphsize)]
+                for sigma, ImageStateID in zip(range(self.alphsize), ImagesStateID):
+                    if all(not b for b in ImageStateID):
+                        continue
+                    for CoverImageStateID in d[ImageStateID]:
+                        foo_ = m[CoverImageStateID]
+                        aut.addTransition(sti1, sigma, foo_)
+            for StateID, CoverStateID in zip(states_id, statesCover):
+                d[StateID] = CoverStateID
+            PreviousStatesID = states_id
+        return aut
+
+    def _notNull(self, v):
+        for i in v:
+            if v != 0:
+                return True
+        return Fa
+    def reverse(self):
+        """ Compute the BitString representation of the reverse of the current language.
+
+        .. versionadded: 2.1.3"""
+        s = self.bst
+        r = _allShuffle(self.alphsize, self.blocksize, s)
+        return BitString(self.blocksize, self.alphsize, r)
+
+    def _reverseGD(self):
+        """ Compute the BitString representation of the reverse of the current language.
+
+        .. versionadded: 2.1.3
+
+        .. note::
+           This version computes the reverse directly but is approximately 10 times slower than the other version"""
+        l = self.alphsize**self.blocksize
+        n = [0 for _i in range(l)]
+        for i in range(l):
+            ib = pad(self.blocksize, inBase(i, self.alphsize))
+            ib.reverse()
+            n[fromBase(ib, self.alphsize)] = self.bst[i]
+        return BitString(self.blocksize, self.alphsize, n)
+
+
+def _coverOfSizeN(vs, pv, n, k, l):
+    bvv = [BitVecVal(ba2int(v), l) for v in vs]
+    pv_ = [ba.to01() for ba in (pv.union({frozenbitarray(l // k)}))]
+    s = [''.join(id) for id in product(pv_, repeat=k)]
+    bvs = [BitVecVal(int(x, 2), l) for x in s]
+    f = BitVecVal(0, l)
+    Ssize = len(s)
+    subset = [Bool(f'x{i}') for i in range(Ssize)]
+    subsetv = []
+    for v in vs:
+        subsetv.append([Bool(f'x{v},{i}') for i in range(Ssize)])
+    solver = Solver()
+    solver.add(Sum(subset) == n)  # subset of size n
+    for i, v in enumerate(bvv):
+        ored = f
+        for j in range(Ssize):
+            solver.add(Implies(subsetv[i][j], subset[j]))  # if subseti[i][j] then subset[j]
+            ored = ored | If(subsetv[i][j], bvs[j], f)  # there must be a sub-subset that Or'ed together equals v
+        solver.add(ored == v)
+    if solver.check() == sat:
+        model = solver.model()
+        result_subset = [frozenbitarray(s[i]) for i in range(Ssize) if is_true(model[subset[i]])]
+        result_subsetv = []
+        for i, _ in enumerate(vs):
+            result_subsetv.append([frozenbitarray(s[j]) for j in range(Ssize) if is_true(model[subsetv[i][j]])])
+        return result_subset, result_subsetv
+    else:
+        return None
+
+def genRndBitString(b: int, k: int) -> BitString:
+    """Generates a random bitstring with alphabet size k and block size b
+
+    Args:
+        b (int): The size of the block
+        k (int): The size of the alphabet
+    Returns:
+        bitarray: the random bitstring
+
+    .. versionadded: 2.1.4"""
+    new = BitString(b, k)
+    for i in range(k**b):
+        new.bst[i]=random.randint(0,1)
+    return new
+
+
+def _pShuffle(k: int, s: int, l: bitarray) -> bitarray:
+    """ Performs a perfect shuffle on a list assumming k to be the size of the alphabet and blksz the lenght of the slices
+        being shuffled
+
+    Args:
+        k (int): the size of the alphabet
+        blksz (int): the size of the slices
+        l (bitarray): the list to be shuffled
+    Returns:
+        bitarray: the shuffled list
+
+    .. versionadded: 2.1.3"""
+    l1, l3 = len(l)//k, 0
+    l2 = [i*l1 for i in range(k)]
+    new = bitarray()
+    while l3 < l1:
+        for i in l2:
+            _x,_y = i+l3, i+l3+s
+            new.extend(l[i+l3:i+l3+s])
+        l3 += s
+    return new
+
+
+def _allShuffle(k: int, blksz: int, l: bitarray) -> bitarray:
+    """ Perform the complete reversal of a bitstring l of a language where k is the size of the alphabet, blksz is
+        the size of the block
+
+    Args:
+        k (int): the size of the alphabet
+        blksz (int): the size of the block
+        l (bitarray): the bitstring of the language
+    Returns:
+        bitarray: the bitstring of the reversed language
+
+    .. versionadded: 2.1.3"""
+    blksz = blksz-1
+    assert len(l) % (k**(blksz-1)) == 0
+    n = l.copy()
+    for i in range(0, blksz):
+        n = _pShuffle(k, k ** i, n)
+    return n
+
+def firstBlockWords(alpzs: int, nwords: int, blksz: int) -> ADFA:
+    """ Generates the minimal ADFA that accepts exactly the first nwords (lexicographic order) of a blksz language
+
+    Args:
+        alpzs (int): alphabet size
+        nwords (int): number of words
+        blksz (int): blksz size
+    Returns:
+        ADFA: the ADFA that recognises exacly those words
+
+    .. versionadded: 2.1.3"""
+    assert 0 < nwords < alpzs**blksz+1
+    rl = padList(inBase(nwords-1, alpzs),blksz)
+    for i in range(blksz):
+        if rl[blksz-1-i] != alpzs-1:
+            break
+    triv, opt = i, i
+    if triv == 0:
+        triv = 1
+    aut = ADFA()
+    aut.setSigma(list(range(alpzs)))
+    ini = aut.addState()
+    aut.setInitial(ini)
+    main, border = ini, ini
+    div, order = False, 0
+    for i in rl[:-triv]:
+        ns = aut.addState()
+        if main == border:
+            if i == 0:
+                aut.addTransition(main,0,ns)
+                main, border = ns, ns
+            else:
+                if opt != 0 and order + triv + 1 == blksz:
+                    for j in range(i + 1):
+                        aut.addTransition(main, j, ns)
+                    main, border = ns, ns
+                else:
+                    for j in range(i):
+                        aut.addTransition(main, j, ns)
+                    div = True
+                    nb =  aut.addState()
+                    aut.addTransition(border, i, nb)
+                    main, border = ns, nb
+        else: # already diverged
+            for j in range(alpzs):
+                aut.addTransition(main, j, ns)
+            for j in range(i):
+                aut.addTransition(border, j, ns)
+            if opt != 0 and order + triv + 1 == blksz:
+                aut.addTransition(border, i, ns)
+                main, border = ns, ns
+            else:
+                nb = aut.addState()
+                aut.addTransition(border, i, nb)
+                main, border = ns, nb
+        order += 1
+    # now deal with the last symbols and its obtimisation
+    while triv != 0:
+        ns = aut.addState()
+        if div:
+            for j in range(alpzs):
+                aut.addTransition(main, j, ns)
+            if border != main:
+                for j in range(rl[-triv]+1):
+                    aut.addTransition(border, j, ns)
+        else:
+            for j in range(rl[-triv]+1):
+                aut.addTransition(main, j, ns)
+        main, border = ns, ns
+        triv -= 1
+    aut.setFinal([ns])
+    return aut
+
+
+def generateBlockTrie(sz: int, alpsz: int) -> ADFA:
+    """Generates a trie for a blksz language
+
+    Args:
+        sz (int): size of the blksz
+        alpsz (int): size of the alphabet
+    Returns:
+        ADFA: the automaton
+
+    .. versionadded:: 2.1.3 """
+    aut = ADFA()
+    aut.setSigma(list(range(alpsz)))
+    sti = aut.addState()
+    aut.setInitial(sti)
+    l = [sti]
+    for i in range(sz):
+        ln = []
+        for st in l:
+            for c in range(alpsz):
+                sti = aut.addState()
+                ln.append(sti)
+                aut.addTransition(st, c, sti)
+        l = ln
+    aut.setFinal(l)
+    return aut
+
+class BlockWords(object):
+    """Block language iterator"""
+    def __init__(self, k:int, b:int):
+        self.k = k
+        self.b = b
+        self.first = True
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self.first:
+            self.s = [0] * self.b
+            self.first = False
+            return self.s
+        y = self._sequent(self.s)
+        if y is None:
+            raise StopIteration
+        self.s = y
+        return self.s
+
+    def _sequent(self, s):
+        for i in range(self.b):
+            if s[self.b-1-i] != self.k-1:
+                return s[:self.b-i-1]+[s[self.b-i-1]+1]+[0]*i
+        return None
```

### Comparing `fado-2.1.2/FAdo/graphs.py` & `fado-2.2.0/FAdo/graphs.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/prax.py` & `fado-2.2.0/FAdo/prax.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/reex.py` & `fado-2.2.0/FAdo/reex.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/regexp_grammar.lark` & `fado-2.2.0/FAdo/regexp_grammar.lark`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/rndadfa.py` & `fado-2.2.0/FAdo/rndadfa.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,28 @@
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.
 
    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA."""
 
+#  Copyright (c) 2023. Rogério Reis <rogerio.reis@fc.up.pt> and Nelma Moreira <nelma.moreira@fc.up.pt>.
+#
+#  This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
+
 from . fa import stringToDFA, DFA
+from . fl import ADFA
 
 from random import randint
 from functools import reduce
+from . common import ParRangError
 
 
 class ADFArnd():
     """ Sets a random generator for Adfas by sources. By default,  s=1 to be initially connected
     
     :var int n: number of states
     :var int k: size of the alphabet
@@ -322,22 +332,60 @@
     if (n, k) not in c_adfa:
         c_adfa[(n, k)] = sum(
             [((-1) ** (n - j)) * binomial(n - 1, j - 1) * ((j + 1) ** (k * (n - j))) * countafaL(j, k, 1) for j in
              range(1, n + 1)])
     return c_adfa[(n, k)]
 
 
-def countadfa(n, k):
+def countadfa(n: int, k: int):
     """  Acyclic (complete) deterministic finite automata  structure (unlabeled)
 
-    :arg n: number of states
-    :arg k: alphabetic size
-    :type n: int
-    :type k: int"""
+    Args:
+        (int) n: number of states
+        (int) k: alphabetic size """
     return countadfaL(n, k) / reduce(lambda x, y: x * y, list(range(1, n)))
 
 
-def tab_adfa(n1, n2, k1, k2):
+def tab_adfa(n1: int , n2: int, k1: int, k2: int) -> None:
     for k in range(k1, k2 + 1):
         print("k=%d" % k)
         for n in range(n1, n2 + 1):
             print("n=%d\t %s" % (n, countadfa(n, k) * 2 ** n))
+
+
+def _genDiff(n: int, b: int, k: int) -> list:
+    r = []
+    for j in range(n):
+        x = [randint(0,k-1) for i in range(b)]
+        while x in r:
+            x = [randint(0,k-1) for i in range(b)]
+        r.append(x)
+    return r
+
+
+def  rndBlockADFA(alpzs: int, nwords: int, blksz: int) -> ADFA:
+    """ Random generation of a block language
+
+    Args:
+        alpzs (int): alphabet size
+        nwords (int): desired number of words
+        blksz (int): desired size of the block
+    Returns:
+        AFDA: the random block language
+
+    .. versionadded:: 2.1.3"""
+    if nwords > alpzs**blksz:
+        raise ParRangError()
+    words = _genDiff(nwords, blksz, alpzs)
+    aut = ADFA()
+    aut.setSigma(list(range(alpzs)))
+    init = aut.addState()
+    fin = aut.addState()
+    aut.setInitial(init)
+    aut.addFinal(fin)
+    for w in words:
+        st = init
+        for c in w[:-1]:
+            st = aut.addTransitionIfNeeded(st, c)
+        aut.addTransition(st, w[-1], fin)
+    return aut.minimal()
+
```

### Comparing `fado-2.1.2/FAdo/rndfap.py` & `fado-2.2.0/FAdo/rndfap.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/ska.py` & `fado-2.2.0/FAdo/ska.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/smwc.py` & `fado-2.2.0/FAdo/smwc.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/ssemigroup.py` & `fado-2.2.0/FAdo/ssemigroup.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/sst.py` & `fado-2.2.0/FAdo/sst.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/tfa.py` & `fado-2.2.0/FAdo/tfa.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/transducers.py` & `fado-2.2.0/FAdo/transducers.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/unionFind.py` & `fado-2.2.0/FAdo/unionFind.py`

 * *Files identical despite different names*

### Comparing `fado-2.1.2/FAdo/witness.py` & `fado-2.2.0/FAdo/witness.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,41 @@
     f.addTransition(0, Sigma[0], 1)
     for i in range(1, m):
         f.addTransition(i, Sigma[0], (i + 1) % m)
         f.addTransition(i, Sigma[1], i)
         f.addTransition(i, Sigma[1], 0)
     return f
 
+def reversalDFAWC2MF(m=5,Sigma=["a","b"]):
+    """ Worst case automata for NFA-> DFA-> reversal DFA with n > 2, k=2
+        ..seealso::
+        A. r. Meyer and M. J. Fischer. Economy of description by automata,
+        grammars, and formal systems. Twelfth Annual Symposium on
+        Switching and Automata Theory, 1971,  188–191. IEEE Society Press.
+
+        :param m: number of states
+        :type m: integer
+        :param Sigma: alphabet
+        :return: a dfa
+        :rtype: NFA"""
+    if m < 3:
+        raise TstError("Number of states must be greater than 2")
+    if len(Sigma) != 2:
+        raise TstError("Alphabet must be binary")
+    f = NFA()
+    f.setSigma(Sigma)
+    f.States = list(range(m))
+    f.setInitial([0])
+    f.addFinal(0)
+    f.addTransition(0, Sigma[0], m-1)
+    for i in range(1, m):
+        f.addTransition(i, Sigma[0], (i - 1) % m)
+        f.addTransition(i, Sigma[1], i)
+        f.addTransition(0, Sigma[1], i)
+    return f
 
 def toDFAWCReMF(m=5, Sigma=["a", "b"]):
     """
     Same as toDFAWC2MF as regular expression
     :param m:
     :param Sigma: alphabet
     :return:
@@ -442,15 +469,15 @@
     d1.States = list(range(m))
     d1.setInitial(0)
     d1.addFinal(0)
     for i in range(m):
         d1.addTransition(i, "a", (i + 1) % m)
         d1.addTransition(i, "b", i)
     d2.setSigma(["a", "b"])
-    d2.States = list(range(m))
+    d2.States = list(range(n))
     d2.setInitial(0)
     d2.addFinal(0)
     for i in range(n):
         d2.addTransition(i, "b", (i + 1) % n)
         d2.addTransition(i, "a", i)
     return d1, d2
 
@@ -476,15 +503,15 @@
     d1.addTransition(0, "a", 1)
     d1.addTransition(0, "b", 0)
     for i in range(1, m):
         d1.addTransition(i, "a", (i + 1) % m)
         d1.addTransition(i, "b", i)
         d1.addFinal(i)
     d2.setSigma(["a", "b"])
-    d2.States = list(range(m))
+    d2.States = list(range(n))
     d2.setInitial(0)
     d2.addTransition(0, "b", 1)
     d2.addTransition(0, "a", 0)
     for i in range(n):
         d2.addTransition(i, "b", (i + 1) % n)
         d2.addTransition(i, "a", i)
     d2.addFinal(0)
```

### Comparing `fado-2.1.2/README.rst` & `fado-2.2.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -15,33 +15,45 @@
 -----------------
 
 It currently includes most standard operations for the manipulation of regular languages. Regular languages can
 be represented by regular expressions (RegExp) or finite automata, among other formalisms. Finite automata may
 be deterministic (DFA), non-deterministic (NFA) or generalized (GFA). In **FAdo** these representations are implemented
 as Python classes.
 
+
+
 Elementary regular languages operations as union, intersection, concatenation, complementation and reverse are
-implemented for each class. Also several combined operations are available for specific models.
+implemented for each class. Also several other regular operations (e.g shuffle) and combined operations are available for specific models.
+
+
+
+* Several conversions between these representations are implemented:
+
+  * NFA -> DFA: subset construction
 
-Several conversions between these representations are implemented:
+  * NFA -> RE: recursive method
 
-* NFA -> DFA: subset construction
+  * GFA -> RE: state elimination, with possible choice of state orderings (several heuristics)
 
-* NFA -> RE: recursive method
+  * RE -> NFA: Thompson, Glushkov/Position, epsilon-Follow, Follow, Partial Derivatives (naive and compressed RE), Prefix; and their duals.
 
-* GFA -> RE: state elimination, with possible choice of state orderings
+  * SRE -> DFA: Brzozowski (SRE are RegExp ACIA, using sets)
 
-* RE -> NFA: Thompson method, Glushkov method, follow, Brzozowski, and partial derivatives.
+  * RE -> DFA: AuPoint (Marked before)  and YMG (Marked after)
 
 * For DFAs several minimization algorithms are available: Moore, Hopcroft, and some incremental algorithms. Brzozowski minimization is available for NFAs.
 
 * An algorithm for hyper-minimization of DFAs
 
+* For DFAs tests for reversability   
+
 * Language equivalence of two DFAs can be determined by reducing their correspondent minimal DFA to a canonical form, or by the Hopcroft and Karp algorithm.
 
+* For NFAs reductions by left and right  bisimilarity
+
 * Enumeration of the first words of a language or all words of a given length (Cross Section)
 
 * Some support for the transition semigroups of DFAs
 
 ----------------
 Finite Languages
 ----------------
@@ -51,14 +63,16 @@
 * Construction of a ADFA (acyclic finite automata) from a set of words
 
 * Minimization of ADFAs
 
 * Several methods for ADFAs random generation
 
 * Methods for deterministic cover finite automata (DCFA)
+  
+* Special methods for Block languages where all words have the same length
 
 -----------
 Transducers
 -----------
 
 Several methods for transducers in standard form (SFT) are available:
 
@@ -79,8 +93,21 @@
 * Maximality i.e. the language satisfies the property and is maximal
 
 * Properties implemented by transducers include: input preserving, input altering, trajectories, and fixed properties
 
 * Computation of the edit distance of a regular language, using input altering transducers
 
 
+----
+PRAX
+----
+
+Polynomial Random Approximation Algorithms allow to decide hard automata problems considering cetrain natural distributions on set of words.
+
+In particular, using the notion of approximate universality
+
+* Test NFA universality for finite languagens
+
+* Test NFA universality for infinite languages using tractable word distributions (Lambert and Dirichlet)  
 
+  
+
```

### Comparing `fado-2.1.2/pyproject.toml` & `fado-2.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 [tool.poetry]
 name = "FAdo"
-version = "2.1.2"
+version = "2.2.0"
 packages = [{ include = "FAdo" }]
 description = "A library of tools to manipulate formal languages' representations  mainly automata and regular expressions."
 authors = ["Rogerio Reis <rogerio.reis@fc.up.pt>", "Nelma Moreira <nelma.moreira@fc.up.pt"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://fado.dcc.fc.up.pt"
 documentation = "https://www.dcc.fc.up.pt/~rvr/FAdoDoc"
-keywords = ["automata theory", "formal languages", "regular expressions", "transducers"]
+keywords = ["automata_theory",
+    "formal_languages",
+    "regular_expressions",
+    "transducers"]
 exclude = ["FAdo/madfa.py",
     "FAdo/.idea",
     "FAdo/aggregation.py",
     "FAdo/aggregationFast.py",
-    "FAdo/avl.c", "FAdo/avl.h", "FAdo/coreFA.c", "FAdo/coreFA.h", "FAdo/coreFA_setup.py", "FAdo/generator.c",
-    "FAdo/generator.h", "FAdo/generator_setup-linux.py", "FAdo/generator_setup-mac.py", "FAdo/icdfa.c",
-    "FAdo/icdfa.h", "FAdo/icdfaCommon.h", "FAdo/icdfaGen.h", "FAdo/icdfaGen.c", "FAdo/rndfa.py", "FAdo/zset.h",
-    "FAdo/boltzmann.py", "FAdo/icdfaboltz.py",
+    "FAdo/avl.c", "FAdo/avl.h",
+    "FAdo/coreFA.c",
+    "FAdo/coreFA.h",
+    "FAdo/coreFA_setup.py",
+    "FAdo/generator.c",
+    "FAdo/generator.h",
+    "FAdo/generator_setup-linux.py",
+    "FAdo/generator_setup-mac.py",
+    "FAdo/icdfa.c",
+    "FAdo/icdfa.h",
+    "FAdo/icdfaCommon.h",
+    "FAdo/icdfaGen.h",
+    "FAdo/icdfaGen.c",
+    "FAdo/rndfa.py",
+    "FAdo/zset.h",
+    "FAdo/boltzmann.py",
+    "FAdo/icdfaboltz.py",
     "FAdo/cliques.py",
     "FAdo/fractran.py",
     "FAdo/genMatrix.py",
     "FAdo/ipython.py",
     "FAdo/ILaser_gen.py",
     "FAdo/Makefile",
     "FAdo/nfaextra.py",
-    "FAdo/peg.py", "FAdo/tdpl.py",
-    "FAdo/pddag.py", "FAdo/pdkoz.py",
+    "FAdo/peg.py",
+    "FAdo/tdpl.py",
+    "FAdo/pddag.py",
+    "FAdo/pdkoz.py",
     "FAdo/enumlang.py",
     "FAdo/autshuffle.py",
     "FAdo/samplereex.py",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -41,14 +59,16 @@
 black = "^22.1.0"
 platformdirs = "^2.5.0"
 prompt-toolkit = "^3.0.27"
 tomli = "^2.0.1"
 jupyter = "^1.0.0"
 mistune = "^2.0.2"
 lark = "^1.1.5"
+bitarray = "^2.9.2"
+z3-solver = "^4.12.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -59,7 +79,13 @@
 testpaths = ["tests"]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
     "anyio"
 
 ]
+
+[tool.poetry_bumpversion.file."FAdo/__init__.py"]
+
+[tool.poetry.scripts]
+my_package_cli = 'my_package.console:run'
+
```

### Comparing `fado-2.1.2/PKG-INFO` & `fado-2.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
-Name: fado
-Version: 2.1.2
+Name: FAdo
+Version: 2.2.0
 Summary: A library of tools to manipulate formal languages' representations  mainly automata and regular expressions.
 Home-page: https://fado.dcc.fc.up.pt
 License: GPL-3.0-or-later
-Keywords: automata theory,formal languages,regular expressions,transducers
+Keywords: automata_theory,formal_languages,regular_expressions,transducers
 Author: Rogerio Reis
 Author-email: rogerio.reis@fc.up.pt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: bitarray (>=2.9.2,<3.0.0)
 Requires-Dist: black (>=22.1.0,<23.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: graphviz (>=0.19.1,<0.20.0)
 Requires-Dist: ipython (>=7.0.0,<8.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: mistune (>=2.0.2,<3.0.0)
 Requires-Dist: networkx (>=2.6.3,<3.0.0)
 Requires-Dist: platformdirs (>=2.5.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.27,<4.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: z3-solver (>=4.12.5.0,<5.0.0.0)
 Project-URL: Documentation, https://www.dcc.fc.up.pt/~rvr/FAdoDoc
 Description-Content-Type: text/x-rst
 
 =============
 What is FAdo?
 =============
 
@@ -44,33 +47,45 @@
 -----------------
 
 It currently includes most standard operations for the manipulation of regular languages. Regular languages can
 be represented by regular expressions (RegExp) or finite automata, among other formalisms. Finite automata may
 be deterministic (DFA), non-deterministic (NFA) or generalized (GFA). In **FAdo** these representations are implemented
 as Python classes.
 
+
+
 Elementary regular languages operations as union, intersection, concatenation, complementation and reverse are
-implemented for each class. Also several combined operations are available for specific models.
+implemented for each class. Also several other regular operations (e.g shuffle) and combined operations are available for specific models.
+
+
+
+* Several conversions between these representations are implemented:
+
+  * NFA -> DFA: subset construction
 
-Several conversions between these representations are implemented:
+  * NFA -> RE: recursive method
 
-* NFA -> DFA: subset construction
+  * GFA -> RE: state elimination, with possible choice of state orderings (several heuristics)
 
-* NFA -> RE: recursive method
+  * RE -> NFA: Thompson, Glushkov/Position, epsilon-Follow, Follow, Partial Derivatives (naive and compressed RE), Prefix; and their duals.
 
-* GFA -> RE: state elimination, with possible choice of state orderings
+  * SRE -> DFA: Brzozowski (SRE are RegExp ACIA, using sets)
 
-* RE -> NFA: Thompson method, Glushkov method, follow, Brzozowski, and partial derivatives.
+  * RE -> DFA: AuPoint (Marked before)  and YMG (Marked after)
 
 * For DFAs several minimization algorithms are available: Moore, Hopcroft, and some incremental algorithms. Brzozowski minimization is available for NFAs.
 
 * An algorithm for hyper-minimization of DFAs
 
+* For DFAs tests for reversability   
+
 * Language equivalence of two DFAs can be determined by reducing their correspondent minimal DFA to a canonical form, or by the Hopcroft and Karp algorithm.
 
+* For NFAs reductions by left and right  bisimilarity
+
 * Enumeration of the first words of a language or all words of a given length (Cross Section)
 
 * Some support for the transition semigroups of DFAs
 
 ----------------
 Finite Languages
 ----------------
@@ -80,14 +95,16 @@
 * Construction of a ADFA (acyclic finite automata) from a set of words
 
 * Minimization of ADFAs
 
 * Several methods for ADFAs random generation
 
 * Methods for deterministic cover finite automata (DCFA)
+  
+* Special methods for Block languages where all words have the same length
 
 -----------
 Transducers
 -----------
 
 Several methods for transducers in standard form (SFT) are available:
 
@@ -108,9 +125,22 @@
 * Maximality i.e. the language satisfies the property and is maximal
 
 * Properties implemented by transducers include: input preserving, input altering, trajectories, and fixed properties
 
 * Computation of the edit distance of a regular language, using input altering transducers
 
 
+----
+PRAX
+----
+
+Polynomial Random Approximation Algorithms allow to decide hard automata problems considering cetrain natural distributions on set of words.
+
+In particular, using the notion of approximate universality
+
+* Test NFA universality for finite languagens
+
+* Test NFA universality for infinite languages using tractable word distributions (Lambert and Dirichlet)  
 
+  
+
```

