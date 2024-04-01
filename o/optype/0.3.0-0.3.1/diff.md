# Comparing `tmp/optype-0.3.0.tar.gz` & `tmp/optype-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optype-0.3.0.tar", max compression
+gzip compressed data, was "optype-0.3.1.tar", max compression
```

## Comparing `optype-0.3.0.tar` & `optype-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1505 2024-01-28 23:47:55.624920 optype-0.3.0/LICENSE
--rw-r--r--   0        0        0    40871 2024-03-21 20:06:54.708302 optype-0.3.0/README.md
--rw-r--r--   0        0        0     9442 2024-03-21 20:06:54.536298 optype-0.3.0/optype/__init__.py
--rw-r--r--   0        0        0    18891 2024-03-21 20:06:54.540298 optype-0.3.0/optype/_can.py
--rw-r--r--   0        0        0     6316 2024-03-21 20:06:54.540298 optype-0.3.0/optype/_do.py
--rw-r--r--   0        0        0    13819 2024-03-21 20:06:54.540298 optype-0.3.0/optype/_does.py
--rw-r--r--   0        0        0     2145 2024-03-21 20:06:54.540298 optype-0.3.0/optype/_has.py
--rw-r--r--   0        0        0        0 2024-01-28 23:47:08.164059 optype-0.3.0/optype/py.typed
--rw-r--r--   0        0        0     5656 2024-03-21 20:06:54.708302 optype-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    41291 1970-01-01 00:00:00.000000 optype-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-01-28 23:47:55.624920 optype-0.3.1/LICENSE
+-rw-r--r--   0        0        0    42333 2024-04-01 18:53:22.419171 optype-0.3.1/README.md
+-rw-r--r--   0        0        0     9442 2024-03-21 20:06:54.536298 optype-0.3.1/optype/__init__.py
+-rw-r--r--   0        0        0    18908 2024-04-01 18:53:22.419171 optype-0.3.1/optype/_can.py
+-rw-r--r--   0        0        0     6166 2024-04-01 18:53:22.419171 optype-0.3.1/optype/_do.py
+-rw-r--r--   0        0        0    13819 2024-03-21 20:06:54.540298 optype-0.3.1/optype/_does.py
+-rw-r--r--   0        0        0     2145 2024-03-21 20:06:54.540298 optype-0.3.1/optype/_has.py
+-rw-r--r--   0        0        0        0 2024-01-28 23:47:08.164059 optype-0.3.1/optype/py.typed
+-rw-r--r--   0        0        0     4733 2024-04-01 18:53:22.583175 optype-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    42751 1970-01-01 00:00:00.000000 optype-0.3.1/PKG-INFO
```

### Comparing `optype-0.3.0/LICENSE` & `optype-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optype-0.3.0/README.md` & `optype-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,55 @@
 
 ```shell
 pip install optype
 ```
 
 [OPTYPE]: https://pypi.org/project/optype/
 
