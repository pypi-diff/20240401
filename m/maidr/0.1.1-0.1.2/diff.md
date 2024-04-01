# Comparing `tmp/maidr-0.1.1.tar.gz` & `tmp/maidr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maidr-0.1.1.tar", max compression
+gzip compressed data, was "maidr-0.1.2.tar", max compression
```

## Comparing `maidr-0.1.1.tar` & `maidr-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0    35823 2024-02-15 13:09:45.734648 maidr-0.1.1/LICENSE
--rw-r--r--   0        0        0      250 2024-03-06 15:50:46.392801 maidr-0.1.1/README.md
--rw-r--r--   0        0        0      194 2024-03-06 15:50:46.396273 maidr-0.1.1/maidr/__init__.py
--rw-r--r--   0        0        0        0 2024-02-15 13:10:02.927912 maidr-0.1.1/maidr/core/__init__.py
--rw-r--r--   0        0        0        0 2024-02-15 13:10:02.927972 maidr-0.1.1/maidr/core/enum/__init__.py
--rw-r--r--   0        0        0      488 2024-03-06 15:50:46.397012 maidr-0.1.1/maidr/core/enum/maidr_key.py
--rw-r--r--   0        0        0      257 2024-03-06 15:50:46.397419 maidr-0.1.1/maidr/core/enum/plot_type.py
--rw-r--r--   0        0        0     4151 2024-03-06 15:50:46.398066 maidr-0.1.1/maidr/core/figure_manager.py
--rw-r--r--   0        0        0     5753 2024-03-06 15:36:44.464647 maidr-0.1.1/maidr/core/maidr.py
--rw-r--r--   0        0        0     2538 2024-03-06 15:37:33.903881 maidr-0.1.1/maidr/core/maidr_plot_data.py
--rw-r--r--   0        0        0     2053 2024-03-06 15:50:46.398292 maidr-0.1.1/maidr/core/maidr_plot_data_factory.py
--rw-r--r--   0        0        0        0 2024-02-24 23:21:07.504868 maidr-0.1.1/maidr/core/plot/__init__.py
--rw-r--r--   0        0        0     4722 2024-03-06 15:36:44.465276 maidr-0.1.1/maidr/core/plot/bar_plot_data.py
--rw-r--r--   0        0        0     5645 2024-03-06 15:36:44.465445 maidr-0.1.1/maidr/core/plot/heat_plot_data.py
--rw-r--r--   0        0        0     4064 2024-03-06 15:50:46.398649 maidr-0.1.1/maidr/core/plot/hist_plot_data.py
--rw-r--r--   0        0        0     2022 2024-03-06 15:50:46.398885 maidr-0.1.1/maidr/core/plot/line_plot_data.py
--rw-r--r--   0        0        0        0 2024-02-20 13:51:08.380134 maidr-0.1.1/maidr/exception/__init__.py
--rw-r--r--   0        0        0     1063 2024-03-06 15:36:44.465928 maidr-0.1.1/maidr/exception/extraction_error.py
--rw-r--r--   0        0        0     3929 2024-03-06 15:50:46.399081 maidr-0.1.1/maidr/maidr.py
--rw-r--r--   0        0        0     1858 2024-03-06 16:16:01.470037 maidr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 maidr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-02-15 13:09:45.734648 maidr-0.1.2/LICENSE
+-rw-r--r--   0        0        0      540 2024-03-27 22:32:11.489094 maidr-0.1.2/README.md
+-rw-r--r--   0        0        0      281 2024-03-28 06:29:42.756287 maidr-0.1.2/maidr/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 13:10:02.927912 maidr-0.1.2/maidr/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 13:10:02.927972 maidr-0.1.2/maidr/core/enum/__init__.py
+-rw-r--r--   0        0        0      736 2024-03-28 18:12:39.091912 maidr-0.1.2/maidr/core/enum/maidr_key.py
+-rw-r--r--   0        0        0      213 2024-03-28 18:12:39.092215 maidr-0.1.2/maidr/core/enum/plot_type.py
+-rw-r--r--   0        0        0     2092 2024-04-01 13:45:39.108450 maidr-0.1.2/maidr/core/figure_manager.py
+-rw-r--r--   0        0        0     3268 2024-03-28 18:12:39.092787 maidr-0.1.2/maidr/core/maidr.py
+-rw-r--r--   0        0        0     1221 2024-03-28 18:12:39.093000 maidr-0.1.2/maidr/core/maidr_plot.py
+-rw-r--r--   0        0        0     1833 2024-04-01 13:45:39.110428 maidr-0.1.2/maidr/core/maidr_plot_factory.py
+-rw-r--r--   0        0        0        0 2024-03-28 18:12:39.093304 maidr-0.1.2/maidr/core/mixin/__init__.py
+-rw-r--r--   0        0        0     2182 2024-03-28 18:12:39.093891 maidr-0.1.2/maidr/core/mixin/extractor_mixin.py
+-rw-r--r--   0        0        0      623 2024-03-28 18:12:39.094128 maidr-0.1.2/maidr/core/mixin/merger_mixin.py
+-rw-r--r--   0        0        0        0 2024-03-28 18:12:39.094163 maidr-0.1.2/maidr/core/plot/__init__.py
+-rw-r--r--   0        0        0     1893 2024-03-28 18:12:39.094402 maidr-0.1.2/maidr/core/plot/bar_plot.py
+-rw-r--r--   0        0        0     5194 2024-04-01 13:58:29.398275 maidr-0.1.2/maidr/core/plot/box_plot.py
+-rw-r--r--   0        0        0     2147 2024-03-28 18:12:39.094720 maidr-0.1.2/maidr/core/plot/grouped_bar_plot.py
+-rw-r--r--   0        0        0     2254 2024-04-01 16:09:36.639507 maidr-0.1.2/maidr/core/plot/heat_plot.py
+-rw-r--r--   0        0        0     1531 2024-03-28 18:12:39.095188 maidr-0.1.2/maidr/core/plot/hist_plot.py
+-rw-r--r--   0        0        0     1090 2024-03-28 18:12:39.095407 maidr-0.1.2/maidr/core/plot/line_plot.py
+-rw-r--r--   0        0        0     1265 2024-03-28 18:12:39.095548 maidr-0.1.2/maidr/core/plot/scatter_plot.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:51:08.380134 maidr-0.1.2/maidr/exception/__init__.py
+-rw-r--r--   0        0        0     1063 2024-03-27 13:21:36.669442 maidr-0.1.2/maidr/exception/extraction_error.py
+-rw-r--r--   0        0        0     4496 2024-04-01 13:58:29.393937 maidr-0.1.2/maidr/maidr.py
+-rw-r--r--   0        0        0     1855 2024-04-01 16:14:04.444635 maidr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 maidr-0.1.2/PKG-INFO
```

### Comparing `maidr-0.1.1/LICENSE` & `maidr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maidr-0.1.1/maidr/core/maidr_plot_data_factory.py` & `maidr-0.1.2/maidr/core/maidr_plot_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from matplotlib.axes import Axes
 
 from maidr.core.enum.plot_type import PlotType
