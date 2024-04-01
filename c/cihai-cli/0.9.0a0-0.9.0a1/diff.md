# Comparing `tmp/cihai-cli-0.9.0a0.tar.gz` & `tmp/cihai-cli-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cihai-cli-0.9.0a0.tar", max compression
+gzip compressed data, was "cihai-cli-0.9.0a1.tar", max compression
```

## Comparing `cihai-cli-0.9.0a0.tar` & `cihai-cli-0.9.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1092 2022-05-22 22:12:48.706400 cihai-cli-0.9.0a0/LICENSE
--rw-r--r--   0        0        0     5213 2022-05-22 22:12:48.706400 cihai-cli-0.9.0a0/README.md
--rw-r--r--   0        0        0      512 2022-05-22 22:12:48.706400 cihai-cli-0.9.0a0/cihai_cli/__about__.py
--rw-r--r--   0        0        0        0 2022-05-22 22:12:48.706400 cihai-cli-0.9.0a0/cihai_cli/__init__.py
--rw-r--r--   0        0        0     4038 2022-05-22 22:12:48.706400 cihai-cli-0.9.0a0/cihai_cli/cli.py
--rw-r--r--   0        0        0     2471 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/pyproject.toml
--rw-r--r--   0        0        0     1038 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/conftest.py
--rw-r--r--   0        0        0     2008 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_DictionaryIndices.txt
--rw-r--r--   0        0        0     1140 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_DictionaryLikeData.txt
--rw-r--r--   0        0        0     1680 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_IRGSources.txt
--rw-r--r--   0        0        0     2428 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_NumericValues.txt
--rw-r--r--   0        0        0     2261 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_OtherMappings.txt
--rw-r--r--   0        0        0     1015 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_RadicalStrokeCounts.txt
--rw-r--r--   0        0        0     3515 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_Readings.txt
--rw-r--r--   0        0        0     1981 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/Unihan_Variants.txt
--rw-r--r--   0        0        0       38 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/fixtures/test_config.yml
--rw-r--r--   0        0        0     1358 2022-05-22 22:12:48.710399 cihai-cli-0.9.0a0/tests/test_cli.py
--rw-r--r--   0        0        0     6239 2022-05-22 22:14:18.848146 cihai-cli-0.9.0a0/setup.py
--rw-r--r--   0        0        0     6738 2022-05-22 22:14:18.848704 cihai-cli-0.9.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-08-16 14:19:56.853447 cihai-cli-0.9.0a1/LICENSE
+-rw-r--r--   0        0        0     5213 2022-08-16 14:19:56.853447 cihai-cli-0.9.0a1/README.md
+-rw-r--r--   0        0        0      512 2022-08-16 14:19:56.853447 cihai-cli-0.9.0a1/cihai_cli/__about__.py
+-rw-r--r--   0        0        0        0 2022-08-16 14:19:56.853447 cihai-cli-0.9.0a1/cihai_cli/__init__.py
+-rw-r--r--   0        0        0     4038 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/cihai_cli/cli.py
+-rw-r--r--   0        0        0     2922 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1038 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/conftest.py
+-rw-r--r--   0        0        0     2008 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_DictionaryIndices.txt
+-rw-r--r--   0        0        0     1140 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_DictionaryLikeData.txt
+-rw-r--r--   0        0        0     1680 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_IRGSources.txt
+-rw-r--r--   0        0        0     2428 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_NumericValues.txt
+-rw-r--r--   0        0        0     2261 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_OtherMappings.txt
+-rw-r--r--   0        0        0     1015 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_RadicalStrokeCounts.txt
+-rw-r--r--   0        0        0     3515 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_Readings.txt
+-rw-r--r--   0        0        0     1981 2022-08-16 14:19:56.857447 cihai-cli-0.9.0a1/tests/fixtures/Unihan_Variants.txt
+-rw-r--r--   0        0        0       38 2022-08-16 14:19:56.861447 cihai-cli-0.9.0a1/tests/fixtures/test_config.yml
+-rw-r--r--   0        0        0     1358 2022-08-16 14:19:56.861447 cihai-cli-0.9.0a1/tests/test_cli.py
+-rw-r--r--   0        0        0     6239 2022-08-16 14:20:46.452719 cihai-cli-0.9.0a1/setup.py
+-rw-r--r--   0        0        0     6935 2022-08-16 14:20:46.453417 cihai-cli-0.9.0a1/PKG-INFO
```

### Comparing `cihai-cli-0.9.0a0/LICENSE` & `cihai-cli-0.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/README.md` & `cihai-cli-0.9.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/cihai_cli/__about__.py` & `cihai-cli-0.9.0a1/cihai_cli/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = "cihai-cli"
 __package_name__ = "cihai_cli"
