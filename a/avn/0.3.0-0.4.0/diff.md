# Comparing `tmp/avn-0.3.0.tar.gz` & `tmp/avn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avn-0.3.0.tar", max compression
+gzip compressed data, was "avn-0.4.0.tar", max compression
```

## Comparing `avn-0.3.0.tar` & `avn-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       23 2023-03-10 17:53:16.740334 avn-0.3.0/avn/__init__.py
--rw-r--r--   0        0        0    54902 2023-03-10 17:48:48.562412 avn-0.3.0/avn/acoustics.py
--rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.3.0/avn/avn.py
--rw-r--r--   0        0        0     7860 2021-11-04 18:21:52.806620 avn-0.3.0/avn/dataloading.py
--rw-r--r--   0        0        0    14928 2021-11-04 18:21:52.806620 avn-0.3.0/avn/plotting.py
--rw-r--r--   0        0        0    83983 2023-03-02 15:05:22.932147 avn-0.3.0/avn/segmentation.py
--rw-r--r--   0        0        0    90270 2023-03-02 15:43:11.871860 avn-0.3.0/avn/syntax.py
--rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.3.0/LICENSE
--rw-r--r--   0        0        0      878 2023-03-10 17:52:25.795055 avn-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1275 2021-05-13 15:54:00.000000 avn-0.3.0/README.md
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 avn-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-01 15:26:16.987651 avn-0.4.0/avn/__init__.py
+-rw-r--r--   0        0        0    54839 2023-03-10 20:46:13.255520 avn-0.4.0/avn/acoustics.py
+-rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.4.0/avn/avn.py
+-rw-r--r--   0        0        0     7864 2023-12-14 19:33:37.323506 avn-0.4.0/avn/dataloading.py
+-rw-r--r--   0        0        0    14928 2021-11-04 18:21:52.806620 avn-0.4.0/avn/plotting.py
+-rw-r--r--   0        0        0    83983 2023-03-02 15:05:22.932147 avn-0.4.0/avn/segmentation.py
+-rw-r--r--   0        0        0    90270 2023-03-10 20:40:35.473692 avn-0.4.0/avn/syntax.py
+-rw-r--r--   0        0        0    34081 2023-12-15 21:05:06.690502 avn-0.4.0/avn/timing.py
+-rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.4.0/LICENSE
+-rw-r--r--   0        0        0      878 2024-04-01 15:25:39.847897 avn-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1275 2021-05-13 15:54:00.000000 avn-0.4.0/README.md
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 avn-0.4.0/PKG-INFO
```

### Comparing `avn-0.3.0/avn/acoustics.py` & `avn-0.4.0/avn/acoustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,36 +651,36 @@
         ax2.plot(x_axis, feature_val, color = 'white', label = feature)
         ax2.set_ylabel(feature);
 
 
 class AcousticData:
     """Acoustic Feature data pertaining to a set of syllables in `syll_df`.
 
-        Args:
-            Bird_ID (str): String containing a unique identifier for the subject bird
-            syll_df (pd.DataFrame): pandas dataframe containing one row for every syllable 
+    Args:
+        Bird_ID (str): String containing a unique identifier for the subject bird.
+        syll_df (pd.DataFrame): pandas dataframe containing one row for every syllable 
             to be analyzed from the subject bird. It must contain columns *onsets* and *offsets* 
             which contain the timestamp in seconds at which the syllable occurs 
             within a file, and *files* which contains the name of the .wav file in 
             which the syllable is found. These can be generated through manual song
             annotation, or automated segmentation methods.
-            song_folder_path (str): Path to folder containing the .wav files of the songs in 
+        song_folder_path (str): Path to folder containing the .wav files of the songs in 
             `syll_df`. Should end with '/'. 
-            win_length (int, optional): Length of window over which to calculate each feature in samples. Defaults to 400.
-            hop_length (int, optional): Number of samples to advance between windows. Defaults to 40.
-            n_fft (int, optional): Length of the transformed axis of the output. If n is smaller than the length of the win_length, 
-                the input is cropped. If it is larger, the input is padded with zeros. Defaults to 1024.
-            max_F0 (int, optional): Maximum allowable fundamental frequency of signal in Hz. Defaults to 1830.
-            min_frequency (int, optional): Lower frequency cutoff in Hz. Only power at frequencies above this will contribute to
-                feature calculation. Defaults to 380.
-            freq_range (float, optional): Proportion of power spectrum frequency bins to consider. Defaults to 0.5, 
-                meaning we only consider the lower half of the frequency range. This is consistent with SAP.
-            baseline_amp (int, optional): Baseline amplitude used to calculated amplitude in dB. Defaults to 70.
-            fmax_yin (int, optional): Maximum frequency in Hz used to estimate fundamental frequency with the YIN algorithm. 
-                Defaults to 8000.
+        win_length (int, optional): Length of window over which to calculate each feature in samples. Defaults to 400.
+        hop_length (int, optional): Number of samples to advance between windows. Defaults to 40.
+        n_fft (int, optional): Length of the transformed axis of the output. If n is smaller than the length of the win_length, 
+            the input is cropped. If it is larger, the input is padded with zeros. Defaults to 1024.
+        max_F0 (int, optional): Maximum allowable fundamental frequency of signal in Hz. Defaults to 1830.
+        min_frequency (int, optional): Lower frequency cutoff in Hz. Only power at frequencies above this will contribute to
+            feature calculation. Defaults to 380.
+        freq_range (float, optional): Proportion of power spectrum frequency bins to consider. Defaults to 0.5, 
+            meaning we only consider the lower half of the frequency range. This is consistent with SAP.
+        baseline_amp (int, optional): Baseline amplitude used to calculated amplitude in dB. Defaults to 70.
+        fmax_yin (int, optional): Maximum frequency in Hz used to estimate fundamental frequency with the YIN algorithm. 
+            Defaults to 8000.
         """
     
     def __init__(self, Bird_ID, syll_df, song_folder_path, 
                  win_length = 400, hop_length = 40, n_fft = 1024, 
                  max_F0 = 1830, min_frequency = 380, freq_range = 0.5, 
                  baseline_amp = 70, fmax_yin = 8000, ):
         """Acoustic Feature data pertaining to a set of syllables in `syll_df`.
```

### Comparing `avn-0.3.0/avn/dataloading.py` & `avn-0.4.0/avn/dataloading.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         ----------
         file_path : str
             Path to the local .wav file to be loaded as a SongFile object.
              
         """
         self.sample_rate, self.data = wavfile.read(file_path)
         self.data = self.data.astype(float)
