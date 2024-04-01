# Comparing `tmp/fast_html-1.0.7.tar.gz` & `tmp/fast_html-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_html-1.0.7.tar", max compression
+gzip compressed data, was "fast_html-1.0.8.tar", max compression
```

## Comparing `fast_html-1.0.7.tar` & `fast_html-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7636 2023-05-08 16:52:22.164958 fast_html-1.0.7/LICENSE
--rw-r--r--   0        0        0     3705 2024-01-24 14:29:44.462688 fast_html-1.0.7/README.rst
--rw-r--r--   0        0        0    13337 2024-01-24 14:38:31.199092 fast_html-1.0.7/fast_html/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 20:10:19.913231 fast_html-1.0.7/fast_html/py.typed
--rw-r--r--   0        0        0     2577 2024-01-24 14:05:55.939255 fast_html-1.0.7/fast_html/utils.py
--rw-r--r--   0        0        0      609 2024-01-24 14:30:05.958376 fast_html-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4633 1970-01-01 00:00:00.000000 fast_html-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     7636 2023-05-08 16:52:22.164958 fast_html-1.0.8/LICENSE
+-rw-r--r--   0        0        0     4516 2024-04-01 15:35:40.352251 fast_html-1.0.8/README.md
+-rw-r--r--   0        0        0    13549 2024-04-01 15:35:30.688085 fast_html-1.0.8/fast_html/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-01 20:10:19.913231 fast_html-1.0.8/fast_html/py.typed
+-rw-r--r--   0        0        0     2577 2024-01-24 14:05:55.939255 fast_html-1.0.8/fast_html/utils.py
+-rw-r--r--   0        0        0      608 2024-04-01 15:39:06.427501 fast_html-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 fast_html-1.0.8/PKG-INFO
```

### Comparing `fast_html-1.0.7/LICENSE` & `fast_html-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.7/fast_html/__init__.py` & `fast_html-1.0.8/fast_html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 __version__ = '1.0.7'
 
 import re
+from html import escape as escape_html
 from typing import Iterator, Union, Optional, Iterable, Any
 
 from .utils import html_to_code
 
 Tag = Iterator[str]
 Inner = Union[Tag, Iterator['Inner'], Any]
 
 _tab = '  '
 _cr = '\n'
 
 indent: bool = False
+escape: bool = False
 
 
 def indent_it(value: bool):
     global indent
     indent = value
 
 
