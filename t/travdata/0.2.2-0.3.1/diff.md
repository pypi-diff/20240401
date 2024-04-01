# Comparing `tmp/travdata-0.2.2.tar.gz` & `tmp/travdata-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travdata-0.2.2.tar", max compression
+gzip compressed data, was "travdata-0.3.1.tar", max compression
```

## Comparing `travdata-0.2.2.tar` & `travdata-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,44 @@
--rw-r--r--   0        0        0     1095 2024-03-30 15:23:08.221284 travdata-0.2.2/LICENSE
--rw-r--r--   0        0        0     4336 2024-03-30 15:23:08.221284 travdata-0.2.2/README.rst
--rw-r--r--   0        0        0     1087 2024-03-30 15:23:08.225284 travdata-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      129 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/__init__.py
--rw-r--r--   0        0        0     2364 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/csvtoyaml.py
--rw-r--r--   0        0        0     4508 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/extractcsvtables.py
--rw-r--r--   0        0        0     2617 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/licenses.py
--rw-r--r--   0        0        0      643 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/listbooks.py
--rw-r--r--   0        0        0    21547 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/cli/cmds/tradetable.py
--rw-r--r--   0        0        0     9353 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/config.py
--rw-r--r--   0        0        0      705 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/dataclassutil.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/__init__.py
--rw-r--r--   0        0        0     3914 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/basic.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/core/__init__.py
--rw-r--r--   0        0        0      685 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/core/trade.py
--rw-r--r--   0        0        0     3156 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/core/worldcreation.py
--rw-r--r--   0        0        0      483 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/datatypes/yamlcodec.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/extraction/__init__.py
--rw-r--r--   0        0        0     2357 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/extraction/parseutil.py
--rw-r--r--   0        0        0     5248 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/extraction/pdfextract.py
--rw-r--r--   0        0        0     3194 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/extraction/tabulautil.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/py.typed
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/core/__init__.py
--rw-r--r--   0        0        0      550 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/core/registry.py
--rw-r--r--   0        0        0     2079 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/core/trade.py
--rw-r--r--   0        0        0     3802 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/core/worldcreation.py
--rw-r--r--   0        0        0     1093 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/tableconverters/registry.py
--rw-r--r--   0        0        0        0 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/travellermap/__init__.py
--rw-r--r--   0        0        0     3686 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/travellermap/apiurls.py
--rw-r--r--   0        0        0     2397 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/travellermap/sectorparse.py
--rw-r--r--   0        0        0     4879 2024-03-30 15:23:08.225284 travdata-0.2.2/src/travdata/travellermap/world.py
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 travdata-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-01 19:18:47.673696 travdata-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6682 2024-04-01 19:18:47.673696 travdata-0.3.1/README.rst
+-rw-r--r--   0        0        0     1296 2024-04-01 19:18:47.677696 travdata-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/__init__.py
+-rwxr-xr-x   0        0        0     1277 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/csvtoyaml.py
+-rw-r--r--   0        0        0     4207 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/extractcsvtables.py
+-rw-r--r--   0        0        0     2617 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/licenses.py
+-rw-r--r--   0        0        0      646 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/listbooks.py
+-rw-r--r--   0        0        0    22253 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/tradetable.py
+-rw-r--r--   0        0        0      521 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/commontext.py
+-rw-r--r--   0        0        0    10245 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/config.py
+-rw-r--r--   0        0        0      616 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/csvutil.py
+-rw-r--r--   0        0        0      705 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/dataclassutil.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/__init__.py
+-rw-r--r--   0        0        0     3914 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/basic.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/core/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/core/trade.py
+-rw-r--r--   0        0        0     3156 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/core/worldcreation.py
+-rw-r--r--   0        0        0      483 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/yamlcodec.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/__init__.py
+-rw-r--r--   0        0        0     2357 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/parseutil.py
+-rw-r--r--   0        0        0     8517 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/pdfextract.py
+-rw-r--r--   0        0        0     4006 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/tabulautil.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/__init__.py
+-rw-r--r--   0        0        0    12253 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/cfgwin.py
+-rw-r--r--   0        0        0     4804 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/runnerwin.py
+-rw-r--r--   0        0        0      862 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/gui.py
+-rw-r--r--   0        0        0      766 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/qtutil.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/py.typed
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/__init__.py
+-rw-r--r--   0        0        0      550 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/registry.py
+-rw-r--r--   0        0        0     2079 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/trade.py
+-rw-r--r--   0        0        0     3802 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/worldcreation.py
+-rw-r--r--   0        0        0     1093 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/registry.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/apiurls.py
+-rw-r--r--   0        0        0     2397 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/sectorparse.py
+-rw-r--r--   0        0        0     4879 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/world.py
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.3.1/PKG-INFO
```

### Comparing `travdata-0.2.2/LICENSE` & `travdata-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/README.rst` & `travdata-0.3.1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,37 @@
 
    Do not distribute the data extracted PDF files without explicit
    permission from the copyright holder.
 
 The purpose of this tool is to extract the data for usage by the legal
 owner of a copy of the original materal that it was extracted from.
 
