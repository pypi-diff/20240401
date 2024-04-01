# Comparing `tmp/MacroQueue-0.2.0.tar.gz` & `tmp/MacroQueue-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacroQueue-0.2.0.tar", last modified: Wed Mar 27 15:07:28 2024, max compression
+gzip compressed data, was "MacroQueue-0.2.1.tar", last modified: Mon Apr  1 16:56:31 2024, max compression
```

## Comparing `MacroQueue-0.2.0.tar` & `MacroQueue-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:28.006530 MacroQueue-0.2.0/
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:27.948504 MacroQueue-0.2.0/MacroQueue/
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:27.952725 MacroQueue-0.2.0/MacroQueue/Bitmaps/
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.239000 MacroQueue-0.2.0/MacroQueue/Bitmaps/DownArrow.bmp
--rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.882000 MacroQueue-0.2.0/MacroQueue/Bitmaps/Remove.bmp
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.090000 MacroQueue-0.2.0/MacroQueue/Bitmaps/UpArrow.bmp
--rw-rw-rw-   0        0        0    68756 2024-03-27 14:08:48.261791 MacroQueue-0.2.0/MacroQueue/Dialogs.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:27.992630 MacroQueue-0.2.0/MacroQueue/Functions/
--rw-rw-rw-   0        0        0     1043 2024-01-11 19:05:47.857710 MacroQueue-0.2.0/MacroQueue/Functions/BField.py
--rw-rw-rw-   0        0        0    21583 2024-03-20 19:07:49.690671 MacroQueue-0.2.0/MacroQueue/Functions/CreaTec.py
--rw-rw-rw-   0        0        0     1334 2024-03-27 14:52:45.709470 MacroQueue-0.2.0/MacroQueue/Functions/General.py
--rw-rw-rw-   0        0        0     1656 2024-03-25 14:52:53.825559 MacroQueue-0.2.0/MacroQueue/Functions/RF.py
--rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.990178 MacroQueue-0.2.0/MacroQueue/Functions/RHK.py
--rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.655627 MacroQueue-0.2.0/MacroQueue/Functions/SXM.py
--rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.699359 MacroQueue-0.2.0/MacroQueue/Functions/SXMRemote.py
--rw-rw-rw-   0        0        0    24521 2024-03-21 18:30:14.367345 MacroQueue-0.2.0/MacroQueue/GUIDesign.py
--rw-rw-rw-   0        0        0    54446 2024-03-27 15:05:12.481079 MacroQueue-0.2.0/MacroQueue/MacroQueue.py
--rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.006571 MacroQueue-0.2.0/MacroQueue/MacroQueueIcon.ico
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:27.992630 MacroQueue-0.2.0/MacroQueue/Macros/
--rw-rw-rw-   0        0        0    15106 2024-03-27 14:53:17.588235 MacroQueue-0.2.0/MacroQueue/Macros/CreaTecMacro.json
--rw-rw-rw-   0        0        0     7924 2022-06-13 16:55:53.604555 MacroQueue-0.2.0/MacroQueue/Macros/RHKMacro.json
--rw-rw-rw-   0        0        0      342 2024-03-19 17:21:26.126224 MacroQueue-0.2.0/MacroQueue/MakeExe.sh
--rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.723712 MacroQueue-0.2.0/MacroQueue/__init__.py
--rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.342250 MacroQueue-0.2.0/MacroQueue/__main__.py
--rw-rw-rw-   0        0        0      733 2024-03-27 15:07:28.006530 MacroQueue-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-03-19 18:30:21.736909 MacroQueue-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1869 2024-03-27 15:07:11.609286 MacroQueue-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:07:28.001501 MacroQueue-0.2.0/test/
--rw-rw-rw-   0        0        0      562 2024-03-19 18:06:33.019995 MacroQueue-0.2.0/test/test_MainFrame.py
--rw-rw-rw-   0        0        0      774 2024-03-19 18:07:50.777916 MacroQueue-0.2.0/test/test_STMthread.py
--rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.005391 MacroQueue-0.2.0/test/test_readdata.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.881284 MacroQueue-0.2.1/
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.848759 MacroQueue-0.2.1/MacroQueue/
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.860059 MacroQueue-0.2.1/MacroQueue/Bitmaps/
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.239000 MacroQueue-0.2.1/MacroQueue/Bitmaps/DownArrow.bmp
+-rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.882000 MacroQueue-0.2.1/MacroQueue/Bitmaps/Remove.bmp
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.090000 MacroQueue-0.2.1/MacroQueue/Bitmaps/UpArrow.bmp
+-rw-rw-rw-   0        0        0    68756 2024-03-27 14:08:48.261791 MacroQueue-0.2.1/MacroQueue/Dialogs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.864710 MacroQueue-0.2.1/MacroQueue/Functions/
+-rw-rw-rw-   0        0        0     1043 2024-01-11 19:05:47.857710 MacroQueue-0.2.1/MacroQueue/Functions/BField.py
+-rw-rw-rw-   0        0        0    21517 2024-04-01 13:25:42.475019 MacroQueue-0.2.1/MacroQueue/Functions/CreaTec.py
+-rw-rw-rw-   0        0        0     1517 2024-03-27 16:22:52.969731 MacroQueue-0.2.1/MacroQueue/Functions/General.py
+-rw-rw-rw-   0        0        0     1656 2024-03-25 14:52:53.825559 MacroQueue-0.2.1/MacroQueue/Functions/RF.py
+-rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.990178 MacroQueue-0.2.1/MacroQueue/Functions/RHK.py
+-rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.655627 MacroQueue-0.2.1/MacroQueue/Functions/SXM.py
+-rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.699359 MacroQueue-0.2.1/MacroQueue/Functions/SXMRemote.py
+-rw-rw-rw-   0        0        0    24521 2024-03-21 18:30:14.367345 MacroQueue-0.2.1/MacroQueue/GUIDesign.py
+-rw-rw-rw-   0        0        0    54897 2024-04-01 15:32:11.063967 MacroQueue-0.2.1/MacroQueue/MacroQueue.py
+-rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.006571 MacroQueue-0.2.1/MacroQueue/MacroQueueIcon.ico
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.876839 MacroQueue-0.2.1/MacroQueue/Macros/
+-rw-rw-rw-   0        0        0    13972 2024-03-27 16:23:14.327309 MacroQueue-0.2.1/MacroQueue/Macros/CreaTecMacro.json
+-rw-rw-rw-   0        0        0     7924 2022-06-13 16:55:53.604555 MacroQueue-0.2.1/MacroQueue/Macros/RHKMacro.json
+-rw-rw-rw-   0        0        0      539 2024-04-01 15:21:24.255119 MacroQueue-0.2.1/MacroQueue/MakeExe.sh
+-rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.723712 MacroQueue-0.2.1/MacroQueue/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.342250 MacroQueue-0.2.1/MacroQueue/__main__.py
+-rw-rw-rw-   0        0        0     3887 2024-04-01 16:56:31.881284 MacroQueue-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:56:28.581338 MacroQueue-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2135 2024-04-01 16:54:07.635444 MacroQueue-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:56:31.881284 MacroQueue-0.2.1/test/
+-rw-rw-rw-   0        0        0      562 2024-03-19 18:06:33.019995 MacroQueue-0.2.1/test/test_MainFrame.py
+-rw-rw-rw-   0        0        0      774 2024-03-19 18:07:50.777916 MacroQueue-0.2.1/test/test_STMthread.py
+-rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.005391 MacroQueue-0.2.1/test/test_readdata.py
```

### Comparing `MacroQueue-0.2.0/MacroQueue/Bitmaps/DownArrow.bmp` & `MacroQueue-0.2.1/MacroQueue/Bitmaps/DownArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Bitmaps/Remove.bmp` & `MacroQueue-0.2.1/MacroQueue/Bitmaps/Remove.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Bitmaps/UpArrow.bmp` & `MacroQueue-0.2.1/MacroQueue/Bitmaps/UpArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Dialogs.py` & `MacroQueue-0.2.1/MacroQueue/Dialogs.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/BField.py` & `MacroQueue-0.2.1/MacroQueue/Functions/BField.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/CreaTec.py` & `MacroQueue-0.2.1/MacroQueue/Functions/CreaTec.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     if STM is not None:
         pass
 
     if BField is not None:
         OutgoingQueue.put(("DontClose","The Magnetic Field is not off.  Run the function 'Turn B Field Off'."))
         MacroQueueSelf.Closing=False
 
