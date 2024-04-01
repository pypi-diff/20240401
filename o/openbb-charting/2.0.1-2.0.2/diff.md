# Comparing `tmp/openbb_charting-2.0.1.tar.gz` & `tmp/openbb_charting-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_charting-2.0.1.tar", max compression
+gzip compressed data, was "openbb_charting-2.0.2.tar", max compression
```

## Comparing `openbb_charting-2.0.1.tar` & `openbb_charting-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     5148 2024-02-23 17:14:57.379013 openbb_charting-2.0.1/README.md
--rw-r--r--   0        0        0     6881 2024-02-28 09:43:45.470704 openbb_charting-2.0.1/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-02-23 17:14:57.379426 openbb_charting-2.0.1/openbb_charting/builder.py
--rw-r--r--   0        0        0     5117 2024-02-23 17:14:57.379504 openbb_charting-2.0.1/openbb_charting/charting_router.py
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.379570 openbb_charting-2.0.1/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-02-23 17:14:57.381108 openbb_charting-2.0.1/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-02-23 17:14:57.389057 openbb_charting-2.0.1/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17115 2024-02-23 17:14:57.389309 openbb_charting-2.0.1/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-02-23 17:14:57.389418 openbb_charting-2.0.1/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.389490 openbb_charting-2.0.1/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     7156 2024-02-23 17:14:57.389586 openbb_charting-2.0.1/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2422 2024-02-23 17:14:57.389664 openbb_charting-2.0.1/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58652 2024-02-23 17:14:57.391344 openbb_charting-2.0.1/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228603 2024-02-23 17:14:57.405576 openbb_charting-2.0.1/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.405769 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     6741 2024-02-23 17:14:57.405891 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12212 2024-02-23 17:14:57.405987 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8398 2024-02-23 17:14:57.406107 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    18829 2024-02-23 17:14:57.406200 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3240 2024-02-23 17:14:57.406299 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5661 2024-02-23 17:14:57.406371 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6817 2024-02-23 17:14:57.406429 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3510 2024-02-23 17:14:57.406494 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    22040 2024-02-28 09:43:45.470865 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1379 2024-02-23 17:14:57.406667 openbb_charting-2.0.1/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   857302 2024-02-23 17:14:57.412167 openbb_charting-2.0.1/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2252 2024-02-23 17:14:57.412316 openbb_charting-2.0.1/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0     3204 2024-02-23 17:14:57.412497 openbb_charting-2.0.1/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0    23603 2024-02-23 17:14:57.412571 openbb_charting-2.0.1/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-02-23 17:14:57.412655 openbb_charting-2.0.1/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-02-23 17:14:57.412751 openbb_charting-2.0.1/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0      600 2024-02-23 17:14:57.412818 openbb_charting-2.0.1/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0      661 2024-03-11 20:00:57.405520 openbb_charting-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 openbb_charting-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5148 2024-03-13 16:36:51.588316 openbb_charting-2.0.2/README.md
+-rw-r--r--   0        0        0     7652 2024-03-19 14:52:38.486399 openbb_charting-2.0.2/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-03-13 16:36:51.588853 openbb_charting-2.0.2/openbb_charting/builder.py
+-rw-r--r--   0        0        0    16542 2024-03-28 17:15:52.353876 openbb_charting-2.0.2/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.589049 openbb_charting-2.0.2/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-03-13 16:36:51.589844 openbb_charting-2.0.2/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-03-13 16:36:51.600822 openbb_charting-2.0.2/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17390 2024-03-28 17:15:52.354340 openbb_charting-2.0.2/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-03-13 16:36:51.601274 openbb_charting-2.0.2/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.601317 openbb_charting-2.0.2/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     7156 2024-03-13 16:36:51.601401 openbb_charting-2.0.2/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2422 2024-03-13 16:36:51.601472 openbb_charting-2.0.2/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58414 2024-03-22 20:01:30.635138 openbb_charting-2.0.2/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228603 2024-03-13 16:36:51.617857 openbb_charting-2.0.2/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.618060 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7101 2024-03-28 17:15:52.355110 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12351 2024-03-28 17:15:52.357139 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8398 2024-03-13 16:36:51.618397 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    18829 2024-03-13 16:36:51.618492 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3240 2024-03-13 16:36:51.618625 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5661 2024-03-13 16:36:51.618717 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6817 2024-03-13 16:36:51.618778 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3510 2024-03-13 16:36:51.618852 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    22181 2024-03-28 17:15:52.357572 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1379 2024-03-13 16:36:51.619542 openbb_charting-2.0.2/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   857302 2024-03-13 16:36:51.622245 openbb_charting-2.0.2/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2252 2024-03-13 16:36:51.622357 openbb_charting-2.0.2/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0     3666 2024-03-19 14:52:38.486656 openbb_charting-2.0.2/openbb_charting/query_params.py
+-rw-r--r--   0        0        0     3204 2024-03-13 16:36:51.622614 openbb_charting-2.0.2/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0    23603 2024-03-13 16:36:51.622688 openbb_charting-2.0.2/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-03-13 16:36:51.622759 openbb_charting-2.0.2/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-03-13 16:36:51.622823 openbb_charting-2.0.2/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0      600 2024-03-13 16:36:51.622881 openbb_charting-2.0.2/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0      661 2024-04-01 14:21:50.494407 openbb_charting-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 openbb_charting-2.0.2/PKG-INFO
```

### Comparing `openbb_charting-2.0.1/README.md` & `openbb_charting-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/__init__.py` & `openbb_charting-2.0.2/openbb_charting/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
-    Tuple,
     Union,
 )
 
 import numpy as np
 import pandas as pd
 from openbb_core.app.model.charts.chart import Chart
 from openbb_core.app.model.extension import Extension
 from openbb_core.app.utils import basemodel_to_df, convert_to_basemodel
 from openbb_core.provider.abstract.data import Data
 
 from openbb_charting import charting_router