+## Example
+
+Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
+Implementing it is trivial, but what about the type annotations?
+
+Because `twice(2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it
+might seem like a good idea to type it as `twice[T](x: T) -> T: ...`.
+However, that wouldn't include cases such as `twice(True) == 2` or
+`twice((42, True)) == (42, True, 42, True)`, where the input- and output types
+differ.
+Moreover, `twice` should accept *any* type with a custom `__rmul__` method
+that accepts `2` as argument.
+
+This is where `optype` comes in handy, which has single-method protocols for
+*all* the builtin special methods.
+For `twice`, we can use `optype.CanRMul[X, Y]`, which, as the name suggests,
+is a protocol with (only) the `def __rmul__(self, x: X) -> Y: ...` method.
+With this, the `twice` function can written as:
+
+```python
+import typing
+import optype
+
+type Two = typing.Literal[2]
+
+def twice[Y](x: optype.CanRMul[Two, Y], /) -> Y:
+    return 2 * x
+```
+
+But what about types that implement `__add__` but not `__radd__`?
+In this case, we could return `x * 2` as fallback.
+Because the `optype.Can*` protocols are runtime-checkable, the revised
+`twice2` function can be compactly written as:
+
+```python
+def twice2[Y](x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y:
+    return 2 * x if isinstance(x, optype.CanRMul) else x * 2
+```
+
+See [`examples/twice.py`](examples/twice.py) for the full example.
+
 ## Overview
 
 The API of `optype` is flat; a single `import optype` is all you need.
 There are four flavors of things that live within `optype`,
 
 - `optype.Can{}` types describe *what can be done* with it.
   For instance, any `CanAbs[T]` type can be used as argument to the `abs()`
```

#### html2text {}

```diff
@@ -1,32 +1,51 @@
                              ************ ooppttyyppee ************
                            One protocol, one method.
               Building blocks for precise & flexible type hints.
   _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_C_h_e_c_k_e_d_ _w_i_t_h
                                    _p_y_r_i_g_h_t_]
 --- ## Installation Optype is available as [`optype`][OPTYPE] on PyPI: ```shell
-pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Overview
-The API of `optype` is flat; a single `import optype` is all you need. There
-are four flavors of things that live within `optype`, - `optype.Can{}` types
-describe *what can be done* with it. For instance, any `CanAbs[T]` type can be
-used as argument to the `abs()` builtin function with return type `T`. Most
-`Can{}` implement a single special method, whose name directly matched that of
-the type. `CanAbs` implements `__abs__`, `CanAdd` implements `__add__`, etc. -
-`optype.Has{}` is the analogue of `Can{}`, but for special *attributes*.
-`HasName` has the `__name__: str` attribute, `HasDict` has a `__dict__`, etc. -
-`optype.Does{}` describe the *type of operators*. So `DoesAbs` is the type of
-the `abs({})` builtin function, and `DoesPos` the type of the `+{}` prefix
-operator. - `optype.do_{}` are the correctly-typed implementations of `Does{}`.
-For each `do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is
-the typed alias of `abs({})`, and `do_pos: DoesPos` is a typed version of
-`operator.pos`. The `optype.do_` operators are more complete than `operators`,
-has runtime-accessible type annotations, and uses a fully predictable naming
-scheme. ## Reference All [typing protocols][PC] here live in the root `optype`
-namespace. They are [runtime-checkable][RC] so that you can do e.g. `isinstance
-('snail', optype.CanAdd)`, in case you want to check whether `snail` implements
+pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Example
+Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
+Implementing it is trivial, but what about the type annotations? Because `twice
+(2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it might seem like a
+good idea to type it as `twice[T](x: T) -> T: ...`. However, that wouldn't
+include cases such as `twice(True) == 2` or `twice((42, True)) == (42, True,
+42, True)`, where the input- and output types differ. Moreover, `twice` should
+accept *any* type with a custom `__rmul__` method that accepts `2` as argument.
+This is where `optype` comes in handy, which has single-method protocols for
+*all* the builtin special methods. For `twice`, we can use `optype.CanRMul[X,
+Y]`, which, as the name suggests, is a protocol with (only) the `def __rmul__
+(self, x: X) -> Y: ...` method. With this, the `twice` function can written as:
+```python import typing import optype type Two = typing.Literal[2] def twice[Y]
+(x: optype.CanRMul[Two, Y], /) -> Y: return 2 * x ``` But what about types that
+implement `__add__` but not `__radd__`? In this case, we could return `x * 2`
+as fallback. Because the `optype.Can*` protocols are runtime-checkable, the
+revised `twice2` function can be compactly written as: ```python def twice2[Y]
+(x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y: return 2 * x if
+isinstance(x, optype.CanRMul) else x * 2 ``` See [`examples/twice.py`]
+(examples/twice.py) for the full example. ## Overview The API of `optype` is
+flat; a single `import optype` is all you need. There are four flavors of
+things that live within `optype`, - `optype.Can{}` types describe *what can be
+done* with it. For instance, any `CanAbs[T]` type can be used as argument to
+the `abs()` builtin function with return type `T`. Most `Can{}` implement a
+single special method, whose name directly matched that of the type. `CanAbs`
+implements `__abs__`, `CanAdd` implements `__add__`, etc. - `optype.Has{}` is
+the analogue of `Can{}`, but for special *attributes*. `HasName` has the
+`__name__: str` attribute, `HasDict` has a `__dict__`, etc. - `optype.Does{}`
+describe the *type of operators*. So `DoesAbs` is the type of the `abs({})`
+builtin function, and `DoesPos` the type of the `+{}` prefix operator. -
+`optype.do_{}` are the correctly-typed implementations of `Does{}`. For each
+`do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is the typed
+alias of `abs({})`, and `do_pos: DoesPos` is a typed version of `operator.pos`.
+The `optype.do_` operators are more complete than `operators`, has runtime-
+accessible type annotations, and uses a fully predictable naming scheme. ##
+Reference All [typing protocols][PC] here live in the root `optype` namespace.
+They are [runtime-checkable][RC] so that you can do e.g. `isinstance('snail',
+optype.CanAdd)`, in case you want to check whether `snail` implements
 `__add__`. > [!NOTE] > It is bad practice to use a [`typing.Protocol`][PC] as
 base class for your > implementation. Because of [`@typing.runtime_checkable`]
 [RC], you can use > `isinstance` either way. Unlike`collections.abc`,
 `optype`'s protocols aren't abstract base classes, i.e. they don't extend
 `abc.ABC`, only `typing.Protocol`. This allows the `optype` protocols to be
 used as building blocks for `.pyi` type stubs. [PC]: https://
 typing.readthedocs.io/en/latest/spec/protocol.html [RC]: https://
```

### Comparing `optype-0.3.0/optype/__init__.py` & `optype-0.3.1/optype/__init__.py`

 * *Files identical despite different names*

### Comparing `optype-0.3.0/optype/_can.py` & `optype-0.3.1/optype/_can.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 @runtime_checkable
 class CanLe[X, Y](Protocol):
     def __le__(self, __x: X) -> Y: ...
 
 
 @runtime_checkable
-class CanEq[X, Y](Protocol):
+class CanEq[X, Y](Protocol):  # noqa: PLW1641
     """
     Unfortunately, `typeshed` incorrectly annotates `object.__eq__` as
     `(Self, object) -> bool`.
     As a counter-example, consider `numpy.ndarray`. It's `__eq__` method
     returns a boolean (mask) array of the same shape as the input array.
     Moreover, `numpy.ndarray` doesn't even implement `CanBool` (`bool()`
     raises a `TypeError` for shapes of size > 1).
```

### Comparing `optype-0.3.0/optype/_do.py` & `optype-0.3.1/optype/_do.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,14 @@
 do_setattr: _d.DoesSetattr = setattr
 do_delattr: _d.DoesDelattr = delattr
 do_dir: _d.DoesDir = dir
 
 
 # callables
 
-# def do_call[**Xs, Y](
-#     func: _c.CanCall[Xs, Y],
-#     *args: Xs.args,
-#     **kwargs: Xs.kwargs,
-# ) -> Y:
-#     return func(*args, **kwargs)
-
 do_call: _d.DoesCall = _o.call
 
 
 # containers and sequences
 
 do_len: _d.DoesLen = len
 do_length_hint: _d.DoesLengthHint = _o.length_hint
```

### Comparing `optype-0.3.0/optype/_does.py` & `optype-0.3.1/optype/_does.py`

 * *Files identical despite different names*

### Comparing `optype-0.3.0/optype/_has.py` & `optype-0.3.1/optype/_has.py`

 * *Files identical despite different names*

### Comparing `optype-0.3.0/PKG-INFO` & `optype-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optype
-Version: 0.3.0
-Summary: Building blocks for precise & flexible Python type hints
+Version: 0.3.1
+Summary: Building blocks for precise type hints in Python 3.12+
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
@@ -68,14 +68,55 @@
 
 ```shell
 pip install optype
 ```
 
 [OPTYPE]: https://pypi.org/project/optype/
 
+## Example
+
+Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
+Implementing it is trivial, but what about the type annotations?
+
+Because `twice(2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it
+might seem like a good idea to type it as `twice[T](x: T) -> T: ...`.
+However, that wouldn't include cases such as `twice(True) == 2` or
+`twice((42, True)) == (42, True, 42, True)`, where the input- and output types
+differ.
+Moreover, `twice` should accept *any* type with a custom `__rmul__` method
+that accepts `2` as argument.
+
+This is where `optype` comes in handy, which has single-method protocols for
+*all* the builtin special methods.
+For `twice`, we can use `optype.CanRMul[X, Y]`, which, as the name suggests,
+is a protocol with (only) the `def __rmul__(self, x: X) -> Y: ...` method.
+With this, the `twice` function can written as:
+
+```python
+import typing
+import optype
+
+type Two = typing.Literal[2]
+
+def twice[Y](x: optype.CanRMul[Two, Y], /) -> Y:
+    return 2 * x
+```
+
+But what about types that implement `__add__` but not `__radd__`?
+In this case, we could return `x * 2` as fallback.
+Because the `optype.Can*` protocols are runtime-checkable, the revised
+`twice2` function can be compactly written as:
+
+```python
+def twice2[Y](x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y:
+    return 2 * x if isinstance(x, optype.CanRMul) else x * 2
+```
+
+See [`examples/twice.py`](examples/twice.py) for the full example.
+
 ## Overview
 
 The API of `optype` is flat; a single `import optype` is all you need.
 There are four flavors of things that live within `optype`,
 
 - `optype.Can{}` types describe *what can be done* with it.
   For instance, any `CanAbs[T]` type can be used as argument to the `abs()`
```

#### html2text {}

```diff
@@ -1,38 +1,57 @@
-Metadata-Version: 2.1 Name: optype Version: 0.3.0 Summary: Building blocks for
-precise & flexible Python type hints License: BSD-3-Clause Author: Joren
+Metadata-Version: 2.1 Name: optype Version: 0.3.1 Summary: Building blocks for
+precise type hints in Python 3.12+ License: BSD-3-Clause Author: Joren
 Hammudoglu Author-email: jhammudoglu@gmail.com Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
                              ************ ooppttyyppee ************
                            One protocol, one method.
               Building blocks for precise & flexible type hints.
   _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_C_h_e_c_k_e_d_ _w_i_t_h
                                    _p_y_r_i_g_h_t_]
 --- ## Installation Optype is available as [`optype`][OPTYPE] on PyPI: ```shell
-pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Overview
-The API of `optype` is flat; a single `import optype` is all you need. There
-are four flavors of things that live within `optype`, - `optype.Can{}` types
-describe *what can be done* with it. For instance, any `CanAbs[T]` type can be
-used as argument to the `abs()` builtin function with return type `T`. Most
-`Can{}` implement a single special method, whose name directly matched that of
-the type. `CanAbs` implements `__abs__`, `CanAdd` implements `__add__`, etc. -
-`optype.Has{}` is the analogue of `Can{}`, but for special *attributes*.
-`HasName` has the `__name__: str` attribute, `HasDict` has a `__dict__`, etc. -
-`optype.Does{}` describe the *type of operators*. So `DoesAbs` is the type of
-the `abs({})` builtin function, and `DoesPos` the type of the `+{}` prefix
-operator. - `optype.do_{}` are the correctly-typed implementations of `Does{}`.
-For each `do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is
-the typed alias of `abs({})`, and `do_pos: DoesPos` is a typed version of
-`operator.pos`. The `optype.do_` operators are more complete than `operators`,
-has runtime-accessible type annotations, and uses a fully predictable naming
-scheme. ## Reference All [typing protocols][PC] here live in the root `optype`
-namespace. They are [runtime-checkable][RC] so that you can do e.g. `isinstance
-('snail', optype.CanAdd)`, in case you want to check whether `snail` implements
+pip install optype ``` [OPTYPE]: https://pypi.org/project/optype/ ## Example
+Let's say you're writing a `twice(x)` function, that evaluates `2 * x`.
+Implementing it is trivial, but what about the type annotations? Because `twice
+(2) == 4`, `twice(3.14) == 6.28` and `twice('I') = 'II'`, it might seem like a
+good idea to type it as `twice[T](x: T) -> T: ...`. However, that wouldn't
+include cases such as `twice(True) == 2` or `twice((42, True)) == (42, True,
+42, True)`, where the input- and output types differ. Moreover, `twice` should
+accept *any* type with a custom `__rmul__` method that accepts `2` as argument.
+This is where `optype` comes in handy, which has single-method protocols for
+*all* the builtin special methods. For `twice`, we can use `optype.CanRMul[X,
+Y]`, which, as the name suggests, is a protocol with (only) the `def __rmul__
+(self, x: X) -> Y: ...` method. With this, the `twice` function can written as:
+```python import typing import optype type Two = typing.Literal[2] def twice[Y]
+(x: optype.CanRMul[Two, Y], /) -> Y: return 2 * x ``` But what about types that
+implement `__add__` but not `__radd__`? In this case, we could return `x * 2`
+as fallback. Because the `optype.Can*` protocols are runtime-checkable, the
+revised `twice2` function can be compactly written as: ```python def twice2[Y]
+(x: optype.CanRMul[Two, Y] | optype.CanMul[Two, Y], /) -> Y: return 2 * x if
+isinstance(x, optype.CanRMul) else x * 2 ``` See [`examples/twice.py`]
+(examples/twice.py) for the full example. ## Overview The API of `optype` is
+flat; a single `import optype` is all you need. There are four flavors of
+things that live within `optype`, - `optype.Can{}` types describe *what can be
+done* with it. For instance, any `CanAbs[T]` type can be used as argument to
+the `abs()` builtin function with return type `T`. Most `Can{}` implement a
+single special method, whose name directly matched that of the type. `CanAbs`
+implements `__abs__`, `CanAdd` implements `__add__`, etc. - `optype.Has{}` is
+the analogue of `Can{}`, but for special *attributes*. `HasName` has the
+`__name__: str` attribute, `HasDict` has a `__dict__`, etc. - `optype.Does{}`
+describe the *type of operators*. So `DoesAbs` is the type of the `abs({})`
+builtin function, and `DoesPos` the type of the `+{}` prefix operator. -
+`optype.do_{}` are the correctly-typed implementations of `Does{}`. For each
+`do_{}` there is a `Does{}`, and vice-versa. So `do_abs: DoesAbs` is the typed
+alias of `abs({})`, and `do_pos: DoesPos` is a typed version of `operator.pos`.
+The `optype.do_` operators are more complete than `operators`, has runtime-
+accessible type annotations, and uses a fully predictable naming scheme. ##
+Reference All [typing protocols][PC] here live in the root `optype` namespace.
+They are [runtime-checkable][RC] so that you can do e.g. `isinstance('snail',
+optype.CanAdd)`, in case you want to check whether `snail` implements
 `__add__`. > [!NOTE] > It is bad practice to use a [`typing.Protocol`][PC] as
 base class for your > implementation. Because of [`@typing.runtime_checkable`]
 [RC], you can use > `isinstance` either way. Unlike`collections.abc`,
 `optype`'s protocols aren't abstract base classes, i.e. they don't extend
 `abc.ABC`, only `typing.Protocol`. This allows the `optype` protocols to be
 used as building blocks for `.pyi` type stubs. [PC]: https://
 typing.readthedocs.io/en/latest/spec/protocol.html [RC]: https://
```

