# Comparing `tmp/typos-1.20.0.tar.gz` & `tmp/typos-1.20.1.tar.gz`

## Comparing `typos-1.20.0.tar` & `typos-1.20.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0     1001      127      589 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos/Cargo.toml
--rw-r--r--   0     1001      127     2794 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos/src/check.rs
--rw-r--r--   0     1001      127     2167 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos/src/dict.rs
--rw-r--r--   0     1001      127       74 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos/src/lib.rs
--rw-r--r--   0     1001      127    46856 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos/src/tokens.rs
--rw-r--r--   0     1001      127     5770 2024-04-01 18:45:58.000000 typos-1.20.0/README.md
--rw-r--r--   0     1001      127      921 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-vars/Cargo.toml
--rw-r--r--   0     1001      127      117 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-vars/src/lib.rs
--rw-r--r--   0     1001      127  6086180 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-vars/src/vars_codegen.rs
--rw-r--r--   0     1001      127      739 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-dict/Cargo.toml
--rw-r--r--   0     1001      127       59 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-dict/src/lib.rs
--rw-r--r--   0     1001      127  7270058 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-dict/src/word_codegen.rs
--rw-r--r--   0     1001      127      541 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon-core/Cargo.toml
--rw-r--r--   0     1001      127     1488 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      127     2850 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon-core/src/lib.rs
--rw-r--r--   0     1001      127    18974 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon-core/src/parser.rs
--rw-r--r--   0     1001      127      646 2024-04-01 18:45:58.000000 typos-1.20.0/crates/dictgen/Cargo.toml
--rw-r--r--   0     1001      127      130 2024-04-01 18:45:58.000000 typos-1.20.0/crates/dictgen/src/lib.rs
--rw-r--r--   0     1001      127     2687 2024-04-01 18:45:58.000000 typos-1.20.0/crates/dictgen/src/map.rs
--rw-r--r--   0     1001      127     3726 2024-04-01 18:45:58.000000 typos-1.20.0/crates/dictgen/src/table.rs
--rw-r--r--   0     1001      127    10629 2024-04-01 18:45:58.000000 typos-1.20.0/crates/dictgen/src/trie.rs
--rw-r--r--   0     1001      127      671 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon/Cargo.toml
--rw-r--r--   0     1001      127 12563224 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon/src/codegen.rs
--rw-r--r--   0     1001      127      432 2024-04-01 18:45:58.000000 typos-1.20.0/crates/varcon/src/lib.rs
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 typos-1.20.0/crates/typos-cli/Cargo.toml
--rw-r--r--   0     1001      127     3092 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/benches/check_file.rs
--rw-r--r--   0     1001      127     5640 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/benches/correct_word.rs
--rw-r--r--   0     1001      127     1724 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/benches/data.rs
--rw-r--r--   0     1001      127     3298 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      127     8981 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      127    12158 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      127    11379 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      127    20949 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/config.rs
--rw-r--r--   0     1001      127    10403 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      127    12513 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/dict.rs
--rw-r--r--   0     1001      127    33435 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/file.rs
--rw-r--r--   0     1001      127     6790 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      127     3460 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/file_type_specifics.rs
--rw-r--r--   0     1001      127      324 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/lib.rs
--rw-r--r--   0     1001      127    17561 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/policy.rs
--rw-r--r--   0     1001      127     5551 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/src/report.rs
--rw-r--r--   0     1001      127      228 2024-04-01 18:45:58.000000 typos-1.20.0/crates/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      127    44059 2024-04-01 18:45:58.000000 typos-1.20.0/Cargo.lock
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 typos-1.20.0/Cargo.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 typos-1.20.0/pyproject.toml
--rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 typos-1.20.0/PKG-INFO
+-rw-r--r--   0     1001      127      646 2024-04-01 21:43:11.000000 typos-1.20.1/crates/dictgen/Cargo.toml
+-rw-r--r--   0     1001      127      130 2024-04-01 21:43:11.000000 typos-1.20.1/crates/dictgen/src/lib.rs
+-rw-r--r--   0     1001      127     2687 2024-04-01 21:43:11.000000 typos-1.20.1/crates/dictgen/src/map.rs
+-rw-r--r--   0     1001      127     3726 2024-04-01 21:43:11.000000 typos-1.20.1/crates/dictgen/src/table.rs
+-rw-r--r--   0     1001      127    10629 2024-04-01 21:43:11.000000 typos-1.20.1/crates/dictgen/src/trie.rs
+-rw-r--r--   0     1001      127      589 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos/Cargo.toml
+-rw-r--r--   0     1001      127     2794 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos/src/check.rs
+-rw-r--r--   0     1001      127     2167 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos/src/dict.rs
+-rw-r--r--   0     1001      127       74 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos/src/lib.rs
+-rw-r--r--   0     1001      127    46856 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos/src/tokens.rs
+-rw-r--r--   0     1001      127     5770 2024-04-01 21:43:11.000000 typos-1.20.1/README.md
+-rw-r--r--   0     1001      127      671 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon/Cargo.toml
+-rw-r--r--   0     1001      127 12563224 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon/src/codegen.rs
+-rw-r--r--   0     1001      127      432 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon/src/lib.rs
+-rw-r--r--   0     1001      127      921 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      127      117 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      127  6086180 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0     1001      127      541 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      127     1488 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      127     2850 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      127    18974 2024-04-01 21:43:11.000000 typos-1.20.1/crates/varcon-core/src/parser.rs
+-rw-r--r--   0     1001      127      740 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      127       59 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-dict/src/lib.rs
+-rw-r--r--   0     1001      127  7269664 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-dict/src/word_codegen.rs
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 typos-1.20.1/crates/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      127     3092 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/benches/check_file.rs
+-rw-r--r--   0     1001      127     5640 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/benches/correct_word.rs
+-rw-r--r--   0     1001      127     1724 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      127     3298 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      127     8981 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      127    12158 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      127    11379 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      127    20949 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/config.rs
+-rw-r--r--   0     1001      127    10403 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      127    12513 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      127    33435 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/file.rs
+-rw-r--r--   0     1001      127     6790 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      127     3460 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/file_type_specifics.rs
+-rw-r--r--   0     1001      127      324 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      127    17561 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      127     5551 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/src/report.rs
+-rw-r--r--   0     1001      127      228 2024-04-01 21:43:11.000000 typos-1.20.1/crates/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      127    44060 2024-04-01 21:43:11.000000 typos-1.20.1/Cargo.lock
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 typos-1.20.1/Cargo.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 typos-1.20.1/pyproject.toml
+-rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 typos-1.20.1/PKG-INFO
```

### Comparing `typos-1.20.0/crates/typos/Cargo.toml` & `typos-1.20.1/crates/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos/src/check.rs` & `typos-1.20.1/crates/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos/src/dict.rs` & `typos-1.20.1/crates/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos/src/tokens.rs` & `typos-1.20.1/crates/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/README.md` & `typos-1.20.1/README.md`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-vars/Cargo.toml` & `typos-1.20.1/crates/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-vars/src/vars_codegen.rs` & `typos-1.20.1/crates/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-dict/Cargo.toml` & `typos-1.20.1/crates/typos-dict/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-dict"
-version = "0.11.9"
+version = "0.11.11"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license.workspace = true
 repository.workspace = true
 edition.workspace = true
```

