# Comparing `tmp/tj_text-0.8.0.tar.gz` & `tmp/tj_text-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tj_text-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tj_text-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tj_text-0.8.0.tar` & `tj_text-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      219 2023-07-17 14:49:50.219051 tj_text-0.8.0/.flake8
--rw-r--r--   0        0        0      102 2023-07-17 14:49:50.219296 tj_text-0.8.0/.gitignore
--rw-r--r--   0        0        0      131 2023-07-17 14:49:50.219542 tj_text-0.8.0/.gitlab-ci-compliance.yml
--rw-r--r--   0        0        0      523 2023-07-17 14:49:50.219749 tj_text-0.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      277 2023-07-17 14:49:50.219948 tj_text-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      175 2023-07-17 14:49:50.220152 tj_text-0.8.0/Makefile
--rw-r--r--   0        0        0     1113 2023-07-17 14:49:50.220361 tj_text-0.8.0/README.md
--rw-r--r--   0        0        0      119 2023-07-17 14:49:50.220562 tj_text-0.8.0/pip.conf
--rw-r--r--   0        0        0      110 2023-07-17 14:49:50.220815 tj_text-0.8.0/policy.yml
--rw-r--r--   0        0        0     1372 2023-07-17 14:49:50.221045 tj_text-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 14:49:50.221281 tj_text-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 14:49:50.221534 tj_text-0.8.0/tests/test_tj_text/__init__.py
--rw-r--r--   0        0        0     7110 2023-07-17 14:49:50.221785 tj_text-0.8.0/tests/test_tj_text/test_expressions.py
--rw-r--r--   0        0        0        0 2023-07-17 14:49:50.222014 tj_text-0.8.0/tj_text/__init__.py
--rw-r--r--   0        0        0      466 2023-07-17 14:49:50.222334 tj_text-0.8.0/tj_text/typograph/__init__.py
--rw-r--r--   0        0        0      834 2023-07-17 14:49:50.222577 tj_text-0.8.0/tj_text/typograph/chars.py
--rw-r--r--   0        0        0      996 2023-07-17 14:49:50.222798 tj_text-0.8.0/tj_text/typograph/constants.py
--rw-r--r--   0        0        0      991 2023-07-17 14:49:50.223005 tj_text-0.8.0/tj_text/typograph/core.py
--rw-r--r--   0        0        0    17878 2023-07-17 14:49:50.223306 tj_text-0.8.0/tj_text/typograph/mixins.py
--rw-r--r--   0        0        0     8811 2023-07-17 14:49:50.223607 tj_text-0.8.0/tj_text/typograph/processors.py
--rw-r--r--   0        0        0     3647 2023-07-17 14:49:50.223855 tj_text-0.8.0/tj_text/typograph/utils.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 tj_text-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      219 2023-07-17 14:49:50.219051 tj_text-0.8.1/.flake8
+-rw-r--r--   0        0        0      102 2023-07-17 14:49:50.219296 tj_text-0.8.1/.gitignore
+-rw-r--r--   0        0        0      131 2023-07-17 14:49:50.219542 tj_text-0.8.1/.gitlab-ci-compliance.yml
+-rw-r--r--   0        0        0      523 2023-07-17 14:49:50.219749 tj_text-0.8.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      372 2024-04-01 12:14:59.968771 tj_text-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0      175 2023-07-17 14:49:50.220152 tj_text-0.8.1/Makefile
+-rw-r--r--   0        0        0     1114 2024-04-01 12:14:59.970279 tj_text-0.8.1/README.md
+-rw-r--r--   0        0        0      119 2023-07-17 14:49:50.220562 tj_text-0.8.1/pip.conf
+-rw-r--r--   0        0        0      110 2023-07-17 14:49:50.220815 tj_text-0.8.1/policy.yml
+-rw-r--r--   0        0        0     1504 2024-04-01 12:14:59.971758 tj_text-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 14:49:50.221281 tj_text-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:49:50.221534 tj_text-0.8.1/tests/test_tj_text/__init__.py
+-rw-r--r--   0        0        0     7683 2024-04-01 12:14:59.974769 tj_text-0.8.1/tests/test_tj_text/test_expressions.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:49:50.222014 tj_text-0.8.1/tj_text/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-17 14:49:50.222334 tj_text-0.8.1/tj_text/typograph/__init__.py
+-rw-r--r--   0        0        0      834 2023-07-17 14:49:50.222577 tj_text-0.8.1/tj_text/typograph/chars.py
+-rw-r--r--   0        0        0      996 2023-07-17 14:49:50.222798 tj_text-0.8.1/tj_text/typograph/constants.py
+-rw-r--r--   0        0        0      991 2023-07-17 14:49:50.223005 tj_text-0.8.1/tj_text/typograph/core.py
+-rw-r--r--   0        0        0    17830 2024-04-01 12:14:59.976537 tj_text-0.8.1/tj_text/typograph/mixins.py
+-rw-r--r--   0        0        0     8811 2023-07-17 14:49:50.223607 tj_text-0.8.1/tj_text/typograph/processors.py
+-rw-r--r--   0        0        0     3647 2023-07-17 14:49:50.223855 tj_text-0.8.1/tj_text/typograph/utils.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 tj_text-0.8.1/PKG-INFO
```

### Comparing `tj_text-0.8.0/.gitlab-ci.yml` & `tj_text-0.8.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/README.md` & `tj_text-0.8.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ### Публикация пакета в pypi
 
 Пакет публикуется в публичный pypi репозиторий 
 [pypi-tj](https://pypi.org/project/tj-text/) на этапе ci по тэгу в мастер.
 
 Для публикации используется общий аккаунт `tinkoffjournal`. 
-Спросить про доступы можно у @a.gabdullin.
+Спросить про доступы можно у @v.troflyanin.
 
 > **Attention**
 > 
 > Пока не удалось исправить проблему с коннектом через прокси 
 > для публикации пакета в pypi в ci. 
 > 
 > Поэтому заливать пакет нужно **вручную** командой `flit publish`
```

### Comparing `tj_text-0.8.0/tests/test_tj_text/test_expressions.py` & `tj_text-0.8.1/tests/test_tj_text/test_expressions.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,14 +84,31 @@
 
     def test_nbsp_after_hbar_start_of_line(self):
         assert en_typus(f'{HBAR} 31') == f'{HBAR}{NBSP}31'
 
     def test_nbsp_before_hbar_end_of_line(self):
         assert en_typus(f'word {HBAR}') == f'word{NBSP}{HBAR}'
 
+    @pytest.mark.parametrize(
+        'source,expected',
+        [
+            ('1 apple', '1_apple'),
+            ('12 apples', '12_apples'),
+            ('123 apples', '123_apples'),
+            ('1234 apples', '1234_apples'),
+            ('1200 км', '1200_км'),
+            ('400 + 3', '400_+ 3'),
+            ('4000 1', '4000_1'),
+            ('40 000,00 bucks', '40_000,00_bucks'),
+            ('12345 apples', '12345 apples'),
+        ],
+    )
+    def test_whitespace_after_digits(self, source, expected):
+        assert en_typus(source, debug=True) == expected
+
 
 class TestRuExpressions:
     """Tests for typograph.mixins.RuExpressions class."""
 
     def test_expressions_from_parent_class_are_in_child(self):
         for expression in ru_typus.expressions:
             assert expression in RuExpressions.expressions
```

### Comparing `tj_text-0.8.0/tj_text/typograph/chars.py` & `tj_text-0.8.1/tj_text/typograph/chars.py`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/tj_text/typograph/constants.py` & `tj_text-0.8.1/tj_text/typograph/constants.py`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/tj_text/typograph/core.py` & `tj_text-0.8.1/tj_text/typograph/core.py`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/tj_text/typograph/mixins.py` & `tj_text-0.8.1/tj_text/typograph/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,28 +270,25 @@
                 r'\1{0}\2{0}\3'.format(NDASH),
             ),
         )
         return expr
 
     def expr_digit_spaces(self):
         """
-        Replaces whitespace with non-breakable space after 4 (and less)
-        length digits if word or digit without comma or math operators
-        found afterwards:
+        Replaces whitespace with non-breaking space after 4 (and less)
+        length digits if word or digit or math operators found afterward:
         3 apples
         40 000 bucks
         400 + 3
         Skips:
-        4000 bucks
-        40 000,00 bucks
+        40000 bucks
         """
-
         expr = (
             (
-                r'\b(\d{{1,3}}){0}(?=[0-9]+\b|{1}|{2})'.format(
+                r'\b(\d{{1,4}}){0}(?=[0-9]+\b|{1}|{2})'.format(
                     WHSP, self.words, self.math_operators
                 ),
                 r'\1' + NBSP,
             ),
         )
         return expr
```

### Comparing `tj_text-0.8.0/tj_text/typograph/processors.py` & `tj_text-0.8.1/tj_text/typograph/processors.py`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/tj_text/typograph/utils.py` & `tj_text-0.8.1/tj_text/typograph/utils.py`

 * *Files identical despite different names*

### Comparing `tj_text-0.8.0/PKG-INFO` & `tj_text-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: tj-text
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tj text utils
 Author-email: Tj <tinkoffjournal@tjournal.tech>
 Requires-Python: >=3.6
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ipython ; extra == "dev"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: isort ; extra == "test"
```