+.. _`_reporting_issues`:
+
+Reporting issues
+================
+
+Report any problems you encounter or feature requests to
+https://github.com/huin/travdata/issues.
+
+Please include:
+
+-  information about which operating system you are using the program
+   on,
+
+-  steps to reproduce the problem,
+
+-  what you expected to happen,
+
+-  what actually happened.
+
+Ideally include text output of any error messages from the program,
+and/or screenshots to demonstrate the problem if text output is not
+relevant.
+
 .. _`_usage`:
 
 Usage
 =====
 
 This package is primarily intended for the provided CLI tools, but API
 access is also possible.
@@ -44,21 +67,25 @@
 
 Prebuilt
 ~~~~~~~~
 
 You can download an executable version of the application for your
 platform at
 `github.com/huin/travdata/releases <https://github.com/huin/travdata/releases>`__.
-Currently executables are only generated for Linux and Windows (as I do
-not have a MacOS device suitable for testing on).
+Currently executables are only generated for Linux and Windows, and seem
+to work on the author’s machines. A MacOS binary is also released, but
+it has not been tested.
 
 Once downloaded, extract the ``.zip`` file to a suitable location. You
 can most easily use the command line interface from the directory that
 it was unpacked to.
 
+You may also wish to make a shortcut to the ``travdata_gui`` executable,
+but it can also be run directly from the unzipped directory.
+
 .. _`_pip_install`:
 
 Pip install
 ~~~~~~~~~~~
 
 This may work on platforms that have no prebuilt executable. Assuming
 that you have Python 3.11 or later installed, and you are running
@@ -68,17 +95,72 @@
 .. code:: console
 
    mkdir travdata
    cd travdata
    python -m venv venv
    source ./venv/bin/activate
 
+You will also need to download a copy of the source code, in order to
+get a copy of the configuration. Visit
+`releases <https://github.com/huin/travdata/releases>`__, pick a recent
+release, and download the "Source code" zip file. Extract the ``config``
+directory from it, and place it in the ``travdata`` directory you
+created earlier, such that the ``travdata`` directory contains two
+subdirectories:
+
+-  ``config``
+
+-  ``venv``
+
 At this point, you can run ``python -m travdata.cli.cli`` instead of
 running ``travdata_cli`` from other examples.
 
+.. _`_gui_literal_travdata_gui_literal`:
+
+GUI ``travdata_gui``
+--------------------
+
+The GUI binary provides a user interface to aid in extracting CSV files,
+similarly to ``travdata_cli extractcsvtables``.
+
+.. figure::
+   https://raw.githubusercontent.com/huin/travdata/main/images/extraction_gui.png
+   :alt: Screenshot of extraction configuration GUI
+
+1. "Extraction configuration" selects the configuration for extraction
+   from PDFs. It should detect its own configuration automatically. If
+   it does not, click "Select configuration" and select the
+   ``_internal/config`` directory that should have come with the
+   download of the program.
+
+2. "Input PDF" selects the PDF to extract from, and the book that that
+   PDF corresponds to.
+
+   Note: only a very limited number of books are supported - at the time
+   of writing, only the Core Rulebook 2022 update.
+
+   Click "Select PDF" and choose the input PDF file.
+
+3. If selecting a PDF file did not automatically choose the correct book
+   (based on its filename), choose it from the drop-down box below
+   "Select PDF".
+
+4. "Output directory" selects a directory to write the extracted CSV
+   data into. Choose an empty directory.
+
+5. "Extract" should now be enabled. Click it to start extraction. It
+   will open a window to display progress and any errors.
+
+6. Close the extraction window once extraction is completed (and if you
+   no longer need the output).
+
+Note: the program will not extract the same table again if it sees that
+the CSV file is present in the output directory. If you wish to force
+re-extraction, delete some or all files from the output directory.
+
 .. _`_cli_literal_travdata_cli_extractcsvtables_literal`:
 
 CLI ``travdata_cli extractcsvtables``
 -------------------------------------
 
 This tool extracts CSV files from tables in the given PDF, based on the
 given configuration files that specifies the specifics of how those
@@ -86,28 +168,21 @@
 extraction of tables from known PDF files, where the individual tables
 have been configured.
 
 The general form of the command is:
 
 .. code:: shell
 
-   travdata_cli extractcsvtables -c CONFIG_DIR BOOK_NAME INPUT.PDF OUT_DIR
+   travdata_cli extractcsvtables BOOK_NAME INPUT.PDF OUT_DIR
 
 Where:
 
