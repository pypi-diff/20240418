# Comparing `tmp/quagnes-1.0.0.tar.gz` & `tmp/quagnes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quagnes-1.0.0.tar", last modified: Thu Apr 11 05:16:29 2024, max compression
+gzip compressed data, was "quagnes-1.1.0.tar", last modified: Thu Apr 18 02:47:51 2024, max compression
```

## Comparing `quagnes-1.0.0.tar` & `quagnes-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/
--r--------   0 yar       (1000) yar       (1000)    35149 2024-03-02 00:03:19.000000 quagnes-1.0.0/LICENSE.txt
--rw-r--r--   0 yar       (1000) yar       (1000)    52358 2024-04-11 05:16:29.317278 quagnes-1.0.0/PKG-INFO
--rwx------   0 yar       (1000) yar       (1000)    11050 2024-04-11 05:11:49.000000 quagnes-1.0.0/README.md
--r--------   0 yar       (1000) yar       (1000)      936 2024-04-04 01:20:53.000000 quagnes-1.0.0/pyproject.toml
--rw-r--r--   0 yar       (1000) yar       (1000)       38 2024-04-11 05:16:29.317278 quagnes-1.0.0/setup.cfg
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.313278 quagnes-1.0.0/src/
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/src/quagnes/
--r-x------   0 yar       (1000) yar       (1000)     3655 2024-04-04 01:20:36.000000 quagnes-1.0.0/src/quagnes/__init__.py
--rwx------   0 yar       (1000) yar       (1000)    77947 2024-04-10 14:43:47.000000 quagnes-1.0.0/src/quagnes/agnes.py
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/src/quagnes.egg-info/
--rw-r--r--   0 yar       (1000) yar       (1000)    52358 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/PKG-INFO
--rw-------   0 yar       (1000) yar       (1000)      221 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/SOURCES.txt
--rw-------   0 yar       (1000) yar       (1000)        1 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/dependency_links.txt
--rw-------   0 yar       (1000) yar       (1000)        8 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/top_level.txt
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-18 02:47:51.599353 quagnes-1.1.0/
+-r--------   0 yar       (1000) yar       (1000)    35149 2024-03-02 00:03:19.000000 quagnes-1.1.0/LICENSE.txt
+-rw-r--r--   0 yar       (1000) yar       (1000)    50715 2024-04-18 02:47:51.599353 quagnes-1.1.0/PKG-INFO
+-rwx------   0 yar       (1000) yar       (1000)     9407 2024-04-17 23:52:36.000000 quagnes-1.1.0/README.md
+-r--------   0 yar       (1000) yar       (1000)      936 2024-04-18 02:45:57.000000 quagnes-1.1.0/pyproject.toml
+-rw-r--r--   0 yar       (1000) yar       (1000)       38 2024-04-18 02:47:51.599353 quagnes-1.1.0/setup.cfg
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-18 02:47:51.595353 quagnes-1.1.0/src/
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-18 02:47:51.599353 quagnes-1.1.0/src/quagnes/
+-r-x------   0 yar       (1000) yar       (1000)     3655 2024-04-13 19:27:46.000000 quagnes-1.1.0/src/quagnes/__init__.py
+-rwx------   0 yar       (1000) yar       (1000)    90728 2024-04-18 00:00:06.000000 quagnes-1.1.0/src/quagnes/agnes.py
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-18 02:47:51.599353 quagnes-1.1.0/src/quagnes.egg-info/
+-rw-r--r--   0 yar       (1000) yar       (1000)    50715 2024-04-18 02:47:51.000000 quagnes-1.1.0/src/quagnes.egg-info/PKG-INFO
+-rw-------   0 yar       (1000) yar       (1000)      221 2024-04-18 02:47:51.000000 quagnes-1.1.0/src/quagnes.egg-info/SOURCES.txt
+-rw-------   0 yar       (1000) yar       (1000)        1 2024-04-18 02:47:51.000000 quagnes-1.1.0/src/quagnes.egg-info/dependency_links.txt
+-rw-------   0 yar       (1000) yar       (1000)        8 2024-04-18 02:47:51.000000 quagnes-1.1.0/src/quagnes.egg-info/top_level.txt
```

### Comparing `quagnes-1.0.0/LICENSE.txt` & `quagnes-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quagnes-1.0.0/PKG-INFO` & `quagnes-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quagnes
-Version: 1.0.0
+Version: 1.1.0
 Summary: This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates.
 Author-email: Ray Griner <rgriner_fwd@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -725,68 +725,47 @@
     #if rc==1:
     #    f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
     #    fwrite(new_game.print_history())
     #    f.close()
 ```
 
 # Release Notes
-## Version 1.0.0
-- Change name of `split_same_suit_runs` parameter to `split_runs` and make
-  parameter applicable regardless of the value of `move_same_suit`.
-- Add optimization for use when the losing state set is disabled.
-Track for each pile the last move depth, the number of cards
-moved, whether the pile was moved from or to, and whether the bottom card
-in the moved pile could be played to the foundation at the time of the move.
-Do not allow moves that: (a) reverse a previous tableau move without an
-intervening move to foundation or deal; (b) make the last deal after a
-tableau move where neither pile is dealt to and neither file had a card
-played to foundation; (c) play the bottom card of the moved pile to the
-foundation after the tableau move if it could have been played at the time
-of the move (and there has been no subsequent move to the pile or deal
-onto the pile).  These optimizations are only employed when the losing
-states set is
-disabled, as they use information not stored in the losing states set to
-determine whether a move can be played.
-- Add optimization when moves to empty piles allow zero or multiple cards
-to reduce the space of moves to consider when the stock is empty or near
-empty (without
-changing the win possibility or maximum score that can be attained). In
-these rules, we use the term 'top card' to describe the highest-rank card
-in the pile being moved and 'same-color top card' to be the card with equal
-rank in the same-color suit. The rules are: (a) when moving runs by suit,
-never split a run between same-suit cards when the stock is empty;
-(b) never split a run between same-suit cards when neither pile can be
-covered by a future deal and the same-color top card is in the foundation;
-(c) when the stock is empty, force a move onto a card of the same suit
-where possible when we know the target pile cannot be needed to move the
-same-color top card (ie, the same-color top card is already in the
-foundation or in same-suit sequence or the card one rank higher than the
-same-color top card is already exposed at the bottom of a pile); (d) when
-the stock is empty, force a move to the foundation if the card being
-moved cannot be needed as a target to be moved onto (ie, if the card in the
-same-color suit that is one rank lower is already in the foundation or in
-same-suit sequence).
-- Add new attributes created for these two optimizations in `_AgnesState` class (`in_suit_seq`, `last_in_pile`,
-  `_all_lmi`) and to output printed when state is printed.
-- Add `_AgnesState.hash_str` attribute to store the string representing
-  the hash of the object that will be stored in the losing states and
-  check loop set. Add `_Agnes_state.update_hash_str()` function called
-  after move is performed or undone to save the string in `hash_str`.
-  Previously, the `hash_str` was recalculated multiple times.
-- Fix bug in `Agnes.print_history` as only half the history was being
-  printed.
-- Use a single set to track whether loop has occured rather than a stack of
-  sets. Save result of check whether state is in the losing states set
-  so that we do not inefficiently (re-)insert the state into the losing
-  states set. Add attributes `is_loop` and `is_loser` to `_AgnesState`
-  class to support this logic.
-- Created for C++ implementation. Move detailed information
-  on the background, game rules, program methodology, and analysis of
-  win rates to that repository from this README. Add win rates
-  for rule variants where the empty rule is *AnyRun* or *HighRun*.
+## Version 1.1.0
+### Fixes Affecting Simultation Results
+- No longer forbid splitting of runs between same-suit cards when the stock
+has two cards left, even when neither the source nor target pile can be
+covered by a future deal. This optimization is incorrect, ie, it could
+force some winning games to be reported as losses.
+- Previously, splitting runs between cards of the same suit was not allowed
+when the stock was empty when runs are moved by suit. Add the condition that
+`Card(rank=last_card.rank - 1, suit=last_card.same_color_suit)` must also be
+in the foundation or meet the criteria for being forced to the foundation
+when it appears (for such splits to be forbidden), where `last_card` is the
+last card in the run moved. The additional condition is because placing the
+same-color suit at the bottom of the pile makes the pile unmovable, and so
+it would matter whether or not the split was performed. So we only forbid
+splits when this cannot be the case.
+
+### Fixes Improving Run-Time
+- When checking whether a card is the last in the pile (which is used to
+determine whether a tableau move should be forced), we previously failed to
+consider the card that would become last in a pile after the move. These
+cards are now considered.
+- Add optimization to force the last deal if the two dealt cards will
+immediately be forced to the foundation if `Card(rank - 2, same_color_suit)`
+is already in the foundation. Attributes were added to the `_AgnesState`
+class to store the last and second to last card, whether they are of the
+same suit in-sequence, and whether they are the same color, but not the
+same suit.
+- Add optimization to sort the tableau piles that can no longer be covered
+by a deal before storing in or checking against the losing states set. The
+piles are sorted by their top card.
+
+### Other Changes
+- Add `in_foundation` function to `_AgnesState` class.
 
 # External Documentation
 A C++ implementation written by this package author also exists in a git
 repository.  Detailed information on the background, game rules, program
 methodology, and analysis of win rates are available [there](https://github.com/ghrgriner/quagnes-cpp/wiki/Rules,-Methodology,-and-Analysis-of-Win-Rates).
 
 # Using the Package
@@ -874,9 +853,9 @@
 [2] Dalton W (1909). "My favourite Patiences" in The Strand Magazine,
     Vol 38.
 
 [3] Parlett D (1979). The Penguin Book of Patience. London: Penguin.
 
 # Disclosures
 We are not affiliated with any of the books, websites, or applications
-discussed in this documentation, except of course for this Python package
-and previously-mentioned C++ implementation which we wrote.
+discussed in this documentation, except for this Python package and
+previously-mentioned C++ implementation which we wrote.
```