-from maidr.core.maidr_plot_data import MaidrPlotData
-from maidr.core.plot.bar_plot_data import BarPlotData
-from maidr.core.plot.heat_plot_data import HeatPlotData
-from maidr.core.plot.hist_plot_data import HistPlotData
-from maidr.core.plot.line_plot_data import LinePlotData
+from maidr.core.maidr_plot import MaidrPlot
+from maidr.core.plot.bar_plot import BarPlot
+from maidr.core.plot.box_plot import BoxPlot
+from maidr.core.plot.heat_plot import HeatPlot
+from maidr.core.plot.hist_plot import HistPlot
+from maidr.core.plot.line_plot import LinePlot
+from maidr.core.plot.scatter_plot import ScatterPlot
+from maidr.core.plot.grouped_bar_plot import GroupedBarPlot
 
 
-class MaidrPlotDataFactory:
+class MaidrPlotFactory:
     """
     A factory for creating instances of `MaidrPlotData` based on the plot type.
 
     This factory is responsible for instantiating the correct `MaidrPlotData` subclass
     based on the provided plot type.
 
     Warnings
@@ -25,40 +28,24 @@
     --------
     MaidrPlotData : The base class for MAIDR plot data objects. It defines the common
         interface for all MAIDR data classes.
     PlotType : An enumeration that defines the supported types of plots within MAIDR.
     """
 
     @staticmethod
