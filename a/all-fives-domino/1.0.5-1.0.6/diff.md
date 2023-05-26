# Comparing `tmp/all-fives-domino-1.0.5.tar.gz` & `tmp/all-fives-domino-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all-fives-domino-1.0.5.tar", last modified: Fri May 26 21:15:55 2023, max compression
+gzip compressed data, was "all-fives-domino-1.0.6.tar", last modified: Fri May 26 22:11:20 2023, max compression
```

## Comparing `all-fives-domino-1.0.5.tar` & `all-fives-domino-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-26 21:15:41.000000 all-fives-domino-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/all_fives_domino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/main/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/game/
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/game/DominoRound.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/game/Piece.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4014 2023-05-26 21:15:41.000000 all-fives-domino-1.0.5/src/main/game/__pycache__/Piece.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/main/game/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/main/player/
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.5/src/main/player/Brain.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/player/Hand.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/player/Player.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/game/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/game/test_pieces.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-26 21:15:43.000000 all-fives-domino-1.0.5/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.889482 all-fives-domino-1.0.6/all_fives_domino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-26 22:11:20.000000 all-fives-domino-1.0.6/all_fives_domino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-05-26 22:11:20.000000 all-fives-domino-1.0.6/all_fives_domino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 22:11:20.000000 all-fives-domino-1.0.6/all_fives_domino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-26 22:11:20.000000 all-fives-domino-1.0.6/all_fives_domino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.889482 all-fives-domino-1.0.6/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.889482 all-fives-domino-1.0.6/src/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.6/src/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.6/src/main/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/game/
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/main/game/DominoRound.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/main/game/Piece.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/main/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/main/game/__pycache__/DominoRound.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     4585 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/main/game/__pycache__/Piece.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.6/src/main/game/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/player/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.6/src/main/player/Brain.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/main/player/Hand.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/main/player/Player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/main/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/main/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/main/player/__pycache__/Hand.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/main/player/__pycache__/Player.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/main/player/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.893482 all-fives-domino-1.0.6/src/test/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.6/src/test/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/src/test/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.6/src/test/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/src/test/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.6/src/test/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)    26801 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/test/game/test_pieces.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/test/game/test_round.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/src/test/player/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/test/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 22:11:20.897482 all-fives-domino-1.0.6/src/test/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/test/player/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-05-26 22:11:06.000000 all-fives-domino-1.0.6/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-26 22:06:49.000000 all-fives-domino-1.0.6/src/test/player/test_hand.py
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-26 22:11:08.000000 all-fives-domino-1.0.6/version.txt
```

### Comparing `all-fives-domino-1.0.5/LICENSE` & `all-fives-domino-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.5/all_fives_domino.egg-info/SOURCES.txt` & `all-fives-domino-1.0.6/all_fives_domino.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,29 @@
 src/__init__.py
 src/__pycache__/__init__.cpython-311.pyc
 src/main/__init__.py
 src/main/__pycache__/__init__.cpython-311.pyc
 src/main/game/DominoRound.py
 src/main/game/Piece.py
 src/main/game/__init__.py
+src/main/game/__pycache__/DominoRound.cpython-311.pyc
 src/main/game/__pycache__/Piece.cpython-311.pyc
 src/main/game/__pycache__/__init__.cpython-311.pyc
 src/main/player/Brain.py
 src/main/player/Hand.py
 src/main/player/Player.py
 src/main/player/__init__.py
+src/main/player/__pycache__/Hand.cpython-311.pyc
+src/main/player/__pycache__/Player.cpython-311.pyc
+src/main/player/__pycache__/__init__.cpython-311.pyc
 src/test/__init__.py
 src/test/__pycache__/__init__.cpython-311.pyc
 src/test/game/__init__.py
 src/test/game/test_pieces.py
+src/test/game/test_round.py
 src/test/game/__pycache__/__init__.cpython-311.pyc
-src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
+src/test/player/__init__.py
+src/test/player/test_hand.py
+src/test/player/__pycache__/__init__.cpython-311.pyc
+src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
```

### Comparing `all-fives-domino-1.0.5/setup.py` & `all-fives-domino-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.5/src/main/game/DominoRound.py` & `all-fives-domino-1.0.6/src/main/game/DominoRound.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import Union, List, Tuple
 
 from src.main.game.Piece import domino_set, Piece
 from src.main.player.Player import Player