### Comparing `typos-1.20.0/crates/typos-dict/src/word_codegen.rs` & `typos-1.20.1/crates/typos-dict/src/word_codegen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -82660,15 +82660,15 @@
         &["otherwise"],
     ],
     range: 2..=7,
 };
 
 static WORD_OG_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_OG_CHILDREN),
-    value: Some(&["of"]),
+    value: None,
 };
 
 pub static WORD_OG_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("anization"),
         dictgen::InsensitiveStr::Ascii("er"),
         dictgen::InsensitiveStr::Ascii("erish"),
@@ -134867,15 +134867,15 @@
     Some(&WORD_EH_NODE),
     Some(&WORD_EI_NODE),
     Some(&WORD_EJ_NODE),
     None,
     Some(&WORD_EL_NODE),
     Some(&WORD_EM_NODE),
     Some(&WORD_EN_NODE),
-    Some(&WORD_EO_NODE),
+    None,
     Some(&WORD_EP_NODE),
     Some(&WORD_EQ_NODE),
     Some(&WORD_ER_NODE),
     Some(&WORD_ES_NODE),
     Some(&WORD_ET_NODE),
     Some(&WORD_EU_NODE),
     Some(&WORD_EV_NODE),
@@ -143329,25 +143329,14 @@
         &["expected"],
         &["expressions"],
         &["explicit"],
     ],
     range: 2..=10,
 };
 
-static WORD_EO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
-    children: dictgen::DictTrieChild::Flat(&WORD_EO_CHILDREN),
-    value: None,
-};
-
-pub static WORD_EO_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("f")],
-    values: &[&["of"]],
-    range: 1..=1,
-};
-
 static WORD_EN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_EN_CHILDREN),
     value: None,
 };
 
 static WORD_EN_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
     Some(&WORD_ENA_NODE),
```

### Comparing `typos-1.20.0/crates/varcon-core/Cargo.toml` & `typos-1.20.1/crates/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/varcon-core/src/borrowed.rs` & `typos-1.20.1/crates/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/varcon-core/src/lib.rs` & `typos-1.20.1/crates/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/varcon-core/src/parser.rs` & `typos-1.20.1/crates/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/dictgen/Cargo.toml` & `typos-1.20.1/crates/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/dictgen/src/map.rs` & `typos-1.20.1/crates/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/dictgen/src/table.rs` & `typos-1.20.1/crates/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/dictgen/src/trie.rs` & `typos-1.20.1/crates/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/varcon/Cargo.toml` & `typos-1.20.1/crates/varcon/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/varcon/src/codegen.rs` & `typos-1.20.1/crates/varcon/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/Cargo.toml` & `typos-1.20.1/crates/typos-cli/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.20.0"
+version = "1.20.1"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license.workspace = true
 repository.workspace = true
 edition.workspace = true
```

### Comparing `typos-1.20.0/crates/typos-cli/benches/check_file.rs` & `typos-1.20.1/crates/typos-cli/benches/check_file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/benches/correct_word.rs` & `typos-1.20.1/crates/typos-cli/benches/correct_word.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/benches/data.rs` & `typos-1.20.1/crates/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/benches/tokenize.rs` & `typos-1.20.1/crates/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.20.1/crates/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.20.1/crates/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.20.1/crates/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/config.rs` & `typos-1.20.1/crates/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/default_types.rs` & `typos-1.20.1/crates/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/dict.rs` & `typos-1.20.1/crates/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/file.rs` & `typos-1.20.1/crates/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/file_type.rs` & `typos-1.20.1/crates/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/file_type_specifics.rs` & `typos-1.20.1/crates/typos-cli/src/file_type_specifics.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/policy.rs` & `typos-1.20.1/crates/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/crates/typos-cli/src/report.rs` & `typos-1.20.1/crates/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.0/Cargo.lock` & `typos-1.20.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1334,15 +1334,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.20.0"
+version = "1.20.1"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "bstr",
@@ -1381,15 +1381,15 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.11.9"
+version = "0.11.11"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "indexmap",
  "itertools 0.12.0",
```

### Comparing `typos-1.20.0/PKG-INFO` & `typos-1.20.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typos
-Version: 1.20.0
+Version: 1.20.1
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