### Comparing `quagnes-1.0.0/README.md` & `quagnes-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,68 +36,47 @@
     #if rc==1:
     #    f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
     #    fwrite(new_game.print_history())
     #    f.close()
 ```
 
 # Release Notes
-## Version 1.0.0
-- Change name of `split_same_suit_runs` parameter to `split_runs` and make
-  parameter applicable regardless of the value of `move_same_suit`.
-- Add optimization for use when the losing state set is disabled.
-Track for each pile the last move depth, the number of cards
-moved, whether the pile was moved from or to, and whether the bottom card
-in the moved pile could be played to the foundation at the time of the move.
-Do not allow moves that: (a) reverse a previous tableau move without an
-intervening move to foundation or deal; (b) make the last deal after a
-tableau move where neither pile is dealt to and neither file had a card
-played to foundation; (c) play the bottom card of the moved pile to the
-foundation after the tableau move if it could have been played at the time
-of the move (and there has been no subsequent move to the pile or deal
-onto the pile).  These optimizations are only employed when the losing
-states set is
-disabled, as they use information not stored in the losing states set to
-determine whether a move can be played.
-- Add optimization when moves to empty piles allow zero or multiple cards
-to reduce the space of moves to consider when the stock is empty or near
-empty (without
-changing the win possibility or maximum score that can be attained). In
-these rules, we use the term 'top card' to describe the highest-rank card
-in the pile being moved and 'same-color top card' to be the card with equal
-rank in the same-color suit. The rules are: (a) when moving runs by suit,
-never split a run between same-suit cards when the stock is empty;
-(b) never split a run between same-suit cards when neither pile can be
-covered by a future deal and the same-color top card is in the foundation;
-(c) when the stock is empty, force a move onto a card of the same suit
-where possible when we know the target pile cannot be needed to move the
-same-color top card (ie, the same-color top card is already in the
-foundation or in same-suit sequence or the card one rank higher than the
-same-color top card is already exposed at the bottom of a pile); (d) when
-the stock is empty, force a move to the foundation if the card being
-moved cannot be needed as a target to be moved onto (ie, if the card in the
-same-color suit that is one rank lower is already in the foundation or in
-same-suit sequence).
-- Add new attributes created for these two optimizations in `_AgnesState` class (`in_suit_seq`, `last_in_pile`,
-  `_all_lmi`) and to output printed when state is printed.
-- Add `_AgnesState.hash_str` attribute to store the string representing
-  the hash of the object that will be stored in the losing states and
-  check loop set. Add `_Agnes_state.update_hash_str()` function called
-  after move is performed or undone to save the string in `hash_str`.
-  Previously, the `hash_str` was recalculated multiple times.
-- Fix bug in `Agnes.print_history` as only half the history was being
-  printed.
-- Use a single set to track whether loop has occured rather than a stack of
-  sets. Save result of check whether state is in the losing states set
-  so that we do not inefficiently (re-)insert the state into the losing
-  states set. Add attributes `is_loop` and `is_loser` to `_AgnesState`
-  class to support this logic.
-- Created for C++ implementation. Move detailed information
-  on the background, game rules, program methodology, and analysis of
-  win rates to that repository from this README. Add win rates
-  for rule variants where the empty rule is *AnyRun* or *HighRun*.
+## Version 1.1.0
+### Fixes Affecting Simultation Results
+- No longer forbid splitting of runs between same-suit cards when the stock
+has two cards left, even when neither the source nor target pile can be
+covered by a future deal. This optimization is incorrect, ie, it could
+force some winning games to be reported as losses.
+- Previously, splitting runs between cards of the same suit was not allowed
+when the stock was empty when runs are moved by suit. Add the condition that
+`Card(rank=last_card.rank - 1, suit=last_card.same_color_suit)` must also be
+in the foundation or meet the criteria for being forced to the foundation
+when it appears (for such splits to be forbidden), where `last_card` is the
+last card in the run moved. The additional condition is because placing the
+same-color suit at the bottom of the pile makes the pile unmovable, and so
+it would matter whether or not the split was performed. So we only forbid
+splits when this cannot be the case.
+
+### Fixes Improving Run-Time
+- When checking whether a card is the last in the pile (which is used to
+determine whether a tableau move should be forced), we previously failed to
+consider the card that would become last in a pile after the move. These
+cards are now considered.
+- Add optimization to force the last deal if the two dealt cards will
+immediately be forced to the foundation if `Card(rank - 2, same_color_suit)`
+is already in the foundation. Attributes were added to the `_AgnesState`
+class to store the last and second to last card, whether they are of the
+same suit in-sequence, and whether they are the same color, but not the
+same suit.
+- Add optimization to sort the tableau piles that can no longer be covered
+by a deal before storing in or checking against the losing states set. The
+piles are sorted by their top card.
+
+### Other Changes
+- Add `in_foundation` function to `_AgnesState` class.
 
 # External Documentation
 A C++ implementation written by this package author also exists in a git
 repository.  Detailed information on the background, game rules, program
 methodology, and analysis of win rates are available [there](https://github.com/ghrgriner/quagnes-cpp/wiki/Rules,-Methodology,-and-Analysis-of-Win-Rates).
 
 # Using the Package
@@ -185,9 +164,9 @@
 [2] Dalton W (1909). "My favourite Patiences" in The Strand Magazine,
     Vol 38.
 
 [3] Parlett D (1979). The Penguin Book of Patience. London: Penguin.
 
 # Disclosures
 We are not affiliated with any of the books, websites, or applications
-discussed in this documentation, except of course for this Python package
-and previously-mentioned C++ implementation which we wrote.
+discussed in this documentation, except for this Python package and
+previously-mentioned C++ implementation which we wrote.
```