-from src.main.player.Brain import Brain
-from src.main.player.Hand import Hand
 
 
 class DominoRound:
-    def __init__(self, brain1: Brain, brain2: Brain, begins: Union[Brain, None]):
+    def __init__(self, brain1: "Brain", brain2: "Brain", begins: Union["Brain", None]):
         self.pool = domino_set()
         self.origin: Union[Piece, None] = None
         self.player1 = Player(brain1, self)
         self.player2 = Player(brain2, self)
         self.current_player = self.player1 if begins == brain1 else (self.player2 if begins == brain2 else None)
         self.has_crossing = False
 
@@ -39,26 +37,28 @@
                 if piece in self.player1.hand:
                     self.current_player = self.player1
                     return piece
                 if piece in self.player2.hand:
                     self.current_player = self.player1
                     return piece
 
-    def score_piece(self, piece: Piece, depth=28):
+    @staticmethod
+    def score_piece(piece: Piece, depth=28):
         piece_score = 0
 
-
+        if piece.linked_to is None and piece.linked == []:
+            return piece.points
 
         return piece_score
 
     def score(self):
         score = self.score_piece(self.origin)
         self.current_player.score += score
 
-    def play(self, player: Player, piece: Piece, origin: Union[Piece, None], close = False):
+    def play(self, player: Player, piece: Piece, origin: Union[Piece, None], close=False):
         if piece not in player.hand:
             raise Exception(f"Player attempted to play {piece}, but it's not in their hand")
 
         if piece.is_double and self.has_crossing and close:
             piece.closed = True
 
         player.hand.pop(piece)