-    if RFGenerator is not None:
-        Turn_Off_RF_Generator()
 
 
 
 
 # {"Name":"B","Units":"T","Min":-1,"Max":1,"Tooltip":"The magnetic field strength in T"}
 def Set_B_Field(B=1):
     if B < -1 or B > 1:
```

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/General.py` & `MacroQueue-0.2.1/MacroQueue/Functions/General.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from time import sleep
 
 Cancel = False
 MacroQueueSelf = None
 
 
+
+# {"Name":"SomeParameter","Max":10}
+def Exception_Function(SomeParameter=5):
+    if SomeParameter > 10:
+        raise ValueError(f"{SomeParameter} is too large.")
+    pass
+
+
 def Bare_Function(SomeParameter,SomeParameter2="a"):
     print(SomeParameter)
     print("Hehehe")
 
 # {"Name":"SomeNumber","Units":"V","Min":-10,"Max":10,"Tooltip":"An example function which only takes numbers"}
 def Numerical_Function(SomeNumber=5):
     print(SomeNumber)
```

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/RF.py` & `MacroQueue-0.2.1/MacroQueue/Functions/RF.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/RHK.py` & `MacroQueue-0.2.1/MacroQueue/Functions/RHK.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/SXM.py` & `MacroQueue-0.2.1/MacroQueue/Functions/SXM.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Functions/SXMRemote.py` & `MacroQueue-0.2.1/MacroQueue/Functions/SXMRemote.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/GUIDesign.py` & `MacroQueue-0.2.1/MacroQueue/GUIDesign.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/MacroQueue.py` & `MacroQueue-0.2.1/MacroQueue/MacroQueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 import queue
 import threading
 import importlib
 import importlib.util
 from inspect import getmembers, isfunction,getcomments
 
 import wx