### Comparing `quagnes-1.0.0/pyproject.toml` & `quagnes-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quagnes"
-version = "1.0.0"
+version = "1.1.0"
 authors = [{name = "Ray Griner", email = "rgriner_fwd@outlook.com"}]
 description = "This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `quagnes-1.0.0/src/quagnes/__init__.py` & `quagnes-1.1.0/src/quagnes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,11 +90,11 @@
 #------------------------------------------------------------------------------
 # File:    __init__.py
 # Date:    2024-03-14
 # Author:  Ray Griner
 # Changes:
 #------------------------------------------------------------------------------
 __author__ = 'Ray Griner'
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __all__ = ['Agnes']
 
 from .agnes import Agnes
```

### Comparing `quagnes-1.0.0/src/quagnes/agnes.py` & `quagnes-1.1.0/src/quagnes/agnes.py`

 * *Files 11% similar despite different names*

```diff
@@ -105,14 +105,45 @@
 #   to only consider the case when such moves are done after the last deal.)
 # (3f) Additional restriction on splitting same suit besides those implied by
 #   `split_runs` (which were implemented in set_n_movable). Only allow splits
 #   of same suit if source or target will be covered by future deal, or
 #   `split_empty_stock=True` or Card(src_card.rank, same_color_suit(src_card))
 #   is not in the foundation, where src_card is the highest-rank card in the
 #   part of the pile that is being moved.
+# 20240413:
+# Fixes to Optimization (8). These were causing wins to be reported as losses
+# for a small number of games.
+# (1) No longer forbid splitting of runs between same-suit cards when the stock
+#   has two cards left, even when neither the source nor target pile can be
+#   covered by a future deal. This optimization was incorrect, it causes a
+#   small umber of wins to be reported as losses.
+# (2) Previously splitting of same-suit runs was not allowed when the stock was
+#   empty when runs are moved by suit. Add the condition that
+#   Card(rank=last_card.rank - 1, suit=same_color_suit) must also be in the
+#   foundation (for such splits to be forbidden) or forcable to the foundation
+#   where last_card is the last card in the run moved. The additional condition
+#   is because placing the same color suit at the bottom of the pile makes the
+#   pile unmovable, and so it would matter whether or not the split was
+#   performed. So we only forbid splits when this cannot be the case.
+#
+# New Optimizations to improve run time:
+# (3) When checking whether a card is the last in the pile (which is used to
+#   determine whether a tableau move should be forced), we previously failed to
+#   consider the cards that will newly last in a pile after a move. These cards
+#   are now considered.
+# (4) Add Optimization (9) to force the last deal if the two dealt cards will
+#   immediately be forced to the foundation according to the first part of
+#   Optimization (8d) (but not considering whether the 1-lower same-color card
+#   is in suit-sequence. Attributes were added to the `AgnesState` class to
+#   store the last and second to last card, whether they are of the same suit
+#   in sequence, and whether they are the same color, but not the same suit.
+# (5) Add Optimization (10) to sort the tableau piles that can no longer be
+#   covered by a deal before storing in or checking against the losing states
+#   set. The piles are sorted by their top card. New attributes `sort_order`
+#   and `pile_sort_info` in AgnesState.
 #------------------------------------------------------------------------------
 """A module for solving Agnes solitaire. """
 
 import random
 import copy
 from typing import Set, Optional, Union, NamedTuple
 from dataclasses import dataclass
@@ -133,15 +164,14 @@
 #Card = tuple[CardRank, CardSuit]
 #Card = collections.namedtuple('Card', 'rank suit')
 #
 #class Card(NamedTuple):
 #    rank: CardRank
 #    suit: CardSuit
 
-# TODO:
 @dataclass(frozen=True, slots=True)
 class LastMoveInfo:
     """Information about the last tableau move performed on a pile.
 
     Attributes
     ----------
     depth : int
@@ -246,14 +276,20 @@
         List of hidden cards in the pile. Highest index indicates cards
         at the bottom of the column in the tableau.
     """
     n_movable: list[int]
     hidden: list[Card]
     exposed: list[Card]
 
+@dataclass
+class PileSortInfo():
+    n_stock_left: int
+    pile_index: int
+    pile: AgnesPile
+
 @dataclass(frozen=True)
 class DealMove:
     """Dataclass representing a deal from the stock."""
     def __str__(self) -> str:
         return 'Deal'
 
 class TablType(Enum):
@@ -643,15 +679,15 @@
         Returns
         -------
         A string as described above.
 
         Notes
         -----
         Because the `Agnes` object has to construct the states by undoing
