# Comparing `tmp/qodex_cameras-2.1.3-py3-none-any.whl.zip` & `tmp/qodex_cameras-2.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 39897 bytes, number of entries: 18
+Zip file size: 39904 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 06:46 qodex_cameras/__init__.py
 -rw-rw-rw-  2.0 fat      166 b- defN 23-May-02 11:08 qodex_cameras/functions.py
 -rw-rw-rw-  2.0 fat     2950 b- defN 24-Feb-26 14:00 qodex_cameras/main.py
 -rw-rw-rw-  2.0 fat     3420 b- defN 24-Feb-26 13:21 qodex_cameras/mixins.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-12 08:58 qodex_cameras/settings.py
--rw-rw-rw-  2.0 fat     2084 b- defN 24-Apr-01 13:48 qodex_cameras/video_saver.py
+-rw-rw-rw-  2.0 fat     2084 b- defN 24-Apr-01 14:29 qodex_cameras/video_saver.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 04:44 qodex_cameras/other/__init__.py
 -rw-rw-rw-  2.0 fat     6078 b- defN 23-May-02 04:46 qodex_cameras/other/pyhik_mode.py
 -rw-rw-rw-  2.0 fat     7365 b- defN 23-May-12 06:25 qodex_cameras/photos/Test.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 05:38 qodex_cameras/photos/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 12:07 qodex_cameras/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 24-Feb-21 14:19 qodex_cameras/tests/main_tests.py
 -rw-rw-rw-  2.0 fat    26529 b- defN 23-May-12 08:58 qodex_cameras/tests/test.png
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-01 13:51 qodex_cameras-2.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      304 b- defN 24-Apr-01 13:51 qodex_cameras-2.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 13:51 qodex_cameras-2.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-01 13:51 qodex_cameras-2.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1508 b- defN 24-Apr-01 13:51 qodex_cameras-2.1.3.dist-info/RECORD
-18 files, 53357 bytes uncompressed, 37399 bytes compressed:  29.9%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-01 14:30 qodex_cameras-2.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      304 b- defN 24-Apr-01 14:30 qodex_cameras-2.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 14:30 qodex_cameras-2.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-01 14:30 qodex_cameras-2.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1508 b- defN 24-Apr-01 14:30 qodex_cameras-2.1.4.dist-info/RECORD
+18 files, 53357 bytes uncompressed, 37406 bytes compressed:  29.9%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: qodex_cameras/tests/main_tests.py
 Comment: 
 
 Filename: qodex_cameras/tests/test.png
 Comment: 
 
-Filename: qodex_cameras-2.1.3.dist-info/LICENSE
+Filename: qodex_cameras-2.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: qodex_cameras-2.1.3.dist-info/METADATA
+Filename: qodex_cameras-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: qodex_cameras-2.1.3.dist-info/WHEEL
+Filename: qodex_cameras-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_cameras-2.1.3.dist-info/top_level.txt
+Filename: qodex_cameras-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_cameras-2.1.3.dist-info/RECORD
+Filename: qodex_cameras-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qodex_cameras/video_saver.py

```diff
@@ -18,41 +18,43 @@
         # The %03d format will number the files sequentially, starting from 000
         output_filepath_pattern = os.path.join(cwd, self.output_path_name)
         print(output_filepath_pattern)
         # Build the ffmpeg command
         command = [
             'ffmpeg',
             '-i', self.rtsp_url,
-            '-c:v', 'copy',
-            '-c:a', 'aac',
-            '-f', 'segment',
-            '-segment_time', '600',  # 600 seconds = 10 minutes
-            '-reset_timestamps', '1',
+            #'-c:v', 'copy',
+            #'-c:a', 'aac',
+            #'-f', 'segment',
+            #'-segment_time', '600',  # 600 seconds = 10 minutes
+            #'-reset_timestamps', '1',
             output_filepath_pattern
         ]
 
         # Try running the command
         try:
             print("Attempting to connect to RTSP stream...")
-            self.proc = subprocess.Popen(command, stdout=subprocess.PIPE,
-                                         shell=False, stdin=subprocess.DEVNULL)
+            self.proc = subprocess.Popen(
+                command, stdout=subprocess.PIPE,
+                shell=False, stdin=subprocess.DEVNULL)
             # self.proc = subprocess.run(command, check=True)
         except subprocess.CalledProcessError:
             print(
                 "Failed to connect to RTSP stream or encountered an error during recording.")
         except KeyboardInterrupt:
             print("\nRecording interrupted by user.")
 
     def stop_record(self):
         print("Stopping video recording...")
         self.record_in_progress = False
         print(self.proc)
         if self.proc:
             handle = self.proc
-            os.killpg(os.getpgid(handle.pid), signal.SIGINT)
+            #s.killpg(os.getpgid(handle.pid), signal.SIGINT)
+
             # self.proc.kill()
 
 
 if __name__ == "__main__":
     d = RTSPVideoWriterObject(
         "rtsp://admin:Assa+123@192.168.60.108:554/Streaming/Channels/101")
     d.start_record()
```

## Comparing `qodex_cameras-2.1.3.dist-info/LICENSE` & `qodex_cameras-2.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qodex_cameras-2.1.3.dist-info/RECORD` & `qodex_cameras-2.1.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 qodex_cameras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/functions.py,sha256=elNHnnx3zelcKnAOLK3E6ETMpV3PZPXfWclPRYSqiZA,166
 qodex_cameras/main.py,sha256=B-zYsIiD9j2nEA2VHG9PEwTdbMFr9FTd15_aWPV5vP8,2950
 qodex_cameras/mixins.py,sha256=DAl-7bRFCuKAQCOfwPum-O6meBmrm6r41SGSd3fLnFM,3420
 qodex_cameras/settings.py,sha256=xupNck2qOhJLj0WQjB47Z6dm179vhVF1FJ-dDcgX4c0,384
-qodex_cameras/video_saver.py,sha256=1Vl5CT2_tQwFw6C_o96H_-dGtnG0h9WsW8e0MT-gyxk,2084
+qodex_cameras/video_saver.py,sha256=pEuZEzhF9bMgH74fGob30HmaU2Qa81UyLByw2DQSQ6c,2084
 qodex_cameras/other/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/other/pyhik_mode.py,sha256=FyG_QWVdcTi5dnSwv3Iq-L0H4PYW6wKBeVJpkYRt58Q,6078
 qodex_cameras/photos/Test.png,sha256=v54Of9PyXTQ-X6_ji_105kC2ISyuxG6UxJDBzcdV4ac,7365
 qodex_cameras/photos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/main_tests.py,sha256=2i8_idlYsYF6jL10A36VtsOPbH-HofShSKPyBkdVAPo,1372
 qodex_cameras/tests/test.png,sha256=EZ4YZtPhTRLJBM2ZMr-ZyXqVMKgYlmW-25syShwy_8s,26529
-qodex_cameras-2.1.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-qodex_cameras-2.1.3.dist-info/METADATA,sha256=qGpK5iASii8GoY6MkEHJW7TjXV_OWdkw17gTO36AYjA,304
-qodex_cameras-2.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-qodex_cameras-2.1.3.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
-qodex_cameras-2.1.3.dist-info/RECORD,,
+qodex_cameras-2.1.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+qodex_cameras-2.1.4.dist-info/METADATA,sha256=PitnrzW4kiIr1kMtbDWPlxWYw-xaCgIaUwDFtvXCgGs,304
+qodex_cameras-2.1.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+qodex_cameras-2.1.4.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
+qodex_cameras-2.1.4.dist-info/RECORD,,
```

