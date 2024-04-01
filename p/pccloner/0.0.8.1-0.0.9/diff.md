# Comparing `tmp/pccloner-0.0.8.1.tar.gz` & `tmp/pccloner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pccloner-0.0.8.1.tar", last modified: Fri Mar 15 20:19:48 2024, max compression
+gzip compressed data, was "pccloner-0.0.9.tar", last modified: Thu Mar 21 20:12:46 2024, max compression
```

## Comparing `pccloner-0.0.8.1.tar` & `pccloner-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     1068 2024-03-12 17:39:19.000000 pccloner-0.0.8.1/LICENSE
--rw-r--r--   0 ezamorag  (1000) ezamorag  (1000)     2239 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/PKG-INFO
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     1684 2024-03-15 20:17:40.000000 pccloner-0.0.8.1/README.md
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       81 2024-03-13 20:26:49.000000 pccloner-0.0.8.1/pyproject.toml
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       38 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/setup.cfg
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)      971 2024-03-15 20:18:36.000000 pccloner-0.0.8.1/setup.py
-drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/src/
-drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/src/pccloner/
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-12 20:06:31.000000 pccloner-0.0.8.1/src/pccloner/__init__.py
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     4056 2024-03-13 20:05:32.000000 pccloner-0.0.8.1/src/pccloner/pcdata.py
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     3597 2024-03-15 18:22:30.000000 pccloner-0.0.8.1/src/pccloner/pctask.py
-drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-15 20:19:48.691719 pccloner-0.0.8.1/src/pccloner.egg-info/
--rw-r--r--   0 ezamorag  (1000) ezamorag  (1000)     2239 2024-03-15 20:19:48.000000 pccloner-0.0.8.1/src/pccloner.egg-info/PKG-INFO
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)      291 2024-03-15 20:19:48.000000 pccloner-0.0.8.1/src/pccloner.egg-info/SOURCES.txt
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        1 2024-03-15 20:19:48.000000 pccloner-0.0.8.1/src/pccloner.egg-info/dependency_links.txt
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       63 2024-03-15 20:19:48.000000 pccloner-0.0.8.1/src/pccloner.egg-info/requires.txt
--rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        9 2024-03-15 20:19:48.000000 pccloner-0.0.8.1/src/pccloner.egg-info/top_level.txt
+drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-21 20:12:46.093648 pccloner-0.0.9/
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     1068 2024-03-12 17:39:19.000000 pccloner-0.0.9/LICENSE
+-rw-r--r--   0 ezamorag  (1000) ezamorag  (1000)     2430 2024-03-21 20:12:46.093648 pccloner-0.0.9/PKG-INFO
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     1878 2024-03-21 19:48:57.000000 pccloner-0.0.9/README.md
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       81 2024-03-13 20:26:49.000000 pccloner-0.0.9/pyproject.toml
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       38 2024-03-21 20:12:46.093648 pccloner-0.0.9/setup.cfg
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)      969 2024-03-21 17:22:06.000000 pccloner-0.0.9/setup.py
+drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-21 20:12:46.089648 pccloner-0.0.9/src/
+drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-21 20:12:46.093648 pccloner-0.0.9/src/pccloner/
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-12 20:06:31.000000 pccloner-0.0.9/src/pccloner/__init__.py
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)     4245 2024-03-21 20:10:44.000000 pccloner-0.0.9/src/pccloner/pcdata.py
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)    11495 2024-03-21 19:35:51.000000 pccloner-0.0.9/src/pccloner/pctask.py
+drwxrwxr-x   0 ezamorag  (1000) ezamorag  (1000)        0 2024-03-21 20:12:46.093648 pccloner-0.0.9/src/pccloner.egg-info/
+-rw-r--r--   0 ezamorag  (1000) ezamorag  (1000)     2430 2024-03-21 20:12:46.000000 pccloner-0.0.9/src/pccloner.egg-info/PKG-INFO
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)      291 2024-03-21 20:12:46.000000 pccloner-0.0.9/src/pccloner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        1 2024-03-21 20:12:46.000000 pccloner-0.0.9/src/pccloner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)       63 2024-03-21 20:12:46.000000 pccloner-0.0.9/src/pccloner.egg-info/requires.txt
+-rw-rw-r--   0 ezamorag  (1000) ezamorag  (1000)        9 2024-03-21 20:12:46.000000 pccloner-0.0.9/src/pccloner.egg-info/top_level.txt
```

### Comparing `pccloner-0.0.8.1/LICENSE` & `pccloner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pccloner-0.0.8.1/PKG-INFO` & `pccloner-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccloner
-Version: 0.0.8.1
+Version: 0.0.9
 Summary: Clone your repetitive PC tasks
 Home-page: https://github.com/ezamorag/pccloner
 Author: Erik Zamora
 Author-email: ezamora1981@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,29 +14,36 @@
 Requires-Dist: pynput>=1.7.6
 Requires-Dist: pyautogui>=0.9.54
 Requires-Dist: keyboard>=0.13.5
 Requires-Dist: pandas>=2.1.4
 
 # pccloner
  When you perform a task on your PC, it stores mouse and keyboard actions along with the concurrent cursor position (and preceding screenshot) and then you can replay the stored task when you want. 
