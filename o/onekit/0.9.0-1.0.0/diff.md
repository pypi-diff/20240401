# Comparing `tmp/onekit-0.9.0.tar.gz` & `tmp/onekit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onekit-0.9.0.tar", max compression
+gzip compressed data, was "onekit-1.0.0.tar", max compression
```

## Comparing `onekit-0.9.0.tar` & `onekit-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     1518 2023-11-20 13:36:52.112681 onekit-0.9.0/LICENSE
--rw-r--r--   0        0        0     1624 2023-11-20 13:36:52.112681 onekit-0.9.0/README.md
--rw-r--r--   0        0        0     2128 2023-11-20 13:37:46.860516 onekit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-11-20 13:36:52.116681 onekit-0.9.0/src/onekit/__init__.py
--rw-r--r--   0        0        0    37727 2023-11-20 13:36:52.116681 onekit-0.9.0/src/onekit/pythonkit.py
--rw-r--r--   0        0        0     2955 2023-11-20 13:36:52.116681 onekit-0.9.0/src/onekit/sparkkit.py
--rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 onekit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-04-01 17:43:00.839363 onekit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1569 2024-04-01 17:43:00.839363 onekit-1.0.0/README.md
+-rw-r--r--   0        0        0     2204 2024-04-01 17:43:55.335367 onekit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/__init__.py
+-rw-r--r--   0        0        0     3965 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/mathkit.py
+-rw-r--r--   0        0        0     1643 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/numpykit.py
+-rw-r--r--   0        0        0    14598 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/optfunckit.py
+-rw-r--r--   0        0        0     6799 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/pandaskit.py
+-rw-r--r--   0        0        0    35788 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/pythonkit.py
+-rw-r--r--   0        0        0    37356 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/sparkkit.py
+-rw-r--r--   0        0        0    20081 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/vizkit.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 onekit-1.0.0/PKG-INFO
```

### Comparing `onekit-0.9.0/LICENSE` & `onekit-1.0.0/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, onekit developers.
+Copyright (c) 2023 Eugen Stripling
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `onekit-0.9.0/README.md` & `onekit-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 <a href="https://github.com/estripling/onekit/actions/workflows/test.yml"><img alt="test" src="https://github.com/estripling/onekit/actions/workflows/test.yml/badge.svg?branch=main"></a>
 <a href="https://codecov.io/gh/estripling/onekit"><img alt="coverage" src="https://codecov.io/github/estripling/onekit/coverage.svg?branch=main"></a>
 <a href="https://github.com/estripling/onekit/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/onekit"></a>
 </p>
 
 ## About
 
-One package for utility functions:
+All-in-One Python Kit:
 
 - [Examples](https://onekit.readthedocs.io/en/stable/examples.html)
 - [Documentation](https://onekit.readthedocs.io/en/stable/index.html)
 - [Developer Guide](https://onekit.readthedocs.io/en/stable/developers.html)
 - [API Reference](https://onekit.readthedocs.io/en/stable/autoapi/index.html)
 
 ## Installation
 
 `onekit` is available on [PyPI](https://pypi.org/project/onekit/) for Python 3.8+:
 
 ```console
 pip install onekit
 ```
 
-## License
+## Disclaimer
 
-`onekit` was created by onekit developers.
-It is licensed under the terms of the BSD 3-Clause license.
+⚠️ This is a personal project: Use at your own risk!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
                                 [onekit logo.]
                   _[_p_y_p_i_]_[_p_y_p_i_]_[_d_o_c_s_]_[_t_e_s_t_]_[_c_o_v_e_r_a_g_e_]_[_l_i_c_e_n_s_e_]
-## About One package for utility functions: - [Examples](https://
-onekit.readthedocs.io/en/stable/examples.html) - [Documentation](https://
-onekit.readthedocs.io/en/stable/index.html) - [Developer Guide](https://
-onekit.readthedocs.io/en/stable/developers.html) - [API Reference](https://
-onekit.readthedocs.io/en/stable/autoapi/index.html) ## Installation `onekit` is
-available on [PyPI](https://pypi.org/project/onekit/) for Python 3.8+:
-```console pip install onekit ``` ## License `onekit` was created by onekit
-developers. It is licensed under the terms of the BSD 3-Clause license.
+## About All-in-One Python Kit: - [Examples](https://onekit.readthedocs.io/en/
+stable/examples.html) - [Documentation](https://onekit.readthedocs.io/en/
+stable/index.html) - [Developer Guide](https://onekit.readthedocs.io/en/stable/
+developers.html) - [API Reference](https://onekit.readthedocs.io/en/stable/
+autoapi/index.html) ## Installation `onekit` is available on [PyPI](https://
+pypi.org/project/onekit/) for Python 3.8+: ```console pip install onekit ``` ##
+Disclaimer â ï¸ This is a personal project: Use at your own risk!
```

