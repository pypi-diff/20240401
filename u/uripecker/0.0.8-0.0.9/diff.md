# Comparing `tmp/uripecker-0.0.8.tar.gz` & `tmp/uripecker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uripecker-0.0.8.tar", last modified: Mon Nov  7 19:20:32 2022, max compression
+gzip compressed data, was "uripecker-0.0.9.tar", last modified: Tue Feb 14 13:19:15 2023, max compression
```

## Comparing `uripecker-0.0.8.tar` & `uripecker-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2022-11-07 19:20:32.986139 uripecker-0.0.8/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      549 2022-11-07 19:20:32.986139 uripecker-0.0.8/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)     1607 2022-11-07 19:20:32.750135 uripecker-0.0.8/setup.py
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2022-11-07 19:20:32.986139 uripecker-0.0.8/src/
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2022-11-07 19:20:32.986139 uripecker-0.0.8/src/uripecker/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      389 2022-11-07 17:45:39.813222 uripecker-0.0.8/src/uripecker/__init__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     3517 2022-10-08 11:43:22.048385 uripecker-0.0.8/src/uripecker/__main__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)      552 2022-11-07 19:20:32.550131 uripecker-0.0.8/src/uripecker/_meta.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     5917 2022-10-21 18:37:07.964672 uripecker-0.0.8/src/uripecker/peck.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-02-14 13:19:15.436804 uripecker-0.0.9/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      871 2023-02-14 13:19:15.436804 uripecker-0.0.9/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    12159 2023-02-14 13:19:14.992796 uripecker-0.0.9/setup.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-02-14 13:19:15.436804 uripecker-0.0.9/src/
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-02-14 13:19:15.436804 uripecker-0.0.9/src/uripecker/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      389 2022-11-07 17:45:39.813222 uripecker-0.0.9/src/uripecker/__init__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     3626 2023-02-14 13:12:19.137248 uripecker-0.0.9/src/uripecker/__main__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      552 2023-02-14 13:19:14.004778 uripecker-0.0.9/src/uripecker/_meta.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     7105 2023-02-14 13:12:19.137248 uripecker-0.0.9/src/uripecker/peck.py
```

### Comparing `uripecker-0.0.8/src/uripecker/__main__.py` & `uripecker-0.0.9/src/uripecker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 
     KEY = VALUE
 
 where any KEY must consist only of letters, numbers, and
 underscore.  VALUE must be a string -- typically a URI
 pattern -- containing a single instance of `%s`.
 
+KEYs are case-insensitive, so a map containing two KEYs
+that only differ in letter case is not a valid map.
+
 Empty lines, lines starting with `#`, and whitespace (except
 whitespace embedded within VALUE) is ignored.
 
 See also uripecker.peck() for details and examples.
 """.strip()
```

### Comparing `uripecker-0.0.8/src/uripecker/_meta.py` & `uripecker-0.0.9/src/uripecker/_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CODENAME: str = """
 
 """.strip()
 
 GIT_LASTHASH: str = """
-8331c801e13d5eb8846989a07a634b17cf396f41
+ccd50a5efad7976dc1f26ca179cbc2ad4267db59
 """.strip()
 
 GIT_LASTSUMMARY: str = """
-Bump version to 0.0.8
+Bump version to 0.0.9
 """.strip()
 
 LICENSE: str = """
 LGPLv2
 """.strip()
 
 MAINTAINER: str = """
@@ -31,9 +31,9 @@
 """.strip()
 
 VCS_BROWSER: str = """
 https://gitlab.com/vornet/python/python-uripecker
 """.strip()
 
 VERSION: str = """
-0.0.8
+0.0.9
 """.strip()
```

### Comparing `uripecker-0.0.8/src/uripecker/peck.py` & `uripecker-0.0.9/src/uripecker/peck.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,14 +102,36 @@
             r'(?:/[^\s>]*)?'
         )   # resource path
     )
     for uri in re.findall(regex, text):
         yield uri.rstrip(').>')
 
 
+class CiDict(dict):
+
+    @classmethod
+    def from_arg(cls, arg):
+        seen = {}
+        for k in arg.keys():
+            lk = k.lower()
+            if lk in seen:
+                raise ValueError(f"duplicate key: {k!r} vs. {seen[lk]!r}")
+            seen[lk] = k
+        return cls(arg)
+
+    def get(self, key, default=None):
+        """
+        Imitate dict.get() but with case-insensitive key comparison
+        """
+        for k, v in self.items():
+            if k.lower() == key.lower():
+                return v
+        return default
+
+
 def _deref(candidates, pmap):
     """
     Turn query (like "g hello" for google) to URI
     """
     for c in candidates:
         LOG.debug('_deref():c.kw=%r' % c.kw)
         LOG.debug('_deref():c.query=%r' % c.query)
@@ -188,15 +210,33 @@
          'http://gitlab.example.org/issue?id=1',
          'http://gitlab.example.org/issue?id=42',
          'http://faq.example.org/faq/14']
 
     Note that the URI pattern can be any kind of URI, such as ftp:// URI,
     (or any string, actually) but the '%s' is converted using HTTP URI
     quoting rules.
+
+    Keys in PATTERN_MAP are treated as case-insensitive, so if the *pmap*
+    argument contains two keys that only differ in case, ValueError is
+    raised.
+
+    Following example uses invalud PATTERN_MAP:
+
+        >>> BAD_PATTERN_MAP = {
+        ... 'issue': 'http://gitlab.example.org/issue?id=%s',
+        ... 'faq': 'http://faq.example.org/faq/%s',
+        ... 'FAQ': 'http://faq.other.example.org/faq/%s',
+        ... }
+        >>> found = list(peck(pmap=BAD_PATTERN_MAP, text=SOURCE_TEXT))
+        Traceback (most recent call last):
+            ...
+        ValueError: duplicate key: 'FAQ' vs. 'faq'
+
     """
+    pmap = CiDict.from_arg(pmap)
     LOG.debug('peck():pmap=%r' % pmap)
     candidates = itertools.chain(
         filter_ids(text),
         filter_exps(text),
         filter_tags(text),
         filter_kws(text),
     )
```

