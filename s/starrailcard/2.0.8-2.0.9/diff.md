# Comparing `tmp/starrailcard-2.0.8.tar.gz` & `tmp/starrailcard-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.0.8.tar", max compression
+gzip compressed data, was "starrailcard-2.0.9.tar", max compression
```

## Comparing `starrailcard-2.0.8.tar` & `starrailcard-2.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.0.8/LICENSE
--rw-r--r--   0        0        0     1147 2024-03-28 19:12:57.158941 starrailcard-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.0.8/README.md
--rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.0.8/starrailcard/__init__.py
--rw-r--r--   0        0        0     9709 2024-03-28 17:26:11.577562 starrailcard-2.0.8/starrailcard/client.py
--rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.0.8/starrailcard/requirements.txt
--rw-r--r--   0        0        0      969 2024-03-28 17:11:10.264563 starrailcard-2.0.8/starrailcard/src/api/api.py
--rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.0.8/starrailcard/src/assets/font/font_hsr.ttf
--rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.0.8/starrailcard/src/data/avatar.json
--rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.0.8/starrailcard/src/data/element.json
--rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.0.8/starrailcard/src/data/keys.json
--rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.0.8/starrailcard/src/data/paths.json
--rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.0.8/starrailcard/src/data/relict_sets.json
--rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.0.8/starrailcard/src/data/stats.json
--rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.0.8/starrailcard/src/data/weapons.json
--rw-r--r--   0        0        0     6680 2024-03-16 23:04:12.294325 starrailcard-2.0.8/starrailcard/src/generator/style_profile_phone.py
--rw-r--r--   0        0        0    23968 2024-03-24 23:40:49.094126 starrailcard-2.0.8/starrailcard/src/generator/style_relict_score.py
--rw-r--r--   0        0        0    29840 2024-03-28 18:58:01.974256 starrailcard-2.0.8/starrailcard/src/generator/style_ticket.py
--rw-r--r--   0        0        0     8410 2024-03-13 13:47:49.948737 starrailcard-2.0.8/starrailcard/src/model/api_mihomo.py
--rw-r--r--   0        0        0     4757 2024-03-27 19:18:51.084890 starrailcard-2.0.8/starrailcard/src/model/StarRailCard.py
--rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.0.8/starrailcard/src/model/style.py
--rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.0.8/starrailcard/src/model/ukrainization_model.py
--rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.0.8/starrailcard/src/model/utils_model.py
--rw-r--r--   0        0        0      373 2024-03-28 19:05:12.724879 starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/max.json
--rw-r--r--   0        0        0       49 2024-03-28 19:05:13.041062 starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-r--r--   0        0        0     3434 2024-03-28 19:05:13.341867 starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-r--r--   0        0        0    87319 2024-03-28 19:05:13.882857 starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/score.json
--rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.0.8/starrailcard/src/tools/calculator/src/utils.py
--rw-r--r--   0        0        0     5733 2024-03-28 17:53:31.209355 starrailcard-2.0.8/starrailcard/src/tools/calculator/stats.py
--rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.0.8/starrailcard/src/tools/cashe.py
--rw-r--r--   0        0        0      563 2024-03-28 16:30:39.886551 starrailcard-2.0.8/starrailcard/src/tools/enums.py
--rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.0.8/starrailcard/src/tools/git.py
--rw-r--r--   0        0        0     6100 2024-03-28 17:26:04.740937 starrailcard-2.0.8/starrailcard/src/tools/http.py
--rw-r--r--   0        0        0      940 2024-03-28 18:26:46.684860 starrailcard-2.0.8/starrailcard/src/tools/json_data.py
--rw-r--r--   0        0        0     6122 2024-02-25 12:22:45.869423 starrailcard-2.0.8/starrailcard/src/tools/options.py
--rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.0.8/starrailcard/src/tools/pill/__init__.py
--rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.0.8/starrailcard/src/tools/pill/color.py
--rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.0.8/starrailcard/src/tools/pill/color_controle.py
--rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.0.8/starrailcard/src/tools/pill/grandiend_v2.py
--rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.0.8/starrailcard/src/tools/pill/grandient_v1.py
--rw-r--r--   0        0        0     3833 2024-03-17 12:15:47.665776 starrailcard-2.0.8/starrailcard/src/tools/pill/image_controle.py
--rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.0.8/starrailcard/src/tools/pill/style_editor.py
--rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.0.8/starrailcard/src/tools/pill/text_controle.py
--rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.0.8/starrailcard/src/tools/translator.py
--rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.0.8/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.0.8/starrailcard/src/tools/ukrainization.py
--rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.0.8/starrailcard/utils.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 starrailcard-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.0.9/LICENSE
+-rw-r--r--   0        0        0     1147 2024-04-01 14:18:45.022456 starrailcard-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.0.9/README.md
+-rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.0.9/starrailcard/__init__.py
+-rw-r--r--   0        0        0     9709 2024-03-28 17:26:11.577562 starrailcard-2.0.9/starrailcard/client.py
+-rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.0.9/starrailcard/requirements.txt
+-rw-r--r--   0        0        0      969 2024-03-28 17:11:10.264563 starrailcard-2.0.9/starrailcard/src/api/api.py
+-rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.0.9/starrailcard/src/assets/font/font_hsr.ttf
+-rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.0.9/starrailcard/src/data/avatar.json
+-rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.0.9/starrailcard/src/data/element.json
+-rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.0.9/starrailcard/src/data/keys.json
+-rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.0.9/starrailcard/src/data/paths.json
+-rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.0.9/starrailcard/src/data/relict_sets.json
+-rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.0.9/starrailcard/src/data/stats.json
+-rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.0.9/starrailcard/src/data/weapons.json
+-rw-r--r--   0        0        0     6680 2024-03-16 23:04:12.294325 starrailcard-2.0.9/starrailcard/src/generator/style_profile_phone.py
+-rw-r--r--   0        0        0    23968 2024-03-24 23:40:49.094126 starrailcard-2.0.9/starrailcard/src/generator/style_relict_score.py
+-rw-r--r--   0        0        0    29840 2024-03-28 18:58:01.974256 starrailcard-2.0.9/starrailcard/src/generator/style_ticket.py
+-rw-r--r--   0        0        0     8410 2024-03-13 13:47:49.948737 starrailcard-2.0.9/starrailcard/src/model/api_mihomo.py
+-rw-r--r--   0        0        0     4757 2024-03-27 19:18:51.084890 starrailcard-2.0.9/starrailcard/src/model/StarRailCard.py
+-rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.0.9/starrailcard/src/model/style.py
+-rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.0.9/starrailcard/src/model/ukrainization_model.py
+-rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.0.9/starrailcard/src/model/utils_model.py
+-rw-r--r--   0        0        0      373 2024-03-28 19:05:12.724879 starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-r--r--   0        0        0       49 2024-03-28 19:05:13.041062 starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-r--r--   0        0        0     3434 2024-03-28 19:05:13.341867 starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-r--r--   0        0        0    87319 2024-03-28 19:05:13.882857 starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.0.9/starrailcard/src/tools/calculator/src/utils.py
+-rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.0.9/starrailcard/src/tools/calculator/stats.py
+-rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.0.9/starrailcard/src/tools/cashe.py
+-rw-r--r--   0        0        0      563 2024-03-28 16:30:39.886551 starrailcard-2.0.9/starrailcard/src/tools/enums.py
+-rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.0.9/starrailcard/src/tools/git.py
+-rw-r--r--   0        0        0     6100 2024-03-28 17:26:04.740937 starrailcard-2.0.9/starrailcard/src/tools/http.py
+-rw-r--r--   0        0        0      940 2024-03-28 18:26:46.684860 starrailcard-2.0.9/starrailcard/src/tools/json_data.py
+-rw-r--r--   0        0        0     6122 2024-02-25 12:22:45.869423 starrailcard-2.0.9/starrailcard/src/tools/options.py
+-rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.0.9/starrailcard/src/tools/pill/__init__.py
+-rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.0.9/starrailcard/src/tools/pill/color.py
+-rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.0.9/starrailcard/src/tools/pill/color_controle.py
+-rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.0.9/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.0.9/starrailcard/src/tools/pill/grandient_v1.py
+-rw-r--r--   0        0        0     3833 2024-03-17 12:15:47.665776 starrailcard-2.0.9/starrailcard/src/tools/pill/image_controle.py
+-rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.0.9/starrailcard/src/tools/pill/style_editor.py
+-rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.0.9/starrailcard/src/tools/pill/text_controle.py
+-rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.0.9/starrailcard/src/tools/translator.py
+-rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.0.9/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.0.9/starrailcard/src/tools/ukrainization.py
+-rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.0.9/starrailcard/utils.py
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 starrailcard-2.0.9/PKG-INFO
```

### Comparing `starrailcard-2.0.8/LICENSE` & `starrailcard-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/pyproject.toml` & `starrailcard-2.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starrailcard"
-version = "2.0.8"
+version = "2.0.9"
 description = "This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players."
 authors = ["DEViantUA <deviantapi@gmail.com>"]
 license = "MIT License with Additional Restrictions"
 
 readme = 'README.md'  # Markdown files are supported
 
 repository = "https://github.com/DEViantUA/StarRailCard"
