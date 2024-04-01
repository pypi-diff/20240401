# Comparing `tmp/function2widgets-0.6.1.tar.gz` & `tmp/function2widgets-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function2widgets-0.6.1.tar", max compression
+gzip compressed data, was "function2widgets-0.6.2.tar", max compression
```

## Comparing `function2widgets-0.6.1.tar` & `function2widgets-0.6.2.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.1/function2widgets/__init__.py
--rw-r--r--   0        0        0     2587 2024-03-31 08:24:42.422890 function2widgets-0.6.1/function2widgets/common.py
--rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.1/function2widgets/factory.py
--rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.1/function2widgets/info.py
--rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.1/function2widgets/parser/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.1/function2widgets/parser/docstr_parser.py
--rw-r--r--   0        0        0     6341 2024-03-31 08:24:42.426892 function2widgets-0.6.1/function2widgets/parser/function_parser.py
--rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.1/function2widgets/parser/parameter_parser.py
--rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.1/function2widgets/parser/widgetconfigs_parser.py
--rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.1/function2widgets/widget.py
--rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.1/function2widgets/widgets/__init__.py
--rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.1/function2widgets/widgets/_sourcecodeedit.py
--rw-r--r--   0        0        0     1744 2024-03-31 08:24:42.432430 function2widgets-0.6.1/function2widgets/widgets/allwidgets.py
--rw-r--r--   0        0        0     6868 2024-03-31 11:37:44.468336 function2widgets-0.6.1/function2widgets/widgets/base.py
--rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.1/function2widgets/widgets/editor/__init__.py
--rw-r--r--   0        0        0     6028 2024-03-31 08:24:42.434438 function2widgets-0.6.1/function2widgets/widgets/editor/base.py
--rw-r--r--   0        0        0     2041 2024-03-31 08:24:42.435447 function2widgets-0.6.1/function2widgets/widgets/editor/codeeditor.py
--rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.1/function2widgets/widgets/editor/dicteditor.py
--rw-r--r--   0        0        0     4244 2024-03-31 08:24:42.437456 function2widgets-0.6.1/function2widgets/widgets/editor/jsoneditor.py
--rw-r--r--   0        0        0     1245 2024-03-31 08:24:42.437456 function2widgets-0.6.1/function2widgets/widgets/editor/listeditor.py
--rw-r--r--   0        0        0     1602 2024-03-31 08:24:42.438534 function2widgets-0.6.1/function2widgets/widgets/editor/tupleeditor.py
--rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.1/function2widgets/widgets/lineedit/__init__.py
--rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.1/function2widgets/widgets/lineedit/floatedit.py
--rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.1/function2widgets/widgets/lineedit/intedit.py
--rw-r--r--   0        0        0     2897 2024-03-31 08:24:42.441427 function2widgets-0.6.1/function2widgets/widgets/lineedit/stredit.py
--rw-r--r--   0        0        0        0 2024-03-31 08:24:42.442430 function2widgets-0.6.1/function2widgets/widgets/misc/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.1/function2widgets/widgets/misc/coloredit.py
--rw-r--r--   0        0        0      231 2024-03-31 08:24:42.443432 function2widgets-0.6.1/function2widgets/widgets/misc/timeedit.py
--rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.1/function2widgets/widgets/numberinput/__init__.py
--rw-r--r--   0        0        0     4498 2024-03-31 08:24:42.445444 function2widgets-0.6.1/function2widgets/widgets/numberinput/dial.py
--rw-r--r--   0        0        0     2852 2024-03-31 08:24:42.446444 function2widgets-0.6.1/function2widgets/widgets/numberinput/floatspin.py
--rw-r--r--   0        0        0     2591 2024-03-31 08:24:42.446444 function2widgets-0.6.1/function2widgets/widgets/numberinput/intspin.py
--rw-r--r--   0        0        0     4957 2024-03-31 08:24:42.447443 function2widgets-0.6.1/function2widgets/widgets/numberinput/slider.py
--rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.1/function2widgets/widgets/pathedit/__init__.py
--rw-r--r--   0        0        0     6027 2024-03-31 08:24:42.448967 function2widgets-0.6.1/function2widgets/widgets/pathedit/base.py
--rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.1/function2widgets/widgets/pathedit/dirpathedit.py
--rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.1/function2widgets/widgets/pathedit/filepathedit.py
--rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.1/function2widgets/widgets/selectwidget/__init__.py
--rw-r--r--   0        0        0     1640 2024-03-31 08:24:42.450995 function2widgets-0.6.1/function2widgets/widgets/selectwidget/checkbox.py
--rw-r--r--   0        0        0     2761 2024-03-31 08:24:42.451979 function2widgets-0.6.1/function2widgets/widgets/selectwidget/checkbox_group.py
--rw-r--r--   0        0        0     2923 2024-03-31 08:24:42.452993 function2widgets-0.6.1/function2widgets/widgets/selectwidget/combobox.py
--rw-r--r--   0        0        0     2205 2024-03-31 08:24:42.452993 function2widgets-0.6.1/function2widgets/widgets/selectwidget/combobox_edit.py
--rw-r--r--   0        0        0     3507 2024-03-31 08:24:42.454138 function2widgets-0.6.1/function2widgets/widgets/selectwidget/radiobutton_group.py
--rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.1/function2widgets/widgets/textedit/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.1/function2widgets/widgets/textedit/codeedit.py
--rw-r--r--   0        0        0     1730 2024-03-31 08:24:42.457977 function2widgets-0.6.1/function2widgets/widgets/textedit/plaintext.py
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.1/License
--rw-r--r--   0        0        0      714 2024-03-31 11:38:33.867213 function2widgets-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.1/README.md
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.2/function2widgets/__init__.py
+-rw-r--r--   0        0        0     2587 2024-03-31 08:24:42.422890 function2widgets-0.6.2/function2widgets/common.py
+-rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.2/function2widgets/factory.py
+-rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.2/function2widgets/info.py
+-rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.2/function2widgets/parser/__init__.py
+-rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.2/function2widgets/parser/docstr_parser.py
+-rw-r--r--   0        0        0     6341 2024-03-31 08:24:42.426892 function2widgets-0.6.2/function2widgets/parser/function_parser.py
+-rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.2/function2widgets/parser/parameter_parser.py
+-rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.2/function2widgets/parser/widgetconfigs_parser.py
+-rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.2/function2widgets/widget.py
+-rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.2/function2widgets/widgets/__init__.py
+-rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.2/function2widgets/widgets/_sourcecodeedit.py
+-rw-r--r--   0        0        0     1744 2024-03-31 08:24:42.432430 function2widgets-0.6.2/function2widgets/widgets/allwidgets.py
+-rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.2/function2widgets/widgets/base.py
+-rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.2/function2widgets/widgets/editor/__init__.py
+-rw-r--r--   0        0        0     6028 2024-03-31 08:24:42.434438 function2widgets-0.6.2/function2widgets/widgets/editor/base.py
+-rw-r--r--   0        0        0     2041 2024-03-31 08:24:42.435447 function2widgets-0.6.2/function2widgets/widgets/editor/codeeditor.py
+-rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.2/function2widgets/widgets/editor/dicteditor.py
+-rw-r--r--   0        0        0     4244 2024-03-31 08:24:42.437456 function2widgets-0.6.2/function2widgets/widgets/editor/jsoneditor.py
+-rw-r--r--   0        0        0     1245 2024-03-31 08:24:42.437456 function2widgets-0.6.2/function2widgets/widgets/editor/listeditor.py
+-rw-r--r--   0        0        0     1602 2024-03-31 08:24:42.438534 function2widgets-0.6.2/function2widgets/widgets/editor/tupleeditor.py
+-rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.2/function2widgets/widgets/lineedit/__init__.py
+-rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.2/function2widgets/widgets/lineedit/floatedit.py
+-rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.2/function2widgets/widgets/lineedit/intedit.py
+-rw-r--r--   0        0        0     2897 2024-03-31 08:24:42.441427 function2widgets-0.6.2/function2widgets/widgets/lineedit/stredit.py
+-rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.2/function2widgets/widgets/misc/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.2/function2widgets/widgets/misc/coloredit.py
+-rw-r--r--   0        0        0     2935 2024-04-01 15:50:20.804298 function2widgets-0.6.2/function2widgets/widgets/misc/dateedit.py
+-rw-r--r--   0        0        0     3481 2024-04-01 15:12:11.106842 function2widgets-0.6.2/function2widgets/widgets/misc/datetimeedit.py
+-rw-r--r--   0        0        0     2815 2024-04-01 15:44:10.500436 function2widgets-0.6.2/function2widgets/widgets/misc/timeedit.py
+-rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.2/function2widgets/widgets/numberinput/__init__.py
+-rw-r--r--   0        0        0     4498 2024-03-31 08:24:42.445444 function2widgets-0.6.2/function2widgets/widgets/numberinput/dial.py
+-rw-r--r--   0        0        0     2852 2024-03-31 08:24:42.446444 function2widgets-0.6.2/function2widgets/widgets/numberinput/floatspin.py
+-rw-r--r--   0        0        0     2591 2024-03-31 08:24:42.446444 function2widgets-0.6.2/function2widgets/widgets/numberinput/intspin.py
+-rw-r--r--   0        0        0     4957 2024-03-31 08:24:42.447443 function2widgets-0.6.2/function2widgets/widgets/numberinput/slider.py
+-rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.2/function2widgets/widgets/pathedit/__init__.py
+-rw-r--r--   0        0        0     6027 2024-03-31 08:24:42.448967 function2widgets-0.6.2/function2widgets/widgets/pathedit/base.py
+-rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.2/function2widgets/widgets/pathedit/dirpathedit.py
+-rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.2/function2widgets/widgets/pathedit/filepathedit.py
+-rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.2/function2widgets/widgets/selectwidget/__init__.py
+-rw-r--r--   0        0        0     1640 2024-03-31 08:24:42.450995 function2widgets-0.6.2/function2widgets/widgets/selectwidget/checkbox.py
+-rw-r--r--   0        0        0     2761 2024-03-31 08:24:42.451979 function2widgets-0.6.2/function2widgets/widgets/selectwidget/checkbox_group.py
+-rw-r--r--   0        0        0     2923 2024-03-31 08:24:42.452993 function2widgets-0.6.2/function2widgets/widgets/selectwidget/combobox.py
+-rw-r--r--   0        0        0     2205 2024-03-31 08:24:42.452993 function2widgets-0.6.2/function2widgets/widgets/selectwidget/combobox_edit.py
+-rw-r--r--   0        0        0     3507 2024-03-31 08:24:42.454138 function2widgets-0.6.2/function2widgets/widgets/selectwidget/radiobutton_group.py
+-rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.2/function2widgets/widgets/textedit/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.2/function2widgets/widgets/textedit/codeedit.py
+-rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.2/function2widgets/widgets/textedit/plaintext.py
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.2/License
+-rw-r--r--   0        0        0      714 2024-04-01 16:14:32.984051 function2widgets-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.2/README.md
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.2/PKG-INFO
```

### Comparing `function2widgets-0.6.1/function2widgets/common.py` & `function2widgets-0.6.2/function2widgets/common.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/factory.py` & `function2widgets-0.6.2/function2widgets/factory.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/info.py` & `function2widgets-0.6.2/function2widgets/info.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/parser/docstr_parser.py` & `function2widgets-0.6.2/function2widgets/parser/docstr_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/parser/function_parser.py` & `function2widgets-0.6.2/function2widgets/parser/function_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/parser/parameter_parser.py` & `function2widgets-0.6.2/function2widgets/parser/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/parser/widgetconfigs_parser.py` & `function2widgets-0.6.2/function2widgets/parser/widgetconfigs_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widget.py` & `function2widgets-0.6.2/function2widgets/widget.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/_sourcecodeedit.py` & `function2widgets-0.6.2/function2widgets/widgets/_sourcecodeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/allwidgets.py` & `function2widgets-0.6.2/function2widgets/widgets/allwidgets.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/base.py` & `function2widgets-0.6.2/function2widgets/widgets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import (
     QWidget,
     QLabel,
     QCheckBox,
     QVBoxLayout,
-    QSpacerItem,
-    QSizePolicy,
     QFrame,
 )
 
 from function2widgets.widget import BaseParameterWidget, WidgetArgs
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/base.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/codeeditor.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/codeeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/dicteditor.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/dicteditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/jsoneditor.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/jsoneditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/listeditor.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/listeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/editor/tupleeditor.py` & `function2widgets-0.6.2/function2widgets/widgets/editor/tupleeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/lineedit/floatedit.py` & `function2widgets-0.6.2/function2widgets/widgets/lineedit/floatedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/lineedit/intedit.py` & `function2widgets-0.6.2/function2widgets/widgets/lineedit/intedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/lineedit/stredit.py` & `function2widgets-0.6.2/function2widgets/widgets/lineedit/stredit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/numberinput/dial.py` & `function2widgets-0.6.2/function2widgets/widgets/numberinput/dial.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/numberinput/floatspin.py` & `function2widgets-0.6.2/function2widgets/widgets/numberinput/floatspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/numberinput/intspin.py` & `function2widgets-0.6.2/function2widgets/widgets/numberinput/intspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/numberinput/slider.py` & `function2widgets-0.6.2/function2widgets/widgets/numberinput/slider.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/pathedit/base.py` & `function2widgets-0.6.2/function2widgets/widgets/pathedit/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/pathedit/dirpathedit.py` & `function2widgets-0.6.2/function2widgets/widgets/pathedit/dirpathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/pathedit/filepathedit.py` & `function2widgets-0.6.2/function2widgets/widgets/pathedit/filepathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/selectwidget/checkbox.py` & `function2widgets-0.6.2/function2widgets/widgets/selectwidget/checkbox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/selectwidget/checkbox_group.py` & `function2widgets-0.6.2/function2widgets/widgets/selectwidget/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/selectwidget/combobox.py` & `function2widgets-0.6.2/function2widgets/widgets/selectwidget/combobox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/selectwidget/combobox_edit.py` & `function2widgets-0.6.2/function2widgets/widgets/selectwidget/combobox_edit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/selectwidget/radiobutton_group.py` & `function2widgets-0.6.2/function2widgets/widgets/selectwidget/radiobutton_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/textedit/codeedit.py` & `function2widgets-0.6.2/function2widgets/widgets/textedit/codeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/function2widgets/widgets/textedit/plaintext.py` & `function2widgets-0.6.2/function2widgets/widgets/textedit/plaintext.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 )
 
 
 @dataclasses.dataclass(frozen=True)
 class PlainTextEditArgs(CommonParameterWidgetArgs):
     parameter_name: str
     default: Optional[str] = ""