-from openbb_charting.core.to_chart import ChartIndicators, OpenBBFigure, to_chart
+from openbb_charting.core.to_chart import ChartIndicators, to_chart
 from openbb_charting.utils.helpers import get_charting_functions
 
 ext = Extension(name="charting")
 
 
 @ext.obbject_accessor
 class Charting:
@@ -45,16 +44,16 @@
         """Initialize Charting extension."""
         # pylint: disable=import-outside-toplevel
         from openbb_core.app.model.charts.charting_settings import ChartingSettings
         from openbb_core.app.model.obbject import OBBject
 
         self._obbject: OBBject = obbject
         self._charting_settings = ChartingSettings(
-            user_settings=self._obbject._user_settings,
-            system_settings=self._obbject._system_settings,
+            user_settings=self._obbject._user_settings,  # type: ignore
+            system_settings=self._obbject._system_settings,  # type: ignore
         )
         self._handle_backend()
 
     @classmethod
     def indicators(cls):
         """Returns a list of the available indicators."""
         return ChartIndicators.get_available_indicators()
@@ -87,15 +86,17 @@
         if (
             hasattr(self._obbject, "_standard_params")
             and self._obbject._standard_params  # pylint: disable=protected-access
         ):
             kwargs["standard_params"] = (
                 self._obbject._standard_params.__dict__  # pylint: disable=protected-access
             )
-
+        kwargs["provider"] = self._obbject.provider  # pylint: disable=protected-access
+        kwargs["extra"] = self._obbject.extra  # pylint: disable=protected-access
+        kwargs["warnings"] = self._obbject.warnings  # pylint: disable=protected-access
         fig, content = charting_function(**kwargs)
         self._obbject.chart = Chart(
             fig=fig, content=content, format=charting_router.CHART_FORMAT
         )
         if render:
             fig.show(**kwargs)
 
@@ -181,21 +182,33 @@
             else None
         )
         data_as_df: pd.DataFrame = (
             basemodel_to_df(convert_to_basemodel(data), index=index)
             if has_data
             else self._obbject.to_dataframe()
         )