```

### Comparing `all-fives-domino-1.0.5/src/main/game/Piece.py` & `all-fives-domino-1.0.6/src/main/game/Piece.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,26 +11,33 @@
 
         linked: List[Piece]     -> Pieces played from this Piece
         is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece
         is_double: Bool         -> Whether both sides of the piece show the same number
         closed: Bool            -> If a double piece is closed (face down), nothing can be appended to it
         points: int             -> Point value of the piece, which is the combined value of both sides
         """
+        if a < 0 or b < 0 or a > 6 or b > 6:
+            raise ValueError(f"Domino Piece sides can only have values 0-6, got [{a}|{b}]")
+
         self.sides = sorted([a, b])
         self.linked: List[Piece] = []
         self.linked_to: Union[Piece, None] = None
         self.is_crossing = False
         self.is_double = self.sides[0] == self.sides[1]
         self.closed = False
         self.points = sum(self.sides)
 
     def append(self, piece):
         self.linked.append(piece)
 
-    def __repr__(self):
+    def unlinked_side(self, other: "Piece") -> int:
+        a, b = self.sides
+        return b if a in other.sides else a
+
+    def __str__(self):
         """Simple visual representation using die face Unicode symbols"""
         if self.closed:
             closed = u"\u25A9"
             return f"[{closed}|{closed}]"
 
         sides = [
             u"\u25A1",
@@ -40,17 +47,21 @@
             u"\u2683",
             u"\u2684",
             u"\u2685"
         ]
 
         return f"[{sides[self.sides[0]]}|{sides[self.sides[1]]}]"
 
+    def __repr__(self):
+        """Use string representation"""
+        return str(self)
+
     def __hash__(self):
-        """Integer representation, e.g. 64 for a [4|6] piece"""
-        return self.sides[1] * 10 + self.sides[0]
+        """Integer representation, e.g. 46 for a [4|6] piece"""
+        return self.sides[0] * 10 + self.sides[1]
 
     def __eq__(self, other):
         """Returns whether the pieces are equal based on their hash"""
         return hash(self) == hash(other)
 
     def __lt__(self, other):
         """Returns whether a piece is bigger based on point value"""
@@ -64,12 +75,8 @@
 def domino_set():
     pieces = set()
     for i in range(7):
         for j in range(7):
             if i <= j:
                 pieces.add(Piece(i, j))
 
-    piece = Piece(7, 7)
-    piece.closed = True
-    pieces.add(piece)
-
     return sorted(pieces)
```

### Comparing `all-fives-domino-1.0.5/src/main/game/__pycache__/Piece.cpython-311.pyc` & `all-fives-domino-1.0.6/src/main/game/__pycache__/Piece.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x75217164 (Fri May 26 21:15:33 2023 UTC)
-files sz: 2324
+moddate:  0x792d7164 (Fri May 26 22:06:49 2023 UTC)
+files sz: 2603
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a016d025a02010002004700640284006403a6
@@ -25,31 +25,31 @@
                 22 LOAD_CONST               2 (<code object Piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 4>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               3 ('Piece')
                 28 PRECALL                  2
                 32 CALL                     2
                 42 STORE_NAME               3 (Piece)
    
-    64          44 LOAD_CONST               4 (<code object domino_set, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 64>)
+    75          44 LOAD_CONST               4 (<code object domino_set, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 75>)
                 46 MAKE_FUNCTION            0
                 48 STORE_NAME               4 (domino_set)
                 50 LOAD_CONST               5 (None)
                 52 RETURN_VALUE
    consts
       0
       ('List', 'Union')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264016503640265036604640384045a04640484
-            005a05640584005a06640684005a07640784005a08640884005a09640984
-            005a0a640a5300
+            005a0564056400640665036604640784045a06640884005a07640984005a
+            08640a84005a09640b84005a0a640c84005a0b640d84005a0c640e5300
            4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Piece')
                        8 STORE_NAME               2 (__qualname__)
          
            5          10 LOAD_CONST               1 ('a')
@@ -57,130 +57,180 @@
                       14 LOAD_CONST               2 ('b')
                       16 LOAD_NAME                3 (int)
                       18 BUILD_TUPLE              4
                       20 LOAD_CONST               3 (<code object __init__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 5>)
                       22 MAKE_FUNCTION            4 (annotations)
                       24 STORE_NAME               4 (__init__)
          
-          26          26 LOAD_CONST               4 (<code object append, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 26>)
+          29          26 LOAD_CONST               4 (<code object append, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 29>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (append)
          
-          29          32 LOAD_CONST               5 (<code object __repr__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 29>)
-                      34 MAKE_FUNCTION            0
-                      36 STORE_NAME               6 (__repr__)
-         
-          47          38 LOAD_CONST               6 (<code object __hash__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 47>)
-                      40 MAKE_FUNCTION            0
-                      42 STORE_NAME               7 (__hash__)
-         
-          51          44 LOAD_CONST               7 (<code object __eq__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 51>)
-                      46 MAKE_FUNCTION            0
-                      48 STORE_NAME               8 (__eq__)
-         
-          55          50 LOAD_CONST               8 (<code object __lt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 55>)
-                      52 MAKE_FUNCTION            0
-                      54 STORE_NAME               9 (__lt__)
-         
-          59          56 LOAD_CONST               9 (<code object __gt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 59>)
-                      58 MAKE_FUNCTION            0
-                      60 STORE_NAME              10 (__gt__)
-                      62 LOAD_CONST              10 (None)
-                      64 RETURN_VALUE
+          32          32 LOAD_CONST               5 ('other')
+                      34 LOAD_CONST               0 ('Piece')
+                      36 LOAD_CONST               6 ('return')
+                      38 LOAD_NAME                3 (int)
+                      40 BUILD_TUPLE              4
+                      42 LOAD_CONST               7 (<code object unlinked_side, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 32>)
+                      44 MAKE_FUNCTION            4 (annotations)
+                      46 STORE_NAME               6 (unlinked_side)
+         
+          36          48 LOAD_CONST               8 (<code object __str__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 36>)
+                      50 MAKE_FUNCTION            0
+                      52 STORE_NAME               7 (__str__)
+         
+          54          54 LOAD_CONST               9 (<code object __repr__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 54>)
+                      56 MAKE_FUNCTION            0
+                      58 STORE_NAME               8 (__repr__)
+         
+          58          60 LOAD_CONST              10 (<code object __hash__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 58>)
+                      62 MAKE_FUNCTION            0
+                      64 STORE_NAME               9 (__hash__)
+         
+          62          66 LOAD_CONST              11 (<code object __eq__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 62>)
+                      68 MAKE_FUNCTION            0
+                      70 STORE_NAME              10 (__eq__)
+         
+          66          72 LOAD_CONST              12 (<code object __lt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 66>)
+                      74 MAKE_FUNCTION            0
+                      76 STORE_NAME              11 (__lt__)
+         
+          70          78 LOAD_CONST              13 (<code object __gt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 70>)
+                      80 MAKE_FUNCTION            0
+                      82 STORE_NAME              12 (__gt__)
+                      84 LOAD_CONST              14 (None)
+                      86 RETURN_VALUE
          consts
             'Piece'
             'a'
             'b'
             code
                argcount  : 3
                nlocals   : 3
-               stacksize : 4
+               stacksize : 7
                flags     : 3
                code
-                  0x97007401000000000000000000007c017c026702a6010000ab01000000
-                  00000000007c005f01000000000000000067007c005f0200000000000000
-                  0064017c005f03000000000000000064027c005f0400000000000000007c
-                  006a0100000000000000006403190000000000000000007c006a01000000
-                  00000000006404190000000000000000006b02000000007c005f05000000
-                  000000000064027c005f060000000000000000740f000000000000000000
-                  007c006a010000000000000000a6010000ab0100000000000000007c005f
-                  08000000000000000064015300
+                  0x97007c0164016b000000000073127c0264016b0000000000730c7c0164
+                  026b040000000073067c0264026b04000000007216740100000000000000
+                  00000064037c019b0064047c029b0064059d05a6010000ab010000000000
+                  00000082017403000000000000000000007c017c026702a6010000ab0100
+                  000000000000007c005f02000000000000000067007c005f030000000000
+                  00000064067c005f04000000000000000064077c005f0500000000000000
+                  007c006a0200000000000000006401190000000000000000007c006a0200
+                  000000000000006408190000000000000000006b02000000007c005f0600
+                  0000000000000064077c005f070000000000000000741100000000000000
+                  0000007c006a020000000000000000a6010000ab0100000000000000007c
+                  005f09000000000000000064065300
                  5           0 RESUME                   0
                
-                18           2 LOAD_GLOBAL              1 (NULL + sorted)
-                            14 LOAD_FAST                1 (a)
-                            16 LOAD_FAST                2 (b)
-                            18 BUILD_LIST               2
-                            20 PRECALL                  1
-                            24 CALL                     1
-                            34 LOAD_FAST                0 (self)
-                            36 STORE_ATTR               1 (sides)
-               
-                19          46 BUILD_LIST               0
-                            48 LOAD_FAST                0 (self)
-                            50 STORE_ATTR               2 (linked)
-               
-                20          60 LOAD_CONST               1 (None)
-                            62 LOAD_FAST                0 (self)
-                            64 STORE_ATTR               3 (linked_to)
-               
-                21          74 LOAD_CONST               2 (False)
-                            76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               4 (is_crossing)
-               
-                22          88 LOAD_FAST                0 (self)
-                            90 LOAD_ATTR                1 (sides)
-                           100 LOAD_CONST               3 (0)
-                           102 BINARY_SUBSCR
-                           112 LOAD_FAST                0 (self)
-                           114 LOAD_ATTR                1 (sides)
-                           124 LOAD_CONST               4 (1)
-                           126 BINARY_SUBSCR
-                           136 COMPARE_OP               2 (==)
-                           142 LOAD_FAST                0 (self)
-                           144 STORE_ATTR               5 (is_double)
-               
-                23         154 LOAD_CONST               2 (False)
-                           156 LOAD_FAST                0 (self)
-                           158 STORE_ATTR               6 (closed)
-               
-                24         168 LOAD_GLOBAL             15 (NULL + sum)
-                           180 LOAD_FAST                0 (self)
-                           182 LOAD_ATTR                1 (sides)
-                           192 PRECALL                  1
-                           196 CALL                     1
-                           206 LOAD_FAST                0 (self)
-                           208 STORE_ATTR               8 (points)
-                           218 LOAD_CONST               1 (None)
-                           220 RETURN_VALUE
+                18           2 LOAD_FAST                1 (a)
+                             4 LOAD_CONST               1 (0)
+                             6 COMPARE_OP               0 (<)
+                            12 POP_JUMP_FORWARD_IF_TRUE    18 (to 50)
+                            14 LOAD_FAST                2 (b)
+                            16 LOAD_CONST               1 (0)
+                            18 COMPARE_OP               0 (<)
+                            24 POP_JUMP_FORWARD_IF_TRUE    12 (to 50)
+                            26 LOAD_FAST                1 (a)
+                            28 LOAD_CONST               2 (6)
+                            30 COMPARE_OP               4 (>)
+                            36 POP_JUMP_FORWARD_IF_TRUE     6 (to 50)
+                            38 LOAD_FAST                2 (b)
+                            40 LOAD_CONST               2 (6)
+                            42 COMPARE_OP               4 (>)
+                            48 POP_JUMP_FORWARD_IF_FALSE    22 (to 94)
+               
+                19     >>   50 LOAD_GLOBAL              1 (NULL + ValueError)
+                            62 LOAD_CONST               3 ('Domino Piece sides can only have values 0-6, got [')
+                            64 LOAD_FAST                1 (a)
+                            66 FORMAT_VALUE             0
+                            68 LOAD_CONST               4 ('|')
+                            70 LOAD_FAST                2 (b)
+                            72 FORMAT_VALUE             0
+                            74 LOAD_CONST               5 (']')
+                            76 BUILD_STRING             5
+                            78 PRECALL                  1
+                            82 CALL                     1
+                            92 RAISE_VARARGS            1
+               
+                21     >>   94 LOAD_GLOBAL              3 (NULL + sorted)
+                           106 LOAD_FAST                1 (a)
+                           108 LOAD_FAST                2 (b)
+                           110 BUILD_LIST               2
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 LOAD_FAST                0 (self)
+                           128 STORE_ATTR               2 (sides)
+               
+                22         138 BUILD_LIST               0
+                           140 LOAD_FAST                0 (self)
+                           142 STORE_ATTR               3 (linked)
+               
+                23         152 LOAD_CONST               6 (None)
+                           154 LOAD_FAST                0 (self)
+                           156 STORE_ATTR               4 (linked_to)
+               
+                24         166 LOAD_CONST               7 (False)
+                           168 LOAD_FAST                0 (self)
+                           170 STORE_ATTR               5 (is_crossing)
+               
+                25         180 LOAD_FAST                0 (self)
+                           182 LOAD_ATTR                2 (sides)
+                           192 LOAD_CONST               1 (0)
+                           194 BINARY_SUBSCR
+                           204 LOAD_FAST                0 (self)
+                           206 LOAD_ATTR                2 (sides)
+                           216 LOAD_CONST               8 (1)
+                           218 BINARY_SUBSCR
+                           228 COMPARE_OP               2 (==)
+                           234 LOAD_FAST                0 (self)
+                           236 STORE_ATTR               6 (is_double)
+               
+                26         246 LOAD_CONST               7 (False)
+                           248 LOAD_FAST                0 (self)
+                           250 STORE_ATTR               7 (closed)
+               
+                27         260 LOAD_GLOBAL             17 (NULL + sum)
+                           272 LOAD_FAST                0 (self)
+                           274 LOAD_ATTR                2 (sides)
+                           284 PRECALL                  1
+                           288 CALL                     1
+                           298 LOAD_FAST                0 (self)
+                           300 STORE_ATTR               9 (points)
+                           310 LOAD_CONST               6 (None)
+                           312 RETURN_VALUE
                consts
                   '\n        Constructor\n\n        a: int                  -> First number on the piece\n        b: int                  -> Second number on the piece\n\n        linked: List[Piece]     -> Pieces played from this Piece\n        is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece\n        is_double: Bool         -> Whether both sides of the piece show the same number\n        closed: Bool            -> If a double piece is closed (face down), nothing can be appended to it\n        points: int             -> Point value of the piece, which is the combined value of both sides\n        '
+                  0
+                  6
+                  'Domino Piece sides can only have values 0-6, got ['
+                  '|'
+                  ']'
                   None
                   False
-                  0
                   1
-               names      ('sorted', 'sides', 'linked', 'linked_to', 'is_crossing', 'is_double', 'closed', 'sum', 'points')
+               names      ('ValueError', 'sorted', 'sides', 'linked', 'linked_to', 'is_crossing', 'is_double', 'closed', 'sum', 'points')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__init__'
                firstlineno 5
-               lnotab 0x020d2c010e010e010e0142010e01
+               lnotab 0x020d30012c022c010e010e010e0142010e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                26           0 RESUME                   0
+                29           0 RESUME                   0
                
-                27           2 LOAD_FAST                0 (self)
+                30           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (linked)
                             14 LOAD_METHOD              1 (append)
                             36 LOAD_FAST                1 (piece)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -189,52 +239,89 @@
                   None
                names      ('linked', 'append')
                varnames   ('self', 'piece')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       'append'
-               firstlineno 26
+               firstlineno 29
                lnotab 0x0201
+            'other'
+            'return'
+            code
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000005c0200007d027d037c027c016a0000
+                  00000000000000760072027c036e017c025300
+                32           0 RESUME                   0
+               
+                33           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (sides)
+                            14 UNPACK_SEQUENCE          2
+                            18 STORE_FAST               2 (a)
+                            20 STORE_FAST               3 (b)
+               
+                34          22 LOAD_FAST                2 (a)
+                            24 LOAD_FAST                1 (other)
+                            26 LOAD_ATTR                0 (sides)
+                            36 CONTAINS_OP              0
+                            38 POP_JUMP_FORWARD_IF_FALSE     2 (to 44)
+                            40 LOAD_FAST                3 (b)
+                            42 JUMP_FORWARD             1 (to 46)
+                       >>   44 LOAD_FAST                2 (a)
+                       >>   46 RETURN_VALUE
+               consts
+                  None
+               names      ('sides',)
+               varnames   ('self', 'other', 'a', 'b')
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'unlinked_side'
+               firstlineno 32
+               lnotab 0x02011401
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000720b64017d0164027c019b0064037c
                   019b0064049d05530067006405a2017d0264027c027c006a010000000000
                   000000640619000000000000000000190000000000000000009b0064037c
                   027c006a0100000000000000006407190000000000000000001900000000
                   00000000009b0064049d055300
-                29           0 RESUME                   0
+                36           0 RESUME                   0
                
-                31           2 LOAD_FAST                0 (self)
+                38           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (closed)
                             14 POP_JUMP_FORWARD_IF_FALSE    11 (to 38)
                
-                32          16 LOAD_CONST               1 ('▩')
+                39          16 LOAD_CONST               1 ('▩')
                             18 STORE_FAST               1 (closed)
                
-                33          20 LOAD_CONST               2 ('[')
+                40          20 LOAD_CONST               2 ('[')
                             22 LOAD_FAST                1 (closed)
                             24 FORMAT_VALUE             0
                             26 LOAD_CONST               3 ('|')
                             28 LOAD_FAST                1 (closed)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               4 (']')
                             34 BUILD_STRING             5
                             36 RETURN_VALUE
                
-                35     >>   38 BUILD_LIST               0
+                42     >>   38 BUILD_LIST               0
                             40 LOAD_CONST               5 (('□', '⚀', '⚁', '⚂', '⚃', '⚄', '⚅'))
                             42 LIST_EXTEND              1
                             44 STORE_FAST               2 (sides)
                
-                45          46 LOAD_CONST               2 ('[')
+                52          46 LOAD_CONST               2 ('[')
                             48 LOAD_FAST                2 (sides)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                1 (sides)
                             62 LOAD_CONST               6 (0)
                             64 BINARY_SUBSCR
                             74 BINARY_SUBSCR
                             84 FORMAT_VALUE             0
@@ -259,65 +346,90 @@
                   0
                   1
                names      ('closed', 'sides')
                varnames   ('self', 'closed', 'sides')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
-               name       '__repr__'
-               firstlineno 29
+               name       '__str__'
+               firstlineno 36
                lnotab 0x02020e0104011202080a
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
+                  0x97007401000000000000000000007c00a6010000ab0100000000000000
+                  005300
+                54           0 RESUME                   0
+               
+                56           2 LOAD_GLOBAL              1 (NULL + str)
+                            14 LOAD_FAST                0 (self)
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 RETURN_VALUE
+               consts
+                  'Use string representation'
+               names      ('str',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__repr__'
+               firstlineno 54
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
                   0x97007c006a00000000000000000064011900000000000000000064027a
                   0500007c006a0000000000000000006403190000000000000000007a0000
                   005300
-                47           0 RESUME                   0
+                58           0 RESUME                   0
                
-                49           2 LOAD_FAST                0 (self)
+                60           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sides)
-                            14 LOAD_CONST               1 (1)
+                            14 LOAD_CONST               1 (0)
                             16 BINARY_SUBSCR
                             26 LOAD_CONST               2 (10)
                             28 BINARY_OP                5 (*)
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                0 (sides)
-                            44 LOAD_CONST               3 (0)
+                            44 LOAD_CONST               3 (1)
                             46 BINARY_SUBSCR
                             56 BINARY_OP                0 (+)
                             60 RETURN_VALUE
                consts
-                  'Integer representation, e.g. 64 for a [4|6] piece'
-                  1
-                  10
+                  'Integer representation, e.g. 46 for a [4|6] piece'
                   0
+                  10
+                  1
                names      ('sides',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__hash__'
-               firstlineno 47
+               firstlineno 58
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   007401000000000000000000007c01a6010000ab0100000000000000006b
                   02000000005300
-                51           0 RESUME                   0
+                62           0 RESUME                   0
                
-                53           2 LOAD_GLOBAL              1 (NULL + hash)
+                64           2 LOAD_GLOBAL              1 (NULL + hash)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_GLOBAL              1 (NULL + hash)
                             42 LOAD_FAST                1 (other)
                             44 PRECALL                  1
                             48 CALL                     1
@@ -327,174 +439,152 @@
                   'Returns whether the pieces are equal based on their hash'
                names      ('hash',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__eq__'
-               firstlineno 51
+               firstlineno 62
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a0000000000000000006b0000
                   0000005300
-                55           0 RESUME                   0
+                66           0 RESUME                   0
                
-                57           2 LOAD_FAST                0 (self)
+                68           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (points)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_ATTR                0 (points)
                             26 COMPARE_OP               0 (<)
                             32 RETURN_VALUE
                consts
                   'Returns whether a piece is bigger based on point value'
                names      ('points',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__lt__'
-               firstlineno 55
+               firstlineno 66
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c016a0000000000000000006b0400
                   0000005300
-                59           0 RESUME                   0
+                70           0 RESUME                   0
                
-                61           2 LOAD_FAST                0 (self)
+                72           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (points)
                             14 LOAD_FAST                1 (other)
                             16 LOAD_ATTR                0 (points)
                             26 COMPARE_OP               4 (>)
                             32 RETURN_VALUE
                consts
                   'Returns whether a piece is smaller based on point value'
                names      ('points',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__gt__'
-               firstlineno 59
+               firstlineno 70
                lnotab 0x0202
             None
-         names      ('__name__', '__module__', '__qualname__', 'int', '__init__', 'append', '__repr__', '__hash__', '__eq__', '__lt__', '__gt__')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__init__', 'append', 'unlinked_side', '__str__', '__repr__', '__hash__', '__eq__', '__lt__', '__gt__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
          name       'Piece'
          firstlineno 4
-         lnotab 0x0a01101506030612060406040604
+         lnotab 0x0a0110180603100406120604060406040604
       'Piece'
       code
          argcount  : 0
-         nlocals   : 4
+         nlocals   : 3
          stacksize : 8
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             007403000000000000000000006401a6010000ab01000000000000000044
             005d3d7d017403000000000000000000006401a6010000ab010000000000
             00000044005d2b7d027c017c026b010000000072237c00a0020000000000
             0000000000000000000000000000007407000000000000000000007c017c
             02a6020000ab020000000000000000a6010000ab01000000000000000001
-            008c2c8c3e74070000000000000000000064016401a6020000ab02000000
-            00000000007d0364027c035f0400000000000000007c00a0020000000000
-            0000000000000000000000000000007c03a6010000ab0100000000000000
-            000100740b000000000000000000007c00a6010000ab0100000000000000
-            005300
-          64           0 RESUME                   0
+            008c2c8c3e7409000000000000000000007c00a6010000ab010000000000
+            0000005300
+          75           0 RESUME                   0
          
-          65           2 LOAD_GLOBAL              1 (NULL + set)
+          76           2 LOAD_GLOBAL              1 (NULL + set)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               0 (pieces)
          
-          66          30 LOAD_GLOBAL              3 (NULL + range)
+          77          30 LOAD_GLOBAL              3 (NULL + range)
                       42 LOAD_CONST               1 (7)
                       44 PRECALL                  1
                       48 CALL                     1
                       58 GET_ITER
                  >>   60 FOR_ITER                61 (to 184)
                       62 STORE_FAST               1 (i)
          
-          67          64 LOAD_GLOBAL              3 (NULL + range)
+          78          64 LOAD_GLOBAL              3 (NULL + range)
                       76 LOAD_CONST               1 (7)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 GET_ITER
                  >>   94 FOR_ITER                43 (to 182)
                       96 STORE_FAST               2 (j)
          
-          68          98 LOAD_FAST                1 (i)
+          79          98 LOAD_FAST                1 (i)
                      100 LOAD_FAST                2 (j)
                      102 COMPARE_OP               1 (<=)
                      108 POP_JUMP_FORWARD_IF_FALSE    35 (to 180)
          
-          69         110 LOAD_FAST                0 (pieces)
+          80         110 LOAD_FAST                0 (pieces)
                      112 LOAD_METHOD              2 (add)
                      134 LOAD_GLOBAL              7 (NULL + Piece)
                      146 LOAD_FAST                1 (i)
                      148 LOAD_FAST                2 (j)
                      150 PRECALL                  2
                      154 CALL                     2
                      164 PRECALL                  1
                      168 CALL                     1
                      178 POP_TOP
                  >>  180 JUMP_BACKWARD           44 (to 94)
          
-          67     >>  182 JUMP_BACKWARD           62 (to 60)
+          78     >>  182 JUMP_BACKWARD           62 (to 60)
          
-          71     >>  184 LOAD_GLOBAL              7 (NULL + Piece)
-                     196 LOAD_CONST               1 (7)
-                     198 LOAD_CONST               1 (7)
-                     200 PRECALL                  2
-                     204 CALL                     2
-                     214 STORE_FAST               3 (piece)
-         
-          72         216 LOAD_CONST               2 (True)
-                     218 LOAD_FAST                3 (piece)
-                     220 STORE_ATTR               4 (closed)
-         
-          73         230 LOAD_FAST                0 (pieces)
-                     232 LOAD_METHOD              2 (add)
-                     254 LOAD_FAST                3 (piece)
-                     256 PRECALL                  1
-                     260 CALL                     1
-                     270 POP_TOP
-         
-          75         272 LOAD_GLOBAL             11 (NULL + sorted)
-                     284 LOAD_FAST                0 (pieces)
-                     286 PRECALL                  1
-                     290 CALL                     1
-                     300 RETURN_VALUE
+          82     >>  184 LOAD_GLOBAL              9 (NULL + sorted)
+                     196 LOAD_FAST                0 (pieces)
+                     198 PRECALL                  1
+                     202 CALL                     1
+                     212 RETURN_VALUE
          consts
             None
             7
-            True
-         names      ('set', 'range', 'add', 'Piece', 'closed', 'sorted')
-         varnames   ('pieces', 'i', 'j', 'piece')
+         names      ('set', 'range', 'add', 'Piece', 'sorted')
+         varnames   ('pieces', 'i', 'j')
          freevars   ()
          cellvars   ()
          filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
          name       'domino_set'
-         firstlineno 64
-         lnotab 0x02011c01220122010c0148fe020420010e012a02
+         firstlineno 75
+         lnotab 0x02011c01220122010c0148fe0204
       None
    names      ('typing', 'List', 'Union', 'Piece', 'domino_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020110031a3c
+   lnotab 0x00ff020110031a47
```

