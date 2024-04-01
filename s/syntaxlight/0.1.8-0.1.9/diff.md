# Comparing `tmp/syntaxlight-0.1.8.tar.gz` & `tmp/syntaxlight-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.8.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.9.tar", max compression
```

## Comparing `syntaxlight-0.1.8.tar` & `syntaxlight-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.8/LICENSE
--rw-r--r--   0        0        0      463 2023-08-08 08:07:50.096903 syntaxlight-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.8/README.md
--rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.8/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.8/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.8/syntaxlight/css/all.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.8/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.8/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.8/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.8/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.8/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.8/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.8/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      876 2023-08-08 02:48:11.688084 syntaxlight-0.1.8/syntaxlight/css/riscvasm.css
--rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.8/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     3068 2023-08-08 01:56:22.718774 syntaxlight-0.1.8/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.8/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      625 2023-08-08 02:07:40.488130 syntaxlight-0.1.8/syntaxlight/css/x86asm.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.8/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.8/syntaxlight/error.py
--rw-r--r--   0        0        0     1941 2023-08-08 02:05:48.378946 syntaxlight-0.1.8/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-08-08 01:51:12.605756 syntaxlight-0.1.8/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.8/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2270 2023-08-08 02:03:57.826551 syntaxlight-0.1.8/syntaxlight/language.py
--rw-r--r--   0        0        0      655 2023-08-08 02:00:04.293166 syntaxlight-0.1.8/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     5624 2023-08-08 02:37:33.290993 syntaxlight-0.1.8/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.8/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12886 2023-08-08 07:48:52.889333 syntaxlight-0.1.8/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.8/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.8/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.8/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.8/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.8/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.8/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.8/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.8/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      432 2023-08-08 01:59:24.336858 syntaxlight-0.1.8/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     4621 2023-08-08 02:47:31.924199 syntaxlight-0.1.8/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.8/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   107472 2023-08-08 08:07:35.217460 syntaxlight-0.1.8/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.8/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.8/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.8/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.8/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.8/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.8/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.8/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.8/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.8/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.8/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.9/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-08 08:13:46.395916 syntaxlight-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.9/README.md
+-rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.9/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.9/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.9/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.9/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2274 2023-08-08 08:13:17.253527 syntaxlight-0.1.9/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.9/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.9/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.9/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.9/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.9/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      876 2023-08-08 02:48:11.688084 syntaxlight-0.1.9/syntaxlight/css/riscvasm.css
+-rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.9/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     3068 2023-08-08 01:56:22.718774 syntaxlight-0.1.9/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.9/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      625 2023-08-08 02:07:40.488130 syntaxlight-0.1.9/syntaxlight/css/x86asm.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.9/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.9/syntaxlight/error.py
+-rw-r--r--   0        0        0     1941 2023-08-08 02:05:48.378946 syntaxlight-0.1.9/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-08-08 01:51:12.605756 syntaxlight-0.1.9/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.9/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2270 2023-08-08 02:03:57.826551 syntaxlight-0.1.9/syntaxlight/language.py
+-rw-r--r--   0        0        0      655 2023-08-08 02:00:04.293166 syntaxlight-0.1.9/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     5624 2023-08-08 02:37:33.290993 syntaxlight-0.1.9/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.9/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12886 2023-08-08 07:48:52.889333 syntaxlight-0.1.9/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.9/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.9/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.9/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.9/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.9/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.9/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.9/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.9/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      432 2023-08-08 01:59:24.336858 syntaxlight-0.1.9/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     4621 2023-08-08 02:47:31.924199 syntaxlight-0.1.9/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.9/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   107371 2023-08-08 08:12:26.010156 syntaxlight-0.1.9/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.9/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.9/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.9/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.9/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.9/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.9/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.9/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.9/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.9/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.9/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.9/PKG-INFO
```

### Comparing `syntaxlight-0.1.8/LICENSE` & `syntaxlight-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/README.md` & `syntaxlight-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/ast.py` & `syntaxlight-0.1.9/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/all.css` & `syntaxlight-0.1.9/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/bnf.css` & `syntaxlight-0.1.9/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/c.css` & `syntaxlight-0.1.9/syntaxlight/css/c.css`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,22 @@
 .Token.TYPEDEF,
 .Token.CONST,
 .Token.VOLATITLE,
 .Token.RESTRICT,
 .Token._ATOMIC,
 .Token._STATIC_ASSERT,
 .Token._GENERIC,
-.Token.GNU-C-Extension {
+.Token.GNU_C_Assembly {
     color: --type;
 }
 
+.Token.GNU_C_Assembly._ATTRIBUTE {
+    color: --function;
+}
+
 .Token.ID {
     color: --variant;
 }
 
 .Token.NUMBER {
     color: --number;
 }
```

### Comparing `syntaxlight-0.1.8/syntaxlight/css/css.css` & `syntaxlight-0.1.9/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/index.css` & `syntaxlight-0.1.9/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/json.css` & `syntaxlight-0.1.9/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/lua.css` & `syntaxlight-0.1.9/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/makefile.css` & `syntaxlight-0.1.9/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/riscvasm.css` & `syntaxlight-0.1.9/syntaxlight/css/riscvasm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/shell.css` & `syntaxlight-0.1.9/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/themes.json` & `syntaxlight-0.1.9/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/toml.css` & `syntaxlight-0.1.9/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/css/x86asm.css` & `syntaxlight-0.1.9/syntaxlight/css/x86asm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/error.py` & `syntaxlight-0.1.9/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/example.py` & `syntaxlight-0.1.9/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/export.py` & `syntaxlight-0.1.9/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/gdt.py` & `syntaxlight-0.1.9/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/language.py` & `syntaxlight-0.1.9/syntaxlight/language.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/__init__.py` & `syntaxlight-0.1.9/syntaxlight/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/asm_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/makefile_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.9/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/asm_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/asm_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/c_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     STRUCTURE_TYPE = "StructureType"
     QUALIFY_TYPE = "QualifyType"
     HEADER_NAME = "HeaderName"
     ALIGN_SPECIFIER = "AlignSpecifier"
     ATOMAIC_TYPE_SPECIFIER = "AtomicTypeSpecifier"
     STRUCTURE_CLASS = "StructureClass"
     GOTO_LABEL = "GotoLabel"
-    GNU_C_EXTENSION = "GNU-C-Extension"
 
 
 class TranslationUnit(AST):
     def __init__(self, declarations) -> None:
         super().__init__()
         self.declarations = declarations
 
@@ -2249,17 +2248,17 @@
                            | inline
                            | goto
 
         <OutputOperands> ::= ":" <STRING>? ( "(" <constant_expression> ")" ) ("," <STRING>? ( "(" <constant_expression> ")" ))*
         """
         node = GNU_C_Assembly()
         assert self.current_token.type in self.cfirst_set.gnu_c_statement_extension
-        node.update(keyword=self.get_keyword(css_type=C_CSS.GNU_C_EXTENSION))
+        node.update(keyword=self.get_keyword())
         if self.current_token.type in (CTokenType.VOLATILE, CTokenType.INLINE, CTokenType.GOTO):
-            node.update(asm_qualifier=self.get_keyword(css_type=C_CSS.GNU_C_EXTENSION))
+            node.update(asm_qualifier=self.get_keyword())
         node.register_token(self.eat(TokenType.LPAREN))
 
         while self.current_token.type == TokenType.STRING:
             self.string_inside_format()
 
         while self.current_token.type == TokenType.COLON:
             node.register_token(self.eat(TokenType.COLON))
```

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.9/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.9/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.8/PKG-INFO` & `syntaxlight-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.8
+Version: 0.1.9
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