-        fig, content = to_chart(
-            data_as_df,
-            indicators=indicators,
-            symbol=symbol,
-            candles=candles,
-            volume=volume,
-            prepost=prepost,
-            volume_ticks_x=volume_ticks_x,
-        )
-        self._obbject.chart = Chart(
-            fig=fig, content=content, format=charting_router.CHART_FORMAT
-        )
-        if render:
-            fig.show(**kwargs)
+        if "date" in data_as_df.columns:
+            data_as_df = data_as_df.set_index("date")
+        try:
+            fig, content = to_chart(
+                data_as_df,
+                indicators=indicators,
+                symbol=symbol,
+                candles=candles,
+                volume=volume,
+                prepost=prepost,
+                volume_ticks_x=volume_ticks_x,
+            )
+            self._obbject.chart = Chart(
+                fig=fig, content=content, format=charting_router.CHART_FORMAT
+            )
+            if render:
+                fig.show(**kwargs)
+
+        except Exception:
+            try:
+                if has_data:
+                    self.show(data=data_as_df, symbol=symbol, render=render, **kwargs)
+                else:
+                    self.show(**kwargs)
+            except Exception as e:
+                raise RuntimeError("Could not create chart from the OBBject.") from e
```

### Comparing `openbb_charting-2.0.1/openbb_charting/builder.py` & `openbb_charting-2.0.2/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/assets/Terminal_icon.png` & `openbb_charting-2.0.2/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_charting-2.0.2/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/backend.py` & `openbb_charting-2.0.2/openbb_charting/core/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,14 @@
 
     def get_json_update(
         self,
         cmd_loc: Optional[str] = None,
         theme: Optional[str] = None,
     ) -> dict:
         """Get the json update for the backend."""
-
         posthog: Dict[str, Any] = dict(collect_logs=self.charting_settings.log_collect)
         if (
             self.charting_settings.log_collect
             and self.charting_settings.user_uuid
             and not self.logged_in
         ):
             self.logged_in = True
@@ -218,14 +217,19 @@
             json_data=json_data,
             export_image=export_image,
             **self.get_kwargs(command_location),
         )
         self.send_outgoing(outgoing)
 
         if export_image and isinstance(export_image, Path):
+            if self.loop.is_closed():  # type: ignore[has-type]
+                # Create a new event loop
+                self.loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(self.loop)
+
             self.loop.run_until_complete(self.process_image(export_image))
 
     async def process_image(self, export_image: Path):
         """Check if the image has been exported to the path."""
         pdf = export_image.suffix == ".pdf"
         img_path = export_image.resolve()
 
@@ -503,20 +507,22 @@
 # To avoid having plotly.js in the repo, we download it if it's not present
 if not PLOTLYJS_PATH.exists() and not JUPYTER_NOTEBOOK:
     # We run this in a thread so we don't block the main thread
     Thread(target=asyncio.run, args=(download_plotly_js(),)).start()
 
 
 def create_backend(charting_settings: Optional["ChartingSettings"] = None):
+    """Create the backend."""
     # # pylint: disable=import-outside-toplevel
     from openbb_core.app.model.charts.charting_settings import ChartingSettings
 
     charting_settings = charting_settings or ChartingSettings()
     global BACKEND  # pylint: disable=W0603 # noqa
     if BACKEND is None:
         BACKEND = Backend(charting_settings)
 
 
 def get_backend() -> Backend:
+    """Get the backend instance."""
     if BACKEND is None:
         raise ValueError("Backend not created")
     return BACKEND
```

### Comparing `openbb_charting-2.0.1/openbb_charting/core/chart_style.py` & `openbb_charting-2.0.2/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/config/openbb_styles.py` & `openbb_charting-2.0.2/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/dummy_backend.py` & `openbb_charting-2.0.2/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/openbb_figure.py` & `openbb_charting-2.0.2/openbb_charting/core/openbb_figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,19 +919,15 @@
 
                 # We send the figure to the backend to be displayed
                 return self._backend.send_figure(self, export_image)
             except Exception as e:
                 # If the backend fails, we just show the figure normally
                 # This is a very rare case, but it's better to have a fallback
 
-                if getattr(self._charting_settings, "debug_mode", False):
-                    warn(f"Failed to show figure with backend: {e}")
-                warn(
-                    f"Failed to show figure with backend: {e}"
-                )  # remove this line when the above lines are figured out
+                warn(f"Failed to show figure with backend. {e}")
 
                 # We check if any figures were initialized before the backend failed
                 # If so, we show them with the default plotly backend
                 queue = self._backend.get_pending()
                 for pending in queue:
                     data = json.loads(pending).get("json_data", {})
                     if data.get("layout", {}):