+import pyvisa
+import pythoncom
+from datetime import datetime
 
 from time import time as timer
 
-sys.path.append(os.path.dirname(__file__))
+application_path = os.path.dirname(sys.executable) if getattr(sys, 'frozen', False) else os.path.dirname(__file__)
+sys.path.append(application_path)
 try:
     from MacroQueue.Dialogs import MyMacroDialog
     from MacroQueue.Dialogs import MyMacroSettingsDialog
     from MacroQueue.Dialogs import MyStartMacroDialog
     from MacroQueue.Dialogs import MyChooseSoftwareDialog
     from MacroQueue.GUIDesign import MyFrame
 except ModuleNotFoundError:
@@ -28,15 +32,18 @@
     from GUIDesign import MyFrame
     
 # from GUIDesign import MacroDialog
 from inspect import getmembers, isfunction
 
 # They all go in try/except just in case the required packages aren't installed for one of them 
 # (e.g. you can still use RHK's functions even without win32com which you need for CreaTec)
-sys.path.append(os.path.dirname(__file__)+"\\Functions")
+if getattr(sys, 'frozen', False):
+    sys.path.append(os.path.dirname(sys.executable)+"\\Functions")
+else:
+    sys.path.append(os.path.dirname(__file__)+"\\Functions")
 
 import json
 
 
 IconFileName = "MacroQueueIcon.ico"
 
 
@@ -95,15 +102,14 @@
     Editting = False
     Functions = {}
 # my_module = importlib.import_module('os.path')
     def __init__(self,test=False):
         self.test = test
         application_path = os.path.dirname(sys.executable) if getattr(sys, 'frozen', False) else os.path.dirname(__file__)
         os.chdir(os.path.realpath(application_path))
-        
         self.SavedSettingsFile = 'MacroQueueSettings.csv'
 
 
         # The GUIDesign is defined in GUIDesign.py as the class MyFrame. It was made with wxFormBuilder
         MyFrame.__init__(self, parent=None) 
         icon_file = os.path.join(os.path.abspath(os.path.dirname(__file__)), IconFileName)
         if os.path.exists(icon_file):
@@ -259,16 +265,17 @@
         if self.Closing:
             self.Destroy()
     def LoadFunctions(self,Reloading=False):
         FunctionNames = [file for file in os.listdir('Functions') if file[-3:] == ".py"]
         self.Functions = {}
         for FunctionName in FunctionNames:
             try:
-                self.Functions[f"{FunctionName[:-3]}"] = import_source_file(os.path.abspath(f'Functions\\{FunctionName}'),os.path.abspath(f'Functions\\{FunctionName}'))         
-            except:
+                self.Functions[f"{FunctionName[:-3]}"] = import_source_file(os.path.abspath(f'Functions\\{FunctionName}'),FunctionName[:-3])         
+                # self.Functions[f"{FunctionName[:-3]}"] = import_source_file(os.path.abspath(f'Functions\\{FunctionName}'),os.path.abspath(f'Functions\\{FunctionName}'))         
+            except Exception as e:
                 pass
         for file in ["CreaTec.py","RHK.py","SXM.py","SXMRemote.py"]:
             try:
                 FunctionNames.remove(file)
             except:
                 pass
         try:
@@ -309,15 +316,15 @@
         
         def WriteFile(AllTheMacros):
             os.makedirs("Macros",exist_ok=True)
             with open(self.MacroPath, 'w') as fp:
                 json.dump(AllTheMacros, fp,indent=1)
 
         # for FunctionName in self.Functions[self.SettingsDict['Software']].keys():
-        
+                
         FunctionList = []
         for FunctionFile in [self.Software,*self.FunctionsLoaded]:
             NewFunctions = getmembers(self.Functions[FunctionFile], isfunction)
             FunctionList = FunctionList + NewFunctions
         FunctionList = [function[0].replace("_"," ") for function in FunctionList]
         for FunctionName,Macro in AllTheMacros.items():
             SkipMacro = False
```

### Comparing `MacroQueue-0.2.0/MacroQueue/MacroQueueIcon.ico` & `MacroQueue-0.2.1/MacroQueue/MacroQueueIcon.ico`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/Macros/CreaTecMacro.json` & `MacroQueue-0.2.1/MacroQueue/Macros/CreaTecMacro.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.94375%*

 * *Differences: {"'Test'": "{0: {insert: [(0, 'Exception Function'), (1, OrderedDict([('SomeParameter', "*

 * *           "OrderedDict([('DefaultValue', '5'), ('Tooltip', '\\nMaximum value: 10'), ('Frozen', "*

 * *           "False), ('ValueType', 'Numerical'), ('InRange', True), ('Name', 'SomeParameter'), "*

 * *           "('Max', 10)]))]))], delete: [1, 0]}, delete: [0]}"}*

```diff
@@ -490,73 +490,27 @@
             "Spectrum",
             {},
             true
         ]
     ],
     "Test": [
         [
-            "Numerical Function",
+            "Exception Function",
             {
-                "SomeNumber": {
+                "SomeParameter": {
                     "DefaultValue": "5",
                     "Frozen": false,
                     "InRange": true,
                     "Max": 10,
-                    "Min": -10,
-                    "Name": "SomeNumber",
-                    "Tooltip": "An example function which only takes numbers\nAcceptable range: (-10,10)",
-                    "Units": "V",
+                    "Name": "SomeParameter",
+                    "Tooltip": "\nMaximum value: 10",
                     "ValueType": "Numerical"
                 }
             },
             true
-        ],
-        [
-            "Complex Function",
-            {
-                "SomeBoolean": {
-                    "DefaultValue": true,
-                    "Frozen": false,
-                    "InRange": true,
-                    "Name": "SomeBoolean",
-                    "Tooltip": "A Boolean parameter produces a checkbox",
-                    "ValueType": "Boolean"
-                },
-                "SomeChoice": {
-                    "DefaultList": [
-                        "Choice",
-                        "Combo",
-                        "3rd",
-                        "4th"
-                    ],
-                    "DefaultValue": "Choice",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Name": "SomeChoice",
-                    "Tooltip": "A Choice parameter produces a dropdown menu",
-                    "ValueType": "Choice"
-                },
-                "SomeFilePath": {
-                    "DefaultValue": "C:\\",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Name": "SomeFilePath",
-                    "Tooltip": "A filepath parameter produces a 'browse' button",
-                    "ValueType": "File"
-                },
-                "SomeString": {
-                    "DefaultValue": "String",
-                    "Frozen": false,
-                    "InRange": true,
-                    "Name": "SomeString",
-                    "Tooltip": "A String parameter produces a textbox",
-                    "ValueType": "String"
-                }
-            },
-            true
         ]
     ],
     "Wait": [
         [
             "Wait",
             {
                 "WaitTime": {
```

### Comparing `MacroQueue-0.2.0/MacroQueue/Macros/RHKMacro.json` & `MacroQueue-0.2.1/MacroQueue/Macros/RHKMacro.json`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/MacroQueue/__init__.py` & `MacroQueue-0.2.1/MacroQueue/__init__.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/test/test_MainFrame.py` & `MacroQueue-0.2.1/test/test_MainFrame.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/test/test_STMthread.py` & `MacroQueue-0.2.1/test/test_STMthread.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.0/test/test_readdata.py` & `MacroQueue-0.2.1/test/test_readdata.py`

 * *Files identical despite different names*

