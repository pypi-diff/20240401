# Comparing `tmp/mkdocs-bibtex-2.8.9.tar.gz` & `tmp/mkdocs-bibtex-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-bibtex-2.8.9.tar", last modified: Sun Jan  8 01:15:43 2023, max compression
+gzip compressed data, was "dist/mkdocs-bibtex-2.9.0.tar", last modified: Tue Jun  6 04:39:26 2023, max compression
```

## Comparing `mkdocs-bibtex-2.8.9.tar` & `mkdocs-bibtex-2.9.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.github/workflows/post-process.yml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/requirements-testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/test_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 01:15:43.000000 mkdocs-bibtex-2.8.9/test_files/multi_bib/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/multi_bib/bib1.bib
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/multi_bib/bib2.bib
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/nature.csl
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/springer-basic-author-date.csl
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/test.bib
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-01-08 01:15:34.000000 mkdocs-bibtex-2.8.9/test_files/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.github/workflows/post-process.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/requirements-testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/test_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/test_files/multi_bib/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/multi_bib/bib1.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:39:26.000000 mkdocs-bibtex-2.9.0/test_files/multi_bib/multi_bib_child_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/multi_bib/multi_bib_child_dir/bib2.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/nature.csl
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/springer-basic-author-date.csl
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/test.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-06 04:39:17.000000 mkdocs-bibtex-2.9.0/test_files/test_utils.py
```

### Comparing `mkdocs-bibtex-2.8.9/.github/workflows/post-process.yml` & `mkdocs-bibtex-2.9.0/.github/workflows/post-process.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/.github/workflows/release.yml` & `mkdocs-bibtex-2.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/.github/workflows/testing.yml` & `mkdocs-bibtex-2.9.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/.gitignore` & `mkdocs-bibtex-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/LICENSE` & `mkdocs-bibtex-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/PKG-INFO` & `mkdocs-bibtex-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-bibtex
-Version: 2.8.9
+Version: 2.9.0
 Summary: An MkDocs plugin that enables managing citations with BibTex
 Home-page: https://github.com/shyamd/mkdocs-bibtex/
 Author: Shyam Dwaraknath
 Author-email: shyamd@lbl.gov
 License: BSD-3-Clause-LBNL
 Description: [![testing](https://github.com/shyamd/mkdocs-bibtex/workflows/testing/badge.svg)](https://github.com/shyamd/mkdocs-bibtex/actions?query=workflow%3Atesting)
         [![codecov](https://codecov.io/gh/shyamd/mkdocs-bibtex/branch/main/graph/badge.svg)](https://codecov.io/gh/shyamd/mkdocs-bibtex)
```

### Comparing `mkdocs-bibtex-2.8.9/README.md` & `mkdocs-bibtex-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/setup.py` & `mkdocs-bibtex-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-bibtex",
     use_scm_version=True,
-    setup_requires=["setuptools_scm", "setuptools"],
+    setup_requires=["setuptools_scm"],
     description="An MkDocs plugin that enables managing citations with BibTex",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs python markdown bibtex",
     url="https://github.com/shyamd/mkdocs-bibtex/",
     author="Shyam Dwaraknath",
     author_email="shyamd@lbl.gov",
```

### Comparing `mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/plugin.py` & `mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         ("bib_file", config_options.Type(str, required=False)),
         ("bib_dir", config_options.Dir(exists=True, required=False)),
         ("bib_command", config_options.Type(str, default="\\bibliography")),
         ("bib_by_default", config_options.Type(bool, default=True)),
         ("full_bib_command", config_options.Type(str, default="\\full_bibliography")),
         ("csl_file", config_options.Type(str, default="")),
         ("cite_inline", config_options.Type(bool, default=False)),
+        ("footnote_format", config_options.Type(str, default="{number}")),
     ]
 
     def __init__(self):
         self.bib_data = None
         self.all_references = OrderedDict()
         self.unescape_for_arithmatex = False
 
@@ -62,15 +63,15 @@
             is_url = validators.url(self.config["bib_file"])
             # if bib_file is a valid URL, cache it with tempfile
             if is_url:
                 bibfiles.append(tempfile_from_url(self.config["bib_file"], ".bib"))
             else:
                 bibfiles.append(self.config["bib_file"])
         elif self.config.get("bib_dir", None) is not None:
-            bibfiles.extend(Path(self.config["bib_dir"]).glob("*.bib"))
+            bibfiles.extend(Path(self.config["bib_dir"]).rglob("*.bib"))
         else:  # pragma: no cover
             raise Exception("Must supply a bibtex file or directory for bibtex files")
 
         # load bibliography data
         refs = {}
         for bibfile in bibfiles:
             bibdata = parse_file(bibfile)
@@ -86,27 +87,32 @@
             self.csl_file = self.config.get("csl_file", None)
 
         # Toggle whether or not to render citations inline (Requires CSL)
         self.cite_inline = self.config.get("cite_inline", False)
         if self.cite_inline and not self.csl_file:  # pragma: no cover
             raise Exception("Must supply a CSL file in order to use cite_inline")
 
+        if "{number}" not in self.config.get("footnote_format"):
+            raise Exception("Must include `{number}` placeholder in footnote_format")
+
+        self.footnote_format = self.config.get("footnote_format")
+
         return config
 
     def on_page_markdown(self, markdown, page, config, files):
         """
         Parses the markdown for each page, extracting the bibtex references
         If a local reference list is requested, this will render that list where requested
 
         1. Finds all cite keys (may include multiple citation references)
         2. Convert all cite keys to citation quads:
             (full cite key,
-            induvidual cite key,
+            individual cite key,
             citation key in corresponding style,
-            citation for induvidual cite key)
+            citation for individual cite key)
         3. Insert formatted cite keys into text
         4. Insert the bibliography into the markdown
         5. Insert the full bibliograph into the markdown
         """
 
         # 1. Grab all the cited keys in the markdown
         cite_keys = find_cite_blocks(markdown)
@@ -146,14 +152,26 @@
             re.escape(full_bib_command),
             self.full_bibliography,
             markdown,
         )
 
         return markdown
 
+    def format_footnote_key(self, number):
+        """
+        Create footnote key based on footnote_format
+
+        Args:
+            number (int): citation number
+
+        Returns:
+            formatted footnote
+        """
+        return self.footnote_format.format(number=number)
+
     def format_citations(self, cite_keys):
         """
         Formats references into citation quads and adds them to the global registry
 
         Args:
             cite_keys (list): List of full cite_keys that maybe compound keys
 
@@ -185,26 +203,34 @@
         if self.csl_file:
             self.all_references.update(format_pandoc(entries, self.csl_file))
         else:
             self.all_references.update(format_simple(entries))
 
         # 4. Construct quads
         quads = [
-            (cite_block, key, numbers[key], self.all_references[key])
+            (
+                cite_block,
+                key,
+                self.format_footnote_key(numbers[key]),
+                self.all_references[key],
+            )
             for cite_block, key in pairs
         ]
 
         # List the quads in order to remove duplicate entries
         return list(dict.fromkeys(quads))
 
     @property
     def full_bibliography(self):
         """
         Returns the full bibliography text
         """
 
         bibliography = []
         for number, (key, citation) in enumerate(self.all_references.items()):
-            bibliography_text = "[^{}]: {}".format(number, citation)
+            bibliography_text = "[^{}]: {}".format(
+                number,
+                citation,
+            )
             bibliography.append(bibliography_text)
 
         return "\n".join(bibliography)
```

### Comparing `mkdocs-bibtex-2.8.9/src/mkdocs_bibtex/utils.py` & `mkdocs-bibtex-2.9.0/src/mkdocs_bibtex/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     return citation.strip()
 
 
 def extract_cite_keys(cite_block):
     """
     Extract just the keys from a citation block
     """
-    cite_regex = re.compile(r"@([\w:-]*)")
+    cite_regex = re.compile(r"@([\w\.:-]*)")
     cite_keys = re.findall(cite_regex, cite_block)
 
     return cite_keys
 
 
 def find_cite_blocks(markdown):
     """
```

### Comparing `mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/PKG-INFO` & `mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-bibtex
-Version: 2.8.9
+Version: 2.9.0
 Summary: An MkDocs plugin that enables managing citations with BibTex
 Home-page: https://github.com/shyamd/mkdocs-bibtex/
 Author: Shyam Dwaraknath
 Author-email: shyamd@lbl.gov
 License: BSD-3-Clause-LBNL
 Description: [![testing](https://github.com/shyamd/mkdocs-bibtex/workflows/testing/badge.svg)](https://github.com/shyamd/mkdocs-bibtex/actions?query=workflow%3Atesting)
         [![codecov](https://codecov.io/gh/shyamd/mkdocs-bibtex/branch/main/graph/badge.svg)](https://codecov.io/gh/shyamd/mkdocs-bibtex)
```

### Comparing `mkdocs-bibtex-2.8.9/src/mkdocs_bibtex.egg-info/SOURCES.txt` & `mkdocs-bibtex-2.9.0/src/mkdocs_bibtex.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,12 @@
 src/mkdocs_bibtex.egg-info/dependency_links.txt
 src/mkdocs_bibtex.egg-info/entry_points.txt
 src/mkdocs_bibtex.egg-info/requires.txt
 src/mkdocs_bibtex.egg-info/top_level.txt
 test_files/nature.csl
 test_files/springer-basic-author-date.csl
 test_files/test.bib
+test_files/test_features.py
 test_files/test_plugin.py
+test_files/test_utils.py
 test_files/multi_bib/bib1.bib
-test_files/multi_bib/bib2.bib
+test_files/multi_bib/multi_bib_child_dir/bib2.bib
```

### Comparing `mkdocs-bibtex-2.8.9/test_files/nature.csl` & `mkdocs-bibtex-2.9.0/test_files/nature.csl`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/test_files/springer-basic-author-date.csl` & `mkdocs-bibtex-2.9.0/test_files/springer-basic-author-date.csl`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/test_files/test.bib` & `mkdocs-bibtex-2.9.0/test_files/test.bib`

 * *Files identical despite different names*

### Comparing `mkdocs-bibtex-2.8.9/test_files/test_plugin.py` & `mkdocs-bibtex-2.9.0/test_files/test_features.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,88 @@
+"""
+This test file checks to make sure each feature works rather than checking each
+function. Each feature should have a single test function that covers all the python
+functions it that would need to be tested
+"""
 import os
 
 import pytest
 import pypandoc
 
-from mkdocs_bibtex.plugin import BibTexPlugin, parse_file
+from mkdocs_bibtex.plugin import BibTexPlugin
+
 from mkdocs_bibtex.utils import (
     find_cite_blocks,
     format_bibliography,
     insert_citation_keys,
-    format_simple,
-    format_pandoc,
 )
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 test_files_dir = os.path.abspath(os.path.join(module_dir, "..", "test_files"))
 
 
 @pytest.fixture
 def plugin():
+    """
+    Basic BibTex Plugin without CSL
+    """
     plugin = BibTexPlugin()
     plugin.load_config(
         options={"bib_file": os.path.join(test_files_dir, "test.bib")},
         config_file_path=test_files_dir,
     )
     plugin.on_config(plugin.config)
+    plugin.csl_file = None
     return plugin
 
 
 @pytest.fixture
-def entries():
-    bibdata = parse_file(os.path.join(test_files_dir, "test.bib"))
-    return bibdata.entries
-
-
-def test_bibtex_loading_bibfile(plugin):
-    assert len(plugin.bib_data.entries) == 4
-
+def plugin_advanced_pandoc(plugin):
+    """
+    Enables advanced features via pandoc
+    """
+    # Only valid for Pandoc > 2.11
+    pandoc_version = pypandoc.get_pandoc_version()
+    pandoc_version_tuple = tuple(int(ver) for ver in pandoc_version.split("."))
+    if pandoc_version_tuple <= (2, 11):
+        pytest.skip(f"Unsupported version of pandoc (v{pandoc_version}) installed.")
 
-def test_bibtex_loading_bib_url():
-    plugin = BibTexPlugin()
-    plugin.load_config(
-        options={
-            "bib_file": "https://raw.githubusercontent.com/shyamd/mkdocs-bibtex/main/test_files/test.bib"
-        },
-        config_file_path=test_files_dir,
+    plugin.config["bib_file"] = os.path.join(test_files_dir, "test.bib")
+    plugin.config["csl_file"] = os.path.join(
+        test_files_dir, "springer-basic-author-date.csl"
     )
+    plugin.config["cite_inline"] = True
 
     plugin.on_config(plugin.config)
-    assert len(plugin.bib_data.entries) == 4
 
+    return plugin
 
-def test_bibtex_loading_bibdir():
-    plugin = BibTexPlugin()
-    plugin.load_config(
-        options={"bib_dir": os.path.join(test_files_dir, "multi_bib")},
-        config_file_path=test_files_dir,
-    )
 
-    plugin.on_config(plugin.config)
-    assert len(plugin.bib_data.entries) == 2
+def test_basic_citations(plugin):
+    """
+    Tests super basic citations using the built-in citation style
+    """
+    assert find_cite_blocks("[@test]") == ["[@test]"]
 
+    assert (
+        insert_citation_keys(
+            [
+                (
+                    "[@test]",
+                    "@test",
+                    "1",
+                    "First Author and Second Author",
+                )
+            ],
+            "[@test]",
+        )
+        == "[^1]"
+    )
 
-def test_format_citations(plugin):
-    plugin.csl_file = None
+    ### TODO: test format_bibliography
 
     assert (
         "[@test]",
         "test",
         "1",
         "First Author and Second Author. Test title. *Testing Journal*, 2019.",
     ) == plugin.format_citations(["[@test]"])[0]
@@ -74,30 +90,14 @@
     assert (
         "[@test2]",
         "test2",
         "1",
         "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019.",
     ) == plugin.format_citations(["[@test2]"])[0]
 
-    # Test compound citation
-    assert [
-        (
-            "[@test; @test2]",
-            "test",
-            "1",
-            "First Author and Second Author. Test title. *Testing Journal*, 2019.",
-        ),
-        (
-            "[@test; @test2]",
-            "test2",
-            "2",
-            "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019.",
-        ),
-    ] == plugin.format_citations(["[@test; @test2]"])
-
     # test long citation
     assert (
         "[@Bivort2016]",
         "Bivort2016",
         "1",
         "Benjamin L. De Bivort and Bruno Van Swinderen. Evidence for selective attention in the insect brain. *Current Opinion in Insect Science*, 15:1–7, 2016. [doi:10.1016/j.cois.2016.02.007](https://doi.org/10.1016/j.cois.2016.02.007).",  # noqa: E501
     ) == plugin.format_citations(["[@Bivort2016]"])[0]
@@ -106,82 +106,24 @@
     assert (
         "[@test_citavi]",
         "test_citavi",
         "1",
         "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019. URL: [\\\\url\\{https://doi.org/10.21577/0103\\-5053.20190253\\}](\\url{https://doi.org/10.21577/0103-5053.20190253}).",  # noqa: E501
     ) == plugin.format_citations(["[@test_citavi]"])[0]
 
-    # Test formatting using a CSL style
-    plugin.csl_file = os.path.join(test_files_dir, "nature.csl")
-    assert (
-        "[@test]",
-        "test",
-        "1",
-        "First Author and Second Author. Test title. *Testing Journal*, 2019.",
-    ) == plugin.format_citations(["[@test]"])[0]
-
-    assert (
-        "[@Bivort2016]",
-        "Bivort2016",
-        "1",
-        "Benjamin L. De Bivort and Bruno Van Swinderen. Evidence for selective attention in the insect brain. *Current Opinion in Insect Science*, 15:1–7, 2016. [doi:10.1016/j.cois.2016.02.007](https://doi.org/10.1016/j.cois.2016.02.007).",  # noqa: E501
-    ) == plugin.format_citations(["[@Bivort2016]"])[0]
-
-    # Test a CSL that outputs references in a different style
-    plugin.csl_file = os.path.join(test_files_dir, "springer-basic-author-date.csl")
-    assert (
-        "[@test]",
-        "test",
-        "1",
-        "First Author and Second Author. Test title. *Testing Journal*, 2019.",
-    ) == plugin.format_citations(["[@test]"])[0]
-
-    assert (
-        "[@test_citavi]",
-        "test_citavi",
-        "1",
-        "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019. URL: [\\\\url\\{https://doi.org/10.21577/0103\\-5053.20190253\\}](\\url{https://doi.org/10.21577/0103-5053.20190253}).",  # noqa: E501
-    ) == plugin.format_citations(["[@test_citavi]"])[0]
-
 
-def test_find_cite_blocks():
-    assert find_cite_blocks("[@test]") == ["[@test]"]
+def test_compound_citations(plugin):
+    """
+    Compound citations are citations that include multiple cite keys
+    """
     assert find_cite_blocks("[@test; @test2]") == ["[@test; @test2]"]
     assert find_cite_blocks("[@test]\n [@test; @test2]") == [
         "[@test]",
         "[@test; @test2]",
     ]
-    # Suppressed authors
-    assert find_cite_blocks("[-@test]") == ["[-@test]"]
-    # Affixes
-    assert find_cite_blocks("[see @test]") == ["[see @test]"]
-    assert find_cite_blocks("[@test, p. 15]") == ["[@test, p. 15]"]
-    assert find_cite_blocks("[see @test, p. 15]") == ["[see @test, p. 15]"]
-    assert find_cite_blocks("[see -@test, p. 15]") == ["[see -@test, p. 15]"]
-    # Invalid blocks
-    assert find_cite_blocks("[ @test]") is not True
-    # Citavi . format
-    assert find_cite_blocks("[@Bermudez.2020]") == ["[@Bermudez.2020]"]
-
-
-def test_insert_citation_keys():
-    assert (
-        insert_citation_keys(
-            [
-                (
-                    "[@test]",
-                    "@test",
-                    "1",
-                    "First Author and Second Author",
-                )
-            ],
-            "[@test]",
-        )
-        == "[^1]"
-    )
 
     assert (
         insert_citation_keys(
             [
                 (
                     "[@test; @test2]",
                     "@test",
@@ -196,16 +138,14 @@
                 ),
             ],
             "[@test; @test2]",
         )
         == "[^1][^2]"
     )
 
-
-def test_format_bibliography():
     quads = [
         (
             "[@test; @test2]",
             "@test",
             "1",
             "First Author and Second Author",
         ),
@@ -221,119 +161,94 @@
 
     assert "[^1]: First Author and Second Author" in bib
     assert (
         "[^2]: First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019"
         in bib
     )
 
-
-def test_format_simple(entries):
-    citations = format_simple(entries)
-
-    assert all(k in citations for k in entries)
-    assert all(entry != citations[k] for k, entry in entries.items())
-
-    assert (
-        citations["test"]
-        == "First Author and Second Author. Test title. *Testing Journal*, 2019."
-    )
-    assert (
-        citations["test2"]
-        == "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019."
-    )
+    assert [
+        (
+            "[@test; @test2]",
+            "test",
+            "1",
+            "First Author and Second Author. Test title. *Testing Journal*, 2019.",
+        ),
+        (
+            "[@test; @test2]",
+            "test2",
+            "2",
+            "First Author and Second Author. Test Title (TT). *Testing Journal (TJ)*, 2019.",
+        ),
+    ] == plugin.format_citations(["[@test; @test2]"])
 
 
-def test_format_pandoc(entries):
-    citations = format_pandoc(entries, os.path.join(test_files_dir, "nature.csl"))
+###############
+# PANDOC ONLY #
+###############
 
-    assert all(k in citations for k in entries)
-    assert all(entry != citations[k] for k, entry in entries.items())
 
+def test_basic_pandoc(plugin):
+    plugin.csl_file = os.path.join(test_files_dir, "nature.csl")
     assert (
-        citations["test"]
-        == "Author, F. & Author, S. Test title. *Testing Journal* **1**, (2019)."
-    )
-    assert (
-        citations["test2"]
-        == "Author, F. & Author, S. Test Title (TT). *Testing Journal (TJ)* **1**, (2019)."
-    )
-
-
-def test_on_page_markdown(plugin):
-    plugin.on_config(plugin.config)
-    # run test with bib_by_default set to False
-    plugin.config["bib_by_default"] = False
-
-    test_markdown = "This is a citation. [@test]\n\n \\bibliography"
+        "[@test]",
+        "test",
+        "1",
+        "Author, F. & Author, S. Test title. *Testing Journal* **1**, (2019).",
+    ) == plugin.format_citations(["[@test]"])[0]
 
     assert (
-        "[^1]: First Author and Second Author. Test title. *Testing Journal*, 2019."
-        in plugin.on_page_markdown(test_markdown, None, None, None)
-    )
-
-    # ensure there are two items in bibliography
-    test_markdown = "This is a citation. [@test2] This is another citation [@test]\n\n \\bibliography"
-
-    assert "[^2]:" in plugin.on_page_markdown(test_markdown, None, None, None)
-
-    # ensure bib_by_default is working
-    plugin.config["bib_by_default"] = True
-    test_markdown = "This is a citation. [@test]"
-
-    assert "[^1]:" in plugin.on_page_markdown(test_markdown, None, None, None)
-    plugin.config["bib_by_default"] = False
-
-    # ensure nonexistant citekeys are removed correctly (not replaced)
-    test_markdown = "A non-existant citekey. [@i_do_not_exist]"
-
-    assert "[@i_do_not_exist]" in plugin.on_page_markdown(
-        test_markdown, None, None, None
-    )
-
-    # Ensure if an item is referenced multiple times, it only shows up as one reference
-    test_markdown = "This is a citation. [@test] This is another citation [@test]\n\n \\bibliography"
-
-    assert "[^2]" not in plugin.on_page_markdown(test_markdown, None, None, None)
-
-    # Ensure item only shows up once even if used in multiple places as both a compound and lone cite key
-    test_markdown = "This is a citation. [@test; @test2] This is another citation [@test]\n\n \\bibliography"
-
-    assert "[^3]" not in plugin.on_page_markdown(test_markdown, None, None, None)
+        "[@Bivort2016]",
+        "Bivort2016",
+        "1",
+        "De Bivort, B. L. & Van Swinderen, B. Evidence for selective attention in the insect brain. *Current Opinion in Insect Science* **15**, 1–7 (2016).",  # noqa: E501
+    ) == plugin.format_citations(["[@Bivort2016]"])[0]
 
+    # Test a CSL that outputs references in a different style
+    plugin.csl_file = os.path.join(test_files_dir, "springer-basic-author-date.csl")
+    assert (
+        "[@test]",
+        "test",
+        "1",
+        "Author, F. & Author, S. Test title. *Testing Journal* **1**, (2019).",
+    ) == plugin.format_citations(["[@test]"])[0]
 
-def test_inline_citations(plugin):
-    plugin.config["bib_file"] = os.path.join(test_files_dir, "test.bib")
-    plugin.config["csl_file"] = os.path.join(
-        test_files_dir, "springer-basic-author-date.csl"
-    )
-    plugin.config["cite_inline"] = True
+    assert (
+        "[@test_citavi]",
+        "test_citavi",
+        "1",
+        "Author F, Author S (2019) Test Title (TT). Testing Journal (TJ) 1:",
+    ) == plugin.format_citations(["[@test_citavi]"])[0]
 
-    plugin.on_config(plugin.config)
 
-    pandoc_version = pypandoc.get_pandoc_version()
-    pandoc_version_tuple = tuple(int(ver) for ver in pandoc_version.split("."))
-    if pandoc_version_tuple <= (2, 11):
-        pytest.skip(f"Unsupported version of pandoc (v{pandoc_version}) installed.")
+def test_inline_ciations(plugin_advanced_pandoc):
+    plugin = plugin_advanced_pandoc
 
     # Ensure inline citation works
     quads = [("[@test]", None, "1", None)]
     test_markdown = "Hello[@test]"
     result = "Hello (Author and Author 2019)[^1]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
 
+
+def test_supressed_authors(plugin_advanced_pandoc):
+    plugin = plugin_advanced_pandoc
+
     # Ensure suppressed authors works
     quads = [("[-@test]", None, "1", None)]
     test_markdown = "Suppressed [-@test]"
     result = "Suppressed (2019)[^1]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
 
+
+def test_affixes(plugin_advanced_pandoc):
+    plugin = plugin_advanced_pandoc
     # Ensure affixes work
     quads = [("[see @test]", None, "1", None)]
     test_markdown = "Hello[see @test]"
     result = "Hello (see Author and Author 2019)[^1]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
@@ -357,14 +272,29 @@
     quads = [("[see -@test, p. 123]", None, "1", None)]
     test_markdown = "Suppressed [see -@test, p. 123]"
     result = "Suppressed (see 2019, p. 123)[^1]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
 
+
+def test_invalid_blocks(plugin_advanced_pandoc):
+    pass
+
+
+def test_citavi_format(plugin_advanced_pandoc):
+    pass
+
+
+def test_duplicate_reference(plugin_advanced_pandoc):
+    """
+    Ensures duplicats references show up appropriately
+    # TODO: These test cases don't seem right
+    """
+    plugin = plugin_advanced_pandoc
     # Ensure multi references work
     quads = [
         ("[@test; @Bivort2016]", None, "1", None),
         ("[@test; @Bivort2016]", None, "2", None),
     ]
     test_markdown = "[@test; @Bivort2016]"
     # CSL defines the order, this ordering is therefore expected with springer.csl
@@ -380,17 +310,39 @@
     test_markdown = "[@test, p. 12; @Bivort2016, p. 15]"
     # CSL defines the order, this ordering is therefore expected with springer.csl
     result = " (De Bivort and Van Swinderen 2016, p. 15; Author and Author 2019, p. 12)[^1][^2]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
 
+
+def test_multi_reference(plugin_advanced_pandoc):
+    """
+    Ensures multiple inline references show up appropriately
+    """
+
+    plugin = plugin_advanced_pandoc
     # Ensure multiple inline references works
     quads = [
         ("[@test]", None, "1", None),
         ("[see @Bivort2016, p. 123]", None, "2", None),
     ]
     test_markdown = "Hello[@test] World [see @Bivort2016, p. 123]"
     result = "Hello (Author and Author 2019)[^1] World (see De Bivort and Van Swinderen 2016, p. 123)[^2]"
     assert result == insert_citation_keys(
         quads, test_markdown, plugin.csl_file, plugin.bib_data.to_string("bibtex")
     )
+
+
+def test_custom_footnote_formatting(plugin):
+
+    assert plugin.format_footnote_key(1) == "1"
+    plugin.footnote_format = "Test Format {number}"
+    assert plugin.format_footnote_key(1) == "Test Format 1"
+
+    plugin.csl_file = os.path.join(test_files_dir, "nature.csl")
+    assert (
+        "[@test]",
+        "test",
+        "Test Format 1",
+        "Author, F. & Author, S. Test title. *Testing Journal* **1**, (2019).",
+    ) == plugin.format_citations(["[@test]"])[0]
```

