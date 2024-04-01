# Comparing `tmp/adaptivecard-0.2.0.tar.gz` & `tmp/adaptivecard-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.2.0.tar", last modified: Mon Mar  4 05:36:25 2024, max compression
+gzip compressed data, was "adaptivecard-0.2.1.tar", last modified: Mon Apr  1 20:07:44 2024, max compression
```

## Comparing `adaptivecard-0.2.0.tar` & `adaptivecard-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.301699 adaptivecard-0.2.0/adaptivecard/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/_base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/card_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    21901 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/containers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2352 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/adaptivecard/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/adaptivecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-04 05:36:25.000000 adaptivecard-0.2.0/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-04 05:36:25.000000 adaptivecard-0.2.0/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 05:36:25.000000 adaptivecard-0.2.0/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-04 05:36:25.000000 adaptivecard-0.2.0/adaptivecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-04 05:36:25.000000 adaptivecard-0.2.0/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:25.305699 adaptivecard-0.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/unit/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/unit/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/unit/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-04 05:36:18.000000 adaptivecard-0.2.0/tests/unit/test_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/adaptivecard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/_base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/card_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21901 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/containers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2352 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/adaptivecard/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/adaptivecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 20:07:44.000000 adaptivecard-0.2.1/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 20:07:44.000000 adaptivecard-0.2.1/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:07:44.000000 adaptivecard-0.2.1/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 20:07:44.000000 adaptivecard-0.2.1/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 20:07:44.000000 adaptivecard-0.2.1/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:44.692720 adaptivecard-0.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/unit/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/unit/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/unit/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-01 20:07:35.000000 adaptivecard-0.2.1/tests/unit/test_inputs.py
```

### Comparing `adaptivecard-0.2.0/LICENSE.txt` & `adaptivecard-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/PKG-INFO` & `adaptivecard-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.2.0
+Version: 0.2.1
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,cards,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.2.0/adaptivecard/__init__.py` & `adaptivecard-0.2.1/adaptivecard/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/_base_types.py` & `adaptivecard-0.2.1/adaptivecard/_base_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -90,14 +90,18 @@
     pass
 
 
 class Time(ABC):
     pass
 
 
+class DataQuery(ABC):
+    pass
+
+
 class Toggle(ABC):
     pass
 
 
 class Choice(ABC):
     pass
 
@@ -115,12 +119,20 @@
 Element.register(Container)
 Element.register(TextBlock)
 Element.register(Image)
 Element.register(Message)
 Element.register(Content)
 Element.register(Action)
 Element.register(ActionSet)
+Element.register(Text)
+Element.register(Number)
+Element.register(Date)
+Element.register(Time)
+Element.register(DataQuery)
+Element.register(Toggle)
+Element.register(Choice)
+Element.register(ChoiceSet)
 Action.register(ShowCard)
 Action.register(Execute)
 Action.register(OpenUrl)
 Action.register(Submit)
 Action.register(ToggleVisibility)
```

### Comparing `adaptivecard-0.2.0/adaptivecard/_mixin.py` & `adaptivecard-0.2.1/adaptivecard/_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Any, get_type_hints
 from adaptivecard._typing import DefaultNone
+from adaptivecard._base_types import Element
 from adaptivecard._utils import check_type, snake_to_camel
 
 
 class Mixin:
     __slots__ = ()
 
     def to_dict(self):
         dic = {}
         for attr_name, attr_value in {attr_name: getattr(self, attr_name) for attr_name in self.__slots__ if hasattr(self, attr_name)}.items():
             camel_formated_attr_name = snake_to_camel(attr_name)
-            if hasattr(attr_value, "__slots__"):
+            if isinstance(attr_value, Element):
                 dic[camel_formated_attr_name] = attr_value.to_dict()
             elif isinstance(attr_value, list):
                 dic[camel_formated_attr_name] = [inner_value.to_dict() for inner_value in attr_value if hasattr(inner_value, "__slots__")]
             else:
                 attr_value = attr_value if attr_value is not None else "none"
                 dic[camel_formated_attr_name] = attr_value
         return dic