```

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly.html` & `openbb_charting-2.0.2/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/base.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from typing import Any, Callable, Dict, Iterator, List, Optional, Type
+"""Base class for charting plugins."""
+
+from typing import Any, Callable, Dict, Iterator, List, Optional, Type, Union
 
 import pandas as pd
 
 from .data_classes import ChartIndicators, TAIndicator
 
 
 def columns_regex(df_ta: pd.DataFrame, name: str) -> List[str]:
-    """Return columns that match regex name"""
+    """Return columns that match regex name."""
     column_name = df_ta.filter(regex=rf"{name}(?=[^\d]|$)").columns.tolist()
 
     return column_name
 
 
 class Indicator:
     """Class for technical indicator."""
@@ -22,27 +24,29 @@
         **attrs: Any,
     ) -> None:
         self.func = func
         self.name = name
         self.attrs = attrs
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        """Call the indicator function."""
         return self.func(*args, **kwargs)
 
 
 class PluginMeta(type):
     """Metaclass for all Plotly plugins."""
 
     __indicators__: List[Indicator] = []
     __static_methods__: list = []
     __ma_mode__: List[str] = []
     __inchart__: List[str] = []
     __subplots__: List[str] = []
 
     def __new__(mcs: Type["PluginMeta"], *args: Any, **kwargs: Any) -> "PluginMeta":
+        """Create a new instance of the class."""
         name, bases, attrs = args
         indicators: Dict[str, Indicator] = {}
         cls_attrs: Dict[str, list] = {
             "__ma_mode__": [],
             "__inchart__": [],
             "__subplots__": [],
         }
@@ -72,42 +76,44 @@
         new_cls.__ma_mode__ = list(set(cls_attrs["__ma_mode__"]))
         new_cls.__inchart__ = list(set(cls_attrs["__inchart__"]))
         new_cls.__subplots__ = list(set(cls_attrs["__subplots__"]))
 
         return new_cls
 
     def __iter__(cls: Type["PluginMeta"]) -> Iterator[Indicator]:  # type: ignore
+        """Iterate over the indicators."""
         return iter(cls.__indicators__)
 
     # pylint: disable=unused-argument
     def __init__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
 
 class PltTA(metaclass=PluginMeta):
     """The base class that all Plotly plugins must inherit from."""
 
     indicators: ChartIndicators
     intraday: bool = False
-    df_stock: pd.DataFrame
-    df_ta: pd.DataFrame
+    df_stock: Union[pd.DataFrame, pd.Series]
+    df_ta: Optional[pd.DataFrame] = None
     df_fib: pd.DataFrame
     close_column: Optional[str] = "close"
-    params: Dict[str, TAIndicator] = {}
+    params: Optional[Dict[str, TAIndicator]] = {}
     inchart_colors: List[str] = []
     show_volume: bool = True
 
     __static_methods__: list = []
     __indicators__: List[Indicator] = []
     __ma_mode__: List[str] = []
     __inchart__: List[str] = []
     __subplots__: List[str] = []
 
     # pylint: disable=unused-argument
     def __new__(cls, *args: Any, **kwargs: Any) -> "PltTA":
+        """Create a new instance of the class."""
         if cls is PltTA:
             raise TypeError("Can't instantiate abstract class Plugin directly")
         self = super().__new__(cls)
 
         static_methods = cls.__static_methods__
         indicators = cls.__indicators__
 
@@ -128,22 +134,23 @@
             ] and value not in getattr(self, attr):
                 getattr(self, attr).extend(value)
 
         return self
 
     @property
     def ma_mode(self) -> List[str]:
+        """Moving average mode."""
         return list(set(self.__ma_mode__))
 
     @ma_mode.setter
     def ma_mode(self, value: List[str]):
         self.__ma_mode__ = value
 
     def add_plugins(self, plugins: List["PltTA"]) -> None:
-        """Add plugins to current instance"""
+        """Add plugins to current instance."""
         for plugin in plugins:
             for item in plugin.__indicators__:
                 # pylint: disable=unnecessary-dunder-call
                 if not hasattr(self, item.name):
                     setattr(self, item.name, item.func.__get__(self, type(self)))
                     self.__indicators__.append(item)
 
@@ -157,28 +164,29 @@
                     "__ma_mode__",
                     "__inchart__",
                     "__subplots__",
                 ] and value not in getattr(self, attr):
                     getattr(self, attr).extend(value)
 
     def remove_plugins(self, plugins: List["PltTA"]) -> None:
-        """Remove plugins from current instance"""
+        """Remove plugins from current instance."""
         for plugin in plugins:
             for item in plugin.__indicators__:
                 delattr(self, item.name)
                 self.__indicators__.remove(item)
 
             for static_method in plugin.__static_methods__:
                 delattr(self, static_method)
 
     def __iter__(self) -> Iterator[Indicator]:
+        """Iterate over the indicators."""
         return iter(self.__indicators__)
 
     def get_float_precision(self) -> str:
-        """Returns f-string precision format"""
+        """Returns f-string precision format."""
         price = self.df_stock[self.close_column].tail(1).values[0]
         float_precision = (
             ",.2f" if price > 1.10 else "" if len(str(price)) < 8 else ".6f"
         )
         return float_precision
```

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,18 +63,14 @@
         "wma",
         "hma",
         "zlma",
         "rma",
     ]
     args: List[Arguments]
 