```

### Comparing `starrailcard-2.0.8/README.md` & `starrailcard-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/client.py` & `starrailcard-2.0.9/starrailcard/client.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/api/api.py` & `starrailcard-2.0.9/starrailcard/src/api/api.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.0.9/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/data/avatar.json` & `starrailcard-2.0.9/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/data/relict_sets.json` & `starrailcard-2.0.9/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/data/stats.json` & `starrailcard-2.0.9/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/data/weapons.json` & `starrailcard-2.0.9/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.0.9/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.0.9/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.0.9/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.0.9/starrailcard/src/model/api_mihomo.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.0.9/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/model/style.py` & `starrailcard-2.0.9/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/model/utils_model.py` & `starrailcard-2.0.9/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.0.9/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.0.9/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.0.9/starrailcard/src/tools/calculator/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 n = "FODFCDE"
 r = "kLMHBJpWBQqBJOgJP@LQGaLW"
 k = "5ceb5d1b20945b82dd21c7`g2909g1e4711d802b"
 
 
 _LINK_SCORE = "https://raw.githubusercontent.com/"+decrypt_url(n,42)+"/"+decrypt_url(r,35)+"/"+"main"+"/generate/weight.json"
 _LINK_DATA = "https://raw.githubusercontent.com/"+decrypt_url(n,42)+"/"+decrypt_url(r,35)+"/"+"main"+"/generate/{name}.json"