-__version__ = "0.9.0a0"
+__version__ = "0.9.0a1"
 __description__ = "Command line frontend for the cihai CJK language library"
 __author__ = "Tony Narlock"
 __email__ = "tony@git-pull.com"
 __github__ = "https://github.com/cihai/cihai-cli"
 __docs__ = "https://cihai-cli.git-pull.com"
 __tracker__ = "https://github.com/cihai/cihai-cli/issues"
 __pypi__ = "https://pypi.org/project/cihai-cli/"
```

### Comparing `cihai-cli-0.9.0a0/cihai_cli/cli.py` & `cihai-cli-0.9.0a1/cihai_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/pyproject.toml` & `cihai-cli-0.9.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cihai-cli"
-version = "0.9.0a0"
+version = "0.9.0a1"
 description = "Command line frontend for the cihai CJK language library"
 license = "MIT"
 authors = ["Tony Narlock <tony@git-pull.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
@@ -13,27 +13,45 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Internationalization",
+  "Topic :: Software Development :: Localization",
   "Topic :: System :: Shells",
-  "Topic :: Utilities"
+  "Topic :: Utilities",
+]
+keywords = [
+  "unihan",
+  "sqlalchemy",
+  "library",
+  "cjk",
+  "unicode",
+  "dictionary",
+  "dataset",
+  "encyclopedia",
+  "chinese",
+  "japanese",
+  "korean",
+  "languages",
+  "study",
+  "cli",
+  "terminal",
+  "shell",
 ]
 homepage = "https://cihai-cli.git-pull.com"
 readme = "README.md"
 packages = [
-    { include = "cihai_cli" }
+  { include = "cihai_cli" },
 ]
 include = [
-    { path = "tests", format = "sdist" }
+  { path = "tests", format = "sdist" },
 ]
 
-
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cihai/cihai-cli/issues"
 Documentation = "https://cihai-cli.git-pull.com"
 Repository = "https://github.com/cihai/cihai-cli"
 "Release notes" = "https://github.com/cihai/cihai-cli/blob/master/CHANGES"
 "Q & A" = "https://github.com/cihai/cihai-cli/discussions"
 
@@ -42,24 +60,25 @@
 click = ">=7<8.2"
 cihai = ">=0.12.0,<0.14.0"
 PyYAML = "<6,>=3.12"
 
 [tool.poetry.dev-dependencies]
 ### Docs ###
 sphinx = "*"
-furo = "^2022.2.23"
-sphinx-autobuild = "^2021.3.14"
-sphinx-autodoc-typehints = "~1.17.0"
+furo = "*"
+sphinx-autobuild = "*"
+sphinx-autodoc-typehints = "*"
 sphinx-click = "*"
-sphinx-issues = "^3.0.0"
+sphinx-issues = "*"
 sphinx-inline-tabs = { version = "*", python = "^3.7" }
 sphinxext-opengraph = "*"
-sphinx-copybutton = "^0.5.0"
+sphinx-copybutton = "*"
 sphinxext-rediraffe = "*"
-myst_parser = "~0.17.0"
+myst_parser = "*"
+docutils = "~0.18.0"
 
 ### Testing ###
 pytest = "*"
 pytest-rerunfailures = "*"
 pytest-watcher = "^0.2.3"
 
 ### Coverage ###
@@ -69,21 +88,43 @@
 
 ### Format ###
 black = "*"
 isort = "*"
 
 ### Lint ###
 flake8 = "*"
+mypy = "*"
+types-PyYAML = "^6.0.11"
 
 [tool.poetry.scripts]
 cihai = 'cihai_cli.cli:cli'
 
 [tool.poetry.extras]
-docs = ["sphinx", "sphinx-issues", "sphinx-click", "sphinx-autodoc-typehints", "sphinx-autobuild", "sphinx-copybutton", "sphinxext-opengraph", "sphinx-inline-tabs", "sphinxext-rediraffe", "myst_parser", "furo"]
+docs = [
+  "docutils",
+  "sphinx",
+  "sphinx-issues",
+  "sphinx-click",
+  "sphinx-autodoc-typehints",
+  "sphinx-autobuild",
+  "sphinx-copybutton",
+  "sphinxext-opengraph",
+  "sphinx-inline-tabs",
+  "sphinxext-rediraffe",
+  "myst_parser",
+  "furo",
+]
 test = ["pytest", "pytest-rerunfailures", "pytest-watcher"]
 coverage = ["codecov", "coverage", "pytest-cov"]
 format = ["black", "isort"]