-``CONFIG_DIR``
-   is the path to the directory containing a ``config.yaml`` file, and
-   subdirectories and ``*.tabula-template.json`` files. This contains
-   information guiding the extraction, and is specific to the PDF being
-   read from. These configurations are provided with the source code to
-   this program in the directories under the ``config`` directory.
-
 ``BOOK_NAME``
    is the identifier for the book to extract tables from. This selects
-   the correct book’s configuration from the ``CONFIG_DIR``. Use
+   the correct book’s configuration from the files that . Use
    ``travdata_cli listbooks`` to list accepted values for this argument.
 
 ``INPUT.PDF``
    is the path to the PDF file to read tables from.
 
 ``OUT_DIR``
    is the path to a (potentially not existing) directory to output the
@@ -119,15 +194,15 @@
 Traveller Core Rulebook 2022, and not all tables are yet supported for
 extraction.
 
 Example:
 
 .. code:: shell
 
-   travdata_cli extractcsvtables -c path/to/config \
+   travdata_cli extractcsvtables \
        core_rulebook_2022 path/to/update_2022_core_rulebook.pdf \
        path_to_output_dir
 
 .. _`_developing`:
 
 Developing
 ==========
```

### Comparing `travdata-0.2.2/pyproject.toml` & `travdata-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travdata"
-version = "0.2.2"
+version = "0.3.1"
 description = "Data utility code for Mongoose Traveller TTRPG."
 authors = ["John Beisley <johnbeisleyuk@gmail.com>"]
 keywords = ["traveller", "ttrpg"]
 license = "MIT"
 readme = "README.rst"  # rebuilt from README.adoc
 repository = "https://github.com/huin/travdata"
 packages = [
@@ -12,14 +12,15 @@
 ]
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/huin/travdata/issues"
 
 [tool.poetry.scripts]
 travdata_cli = "travdata.cli.cli:main"
+travdata_gui = "travdata.gui.gui:main"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 mypy = "^1.9.0"
 pylint = "^3.1.0"
 pytest = "^8.0.2"
 testfixtures = "^8.0.0"
@@ -30,16 +31,23 @@
 version = "^6.5.0"
 python = ">=3.11,<3.13"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry.dependencies]
+jpype1 = "^1.5.0"
 pip-licenses-lib = "^0.2.1"
 progress = "^1.6"
 python = "^3.11"
 tabula-py = {extras = ["jpype"], version = "^2.9.0"}
 ruamel-yaml = "^0.18.6"
