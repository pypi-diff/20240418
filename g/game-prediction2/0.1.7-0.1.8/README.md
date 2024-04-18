# Comparing `tmp/game_prediction2-0.1.7.tar.gz` & `tmp/game_prediction2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_prediction2-0.1.7.tar", last modified: Tue Apr 16 07:42:24 2024, max compression
+gzip compressed data, was "game_prediction2-0.1.8.tar", last modified: Thu Apr 18 13:07:49 2024, max compression
```

## Comparing `game_prediction2-0.1.7.tar` & `game_prediction2-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-16 07:42:22.000000 game_prediction2-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.394862 game_prediction2-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.394862 game_prediction2-0.1.7/src/game_prediction2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.7/src/game_prediction2/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/beam/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.7/src/game_prediction2/beam/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1933 2024-04-16 07:38:02.000000 game_prediction2-0.1.7/src/game_prediction2/beam/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-16 07:37:30.000000 game_prediction2-0.1.7/src/game_prediction2/beam/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2061 2024-04-16 07:37:29.000000 game_prediction2-0.1.7/src/game_prediction2/beam/searching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.7/src/game_prediction2/beam/succs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.7/src/game_prediction2/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.7/src/game_prediction2/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/aggregate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3409 2024-04-16 07:27:38.000000 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/logprobs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/predict/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.7/src/game_prediction2/util/predict/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1468 2024-04-16 07:27:05.000000 game_prediction2-0.1.7/src/game_prediction2/util/predict/predict.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-18 13:07:46.000000 game_prediction2-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.955339 game_prediction2-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.8/src/game_prediction2/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/beam/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.8/src/game_prediction2/beam/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1933 2024-04-16 07:38:02.000000 game_prediction2-0.1.8/src/game_prediction2/beam/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-16 07:37:30.000000 game_prediction2-0.1.8/src/game_prediction2/beam/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2068 2024-04-16 11:55:55.000000 game_prediction2-0.1.8/src/game_prediction2/beam/searching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.8/src/game_prediction2/beam/succs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.8/src/game_prediction2/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.8/src/game_prediction2/util/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/aggregate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3341 2024-04-16 09:16:03.000000 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/logprobs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/predict/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.8/src/game_prediction2/util/predict/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1468 2024-04-16 07:27:05.000000 game_prediction2-0.1.8/src/game_prediction2/util/predict/predict.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/top_level.txt
```

### Comparing `game_prediction2-0.1.7/pyproject.toml` & `game_prediction2-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "game-prediction2"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game prediction, simplified. No edits, no GCP. Everything's just `AsyncIterables` in and out."
 dependencies = [
     "haskellian",
     "lcz",
```

### Comparing `game_prediction2-0.1.7/src/game_prediction2/beam/decoding.py` & `game_prediction2-0.1.8/src/game_prediction2/beam/decoding.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2/beam/main.py` & `game_prediction2-0.1.8/src/game_prediction2/beam/main.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2/beam/searching.py` & `game_prediction2-0.1.8/src/game_prediction2/beam/searching.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,28 @@
   def __call__(self, ply: int) -> int:
     ...
 
 class SearchParams(SuccParams):
   uci_prior: NotRequired[UCIPrior]
   agg_logp: NotRequired[AggregateLogps]
   beam_width: NotRequired[BeamWidth]
-  fen: NotRequired[str]
+  fen: NotRequired[str|None]
   
 Beam = Iterable[Node]
 
 async def search(logprobs: AsyncIterable[Logprob], **p: Unpack[SearchParams]) -> AsyncIterable[Beam]:
   """Beam search across the forest of moves stemming from `start_fens`
   - `logprobs[ply](san, piece)`: (OCR) log-probability of `san` (which captures `piece`) at `ply`
   - `uci_prior(fens)`: batched prior distribution of legal moves (defaults to using `MaiaChess` with `Leela Chess Zero`)
   - `agg_logp(logp, logq)`: aggregation function of the OCR and prior log-probabilities. Defaults to a weighted geometric average giving the OCR probabilities 10x the importance. I.e. `(p^10 * q)^(1/11)` (but in log-space, ofc)
   """
   uci_prior = p.get('uci_prior', lcz.eval)
   agg_logp = p.get('agg_logp', lambda logp_ocr, logp_prior: logps.weighted_geo_mean(logp_ocr, logp_prior, a=10, b=1))
   beam_width = p.get('beam_width', lambda _: 4)
-  fen = p.get('fen', chess.STARTING_FEN)
+  fen = p.get('fen') or chess.STARTING_FEN
 
   beam: Beam = [Node(fen)]
   priors = uci_prior([fen])
   async for i, lp in AI.enumerate(logprobs):
     inputs = zip(beam, priors)
     nested_succs = hk.starmap(lambda node, prior: successors(node, prior, lp, agg_logp))(inputs)
     succs = list(hk.flatten(nested_succs))
```

### Comparing `game_prediction2-0.1.7/src/game_prediction2/beam/succs.py` & `game_prediction2-0.1.8/src/game_prediction2/beam/succs.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2/main.py` & `game_prediction2-0.1.8/src/game_prediction2/main.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2/util/aggregate/aggregate.py` & `game_prediction2-0.1.8/src/game_prediction2/util/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2/util/logprobs/logprobs.py` & `game_prediction2-0.1.8/src/game_prediction2/util/logprobs/logprobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from editdistance import distance as edit_dist
+from itertools import zip_longest
 import numpy as np
 from pydantic import BaseModel
 from chess_notation.represent import representations, MotionStyles
 from chess_notation.styles import PawnCapture, PieceCapture
 from chess_notation.language import Language
 from chess_utils import CapturablePiece
 from ...beam import Logprob
@@ -46,18 +47,18 @@
   """Max `pseudo_logp` across all possible representations of `san`"""
   reprs = representations(san, motions=ann.motions(), captured_piece=captured_piece, languages=ann.langs() or ['CA', 'EN'])
   return max(pseudo_logp(r, top_preds) for r in reprs)
 
 def players_max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> float:
   """Max `max_pseudo_logp` across players"""
   annotations = annotations or [Annotations() for _ in players_preds]
-  assert len(players_preds) == len(annotations), f'ERROR: Inconsistent number of players: {len(players_preds)} preds, but {len(annotations)} annotations'
   return max(
-    max_pseudo_logp(san, captured_piece, preds, ann)
-    for preds, ann in zip(players_preds, annotations)
+    max_pseudo_logp(san, captured_piece, preds, ann or Annotations())
+    for preds, ann in zip_longest(players_preds, annotations)
+      if preds is not None
   )
 
 
 def logprob(players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> Logprob:
   """Curried version of `players_max_pseudo_logp`"""
   def _logprob(san: str, captured_piece: CapturablePiece | None):
     return players_max_pseudo_logp(san, captured_piece, players_preds, annotations)
```

### Comparing `game_prediction2-0.1.7/src/game_prediction2/util/predict/predict.py` & `game_prediction2-0.1.8/src/game_prediction2/util/predict/predict.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.7/src/game_prediction2.egg-info/SOURCES.txt` & `game_prediction2-0.1.8/src/game_prediction2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