```

### Comparing `adaptivecard-0.2.0/adaptivecard/_typing.py` & `adaptivecard-0.2.1/adaptivecard/_typing.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/_utils.py` & `adaptivecard-0.2.1/adaptivecard/_utils.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/actions.py` & `adaptivecard-0.2.1/adaptivecard/actions.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/card_elements.py` & `adaptivecard-0.2.1/adaptivecard/card_elements.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/containers.py` & `adaptivecard-0.2.1/adaptivecard/containers.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/exceptions.py` & `adaptivecard-0.2.1/adaptivecard/exceptions.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/adaptivecard/inputs.py` & `adaptivecard-0.2.1/adaptivecard/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,16 @@
                  spacing: Literal["default", "none", "small", "medium", "large", "extraLarge",
                                   "padding"] | None = DefaultNone,
                  is_visible: bool = DefaultNone,
                  ):
 
         self.type = "Input.ChoiceSet"
         self.id = id
+        if choices is DefaultNone:
+            choices = ChoiceList()
         self.choices: ChoiceList = choices
         self.choices_data = choices_data
         self.is_multiselect = is_multiselect
         self.style = style
         self.value = value
         self.placeholder = placeholder
         self.wrap = wrap
@@ -253,23 +255,25 @@
         self.is_required = is_required
         self.label = label
         self.fallback = fallback
         self.height = height
         self.separator = separator
         self.spacing = spacing
         self.is_visible = is_visible
+    
+    def append(self, choice: Choice):
+        self.choices.append(choice)
 
     def to_dict(self):
-        dic = {}
-        for attr_name in self.__slots__:
-            if hasattr(self, attr_name):
-                attr_value = getattr(self, attr_name)
-                if attr_value == "choices_data":
-                    attr_value = attr_value.replace('_', '.')
-                dic[attr_name] = attr_value
+        dic = super().to_dict()
+        dic = {
+            key: value if key != "choices_data"
+            else "choices.data"
+            for key, value in dic.items()
+        }
         return dic
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         if __name == "choices":
             if isinstance(__value, Choice):
                 __value = ChoiceList([__value])
             elif isinstance(__value, ListLike) and not isinstance(__value, ChoiceList):
@@ -278,12 +282,13 @@
         return super().__setattr__(__name, __value)
     
 
 _base_types.Text.register(Text)
 _base_types.Number.register(Number)
 _base_types.Date.register(Date)
 _base_types.Time.register(Time)
+_base_types.DataQuery.register(DataQuery)
 _base_types.Toggle.register(Toggle)
 _base_types.Choice.register(Choice)
 _base_types.ChoiceSet.register(ChoiceSet)
```

### Comparing `adaptivecard-0.2.0/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.2.1/adaptivecard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.2.0
+Version: 0.2.1
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,cards,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.2.0/adaptivecard.egg-info/SOURCES.txt` & `adaptivecard-0.2.1/adaptivecard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/setup.py` & `adaptivecard-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 
 with open("requirements.txt") as f:
     requires = f.read().split()
```

### Comparing `adaptivecard-0.2.0/tests/integration/test_integration.py` & `adaptivecard-0.2.1/tests/integration/test_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from adaptivecard import AdaptiveCard
 from adaptivecard.containers import Container, ColumnSet, Column, Table, TableRow
 from adaptivecard.card_elements import TextBlock, Image
-
+from adaptivecard.inputs import Text, Time, ChoiceSet, Choice
 
 class Test:
     def test_message(self):
         card = AdaptiveCard()
         container = Container(style='warning', bleed=True, min_height=10)
         columns = [Column([1,1,1]), Column([2,2,2])]
         column_set = ColumnSet((columns), style='warning', min_height=8, height='auto')
@@ -20,10 +20,18 @@
         table[1][0] = 100
         assert table[1][0][0].text == "100"
         container_2.append(table)
         card.append(container_2)
         img = Image("https://hips.hearstapps.com/hmg-prod/images/dog-puppy-on-garden-royalty-free-image-1586966191.jpg?crop=1xw:0.74975xh;center,top&resize=1200:*",
                     size='medium', style='person', separator=True, height=70)
         card.append(img)
+        text_input = Text(id="text input id")
+        time_input = Time(id="time id")
+        card.append(text_input)
+        card.append(time_input)
+        choice_set = ChoiceSet(id="choice set id")
+        choice = Choice(title="some title", value="value1")
+        choice_set.append(choice)
+        card.append(choice_set)
         msg = card.to_message()
         json = msg.to_dict()
         assert isinstance(json, dict)
```

### Comparing `adaptivecard-0.2.0/tests/unit/test_actions.py` & `adaptivecard-0.2.1/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/tests/unit/test_containers.py` & `adaptivecard-0.2.1/tests/unit/test_containers.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/tests/unit/test_init.py` & `adaptivecard-0.2.1/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.2.0/tests/unit/test_inputs.py` & `adaptivecard-0.2.1/tests/unit/test_inputs.py`

 * *Files identical despite different names*