-lint = ["flake8"]
+lint = ["flake8", "mypy", "types-PyYAML"]
+
+[[tool.mypy.overrides]]
+module = [
+  "cihai.*",
+  "unihan_etl.*"
+]
+ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cihai-cli-0.9.0a0/tests/conftest.py` & `cihai-cli-0.9.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_DictionaryIndices.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_DictionaryIndices.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_DictionaryLikeData.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_DictionaryLikeData.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_IRGSources.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_IRGSources.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_NumericValues.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_NumericValues.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_OtherMappings.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_OtherMappings.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_RadicalStrokeCounts.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_RadicalStrokeCounts.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_Readings.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_Readings.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/fixtures/Unihan_Variants.txt` & `cihai-cli-0.9.0a1/tests/fixtures/Unihan_Variants.txt`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/tests/test_cli.py` & `cihai-cli-0.9.0a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cihai-cli-0.9.0a0/setup.py` & `cihai-cli-0.9.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['PyYAML>=3.12,<6', 'cihai>=0.12.0,<0.14.0', 'click>=7']
 
 entry_points = \
 {'console_scripts': ['cihai = cihai_cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'cihai-cli',
-    'version': '0.9.0a0',
+    'version': '0.9.0a1',
     'description': 'Command line frontend for the cihai CJK language library',
     'long_description': '# cihai-cli\n\nCommand line interface to the [cihai](https://cihai.git-pull.com)\n[CJK](https://cihai.git-pull.com/glossary.html#term-cjk)-language library\n\n[![Python Package](https://img.shields.io/pypi/v/cihai_cli.svg)](https://pypi.org/project/cihai-cli/)\n[![Docs](https://github.com/cihai/cihai-cli/workflows/docs/badge.svg)](https://cihai-cli.git-pull.com/)\n[![Build Status](https://github.com/cihai/cihai-cli/workflows/tests/badge.svg)](https://github.com/cihai/cihai-cli/actions?query=workflow%3A%22tests%22)\n[![Code Coverage](https://codecov.io/gh/cihai/cihai-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/cihai/cihai-cli)\n[![License](https://img.shields.io/github/license/cihai/cihai-cli.svg)](https://github.com/cihai/cihai-cli/blob/master/LICENSE)\n\nThis project is under active development. Follow our progress and check back for updates!\n\n## Installation\n\n```console\n$ pip install --user cihai[cli]\n```\n\n### Developmental releases\n\nYou can test the unpublished version of cihai-cli before its released.\n\n- [pip](https://pip.pypa.io/en/stable/):\n\n  ```console\n  $ pip install --user --upgrade --pre cihai[cli]\n  ```\n\n- [pipx](https://pypa.github.io/pipx/docs/):\n\n  ```console\n  $ pipx install --suffix=@next \'cihai[cli]\' --pip-args \'\\--pre\' --include-deps --force\n  ```\n\n  Then use `cihai@next info 好`.\n\nFor more information see\n[developmental releases](https://cihai-cli.git-pull.com/quickstart.html#developmental-releases)\n\n## Character lookup\n\nSee [CLI](https://cihai-cli.git-pull.com/cli.html) in the documentation for full usage information.\n\n```console\n$ cihai info 好\nchar: 好\nkCantonese: hou2 hou3\nkDefinition: good, excellent, fine; well\nkHangul: 호\nkJapaneseOn: KOU\nkKorean: HO\nkMandarin: hǎo\nkTang: \'*xɑ̀u *xɑ̌u\'\nkTotalStrokes: \'6\'\nucn: U+597D\n\n# retrieve all character information (including book indices)\n$ cihai info 好 -a\nchar: 好\nkCangjie: VND\nkCantonese: hou2 hou3\nkCihaiT: \'378.103\'\nkDefinition: good, excellent, fine; well\nkFenn: 552A\nkFourCornerCode: \'4744.7\'\nkFrequency: \'1\'\nkGradeLevel: \'1\'\nkHKGlyph: 0871\nkHangul: 호\nkHanyuPinlu: hǎo(6060) hāo(142) hào(115)\nkHanyuPinyin: 21028.010:hǎo,hào\nkJapaneseKun: KONOMU SUKU YOI\nkJapaneseOn: KOU\nkKorean: HO\nkMandarin: hǎo\nkPhonetic: \'481\'\nkRSAdobe_Japan1_6: C+1975+38.3.3 C+1975+39.3.3\nkRSKangXi: \'38.3\'\nkTang: \'*xɑ̀u *xɑ̌u\'\nkTotalStrokes: \'6\'\nkVietnamese: háo\nkXHC1983: 0445.030:hǎo 0448.030:hào\nucn: U+597D\n```\n\n## Reverse lookup\n\n```console\n$ cihai reverse library\nchar: 圕\nkCantonese: syu1\nkDefinition: library\nkJapaneseOn: TOSHOKAN SHO\nkMandarin: tú\nkTotalStrokes: \'13\'\nucn: U+5715\n--------\nchar: 嫏\nkCantonese: long4\nkDefinition: the place where the supreme stores his books; library\nkJapaneseOn: ROU\nkMandarin: láng\nkTotalStrokes: \'11\'\nucn: U+5ACF\n--------\n```\n\n## Developing\n\n[poetry](https://python-poetry.org/) is a required package to develop.\n\n`git clone https://github.com/cihai/cihai-cli.git`\n\n`cd cihai-cli`\n\n`poetry install -E "docs test coverage lint format"`\n\nMakefile commands prefixed with `watch_` will watch files and rerun.\n\n### Tests\n\n`poetry run py.test`\n\nHelpers: `make test` Rerun tests on file change: `make watch_test` (requires\n[entr(1)](http://eradman.com/entrproject/))\n\n### Documentation\n\nDefault preview server: <http://localhost:8037>\n\n`cd docs/` and `make html` to build. `make serve` to start http server.\n\nHelpers: `make build_docs`, `make serve_docs`\n\nRebuild docs on file change: `make watch_docs` (requires [entr(1)](http://eradman.com/entrproject/))\n\nRebuild docs and run server via one terminal: `make dev_docs` (requires above, and a `make(1)` with\n`-J` support, e.g. GNU Make)\n\n### Formatting / Linting\n\nThe project uses [black](https://github.com/psf/black) and [isort](https://pypi.org/project/isort/)\n(one after the other) and runs [flake8](https://flake8.pycqa.org/) via CI. See the configuration in\n<span class="title-ref">pyproject.toml</span> and \\`setup.cfg\\`:\n\n`make black isort`: Run `black` first, then `isort` to handle import nuances `make flake8`, to watch\n(requires `entr(1)`): `make watch_flake8`\n\n### Releasing\n\nAs of 0.6, [poetry](https://python-poetry.org/) handles virtualenv creation, package requirements,\nversioning, building, and publishing. Therefore there is no setup.py or requirements files.\n\nUpdate <span class="title-ref">\\_\\_version\\_\\_</span> in <span\nclass="title-ref">\\_\\_about\\_\\_.py</span> and \\`pyproject.toml\\`:\n\n    git commit -m \'build(cihai-cli): Tag v0.1.1\'\n    git tag v0.1.1\n    git push\n    git push --tags\n    poetry build\n    poetry deploy\n\n## Quick links\n\n- [Quickstart](https://cihai-cli.git-pull.com/quickstart.html)\n- Python [API](https://cihai-cli.git-pull.com/api.html)\n- [2017 roadmap](https://cihai.git-pull.com/design-and-planning/2017/spec.html)\n- Python support: >= 3.7, pypy\n- Source: <https://github.com/cihai/cihai-cli>\n- Docs: <https://cihai-cli.git-pull.com>\n- Changelog: <https://cihai-cli.git-pull.com/history.html>\n- API: <https://cihai-cli.git-pull.com/api.html>\n- Issues: <https://github.com/cihai/cihai-cli/issues>\n- Test coverage <https://codecov.io/gh/cihai/cihai-cli>\n- pypi: <https://pypi.python.org/pypi/cihai-cli>\n- OpenHub: <https://www.openhub.net/p/cihai-cli>\n- License: MIT\n',
     'author': 'Tony Narlock',
     'author_email': 'tony@git-pull.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://cihai-cli.git-pull.com',
```

### Comparing `cihai-cli-0.9.0a0/PKG-INFO` & `cihai-cli-0.9.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cihai-cli
-Version: 0.9.0a0
+Version: 0.9.0a1
 Summary: Command line frontend for the cihai CJK language library
 Home-page: https://cihai-cli.git-pull.com
 License: MIT
+Keywords: unihan,sqlalchemy,library,cjk,unicode,dictionary,dataset,encyclopedia,chinese,japanese,korean,languages,study,cli,terminal,shell
 Author: Tony Narlock
 Author-email: tony@git-pull.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Internationalization
+Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: test
```

