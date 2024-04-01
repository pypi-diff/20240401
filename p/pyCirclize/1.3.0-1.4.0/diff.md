# Comparing `tmp/pycirclize-1.3.0.tar.gz` & `tmp/pycirclize-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-1.3.0.tar", max compression
+gzip compressed data, was "pycirclize-1.4.0.tar", max compression
```

## Comparing `pycirclize-1.3.0.tar` & `pycirclize-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1062 2024-02-18 12:11:31.867125 pycirclize-1.3.0/LICENSE
--rw-r--r--   0        0        0     8417 2024-02-18 12:11:31.867125 pycirclize-1.3.0/README.md
--rw-r--r--   0        0        0     2061 2024-02-18 12:11:32.007124 pycirclize-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    38098 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/circos.py
--rw-r--r--   0        0        0     3078 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/config.py
--rw-r--r--   0        0        0      307 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    18483 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    17735 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     8157 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0     5324 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/parser/table.py
--rw-r--r--   0        0        0    16391 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/patches.py
--rw-r--r--   0        0        0    16891 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/sector.py
--rw-r--r--   0        0        0    52111 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/track.py
--rw-r--r--   0        0        0    25330 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/tree.py
--rw-r--r--   0        0        0      533 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     7829 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     9955 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/example_data/images/python_logo.png
--rw-r--r--   0        0        0      565 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
--rw-r--r--   0        0        0     7112 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/large_example.nwk
--rw-r--r--   0        0        0      778 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
--rw-r--r--   0        0        0      227 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/small_example.nwk
--rw-r--r--   0        0        0     3870 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     2314 2024-02-18 12:11:32.007124 pycirclize-1.3.0/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0        0 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1941 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     2839 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     2004 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/parser/test_gff.py
--rw-r--r--   0        0        0     4351 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     2883 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/parser/test_table.py
--rw-r--r--   0        0        0     2765 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/test_circos.py
--rw-r--r--   0        0        0    24896 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/test_plot.py
--rw-r--r--   0        0        0     2887 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/test_sector.py
--rw-r--r--   0        0        0      988 2024-02-18 12:11:32.007124 pycirclize-1.3.0/tests/test_track.py
--rw-r--r--   0        0        0      755 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0   580710 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
--rw-r--r--   0        0        0    58530 2024-02-18 12:11:32.011124 pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
--rw-r--r--   0        0        0    57946 2024-02-18 12:11:32.015124 pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz
--rw-r--r--   0        0        0        0 2024-02-18 12:11:32.015124 pycirclize-1.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1851 2024-02-18 12:11:32.015124 pycirclize-1.3.0/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2024-02-18 12:11:32.015124 pycirclize-1.3.0/tests/utils/test_helper.py
--rw-r--r--   0        0        0     9428 1970-01-01 00:00:00.000000 pycirclize-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-01 13:00:56.095008 pycirclize-1.4.0/LICENSE
+-rw-r--r--   0        0        0     9304 2024-04-01 13:00:56.095008 pycirclize-1.4.0/README.md
+-rw-r--r--   0        0        0     2088 2024-04-01 13:00:56.239009 pycirclize-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    45398 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     3078 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/config.py
+-rw-r--r--   0        0        0      337 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    15407 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    17077 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     8157 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0     6182 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/parser/table.py
+-rw-r--r--   0        0        0    16391 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    16891 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    52377 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/track.py
+-rw-r--r--   0        0        0    25330 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/tree.py
+-rw-r--r--   0        0        0      533 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     7829 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     9955 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/images/python_logo.png
+-rw-r--r--   0        0        0      565 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
+-rw-r--r--   0        0        0     7112 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/large_example.nwk
+-rw-r--r--   0        0        0      778 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
+-rw-r--r--   0        0        0      227 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/small_example.nwk
+-rw-r--r--   0        0        0     3870 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     2314 2024-04-01 13:00:56.239009 pycirclize-1.4.0/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2601 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:56.239009 pycirclize-1.4.0/tests/parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     1827 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     4351 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_matrix.py
+-rw-r--r--   0        0        0     3700 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/parser/test_table.py
+-rw-r--r--   0        0        0     2765 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_circos.py
+-rw-r--r--   0        0        0    25147 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_plot.py
+-rw-r--r--   0        0        0     2887 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_sector.py
+-rw-r--r--   0        0        0      988 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/test_track.py
+-rw-r--r--   0        0        0      755 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
+-rw-r--r--   0        0        0    30808 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
+-rw-r--r--   0        0        0   283582 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
+-rw-r--r--   0        0        0   148834 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
+-rw-r--r--   0        0        0    36204 2024-04-01 13:00:56.243008 pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff
+-rw-r--r--   0        0        0   580710 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
+-rw-r--r--   0        0        0    58530 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
+-rw-r--r--   0        0        0    57946 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/test_dataset.py
+-rw-r--r--   0        0        0     1839 2024-04-01 13:00:56.247008 pycirclize-1.4.0/tests/utils/test_helper.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pycirclize-1.4.0/PKG-INFO
```

### Comparing `pycirclize-1.3.0/LICENSE` & `pycirclize-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/README.md` & `pycirclize-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ## API Usage
 
 API usage is described in each of the following sections in the [document](https://moshi4.github.io/pyCirclize/).
 
 - [Getting Started](https://moshi4.github.io/pyCirclize/getting_started/)
 - [Plot API Example](https://moshi4.github.io/pyCirclize/plot_api_example/)
 - [Chord Diagram](https://moshi4.github.io/pyCirclize/chord_diagram/)
+- [Radar Chart](https://moshi4.github.io/pyCirclize/radar_chart/)
 - [Circos Plot (Genomics)](https://moshi4.github.io/pyCirclize/circos_plot/)
 - [Phylogenetic Tree](https://moshi4.github.io/pyCirclize/phylogenetic_tree/)
 - [Plot Tips](https://moshi4.github.io/pyCirclize/plot_tips/)
 
 ## Code Example
 
 ### 1. Circos Plot
@@ -121,16 +122,16 @@
 r_cds_track = sector.add_track((90, 95))
 r_cds_feats = gbk.extract_features("CDS", target_strand=-1)
 r_cds_track.genomic_features(r_cds_feats, plotstyle="arrow", fc="skyblue", lw=0.5)
 
 # Plot 'gene' qualifier label if exists
 labels, label_pos_list = [], []
 for feat in gbk.extract_features("CDS"):
-    start = int(str(feat.location.start))
-    end = int(str(feat.location.end))
+    start = int(feat.location.start)
+    end = int(feat.location.end)
     label_pos = (start + end) / 2
     gene_name = feat.qualifiers.get("gene", [None])[0]
     if gene_name is not None:
         labels.append(gene_name)
         label_pos_list.append(label_pos)
 f_cds_track.xticks(label_pos_list, labels, label_size=6, label_orientation="vertical")
 
@@ -219,20 +220,54 @@
     bbox_to_anchor=(0.5, 0.5),
 )
 fig.savefig("example04.png")
 ```
 
 ![example04.png](https://raw.githubusercontent.com/moshi4/pyCirclize/main/docs/images/example04.png)  
 
+### 5. Radar Chart
+
+```python
+from pycirclize import Circos
+import pandas as pd
+
+# Create RPG jobs parameter dataframe (3 jobs, 7 parameters)
+df = pd.DataFrame(
+    data=[
+        [80, 80, 80, 80, 80, 80, 80],
+        [90, 20, 95, 95, 30, 30, 80],
+        [60, 90, 20, 20, 100, 90, 50],
+    ],
+    index=["Hero", "Warrior", "Wizard"],
+    columns=["HP", "MP", "ATK", "DEF", "SP.ATK", "SP.DEF", "SPD"],
+)
+
+# Initialize Circos instance for radar chart plot
+circos = Circos.radar_chart(
+    df,
+    vmax=100,
+    marker_size=6,
+    grid_interval_ratio=0.2,
+)
+
+# Plot figure & set legend on upper right
+fig = circos.plotfig()
+_ = circos.ax.legend(loc="upper right", fontsize=10)
+fig.savefig("example05.png")
+```
+
+![example05.png](https://raw.githubusercontent.com/moshi4/pyCirclize/main/docs/images/example05.png)  
+
 ## Not Implemented Features
 
 List of features implemented in other Circos plotting tools but not yet implemented in pyCirclize.
 I may implement them when I feel like it.
 
 - Plot histogram
 - Plot boxplot
 - Plot violin
-- Label position auto adjustment
+- Plot curved text
+- Adjust overlap label position
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=moshi4/pyCirclize&type=Date)](https://star-history.com/#moshi4/pyCirclize&Date)
```

### Comparing `pycirclize-1.3.0/pyproject.toml` & `pycirclize-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyCirclize"
-version = "1.3.0"
+version = "1.4.0"
 description = "Circular visualization in Python"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyCirclize/"
 repository = "https://github.com/moshi4/pyCirclize/"
 readme = "README.md"
 keywords = [
@@ -19,15 +19,15 @@
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Framework :: Matplotlib",
 ]
 include = ["tests"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--cov=src --tb=line --cov-report=xml --cov-report=term"
+addopts = "--cov=src --tb=long -vv --cov-report=xml --cov-report=term"
 testpaths = ["tests"]
 
 [tool.ruff]
 src = ["src", "tests"]
 line-length = 88
 
 # Lint Rules: https://docs.astral.sh/ruff/rules/
@@ -53,20 +53,21 @@
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 matplotlib = ">=3.5.2"
-biopython = ">=1.79"
+biopython = ">=1.80"
 numpy = ">=1.21.1"
 pandas = ">=1.3.5"
 
 [tool.poetry.group.dev.dependencies]
 ruff = ">=0.1.6"
+pre-commit = ">=3.5.0"
 pytest = ">=7.1.2"
 pytest-cov = ">=4.0.0"
 ipykernel = ">=6.13.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = ">=1.2"
 mkdocstrings = { extras = ["python"], version = ">=0.19.0" }
```

### Comparing `pycirclize-1.3.0/src/pycirclize/circos.py` & `pycirclize-1.4.0/src/pycirclize/circos.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from collections import defaultdict
 from collections.abc import Mapping
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable
 
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 from Bio.Phylo.BaseTree import Tree
 from matplotlib.axes import Axes
 from matplotlib.collections import PatchCollection
 from matplotlib.colorbar import Colorbar
 from matplotlib.colors import Colormap, Normalize
 from matplotlib.figure import Figure
 from matplotlib.patches import Patch
 from matplotlib.projections.polar import PolarAxes
 
 from pycirclize import config, utils
-from pycirclize.parser import Bed, Matrix
+from pycirclize.parser import Bed, Matrix, RadarTable
 from pycirclize.patches import (
     ArcLine,
     ArcRectangle,
     BezierCurveLine,
     BezierCurveLink,
     Line,
 )
@@ -171,14 +172,162 @@
         return self._ax
 
     ############################################################
     # Public Method
     ############################################################
 
     @staticmethod
+    def radar_chart(
+        table: str | Path | pd.DataFrame | RadarTable,
+        *,
+        r_lim: tuple[float, float] = (0, 100),
+        vmax: float = 100,
+        fill: bool = True,
+        marker_size: int = 0,
+        bg_color: str | None = "#eeeeee80",
+        circular: bool = False,
+        cmap: str | dict[str, str] = "Set2",
+        show_grid_label: bool = True,
+        grid_interval_ratio: float | None = 0.2,
+        grid_line_kws: dict[str, Any] | None = None,
+        grid_label_kws: dict[str, Any] | None = None,
+        grid_label_formatter: Callable[[float], str] | None = None,
+        label_kws_handler: Callable[[str], dict[str, Any]] | None = None,
+        line_kws_handler: Callable[[str], dict[str, Any]] | None = None,
+        marker_kws_handler: Callable[[str], dict[str, Any]] | None = None,
+    ) -> Circos:
+        """Plot radar chart
+
+        Parameters
+        ----------
+        table : str | Path | pd.DataFrame | RadarTable
+            Table file or Table dataframe or RadarTable instance
+        r_lim : tuple[float, float], optional
+            Radar chart radius limit region (0 - 100)
+        vmax : float, optional
+            Max value
+        fill : bool, optional
+            If True, fill color of radar chart.
+        marker_size : int, optional
+            Marker size
+        bg_color : str | None, optional
+            Background color
+        circular : bool, optional
+            If True, plot with circular style.
+        cmap : str | dict[str, str], optional
+            Colormap assigned to each target row(index) in table.
+            User can set matplotlib's colormap (e.g. `tab10`, `Set2`) or
+            target_name -> color dict (e.g. `dict(A="red", B="blue", C="green", ...)`)
+        show_grid_label : bool, optional
+            If True, show grid label.
+        grid_interval_ratio : float | None, optional
+            Grid interval ratio (0.0 - 1.0)
+        grid_line_kws : dict[str, Any] | None, optional
+            Keyword arguments passed to `track.line()` method
+            (e.g. `dict(color="black", ls="dotted", lw=1.0, ...)`)
+        grid_label_kws : dict[str, Any] | None, optional
+            Keyword arguments passed to `track.text()` method
+            (e.g. `dict(size=12, color="red", ...)`)
+        grid_label_formatter : Callable[[float], str] | None, optional
+            User-defined function to format grid label (e.g. `lambda v: f"{v:.1f}%"`).
+        label_kws_handler : Callable[[str], dict[str, Any]] | None, optional
+            Handler function for keyword arguments passed to `track.text()` method.
+            Handler function takes each column name of table as an argument.
+        line_kws_handler : Callable[[str], dict[str, Any]] | None, optional
+            Handler function for keyword arguments passed to `track.line()` method.
+            Handler function takes each row(index) name of table as an argument.
+        marker_kws_handler : Callable[[str], dict[str, Any]] | None, optional
+            Handler function for keyword arguments passed to `track.scatter()` method.
+            Handler function takes each row(index) name of table as an argument.
+
+        Returns
+        -------
+        circos : Circos
+            Circos instance initialized for radar chart
+        """
+        # Setup default properties
+        grid_line_kws = {} if grid_line_kws is None else deepcopy(grid_line_kws)
+        for k, v in dict(color="grey", ls="dashed", lw=0.5).items():
+            grid_line_kws.setdefault(k, v)
+
+        grid_label_kws = {} if grid_label_kws is None else deepcopy(grid_label_kws)
+        for k, v in dict(color="dimgrey", size=10, ha="left", va="top").items():
+            grid_label_kws.setdefault(k, v)
+
+        # Initialize circos for radar chart
+        radar_table = table if isinstance(table, RadarTable) else RadarTable(table)
+        circos = Circos(dict(radar=radar_table.col_num))
+        sector = circos.sectors[0]
+        track = sector.add_track(r_lim)
+        x = np.arange(radar_table.col_num + 1)
+
+        # Plot background color
+        if bg_color:
+            track.fill_between(x, [vmax] * len(x), arc=circular, color=bg_color)
+
+        # Plot grid line
+        if grid_interval_ratio:
+            if not 0 < grid_interval_ratio <= 1.0:
+                raise ValueError(f"{grid_interval_ratio=} is invalid.")
+            # Plot horizontal grid line & label
+            stop, step = vmax + (vmax / 1000), vmax * grid_interval_ratio
+            for v in np.arange(0, stop, step):
+                track.line(x, [v] * len(x), vmax=vmax, arc=circular, **grid_line_kws)
+                if show_grid_label:
+                    r = track._y_to_r(v, 0, vmax)
+                    # Format grid label
+                    if grid_label_formatter:
+                        text = grid_label_formatter(v)
+                    else:
+                        v = float(f"{v:.9f}")  # Correct rounding error
+                        text = f"{v:.0f}" if math.isclose(int(v), float(v)) else str(v)
+                    track.text(text, 0, r, **grid_label_kws)
+            # Plot vertical grid line
+            for p in x[:-1]:
+                track.line([p, p], [0, vmax], vmax=vmax, **grid_line_kws)
+
+        # Plot radar charts
+        if isinstance(cmap, str):
+            row_name2color = radar_table.get_row_name2color(cmap)
+        else:
+            row_name2color = cmap
+        for row_name, values in radar_table.row_name2values.items():
+            y = values + [values[0]]
+            color = row_name2color[row_name]
+            line_kws = line_kws_handler(row_name) if line_kws_handler else {}
+            line_kws.setdefault("lw", 1.0)
+            line_kws.setdefault("label", row_name)
+            track.line(x, y, vmax=vmax, arc=False, color=color, **line_kws)
+            if marker_size > 0:
+                marker_kws = marker_kws_handler(row_name) if marker_kws_handler else {}
+                marker_kws.setdefault("marker", "o")
+                marker_kws.setdefault("zorder", 2)
+                marker_kws.update(s=marker_size**2)
+                track.scatter(x, y, vmax=vmax, color=color, **marker_kws)
+            if fill:
+                track.fill_between(x, y, vmax=vmax, arc=False, color=color, alpha=0.5)
+
+        # Plot column names
+        for idx, col_name in enumerate(radar_table.col_names):
+            deg = 360 * (idx / sector.size)
+            label_kws = label_kws_handler(col_name) if label_kws_handler else {}
+            label_kws.setdefault("size", 12)
+            if math.isclose(deg, 0):
+                label_kws.update(va="bottom")
+            elif math.isclose(deg, 180):
+                label_kws.update(va="top")
+            elif 0 < deg < 180:
+                label_kws.update(ha="left")
+            elif 180 < deg < 360:
+                label_kws.update(ha="right")
+            track.text(col_name, idx, r=105, adjust_rotation=False, **label_kws)
+
+        return circos
+
+    @staticmethod
     def initialize_from_matrix(
         matrix: str | Path | pd.DataFrame | Matrix,
         *,
         start: float = 0,
         end: float = 360,
         space: float | list[float] = 0,
         endspace: bool = True,
@@ -298,14 +447,16 @@
                 handle_link_kws = link_kws_handler(from_label, to_label)
                 if handle_link_kws is not None:
                     _link_kws.update(handle_link_kws)
             circos.link(*link, **_link_kws)
 
         return circos
 
+    chord_diagram = initialize_from_matrix
+
     @staticmethod
     def initialize_from_tree(
         tree_data: str | Path | Tree,
         *,
         start: float = 0,
         end: float = 360,
         r_lim: tuple[float, float] = (50, 100),
@@ -833,32 +984,35 @@
         self._plot_funcs.append(plot_colorbar)
 
     def plotfig(
         self,
         dpi: int = 100,
         *,
         ax: PolarAxes | None = None,
+        figsize: tuple[float, float] = (8, 8),
     ) -> Figure:
         """Plot figure
 
         Parameters
         ----------
         dpi : int, optional
             Figure DPI
         ax : PolarAxes | None
             If None, figure and axes are newly created.
+        figsize : tuple[float, float], optional
+            Figure size
 
         Returns
         -------
         figure : Figure
             Circos matplotlib figure
         """
         if ax is None:
             # Initialize Figure & PolarAxes
-            fig, ax = self._initialize_figure(dpi=dpi)
+            fig, ax = self._initialize_figure(figsize=figsize, dpi=dpi)
         else:
             # Check PolarAxes or not
             if not isinstance(ax, PolarAxes):
                 ax_class_name = type(ax).__name__
                 err_msg = f"Input ax is not PolarAxes (={ax_class_name})."
                 raise ValueError(err_msg)
             fig = ax.get_figure()
@@ -887,31 +1041,34 @@
         return fig
 
     def savefig(
         self,
         savefile: str | Path,
         *,
         dpi: int = 100,
+        figsize: tuple[float, float] = (8, 8),
         pad_inches: float = 0.5,
     ) -> None:
         """Save figure to file
 
         `circos.savefig("result.png")` is alias for
         `circos.plotfig().savefig("result.png")`
 
         Parameters
         ----------
         savefile : str | Path
             Save file (`*.png`|`*.jpg`|`*.svg`|`*.pdf`)
         dpi : int, optional
             DPI
+        figsize : tuple[float, float], optional
+            Figure size
         pad_inches : float, optional
             Padding inches
         """
-        fig = self.plotfig(dpi=dpi)
+        fig = self.plotfig(dpi=dpi, figsize=figsize)
         fig.savefig(
             fname=savefile,  # type: ignore
             dpi=dpi,
             pad_inches=pad_inches,
             bbox_inches="tight",
         )
         # Clear & close figure to suppress memory leak
```

### Comparing `pycirclize-1.3.0/src/pycirclize/config.py` & `pycirclize-1.4.0/src/pycirclize/config.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/parser/bed.py` & `pycirclize-1.4.0/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/parser/genbank.py` & `pycirclize-1.4.0/src/pycirclize/parser/genbank.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,128 @@
 from __future__ import annotations
 
 import bz2
 import gzip
+import warnings
 import zipfile
 from collections import defaultdict
 from io import StringIO, TextIOWrapper
 from pathlib import Path
-from typing import Any
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
 from Bio.SeqFeature import Seq, SeqFeature, SimpleLocation
 from Bio.SeqRecord import SeqRecord
 
 
 class Genbank:
     """Genbank Parser Class"""
 
     def __init__(
         self,
-        gbk_source: str | Path | TextIOWrapper,
+        gbk_source: str | Path | TextIOWrapper | list[SeqRecord],
+        *,
         name: str | None = None,
-        reverse: bool = False,
-        min_range: int | None = None,
-        max_range: int | None = None,
+        min_range: None = None,
+        max_range: None = None,
     ):
         """
         Parameters
         ----------
-        gbk_source : str | Path | TextIOWrapper
+        gbk_source : str | Path | TextIOWrapper | list[SeqRecord]
             Genbank file or source
             (`*.gz`, `*.bz2`, `*.zip` compressed file can be readable)
         name : str | None, optional
             name (If None, `file name` or `record name` is set)
-        reverse : bool, optional
-            If True, reverse complement genome is used
-        min_range : int | None, optional
-            Min range to be extracted (Default: `0`)
-        max_range : int | None, optional
-            Max range to be extracted (Default: `genome length`)
+        min_range : None, optional
+            No longer used. Left for backward compatibility.
+        max_range : None, optional
+            No longer used. Left for backward compatibility.
         """
         self._gbk_source = gbk_source
-        self._name = name
-        self._records = self._parse_gbk_source(gbk_source)
-        self.reverse = reverse
-        self.min_range = 0 if min_range is None else min_range
-        self.max_range = self.full_genome_length if max_range is None else max_range
-
-        if not 0 <= self.min_range <= self.max_range <= self.full_genome_length:
-            err_msg = f"min_range={min_range}, max_range={max_range} is invalid. \n"
-            err_msg += "Range must be "
-            err_msg += f"'0 <= min_range <= max_range <= {self.full_genome_length}'"
-            raise ValueError(err_msg)
+        if isinstance(gbk_source, (str, Path, StringIO, TextIOWrapper)):
+            self._records = self._parse_gbk_source(gbk_source)
+        else:
+            self._records = gbk_source
 
-    def _parse_gbk_source(
-        self, gbk_source: str | Path | TextIOWrapper
-    ) -> list[SeqRecord]:
-        """Parse genbank source
+        # Set genbank name
+        if name is not None:
+            self._name = name
+        elif isinstance(self._gbk_source, (str, Path)):
+            gbk_file = Path(self._gbk_source)
+            if gbk_file.suffix in (".gz", ".bz2", ".zip"):
+                self._name = gbk_file.with_suffix("").with_suffix("").name
+            else:
+                self._name = gbk_file.with_suffix("").name
+        elif isinstance(self._gbk_source, (StringIO, TextIOWrapper)):
+            self._name = self._records[0].name
+        else:
+            raise NotImplementedError("Failed to get name.")
 
-        Parameters
-        ----------
-        gbk_source : str | Path | TextIOWrapper
-            Genbank file or source
+        if min_range or max_range:
+            warnings.warn("min_range & max_range is no longer used in Genbank parser.")
 
-        Returns
-        -------
-        list[SeqRecord]
-            Genbank SeqRecords
-        """
-        # Parse compressed file
-        if isinstance(gbk_source, (str, Path)):
-            if Path(gbk_source).suffix == ".gz":
-                with gzip.open(gbk_source, mode="rt") as f:
-                    return list(SeqIO.parse(f, "genbank"))
-            elif Path(gbk_source).suffix == ".bz2":
-                with bz2.open(gbk_source, mode="rt") as f:
-                    return list(SeqIO.parse(f, "genbank"))
-            elif Path(gbk_source).suffix == ".zip":
-                with zipfile.ZipFile(gbk_source) as zip:
-                    with zip.open(zip.namelist()[0]) as f:
-                        return list(SeqIO.parse(TextIOWrapper(f), "genbank"))
-        # Parse no compressed file or TextIOWrapper
-        return list(SeqIO.parse(gbk_source, "genbank"))
+    ############################################################
+    # Property
+    ############################################################
 
     @property
     def name(self) -> str:
         """Name"""
-        if self._name is not None:
-            return self._name
-        if isinstance(self._gbk_source, (str, Path)):
-            gbk_file = Path(self._gbk_source)
-            if gbk_file.suffix in (".gz", ".bz2", ".zip"):
-                return gbk_file.with_suffix("").with_suffix("").name
-            else:
-                return gbk_file.with_suffix("").name
-        elif isinstance(self._gbk_source, (StringIO, TextIOWrapper)):
-            return self._records[0].name
-        else:
-            raise NotImplementedError()
+        return self._name
 
     @property
     def records(self) -> list[SeqRecord]:
         """Genbank records"""
-        if self.reverse:
-            return list(reversed([r.reverse_complement() for r in self._records]))
-        else:
-            return self._records
+        return self._records
 
     @property
-    def full_genome_length(self) -> int:
-        """Full genome sequence length"""
-        return len(self.full_genome_seq)
+    def genome_seq(self) -> str:
+        """Genome sequence (only first record)"""
+        return str(self.records[0].seq)
 
     @property
     def genome_length(self) -> int:
-        """Range genome sequence length (Same as `range_size`)"""
+        """Genome length (only first record)"""
         return len(self.genome_seq)
 
     @property
     def range_size(self) -> int:
-        """Range size (`max_range - min_range`)"""
-        return self.max_range - self.min_range
+        """Same as `self.genome_length` (Left for backward compatibility)"""
+        return self.genome_length
 
     @property
     def full_genome_seq(self) -> str:
-        """Full genome sequence"""
+        """Full genome sequence (concatenate all records)"""
         return "".join(str(r.seq) for r in self.records)
 
     @property
-    def genome_seq(self) -> str:
-        """Range genome sequence"""
-        seq = "".join(str(r.seq) for r in self.records)
-        return seq[self.min_range : self.max_range]
-
-    def calc_genome_gc_content(self) -> float:
-        """Calculate genome GC content"""
-        try:
-            gc_content = SeqUtils.gc_fraction(self.genome_seq) * 100
-        except AttributeError:
-            # For backward compatibility, biopython <= 1.79
-            gc_content = SeqUtils.GC(self.genome_seq)  # type: ignore
+    def full_genome_length(self) -> int:
+        """Full genome length (concatenate all records)"""
+        return len(self.full_genome_seq)
+
+    ############################################################
+    # Public Method
+    ############################################################
+
+    def calc_genome_gc_content(self, seq: str | None = None) -> float:
+        """Calculate genome GC content
+
+        Parameters
+        ----------
+        seq : str | None, optional
+            Sequence for GC content calculation (Default: `self.genome_seq`)
+
+        Returns
+        -------
+        gc_content : float
+            GC content
+        """
+        seq = self.genome_seq if seq is None else seq
+        gc_content = SeqUtils.gc_fraction(seq) * 100
         return gc_content
 
     def calc_gc_skew(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
         *,
@@ -203,15 +182,15 @@
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
-            Sequence for GCskew calculation (Default: `self.genome_seq`)
+            Sequence for GC content calculation (Default: `self.genome_seq`)
 
         Returns
         -------
         gc_content_result_tuple : tuple[np.ndarray, np.ndarray]
             Position list & GC content list
         """
         pos_list, gc_content_list = [], []
@@ -226,19 +205,15 @@
         for pos in pos_list:
             window_start_pos = pos - int(window_size / 2)
             window_end_pos = pos + int(window_size / 2)
             window_start_pos = 0 if window_start_pos < 0 else window_start_pos
             window_end_pos = len(seq) if window_end_pos > len(seq) else window_end_pos
 
             subseq = seq[window_start_pos:window_end_pos]
-            try:
-                gc_content = SeqUtils.gc_fraction(subseq) * 100
-            except AttributeError:
-                # For backward compatibility, biopython <= 1.79
-                gc_content = SeqUtils.GC(subseq)  # type: ignore
+            gc_content = SeqUtils.gc_fraction(subseq) * 100
             gc_content_list.append(gc_content)
 
         return (np.array(pos_list), np.array(gc_content_list))
 
     def get_seqid2seq(self) -> dict[str, str]:
         """Get seqid & complete/contig/scaffold genome sequence dict
 
@@ -259,229 +234,192 @@
         """
         return {seqid: len(seq) for seqid, seq in self.get_seqid2seq().items()}
 
     def get_seqid2features(
         self,
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool | None = False,
     ) -> dict[str, list[SeqFeature]]:
         """Get seqid & features in target seqid genome dict
 
         Parameters
         ----------
         feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
-        pseudogene : bool | None, optional
-            If True, `pseudo=`, `pseudogene=` tagged record only extract.
-            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
-            If None, extract regardless of pseudogene tag.
 
         Returns
         -------
         seqid2features : dict[str, list[SeqFeature]]
             seqid & features dict
         """
         seqid2features = defaultdict(list)
         for rec in self.records:
-            feat: SeqFeature
-            for feat in rec.features:
-                strand = feat.location.strand
-                if feature_type is not None and feat.type != feature_type:
+            feature: SeqFeature
+            for feature in rec.features:
+                strand = feature.location.strand
+                if feature_type is not None and feature.type != feature_type:
                     continue
                 if target_strand is not None and strand != target_strand:
                     continue
-                if strand == -1:
-                    start = self._to_int(feat.location.parts[-1].start)
-                    end = self._to_int(feat.location.parts[0].end)
-                else:
-                    start = self._to_int(feat.location.parts[0].start)
-                    end = self._to_int(feat.location.parts[-1].end)
-
-                qual = feat.qualifiers
-                has_pseudo_qual = "pseudo" in qual or "pseudogene" in qual
-                if (
-                    pseudogene is None
-                    or (pseudogene is True and has_pseudo_qual)
-                    or (pseudogene is False and not has_pseudo_qual)
-                ):
-                    seqid2features[rec.id].append(
-                        SeqFeature(
-                            location=SimpleLocation(start, end, strand),
-                            type=feat.type,
-                            qualifiers=feat.qualifiers,
-                        ),
-                    )
+                # Exclude feature which straddle genome start position
+                if self._is_straddle_feature(feature):
+                    continue
+                start = int(feature.location.start)  # type: ignore
+                end = int(feature.location.end)  # type: ignore
+                seqid2features[rec.id].append(
+                    SeqFeature(
+                        location=SimpleLocation(start, end, strand),
+                        type=feature.type,
+                        qualifiers=feature.qualifiers,
+                    ),
+                )
         return seqid2features
 
     def extract_features(
         self,
-        feature_type: str = "CDS",
+        feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        fix_position: bool = False,
-        allow_partial: bool = False,
-        pseudogene: bool = False,
+        target_range: tuple[int, int] | None = None,
     ) -> list[SeqFeature]:
-        """Extract features within min-max range
+        """Extract features (only first record)
 
         Parameters
         ----------
-        feature_type : str, optional
-            Extract feature type
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
         target_strand : int | None, optional
-            Extract target strand
-        fix_position : bool, optional
-            If True, fix feature start & end position by specified min_range parameter
-            (fixed_start = start - min_range, fixed_end = end - min_range)
-        allow_partial : bool, optional
-            If True, allow extraction of features that are partially included in range
-        pseudogene : bool, optional
-            If True and `feature_type='CDS'`, only extract CDS features with
-            `/pseudo` or `/pseudogene` qualifiers.
+            Extract target strand. If None, extract regardless of strand.
+        target_range : tuple[int, int] | None, optional
+            Extract target range. If None, extract regardless of range.
 
         Returns
         -------
         features : list[SeqFeature]
             Extracted features
         """
-        extract_features = []
-        min_range, max_range = self.min_range, self.max_range
-        base_len = 0
-        for record in self.records:
-            features = [f for f in record.features if f.type == feature_type]
-            for f in features:
-                if feature_type == "CDS":
-                    if pseudogene:
-                        # Only extract pseudogene
-                        qual = f.qualifiers
-                        if "pseudo" not in qual and "pseudogene" not in qual:
-                            continue
-                    else:
-                        # Exclude pseudogene (no translated gene)
-                        translation = f.qualifiers.get("translation", [None])[0]
-                        if translation is None:
-                            continue
-                strand = f.location.strand
-                if strand == -1:
-                    # Handle rare case (complement & join)
-                    # Found in NC_00913 protein_id=NP_417367.1
-                    start = self._to_int(f.location.parts[-1].start) + base_len
-                    end = self._to_int(f.location.parts[0].end) + base_len
-                else:
-                    start = self._to_int(f.location.parts[0].start) + base_len
-                    end = self._to_int(f.location.parts[-1].end) + base_len
-                # Restrict features in range
-                if allow_partial:
-                    if (
-                        not min_range <= start <= max_range
-                        and not min_range <= end <= max_range
-                    ):
-                        # Ignore completely out of range features
-                        continue
-                    # If partially within range, fix position to within range
-                    if start <= min_range <= end <= max_range:
-                        start = min_range
-                    if min_range <= start <= max_range <= end:
-                        end = max_range
-                else:
-                    if not min_range <= start <= end <= max_range:
-                        # Ignore out of range features
-                        continue
-                # Extract only target strand feature
-                if target_strand is not None and strand != target_strand:
-                    continue
-                # Fix start & end position by min_range
-                if fix_position:
-                    start -= min_range
-                    end -= min_range
-
-                extract_features.append(
-                    SeqFeature(
-                        location=SimpleLocation(start, end, strand),
-                        type=f.type,
-                        qualifiers=f.qualifiers,
-                    ),
-                )
-            base_len += len(record.seq)
-
-        return extract_features
+        seqid2features = self.get_seqid2features(feature_type, target_strand)
+        first_record_features = list(seqid2features.values())[0]
+        if target_range:
+            target_features = []
+            for feature in first_record_features:
+                start = int(feature.location.start)  # type: ignore
+                end = int(feature.location.end)  # type: ignore
+                if min(target_range) <= start <= end <= max(target_range):
+                    target_features.append(feature)
+            return target_features
+        else:
+            return first_record_features
 
-    def write_cds_fasta(
-        self,
-        fasta_outfile: str | Path,
-        seqtype: str = "protein",
-        fix_position: bool = False,
-        allow_partial: bool = False,
-    ):
-        """Write CDS protein features fasta file
+    def write_cds_fasta(self, outfile: str | Path) -> None:
+        """Write CDS fasta file
 
         Parameters
         ----------
-        fasta_outfile : str | Path
-            CDS fasta file
-        seqtype : str, optional
-            Sequence type (`protein`|`nucleotide`)
-        fix_position : bool, optional
-            If True, fix feature start & end position by specified min_range parameter
-            (fixed_start = start - min_range, fixed_end = end - min_range)
-        allow_partial : bool, optional
-            If True, features that are partially included in range are also extracted
-        """
-        features = self.extract_features("CDS", None, fix_position, allow_partial)
-        cds_seq_records: list[SeqRecord] = []
-        for idx, feature in enumerate(features, 1):
-            qualifiers = feature.qualifiers
-            protein_id = qualifiers.get("protein_id", [None])[0]
-            product = qualifiers.get("product", [""])[0]
-            translation = qualifiers.get("translation", [None])[0]
-
-            start = self._to_int(feature.location.start)
-            end = self._to_int(feature.location.end)
-            strand = -1 if feature.location.strand == -1 else 1
-
-            location_id = f"|{start}_{end}_{strand}|"
-            if protein_id is None:
-                seq_id = f"GENE{idx:06d}{location_id}"
-            else:
-                seq_id = f"GENE{idx:06d}_{protein_id}{location_id}"
-
-            if seqtype == "protein":
+        outfile : str | Path
+            Output CDS fasta file
+        """
+        cds_records: list[SeqRecord] = []
+        counter = 0
+        seqid2cds_features = self.get_seqid2features(feature_type="CDS")
+        for seqid, cds_features in seqid2cds_features.items():
+            for cds_feature in cds_features:
+                # Ignore no translation feature
+                translation = cds_feature.qualifiers.get("translation", [None])[0]
+                if translation is None:
+                    continue
+                # Get feature location
+                start = int(cds_feature.location.start)  # type: ignore
+                end = int(cds_feature.location.end)  # type: ignore
+                strand = -1 if cds_feature.location.strand == -1 else 1
+                # Set feature id
+                location_id = f"|{seqid}|{start}_{end}_{strand}|"
+                protein_id = cds_feature.qualifiers.get("protein_id", [None])[0]
+                if protein_id is None:
+                    feature_id = f"GENE{counter:06d}{location_id}"
+                else:
+                    feature_id = f"GENE{counter:06d}_{protein_id}{location_id}"
+                counter += 1
+                # Add SeqRecord of CDS feature
                 seq = Seq(translation)
-            elif seqtype == "nucleotide":
-                seq = Seq(feature.location.extract(self.genome_seq))  # type: ignore
-            else:
-                raise ValueError(f"{seqtype=} is invalid.")
-
-            cds_seq_record = SeqRecord(seq=seq, id=seq_id, description=product)
-            cds_seq_records.append(cds_seq_record)
-
-        SeqIO.write(cds_seq_records, fasta_outfile, "fasta-2line")
+                product = cds_feature.qualifiers.get("product", [""])[0]
+                seq_record = SeqRecord(seq, feature_id, description=product)
+                cds_records.append(seq_record)
+        # Write CDS file
+        SeqIO.write(cds_records, outfile, "fasta-2line")
 
-    def write_genome_fasta(
-        self,
-        outfile: str | Path,
-    ) -> None:
+    def write_genome_fasta(self, outfile: str | Path) -> None:
         """Write genome fasta file
 
         Parameters
         ----------
         outfile : str | Path
             Output genome fasta file
         """
-        write_seq = self.genome_seq
         with open(outfile, "w") as f:
-            f.write(f">{self.name}\n{write_seq}\n")
+            for seqid, seq in self.get_seqid2seq().items():
+                f.write(f">{seqid}\n{seq}\n")
 
-    def _to_int(self, value: Any) -> int:
-        """Convert to int (Required for AbstractPosition|ExactPosition)"""
-        return int(str(value).replace("<", "").replace(">", ""))
+    ############################################################
+    # Private Method
+    ############################################################
 
-    def __str__(self):
-        name = str(self._gbk_source)
-        min_max_range = f"{self.min_range:,} - {self.max_range:,} bp"
-        if self.reverse:
-            return f"{name} ({min_max_range}) [Reverse Complement]"
+    def _parse_gbk_source(
+        self, gbk_source: str | Path | TextIOWrapper
+    ) -> list[SeqRecord]:
+        """Parse genbank source
+
+        Parameters
+        ----------
+        gbk_source : str | Path | TextIOWrapper
+            Genbank file or source
+
+        Returns
+        -------
+        list[SeqRecord]
+            Genbank SeqRecords
+        """
+        # Parse compressed file
+        if isinstance(gbk_source, (str, Path)):
+            if Path(gbk_source).suffix == ".gz":
+                with gzip.open(gbk_source, mode="rt") as f:
+                    return list(SeqIO.parse(f, "genbank"))
+            elif Path(gbk_source).suffix == ".bz2":
+                with bz2.open(gbk_source, mode="rt") as f:
+                    return list(SeqIO.parse(f, "genbank"))
+            elif Path(gbk_source).suffix == ".zip":
+                with zipfile.ZipFile(gbk_source) as zip:
+                    with zip.open(zip.namelist()[0]) as f:
+                        return list(SeqIO.parse(TextIOWrapper(f), "genbank"))
+        # Parse no compressed file or TextIOWrapper
+        return list(SeqIO.parse(gbk_source, "genbank"))
+
+    def _is_straddle_feature(self, feature: SeqFeature) -> bool:
+        """Check target feature straddle genome start position or not
+
+        Parameters
+        ----------
+        feature : SeqFeature
+            Target feature
+
+        Returns
+        -------
+        result : bool
+            Check result
+        """
+        strand = feature.location.strand
+        if strand == -1:
+            start = int(feature.location.parts[-1].start)  # type: ignore
+            end = int(feature.location.parts[0].end)  # type: ignore
         else:
-            return f"{name} ({min_max_range})"
+            start = int(feature.location.parts[0].start)  # type: ignore
+            end = int(feature.location.parts[-1].end)  # type: ignore
+        return True if start > end else False
+
+    def __str__(self):
+        text = f"{self.name}: {len(self.records)} records\n"
+        for num, (seqid, size) in enumerate(self.get_seqid2size().items(), 1):
+            text += f"{num:02d}. {seqid} ({size:,} bp)\n"
+        return text
```

### Comparing `pycirclize-1.3.0/src/pycirclize/parser/gff.py` & `pycirclize-1.4.0/src/pycirclize/parser/gff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import bz2
 import gzip
+import warnings
 import zipfile
 from collections import defaultdict
 from dataclasses import dataclass
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Any, TextIO
 
@@ -14,148 +15,45 @@
 
 class Gff:
     """GFF Parser Class"""
 
     def __init__(
         self,
         gff_file: str | Path,
+        *,
         name: str | None = None,
         target_seqid: str | None = None,
-        min_range: int | None = None,
-        max_range: int | None = None,
+        min_range: None = None,
+        max_range: None = None,
     ):
         """
         Parameters
         ----------
         gff_file : str | Path
             GFF file (`*.gz`, `*.bz2`, `*.zip` compressed file can be readable)
         name : str | None, optional
             name (If None, `file name` is set)
         target_seqid : str | None, optional
             Target seqid to be extracted. If None, only first seqid record is extracted.
-        min_range : int | None, optional
-            Min range to be extracted.
-            If None, appropriate value is taken from GFF records.
-        max_range : int | None, optional
-            Max range to be extracted.
-            If None, appropriate value is taken from GFF records.
+        min_range : None, optional
+            No longer used. Left for backward compatibility.
+        max_range : None, optional
+            No longer used. Left for backward compatibility.
         """
         self._gff_file = Path(gff_file)
         self._name = name
         self._records, start, end = self._parse_gff(gff_file, target_seqid)
-        self.min_range = start if min_range is None else min_range
-        self.max_range = end if max_range is None else max_range
         self._seq_region = (start, end)
 
-        if not 0 <= self.min_range <= self.max_range:
-            err_msg = "Range must be '0 <= min_range <= max_range' "
-            err_msg += f"({self.min_range=}, {self.max_range=})"
-            raise ValueError(err_msg)
-
-    def _parse_gff(
-        self,
-        gff_file: str | Path,
-        target_seqid: str | None,
-    ) -> tuple[list[GffRecord], int, int]:
-        """Parse GFF file
-
-        Only parse target seqid record.
-        If target_record is None, only parse first seqid record.
+        if min_range or max_range:
+            warnings.warn("min_range & max_range is no longer used in Gff parser.")
 
-        Parameters
-        ----------
-        gff_file : str | Path
-            GFF file
-        target_seqid : str | None
-            Target seqid to be extracted
-
-        Returns
-        -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
-        """
-        gff_file = Path(gff_file)
-        if gff_file.suffix == ".gz":
-            with gzip.open(gff_file, mode="rt") as f:
-                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
-        elif gff_file.suffix == ".bz2":
-            with bz2.open(gff_file, mode="rt") as f:
-                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
-        elif gff_file.suffix == ".zip":
-            with zipfile.ZipFile(gff_file) as zip:
-                with zip.open(zip.namelist()[0]) as f:
-                    io = TextIOWrapper(f)
-                    gff_records, start, end = self._parse_gff_textio(io, target_seqid)
-        else:
-            with open(gff_file) as f:
-                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
-
-        return gff_records, start, end
-
-    def _parse_gff_textio(
-        self,
-        handle: TextIO,
-        target_seqid: str | None = None,
-    ) -> tuple[list[GffRecord], int, int]:
-        """Parse GFF file TextIO
-
-        Parameters
-        ----------
-        handle : TextIO
-            GFF TextIO handle
-        target_seqid : str | None, optional
-            GFF target seqid
-
-        Returns
-        -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
-        """
-        # Parse GFF lines
-        gff_all_lines = handle.read().splitlines()
-        gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
-        gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
-        if len(gff_records) == 0:
-            err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
-            raise ValueError(err_msg)
-
-        # Get target seqid & GFF records
-        seqid_list = list(dict.fromkeys([rec.seqid for rec in gff_records]))
-        if target_seqid is None:
-            target_seqid = seqid_list[0]
-        if target_seqid not in seqid_list:
-            err_msg = f"Not found {target_seqid=} in '{self._gff_file}'"
-            raise ValueError(err_msg)
-        target_gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
-
-        # Try to get start-end region from '##sequence-region' annotation line
-        # If not found, (0, max_coordinate) is set as start-end
-        seqid2start_end: dict[str, tuple[int, int]] = {}
-        for seqid in seqid_list:
-            start, end = None, None
-            for line in gff_all_lines:
-                if line.startswith("##sequence-region"):
-                    # e.g. `##sequence-region NC_XXXXXX 1 10000` (seqid, start, end)
-                    if len(line.split()) == 4 and line.split()[1] == seqid:
-                        start, end = line.split()[2:4]
-                        start, end = int(start) - 1, int(end)
-                        break
-            if start is None or end is None:
-                seqid_gff_records = [rec for rec in gff_records if rec.seqid == seqid]
-                start, end = 0, max([r.end for r in seqid_gff_records])
-            seqid2start_end[seqid] = (start, end)
-        seqid2size = {seqid: e - s for seqid, (s, e) in seqid2start_end.items()}
-
-        # Set properties
-        self._target_seqid = target_seqid
-        self._seqid_list = seqid_list
-        self._all_records = gff_records
-        self._seqid2size = seqid2size
-
-        return target_gff_records, *seqid2start_end[target_seqid]
+    ############################################################
+    # Property
+    ############################################################
 
     @property
     def name(self) -> str:
         """Name"""
         if self._name is not None:
             return self._name
         if self._gff_file.suffix in (".gz", ".bz2", ".zip"):
@@ -169,46 +67,51 @@
 
         If `##sequence-region` pragma is not found, seq_region=`(0, max_coords_value)`
         """
         return self._seq_region
 
     @property
     def records(self) -> list[GffRecord]:
-        """GFF records (target seqid only)"""
+        """GFF records (only target seqid)"""
         return self._records
 
     @property
     def all_records(self) -> list[GffRecord]:
         """All GFF records"""
         return self._all_records
 
     @property
-    def records_within_range(self) -> list[GffRecord]:
-        """GFF records within min-max range"""
-        target_gff_records: list[GffRecord] = []
-        for rec in self.records:
-            if rec.is_within_range(self.min_range, self.max_range):
-                target_gff_records.append(rec)
-        return target_gff_records
-
-    @property
-    def range_size(self) -> int:
-        """Range size (`max_range - min_range`)"""
-        return self.max_range - self.min_range
-
-    @property
     def target_seqid(self) -> str:
         """Target seqid"""
         return self._target_seqid
 
     @property
     def seqid_list(self) -> list[str]:
         """seqid list"""
         return self._seqid_list
 
+    @property
+    def genome_length(self) -> int:
+        """Genome length (target seqid record)"""
+        return max(self.seq_region)
+
+    @property
+    def range_size(self) -> int:
+        """Same as `self.genome_length` (Left for backward compatibility)"""
+        return self.genome_length
+
+    @property
+    def full_genome_length(self) -> int:
+        """Full genome length (concatenate all records)"""
+        return sum(list(self.get_seqid2size().values()))
+
+    ############################################################
+    # Public Method
+    ############################################################
+
     def get_seqid2size(self) -> dict[str, int]:
         """Get seqid & complete/contig/scaffold genome size dict
 
         By default, size is defined by `##sequence-region` pragma of target seqid.
         If `##sequence-region` is not found, size is defined by max coordinate size in
         target seqid features. This may differ from actual genome size.
 
@@ -219,83 +122,75 @@
         """
         return self._seqid2size
 
     def get_seqid2features(
         self,
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool | None = False,
     ) -> dict[str, list[SeqFeature]]:
         """Get seqid & features in target seqid genome dict
 
         Parameters
         ----------
         feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
-        pseudogene : bool | None, optional
-            If True, `pseudo=`, `pseudogene=` tagged record only extract.
-            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
-            If None, extract regardless of pseudogene tag.
 
         Returns
         -------
         seqid2features : dict[str, list[SeqFeature]]
             seqid & features dict
         """
         gff_records = GffRecord.filter_records(
             self.all_records,
             feature_type=feature_type,
             target_strand=target_strand,
-            pseudogene=pseudogene,
         )
         seqid2features: dict[str, list[SeqFeature]] = {}
         for seqid in self.seqid_list:
             seqid2features[seqid] = []
         for rec in gff_records:
             seqid2features[rec.seqid].append(rec.to_seq_feature())
         return seqid2features
 
     def extract_features(
         self,
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool | None = False,
+        target_range: tuple[int, int] | None = None,
     ) -> list[SeqFeature]:
-        """Extract features within min-max range
+        """Extract features
 
         Parameters
         ----------
         feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
             If None, extract regardless of feature type.
         target_strand : int | None, optional
             Extract target strand. If None, extract regardless of strand.
-        pseudogene : bool | None, optional
-            If True, `pseudo=`, `pseudogene=` tagged record only extract.
-            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
-            If None, extract all regardless of pseudogene tag.
+        target_range : tuple[int, int] | None, optional
+            Extract target range. If None, extract regardless of range.
 
         Returns
         -------
         features : list[SeqFeature]
             Feature list
         """
         gff_records = GffRecord.filter_records(
-            self.records_within_range,
+            self.records,
             feature_type=feature_type,
             target_strand=target_strand,
-            pseudogene=pseudogene,
+            target_range=target_range,
         )
         return [rec.to_seq_feature() for rec in gff_records]
 
     def extract_exon_features(self, feature_type: str = "mRNA") -> list[SeqFeature]:
-        """Extract exon structure features within min-max range
+        """Extract exon structure features
 
         Extract exons based on `parent feature` and `exon` ID-Parent relation
 
         Parameters
         ----------
         feature_type : str, optional
             Feature type (e.g. `mRNA`, `ncRNA` , etc...)
@@ -305,15 +200,15 @@
         features : list[SeqFeature]
             Feature list
         """
         # Extract exon features by mRNA-exon relation
         parent_id = None
         parent_id2record: dict[str, GffRecord] = {}
         parent_id2exons: dict[str, list[GffRecord]] = defaultdict(list)
-        for rec in self.records_within_range:
+        for rec in self._records:
             if rec.type == feature_type:
                 parent_id = rec.attrs.get("ID", [None])[0]
                 if parent_id is None:
                     continue
                 parent_id2record[parent_id] = rec
             if rec.type == "exon":
                 if parent_id is not None and parent_id == rec.attrs["Parent"][0]:
@@ -341,26 +236,129 @@
                 # If no exon exists, skip feature extraction
                 continue
 
             exon_features.append(exon_feature)
 
         return exon_features
 
-    def __str__(self):
-        return f"{self.name} ({self.min_range:,} - {self.max_range:,} bp)"
+    ############################################################
+    # Private Method
+    ############################################################
+
+    def _parse_gff(
+        self,
+        gff_file: str | Path,
+        target_seqid: str | None,
+    ) -> tuple[list[GffRecord], int, int]:
+        """Parse GFF file
+
+        Only parse target seqid record.
+        If target_record is None, only parse first seqid record.
+
+        Parameters
+        ----------
+        gff_file : str | Path
+            GFF file
+        target_seqid : str | None
+            Target seqid to be extracted
+
+        Returns
+        -------
+        gff_records, start, end : tuple[list[GffRecord], int, int]
+            GFF record list, start, end
+        """
+        gff_file = Path(gff_file)
+        if gff_file.suffix == ".gz":
+            with gzip.open(gff_file, mode="rt") as f:
+                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
+        elif gff_file.suffix == ".bz2":
+            with bz2.open(gff_file, mode="rt") as f:
+                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
+        elif gff_file.suffix == ".zip":
+            with zipfile.ZipFile(gff_file) as zip:
+                with zip.open(zip.namelist()[0]) as f:
+                    io = TextIOWrapper(f)
+                    gff_records, start, end = self._parse_gff_textio(io, target_seqid)
+        else:
+            with open(gff_file) as f:
+                gff_records, start, end = self._parse_gff_textio(f, target_seqid)
+
+        return gff_records, start, end
+
+    def _parse_gff_textio(
+        self,
+        handle: TextIO,
+        target_seqid: str | None = None,
+    ) -> tuple[list[GffRecord], int, int]:
+        """Parse GFF file TextIO
+
+        Parameters
+        ----------
+        handle : TextIO
+            GFF TextIO handle
+        target_seqid : str | None, optional
+            GFF target seqid
+
+        Returns
+        -------
+        gff_records, start, end : tuple[list[GffRecord], int, int]
+            GFF record list, start, end
+        """
+        # Parse GFF lines
+        gff_all_lines = handle.read().splitlines()
+        gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
+        gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
+        if len(gff_records) == 0:
+            err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
+            raise ValueError(err_msg)
+
+        # Get target seqid & GFF records
+        seqid_list = list(dict.fromkeys([rec.seqid for rec in gff_records]))
+        if target_seqid is None:
+            target_seqid = seqid_list[0]
+        if target_seqid not in seqid_list:
+            err_msg = f"Not found {target_seqid=} in '{self._gff_file}'"
+            raise ValueError(err_msg)
+        target_gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
+
+        # Try to get start-end region from '##sequence-region' annotation line
+        # If not found, (0, max_coordinate) is set as start-end
+        seqid2start_end: dict[str, tuple[int, int]] = {}
+        for seqid in seqid_list:
+            start, end = None, None
+            for line in gff_all_lines:
+                if line.startswith("##sequence-region"):
+                    # e.g. `##sequence-region NC_XXXXXX 1 10000` (seqid, start, end)
+                    if len(line.split()) == 4 and line.split()[1] == seqid:
+                        start, end = line.split()[2:4]
+                        start, end = int(start) - 1, int(end)
+                        break
+            if start is None or end is None:
+                seqid_gff_records = [rec for rec in gff_records if rec.seqid == seqid]
+                start, end = 0, max([r.end for r in seqid_gff_records])
+            seqid2start_end[seqid] = (start, end)
+        seqid2size = {seqid: e - s for seqid, (s, e) in seqid2start_end.items()}
+
+        # Set properties
+        self._target_seqid = target_seqid
+        self._seqid_list = seqid_list
+        self._all_records = gff_records
+        self._seqid2size = seqid2size
+
+        return target_gff_records, *seqid2start_end[target_seqid]
 
 
 @dataclass
 class GffRecord:
     """GFF Record DataClass"""
 
     seqid: str
     source: str
     type: str
-    start: int
+    start: int  # 1-based coordinate
     end: int
     score: float | None
     strand: int
     phase: int | None
     attrs: dict[str, list[str]]
 
     def is_within_range(self, min_range: int, max_range: int) -> bool:
@@ -380,46 +378,46 @@
         """
         if min_range <= self.start <= self.end <= max_range:
             return True
         else:
             return False
 
     def to_seq_feature(self) -> SeqFeature:
-        """Convert GffRecord to SeqFeature"""
+        """Convert GffRecord to SeqFeature (1-based to 0-based coordinate)"""
         return SeqFeature(
             location=self.to_feature_location(),
             type=self.type,
             id=self.attrs.get("ID", [""])[0],
             qualifiers=self.attrs,
         )
 
     def to_feature_location(self) -> SimpleLocation:
-        """Convert GffRecord to SimpleLocation
+        """Convert GffRecord to SimpleLocation (1-based to 0-based coordinate)
 
         Returns
         -------
-        location : SimpleLocation
-            Location
+        feature_location : SimpleLocation
+            Simple location
         """
-        return SimpleLocation(self.start, self.end, self.strand)
+        return SimpleLocation(self.start - 1, self.end, self.strand)
 
     def to_gff_line(self) -> str:
         """Convert GffRecord to GFF record line
 
         Returns
         -------
         gff_line : str
-            GFF record line (1-based coordinates)
+            GFF record line
         """
         return "\t".join(
             (
                 self.seqid,
                 self.source,
                 self.type,
-                str(self.start + 1),
+                str(self.start),
                 str(self.end),
                 "." if self.score is None else str(self.score),
                 "-" if self.strand == -1 else "+",
                 "." if self.phase is None else str(self.phase),
                 ";".join([f"{k}={','.join(v)}" for k, v in self.attrs.items()]),
             )
         )
@@ -446,24 +444,24 @@
     @staticmethod
     def parse_gff_line(gff_line: str) -> GffRecord:
         """Parse GFF record line
 
         Parameters
         ----------
         gff_line : str
-            GFF record line (1-based coordinates)
+            GFF record line
 
         Returns
         -------
         gff_record : GffRecord
-            GFF record (0-based coordinates)
+            GFF record
         """
         gff_elms: list[Any] = gff_line.split("\t")[0:9]
         # start, end
-        gff_elms[3], gff_elms[4] = int(gff_elms[3]) - 1, int(gff_elms[4])
+        gff_elms[3], gff_elms[4] = int(gff_elms[3]), int(gff_elms[4])
         # score
         gff_elms[5] = None if gff_elms[5] in (".", "") else float(gff_elms[5])
         # strand
         if gff_elms[6] == "+":
             gff_elms[6] = 1
         elif gff_elms[6] == "-":
             gff_elms[6] = -1
@@ -483,43 +481,39 @@
         return GffRecord(*gff_elms)
 
     @staticmethod
     def filter_records(
         gff_records: list[GffRecord],
         feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool | None = False,
+        target_range: tuple[int, int] | None = None,
     ) -> list[GffRecord]:
-        """Filter GFF records (feature_type, strand, pseudogene)
+        """Filter GFF records by feature_type, strand, range
 
         Parameters
         ----------
         gff_records : list[GffRecord]
             GFF records to be filterd
         feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...). If None, no filter.
         target_strand : int | None, optional
             Target strand. If None, no filter.
-        pseudogene : bool | None, optional
-            If True, `pseudo=`, `pseudogene=` tagged record only filter.
-            If False, `pseudo=`, `pseudogene=` not tagged record only filter.
-            If None, no filter.
+        target_range : tuple[int, int] | None, optional
+            Target range. If None, no filter.
 
         Returns
         -------
         filter_gff_records : list[SeqFeature]
             Filtered GFF records
         """
         filter_gff_records = []
         for rec in gff_records:
             if feature_type is not None and rec.type != feature_type:
                 continue
             if target_strand is not None and rec.strand != target_strand:
                 continue
-            has_pseudo_attr = "pseudo" in rec.attrs or "pseudogene" in rec.attrs
-            if (
-                pseudogene is None
-                or (pseudogene is True and has_pseudo_attr)
-                or (pseudogene is False and not has_pseudo_attr)
-            ):
-                filter_gff_records.append(rec)
+            if target_range is not None:
+                min_range, max_range = min(target_range), max(target_range)
+                if not min_range <= rec.start <= rec.end <= max_range:
+                    continue
+            filter_gff_records.append(rec)
         return filter_gff_records
```

### Comparing `pycirclize-1.3.0/src/pycirclize/parser/matrix.py` & `pycirclize-1.4.0/src/pycirclize/parser/matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/parser/table.py` & `pycirclize-1.4.0/src/pycirclize/parser/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 from pathlib import Path
 
 import pandas as pd
 
 from pycirclize.utils import ColorCycler
 
 
-class StackedBarTable:
-    """Table Parser Class
-
-    Basically used for plotting stacked bar chart
-    """
+class Table:
+    """Table Parser Base Class"""
 
     def __init__(
         self,
         table_data: str | Path | pd.DataFrame,
         *,
         delimiter: str = "\t",
     ):
@@ -24,15 +21,15 @@
         ----------
         table_data : str | Path | pd.DataFrame
             Table file or Table DataFrame
         delimiter : str, optional
             Table file delimiter. By default, `tab` delimiter.
         """
         if isinstance(table_data, (str, Path)):
-            table_data = pd.read_csv(table_data, sep=delimiter)
+            table_data = pd.read_csv(table_data, sep=delimiter, index_col=0)
         self._dataframe = table_data
 
     @property
     def dataframe(self) -> pd.DataFrame:
         """Table dataframe"""
         return self._dataframe
 
@@ -52,14 +49,56 @@
         return len(self.dataframe.index)
 
     @property
     def col_num(self) -> int:
         """Table column count number"""
         return len(self.dataframe.columns)
 
+    def get_col_name2color(self, cmap: str = "tab10") -> dict[str, str]:
+        """Get column name & color dict
+
+        Parameters
+        ----------
+        cmap : str, optional
+            Colormap (e.g. `tab10`, `Set3`)
+
+        Returns
+        -------
+        col_name2color : dict[str, str]
+            Column name & color dict
+        """
+        ColorCycler.set_cmap(cmap)
+        return {n: ColorCycler.get_color() for n in self.col_names}
+
+    def get_row_name2color(self, cmap: str = "tab10") -> dict[str, str]:
+        """Get row name & color dict
+
+        Parameters
+        ----------
+        cmap : str, optional
+            Colormap (e.g. `tab10`, `Set3`)
+
+        Returns
+        -------
+        col_name2color : dict[str, str]
+            Column name & color dict
+        """
+        ColorCycler.set_cmap(cmap)
+        return {n: ColorCycler.get_color() for n in self.row_names}
+
+    def __str__(self):
+        return str(self.dataframe)
+
+
+class StackedBarTable(Table):
+    """Table Parser Class
+
+    Basically used for plotting stacked bar chart
+    """
+
     @property
     def row_sum_vmax(self) -> float:
         """Max value in each row values sum"""
         return max(map(sum, self.dataframe.itertuples(index=False)))
 
     @property
     def row_name2sum(self) -> dict[str, float]:
@@ -81,30 +120,14 @@
             bottom = [row_name2stack_value[name] for name in self.row_names]
             for row_name in self.row_names:
                 value = float(self.dataframe[col_name][row_name])
                 row_name2stack_value[row_name] += value
             bottoms.append(bottom)
         return bottoms
 
-    def get_col_name2color(self, cmap: str = "tab10") -> dict[str, str]:
-        """Get column name & color dict
-
-        Parameters
-        ----------
-        cmap : str, optional
-            Colormap (e.g. `tab10`, `Set3`)
-
-        Returns
-        -------
-        col_name2color : dict[str, str]
-            Column name & color dict
-        """
-        ColorCycler.set_cmap(cmap)
-        return {n: ColorCycler.get_color() for n in self.col_names}
-
     def calc_bar_label_x_list(
         self,
         track_size: float,
     ) -> list[float]:
         """Calculate list of x position for bar label plot
 
         Parameters
@@ -169,9 +192,18 @@
         for cnt in range(len(self.row_names)):
             r_center = rmax - (interval * cnt) - (interval / 2)
             r_top = r_center + (interval / 2) * width
             r_bottom = r_center - (interval / 2) * width
             bar_r_lim_list.append((r_bottom, r_top))
         return bar_r_lim_list
 
-    def __str__(self):
-        return str(self.dataframe)
+
+class RadarTable(Table):
+    """Radar Table Parser Class"""
+
+    @property
+    def row_name2values(self) -> dict[str, list[float]]:
+        """Row name & values"""
+        row_name2values = {}
+        for row_name in self.row_names:
+            row_name2values[row_name] = list(self.dataframe.loc[row_name])
+        return row_name2values
```

### Comparing `pycirclize-1.3.0/src/pycirclize/patches.py` & `pycirclize-1.4.0/src/pycirclize/patches.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/sector.py` & `pycirclize-1.4.0/src/pycirclize/sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/track.py` & `pycirclize-1.4.0/src/pycirclize/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -983,14 +983,15 @@
         self,
         x: list[float] | np.ndarray,
         y1: list[float] | np.ndarray,
         y2: float | list[float] | np.ndarray = 0,
         *,
         vmin: float = 0,
         vmax: float | None = None,
+        arc: bool = True,
         **kwargs,
     ) -> None:
         """Fill the area between two horizontal(y1, y2) curves
 
         Parameters
         ----------
         x : list[float] | np.ndarray
@@ -999,14 +1000,17 @@
             Y coordinates (first curve definition)
         y2 : float | list[float] | np.ndarray, optional
             Y coordinate[s] (second curve definition)
         vmin : float, optional
             Y min value
         vmax : float | None, optional
             Y max value. If None, `max(y1 + y2)` is set.
+        arc : bool, optional
+            If True, plot arc style line for polar projection.
+            If False, simply plot linear style line.
         **kwargs : dict, optional
             Axes.fill_between properties (e.g. `fc="red", ec="black", lw=0.1, ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.fill_between.html>
         """
         rad = list(map(self.x_to_rad, x))
         if isinstance(y2, (list, tuple, np.ndarray)):
             y_all = list(y1) + list(y2)
@@ -1014,20 +1018,23 @@
             y_all = list(y1) + [y2]
             y2 = [float(y2)] * len(x)
         vmin = min(y_all) if vmin is None else vmin
         vmax = max(y_all) if vmax is None else vmax
         self._check_value_min_max(y_all, vmin, vmax)
 
         r2 = [self._y_to_r(v, vmin, vmax) for v in y2]
-        arc_rad, arc_r2 = self._to_arc_radr(rad, r2)
         r = [self._y_to_r(v, vmin, vmax) for v in y1]
-        _, arc_r = self._to_arc_radr(rad, r)
+        if arc:
+            plot_rad, plot_r2 = self._to_arc_radr(rad, r2)
+            _, plot_r = self._to_arc_radr(rad, r)
+        else:
+            plot_rad, plot_r, plot_r2 = rad, r, r2
 
         def plot_fill_between(ax: PolarAxes) -> None:
-            ax.fill_between(arc_rad, arc_r, arc_r2, **kwargs)  # type: ignore
+            ax.fill_between(plot_rad, plot_r, plot_r2, **kwargs)  # type: ignore
 
         self._plot_funcs.append(plot_fill_between)
 
     def heatmap(
         self,
         data: list | np.ndarray,
         *,
```

### Comparing `pycirclize-1.3.0/src/pycirclize/tree.py` & `pycirclize-1.4.0/src/pycirclize/tree.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/__init__.py` & `pycirclize-1.4.0/src/pycirclize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/dataset.py` & `pycirclize-1.4.0/src/pycirclize/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/example_data/images/python_logo.png` & `pycirclize-1.4.0/src/pycirclize/utils/example_data/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/alphabet.nwk` & `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/alphabet.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/large_example.nwk` & `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/large_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/example_data/trees/medium_example.nwk` & `pycirclize-1.4.0/src/pycirclize/utils/example_data/trees/medium_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/helper.py` & `pycirclize-1.4.0/src/pycirclize/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/src/pycirclize/utils/plot.py` & `pycirclize-1.4.0/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/conftest.py` & `pycirclize-1.4.0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,20 +59,42 @@
             ["E", "A", 20],
             ["E", "D", 6],
         ],
     )
 
 
 @pytest.fixture
+def radar_table_df() -> pd.DataFrame:
+    """Pandas radar table dataframe"""
+    return pd.DataFrame(
+        data=[
+            [80, 80, 80, 80, 80, 80],
+            [90, 95, 95, 30, 30, 80],
+            [60, 20, 20, 100, 90, 50],
+        ],
+        index=["Hero", "Warrior", "Wizard"],
+        columns=["HP", "ATK", "DEF", "SP.ATK", "SP.DEF", "SPD"],
+    )
+
+
+@pytest.fixture
 def csv_matrix_file(matrix_df: pd.DataFrame, tmp_path: Path) -> Path:
     """CSV matrix file fixture"""
     csv_matrix_file = tmp_path / "matrix.csv"
     matrix_df.to_csv(csv_matrix_file)
     return csv_matrix_file
 
 
 @pytest.fixture
 def tsv_matrix_file(matrix_df: pd.DataFrame, tmp_path: Path) -> Path:
     """TSV matrix file fixture"""
     tsv_matrix_file = tmp_path / "matrix.tsv"
     matrix_df.to_csv(tsv_matrix_file, sep="\t")
     return tsv_matrix_file
+
+
+@pytest.fixture
+def tsv_radar_table_file(radar_table_df: pd.DataFrame, tmp_path: Path) -> Path:
+    """TSV radar table file fixture"""
+    tsv_radar_table_file = tmp_path / "radar_table.tsv"
+    radar_table_df.to_csv(tsv_radar_table_file, sep="\t")
+    return tsv_radar_table_file
```

### Comparing `pycirclize-1.3.0/tests/parser/test_genbank.py` & `pycirclize-1.4.0/tests/parser/test_genbank.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     gbk = Genbank(gbk_file)
     seqid = "NC_000902.1"
     assert gbk.name == "enterobacteria_phage"
     max_genome_size = 60942
     assert gbk.range_size == max_genome_size
     assert gbk.genome_length == max_genome_size
     assert gbk.full_genome_length == max_genome_size
-    assert gbk.min_range == 0
-    assert gbk.max_range == max_genome_size
     assert gbk.get_seqid2size() == {seqid: max_genome_size}
 
 
 def test_parse_contig_genomes(prokaryote_testdata_dir: Path):
     """Test parse contig genomes"""
     gbk_file = prokaryote_testdata_dir / "mycoplasma_alvi.gbk.gz"
     gbk = Genbank(gbk_file)
@@ -27,27 +25,25 @@
         "NZ_JNJU01000002.1": 190782,
         "NZ_KL370824.1": 158240,
         "NZ_KL370825.1": 155515,
         "NZ_JNJU01000007.1": 67647,
         "NZ_JNJU01000008.1": 2683,
         "NZ_JNJU01000009.1": 1108,
     }
-    total_genome_size = sum(list(seqid2size.values()))
+    size_list = list(seqid2size.values())
 
     assert gbk.name == "mycoplasma_alvi"
-    assert gbk.range_size == total_genome_size
-    assert gbk.min_range == 0
-    assert gbk.max_range == total_genome_size
+    assert gbk.range_size == size_list[0]
     assert gbk.get_seqid2size() == seqid2size
 
-    seqid2cds_features = gbk.get_seqid2features(pseudogene=None)
+    seqid2cds_features = gbk.get_seqid2features()
     first_contig_cds_features = list(seqid2cds_features.values())[0]
     assert len(first_contig_cds_features) == 204
 
-    seqid2trna_features = gbk.get_seqid2features("tRNA", pseudogene=None)
+    seqid2trna_features = gbk.get_seqid2features("tRNA")
     first_contig_trna_features = list(seqid2trna_features.values())[0]
     assert len(first_contig_trna_features) == 12
 
 
 def test_calc_gc(prokaryote_testdata_dir: Path):
     """Test GCskew, GCcontent calculation"""
     gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
```

### Comparing `pycirclize-1.3.0/tests/parser/test_gff.py` & `pycirclize-1.4.0/tests/parser/test_gff.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     """Test parse complete genome"""
     gff_file = prokaryote_testdata_dir / "enterobacteria_phage.gff"
     gff = Gff(gff_file)
     seqid = "NC_000902.1"
     assert gff.target_seqid == seqid
     max_genome_size = 60942
     assert gff.range_size == max_genome_size
-    assert gff.min_range == 0
-    assert gff.max_range == max_genome_size
     assert gff.seq_region == (0, max_genome_size)
     assert gff.seqid_list == [seqid]
     assert gff.get_seqid2size() == {seqid: max_genome_size}
 
 
 @pytest.mark.parametrize(
     "gff_filename",
@@ -41,20 +39,18 @@
         "NZ_JNJU01000009.1": 1108,
     }
     seqid_list = list(seqid2size.keys())
     size_list = list(seqid2size.values())
 
     assert gff.target_seqid == list(seqid2size.keys())[0]
     assert gff.range_size == size_list[0]
-    assert gff.min_range == 0
-    assert gff.max_range == size_list[0]
     assert gff.seq_region == (0, size_list[0])
     assert gff.seqid_list == seqid_list
     assert gff.get_seqid2size() == seqid2size
 
-    seqid2cds_features = gff.get_seqid2features(pseudogene=None)
+    seqid2cds_features = gff.get_seqid2features()
     first_contig_cds_features = list(seqid2cds_features.values())[0]
     assert len(first_contig_cds_features) == 204
 
-    seqid2trna_features = gff.get_seqid2features("tRNA", pseudogene=None)
+    seqid2trna_features = gff.get_seqid2features("tRNA")
     first_contig_trna_features = list(seqid2trna_features.values())[0]
     assert len(first_contig_trna_features) == 12
```

### Comparing `pycirclize-1.3.0/tests/parser/test_matrix.py` & `pycirclize-1.4.0/tests/parser/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/parser/test_table.py` & `pycirclize-1.4.0/tests/parser/test_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import pandas as pd
 import pytest
 
-from pycirclize.parser import StackedBarTable
+from pycirclize.parser import RadarTable, StackedBarTable
 
 
 class TestStackedBarTable:
     """Test StackedBarTable Class"""
 
     @pytest.fixture
     def sb_table(self):
@@ -91,7 +91,33 @@
         track_r_lim: tuple[float, float],
         width: float,
         expected_r_lim_list: list[tuple[float, float]],
     ):
         """Test `calc_barh_r_lim_list()`"""
         r_lim_list = sb_table.calc_barh_r_lim_list(track_r_lim, width)
         assert r_lim_list == expected_r_lim_list
+
+
+class TestRaderTable:
+    """Test RadarTable Class"""
+
+    @pytest.fixture
+    def radar_table(self):
+        """Initialize radar table fixture"""
+        table_df = pd.DataFrame(
+            data=[
+                [80, 80, 80, 80, 80, 80],
+                [90, 95, 95, 30, 30, 80],
+                [60, 20, 20, 100, 90, 50],
+            ],
+            index=["Hero", "Warrior", "Wizard"],
+            columns=["HP", "ATK", "DEF", "SP.ATK", "SP.DEF", "SPD"],
+        )
+        return RadarTable(table_df)
+
+    def test_row_name2values(self, radar_table: RadarTable):
+        """Test `row_name2values()`"""
+        assert radar_table.row_name2values == dict(
+            Hero=[80, 80, 80, 80, 80, 80],
+            Warrior=[90, 95, 95, 30, 30, 80],
+            Wizard=[60, 20, 20, 100, 90, 50],
+        )
```

### Comparing `pycirclize-1.3.0/tests/test_circos.py` & `pycirclize-1.4.0/tests/test_circos.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/test_plot.py` & `pycirclize-1.4.0/tests/test_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,21 @@
         tick_kws=dict(labelsize=12, colors="red"),
     )
 
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
 
 
+def test_radar_chart_plot(fig_outfile: Path, tsv_radar_table_file: Path):
+    """Test radar chart plot"""
+    circos = Circos.radar_chart(tsv_radar_table_file, vmax=100, marker_size=6)
+    circos.savefig(fig_outfile)
+    assert fig_outfile.exists()
+
+
 def test_chord_diagram_plot(fig_outfile: Path, tsv_matrix_file: pd.DataFrame):
     """Test chord diagram plot"""
     circos = Circos.initialize_from_matrix(tsv_matrix_file)
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
```

### Comparing `pycirclize-1.3.0/tests/test_sector.py` & `pycirclize-1.4.0/tests/test_sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/test_track.py` & `pycirclize-1.4.0/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_chr.bed` & `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv` & `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv` & `pycirclize-1.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/prokaryote/enterobacteria_phage.gbk` & `pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/prokaryote/enterobacteria_phage.gff` & `pycirclize-1.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz` & `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz` & `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz` & `pycirclize-1.4.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/utils/test_dataset.py` & `pycirclize-1.4.0/tests/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/tests/utils/test_helper.py` & `pycirclize-1.4.0/tests/utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.3.0/PKG-INFO` & `pycirclize-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCirclize
-Version: 1.3.0
+Version: 1.4.0
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Dist: biopython (>=1.79)
+Requires-Dist: biopython (>=1.80)
 Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: numpy (>=1.21.1)
 Requires-Dist: pandas (>=1.3.5)
 Project-URL: Repository, https://github.com/moshi4/pyCirclize/
 Description-Content-Type: text/markdown
 
 # pyCirclize: Circular visualization in Python
@@ -68,14 +68,15 @@
 ## API Usage
 
 API usage is described in each of the following sections in the [document](https://moshi4.github.io/pyCirclize/).
 
 - [Getting Started](https://moshi4.github.io/pyCirclize/getting_started/)
 - [Plot API Example](https://moshi4.github.io/pyCirclize/plot_api_example/)
 - [Chord Diagram](https://moshi4.github.io/pyCirclize/chord_diagram/)
+- [Radar Chart](https://moshi4.github.io/pyCirclize/radar_chart/)
 - [Circos Plot (Genomics)](https://moshi4.github.io/pyCirclize/circos_plot/)
 - [Phylogenetic Tree](https://moshi4.github.io/pyCirclize/phylogenetic_tree/)
 - [Plot Tips](https://moshi4.github.io/pyCirclize/plot_tips/)
 
 ## Code Example
 
 ### 1. Circos Plot
@@ -147,16 +148,16 @@
 r_cds_track = sector.add_track((90, 95))
 r_cds_feats = gbk.extract_features("CDS", target_strand=-1)
 r_cds_track.genomic_features(r_cds_feats, plotstyle="arrow", fc="skyblue", lw=0.5)
 
 # Plot 'gene' qualifier label if exists
 labels, label_pos_list = [], []
 for feat in gbk.extract_features("CDS"):
-    start = int(str(feat.location.start))
-    end = int(str(feat.location.end))
+    start = int(feat.location.start)
+    end = int(feat.location.end)
     label_pos = (start + end) / 2
     gene_name = feat.qualifiers.get("gene", [None])[0]
     if gene_name is not None:
         labels.append(gene_name)
         label_pos_list.append(label_pos)
 f_cds_track.xticks(label_pos_list, labels, label_size=6, label_orientation="vertical")
 
@@ -245,21 +246,55 @@
     bbox_to_anchor=(0.5, 0.5),
 )
 fig.savefig("example04.png")
 ```
 
 ![example04.png](https://raw.githubusercontent.com/moshi4/pyCirclize/main/docs/images/example04.png)  
 
+### 5. Radar Chart
+
+```python
+from pycirclize import Circos
+import pandas as pd
+
+# Create RPG jobs parameter dataframe (3 jobs, 7 parameters)
+df = pd.DataFrame(
+    data=[
+        [80, 80, 80, 80, 80, 80, 80],
+        [90, 20, 95, 95, 30, 30, 80],
+        [60, 90, 20, 20, 100, 90, 50],
+    ],
+    index=["Hero", "Warrior", "Wizard"],
+    columns=["HP", "MP", "ATK", "DEF", "SP.ATK", "SP.DEF", "SPD"],
+)
+
+# Initialize Circos instance for radar chart plot
+circos = Circos.radar_chart(
+    df,
+    vmax=100,
+    marker_size=6,
+    grid_interval_ratio=0.2,
+)
+
+# Plot figure & set legend on upper right
+fig = circos.plotfig()
+_ = circos.ax.legend(loc="upper right", fontsize=10)
+fig.savefig("example05.png")
+```
+
+![example05.png](https://raw.githubusercontent.com/moshi4/pyCirclize/main/docs/images/example05.png)  
+
 ## Not Implemented Features
 
 List of features implemented in other Circos plotting tools but not yet implemented in pyCirclize.
 I may implement them when I feel like it.
 
 - Plot histogram
 - Plot boxplot
 - Plot violin
-- Label position auto adjustment
+- Plot curved text
+- Adjust overlap label position
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=moshi4/pyCirclize&type=Date)](https://star-history.com/#moshi4/pyCirclize&Date)
```

