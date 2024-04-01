# Comparing `tmp/convictquandary-0.0.3.tar.gz` & `tmp/convictquandary-0.0.4.tar.gz`

## Comparing `convictquandary-0.0.3.tar` & `convictquandary-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 convictquandary-0.0.3/.flake8
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 convictquandary-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 convictquandary-0.0.3/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convictquandary-0.0.3/tox.ini
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 convictquandary-0.0.3/.github/workflows/test-and-publish.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/constants.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/game.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/player.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/player_logic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/utils.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/player_logics/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 convictquandary-0.0.3/src/convictquandary/player_logics/logic_always_defect_believe_truth.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 convictquandary-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 convictquandary-0.0.3/tests/test_game.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 convictquandary-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 convictquandary-0.0.3/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 convictquandary-0.0.3/README.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 convictquandary-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 convictquandary-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 convictquandary-0.0.4/.flake8
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 convictquandary-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 convictquandary-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convictquandary-0.0.4/tox.ini
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 convictquandary-0.0.4/.github/workflows/test-and-publish.yaml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/constants.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/game.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/player.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/player_logic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/utils.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/player_logics/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 convictquandary-0.0.4/src/convictquandary/player_logics/logic_always_defect_believe_truth.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 convictquandary-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 convictquandary-0.0.4/tests/test_game.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 convictquandary-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 convictquandary-0.0.4/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 convictquandary-0.0.4/README.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 convictquandary-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 convictquandary-0.0.4/PKG-INFO
```

### Comparing `convictquandary-0.0.3/.pre-commit-config.yaml` & `convictquandary-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/requirements.txt` & `convictquandary-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/tox.ini` & `convictquandary-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/.github/workflows/test-and-publish.yaml` & `convictquandary-0.0.4/.github/workflows/test-and-publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
           - "3.9"
           - "3.10"
           - "3.11"
           - "3.12"
 
     steps:
       - name: "Check out the repo"
-        uses: "actions/checkout@v2"
+        uses: "actions/checkout@v4"
 
       - name: "Set up Python"
-        uses: "actions/setup-python@v2"
+        uses: "actions/setup-python@v5"
         with:
           python-version: "${{ matrix.python-version }}"
 
       - name: "Install dependencies"
         run: |
           python -m pip install tox tox-gh-actions
 
@@ -53,18 +53,18 @@
 
   coverage:
     name: Coverage
     needs: lint-and-tests
     runs-on: ubuntu-latest
     steps:
       - name: "Check out the repo"
-        uses: "actions/checkout@v2"
+        uses: "actions/checkout@v4"
 
       - name: "Set up Python"
-        uses: "actions/setup-python@v2"
+        uses: "actions/setup-python@v5"
         with:
           python-version: "3.12"
 
       - name: "Install dependencies"
         run: |
           python -m pip install tox tox-gh-actions
 
@@ -99,15 +99,15 @@
       - lint-and-tests
       - coverage
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
```

### Comparing `convictquandary-0.0.3/src/convictquandary/game.py` & `convictquandary-0.0.4/src/convictquandary/game.py`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/src/convictquandary/player.py` & `convictquandary-0.0.4/src/convictquandary/player.py`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py` & `convictquandary-0.0.4/src/convictquandary/player_logics/logic_always_cooperate_believe_truth.py`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/src/convictquandary/player_logics/logic_always_defect_believe_truth.py` & `convictquandary-0.0.4/src/convictquandary/player_logics/logic_always_defect_believe_truth.py`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/tests/test_game.py` & `convictquandary-0.0.4/tests/test_game.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from convictquandary import Game, Player
+import pytest
+
+from convictquandary import Game, Player, utils
 from convictquandary.player_logics import (
     LogicAlwaysCooperateBelieveTruth,
     LogicAlwaysDefectBelieveTruth,
 )
 
 
 def test_1v1_game_always_defect_win():
@@ -26,7 +28,29 @@
 
 def test_1v1_game_always_cooperate_against_itself():
     player1 = Player(LogicAlwaysCooperateBelieveTruth)
     player2 = Player(LogicAlwaysCooperateBelieveTruth)
     game = Game(player1, player2, 200)
     game.play_game()
     assert game.get_game_result() == (600, 600), "Always cooperate not score 600"
+
+
+def test_1v1_game_get_players():
+    player1 = Player(LogicAlwaysCooperateBelieveTruth)
+    player2 = Player(LogicAlwaysCooperateBelieveTruth)
+    game = Game(player1, player2, 200)
+    p1, p2 = game.get_players()
+    assert (p1, p2) == (player1, player2), "Game returns correct players"
+
+
+def test_1v1_game_already_played():
+    player1 = Player(LogicAlwaysCooperateBelieveTruth)
+    player2 = Player(LogicAlwaysCooperateBelieveTruth)
+    game = Game(player1, player2, 200)
+    game.play_game()
+    with pytest.raises(ValueError, match="Game already finished"):
+        game.play_game()
+
+
+def test_utils_exception_factory():
+    with pytest.raises(ValueError, match="Test message"):
+        raise utils.exception_factory(ValueError, "Test message")
```

### Comparing `convictquandary-0.0.3/.gitignore` & `convictquandary-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/LICENSE` & `convictquandary-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/README.md` & `convictquandary-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/pyproject.toml` & `convictquandary-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `convictquandary-0.0.3/PKG-INFO` & `convictquandary-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: convictquandary
-Version: 0.0.3
+Version: 0.0.4
 Summary: A extension of the iterated prisoners dilemma tournaments by Axelrod
 Project-URL: Homepage, https://github.com/prashant94/convict_quandary
 Project-URL: Issues, https://github.com/prashant94/convict_quandary/issues
 Author-email: Prashant Sinha <prashantsinha94@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Prashant Sinha
```