-        self.duration = librosa.get_duration(self.data, sr = self.sample_rate)
+        self.duration = librosa.get_duration(y = self.data, sr = self.sample_rate)
         self.file_path = file_path
         
         #get file name -- This may be windows specific. 
         file_name_regex = re.compile("\\\\")
         self.file_name = file_name_regex.split(self.file_path)[-1]
                                                   
     def bandpass_filter(self, lower_cutoff, upper_cutoff):
```

### Comparing `avn-0.3.0/avn/plotting.py` & `avn-0.4.0/avn/plotting.py`

 * *Files identical despite different names*

### Comparing `avn-0.3.0/avn/segmentation.py` & `avn-0.4.0/avn/segmentation.py`

 * *Files identical despite different names*

### Comparing `avn-0.3.0/avn/syntax.py` & `avn-0.4.0/avn/syntax.py`

 * *Files identical despite different names*

### Comparing `avn-0.3.0/pyproject.toml` & `avn-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avn"
-version = "0.3.0"
+version = "0.4.0"
 description = "Package for zebra finch song analysis."
 authors = ["Therese Koch"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 documentation = "https://avn.readthedocs.io/en/latest/"
 homepage = "https://github.com/theresekoch/avn"
 repository = "https://github.com/theresekoch/avn"
```

### Comparing `avn-0.3.0/README.md` & `avn-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `avn-0.3.0/PKG-INFO` & `avn-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avn
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for zebra finch song analysis.
 Home-page: https://github.com/theresekoch/avn
 License: GNU General Public License v3.0
 Author: Therese Koch
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

