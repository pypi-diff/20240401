# Comparing `tmp/botnikkk-0.0.5.tar.gz` & `tmp/botnikkk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.0.5.tar", last modified: Mon Apr  1 12:43:28 2024, max compression
+gzip compressed data, was "botnikkk-0.0.6.tar", last modified: Mon Apr  1 16:08:27 2024, max compression
```

## Comparing `botnikkk-0.0.5.tar` & `botnikkk-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.076300 botnikkk-0.0.5/
--rw-rw-rw-   0        0        0      559 2024-04-01 12:43:28.072298 botnikkk-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-03-30 21:04:38.000000 botnikkk-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.058299 botnikkk-0.0.5/botnikkk/
--rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.5/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     2453 2024-04-01 12:42:28.000000 botnikkk-0.0.5/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.071298 botnikkk-0.0.5/botnikkk.egg-info/
--rw-rw-rw-   0        0        0      559 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 12:43:28.076300 botnikkk-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      961 2024-04-01 12:43:10.000000 botnikkk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.182315 botnikkk-0.0.6/
+-rw-rw-rw-   0        0        0     2273 2024-04-01 16:08:27.179316 botnikkk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-04-01 16:06:13.000000 botnikkk-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.167320 botnikkk-0.0.6/botnikkk/
+-rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.6/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.6/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.178316 botnikkk-0.0.6/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     2273 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:08:27.182315 botnikkk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-01 16:07:43.000000 botnikkk-0.0.6/setup.py
```

### Comparing `botnikkk-0.0.5/botnikkk/formatting.py` & `botnikkk-0.0.6/botnikkk/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import screeninfo
 import asyncio
 
 screen_width = screeninfo.get_monitors()[0].width
 middle = " "*int(((screen_width/9)-128)/2)
 
-def centre(title,symbol=" ",str_end="\n") :
+def centre(title='',symbol=" ",str_end="\n") :
     #aligns the title in centre with symbols around it
     gap = str(symbol)*(64-int((len(title)/2)))
     gap2 = str(symbol)*(128- len(title) - len(gap))
     if str_end != '\r' :
         print(( middle + "|" + gap + title + gap2 + "|" + "\n" + middle + "|" + 128*" " + "|"),end=str_end)
     else :
         print(( middle + "|" + gap + title + gap2 + "|"),end='\r')
     return screen_width, middle
 
+def format_input(ques='') : 
+    string  = middle + "| " + ques  + " "*(127-(len(ques))) +  "|\n" + middle  + "| -" 
+    output = input(string)
+    return output
+
 def int_check(answer='') :
     answer = str(answer).strip()
     integer = -1
     while integer < 1 :
         try : 
             int(answer)
             integer = int(answer)
@@ -25,40 +30,37 @@
             centre("Please enter a valid integer !")
             ques = "Enter a number -"
             string  = middle + "| " + ques  + " "*(127-(len(ques))) +  "|\n" + middle  + "| -" 
             answer = input(string) 
             continue
     return int(answer)
 
-def format_input(ques='') : 
-    string  = middle + "| " + ques  + " "*(127-(len(ques))) +  "|\n" + middle  + "| -" 
-    output = input(string)
-    return output
-
 def ans_check(option_list=[]) :    
-
-    #prints and detetcs the answers and returns the choose answer
-    centre("-","-")
-    for i in option_list : 
-        centre(symbol=" ", title=(str(option_list.index(i) + 1) + ".) " + str(i)))
-    centre("-","-")
-    ques = "Choose a option"
-    string  = middle + "| " + ques  + " "*(127-(len(ques))) +  "|\n" + middle  + "| -" 
-    answer = input(string)
-    answer = answer.strip()
-    answer = int_check(answer)
-    while int(answer) > len(option_list) :
-            centre("Not a valid answer !")
-            answer = format_input("Choose a option")
-            try :
-                int(answer) 
-            except  :
-                answer = int_check(answer)
-        
-    return option_list[int(answer) - 1]
+    if type(option_list) is not list :
+        print('please input a list')
+    else:
+        #prints and detetcs the answers and returns the choose answer
+        centre("-","-")
+        for i in option_list : 
+            centre(symbol=" ", title=(str(option_list.index(i) + 1) + ".) " + str(i)))
+        centre("-","-")
+        ques = "Choose a option"
+        string  = middle + "| " + ques  + " "*(127-(len(ques))) +  "|\n" + middle  + "| -" 
+        answer = input(string)
+        answer = answer.strip()
+        answer = int_check(answer)
+        while int(answer) > len(option_list) :
+                centre("Not a valid answer !")
+                answer = format_input("Choose a option")
+                try :
+                    int(answer) 
+                except  :
+                    answer = int_check(answer)
+            
+        return option_list[int(answer) - 1]
 
 async def redirect_function(redirect):
     for i in range(3,0,-1):
         title = f"Redirecting to {redirect} in {i}..."
         symbol = " "
         gap = str(symbol)*(64-int((len(title)/2)))
         gap2 = str(symbol)*(128- len(title) - len(gap))
```

