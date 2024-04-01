# Comparing `tmp/EasyOutput-0.0.4.tar.gz` & `tmp/EasyOutput-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyOutput-0.0.4.tar", last modified: Mon Apr  1 02:25:13 2024, max compression
+gzip compressed data, was "EasyOutput-0.0.5.tar", last modified: Mon Apr  1 16:06:05 2024, max compression
```

## Comparing `EasyOutput-0.0.4.tar` & `EasyOutput-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 02:25:13.700392 EasyOutput-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-01 02:25:13.698319 EasyOutput-0.0.4/EasyOutput.egg-info/
--rw-rw-rw-   0        0        0     2470 2024-04-01 02:25:13.000000 EasyOutput-0.0.4/EasyOutput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-04-01 02:25:13.000000 EasyOutput-0.0.4/EasyOutput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 02:25:13.000000 EasyOutput-0.0.4/EasyOutput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 02:25:13.000000 EasyOutput-0.0.4/EasyOutput.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-01 02:25:13.000000 EasyOutput-0.0.4/EasyOutput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-01 00:48:36.000000 EasyOutput-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2470 2024-04-01 02:25:13.699877 EasyOutput-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2024-04-01 02:25:06.000000 EasyOutput-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 02:25:13.697301 EasyOutput-0.0.4/pkg/
--rw-rw-rw-   0        0        0      153 2024-04-01 00:53:10.000000 EasyOutput-0.0.4/pkg/__init__.py
--rw-rw-rw-   0        0        0     2338 2024-04-01 02:16:23.000000 EasyOutput-0.0.4/pkg/easyoutput.py
--rw-rw-rw-   0        0        0       42 2024-04-01 02:25:13.700392 EasyOutput-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1179 2024-04-01 02:24:51.000000 EasyOutput-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:06:05.291528 EasyOutput-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-04-01 16:06:05.289529 EasyOutput-0.0.5/EasyOutput.egg-info/
+-rw-rw-rw-   0        0        0     2462 2024-04-01 16:06:05.000000 EasyOutput-0.0.5/EasyOutput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-04-01 16:06:05.000000 EasyOutput-0.0.5/EasyOutput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:06:05.000000 EasyOutput-0.0.5/EasyOutput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 16:06:05.000000 EasyOutput-0.0.5/EasyOutput.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-01 16:06:05.000000 EasyOutput-0.0.5/EasyOutput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-04-01 00:48:36.000000 EasyOutput-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2462 2024-04-01 16:06:05.290528 EasyOutput-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1731 2024-04-01 02:25:06.000000 EasyOutput-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:06:05.288522 EasyOutput-0.0.5/pkg/
+-rw-rw-rw-   0        0        0      351 2024-04-01 16:06:01.000000 EasyOutput-0.0.5/pkg/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-04-01 16:04:56.000000 EasyOutput-0.0.5/pkg/easyoutput.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:06:05.292528 EasyOutput-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1171 2024-04-01 16:06:01.000000 EasyOutput-0.0.5/setup.py
```

### Comparing `EasyOutput-0.0.4/EasyOutput.egg-info/PKG-INFO` & `EasyOutput-0.0.5/EasyOutput.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: EasyOutput
-Version: 0.0.4
+Version: 0.0.5
 Summary: Colored messages in the palm of your hand
 Author: FrankAustin
 Author-email: <frankaustindev808@gmail.com>
 Keywords: python,colored print,error message,success message,colored message
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EasyOutput-0.0.4/PKG-INFO` & `EasyOutput-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: EasyOutput
-Version: 0.0.4
+Version: 0.0.5
 Summary: Colored messages in the palm of your hand
 Author: FrankAustin
 Author-email: <frankaustindev808@gmail.com>
 Keywords: python,colored print,error message,success message,colored message
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EasyOutput-0.0.4/README.md` & `EasyOutput-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `EasyOutput-0.0.4/pkg/easyoutput.py` & `EasyOutput-0.0.5/pkg/easyoutput.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,93 +1,75 @@
+from typing import Optional
 from colorama import Fore, Style
 
 def Info_Message(message):
     """
     Prints a message notifying the user of specific need to know information.
-    
     Color: Blue
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.BLUE + Style.BRIGHT}Info{Style.RESET_ALL}: {message}")
-
+    
 def Error_Message(message):
     """
     Prints a message notifying the user of an error.
-    
     Color: Red
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.RED}Error{Style.RESET_ALL}: {Fore.YELLOW + message + Style.RESET_ALL}")
-
+    
 def Connection_Error_Message(message):
     """
     Prints a message notifying the user of a connection error.
-    
     Color: Red
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.RED}Connection Error{Style.RESET_ALL}: {Fore.YELLOW + message + Style.RESET_ALL}")
-
+    
 def Success_Message(message):
     """
     Prints a message notifying the user of a success.
-    
     Color: Bright Green
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
     
 def Successful_Connection_Message(message):
     """
     Prints a message notifying the user of a successful connection.
-    
     Color: Bright Green
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.GREEN + Style.BRIGHT}Successful Connection{Style.RESET_ALL}: {message}")
     
 def Note_Message(message):
     """
-
     Prints a note notifying the user of something they should be made aware of.
-    
     Color: Yellow
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.YELLOW}Note{Style.RESET_ALL}: {message}")
-
     
 def Wait_Message(message):
     """
-    
     Prints a wait message for the user indicating your code is running.
-    
     Color: White
-    
     Args:
         message (_type_): _description_
     """
     print(f"{Fore.LIGHTWHITE_EX}Wait{Style.RESET_ALL}: {message}")
     
 def Title_Print(title):
     """
-
     Prints a title for grouping lists and anything else you can think of.
-    
     Color: Bright Green
-    
     Args:
         title (_type_): _description_
     """
-    print(f"=== {Fore.GREEN + Style.BRIGHT + title + Style.RESET_ALL} ===")
+    print(f"=== {Fore.GREEN + Style.BRIGHT + title + Style.RESET_ALL} ===")
+
```