+    placeholder: Optional[str] = None
+    readonly: bool = False
+    overwrite_mode: bool = False
+    line_wrap_mode: bool = False
 
 
 class PlainTextEdit(CommonParameterWidget):
     HIDE_DEFAULT_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = PlainTextEditArgs
@@ -32,14 +36,24 @@
     @property
     def _args(self) -> PlainTextEditArgs:
         return cast(PlainTextEditArgs, super()._args)
 
     def setup_center_widget(self, center_widget: QWidget):
         self._value_widget = QPlainTextEdit(center_widget)
 
+        if self._args.placeholder:
+            self._value_widget.setPlaceholderText(self._args.placeholder)
+
+        self._value_widget.setReadOnly(self._args.readonly is True)
+        self._value_widget.setOverwriteMode(self._args.overwrite_mode is True)
+        if self._args.line_wrap_mode:
+            self._value_widget.setLineWrapMode(QPlainTextEdit.LineWrapMode.WidgetWidth)
+        else:
+            self._value_widget.setLineWrapMode(QPlainTextEdit.LineWrapMode.NoWrap)
+
         center_widget_layout = QVBoxLayout(center_widget)
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
         center_widget_layout.addWidget(self._value_widget)
 
     def get_value(self) -> Optional[str]:
```

### Comparing `function2widgets-0.6.1/License` & `function2widgets-0.6.2/License`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/pyproject.toml` & `function2widgets-0.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "function2widgets"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 packages = [
     {include="function2widgets"}
 ]
```

### Comparing `function2widgets-0.6.1/README.md` & `function2widgets-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.1/PKG-INFO` & `function2widgets-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function2widgets
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Home-page: https://github.com/zimolab/function2widgets
 License: GPL-3.0
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