-
- Current limitations: 
- * No drag actions 
- * Not pressed two keys o more at the same time
- * The replayer is not prepared for all events
- * It has been tested only on Ubuntu 20.04.
- * The initial screen state at replaying must be similar to the stored initial screen state. 
- * Your replayed task performs well on the same computer with similar conditions.  
+ 
+Supported features: 
+ * It can replay double clicks and drag motions
+ * It is prepared to replay almost all single keyboard events (please report to me if you find one not supported) 
+ * It has been tested on Ubuntu 20.04 and Windows 11.
+ 
+Current limitations: 
+ * Hotkeys are not supported. 
+ * The initial screen state at replaying must be similar to the stored initial screen state to work well. 
+ * Store task must be replayed in the same computer.
 
 ## Authors
 - [Erik Zamora](https://www.ezamorag.com)
 ## Installation
 ```bash
 pip install pccloner
 ```
+On ubuntu: it requires to install gnome-screenshot.
+```bash
+sudo apt install gnome-screenshot
+```
+
 ## Usage
 1. Write a python script with following lines:
 ```bash
 File: collector.py
 
 from pccloner.pcdata import Collector
```

### Comparing `pccloner-0.0.8.1/README.md` & `pccloner-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # pccloner
  When you perform a task on your PC, it stores mouse and keyboard actions along with the concurrent cursor position (and preceding screenshot) and then you can replay the stored task when you want. 
-
- Current limitations: 
- * No drag actions 
- * Not pressed two keys o more at the same time
- * The replayer is not prepared for all events
- * It has been tested only on Ubuntu 20.04.
- * The initial screen state at replaying must be similar to the stored initial screen state. 
- * Your replayed task performs well on the same computer with similar conditions.  
+ 
+Supported features: 
+ * It can replay double clicks and drag motions
+ * It is prepared to replay almost all single keyboard events (please report to me if you find one not supported) 
+ * It has been tested on Ubuntu 20.04 and Windows 11.
+ 
+Current limitations: 
+ * Hotkeys are not supported. 
+ * The initial screen state at replaying must be similar to the stored initial screen state to work well. 
+ * Store task must be replayed in the same computer.
 
 ## Authors
 - [Erik Zamora](https://www.ezamorag.com)
 ## Installation
 ```bash
 pip install pccloner
 ```
+On ubuntu: it requires to install gnome-screenshot.
+```bash
+sudo apt install gnome-screenshot
+```
+
 ## Usage
 1. Write a python script with following lines:
 ```bash
 File: collector.py
 
 from pccloner.pcdata import Collector
 
@@ -35,8 +42,8 @@
 
 sample_paths = glob('./data/*/*.csv')   # Select the right path of your stored tasks
 ix_sample = 2  # Select your stored task 
 
 sample = pd.read_csv(sample_paths[ix_sample], index_col=0)
 task1 = Replayer(sample, data_dir='./')
 task1.execute()
-```
+```
```

### Comparing `pccloner-0.0.8.1/setup.py` & `pccloner-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pccloner',
-    version='0.0.8.1',
+    version='0.0.9',
     description= "Clone your repetitive PC tasks",
     py_modules = ['pccloner.pcdata', 'pccloner.pctask'],
     packages = find_packages(),
     package_dir = {'':'src'},
     
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

### Comparing `pccloner-0.0.8.1/src/pccloner/pcdata.py` & `pccloner-0.0.9/src/pccloner/pcdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import datetime
 
 # Future work: 
 #   Include PC sound, microphone, webcam
 #   Make the same for smartphones
 #   avoid adsminitrator permissions on ubuntu
 #   The key identification for alt and other some keys will be changed from keyboard to keyboard 
+#   Upload data https://ragug.medium.com/how-to-upload-files-using-the-google-drive-api-in-python-ebefdfd63eab
 
 #   Make easy installation for windows users using pip install 
 
 class Collector:
     def __init__(self, base_folder='data/'):
         self.mouse = mouse.Controller()
         self.counter = 0
@@ -30,26 +31,26 @@
     # Monitoring
     def start(self):
         print("Waiting for activation with ESC key ...")
         kb.wait('esc')
 
         print("Monitoring is working ...")
         self.movelistener.start()  
-        self.date = datetime.datetime.now()
+        self.date = str(datetime.datetime.now()).split('.')[0].replace(':','-').replace(' ','_')
         self.running = True
         self.start_time = time.perf_counter()
         self.lastscreen = (time.perf_counter() - self.start_time, pyautogui.screenshot())
         with mouse.Listener(on_click=self.on_click, on_scroll=self.on_scroll), \
              keyboard.Listener(on_press=self.on_press, on_release=self.on_release):
             while self.running:
                 self.lastscreen = (time.perf_counter() - self.start_time, pyautogui.screenshot())
         print("Monitoring was ended ...")
 
         data_df = pd.DataFrame(self.data, columns =['timestamp', 'img_path', 'px', 'py', 'event', 'trajectory'])
-        data_df.to_csv(self.sample_folder + f'rawdata_{self.date}.csv')
+        data_df.to_csv(self.sample_folder + f'raw_pcdata_{self.date}.csv')
         self.movelistener.stop()
 
     # Mouse events
     def on_move(self, x, y):
         if self.movesflag == True:
             self.moves.append((time.perf_counter() - self.start_time, x, y)) 
         else:
@@ -61,19 +62,19 @@
             self.savedata(px, py, event=f'pressed {button}')
         else:
             self.movesflag = False
             self.savedata(px, py, event=f'released {button}', trajectory=self.moves)
 
     def on_scroll(self, px, py, dx, dy):
         if dy == 1:
-            scroll = 'scroll_down' 
+            scroll = 'pressed Scroll.down' 
         elif dy == -1:
-            scroll = 'scroll_up'
+            scroll = 'pressed Scroll.up'
         else:
-            scroll = 'what?_scroll'
+            scroll = 'pressed Scroll.what?'
         self.savedata(px, py, event=scroll)
     
     # Keyboard events 
     def on_press(self, key):
         if key == keyboard.Key.esc: 
             self.running = False
         key = str(key).strip("'")
@@ -81,15 +82,15 @@
         self.savedata(px, py, event=f'pressed {key}')
         
     def on_release(self, key):
         key = str(key).strip("'")
         px, py = self.mouse.position
         self.savedata(px, py, event=f'released {key}')
 
-    def savedata(self, px, py, event, trajectory=None):
+    def savedata(self, px, py, event, trajectory=[]):
         timestamp = time.perf_counter() - self.start_time
         t, img = self.lastscreen
         img_path = self.sample_folder + 'screen{:010}_{}.jpg'.format(self.counter, t)
         self.data.append((timestamp, img_path, px, py, event, trajectory))
         img.save(img_path)
         self.counter += 1
```

### Comparing `pccloner-0.0.8.1/src/pccloner.egg-info/PKG-INFO` & `pccloner-0.0.9/src/pccloner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccloner
-Version: 0.0.8.1
+Version: 0.0.9
 Summary: Clone your repetitive PC tasks
 Home-page: https://github.com/ezamorag/pccloner
 Author: Erik Zamora
 Author-email: ezamora1981@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,29 +14,36 @@
 Requires-Dist: pynput>=1.7.6
 Requires-Dist: pyautogui>=0.9.54
 Requires-Dist: keyboard>=0.13.5
 Requires-Dist: pandas>=2.1.4
 
 # pccloner
  When you perform a task on your PC, it stores mouse and keyboard actions along with the concurrent cursor position (and preceding screenshot) and then you can replay the stored task when you want. 
-
- Current limitations: 
- * No drag actions 
- * Not pressed two keys o more at the same time
- * The replayer is not prepared for all events
- * It has been tested only on Ubuntu 20.04.
- * The initial screen state at replaying must be similar to the stored initial screen state. 
- * Your replayed task performs well on the same computer with similar conditions.  
+ 
+Supported features: 
+ * It can replay double clicks and drag motions
+ * It is prepared to replay almost all single keyboard events (please report to me if you find one not supported) 
+ * It has been tested on Ubuntu 20.04 and Windows 11.
+ 
+Current limitations: 
+ * Hotkeys are not supported. 
+ * The initial screen state at replaying must be similar to the stored initial screen state to work well. 
+ * Store task must be replayed in the same computer.
 
 ## Authors
 - [Erik Zamora](https://www.ezamorag.com)
 ## Installation
 ```bash
 pip install pccloner
 ```
+On ubuntu: it requires to install gnome-screenshot.
+```bash
+sudo apt install gnome-screenshot
+```
+
 ## Usage
 1. Write a python script with following lines:
 ```bash
 File: collector.py
 
 from pccloner.pcdata import Collector
```