### Comparing `onekit-0.9.0/pyproject.toml` & `onekit-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "onekit"
-version = "0.9.0"
-description = "One package for utility functions."
-authors = ["onekit developers"]
+version = "1.0.0"
+description = "All-in-One Python Kit."
+authors = ["Eugen Stripling <estripling042@gmail.com>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/onekit"
 documentation = "https://onekit.readthedocs.io/en/stable/"
 keywords = ["onekit"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
@@ -48,14 +48,17 @@
 
 [tool.poetry.group.pandaskit.dependencies]
 pandas = ">=0.23.2"
 
 [tool.poetry.group.sparkkit.dependencies]
 pyspark = "3.1.1"
 
+[tool.poetry.group.vizkit.dependencies]
+matplotlib = ">=3.7.1"
+
 [tool.black]
 line-length = 88
 target-version = ["py38"]
 
 [tool.isort]
 py_version = "auto"
 profile = "black"
```

### Comparing `onekit-0.9.0/src/onekit/pythonkit.py` & `onekit-1.0.0/src/onekit/pythonkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from contextlib import ContextDecorator
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import (
     Any,
     Callable,
     Generator,
-    Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
@@ -31,41 +30,39 @@
 from toolz import curried
 
 __all__ = (
     "archive_files",
     "are_predicates_true",
     "check_random_state",
     "coinflip",
-    "collatz",
     "concat_strings",
     "contrast_sets",
     "create_path",
+    "date_ago",
+    "date_ahead",
+    "date_count_backward",
+    "date_count_forward",
+    "date_range",
     "date_to_str",
-    "daterange",
-    "daycount",
     "extend_range",
-    "fibonacci",
     "flatten",
     "filter_regex",
     "func_name",
     "headline",
     "highlight_string_differences",
     "humantime",
-    "isdivisible",
-    "iseven",
-    "isodd",
     "last_date_of_month",
     "lazy_read_lines",
     "map_regex",
-    "n_days",
     "num_to_str",
+    "number_of_days",
+    "op",
     "prompt_yes_no",
     "reduce_sets",
     "remove_punctuation",
-    "relative_date",
     "signif",
     "source_code",
     "stopwatch",
     "str_to_date",
     "weekday",
 )
 
@@ -133,22 +130,23 @@
 
         shutil.make_archive(name, kind, tmpdir)
 
 
 def are_predicates_true(
     func: Callable[..., bool],
     /,
-    *predicates: Iterable[Predicate],
+    *predicates: Predicate,
 ) -> Predicate:
     """Evaluate if predicates are true.
 
     A predicate is of the form :math:`P\\colon X \\rightarrow \\{False, True\\}`
 
     Examples
     --------
+    >>> import onekit.mathkit as mk
     >>> import onekit.pythonkit as pk
     >>> pk.are_predicates_true(all, lambda x: x % 2 == 0, lambda x: x % 5 == 0)(10)
     True
 
     >>> pk.are_predicates_true(all, lambda x: x % 2 == 0, lambda x: x % 5 == 0)(12)
     False
 
@@ -156,28 +154,28 @@
     True
 
     >>> pk.are_predicates_true(any, lambda x: x % 2 == 0, lambda x: x % 5 == 0)(13)
     False
 
     >>> is_x_divisible_by_3_and_5 = pk.are_predicates_true(
     ...     all,
-    ...     pk.isdivisible(n=3),
-    ...     pk.isdivisible(n=5),
+    ...     mk.isdivisible(n=3),
+    ...     mk.isdivisible(n=5),
     ... )
     >>> type(is_x_divisible_by_3_and_5)
     <class 'function'>
     >>> is_x_divisible_by_3_and_5(60)
     True
     >>> is_x_divisible_by_3_and_5(9)
     False
 
     >>> is_x_divisible_by_3_or_5 = pk.are_predicates_true(
     ...     any,
-    ...     pk.isdivisible(n=3),
-    ...     pk.isdivisible(n=5),
+    ...     mk.isdivisible(n=3),
+    ...     mk.isdivisible(n=5),
     ... )
     >>> type(is_x_divisible_by_3_or_5)
     <class 'function'>
     >>> is_x_divisible_by_3_or_5(60)
     True
     >>> is_x_divisible_by_3_or_5(9)
     True
@@ -249,80 +247,15 @@
         raise ValueError(f"{bias=} - must be a float in [0, 1]")
 
     rng = check_random_state(seed)
 
     return rng.random() < bias
 
 
-def collatz(n: int, /) -> Generator:
-    """Generate a Collatz sequence.
-
-    The famous 3n + 1 conjecture [c1]_ [c2]_. Given a positive integer :math:`n > 0`,
-    the next term in the Collatz sequence is half of :math:`n`
-    if :math:`n` is even; otherwise, if :math:`n` is odd,
-    the next term is 3 times :math:`n` plus 1.
-    Symbolically,
-
-    .. math::
-
-        f(n) =
-        \\begin{cases}
-             n / 2 & \\text{ if } n \\equiv 0 \\text{ (mod 2) } \\\\[6pt]
-            3n + 1 & \\text{ if } n \\equiv 1 \\text{ (mod 2) }
-        \\end{cases}
-
-    The Collatz conjecture is that the sequence always reaches 1
-    for any positive integer :math:`n`.
-
-    Parameters
-    ----------
-    n : int
-        A positive integer seeding the Collatz sequence.
-
-    Yields
-    ------
-    int
-        A generator of Collatz numbers that breaks when 1 is reached.
-
-    Raises
-    ------
-    ValueError
-        If ``n`` is not a positive integer.
-
-    References
-    ----------
-    .. [c1] "Collatz", The On-Line Encyclopedia of Integer Sequences®,
-            https://oeis.org/A006370
-    .. [c2] "Collatz conjecture", Wikipedia,
-            https://en.wikipedia.org/wiki/Collatz_conjecture
-
-    Examples
-    --------
-    >>> import toolz
-    >>> import onekit.pythonkit as pk
-    >>> n = 12
-    >>> list(pk.collatz(n))
-    [12, 6, 3, 10, 5, 16, 8, 4, 2, 1]
-    >>> toolz.count(pk.collatz(n))
-    10
-    """
-    if not isinstance(n, int) or n < 1:
-        raise ValueError(f"{n=} - must be a positive integer")
-
-    while True:
-        yield n
-
-        if n == 1:
-            break
-
-        # update
-        n = n // 2 if iseven(n) else 3 * n + 1
-
-
-def concat_strings(sep: str, /, *strings: Iterable[str]) -> str:
+def concat_strings(sep: str, /, *strings: str) -> str:
     """Concatenate strings.
 
     Examples
     --------
     >>> from functools import partial
     >>> import onekit.pythonkit as pk
     >>> pk.concat_strings(" ", "Hello", "World")
@@ -331,14 +264,19 @@
     'Hello World'
 
     >>> plus_concat = partial(pk.concat_strings, " + ")
     >>> plus_concat("Hello", "World")
     'Hello + World'
     >>> plus_concat(["Hello", "World"])
     'Hello + World'
+
+    >>> # map onto list of lists of strings
+    >>> ws_concat = partial(pk.concat_strings, " ")
+    >>> list(map(ws_concat, [["Hello", "World"], ["Hi", "there"]]))
+    ['Hello World', 'Hi there']
     """
     return sep.join(toolz.pipe(strings, flatten, curried.map(str)))
 
 
 def contrast_sets(x: set, y: set, /, *, n: int = 3) -> dict:
     """Contrast sets.
 
@@ -445,122 +383,196 @@
 
     output.update(tmp)
     output["report"] = "\n".join(lines)
 
     return output
 
 
-def create_path(*strings: Iterable[str]) -> str:
+def create_path(*strings: str) -> str:
     """Create path by concatenating strings.
 
     Examples
     --------
     >>> import onekit.pythonkit as pk
     >>> pk.create_path("path", "to", "file")
     'path/to/file'
 
     >>> pk.create_path(["hdfs://", "path", "to", "file"])
     'hdfs://path/to/file'
     """
     return functools.reduce(os.path.join, flatten(strings))
 
 
-def date_to_str(d: dt.date, /) -> str:
-    """Cast date to string in ISO format: YYYY-MM-DD.
+@toolz.curry
+def date_ago(d0: dt.date, /, n: int) -> dt.date:
+    """Compute date that is :math:`n \\in \\mathbb{N}_{0}` days ago.
 
     Examples
     --------
     >>> import datetime as dt
     >>> import onekit.pythonkit as pk
-    >>> pk.date_to_str(dt.date(2022, 1, 1))
-    '2022-01-01'
+    >>> d0 = dt.date(2022, 1, 1)
+
+    >>> # function is curried
+    >>> today_ds = pk.date_ago(d0)
+    >>> today_ds(n=0)
+    datetime.date(2022, 1, 1)
+    >>> today_ds(1)
+    datetime.date(2021, 12, 31)
+    >>> today_ds(2)
+    datetime.date(2021, 12, 30)
+
+    >>> lag3 = pk.date_ago(n=3)
+    >>> lag3(dt.date(2024, 1, 1))
+    datetime.date(2023, 12, 29)
+    """
+    if not isinstance(n, int) or n < 0:
+        raise ValueError(f"{n=} - must be a non-negative integer")
+    return d0 - dt.timedelta(days=n)
+
+
+@toolz.curry
+def date_ahead(d0: dt.date, /, n: int) -> dt.date:
+    """Compute date that is :math:`n \\in \\mathbb{N}_{0}` days ahead.
+
+    Examples
+    --------
+    >>> import datetime as dt
+    >>> import onekit.pythonkit as pk
+    >>> d0 = dt.date(2022, 1, 1)
+
+    >>> # function is curried
+    >>> today_ds = pk.date_ahead(d0)
+    >>> today_ds(n=0)
+    datetime.date(2022, 1, 1)
+    >>> today_ds(1)
+    datetime.date(2022, 1, 2)
+    >>> today_ds(2)
+    datetime.date(2022, 1, 3)
+
+    >>> lead3 = pk.date_ahead(n=3)
+    >>> lead3(dt.date(2024, 1, 1))
+    datetime.date(2024, 1, 4)
     """
-    return d.isoformat()
+    if not isinstance(n, int) or n < 0:
+        raise ValueError(f"{n=} - must be a non-negative integer")
+    return d0 + dt.timedelta(days=n)
+
+
+def date_count_backward(d0: dt.date, /) -> Generator:
+    """Generate sequence of consecutive dates in backward manner w.r.t. :math:`d_{0}`.
+
+    Examples
+    --------
+    >>> import datetime as dt
+    >>> from toolz import curried
+    >>> import onekit.pythonkit as pk
+    >>> d0 = dt.date(2022, 1, 1)
+    >>> curried.pipe(
+    ...     pk.date_count_backward(d0),
+    ...     curried.map(pk.date_to_str),
+    ...     curried.take(3),
+    ...     list,
+    ... )
+    ['2022-01-01', '2021-12-31', '2021-12-30']
+    """
+    successor = operator.sub
+    return toolz.iterate(lambda d: successor(d, dt.timedelta(1)), d0)
 
 
-def daterange(
-    start: dt.date,
-    end: dt.date,
+def date_count_forward(d0: dt.date, /) -> Generator:
+    """Generate sequence of consecutive dates in forward manner w.r.t. :math:`d_{0}`.
+
+    Examples
+    --------
+    >>> import datetime as dt
+    >>> from toolz import curried
+    >>> import onekit.pythonkit as pk
+    >>> d0 = dt.date(2022, 1, 1)
+    >>> curried.pipe(
+    ...     pk.date_count_forward(d0),
+    ...     curried.map(pk.date_to_str),
+    ...     curried.take(3),
+    ...     list,
+    ... )
+    ['2022-01-01', '2022-01-02', '2022-01-03']
+    """
+    successor = operator.add
+    return toolz.iterate(lambda d: successor(d, dt.timedelta(1)), d0)
+
+
+def date_range(
+    min_date: dt.date,
+    max_date: dt.date,
     /,
     *,
-    incl_start: bool = True,
-    incl_end: bool = True,
+    incl_min: bool = True,
+    incl_max: bool = True,
 ) -> Generator:
     """Generate sequence of consecutive dates between two dates.
 
     Examples
     --------
     >>> import datetime as dt
     >>> from toolz import curried
     >>> import onekit.pythonkit as pk
     >>> d1 = dt.date(2022, 1, 1)
     >>> d2 = dt.date(2022, 1, 3)
 
-    >>> curried.pipe(pk.daterange(d1, d2), curried.map(pk.date_to_str), list)
+    >>> curried.pipe(pk.date_range(d1, d2), curried.map(pk.date_to_str), list)
     ['2022-01-01', '2022-01-02', '2022-01-03']
 
     >>> curried.pipe(
-    ...     pk.daterange(d1, d2, incl_start=False, incl_end=True),
+    ...     pk.date_range(d1, d2, incl_min=False, incl_max=True),
     ...     curried.map(pk.date_to_str),
     ...     list,
     ... )
     ['2022-01-02', '2022-01-03']
 
     >>> curried.pipe(
-    ...     pk.daterange(d1, d2, incl_start=True, incl_end=False),
+    ...     pk.date_range(d1, d2, incl_min=True, incl_max=False),
     ...     curried.map(pk.date_to_str),
     ...     list,
     ... )
     ['2022-01-01', '2022-01-02']
 
     >>> curried.pipe(
-    ...     pk.daterange(d1, d2, incl_start=False, incl_end=False),
+    ...     pk.date_range(d1, d2, incl_min=False, incl_max=False),
     ...     curried.map(pk.date_to_str),
     ...     list,
     ... )
     ['2022-01-02']
 
-    >>> list(pk.daterange(d1, dt.date(2022, 1, 1)))
+    >>> list(pk.date_range(d1, dt.date(2022, 1, 1)))
     [datetime.date(2022, 1, 1)]
 
-    >>> list(pk.daterange(d1, dt.date(2022, 1, 1), incl_start=False))
+    >>> list(pk.date_range(d1, dt.date(2022, 1, 1), incl_min=False))
     []
 
     >>> # function makes sure: start <= end
-    >>> curried.pipe(pk.daterange(d2, d1), curried.map(pk.date_to_str), list)
+    >>> curried.pipe(pk.date_range(d2, d1), curried.map(pk.date_to_str), list)
     ['2022-01-01', '2022-01-02', '2022-01-03']
     """
-    start, end = sorted([start, end])
-    start = start if incl_start else start + dt.timedelta(1)
-    end = end if incl_end else end - dt.timedelta(1)
-    return itertools.takewhile(lambda d: d <= end, daycount(start, forward=True))
+    d1, d2 = sorted([min_date, max_date])
+    d1 = d1 if incl_min else d1 + dt.timedelta(1)
+    d2 = d2 if incl_max else d2 - dt.timedelta(1)
+    return itertools.takewhile(lambda d: d <= d2, date_count_forward(d1))
 
 
-def daycount(start: dt.date, /, *, forward: bool = True) -> Generator:
-    """Generate sequence of consecutive dates.
+def date_to_str(d: dt.date, /) -> str:
+    """Cast date to string in ISO format: YYYY-MM-DD.
 
     Examples
     --------
     >>> import datetime as dt
-    >>> from toolz import curried
     >>> import onekit.pythonkit as pk
-    >>> start = dt.date(2022, 1, 1)
-    >>> curried.pipe(pk.daycount(start), curried.take(3), list)
-    [datetime.date(2022, 1, 1), datetime.date(2022, 1, 2), datetime.date(2022, 1, 3)]
-
-    >>> curried.pipe(
-    ...     pk.daycount(start, forward=False),
-    ...     curried.map(pk.date_to_str),
-    ...     curried.take(3),
-    ...     list,
-    ... )
-    ['2022-01-01', '2021-12-31', '2021-12-30']
+    >>> pk.date_to_str(dt.date(2022, 1, 1))
+    '2022-01-01'
     """
-    successor = operator.add if forward else operator.sub
-    return toolz.iterate(lambda d: successor(d, dt.timedelta(1)), start)
+    return d.isoformat()
 
 
 def extend_range(xmin: float, xmax: float, /, *, factor: float = 0.05) -> Pair:
     """Extend value range ``xmax - xmin`` by factor.
 
     Examples
     --------
@@ -579,64 +591,15 @@
 
     new_xmin = xmin - factor * value_range
     new_xmax = xmax + factor * value_range
 
     return new_xmin, new_xmax
 
 
-def fibonacci() -> Generator:
-    """Generate the Fibonacci sequence.
-
-    For :math:`n > 1`, Fibonacci numbers may be defined by [f1]_ [f2]_:
-
-    .. math::
-
-        F(n) = F(n-1) + F(n-2) \\text{ with } F(0) = 0 \\text{ and } F(1) = 1.
-
-    As such, the sequence starts as follows:
-
-    .. math::
-
-        0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, \\dots
-
-    Yields
-    ------
-    int
-        A generator of consecutive Fibonacci numbers.
-
-    References
-    ----------
-    .. [f1] "Fibonacci numbers", The On-Line Encyclopedia of Integer Sequences®,
-            https://oeis.org/A000045
-    .. [f2] "Fibonacci number", Wikipedia,
-            https://en.wikipedia.org/wiki/Fibonacci_number
-
-    Examples
-    --------
-    >>> import toolz
-    >>> import onekit.pythonkit as pk
-    >>> list(toolz.take(13, pk.fibonacci()))
-    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144]
-    """
-    lag2, lag1 = 0, 1
-    yield lag2
-    yield lag1
-
-    while True:
-        lag0 = lag2 + lag1
-        yield lag0
-        lag2, lag1 = lag1, lag0
-
-
-def filter_regex(
-    pattern: str,
-    /,
-    *strings: Iterable[str],
-    flags=re.IGNORECASE,
-) -> Generator:
+def filter_regex(pattern: str, /, *strings: str, flags=re.IGNORECASE) -> Generator:
     """Filter iterable of strings with regex.
 
     Examples
     --------
     >>> from functools import partial
     >>> import onekit.pythonkit as pk
     >>> list(pk.filter_regex("hello", "Hello, World!", "Hi, there!", "Hello!"))
@@ -654,15 +617,15 @@
     >>> filter_regex__hi = partial(pk.filter_regex, "hi")
     >>> list(filter_regex__hi("Hello, World!", "Hi, there!", "Hello!"))
     ['Hi, there!']
     """
     return filter(functools.partial(re.findall, pattern, flags=flags), flatten(strings))
 
 
-def flatten(*items: Iterable[Any]) -> Generator:
+def flatten(*items: Any) -> Generator:
     """Flatten iterable of items.
 
     Examples
     --------
     >>> import onekit.pythonkit as pk
     >>> list(pk.flatten([[1, 2], *[3, 4], [5]]))
     [1, 2, 3, 4, 5]
@@ -795,75 +758,14 @@
 
     if seconds:
         output.append(f"{seconds}s")
 
     return " ".join(output)
 
 
-@toolz.curry
-def isdivisible(x: Union[int, float], /, n: int) -> bool:
-    """Evaluate if :math:`x` is evenly divisible by :math:`n`.
-
-    Examples
-    --------
-    >>> import onekit.pythonkit as pk
-    >>> pk.isdivisible(49, 7)
-    True
-
-    >>> # function is curried
-    >>> pk.isdivisible(10)(5)
-    True
-    >>> is_10_divisible_by = pk.isdivisible(10)
-    >>> is_10_divisible_by(5)
-    True
-    >>> is_x_divisible_by_5 = pk.isdivisible(n=5)
-    >>> is_x_divisible_by_5(10)
-    True
-    >>> is_x_divisible_by_5(11.0)
-    False
-    """
-    return x % n == 0
-
-
-def iseven(x: Union[int, float], /) -> bool:
-    """Evaluate if :math:`x` is even.
-
-    Examples
-    --------
-    >>> import onekit.pythonkit as pk
-    >>> pk.iseven(0)
-    True
-
-    >>> pk.iseven(1)
-    False
-
-    >>> pk.iseven(2)
-    True
-    """
-    return isdivisible(x, n=2)
-
-
-def isodd(x: Union[int, float], /) -> bool:
-    """Evaluate if :math:`x` is odd.
-
-    Examples
-    --------
-    >>> import onekit.pythonkit as pk
-    >>> pk.isodd(0)
-    False
-
-    >>> pk.isodd(1)
-    True
-
-    >>> pk.isodd(2)
-    False
-    """
-    return toolz.complement(iseven)(x)
-
-
 def last_date_of_month(year: int, month: int, /) -> dt.date:
     """Get the last date of the month.
 
     Examples
     --------
     >>> import onekit.pythonkit as pk
     >>> pk.last_date_of_month(2022, 1)
@@ -903,20 +805,15 @@
         errors=errors,
         newline=newline,
     ) as lines:
         for line in lines:
             yield line
 
 
-def map_regex(
-    pattern: str,
-    /,
-    *strings: Iterable[str],
-    flags=re.IGNORECASE,
-) -> Generator:
+def map_regex(pattern: str, /, *strings: str, flags=re.IGNORECASE) -> Generator:
     """Match regex to iterable of strings.
 
     Examples
     --------
     >>> from functools import partial
     >>> import onekit.pythonkit as pk
     >>> list(pk.map_regex("hello", "Hello, World!", "Hi, there!", "Hello!"))
@@ -934,48 +831,76 @@
     >>> map_regex__hi = partial(pk.map_regex, "hi")
     >>> list(map_regex__hi("Hello, World!", "Hi, there!", "Hello!"))
     [[], ['Hi'], []]
     """
     return map(functools.partial(re.findall, pattern, flags=flags), flatten(strings))
 
 
-def n_days(d1: dt.date, d2: dt.date, /) -> int:
-    """Compute number of days between two dates.
+def num_to_str(x: Union[int, float], /) -> str:
+    """Cast number to string with underscores as thousands separator.
+
+    Examples
+    --------
+    >>> import onekit.pythonkit as pk
+    >>> pk.num_to_str(1000000)
+    '1_000_000'
+
+    >>> pk.num_to_str(100000.0)
+    '100_000.0'
+    """
+    return f"{x:_}"
+
+
+def number_of_days(d1: dt.date, d2: dt.date, /) -> int:
+    """Compute the number of days between two dates (both inclusive).
 
     Examples
     --------
     >>> import datetime as dt
     >>> import onekit.pythonkit as pk
-    >>> pk.n_days(dt.date(2022, 8, 1), dt.date(2022, 8, 1))
+    >>> pk.number_of_days(dt.date(2022, 8, 1), dt.date(2022, 8, 1))
     1
 
-    >>> pk.n_days(dt.date(2022, 8, 1), dt.date(2022, 8, 7))
+    >>> pk.number_of_days(dt.date(2022, 8, 1), dt.date(2022, 8, 2))
+    2
+
+    >>> pk.number_of_days(dt.date(2022, 8, 1), dt.date(2022, 8, 7))
     7
 
     >>> # function makes sure: start <= end
-    >>> pk.n_days(dt.date(2022, 8, 7), dt.date(2022, 8, 1))
+    >>> pk.number_of_days(dt.date(2022, 8, 7), dt.date(2022, 8, 1))
     7
     """
     start, end = sorted([d1, d2])
     return (end - start).days + 1
 
 
-def num_to_str(x: Union[int, float], /) -> str:
-    """Cast number to string with underscores as thousands separator.
+@toolz.curry
+def op(func: Callable, a: Any, x: Any, /) -> Any:
+    """Leverage operator functions.
+
+    Use ``op`` to create functions of ``x`` with fixed ``a``.
 
     Examples
     --------
+    >>> import operator
     >>> import onekit.pythonkit as pk
-    >>> pk.num_to_str(1000000)
-    '1_000_000'
+    >>> pk.op(operator.add, 1, 1)
+    2
 
-    >>> pk.num_to_str(100000.0)
-    '100_000.0'
+    >>> # function is curried
+    >>> inc = pk.op(operator.add, 1)
+    >>> inc(1)
+    2
+
+    >>> dec = pk.op(operator.sub, 1)
+    >>> dec(1)
+    0
     """
-    return f"{x:_}"
+    return func(x, a)
 
 
 def prompt_yes_no(question: str, /, *, default: Optional[str] = None) -> bool:
     """Prompt yes-no question.
 
     Examples
     --------
@@ -1020,15 +945,15 @@
                 "Y" if default == "yes" else "y",
                 "N" if default == "no" else "n",
             )
             answer = input(response_text).lower()
 
 
 @toolz.curry
-def reduce_sets(func: Callable[[set, set], set], /, *sets: Iterable[set]) -> set:
+def reduce_sets(func: Callable[[set, set], set], /, *sets: set) -> set:
     """Apply function of two set arguments to reduce iterable of sets.
 
     Examples
     --------
     >>> import onekit.pythonkit as pk
     >>> x = {0, 1, 2, 3}
     >>> y = {2, 4, 6}
@@ -1062,44 +987,14 @@
     >>> pk.remove_punctuation("I think, therefore I am. --Descartes")
     'I think therefore I am Descartes'
     """
     return text.translate(str.maketrans("", "", string.punctuation))
 
 
 @toolz.curry
-def relative_date(d0: dt.date, /, n: int) -> dt.date:
-    """Compute date :math:`n \\in \\mathbb{Z}` days from reference date :math:`d_{0}`.
-
-    Examples
-    --------
-    >>> import datetime as dt
-    >>> import onekit.pythonkit as pk
-    >>> d0 = dt.date(2022, 1, 1)
-
-    >>> # function is curried
-    >>> today_ds = pk.relative_date(d0)
-    >>> today_ds(n=0)
-    datetime.date(2022, 1, 1)
-    >>> today_ds(1)
-    datetime.date(2022, 1, 2)
-    >>> today_ds(2)
-    datetime.date(2022, 1, 3)
-
-    >>> lead3 = pk.relative_date(n=3)
-    >>> lead3(d0)
-    datetime.date(2022, 1, 4)
-
-    >>> lag3 = pk.relative_date(n=-4)
-    >>> lag3(d0)
-    datetime.date(2021, 12, 28)
-    """
-    return d0 + dt.timedelta(days=n)
-
-
-@toolz.curry
 def signif(x: Union[int, float], /, n: int) -> Union[int, float]:
     """Round :math:`x` to its :math:`n` significant digits.
 
     Examples
     --------
     >>> import onekit.pythonkit as pk
     >>> pk.signif(987654321, 3)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `onekit-0.9.0/PKG-INFO` & `onekit-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: onekit
-Version: 0.9.0
-Summary: One package for utility functions.
+Version: 1.0.0
+Summary: All-in-One Python Kit.
 Home-page: https://github.com/estripling/onekit
 License: BSD 3-Clause
 Keywords: onekit
-Author: onekit developers
+Author: Eugen Stripling
+Author-email: estripling042@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,27 +32,26 @@
 <a href="https://github.com/estripling/onekit/actions/workflows/test.yml"><img alt="test" src="https://github.com/estripling/onekit/actions/workflows/test.yml/badge.svg?branch=main"></a>
 <a href="https://codecov.io/gh/estripling/onekit"><img alt="coverage" src="https://codecov.io/github/estripling/onekit/coverage.svg?branch=main"></a>
 <a href="https://github.com/estripling/onekit/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/onekit"></a>
 </p>
 
 ## About
 
-One package for utility functions:
+All-in-One Python Kit:
 
 - [Examples](https://onekit.readthedocs.io/en/stable/examples.html)
 - [Documentation](https://onekit.readthedocs.io/en/stable/index.html)
 - [Developer Guide](https://onekit.readthedocs.io/en/stable/developers.html)
 - [API Reference](https://onekit.readthedocs.io/en/stable/autoapi/index.html)
 
 ## Installation
 
 `onekit` is available on [PyPI](https://pypi.org/project/onekit/) for Python 3.8+:
 
 ```console
 pip install onekit
 ```
 
-## License
+## Disclaimer
 
-`onekit` was created by onekit developers.
-It is licensed under the terms of the BSD 3-Clause license.
+⚠️ This is a personal project: Use at your own risk!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: onekit Version: 0.9.0 Summary: One package for
-utility functions. Home-page: https://github.com/estripling/onekit License: BSD
-3-Clause Keywords: onekit Author: onekit developers Requires-Python:
->=3.8.1,<4.0 Classifier: License :: Other/Proprietary License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8 Requires-Dist: toolz
+Metadata-Version: 2.1 Name: onekit Version: 1.0.0 Summary: All-in-One Python
+Kit. Home-page: https://github.com/estripling/onekit License: BSD 3-Clause
+Keywords: onekit Author: Eugen Stripling Author-email: estripling042@gmail.com
+Requires-Python: >=3.8.1,<4.0 Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Programming Language :: Python :: 3.8 Requires-Dist: toolz
 (>=0.12.0,<0.13.0) Project-URL: Documentation, https://onekit.readthedocs.io/
 en/stable/ Project-URL: Repository, https://github.com/estripling/onekit
 Description-Content-Type: text/markdown
                                 [onekit logo.]
                   _[_p_y_p_i_]_[_p_y_p_i_]_[_d_o_c_s_]_[_t_e_s_t_]_[_c_o_v_e_r_a_g_e_]_[_l_i_c_e_n_s_e_]
-## About One package for utility functions: - [Examples](https://
-onekit.readthedocs.io/en/stable/examples.html) - [Documentation](https://
-onekit.readthedocs.io/en/stable/index.html) - [Developer Guide](https://
-onekit.readthedocs.io/en/stable/developers.html) - [API Reference](https://
-onekit.readthedocs.io/en/stable/autoapi/index.html) ## Installation `onekit` is
-available on [PyPI](https://pypi.org/project/onekit/) for Python 3.8+:
-```console pip install onekit ``` ## License `onekit` was created by onekit
-developers. It is licensed under the terms of the BSD 3-Clause license.
+## About All-in-One Python Kit: - [Examples](https://onekit.readthedocs.io/en/
+stable/examples.html) - [Documentation](https://onekit.readthedocs.io/en/
+stable/index.html) - [Developer Guide](https://onekit.readthedocs.io/en/stable/
+developers.html) - [API Reference](https://onekit.readthedocs.io/en/stable/
+autoapi/index.html) ## Installation `onekit` is available on [PyPI](https://
+pypi.org/project/onekit/) for Python 3.8+: ```console pip install onekit ``` ##
+Disclaimer â ï¸ This is a personal project: Use at your own risk!
```