-    def create(ax: Axes, plot_type: PlotType) -> MaidrPlotData:
-        """
-        Creates an instance of `MaidrPlotData` based on the provided plot type.
-
-        Parameters
-        ----------
-        ax : Axes
-            The axes object on which the plot is displayed.
-        plot_type : PlotType
-            The type of plot.
-
-        Returns
-        -------
-        MaidrPlotData
-            An instance of the `MaidrPlotData` subclass corresponding to the specified
-            `plot_type`.
-
-        Raises
-        ------
-        TypeError
-            If the provided `plot_type` does not have a corresponding `MaidrPlotData`
-            subclass.
-        """
+    def create(ax: Axes, plot_type: PlotType, **kwargs) -> MaidrPlot:
         if PlotType.BAR == plot_type:
-            return BarPlotData(ax)
+            return BarPlot(ax)
+        elif PlotType.BOX == plot_type:
+            return BoxPlot(ax, **kwargs)
         elif PlotType.HEAT == plot_type:
-            return HeatPlotData(ax)
+            return HeatPlot(ax)
         elif PlotType.HIST == plot_type:
-            return HistPlotData(ax)
+            return HistPlot(ax)
         elif PlotType.LINE == plot_type:
-            return LinePlotData(ax)
+            return LinePlot(ax)
+        elif PlotType.SCATTER == plot_type:
+            return ScatterPlot(ax)
+        elif PlotType.DODGED == plot_type or PlotType.STACKED == plot_type:
+            return GroupedBarPlot(ax, plot_type)
         else:
             raise TypeError(f"Unsupported plot type: {plot_type}")
```

### Comparing `maidr-0.1.1/maidr/core/plot/line_plot_data.py` & `maidr-0.1.2/maidr/core/plot/grouped_bar_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 from __future__ import annotations
 
 from matplotlib.axes import Axes
-from matplotlib.lines import Line2D
+from matplotlib.container import BarContainer
 
 from maidr.core.enum.maidr_key import MaidrKey
 from maidr.core.enum.plot_type import PlotType
-from maidr.core.maidr_plot_data import MaidrPlotData
+from maidr.core.maidr_plot import MaidrPlot
+from maidr.core.mixin.extractor_mixin import (
+    LevelExtractorMixin,
+    ContainerExtractorMixin,
+)
+from maidr.core.mixin.merger_mixin import DictMergerMixin
 from maidr.exception.extraction_error import ExtractionError
 
 