+def escape_it(value: bool):
+    global escape
+    escape = value
+
+
 def render(gen: Tag) -> str:
     return ''.join(render(t) for t in gen) if isinstance(gen, list) else ''.join(gen)
 
 
 def solo_tag(tag_name: str, **kwargs) -> Tag:
     """returns a tag without innerHTML, e.g. `<br id="1">`
 
@@ -74,14 +81,16 @@
     if 'i' in kwargs:
         inner = kwargs['i']
         del kwargs['i']
 
     yield from solo_tag(tag_name, **kwargs)
 
     if inner is not None:
+        if escape and isinstance(inner, str):
+            inner = escape_html(inner)
         yield from _inner(inner, with_cr = True)
 
     yield f"</{tag_name}>{_cr if indent else ''}"
 
 
 # in alphabetic order
```

### Comparing `fast_html-1.0.7/fast_html/utils.py` & `fast_html-1.0.8/fast_html/utils.py`

 * *Files identical despite different names*

### Comparing `fast_html-1.0.7/pyproject.toml` & `fast_html-1.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "fast_html"
-version = "1.0.7"
+version = "1.0.8"
 description = "A fast, minimalist HTML generator"
 authors = ["Pierre <pierre.carbonnelle@gmail.com>"]
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/pcarbonn/fast_html"
 license = "LGPL-3.0-or-later"
 keywords = ["HTML", "HTMX"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Internet :: WWW/HTTP"
```

### Comparing `fast_html-1.0.7/PKG-INFO` & `fast_html-1.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-html
-Version: 1.0.7
+Version: 1.0.8
 Summary: A fast, minimalist HTML generator
 Home-page: https://github.com/pcarbonn/fast_html
 License: LGPL-3.0-or-later
 Keywords: HTML,HTMX
 Author: Pierre
 Author-email: pierre.carbonnelle@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,136 +15,160 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Project-URL: Repository, https://github.com/pcarbonn/fast_html
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
 **fast_html** is a fast, minimalist HTML generator.
 
 
 It is an alternative to templating engines, like Jinja,
-for use with, e.g., `htmx <https://htmx.org/>`__.
+for use with, e.g., [htmx](https://htmx.org/).
 
 **Pros:**
 
 - use familiar python syntax
 
 - use efficient concatenation techniques
 
 - optional automatic indentation
 
-Unlike other HTML generators (e.g. `Dominate <https://pypi.org/project/dominate/>`__) that use python objects to represent HTML snippets,
-fast_html represents HTML snippets using string `generators <https://docs.python.org/3/glossary.html#term-generator>`__
-that can be rendered extremely fast using ``join``.
-(see `here <https://python.plainenglish.io/concatenating-strings-efficiently-in-python-9bfc8e8d6f6e>`__)
+Unlike other HTML generators (e.g. [Dominate](https://pypi.org/project/dominate/)) that use python objects to represent HTML snippets,
+fast_html represents HTML snippets using string [generators](https://docs.python.org/3/glossary.html#term-generator)
+that can be rendered extremely fast using `join`.
+(see [here](https://python.plainenglish.io/concatenating-strings-efficiently-in-python-9bfc8e8d6f6e))
 
 **Like other HTML generators, one needs to remember:**
 
-- the name of some tags and attributes is changed (e.g., ``class_`` instead of ``class``, due to Python parser)
+- the name of some tags and attributes is changed (e.g., `class_` instead of `class`, due to Python parser)
 
 - there may be conflicts of function names with your code base
 
 
 Installation
 ============
-``pip install fast_html`` or copy the (single) source file in your project.
+`pip install fast_html` or copy the (single) source file in your project.
 
 Don't forget to `add a star on GitHub <https://github.com/pcarbonn/fast_html>`_ ! Thanks.
 
 
 Tutorial:
 =========
 
->>> from fast_html import *
+    >>> from fast_html import *
 
 A tag is created by calling a function of the corresponding name,
-and rendered using ``render``:
-
->>> print(render(p("text")))
-<p>text</p>
+and rendered using `render`:
 
+    >>> print(render(p("text")))
+    <p>text</p>
 
 Tag attributes are specified using named arguments:
 
->>> print(render(br(id=1)))
-<br id="1">
+    >>> print(render(br(id=1)))
+    <br id="1">
 
->>> print(render(br(id=None)))
-<br>
+    >>> print(render(br(id=None)))
+    <br>
 
->>> print(render(ul(li("text", selected=True))))
-<ul><li selected>text</li></ul>
+    >>> print(render(ul(li("text", selected=True))))
+    <ul><li selected>text</li></ul>
 
->>> print(render(ul(li("text", selected=False))))
-<ul><li>text</li></ul>
+    >>> print(render(ul(li("text", selected=False))))
+    <ul><li>text</li></ul>
 
 The python parser introduces some constraints:
 
-- The following tags require a trailing underscore: ``del_``, ``input_``, ``map_``, ``object_``.
+- The following tags require a trailing underscore: `del_`, `input_`, `map_`, `object_`.
 
-- The following tag attributes require a trailing underscore: ``class_``, ``for_``.
+- The following tag attributes require a trailing underscore: `class_`, `for_`.
 
 In fact, the trailing underscore in attribute names is always removed by fast_html,
-and other underscores are replaced by ``-``.
-For example, the htmx attribute ``hx-get`` is set using ``hx_get="url"``.
-
->>> print(render(object_("text", class_="s12", hx_get="url")))
-<object class="s12" hx-get="url">text</object>
+and other underscores are replaced by `-`.
+For example, the htmx attribute `hx-get` is set using `hx_get="url"`.
 
->>> print(render(button("Click me", hx_post="/clicked", hx_swap="outerHTML")))
-<button hx-post="/clicked" hx-swap="outerHTML">Click me</button>
+    >>> print(render(object_("text", class_="s12", hx_get="url")))
+    <object class="s12" hx-get="url">text</object>
 
+    >>> print(render(button("Click me", hx_post="/clicked", hx_swap="outerHTML")))
+    <button hx-post="/clicked" hx-swap="outerHTML">Click me</button>
 
 The innerHTML can be a list:
 
->>> print(render(div(["text", span("item 1"), span("item 2")])))
-<div>text<span>item 1</span><span>item 2</span></div>
+    >>> print(render(div(["text", span("item 1"), span("item 2")])))
+    <div>text<span>item 1</span><span>item 2</span></div>
 
 The innerHTML can also be a list of lists:
 
->>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))
-<div>text<span>item 1</span><span>item 2</span></div>
+    >>> print(render(div(["text", [span(f"item {i}") for i in [1,2]]])))
+    <div>text<span>item 1</span><span>item 2</span></div>
 
->>> print(render([br(), br()]))
-<br><br>
+    >>> print(render([br(), br()]))
+    <br><br>
 
-The innerHTML can also be specified using the ``i`` parameter,
+The innerHTML can also be specified using the `i` parameter,
 after the other attributes, to match the order of rendering:
 
->>> print(render(ul(class_="s12", i=[
-...                 li("item 1"),
-...                 li("item 2")]
-...      )))
-<ul class="s12"><li>item 1</li><li>item 2</li></ul>
-
-You can create your own tag using the ``tag`` function:
-
->>> def my_tag(inner=None, **kwargs):
-...     yield from tag("my_tag", inner, **kwargs)
->>> print(render(my_tag("text")))
-<my_tag>text</my_tag>
-
-
-When debugging your code, you can set global variable ``indent`` to ``True``
-(or call ``indent_it(True)``) to obtain HTML with tag indentation, e.g.,
-
->>> indent_it(True); print(render(div(class_="s12", i=["text\n", span("item 1"), span("item 2")])))
-<div class="s12">
-  text
-  <span>
-    item 1
-  </span>
-  <span>
-    item 2
-  </span>
-</div>
-<BLANKLINE>
+    >>> print(render(ul(class_="s12", i=[
+    ...                 li("item 1"),
+    ...                 li("item 2")]
+    ...      )))
+    <ul class="s12"><li>item 1</li><li>item 2</li></ul>
+
+You can create your own tag using the `tag` function:
+
+    >>> def my_tag(inner=None, **kwargs):
+    ...     yield from tag("my_tag", inner, **kwargs)
+    >>> print(render(my_tag("text")))
+    <my_tag>text</my_tag>
+
+
+Options:
+========
+
+By default, the inner string of a tag is not escaped:
+characters `&`, `<` and `>` in it are not converted to HTML-safe sequences.
+
+
+    >>> print(render(p("<bold>text</bold>")))
+    <p><bold>text</bold></p>
+
+Of course, you can escape strings before calling fast_html:
+
+
+    >>> from html import escape
+    >>> print(render(p(escape("<bold>text</bold>"))))
+    <p>&lt;bold&gt;text&lt;/bold&gt;</p>
+
+If your policy is to escape every inner string,
+you can activate escaping by setting the variable `escape` to `False`
+(or by calling `escape_it(False)`).
+
+    >>> escape_it(True)
+    >>> print(render(p("<bold>text</bold>")))
+    <p>&lt;bold&gt;text&lt;/bold&gt;</p>
+
+When debugging your code, you can set global variable `indent` to `True`
+(or call `indent_it(True)`) to obtain HTML with tag indentation, e.g.,
+
+    >>> indent_it(True)
+    >>> print(render(div(class_="s12", i=["text\n", span("item 1"), span("item 2")])))
+    <div class="s12">
+      text
+      <span>
+        item 1
+      </span>
+      <span>
+        item 2
+      </span>
+    </div>
+    <BLANKLINE>
 
 You can also convert an HTML string to a function-based code representation:
 
->>> print(html_to_code('<div class="example"><p>Some text</p></div>'))
-[div([p(['Some text'], )], class_="example")]
+    >>> print(html_to_code('<div class="example"><p>Some text</p></div>'))
+    [div([p(['Some text'], )], class_="example")]
```