-    def __post_init__(self):
-        """Post init."""
-        self.args = [Arguments(**arg) for arg in self.args]
-
     def __iter__(self):
         """Return iterator."""
         return iter(self.args)
 
     def get_args(self, label: str) -> Union[Arguments, None]:
         """Return arguments by label."""
         output = None
@@ -94,22 +90,14 @@
 
 @dataclass(**datacls_kwargs)
 class ChartIndicators:
     """Chart technical analysis indicators."""
 
     indicators: Optional[List[TAIndicator]] = None
 
-    def __post_init__(self):
-        """Post init."""
-        self.indicators = (
-            [TAIndicator(**indicator) for indicator in self.indicators]
-            if self.indicators
-            else []
-        )
-
     def get_indicator(self, name: str) -> Union[TAIndicator, None]:
         """Return indicator with given name."""
         output = None
         for indicator in self.indicators:  # type: ignore
             if indicator.name == name:
                 output = indicator
         return output
@@ -161,29 +149,51 @@
                 output[opt] = self.get_indicator_args(name, opt)
 
         return output
 
     @staticmethod
     def get_available_indicators() -> Tuple[str, ...]:
         """Return tuple of available indicators."""
-        return list(
+        return tuple(
             TAIndicator.__annotations__["name"].__args__  # pylint: disable=E1101
         )
 
     @classmethod
-    def from_dict(cls, indicators: Dict[str, Dict[str, Any]]) -> "ChartIndicators":
-        """Return ChartIndicators from dictionary."""
-        data = []
-        for indicator in indicators:
-            args = []
-            for arg in indicators[indicator]:
-                args.append({"label": arg, "values": indicators[indicator][arg]})
-            data.append({"name": indicator, "args": args})
-
-        return cls(indicators=data)  # type: ignore
+    def from_dict(
+        cls, indicators: Dict[str, Dict[str, List[Dict[str, Any]]]]
+    ) -> "ChartIndicators":
+        """Return ChartIndicators from dictionary.
+
+        Example
+        -------
+        ChartIndicators.from_dict(
+            {
+                "ad": {
+                    "args": [
+                        {
+                            "label": "AD_LABEL",
+                            "values": [1, 2, 3],
+                        }
+                    ]
+                }
+            }
+        )
+        """
+        return cls(
+            indicators=[
+                TAIndicator(
+                    name=name,  # type: ignore[arg-type]
+                    args=[
+                        Arguments(label=label, values=values)
+                        for label, values in args.items()
+                    ],
+                )
+                for name, args in indicators.items()
+            ]
+        )
 
     def to_dataframe(
         self, df_ta: pd.DataFrame, ma_mode: Optional[List[str]] = None
     ) -> pd.DataFrame:
         """Calculate technical analysis indicators and return dataframe."""
         output = df_ta.copy()
         if not output.empty and self.indicators:
```

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     >>> fig2 = ta.plot(df2)
     >>> fig.show()
     >>> fig2.show()
     """
 
     inchart_colors: List[str] = []
     plugins: List[Type[PltTA]] = []
-    df_ta: pd.DataFrame = None
+    df_ta: Optional[pd.DataFrame] = None
     close_column: Optional[str] = "close"
     has_volume: bool = True
     show_volume: bool = True
     prepost: bool = False
     charting_settings: Optional["ChartingSettings"] = None
     theme: Optional[ChartStyle] = None
 
@@ -108,19 +108,19 @@
         cls.inchart_colors = cls.theme.get_colors()
 
         global PLOTLY_TA  # pylint: disable=global-statement # noqa
         if PLOTLY_TA is None:
             # Creates the instance of the class and loads the plugins
             # We set the global variable to the instance of the class so that
             # the plugins are only loaded once
-            PLOTLY_TA = super().__new__(cls)
-            PLOTLY_TA._locate_plugins(
+            PLOTLY_TA = super().__new__(cls)  # type: ignore[attr-defined, assignment]
+            PLOTLY_TA._locate_plugins(  # type: ignore[attr-defined]
                 getattr(cls.charting_settings, "debug_mode", False)
             )
-            PLOTLY_TA.add_plugins(PLOTLY_TA.plugins)
+            PLOTLY_TA.add_plugins(PLOTLY_TA.plugins)  # type: ignore[attr-defined, assignment]
 
         return PLOTLY_TA
 
     def __init__(self, *args, **kwargs):
         """Method is overridden to do nothing, except to clear the internal data structures."""
         if not args and not kwargs:
             self._clear_data()
@@ -176,15 +176,15 @@
         volume_ticks_x: int = 7,
     ) -> OpenBBFigure:
         """Method should not be called directly. Use the PlotlyTA.plot() static method instead."""
         if isinstance(df_stock, pd.Series):
             df_stock = df_stock.to_frame()
 
         if not isinstance(indicators, ChartIndicators):
-            indicators = ChartIndicators.from_dict(indicators or dict(dict()))
+            indicators = ChartIndicators.from_dict(indicators or {})
 
         # Apply to_datetime to the index in a way that handles daylight savings.
         df_stock.loc[:, "date"] = df_stock.index  # type: ignore
         df_stock["date"] = df_stock["date"].apply(pd.to_datetime)
         df_stock.index = df_stock["date"]  # type: ignore
         df_stock.drop(columns=["date"], inplace=True)
 
@@ -285,15 +285,15 @@
                     and obj != PlotlyTA.__class__
                 ) and obj not in PlotlyTA.plugins:
                     PlotlyTA.plugins.append(obj)
 
     def _clear_data(self):
         """Clear and reset all data to default values."""
         self.df_stock = None
-        self.indicators = {}
+        self.indicators = ChartIndicators.from_dict({})
         self.params = None
         self.intraday = False
         self.show_volume = True
 
     def calculate_indicators(self):
         """Return dataframe with all indicators."""
         return self.indicators.to_dataframe(self.df_stock.copy(), self.ma_mode)
```

### Comparing `openbb_charting-2.0.1/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_charting-2.0.2/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/table.html` & `openbb_charting-2.0.2/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/core/to_chart.py` & `openbb_charting-2.0.2/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_charting-2.0.2/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/styles/default/light.pltstyle.json` & `openbb_charting-2.0.2/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_charting-2.0.2/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/openbb_charting/utils/helpers.py` & `openbb_charting-2.0.2/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_charting-2.0.1/pyproject.toml` & `openbb_charting-2.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-charting"
-version = "2.0.1"
+version = "2.0.2"
 description = "Charting extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_charting" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
@@ -12,15 +12,15 @@
 plotly = "^5.17.0"
 statsmodels = "^0.14.0"
 reportlab = "^4.0.4"
 pywry = "^0.6.1"
 svglib = "^1.5.1"
 nbformat = "^5.9.2"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_obbject_extension"]
 openbb_charting = "openbb_charting:ext"
```

### Comparing `openbb_charting-2.0.1/PKG-INFO` & `openbb_charting-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-charting
-Version: 2.0.1
+Version: 2.0.2
 Summary: Charting extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: plotly (>=5.17.0,<6.0.0)
 Requires-Dist: pywry (>=0.6.1,<0.7.0)
 Requires-Dist: reportlab (>=4.0.4,<5.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: svglib (>=1.5.1,<2.0.0)
```