-class LinePlotData(MaidrPlotData):
-    last_extracted_id = -1
-
-    def __init__(self, axes: Axes) -> None:
-        super().__init__(axes, PlotType.LINE)
-
-    def _extract_maidr_data(self) -> dict:
-        plt_type = self.type.value
-        ax = self.axes
-
-        maidr = {
-            MaidrKey.TYPE.value: plt_type,
-            MaidrKey.TITLE.value: ax.get_title(),
-            MaidrKey.AXES.value: {
-                MaidrKey.X.value: {
-                    MaidrKey.LABEL.value: ax.get_xlabel(),
-                },
-                MaidrKey.Y.value: {
-                    MaidrKey.LABEL.value: ax.get_ylabel(),
-                },
+class GroupedBarPlot(
+    MaidrPlot, ContainerExtractorMixin, LevelExtractorMixin, DictMergerMixin
+):
+    def __init__(self, ax: Axes, plot_type: PlotType) -> None:
+        super().__init__(ax, plot_type)
+
+    def _extract_axes_data(self) -> dict:
+        base_ax_schema = super()._extract_axes_data()
+        grouped_ax_schema = {
+            MaidrKey.X.value: {
+                MaidrKey.LEVEL.value: self.extract_level(self.ax, MaidrKey.X),
+            },
+            MaidrKey.FILL.value: {
+                MaidrKey.LABEL.value: "Fill",
+                MaidrKey.LEVEL.value: self.extract_level(self.ax, MaidrKey.FILL),
             },
-            MaidrKey.DATA.value: self.__extract_data(),
         }
+        return self.merge_dict(base_ax_schema, grouped_ax_schema)
 
-        return maidr
-
-    def __extract_data(self) -> list[dict]:
-        ax = self.axes
-        plot = None
-        data = None
-
-        if isinstance(ax, Axes):
-            self.last_extracted_id += 1
-            plot = LinePlotData.__extract_line(ax, self.last_extracted_id)
-        if isinstance(plot, Line2D):
-            data = LinePlotData.__extract_line_data(plot)
+    def _extract_plot_data(self):
+        plot = self.extract_container(self.ax, BarContainer, include_all=True)
+        data = self.__extract_grouped_bar_data(plot)
 
         if data is None:
             raise ExtractionError(self.type, plot)
 
         return data
 
-    @staticmethod
-    def __extract_line_data(plot: Line2D) -> list[dict] | None:
+    def __extract_grouped_bar_data(
+        self, plot: list[BarContainer] | None
+    ) -> list[dict] | None:
         if plot is None:
             return None
 
-        return [
-            {
-                MaidrKey.X.value: float(x),
-                MaidrKey.Y.value: float(y),
-            }
-            for x, y in plot.get_xydata()
-        ]
-
-    @staticmethod
-    def __extract_line(plot: Axes, line_id: int) -> Line2D | None:
-        if plot is None or plot.get_lines() is None:
-            return None
+        x_level = self.extract_level(self.ax)
+        data = list()
+
+        for container in plot:
+            if len(x_level) != len(container.patches):
+                return None
+
+            for x, y in zip(x_level, container.patches):
+                data.append(
+                    {
+                        MaidrKey.X.value: x,
+                        MaidrKey.FILL.value: container.get_label(),
+                        MaidrKey.Y.value: float(y.get_height()),
+                    }
+                )
 
-        return plot.get_lines()[line_id]
+        return data
```

### Comparing `maidr-0.1.1/maidr/exception/extraction_error.py` & `maidr-0.1.2/maidr/exception/extraction_error.py`

 * *Files identical despite different names*

### Comparing `maidr-0.1.1/pyproject.toml` & `maidr-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 keywords = ["accessibility", "visualization", "sonification", "braille", "tactile", "multimodal", "data representation", "blind", "low vision", "visual impairments"]
 license = "GPL-3.0-or-later"
 authors = [
   "JooYoung Seo <jseo1005@illinois.edu>",
   "Saairam Venkatesh <saairam2@illinois.edu>"
 ]
-version = "0.1.1"
+version = "0.1.2"
 classifiers = [
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: Financial and Insurance Industry",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Healthcare Industry",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -28,20 +28,20 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/xability/py_maidr"
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
-matplotlib = "^3.7.1"
-numpy = "^1.24.3"
-seaborn = "^0.13.2"
-lxml = "^5.1.0"
-htmltools = ">=0.5.1"
+python = ">=3.8"
+matplotlib = ">=3.7"
+numpy = ">=1.24"
+seaborn = ">=0.13"
+lxml = ">=5.1.0"
+htmltools = ">=0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 sphinx = "^7.0.1"
 pre-commit = "^3.3.2"
 pytest = "^7.3.2"
```

### Comparing `maidr-0.1.1/PKG-INFO` & `maidr-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maidr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multimodal Access and Interactive Data Representations
 License: GPL-3.0-or-later
 Keywords: accessibility,visualization,sonification,braille,tactile,multimodal,data representation,blind,low vision,visual impairments
 Author: JooYoung Seo
 Author-email: jseo1005@illinois.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -23,21 +23,29 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Dist: htmltools (>=0.5.1)
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: htmltools (>=0.5)
+Requires-Dist: lxml (>=5.1.0)
+Requires-Dist: matplotlib (>=3.7)
+Requires-Dist: numpy (>=1.24)
+Requires-Dist: seaborn (>=0.13)
 Description-Content-Type: text/markdown
 
+<div align="center">
+
+<img src="https://github.com/xability/maidr/blob/main/logo/logo.svg" width="350px" alt="A stylized MAIDR logo, with curved characters for M A, a hand pointing for an I, the D character, and R represented in braille."/>
+
+<hr style="color:transparent" />
+<br />
+</div>
+
 # py-maidr
 
 Python binder for maidr library
 
 ## Install and Upgrade
 
 ``` sh
```