-_LINK_SCORE_V2 = "https://raw.githubusercontent.com/Mar-7th/StarRailScore/master/score.json"
+_LINK_SCORE_V2 = "https://raw.githubusercontent.com/"+decrypt_url(n,42)+"/StarRailScore/master/score.json"
 
 _PATH = Path(__file__).parent /"src"/"assets"
 
 _PATH_FILE_NAME = [
     "max",
     "relic_id",
     "rolls",
```

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/cashe.py` & `starrailcard-2.0.9/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/enums.py` & `starrailcard-2.0.9/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/git.py` & `starrailcard-2.0.9/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/http.py` & `starrailcard-2.0.9/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/json_data.py` & `starrailcard-2.0.9/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/options.py` & `starrailcard-2.0.9/starrailcard/src/tools/options.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/color.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/image_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.0.9/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/translator.py` & `starrailcard-2.0.9/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/treePaths.py` & `starrailcard-2.0.9/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.0.9/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/starrailcard/utils.py` & `starrailcard-2.0.9/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.0.8/PKG-INFO` & `starrailcard-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.0.8
+Version: 2.0.9
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 License: MIT License with Additional Restrictions
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Author: DEViantUA
 Author-email: deviantapi@gmail.com
 Requires-Python: >=3.9,<4.0
```

