# Comparing `tmp/unibot_hn-0.0.7.tar.gz` & `tmp/unibot_hn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibot_hn-0.0.7.tar", max compression
+gzip compressed data, was "unibot_hn-0.0.8.tar", max compression
```

## Comparing `unibot_hn-0.0.7.tar` & `unibot_hn-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.0.7/LICENSE
--rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.0.7/README.md
--rw-r--r--   0        0        0      316 2024-03-25 08:19:44.223649 unibot_hn-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-03-22 14:55:21.004090 unibot_hn-0.0.7/unibot_hn/.DS_Store
--rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.0.7/unibot_hn/Misc.py
--rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.0.7/unibot_hn/PID.py
--rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.0.7/unibot_hn/__init__.py
--rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.0.7/unibot_hn/board.py
--rw-r--r--   0        0        0    19870 2024-03-23 16:05:42.533817 unibot_hn-0.0.7/unibot_hn/camera.py
--rw-r--r--   0        0        0    12089 2024-03-25 08:19:31.953925 unibot_hn-0.0.7/unibot_hn/config_function.py
--rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.0.7/unibot_hn/img_processing.py
--rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.0.7/unibot_hn/robot_config.py
--rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.0.7/unibot_hn/robot_param_init.txt
--rw-r--r--   0        0        0     7727 2024-03-24 05:09:46.277825 unibot_hn-0.0.7/unibot_hn/servo_config_function.py
--rw-r--r--   0        0        0    21131 2024-03-24 13:53:44.440386 unibot_hn-0.0.7/unibot_hn/unibot.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.0.8/LICENSE
+-rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.0.8/README.md
+-rw-r--r--   0        0        0      316 2024-03-26 05:14:26.565442 unibot_hn-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-03-22 14:55:21.004090 unibot_hn-0.0.8/unibot_hn/.DS_Store
+-rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.0.8/unibot_hn/Misc.py
+-rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.0.8/unibot_hn/PID.py
+-rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.0.8/unibot_hn/__init__.py
+-rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.0.8/unibot_hn/board.py
+-rw-r--r--   0        0        0    19870 2024-03-23 16:05:42.533817 unibot_hn-0.0.8/unibot_hn/camera.py
+-rw-r--r--   0        0        0    12089 2024-03-26 05:14:10.015607 unibot_hn-0.0.8/unibot_hn/config_function.py
+-rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.0.8/unibot_hn/img_processing.py
+-rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.0.8/unibot_hn/robot_config.py
+-rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.0.8/unibot_hn/robot_param_init.txt
+-rw-r--r--   0        0        0     7727 2024-03-24 05:09:46.277825 unibot_hn-0.0.8/unibot_hn/servo_config_function.py
+-rw-r--r--   0        0        0    21130 2024-03-26 05:10:40.644892 unibot_hn-0.0.8/unibot_hn/unibot.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.0.8/PKG-INFO
```

### Comparing `unibot_hn-0.0.7/LICENSE` & `unibot_hn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/.DS_Store` & `unibot_hn-0.0.8/unibot_hn/.DS_Store`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/PID.py` & `unibot_hn-0.0.8/unibot_hn/PID.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/board.py` & `unibot_hn-0.0.8/unibot_hn/board.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/camera.py` & `unibot_hn-0.0.8/unibot_hn/camera.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/config_function.py` & `unibot_hn-0.0.8/unibot_hn/config_function.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/img_processing.py` & `unibot_hn-0.0.8/unibot_hn/img_processing.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/robot_config.py` & `unibot_hn-0.0.8/unibot_hn/robot_config.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/robot_param_init.txt` & `unibot_hn-0.0.8/unibot_hn/robot_param_init.txt`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/servo_config_function.py` & `unibot_hn-0.0.8/unibot_hn/servo_config_function.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.7/unibot_hn/unibot.py` & `unibot_hn-0.0.8/unibot_hn/unibot.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         self.chassis = MecanumChassis(self.board)
         self.gripper = Gripper(self.board)
         self.params = Device_Config('/root/unibot/robot_param_init.txt')
 
         servo_init_error_default = self.params.readconfsectionkeyvalue('SERVO_ERR_INIT')
         servo_init_direction_default = self.params.readconfsectionkeyvalue('SERVO_DIR_INIT')
         self.left_holder_servo_position = self.params.readconfsectionkeyvalue('LEFT_PUT_ROUND')
-        self.right_holder_servo_position = self.params.readconfsectionkeyvalue('RIGHT_PUT_ROUND')
+        self.right_holder_servo_position = self.params.readconfsectionkeyvalue('LEFT_GET_ROUND')
         self.robotic_arm = RoboticArm(self.board, servo_init_error_default, servo_init_direction_default)
         self.camera = Camera()
 
     def get_battery(self):
         return self.board.get_battery()
 
     def follow_line(self, point_index):
```

### Comparing `unibot_hn-0.0.7/PKG-INFO` & `unibot_hn-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibot_hn
-Version: 0.0.7
+Version: 0.0.8
 Summary: unibot_hn
 License: MIT
 Author: QuWan
 Requires-Python: >=3.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