-        moves, a deepcopy of the object is made before starting. This also 
+        moves, a deepcopy of the object is made before starting. This also
         (unnecessarily) copies the perhaps quite large `_losing_states`
         attribute. Therefore, it is probably best to use this only for
         debugging rather than printing the history for all winners.
         """
         states: list[_AgnesState] = []
         # inefficient, since losing_states set may be quite large, but we
         # expect to only do once for each winning game
@@ -794,14 +830,15 @@
 
         # Reset the indexing of all cards so base card has rank 0
         self._deck = []
         for i in range(0, 13*4):
             self._deck.append(Card(rank=(self._initial_deck[i].rank
                                 - self._initial_deck[0].rank) % 13,
                                    suit=self._initial_deck[i].suit))
+        first_state.set_last_cards(self._deck)
         # Deal base card to foundation
         first_state.play_base_card(self._deck[0])
 
         snm_opts: SetNMovableOpts = SetNMovableOpts(
             move_same_suit=self.move_same_suit, split_runs=self.split_runs,
             split_empty_stock=self.split_empty_stock)
 
@@ -892,19 +929,22 @@
             # if we exposed a card when we moved the card beneath it to the
             # foundation, turn it back over before moving the card back from
             # the foundation
             if curr_move.expose:
                 new_state.piles[curr_move.from_].hidden.append(
                     new_state.piles[curr_move.from_].exposed.pop())
             # now move the card back from the foundation
+
             new_state.piles[curr_move.from_].exposed.append(
                 Card(rank=new_state.foundation[curr_move.suit],
                      suit=curr_move.suit))
             new_state.foundation[curr_move.suit] -= 1
             new_state.set_n_movable(curr_move.from_, snm_opts)
+            if len(new_state.piles[curr_move.from_].exposed) == 1:
+                new_state.set_sort_order(self._enum_to_empty_pile)
         elif isinstance(curr_move, DealMove):
             # Deal from stock
             if new_state.n_stock_left == 0:
                 # Put two cards back on deck and remove them from the tableau
                 new_state.undo_deal_for_pile(0)
                 new_state.undo_deal_for_pile(1)
                 # set_n_movable depends on whether n_stock_left>0, so need
@@ -912,14 +952,18 @@
                 for pile_index in range(0,7):
                     new_state.set_n_movable(pile_index, snm_opts)
             else:
                 for pile_index, _ in enumerate(new_state.piles):
                     new_state.undo_deal_for_pile(pile_index)
                 for i in range(0, 7):
                     new_state.set_n_movable(i, snm_opts)
+            for i in range(0, 7):
+                new_state.pile_sort_info[i].n_stock_left = (
+                    new_state.n_stock_left)
+            new_state.set_sort_order(self._enum_to_empty_pile)
         elif isinstance(curr_move, TablMove):
             # since we are undoing the move here, the curr_move.to_ pile
             #  is now the one we are moving the run from
             from_pile = new_state.piles[curr_move.to_].exposed
             to_pile = new_state.piles[curr_move.from_].exposed
             top_card = from_pile[-curr_move.n_cards]
             if curr_move.tabltype == TablType.JOIN:
@@ -932,24 +976,28 @@
                 new_state.last_in_pile[prev_card.rank][prev_card.suit] = True
             if to_pile:
                 new_state.last_in_pile[to_pile[-1].rank][
                     to_pile[-1].suit] = False
 
             # if we exposed a card when we moved the pile, turn it back over
             # before moving the pile back
+            pre_from_size = len(new_state.piles[curr_move.from_].exposed)
             if curr_move.expose:
                 new_state.piles[curr_move.from_].hidden.append(
                     new_state.piles[curr_move.from_].exposed.pop())
             # now move the pile back
             for n_to_pop in range(-1*curr_move.n_cards,0):
                 new_state.piles[curr_move.from_].exposed.append(
                     new_state.piles[curr_move.to_].exposed.pop(n_to_pop)
                     )
             new_state.set_n_movable(curr_move.from_, snm_opts)
             new_state.set_n_movable(curr_move.to_, snm_opts)
+            if (not new_state.piles[curr_move.to_].exposed
+                    or pre_from_size == 0):
+                new_state.set_sort_order(self._enum_to_empty_pile)
 
         new_state.update_hash_str()
 
         if self._moves:
             new_state.curr_move = self._moves[-1]
         else:
             new_state.curr_move = None
@@ -1046,14 +1094,16 @@
                 if score == 52: won_game = True
                 new_state.set_n_movable(curr_move.from_, snm_opts)
                 last_move_info[curr_move.from_] = LastMoveInfo(depth = 0,
                     n_moved = 0, moved_to = False, can_move_to_found = True)
                 if curr_move.tabltype == TablType.NONE:
                     new_state.in_suit_seq[last_card.rank][last_card.suit] = (
                         True)
+                if not new_state.piles[curr_move.from_].exposed:
+                    new_state.set_sort_order(self._enum_to_empty_pile)
             elif isinstance(curr_move, DealMove):
                 # Deal from stock
                 if new_state.n_stock_left == 2:
                     new_state.deal_onto_pile(0, self._deck, True)
                     new_state.deal_onto_pile(1, self._deck, True)
                     # set_n_movable depends on whether n_stock_left>0, so need
                     # to call it for all piles, not just the first two
@@ -1076,14 +1126,20 @@
                 # up run-time by seeing if any lower cards are blocked by
                 # the highest card won't work, because the highest card
                 # could be moved to an empty pile
                 if (self._enum_to_empty_pile == EmptyRule.NONE
                         and not self.maximize_score):
                     any_pile_blocked = new_state.any_pile_blocked()
                 self.n_deal += 1
+                # When undoing move, always update sort order, because it does
+                # not seem worth it to check if any pile is being emptied
+                for i in range(0, 7):
+                    new_state.pile_sort_info[i].n_stock_left = (
+                        new_state.n_stock_left)
+                new_state.set_sort_order(self._enum_to_empty_pile)
             elif isinstance(curr_move, TablMove):
                 self.n_move_card_in_tableau += 1
                 from_pile = new_state.piles[curr_move.from_].exposed
                 to_pile = new_state.piles[curr_move.to_].exposed
                 if len(from_pile) != curr_move.n_cards:
                     last_card = from_pile[-1 *(curr_move.n_cards+1)]
                     new_state.last_in_pile[last_card.rank][last_card.suit] = (
@@ -1105,23 +1161,27 @@
                 last_move_info[curr_move.to_] = LastMoveInfo(
                     depth = new_state.depth, n_moved = curr_move.n_cards,
                     moved_to = True,
                     can_move_to_found = (
                        not (new_state.foundation[last_card.suit]
                             == (last_card.rank - 1))))
 
+                size_tgt_pre = len(new_state.piles[curr_move.to_].exposed)
                 for n_to_pop in range(-1*curr_move.n_cards,0):
                     new_state.piles[curr_move.to_].exposed.append(
                         new_state.piles[curr_move.from_].exposed.pop(n_to_pop)
                         )
                 if curr_move.expose:
                     new_state.piles[curr_move.from_].exposed.append(
                         new_state.piles[curr_move.from_].hidden.pop())
                 new_state.set_n_movable(curr_move.from_, snm_opts)
                 new_state.set_n_movable(curr_move.to_, snm_opts)
+                if (not new_state.piles[curr_move.from_].exposed
+                        or size_tgt_pre == 0):
+                    new_state.set_sort_order(self._enum_to_empty_pile)
             else:
                 raise TypeError(f'curr_move is {curr_move}')
 
             new_state.update_hash_str()
             new_state.is_loop = False
             new_state.is_loser = False
             if self._check_for_loops:
@@ -1210,16 +1270,16 @@
         List of size four representing the top card in each of the four
         foundations. A value of -1 indicates no card in the foundation.
     curr_move : list[int]
         Last move played to reach this state
     valid_moves : list[AgnesMove]
         List of valid moves for this state. It is initialized when the state
         is created and then moves are popped off as they are tried.
-    force_move : list[AgnesMove]
-        List of move that will be forced. This will override the list of
+    force_move : Optional[AgnesMove]
+        Move that will be forced. This will override the list of
         valid moves. For example, moving a card from the tableau to an
         empty foundation pile may be forced. See `set_valid_states`
         for details.
     in_suit_seq : list[list[bool]]
         True for a given card if the card is in an exposed pile in sequence
         under a card of the same suit or is in the foundation. Access
         as: in_suit_seq[card.rank][card.suit].
@@ -1227,14 +1287,23 @@
         True for a given card if the card is the last card in an exposed
         pile (ie, first available for play) or is in the foundation.
         Access as: last_in_pile[card.rank][card.suit].
     hash_str : str
         Somewhat compressed representation of the cards left in the stock and
         and tableau cards. This will be stored in the sets that check for
         loops and previously losing states.
+    lower_last : Card
+        The lower-ranked of the two last cards in the deck.
+    upper_last : Card
+        The higher-ranked of the two last cards in the deck.
+    last_same_suit_seq : bool
+        True if lower_last and upper_last are the same suit and in order.
+    last_same_color_not_suit : bool
+        True if lower_last and upper_last are the same color and not the
+        same suit.
     """
     # default constructor
     def __init__(self) -> None:
         self.depth = 0
         self.n_stock_left = 52
         # Exposed and hidden cards in tableau.
         self.piles: tuple[AgnesPile, ...] = (AgnesPile([], [], []),
@@ -1249,15 +1318,25 @@
         self.is_loser = False
         self.in_suit_seq: list[list[bool]] = []
         self.last_in_pile: list[list[bool]] = []
         self.hash_str: str = ''
         for _ in range(0, 13):
             self.in_suit_seq.append([False, False, False, False])
             self.last_in_pile.append([False, False, False, False])
-
+        self.pile_sort_info: list[PileSortInfo] = []
+        self.sort_order: list[int] = [0, 1, 2, 3, 4, 5, 6]
+        self.lower_last: Card = Card(0, 0)
+        self.upper_last: Card = Card(0, 0)
+        self.last_same_suit_seq: bool = False
+        self.last_same_color_not_suit: bool = False
+
+        for pile_index in range(0, 7):
+            self.pile_sort_info.append(PileSortInfo(pile_index = pile_index,
+                pile = self.piles[pile_index], n_stock_left = 52))
+            self.sort_order[pile_index] = pile_index
 
     # String representation of object (print() will use this)
     #def vertstr(self) -> str:
     #    str1 = (f'\nMove: {_describe_move(self.curr_move)}\n\n'
     #        f'depth:{self.depth}, n_stock_left:{self.n_stock_left}, '
     #        f'valid_moves:{self.valid_moves}\n')
     #
@@ -1268,14 +1347,17 @@
     #        else
     #            foundlist.append(Card(rank=value, suit=suit).twochar())
     #    str2 = 'Foundations:' + ' '.join(foundlist)
 
     def __repr__(self) -> str:
         return (f'\nMove: {_describe_move(self.curr_move)}\n\n'
             f'piles:{self.struncomp()}\n'
+        ##    f'hash_str:{self.hash_str}\n'
+        ##    f'sort_order:{self.sort_order}\n'
+        ##    f'n_movable:{[item.n_movable for item in self.piles]}\n'
             f'depth:{self.depth}, n_stock_left:{self.n_stock_left}, '
             f'valid_moves:{self.valid_moves}\nFoundations:{self.foundation}\n'
             f'T0:{self.piles[0].hidden} | {self.piles[0].exposed}\n'
             f'T1:{self.piles[1].hidden} | {self.piles[1].exposed}\n'
             f'T2:{self.piles[2].hidden} | {self.piles[2].exposed}\n'
             f'T3:{self.piles[3].hidden} | {self.piles[3].exposed}\n'
             f'T4:{self.piles[4].hidden} | {self.piles[4].exposed}\n'
@@ -1317,15 +1399,16 @@
             outlist.append(''.join(suitlist))
         return ' '.join(outlist)
 
     def update_hash_str(self) -> None:
         """Compressed string representation of the state.
         """
         retlist = [str(chr(self.n_stock_left))]
-        for pile in self.piles:
+        for pile_index in range(0, 7):
+            pile = self.piles[self.sort_order[pile_index]]  # 20240413: add
             retlist.append(_strpilecomp(pile.exposed))
             retlist.append(_strpilecomp(pile.hidden))
         self.hash_str = '-'.join(retlist)
 
     def struncomp(self) -> str:
         """Uncompressed string representation of the state.
         """
@@ -1352,18 +1435,35 @@
         """Set self.piles[pile_index].n_movable.
 
         Note this just checks the number of cards from the bottom of the
         pile than can be moved according to the rules. It does not check
         whether there is somewhere the selected set of cards can be moved
         to. The latter is done in `set_valid_moves`.
 
-        The value of self.n_stock_left is used in addition to the
-        parameters passed in to determine if the stock is empty. Therefore,
-        this function must be called for all piles when the stock is
-        made empty (or such a move undone).
+        It sets the number cards from the bottom of the pile that can be
+        moved according to the `move_same_suit` and `split_runs` parameter.
+
+        While doing so, it also applies additional optimizations
+        when the stock is empty and `split_empty_stock` is false about
+        whether to allow splitting a run between two cards of the same
+        suit (even when `split_runs` is True). Namely:
+          (1) If runs are moved by color, such splits are never allowed.
+          (2) If runs are moved by suit, such splits are not allowed
+          if it is certain the last card in the pile being moved is not
+          needed as a move target for the suit of the same color (ie,
+          if Card(last_card.rank - 1, last_card.same_color_suit) is
+          in the foundation or can be forced to the foundation, the split is
+          not allowed. [However, this second condition is implemented in
+          set_valid_moves rather than here, because this function is only
+          called when piles are touched and it's possible an operation on a
+          different pile activated or deactivated condition (2).
+
+        Because the function checks whether `self.n_stock_left == 0`, it
+        must be called for all piles when the stock is made empty (or such
+        a move undone). The call must follow updating of all piles.
 
         Arguments
         ---------
         pile_index : int
             Index of the pile to check
         snm_opts : SetNMovableOpts
             Tuple holding `Agnes` parameter values `move_same_suit`,
@@ -1402,22 +1502,36 @@
                         and above_card.suit == card.suit)
                     is_split_same_color = (above_card.rank == card.rank + 1
                         and (above_card.suit - card.suit) % 2 == 0)
                 else:
                     is_split_same_suit = False
                     is_split_same_color = False
 
+                # Lastly, only add to n_movable if we are allowed to split
+                # runs (conditional line 1) or the move is not splitting a run
+                # (remaining lines of conditional).
+                #--------------------------------------------------------------
                 if (snm_opts.split_runs
                         or (snm_opts.move_same_suit
                             and not is_split_same_suit)
                         or (not snm_opts.move_same_suit
                             and not is_split_same_color)):
+                    # 20240413 - add check in foundation when move_same_suit
+                    #---------------------------------------------------------
+                    # But... we should also never split between the same suit
+                    # in sequence when the stock is 0 and split_empty_stock is
+                    # false: (1) when we are moving by suit, we forbid the
+                    # split as long as we can be sure we won't need to move
+                    # the other suit onto the pile; (2) when moving by color,
+                    # never need to split runs
+                    #----------------------------------------------------------
                     if (self.n_stock_left == 0
                             and not snm_opts.split_empty_stock
-                            and is_split_same_suit):
+                            and ((not snm_opts.move_same_suit
+                                    and is_split_same_suit))):
                         continue
                     self.piles[pile_index].n_movable.append(card_index + 1)
 
     def undo_deal_for_pile(self, pile_index: int) -> None:
         """Undo deal of one card for pile identified by pile_index.
 
         Set `in_suit_seq` and `last_in_pile` = False for the card being
@@ -1511,78 +1625,73 @@
                         if (king_found[k]
                                     and (current_card.rank < 12
                                          or current_card.suit != k)):
                             graph[k].add(current_card.suit)
         return _cyclic(graph)
 
     # Set self.validmoves with the three types of moves
-    # TODO: update docstring description
     def set_valid_moves(self, enum_to_empty_pile: EmptyRule,
                         move_same_suit: bool, split_empty_stock: bool,
                         track_threshold: int,
                         last_move_info: list[LastMoveInfo]) -> None:
         """Set self.valid_moves to the valid moves available.
 
         Three types: DealMove()
                      TablMove(from_=, to_=, n_cards=, expose=, tabltype=)
                      MoveToFound(from_=, suit=, expose=, tabltype=)
 
-        The `n_movable` attribute in a pile contains a list of the number
-        of cards in a pile that can be moved (based on the `move_same_suit`
-        and `split_runs` parameters when the `Agnes` object was created.
-        It also takes into account the optimization that there is no
-        benefit to splitting a sequence between two cards of the same
-        suit when the stock is empty, unless the empty rule is 'any 1' or
-        'high 1'.
-
         This function creates a list of all valid moves that can be done
         by seeing if a deal is available, which cards can be moved to which
         target piles, and which cards can be moved to the foundation.
 
         Various optimizations reduce the moves available. Forcing a move
-        means this is the only move that can be played. (If multiple moves
-        meet the forcing criteria, the last forced is used.)
-
-        (1) If n_stock_left == 2 and if track_threshold > 2, do not allow
-        the deal if there was a move between two piles that won't be covered
-        by the final deal. (Purpose is to reduce the search tree by forcing
-        these moves to occur after the final deal. This is only done when
-        track_threshold > 2 because otherwise we need to store the
-        information from LastMoveInfo in the `Agnes.losing_states` set.
+        means this is the only move that can be played. Forced moves are
+        designed to reduce the space of moves that need to be searched
+        without changing the final score of the game. If more than one
+        move meets the criteria to be forced, the last move is chosen.
 
-        (2) If there are multiple empty piles that won't be covered by
+        (1) If there are multiple empty piles that won't be covered by
         a future deal, only allow moves to the first pile.
 
-        (3) If we are not using the `losing_states` set (track_threshold >
+        (2) If we are not using the `losing_states` set (track_threshold >
         `n_stock_left`), do not reverse a move (ie, move the same number
         of cards from one pile to another).
 
-        (4) Force joins by suit sequence when the stock is empty and
+        (3) Force joins by suit sequence when the stock is empty and
         `split_empty_stock is False` if the same-color top card of the
         pile being moved satisfies (i) next lowest card is already in
         the foundation or (ii) `move_same_suit = False` and already under
         the next-highest card of the same suit or (iii)
-        `move_same_suit = False` and next-highest card is available to be
-        played on. For example, suppose we have a run starting with 4C
-        that we might put under 5C. This move is forced if (i) 3S in
-        foundation, (ii) `move_same_suit = False` and 4S already under 5S,
-        or (iii) `move_same_suit = False` and 5S is last in pile.
-
-        (5) Force move to foundation if (a) rank <= (highest rank in
-        foundation of same-color suit + 2) or (b) stock is empty and
-        `split_empty_stock = False` and next lowest rank of the same
-        color is already under in sequence under the same suit.
-
-        (6) Additional restriction on splitting same suit besides those
-        implied by `split_runs` (which were implemented in set_n_movable).
-        Only allow splits of same suit if source or target will be covered
-        by future deal, or split_empty_stock=true or Card(src_card.rank,
-        same_color_suit(src_card)) is not in the foundation, where src_card
-        is the highest-rank card in the part of the pile that is being
-        moved.
+        `move_same_suit = False` and next-highest card will be available
+        to be played on after the move (last_in_pile or will be the new
+        last card after the move from the current pile). For example,
+        suppose we have a run starting with 4C that we might put under 5C.
+        This move is forced if (i) 3S in foundation, or
+        (ii) `move_same_suit = False` and 4S already under 5S, or
+        (iii) `move_same_suit = False` and 5S is last in pile or we are
+        moving the 4C from under the 5S.
+
+        (4) Force move to foundation if (a) Card(rank - 2, same_color_suit)
+        is already in the foundation or (b) stock is empty and
+        `split_empty_stock = False` and Card(rank - 1, same_color_suit)
+        is already under Card(rank, same_color_suit).
+
+        (5) Force the last deal if the two dealt cards can immediately be
+        forced to the foundation.
+
+        (6) There are additional restrictions when the stock is empty for
+        when a run can be split between two cards of the same suit, even
+        when `split_runs=True`. When `move_same_suit is False`, the split
+        is never allowed (enforced in the `set_n_movable` function). Otherwise,
+        the split is allowed only if the last card in the pile being moved
+        will never need to have the same-color suit added, which means
+        Card(rank - 1, same_color_suit) is in the foundation or can be forced
+        to the foundation [Card(rank - 2, same_color_suit in foundation), and
+        Card(rank - 3, suit) in foundation] (where all ranks and suits refer to
+        the last card of the pile being moved).
 
         Parameters
         ----------
         enum_to_empty_pile : EmptyRule
             `Agnes.move_to_empty_pile` parameter converted to enum.
         move_same_suit : bool
             `Agnes.move_same_suit` parameter
@@ -1602,38 +1711,47 @@
 
         # Deal (DealMove dataclass)
         if (self.n_stock_left > 2
                 or (self.n_stock_left == 2
                     and (track_threshold <= 2
                         or not _dont_deal_last(last_move_info)))):
             self.valid_moves.append(DealMove())
+            if self.is_deal_forced():
+                force_move = DealMove()
 
         for pile_index, pile in enumerate(self.piles):
             exp_pile = pile.exposed
+            len_exp_pile = len(pile.exposed)
+            if len_exp_pile == 0: continue
+            last_card = exp_pile[-1]
             tabltype: TablType = TablType.NONE
             # Moves in tableau (TablMove dataclass)
             #
             # Get a list of the number of cards that are movable
             # according to the input parameters. This does not yet consider
             # if there is a location the cards can be moved to.
             #n_movable = self.set_n_movable(pile_index, move_same_suit,
             #                                split_same_suit_runs)
 
             for n_to_move in pile.n_movable:
                 tabltype = TablType.NONE
+                src_in_next_suit_seq = False   # 20240413: add
                 # 'Source' card: the one we want to move
                 src_card = exp_pile[-n_to_move]
-                if n_to_move == len(exp_pile):
+                if n_to_move == len_exp_pile:
                     expose = bool(pile.hidden)
                 else:
                     expose = False
                     card_above = exp_pile[-n_to_move - 1]
                     if (src_card.rank + 1 == card_above.rank
                             and src_card.suit == card_above.suit):
                         tabltype = TablType.SPLIT
+                    if (src_card.rank + 1 == card_above.rank
+                            and (src_card.suit + 2) % 4 == card_above.suit):
+                        src_in_next_suit_seq = True   # 20240413: add
 
                 # 'target' pile is the pile we are trying to move to
                 found_empty_target = False
                 for target_index in range(0,7):
                     if (target_index == pile_index
                         or (not self.piles[target_index].exposed
                             and found_empty_target)
@@ -1648,93 +1766,99 @@
 
                     if self.piles[target_index].exposed:
                         target_card = self.piles[target_index].exposed[-1]
                     elif target_index >= self.n_stock_left:
                         found_empty_target = True
 
                     if not self.piles[target_index].exposed:
-                        if (( n_to_move != len(exp_pile)
-                            or (n_to_move == len(exp_pile)
+                        if (( n_to_move != len_exp_pile
+                            or (n_to_move == len_exp_pile
                                  and (target_index < self.n_stock_left
                                        or pile_index < self.n_stock_left)))
                             and
                                (((enum_to_empty_pile == EmptyRule.ANY1 or
                              (enum_to_empty_pile == EmptyRule.HIGH1
                               and src_card.rank == 12)) and n_to_move == 1) or
                              ((enum_to_empty_pile == EmptyRule.ANYRUN or
                              (enum_to_empty_pile == EmptyRule.HIGHRUN
                               and src_card.rank == 12))))):
-                            if (pile_index < self.n_stock_left
-                                or target_index < self.n_stock_left
+                            if (self.n_stock_left > 0
                                 or tabltype != TablType.SPLIT
                                 or split_empty_stock
-                                or self.foundation[
-                                   ((src_card.suit + 2) % 4)] < src_card.rank):
+                                or not (self.in_foundation(last_card.rank - 1,
+                                                 (last_card.suit + 2) % 4)
+                                or (self.in_foundation(last_card.rank - 2,
+                                                 (last_card.suit + 2) % 4)
+                                    and self.in_foundation(last_card.rank - 3,
+                                                  last_card.suit)))):
                                 self.valid_moves.append(TablMove(
                                     from_=pile_index, n_cards=n_to_move,
                                     to_=target_index, expose=expose,
                                     tabltype=tabltype))
                     elif (self.piles[target_index].exposed
                             and src_card.rank == target_card.rank - 1
-                            and ((src_card.suit
-                                  - target_card.suit) % 2 == 0)):
+                            and (src_card.suit % 2 == target_card.suit % 2)):
                         if src_card.suit == target_card.suit:
                             tabltype = TablType.JOIN
 
-                        if (pile_index < self.n_stock_left
-                            or target_index < self.n_stock_left
+                        if (self.n_stock_left > 0
                             or tabltype != TablType.SPLIT
                             or split_empty_stock
-                            or self.foundation[
-                               ((src_card.suit + 2) % 4)] < src_card.rank):
+                            or not (self.in_foundation(last_card.rank - 1,
+                                                 (last_card.suit + 2) % 4)
+                            or (self.in_foundation(last_card.rank - 2,
+                                                 (last_card.suit + 2) % 4)
+                                and self.in_foundation(last_card.rank - 3,
+                                                  last_card.suit)))):
                             self.valid_moves.append(TablMove(
                                 from_=pile_index, n_cards=n_to_move,
                                 to_=target_index, expose=expose,
                                 tabltype=tabltype))
+
+                        # 20240413: add src_in_next_suit_seq to condition
                         if (not self.n_stock_left
                             and not split_empty_stock
                             and target_card.suit == src_card.suit
-                            and ((self.foundation[(src_card.suit+2)%4] + 1
-                                >= src_card.rank)
+                            and (self.in_foundation(src_card.rank,
+                                                   (src_card.suit+2) % 4)
                                 or (not move_same_suit
                                     and (self.in_suit_seq[src_card.rank][
       (src_card.suit + 2) % 4]
                                          or (src_card.rank < 12
-                                             and self.last_in_pile[
-      src_card.rank+1][(src_card.suit + 2) % 4]))))):
+                                             and (self.last_in_pile[
+      src_card.rank+1][(src_card.suit + 2) % 4])
+        or src_in_next_suit_seq))))):
                             force_move = TablMove(
                                 from_=pile_index, n_cards=n_to_move,
                                 to_=target_index, expose=expose,
                                 tabltype=tabltype)
 
-            if exp_pile:
-                # Move card to foundation (MoveToFound dataclass)
-                last_card = exp_pile[-1]
-                expose = bool(len(exp_pile) == 1 and pile.hidden)
-                if (last_card.rank - 1 == self.foundation[last_card.suit]
-                    and (track_threshold <= self.n_stock_left
-                        or not last_move_info[pile_index].depth
-                        or last_move_info[pile_index].can_move_to_found)):
-                    if self.in_suit_seq[last_card.rank][last_card.suit]:
-                        tabltype = TablType.SPLIT
-                    else:
-                        tabltype = TablType.NONE
-                    self.valid_moves.append(MoveToFound(from_=pile_index,
-                            suit=last_card.suit, expose = expose,
-                            tabltype=tabltype))
-                    same_color_suit = (last_card.suit + 2) % 4
-
-                    # See discussion in docstring about forcing moves
-                    if (last_card.rank <= self.foundation[same_color_suit] + 2
-                        or (self.n_stock_left == 0 and not split_empty_stock
-                            and self.in_suit_seq[last_card.rank - 1][
-                                same_color_suit])):
-                        force_move = MoveToFound(from_=pile_index,
-                                suit=last_card.suit, expose=expose,
-                                tabltype=tabltype)
+            # Move card to foundation (MoveToFound dataclass)
+            expose = bool(len_exp_pile == 1 and pile.hidden)
+            if (last_card.rank - 1 == self.foundation[last_card.suit]
+                and (track_threshold <= self.n_stock_left
+                    or not last_move_info[pile_index].depth
+                    or last_move_info[pile_index].can_move_to_found)):
+                if self.in_suit_seq[last_card.rank][last_card.suit]:
+                    tabltype = TablType.SPLIT
+                else:
+                    tabltype = TablType.NONE
+                self.valid_moves.append(MoveToFound(from_=pile_index,
+                        suit=last_card.suit, expose = expose,
+                        tabltype=tabltype))
+                same_color_suit = (last_card.suit + 2) % 4
+
+                # See discussion in docstring about forcing moves
+                if (self.in_foundation(last_card.rank - 2, same_color_suit)
+                    or (self.n_stock_left == 0 and not split_empty_stock
+                        and self.in_suit_seq[last_card.rank - 1][
+                            same_color_suit])):
+                    force_move = MoveToFound(from_=pile_index,
+                            suit=last_card.suit, expose=expose,
+                            tabltype=tabltype)
 
         if force_move:
             self.valid_moves.clear()
             self.valid_moves.append(force_move)
 
     def play_base_card(self, base_card: Card) -> None:
         """Play the base card into the foundation.
@@ -1747,7 +1871,138 @@
         -------
         None
         """
         self.foundation[base_card.suit] = 0
         self.last_in_pile[0][base_card.suit] = True
         self.in_suit_seq[0][base_card.suit] = True
         self.n_stock_left = self.n_stock_left - 1
+
+    # TODO: probably should be moved to constructor
+    def set_last_cards(self, deck: list[Card]) -> None:
+        """Set information about last cards in deck for use by is_deal_blocked.
+
+        This isn't used to deal, so we don't store which card is actually the
+        last, we only store their values and which is lower and two indicator
+        variables.
+        """
+        if deck[-1].rank < deck[-2].rank:
+            self.lower_last = deck[-1]
+            self.upper_last = deck[-2]
+        else:
+            self.lower_last = deck[-2]
+            self.upper_last = deck[-1]
+
+        card1 = self.lower_last
+        card2 = self.upper_last
+
+        self.last_same_suit_seq = (card1.suit == card2.suit
+             and card1.rank + 1 == card2.rank)
+        self.last_same_color_not_suit = card1.suit ==(card2.suit + 2) % 4
+
+    def is_deal_forced(self) -> bool:
+        """Check if deal can be forced (if cards can be forced to foundation).
+
+        Generally, a card can be forced to the foundation if (1) the card
+        below it is already in the foundation, and
+        (2a) Card(rank - 2, same_color_suit) is already in the foundation, or
+        (2b) Card(rank - 1, same_color_suit) is in sequence under a card of
+        the same suit and split_empty_stock is False.
+
+        Here we consider only (1)+(2a), as the correctness is easier to
+        discern and the effect of (1)+(2b) is negligible.
+
+        This code also handles the case where the two last cards might be
+        the same color but different suits (in which case putting the first
+        card into the foundation will increase the threshold at which the
+        second card would be forced into the foundation).
+
+        Returns
+        -------
+        Boolean indicating whether the deal should be forced.
+        """
+        card1 = self.lower_last
+        card2 = self.upper_last
+        if self.n_stock_left != 2:
+            return False
+        else:
+            can_put1 = False
+            can_put2 = False
+            if self.last_same_suit_seq:
+                can_put1 = self.in_foundation(card1.rank - 1, card1.suit)
+                can_put2 = can_put1
+            else:
+                can_put1 = self.in_foundation(card1.rank - 1, card1.suit)
+                can_put2 = self.in_foundation(card2.rank - 1, card2.suit)
+
+            card1_forcable = (can_put1
+                and (self.in_foundation(card1.rank - 2, (card1.suit + 2) % 4)))
+            card2_forcable = (can_put2
+                and (self.in_foundation(card2.rank - 2, (card2.suit + 2) % 4)))
+
+            # TODO: maybe can get rid of one of the if branches since
+            # card1.rank <= card2.rank
+            if card1_forcable and card2_forcable:
+                return True
+            elif (not self.last_same_color_not_suit
+                    or (not card1_forcable and not card2_forcable)):
+                return False
+            elif (card1_forcable and can_put2
+                    and self.in_foundation(card2.rank - 3, card1.suit)):
+                return True
+            elif (card2_forcable and can_put1
+                    and self.in_foundation(card1.rank - 3, card2.suit)):
+                return True
+            else:
+                return False
+
+    def set_sort_order(self, move_to_empty_pile: EmptyRule) -> None:
+        """Set sort_order.
+
+        Update the sort_order using pile_sort_key as the key.
+        """
+        # TODO: could move this out to perform_move and undo_move
+        for pile_index in range(0, 7):
+            self.sort_order[pile_index] = pile_index
+
+        if self.n_stock_left > 2:
+            #print(self.sort_order)
+            #print(self.hash_str)
+            return
+        elif move_to_empty_pile != EmptyRule.NONE:
+            self.sort_order.sort(key = lambda x: pile_sort_key(
+                    self.pile_sort_info[x]))
+            #self.sort_order = sorted(self.sort_order,
+            #    key=lambda x: pile_sort_key(self.pile_sort_info[x]))
+        #print(self.sort_order)
+        #print(self.hash_str)
+
+    def in_foundation(self, rank: int, suit: int) -> bool:
+        return self.foundation[suit] >= rank
+
+def pile_sort_key(pile_sort_info: PileSortInfo) -> int:
+    """Sort piles for losing states set.
+
+    If n_stock_left = 2, the first two piles will be covered by the last deal,
+    so they are not equivalent to each other or the other two and are always
+    sorted first by their index. Otherwise, sort empty piles before non-empty
+    and if non-empty, sort by card value.
+
+    Returns
+    -------
+    Integer taking values:
+       (0-1) if n_stock_left = 2 and pile_index <= 1,
+       (2-9) calculated as pile_index+2 if the pile is empty
+       (10-62) calculated as Card(value) + 10 otherwise, where the card is the
+             top card in the pile (index=0)
+    """
+    if pile_sort_info.n_stock_left == 2 and pile_sort_info.pile_index <= 1:
+        retval = pile_sort_info.pile_index
+    elif pile_sort_info.pile.hidden:
+        retval = (pile_sort_info.pile.hidden[0].rank*4
+                 + pile_sort_info.pile.hidden[0].suit + 10)
+    elif pile_sort_info.pile.exposed:
+        retval = (pile_sort_info.pile.exposed[0].rank*4
+                 + pile_sort_info.pile.exposed[0].suit + 10)
+    else:
+        retval = pile_sort_info.pile_index + 2
+    return retval
+
```

### Comparing `quagnes-1.0.0/src/quagnes.egg-info/PKG-INFO` & `quagnes-1.1.0/src/quagnes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quagnes
-Version: 1.0.0
+Version: 1.1.0
 Summary: This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates.
 Author-email: Ray Griner <rgriner_fwd@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -725,68 +725,47 @@
     #if rc==1:
     #    f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
     #    fwrite(new_game.print_history())
     #    f.close()
 ```
 
 # Release Notes
-## Version 1.0.0
-- Change name of `split_same_suit_runs` parameter to `split_runs` and make
-  parameter applicable regardless of the value of `move_same_suit`.
-- Add optimization for use when the losing state set is disabled.
-Track for each pile the last move depth, the number of cards
-moved, whether the pile was moved from or to, and whether the bottom card
-in the moved pile could be played to the foundation at the time of the move.
-Do not allow moves that: (a) reverse a previous tableau move without an
-intervening move to foundation or deal; (b) make the last deal after a
-tableau move where neither pile is dealt to and neither file had a card
-played to foundation; (c) play the bottom card of the moved pile to the
-foundation after the tableau move if it could have been played at the time
-of the move (and there has been no subsequent move to the pile or deal
-onto the pile).  These optimizations are only employed when the losing
-states set is
-disabled, as they use information not stored in the losing states set to
-determine whether a move can be played.
-- Add optimization when moves to empty piles allow zero or multiple cards
-to reduce the space of moves to consider when the stock is empty or near
-empty (without
-changing the win possibility or maximum score that can be attained). In
-these rules, we use the term 'top card' to describe the highest-rank card
-in the pile being moved and 'same-color top card' to be the card with equal
-rank in the same-color suit. The rules are: (a) when moving runs by suit,
-never split a run between same-suit cards when the stock is empty;
-(b) never split a run between same-suit cards when neither pile can be
-covered by a future deal and the same-color top card is in the foundation;
-(c) when the stock is empty, force a move onto a card of the same suit
-where possible when we know the target pile cannot be needed to move the
-same-color top card (ie, the same-color top card is already in the
-foundation or in same-suit sequence or the card one rank higher than the
-same-color top card is already exposed at the bottom of a pile); (d) when
-the stock is empty, force a move to the foundation if the card being
-moved cannot be needed as a target to be moved onto (ie, if the card in the
-same-color suit that is one rank lower is already in the foundation or in
-same-suit sequence).
-- Add new attributes created for these two optimizations in `_AgnesState` class (`in_suit_seq`, `last_in_pile`,
-  `_all_lmi`) and to output printed when state is printed.
-- Add `_AgnesState.hash_str` attribute to store the string representing
-  the hash of the object that will be stored in the losing states and
-  check loop set. Add `_Agnes_state.update_hash_str()` function called
-  after move is performed or undone to save the string in `hash_str`.
-  Previously, the `hash_str` was recalculated multiple times.
-- Fix bug in `Agnes.print_history` as only half the history was being
-  printed.
-- Use a single set to track whether loop has occured rather than a stack of
-  sets. Save result of check whether state is in the losing states set
-  so that we do not inefficiently (re-)insert the state into the losing
-  states set. Add attributes `is_loop` and `is_loser` to `_AgnesState`
-  class to support this logic.
-- Created for C++ implementation. Move detailed information
-  on the background, game rules, program methodology, and analysis of
-  win rates to that repository from this README. Add win rates
-  for rule variants where the empty rule is *AnyRun* or *HighRun*.
+## Version 1.1.0
+### Fixes Affecting Simultation Results
+- No longer forbid splitting of runs between same-suit cards when the stock
+has two cards left, even when neither the source nor target pile can be
+covered by a future deal. This optimization is incorrect, ie, it could
+force some winning games to be reported as losses.
+- Previously, splitting runs between cards of the same suit was not allowed
+when the stock was empty when runs are moved by suit. Add the condition that
+`Card(rank=last_card.rank - 1, suit=last_card.same_color_suit)` must also be
+in the foundation or meet the criteria for being forced to the foundation
+when it appears (for such splits to be forbidden), where `last_card` is the
+last card in the run moved. The additional condition is because placing the
+same-color suit at the bottom of the pile makes the pile unmovable, and so
+it would matter whether or not the split was performed. So we only forbid
+splits when this cannot be the case.
+
+### Fixes Improving Run-Time
+- When checking whether a card is the last in the pile (which is used to
+determine whether a tableau move should be forced), we previously failed to
+consider the card that would become last in a pile after the move. These
+cards are now considered.
+- Add optimization to force the last deal if the two dealt cards will
+immediately be forced to the foundation if `Card(rank - 2, same_color_suit)`
+is already in the foundation. Attributes were added to the `_AgnesState`
+class to store the last and second to last card, whether they are of the
+same suit in-sequence, and whether they are the same color, but not the
+same suit.
+- Add optimization to sort the tableau piles that can no longer be covered
+by a deal before storing in or checking against the losing states set. The
+piles are sorted by their top card.
+
+### Other Changes
+- Add `in_foundation` function to `_AgnesState` class.
 
 # External Documentation
 A C++ implementation written by this package author also exists in a git
 repository.  Detailed information on the background, game rules, program
 methodology, and analysis of win rates are available [there](https://github.com/ghrgriner/quagnes-cpp/wiki/Rules,-Methodology,-and-Analysis-of-Win-Rates).
 
 # Using the Package
@@ -874,9 +853,9 @@
 [2] Dalton W (1909). "My favourite Patiences" in The Strand Magazine,
     Vol 38.
 
 [3] Parlett D (1979). The Penguin Book of Patience. London: Penguin.
 
 # Disclosures
 We are not affiliated with any of the books, websites, or applications
-discussed in this documentation, except of course for this Python package
-and previously-mentioned C++ implementation which we wrote.
+discussed in this documentation, except for this Python package and
+previously-mentioned C++ implementation which we wrote.
```