+pyside6-essentials = {version = "^6.6.3", python = ">=3.11,<3.13"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+exclude = '''(?x)(
+    travdata/gui/.*  # QtCore.pyi syntax error.
+)'''
```

### Comparing `travdata-0.2.2/src/travdata/cli/cmds/csvtoyaml.py` & `travdata-0.3.1/src/travdata/cli/cmds/csvtoyaml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 Converts CSV data tables from the Mongoose Traveller 2022 core rules PDF into
 YAML files.
-
-The extracted data is *not* for redistribution, as it is almost certainly
-subject to copyright. This utility (and its output) is intended as an aid to
-those who legally own a copy of the Mongoose Traveller materials, and wish to
-make use of the data for their own purposes.
-
-It is the sole responsibility of the user of this program to use the extracted
-data in a manner that respects the publisher's IP rights.
 """
 
 import argparse
 import csv
 import pathlib
 
+from travdata import csvutil
 from travdata.datatypes import yamlcodec
 from travdata.tableconverters.core import registry
 
 
 def add_subparser(subparsers) -> None:
     """Adds a subcommand parser to ``subparsers``."""
     argparser: argparse.ArgumentParser = subparsers.add_parser(
@@ -51,18 +44,16 @@
     created_directories: set[pathlib.Path] = set()
     for conv_key, conv_fn in registry.CONVERTERS.converters.items():
         in_group_dir = args.input_dir / conv_key.group_name
         out_group_dir = args.output_dir / conv_key.group_name
         if out_group_dir not in created_directories:
             out_group_dir.mkdir(parents=True, exist_ok=True)
         with (
-            open(
+            csvutil.open_read(
                 in_group_dir / f"{conv_key.table_name}.csv",
-                "rt",
-                encoding="utf-8",
             ) as csv_file_in,
             open(
                 out_group_dir / f"{conv_key.table_name}.yaml",
                 "wt",
                 encoding="utf-8",
             ) as yaml_file_out,
         ):
```

### Comparing `travdata-0.2.2/src/travdata/cli/cmds/extractcsvtables.py` & `travdata-0.3.1/src/travdata/cli/cmds/extractcsvtables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Extracts data tables from the Mongoose Traveller 2022 core rules PDF as
 CSV files.
 """
 
 import argparse
-import csv
+import contextlib
 import pathlib
 import sys
 import textwrap
-from typing import cast
+from typing import Callable, Iterator
 
 from progress import bar as progress  # type: ignore[import-untyped]
 from travdata import config
 from travdata.extraction import pdfextract, tabulautil
 
 
 def add_subparser(subparsers) -> None:
@@ -81,70 +81,67 @@
             """
         ),
         action="store_true",
         default=False,
     )
 
 
+@contextlib.contextmanager
+def _progress_reporter(no_progress: bool) -> Iterator[Callable[[pdfextract.Progress], None]]:
+    if no_progress:
+        progress_bar = None
+
+        def on_progress(p: pdfextract.Progress) -> None:
+            del p  # unused
+
+    else:
+        progress_bar = progress.Bar("Extracting tables")
+        progress_bar.start()
+
+        def on_progress(p: pdfextract.Progress) -> None:
+            progress_bar.index = p.completed
+            progress_bar.max = p.total
+            progress_bar.update()
+
+    try:
+        yield on_progress
+    finally:
+        if progress_bar is not None:
+            progress_bar.finish()
+
+
 def run(args: argparse.Namespace) -> int:
     """CLI entry point."""
 
-    tabula_client = tabulautil.TabulaClient(
-        force_subprocess=args.tabula_force_subprocess,
-    )
-
     cfg = config.load_config_from_flag(args, [args.book_name])
     try:
         book_cfg = cfg.books[args.book_name]
     except KeyError:
         print(f"Book {args.book_name} is unknown.", file=sys.stderr)
         return 1
+    if book_cfg.group is None:
+        raise RuntimeError("book_cfg.group should have been loaded, but is None")
 
-    output_tables: list[tuple[pathlib.Path, config.Table]] = []
-    for table in book_cfg.all_tables():
-        if table.extraction is None:
-            continue
-        out_filepath = args.output_dir / table.file_stem.with_suffix(".csv")
-
-        if args.overwrite_existing or not out_filepath.exists():
-            output_tables.append((out_filepath, table))
-
-    if not args.no_progress:
-        monitored_output_tables = progress.Bar(
-            "Extracting tables",
-            max=len(output_tables),
-        ).iter(output_tables)
-    else:
-        monitored_output_tables = iter(output_tables)
+    def on_error(error: str) -> None:
+        print(error, file=sys.stderr)
 
-    created_directories: set[pathlib.Path] = set()
-    for out_filepath, table in monitored_output_tables:
-        if table.extraction is None:
-            continue
-        extraction = table.extraction
-
-        out_filepath = cast(pathlib.Path, out_filepath)
-        table = cast(config.Table, table)
-
-        group_dir = out_filepath.parent
-        if group_dir not in created_directories:
-            group_dir.mkdir(parents=True, exist_ok=True)
-            created_directories.add(group_dir)
-
-        try:
-            try:
-                rows = pdfextract.extract_table(
-                    config_dir=args.config_dir,
-                    pdf_path=args.input_pdf,
-                    file_stem=table.file_stem,
-                    extraction=extraction,
-                    table_reader=tabula_client,
-                )
-                with open(out_filepath, "wt", encoding="utf-8") as f:
-                    csv.writer(f).writerows(rows)
-            except Exception as e:
-                e.add_note(f"Error while processing table {table.file_stem}: {e}")
-                raise
-        except pdfextract.ConfigurationError as e:
-            print(e, file=sys.stderr)
+    with (
+        tabulautil.TabulaClient(force_subprocess=args.tabula_force_subprocess) as tabula_client,
+        _progress_reporter(args.no_progress) as on_progress,
+    ):
+        pdfextract.extract_book(
+            table_reader=tabula_client,
+            cfg=pdfextract.ExtractionConfig(
+                config_dir=args.config_dir,
+                output_dir=args.output_dir,
+                input_pdf=args.input_pdf,
+                book_cfg=book_cfg,
+                overwrite_existing=args.overwrite_existing,
+            ),
+            events=pdfextract.ExtractEvents(
+                on_progress=on_progress,
+                on_error=on_error,
+                do_continue=lambda: True,
+            ),
+        )
 
     return 0
```

### Comparing `travdata-0.2.2/src/travdata/cli/cmds/licenses.py` & `travdata-0.3.1/src/travdata/cli/cmds/licenses.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/cli/cmds/listbooks.py` & `travdata-0.3.1/src/travdata/cli/cmds/listbooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     argparser.set_defaults(run=run)
 
 
 def run(args: argparse.Namespace) -> None:
     """CLI entry point."""
 
     cfg = config.load_config_from_flag(args, [])
-    for name in cfg.book_names:
+    for name in sorted(cfg.books):
         print(name)
```

### Comparing `travdata-0.2.2/src/travdata/cli/cmds/tradetable.py` & `travdata-0.3.1/src/travdata/cli/cmds/tradetable.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Optional,
     Protocol,
     TypeAlias,
     TypeVar,
     cast,
 )
 
+from travdata import csvutil
 from travdata.datatypes import yamlcodec
 from travdata.datatypes.core import trade, worldcreation
 from travdata.extraction import parseutil
 from travdata.travellermap import apiurls, sectorparse, world
 
 T = TypeVar("T")
 # Maps from TradeGood.d66 to the lowest law level at which that good is illegal.
@@ -86,15 +87,15 @@
     - "Name" - the name of the world.
     - "UWP" - the UWP code.
     - "Trade Codes" - a colon (":") delimited list of two-letter trade codes.
 
     :param fp: File to read CSV data from.
     :yield: World data.
     """
-    with open(path, "rt", encoding="utf-8") as fp:
+    with csvutil.open_read(pathlib.Path(path)) as fp:
         r = csv.DictReader(fp)
         for row in r:
             yield world.World(
                 name=row["Name"],
                 location=world.WorldLocation(
                     subsector_hex=world.SubSectorLoc.parse(row["Location"]),
                 ),
@@ -146,25 +147,26 @@
     if v == "true":
         return True
     if v == "false":
         return False
     raise ValueError(v)
 
 
-def _load_world_trade_overrides(fp: io.TextIOBase) -> WorldTradeOverridesMap:
-    r = csv.DictReader(fp)
+def _load_world_trade_overrides(path: pathlib.Path) -> WorldTradeOverridesMap:
     result: WorldTradeOverridesMap = {}
-    for row in r:
-        key = row["Location"], row["D66"]
-        result[key] = WorldTradeOverrides(
-            available=parseutil.map_opt_dict_key(_pbool, row, "Available"),
-            purchase_dm=parseutil.map_opt_dict_key(int, row, "Purchase DM"),
-            sale_dm=parseutil.map_opt_dict_key(int, row, "Sale DM"),
-            illegal=parseutil.map_opt_dict_key(_pbool, row, "Illegal"),
-        )
+    with csvutil.open_read(path) as fp:
+        r = csv.DictReader(fp)
+        for row in r:
+            key = row["Location"], row["D66"]
+            result[key] = WorldTradeOverrides(
+                available=parseutil.map_opt_dict_key(_pbool, row, "Available"),
+                purchase_dm=parseutil.map_opt_dict_key(int, row, "Purchase DM"),
+                sale_dm=parseutil.map_opt_dict_key(int, row, "Sale DM"),
+                illegal=parseutil.map_opt_dict_key(_pbool, row, "Illegal"),
+            )
     return result
 
 
 def _trade_dm(dms: dict[str, int], world_trades: set[str]) -> int:
     return max(
         (dms[wt] for wt in world_trades if wt in dms),
         default=0,
@@ -203,15 +205,15 @@
         "--world-trade-overrides",
         help=textwrap.dedent(
             """
             File containing trade overrides for the worlds. CSV file with
             columns: Location,D66,Available,Purchase DM,Sale DM,Illegal
             """
         ),
-        type=argparse.FileType("rt"),
+        type=pathlib.Path,
         metavar="world-trade-overrides.csv",
     )
     data_inputs_grp.add_argument(
         "world_data",
         help=textwrap.dedent(
             """
             World data within a single subsector. The meaning and interpretation
@@ -270,14 +272,21 @@
         "--output-format",
         help="""Format of the output trading sheet.""",
         choices=_RESULT_WRITERS.keys(),
         metavar="FORMAT",
     )
 
     argparser.add_argument(
+        "output_path",
+        help="Path to the file to write.",
+        type=pathlib.Path,
+        metavar="FILE",
+    )
+
+    argparser.add_argument(
         "--ignore-unknowns",
         help="""Ignore unknown trade codes.""",
         choices=sorted(_IgnoreUnknown),
         action="append",
     )
 
     inc_grp = argparser.add_argument_group("Extra information to include")
@@ -510,140 +519,142 @@
         return [(fmt.format(example_dm), explanation) for fmt, explanation in entries]
 
 
 class _ResultWriter(Protocol):  # pylint: disable=too-few-public-methods
     def __call__(
         self,
         *,
-        fp: io.TextIOBase,
+        output_path: pathlib.Path,
         world_views: list[_WorldView],
         tgood_results: list[_ResultTradeGoodDMs],
         opts: _OutputOpts,
     ) -> None: ...
 
 
 def _write_results_asciidoc(
     *,
-    fp: io.TextIOBase,
+    output_path: pathlib.Path,
     world_views: list[_WorldView],
     tgood_results: list[_ResultTradeGoodDMs],
     opts: _OutputOpts,
 ) -> None:
-    def writeln(s: str = "") -> None:
-        print(s, file=fp)
+    with open(output_path, "wt", encoding="utf-8") as fp:
 
-    def writecell(s: str, duplication: int = 1, operators: str = "") -> None:
-        if duplication == 1:
-            print(f"{operators}|{s}", file=fp)
-        else:
-            print(f"{duplication}*{operators}|{s}", file=fp)
+        def writeln(s: str = "") -> None:
+            print(s, file=fp)
 
-    writeln("= Trading DM Table")
-    writeln()
+        def writecell(s: str, duplication: int = 1, operators: str = "") -> None:
+            if duplication == 1:
+                print(f"{operators}|{s}", file=fp)
+            else:
+                print(f"{duplication}*{operators}|{s}", file=fp)
 
-    col_specs = ["1", "4", "2", "3", f"{len(world_views)}*1"]
-    writeln(f"[cols=\"{','.join(col_specs)}\"]")
-    writeln("|===")  # Start of table content.
-    writeln(
-        "|"
-        + " |".join(
-            [
-                "D66",
-                "Goods",
-                "Tons",
-                "Base Price (cr)",
-            ]
-            + [world_view.subsector_loc for world_view in world_views]
-        )
-    )
+        writeln("= Trading DM Table")
+        writeln()
 
-    for tgood_result in tgood_results:
-        writeln()  # Start of new row.
-        tgood = tgood_result.tgood
-        writecell(tgood.d66)
-        writecell(tgood.name)
-
-        if tprops := tgood_result.tgood.properties:
-            writecell(tprops.tons)
-            writecell(str(tprops.base_price))
-        else:
-            writecell("", duplication=2)
+        col_specs = ["1", "4", "2", "3", f"{len(world_views)}*1"]
+        writeln(f"[cols=\"{','.join(col_specs)}\"]")
+        writeln("|===")  # Start of table content.
+        writeln(
+            "|"
+            + " |".join(
+                [
+                    "D66",
+                    "Goods",
+                    "Tons",
+                    "Base Price (cr)",
+                ]
+                + [world_view.subsector_loc for world_view in world_views]
+            )
+        )
 
-        if not tgood_result.dms:
-            writecell("", duplication=len(world_views))
-            continue
+        for tgood_result in tgood_results:
+            writeln()  # Start of new row.
+            writecell(tgood_result.tgood.d66)
+            writecell(tgood_result.tgood.name)
+
+            if tprops := tgood_result.tgood.properties:
+                writecell(tprops.tons)
+                writecell(str(tprops.base_price))
+            else:
+                writecell("", duplication=2)
 
-        for world_view in world_views:
-            world_dm = tgood_result.dms.get(world_view.id)
-            if not world_dm:
-                writecell("")
+            if not tgood_result.dms:
+                writecell("", duplication=len(world_views))
                 continue
-            writecell(opts.formats.fmt_dm(world_dm), operators="m")
 
-    writeln("|===")  # End of table content.
-
-    if opts.include_key:
-        writeln()
-        writeln("== Key")
-        for key_item, explanation in opts.formats.key("+2"):
-            writeln(f"{explanation}:: `{key_item}`")
-
-    if opts.include_explanation:
-        writeln()
-        writeln("== How to use")
-        for s in _DM_EXPLANATION_SENTENCES:
-            writeln(f"- {s}")
+            for world_view in world_views:
+                world_dm = tgood_result.dms.get(world_view.id)
+                if not world_dm:
+                    writecell("")
+                    continue
+                writecell(opts.formats.fmt_dm(world_dm), operators="m")
+
+        writeln("|===")  # End of table content.
+
+        if opts.include_key:
+            writeln()
+            writeln("== Key")
+            for key_item, explanation in opts.formats.key("+2"):
+                writeln(f"{explanation}:: `{key_item}`")
+
+        if opts.include_explanation:
+            writeln()
+            writeln("== How to use")
+            for s in _DM_EXPLANATION_SENTENCES:
+                writeln(f"- {s}")
 
 
 def _write_results_csv(
     *,
-    fp: io.TextIOBase,
+    output_path: pathlib.Path,
     world_views: list[_WorldView],
     tgood_results: list[_ResultTradeGoodDMs],
     opts: _OutputOpts,
 ) -> None:
-    csv_writer = csv.writer(fp)
-    if opts.include_headers:
-        csv_writer.writerow(
-            ["D66", "Goods", "Tons", "Base Price (cr)"] + [w.subsector_loc for w in world_views]
-        )
-
-    for tgood_result in tgood_results:
-        tgood = tgood_result.tgood
-        row = [tgood.d66, tgood.name]
-
-        if tprops := tgood_result.tgood.properties:
-            row.append(tprops.tons)
-            row.append(str(tprops.base_price))
-        else:
-            row.extend(["", ""])
+    with csvutil.open_write(output_path) as fp:
+        csv_writer = csv.writer(fp)
+        if opts.include_headers:
+            csv_writer.writerow(
+                ["D66", "Goods", "Tons", "Base Price (cr)"] + [w.subsector_loc for w in world_views]
+            )
 
-        if not tgood_result.dms:
-            csv_writer.writerow(row)
-            continue
+        for tgood_result in tgood_results:
+            tgood = tgood_result.tgood
+            row = [tgood.d66, tgood.name]
+
+            if tprops := tgood_result.tgood.properties:
+                row.append(tprops.tons)
+                row.append(str(tprops.base_price))
+            else:
+                row.extend(["", ""])
 
-        for world_view in world_views:
-            world_dm = tgood_result.dms.get(world_view.id)
-            if not world_dm:
-                row.append("")
+            if not tgood_result.dms:
+                csv_writer.writerow(row)
                 continue
-            row.append(opts.formats.fmt_dm(world_dm))
 
-        csv_writer.writerow(row)
+            for world_view in world_views:
+                world_dm = tgood_result.dms.get(world_view.id)
+                if not world_dm:
+                    row.append("")
+                    continue
+                row.append(opts.formats.fmt_dm(world_dm))
+
+            csv_writer.writerow(row)
 
-    if opts.include_key:
-        csv_writer.writerow([])
-        csv_writer.writerow(["Key:"])
-        for key_item, explanation in opts.formats.key("+2"):
-            csv_writer.writerow([key_item, explanation])
-
-    if opts.include_explanation:
-        csv_writer.writerow([])
-        for s in _DM_EXPLANATION_SENTENCES:
-            csv_writer.writerow([s])
+        if opts.include_key:
+            csv_writer.writerow([])
+            csv_writer.writerow(["Key:"])
+            for key_item, explanation in opts.formats.key("+2"):
+                csv_writer.writerow([key_item, explanation])
+
+        if opts.include_explanation:
+            csv_writer.writerow([])
+            for s in _DM_EXPLANATION_SENTENCES:
+                csv_writer.writerow([s])
 
 
 _RESULT_WRITERS: dict[str, _ResultWriter] = {
     "asciidoc": _write_results_asciidoc,
     "csv": _write_results_csv,
 }
 
@@ -682,15 +693,15 @@
             world_views=world_views,
             wt_overrides=wt_overrides,
         )
     )
 
     result_writer = _RESULT_WRITERS[args.output_format]
     result_writer(
-        fp=cast(io.TextIOBase, sys.stdout),
+        output_path=args.output_path,
         tgood_results=tgood_results,
         world_views=world_views,
         opts=_OutputOpts(
             include_headers=args.include_headers,
             formats=_Formats(
                 common=args.format_common,
                 unavailable=args.format_unavailable,
```

### Comparing `travdata-0.2.2/src/travdata/config.py` & `travdata-0.3.1/src/travdata/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,20 +117,29 @@
         """
         yield from self.tables.values()
         for group in self.groups.values():
             yield from group.all_tables()
 
 
 @dataclasses.dataclass
+class Book(YamlDataclassMixin):
+    """Top level information about a book."""
+
+    id_: str
+    name: str
+    default_filename: str
+    group: Optional[Group] = None
+
+
+@dataclasses.dataclass
 class Config:
     """Top-level configuration."""
 
     directory: pathlib.Path
-    books: dict[str, Group] = dataclasses.field(default_factory=dict)
-    book_names: list[str] = dataclasses.field(default_factory=list)
+    books: dict[str, Book] = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
 @_YAML.register_class
 class _YamlTable(YamlDataclassMixin):
     yaml_tag: ClassVar = "!Table"
     type: Optional[str] = None
@@ -175,54 +184,80 @@
             # anchoring and aliasing by the YAML file author at the time of YAML
             # parsing.
         )
 
 
 @dataclasses.dataclass
 @_YAML.register_class
+class _YamlBook(YamlDataclassMixin):
+    yaml_tag: ClassVar = "!Book"
+    name: str
+    default_filename: str
+
+    def prepare(
+        self,
+        cfg_dir: pathlib.Path,
+        book_id: str,
+        limit_books: list[str],
+    ) -> Book:
+        """Creates a ``Book`` from self.
+
+        :param cfg_dir: Path to the directory of the ``Config``.
+        :param book_id: ID of the book within the parent _YamlConfig.
+        :param limit_books: Allowlist of book names to load configuration for.
+        :return: Prepared ``Book``.
+        """
+        book = Book(
+            id_=book_id,
+            name=self.name,
+            default_filename=self.default_filename,
+        )
+        if book_id in limit_books:
+            rel_book_dir = pathlib.Path(book_id)
+            cfg = _YAML.load(cfg_dir / rel_book_dir / "book.yaml")
+            book.group = _prepare_group(cfg, rel_book_dir)
+        return book
+
+
+@dataclasses.dataclass
+@_YAML.register_class
 class _YamlConfig(YamlDataclassMixin):
     yaml_tag: ClassVar = "!Config"
-    books: list[str] = dataclasses.field(default_factory=list)
+    books: dict[str, _YamlBook]
 
     def prepare(self, cfg_dir: pathlib.Path, limit_books: list[str]) -> Config:
         """Creates a ``Group`` from self.
 
         :param cfg_dir: Path to the directory of the ``Config``.
         :param limit_books: Allowlist of book names to load configuration for.
         :return: Prepared ``Config``.
         """
-        books: dict[str, Group] = {}
-        for book_name in limit_books:
-            if book_name not in self.books:
-                raise UserError(f"book {book_name!r} does not exist")
-            book_dir = pathlib.Path(book_name)
-            books[book_name] = _load_book_config(cfg_dir, book_dir)
+        books: dict[str, Book] = {}
+        for book_id, yaml_book in self.books.items():
+            books[book_id] = yaml_book.prepare(
+                cfg_dir=cfg_dir,
+                book_id=book_id,
+                limit_books=limit_books,
+            )
         return Config(
             directory=cfg_dir,
             books=books,
-            book_names=self.books,
         )
 
 
-def _prepare_book_config(cfg: Any, rel_book_dir: pathlib.Path) -> Group:
+def _prepare_group(cfg: Any, rel_book_dir: pathlib.Path) -> Group:
     if not isinstance(cfg, _YamlGroup):
         raise TypeError(cfg)
     return cfg.prepare(rel_book_dir)
 
 
-def load_book_config_from_str(yaml_str: str) -> Group:
+def load_group_from_str(yaml_str: str) -> Group:
     """Loads the configuration from the given string containing YAML."""
     cfg = _YAML.load(yaml_str)
-    return _prepare_book_config(cfg, pathlib.Path("."))
-
-
-def _load_book_config(cfg_dir: pathlib.Path, rel_book_dir: pathlib.Path) -> Group:
-    """Loads the configuration from the directory."""
-    cfg = _YAML.load(cfg_dir / rel_book_dir / "book.yaml")
-    return _prepare_book_config(cfg, rel_book_dir)
+    return _prepare_group(cfg, pathlib.Path("."))
 
 
 def _prepare_config(cfg: Any, cfg_dir: pathlib.Path, limit_books: list[str]) -> Config:
     if not isinstance(cfg, _YamlConfig):
         raise TypeError(cfg)
     return cfg.prepare(cfg_dir, limit_books)
 
@@ -232,15 +267,15 @@
     cfg = _YAML.load(cfg_dir / "config.yaml")
     return _prepare_config(cfg=cfg, cfg_dir=cfg_dir, limit_books=limit_books)
 
 
 def add_config_flag(argparser: argparse.ArgumentParser) -> None:
     """Adds the flag required to call ``load_config_from_flag`` on the parsed args."""
 
-    default_config_dir = _get_default_config_path()
+    default_config_dir = get_default_config_path()
 
     argparser.add_argument(
         "--config-dir",
         "-c",
         help=textwrap.dedent(
             """
             Path to the configuration directory. This must contain a config.yaml
@@ -251,15 +286,20 @@
         type=pathlib.Path,
         metavar="CONFIG_DIR",
         required=default_config_dir is None,
         default=default_config_dir,
     )
 
 
-def _get_default_config_path() -> Optional[pathlib.Path]:
+def get_default_config_path() -> Optional[pathlib.Path]:
+    """Returns the default path to the config directory.
+
+    :raises RuntimeError: If the environment is not recognised.
+    :return: Default path to the config directory, if known.
+    """
     match __executable_environment__:
         case "development":
             install_dir = _data_dir_for_development()
         case "pyinstaller":
             install_dir = _data_dir_for_pyinstaller()
         case unknown_env:
             raise RuntimeError(f"unknown executable environment {unknown_env!r}")
```

### Comparing `travdata-0.2.2/src/travdata/dataclassutil.py` & `travdata-0.3.1/src/travdata/dataclassutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/datatypes/basic.py` & `travdata-0.3.1/src/travdata/datatypes/basic.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/datatypes/core/trade.py` & `travdata-0.3.1/src/travdata/datatypes/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/datatypes/core/worldcreation.py` & `travdata-0.3.1/src/travdata/datatypes/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/extraction/parseutil.py` & `travdata-0.3.1/src/travdata/extraction/parseutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/tableconverters/core/registry.py` & `travdata-0.3.1/src/travdata/tableconverters/core/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/tableconverters/core/trade.py` & `travdata-0.3.1/src/travdata/tableconverters/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/tableconverters/core/worldcreation.py` & `travdata-0.3.1/src/travdata/tableconverters/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/tableconverters/registry.py` & `travdata-0.3.1/src/travdata/tableconverters/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/travellermap/apiurls.py` & `travdata-0.3.1/src/travdata/travellermap/apiurls.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/travellermap/sectorparse.py` & `travdata-0.3.1/src/travdata/travellermap/sectorparse.py`

 * *Files identical despite different names*

### Comparing `travdata-0.2.2/src/travdata/travellermap/world.py` & `travdata-0.3.1/src/travdata/travellermap/world.py`

 * *Files identical despite different names*

